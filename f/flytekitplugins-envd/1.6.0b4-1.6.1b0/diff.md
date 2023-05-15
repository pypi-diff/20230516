# Comparing `tmp/flytekitplugins-envd-1.6.0b4.tar.gz` & `tmp/flytekitplugins-envd-1.6.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-envd-1.6.0b4.tar", last modified: Tue May  9 00:42:34 2023, max compression
+gzip compressed data, was "flytekitplugins-envd-1.6.1b0.tar", last modified: Mon May 15 22:07:04 2023, max compression
```

## Comparing `flytekitplugins-envd-1.6.0b4.tar` & `flytekitplugins-envd-1.6.1b0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:34.292762 flytekitplugins-envd-1.6.0b4/
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-09 00:42:34.292762 flytekitplugins-envd-1.6.0b4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-09 00:42:14.000000 flytekitplugins-envd-1.6.0b4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:34.288762 flytekitplugins-envd-1.6.0b4/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:34.288762 flytekitplugins-envd-1.6.0b4/flytekitplugins/envd/
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-09 00:42:14.000000 flytekitplugins-envd-1.6.0b4/flytekitplugins/envd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-05-09 00:42:14.000000 flytekitplugins-envd-1.6.0b4/flytekitplugins/envd/image_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:34.292762 flytekitplugins-envd-1.6.0b4/flytekitplugins_envd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-09 00:42:34.000000 flytekitplugins-envd-1.6.0b4/flytekitplugins_envd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-09 00:42:34.000000 flytekitplugins-envd-1.6.0b4/flytekitplugins_envd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 00:42:34.000000 flytekitplugins-envd-1.6.0b4/flytekitplugins_envd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-09 00:42:34.000000 flytekitplugins-envd-1.6.0b4/flytekitplugins_envd.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-09 00:42:34.000000 flytekitplugins-envd-1.6.0b4/flytekitplugins_envd.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-09 00:42:34.000000 flytekitplugins-envd-1.6.0b4/flytekitplugins_envd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-09 00:42:34.000000 flytekitplugins-envd-1.6.0b4/flytekitplugins_envd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 00:42:34.292762 flytekitplugins-envd-1.6.0b4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-05-09 00:42:30.000000 flytekitplugins-envd-1.6.0b4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:07:04.495821 flytekitplugins-envd-1.6.1b0/
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-15 22:07:04.495821 flytekitplugins-envd-1.6.1b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-15 22:06:44.000000 flytekitplugins-envd-1.6.1b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:07:04.495821 flytekitplugins-envd-1.6.1b0/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:07:04.495821 flytekitplugins-envd-1.6.1b0/flytekitplugins/envd/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-15 22:06:44.000000 flytekitplugins-envd-1.6.1b0/flytekitplugins/envd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-05-15 22:06:44.000000 flytekitplugins-envd-1.6.1b0/flytekitplugins/envd/image_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:07:04.495821 flytekitplugins-envd-1.6.1b0/flytekitplugins_envd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-15 22:07:04.000000 flytekitplugins-envd-1.6.1b0/flytekitplugins_envd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-15 22:07:04.000000 flytekitplugins-envd-1.6.1b0/flytekitplugins_envd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 22:07:04.000000 flytekitplugins-envd-1.6.1b0/flytekitplugins_envd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-15 22:07:04.000000 flytekitplugins-envd-1.6.1b0/flytekitplugins_envd.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-15 22:07:04.000000 flytekitplugins-envd-1.6.1b0/flytekitplugins_envd.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-15 22:07:04.000000 flytekitplugins-envd-1.6.1b0/flytekitplugins_envd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-15 22:07:04.000000 flytekitplugins-envd-1.6.1b0/flytekitplugins_envd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 22:07:04.495821 flytekitplugins-envd-1.6.1b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-05-15 22:07:00.000000 flytekitplugins-envd-1.6.1b0/setup.py
```

### Comparing `flytekitplugins-envd-1.6.0b4/PKG-INFO` & `flytekitplugins-envd-1.6.1b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-envd
-Version: 1.6.0b4
+Version: 1.6.1b0
 Summary: This package enables users to easily build a Docker image for tasks or workflows.
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-envd-1.6.0b4/README.md` & `flytekitplugins-envd-1.6.1b0/README.md`

 * *Files identical despite different names*

### Comparing `flytekitplugins-envd-1.6.0b4/flytekitplugins/envd/image_builder.py` & `flytekitplugins-envd-1.6.1b0/flytekitplugins/envd/image_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 class EnvdImageSpecBuilder(ImageSpecBuilder):
     """
     This class is used to build a docker image using envd.
     """
 
     def build_image(self, image_spec: ImageSpec):
         cfg_path = create_envd_config(image_spec)
-        command = f"envd build --path {pathlib.Path(cfg_path).parent}"
+        command = f"envd build --path {pathlib.Path(cfg_path).parent}  --platform {image_spec.platform}"
         if image_spec.registry:
             command += f" --output type=image,name={image_spec.image_name()},push=true"
         click.secho(f"Run command: {command} ", fg="blue")
         p = subprocess.Popen(command.split(), stdout=subprocess.PIPE, stderr=subprocess.PIPE)
         for line in iter(p.stdout.readline, ""):
             if p.poll() is not None:
                 break
```

### Comparing `flytekitplugins-envd-1.6.0b4/flytekitplugins_envd.egg-info/PKG-INFO` & `flytekitplugins-envd-1.6.1b0/flytekitplugins_envd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-envd
-Version: 1.6.0b4
+Version: 1.6.1b0
 Summary: This package enables users to easily build a Docker image for tasks or workflows.
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-envd-1.6.0b4/setup.py` & `flytekitplugins-envd-1.6.1b0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup
 
 PLUGIN_NAME = "envd"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
-plugin_requires = ["flytekit", "envd"]
+plugin_requires = ["flytekit", "envd>=0.3.22"]
 
-__version__ = "1.6.0b4"
+__version__ = "1.6.1b0"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="This package enables users to easily build a Docker image for tasks or workflows.",
```

