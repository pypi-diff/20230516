# Comparing `tmp/params_aws-0.1.0.tar.gz` & `tmp/params_aws-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "params_aws-0.1.0.tar", max compression
+gzip compressed data, was "params_aws-0.1.1.tar", max compression
```

## Comparing `params_aws-0.1.0.tar` & `params_aws-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0        0 2023-05-16 04:05:04.513569 params_aws-0.1.0/README.md
--rw-r--r--   0        0        0     1595 2023-05-14 19:22:54.171085 params_aws-0.1.0/params_aws/aws_params.py
--rw-r--r--   0        0        0     2123 2023-05-14 19:22:34.834692 params_aws-0.1.0/params_aws/aws_params_cli.py
--rw-r--r--   0        0        0      786 2023-05-14 19:22:28.266444 params_aws-0.1.0/params_aws/model.py
--rw-r--r--   0        0        0      394 2023-05-14 18:36:28.396068 params_aws-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      589 1970-01-01 00:00:00.000000 params_aws-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1280 2023-05-16 04:41:03.997534 params_aws-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-16 04:15:12.535753 params_aws-0.1.1/params_aws/__init__.py
+-rw-r--r--   0        0        0      786 2023-05-14 19:22:28.266444 params_aws-0.1.1/params_aws/model.py
+-rw-r--r--   0        0        0     1800 2023-05-16 04:39:42.320028 params_aws-0.1.1/params_aws/params_aws.py
+-rw-r--r--   0        0        0     2718 2023-05-16 04:38:44.003159 params_aws-0.1.1/params_aws/params_aws_cli.py
+-rw-r--r--   0        0        0      465 2023-05-16 04:39:50.882714 params_aws-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1869 1970-01-01 00:00:00.000000 params_aws-0.1.1/PKG-INFO
```

### Comparing `params_aws-0.1.0/params_aws/aws_params.py` & `params_aws-0.1.1/params_aws/params_aws.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,25 +8,30 @@
 from pydantic import BaseModel
 
 TTL = 12 * 60 * 60 
 MAXSIZE = 5000
 
 client = boto3.client('ssm')
 
-def _get_parameter_not_cached(name: str, modelType: type[BaseModel]) -> Optional[str]:
+def _get_parameter_value(name:str) -> Optional[str]:
     try:
         response = client.get_parameter(Name=name)
-        raw_parameter_value = response["Parameter"]["Value"]
-        return modelType.parse_raw(raw_parameter_value)
+        return response["Parameter"]["Value"]
     except botocore.exceptions.ClientError as e:
         if e.response['Error']['Code'] == 'ParameterNotFound':
             return None
         else:
             raise e
-        
+
+def _get_parameter_not_cached(name: str, modelType: type[BaseModel]) -> Optional[str]:
+    value = _get_parameter_value(name=name)
+    if value:
+        return modelType.parse_raw(value)
+    else:
+        return None
 
 @cached(cache=TTLCache(maxsize=MAXSIZE, ttl=TTL))
 def _get_parameter_cached(name: str, modelType: type[BaseModel]) -> Optional[str]:
     return _get_parameter_not_cached(name, modelType)
 
 
 def get_parameter_names() -> List[str]:
@@ -35,14 +40,17 @@
     return [parameter['Name'] for parameter in responses["Parameters"]]
 
 def get_parameter(name: str, modelType: type[BaseModel], cached=True) -> Optional[str]:
     if cached:
         return _get_parameter_cached(name, modelType)
     else: 
         return _get_parameter_not_cached(name, modelType)
+    
+def get_parameter_value(name: str) -> Optional[str]:
+    return _get_parameter_value(name=name)
 
 def put_parameter(name: str, modelType: type[BaseModel], value_str: str):
     # To validate
     modelType.parse_raw(value_str)
 
     client.put_parameter(
         Name=name,
```

### Comparing `params_aws-0.1.0/params_aws/aws_params_cli.py` & `params_aws-0.1.1/params_aws/params_aws_cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,51 @@
 import click
-import aws_params
-from model import DBConfig, GGAPIConfig, HashID
+from params_aws import params_aws
+from params_aws.model import DBConfig, GGAPIConfig, HashID
 import os
 import traceback
 from asyncio.log import logger
 import uuid
 import json
 
 DEFAULT_EDITOR = "/usr/bin/nano"
 KNOWN_TYPES = [DBConfig.__name__, GGAPIConfig.__name__, HashID.__name__]
 
 @click.group()
 def cli():
   pass
 
-@cli.command(help="Get secret value and display on screen")
+@cli.command(help="Get known types")
+def types():
+  for known_type in KNOWN_TYPES:
+    click.echo(known_type)
+
+@cli.command(help="Get all names at root path")
+def names():
+  names = params_aws.get_parameter_names()
+  for name in names:
+    click.echo(name)
+
+@cli.command(help="Get raw secret value")
 @click.argument('name', nargs=1)
-def get(name):
-  param_value = aws_params.get_parameter(name=name)
+def get_value(name):
+  click.echo(params_aws.get_parameter_value(name=name))
+
+
+@cli.command(help="Get secret value")
+@click.argument('name', nargs=1)
+@click.argument('model', nargs=1)
+def get(name, model):
+  if model not in KNOWN_TYPES:
+    click.echo(f"Unknown type: {model}")
+    exit(-1)
+
+  pd_class = globals()[model]
+
+  param_value = params_aws.get_parameter(name=name, modelType=pd_class)
 
   click.echo(param_value)
 
 def _open_file(path: str):
   import subprocess
   subprocess.run([DEFAULT_EDITOR, path], check=True)
 
@@ -31,15 +55,15 @@
 def put(name, model):
   if model not in KNOWN_TYPES:
     click.echo(f"Unknown type: {model}")
     exit(-1)
 
   pd_class = globals()[model]
   
-  param_obj = aws_params.get_parameter(name, pd_class, cached=False)
+  param_obj = params_aws.get_parameter(name, pd_class, cached=False)
   if not param_obj:
     param = pd_class.get_example()
   else:
     param = json.dumps(param_obj.dict(), indent=2)
 
   tmp_file = "/tmp/secret-" + uuid.uuid4().hex
 
@@ -67,15 +91,15 @@
       else:
         logger.warning("No content changed")
       valid_value = True
 
     if file_changed and valid_value:
       logger.info(f"Saving value for: {name}")
       with open(tmp_file, "r") as f:
-        aws_params.put_parameter(name=name, modelType=pd_class, value_str=f.read())
+        params_aws.put_parameter(name=name, modelType=pd_class, value_str=f.read())
 
   except Exception as e:
       logger.error(e)
   finally:
     if not os.path.exists(tmp_file):
       os.remove(tmp_file)
```

### Comparing `params_aws-0.1.0/params_aws/model.py` & `params_aws-0.1.1/params_aws/model.py`

 * *Files identical despite different names*

