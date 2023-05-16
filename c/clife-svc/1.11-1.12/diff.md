# Comparing `tmp/clife_svc-1.11.tar.gz` & `tmp/clife_svc-1.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clife_svc-1.11.tar", last modified: Thu Apr 27 10:56:05 2023, max compression
+gzip compressed data, was "clife_svc-1.12.tar", last modified: Tue May 16 02:54:47 2023, max compression
```

## Comparing `clife_svc-1.11.tar` & `clife_svc-1.12.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 10:56:05.931491 clife_svc-1.11/
--rw-rw-rw-   0        0        0      420 2023-04-27 10:56:05.930494 clife_svc-1.11/PKG-INFO
--rw-rw-rw-   0        0        0       12 2021-12-20 11:08:06.000000 clife_svc-1.11/README.md
-drwxrwxrwx   0        0        0        0 2023-04-27 10:56:05.799795 clife_svc-1.11/clife_svc/
--rw-rw-rw-   0        0        0        2 2021-12-20 11:08:06.000000 clife_svc-1.11/clife_svc/__init__.py
--rw-rw-rw-   0        0        0    12238 2023-04-27 10:53:11.000000 clife_svc-1.11/clife_svc/application.py
-drwxrwxrwx   0        0        0        0 2023-04-27 10:56:05.840733 clife_svc-1.11/clife_svc/config/
--rw-rw-rw-   0        0        0        0 2023-01-13 06:18:27.000000 clife_svc-1.11/clife_svc/config/__init__.py
--rw-rw-rw-   0        0        0     2078 2023-01-13 06:38:28.000000 clife_svc-1.11/clife_svc/config/configmap.py
--rw-rw-rw-   0        0        0     5582 2023-04-27 09:54:37.000000 clife_svc-1.11/clife_svc/config/disconf.py
-drwxrwxrwx   0        0        0        0 2023-04-27 10:56:05.866664 clife_svc-1.11/clife_svc/errors/
--rw-rw-rw-   0        0        0        2 2021-12-20 11:08:06.000000 clife_svc-1.11/clife_svc/errors/__init__.py
--rw-rw-rw-   0        0        0     3589 2022-09-01 09:09:26.000000 clife_svc-1.11/clife_svc/errors/error_code.py
-drwxrwxrwx   0        0        0        0 2023-04-27 10:56:05.928499 clife_svc-1.11/clife_svc/libs/
--rw-rw-rw-   0        0        0        2 2021-12-20 11:08:06.000000 clife_svc-1.11/clife_svc/libs/__init__.py
--rw-rw-rw-   0        0        0      284 2021-12-23 09:51:21.000000 clife_svc-1.11/clife_svc/libs/context.py
--rw-rw-rw-   0        0        0    14254 2023-01-31 09:11:49.000000 clife_svc-1.11/clife_svc/libs/http_request.py
--rw-rw-rw-   0        0        0     2649 2023-04-27 10:46:36.000000 clife_svc-1.11/clife_svc/libs/log.py
--rw-rw-rw-   0        0        0     3461 2023-01-13 06:23:00.000000 clife_svc-1.11/clife_svc/libs/mq_handler.py
--rw-rw-rw-   0        0        0     1282 2023-01-13 07:00:07.000000 clife_svc-1.11/clife_svc/libs/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-27 10:56:05.808770 clife_svc-1.11/clife_svc.egg-info/
--rw-rw-rw-   0        0        0      420 2023-04-27 10:56:05.000000 clife_svc-1.11/clife_svc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      535 2023-04-27 10:56:05.000000 clife_svc-1.11/clife_svc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 10:56:05.000000 clife_svc-1.11/clife_svc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       92 2023-04-27 10:56:05.000000 clife_svc-1.11/clife_svc.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-27 10:56:05.000000 clife_svc-1.11/clife_svc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-27 10:56:05.931491 clife_svc-1.11/setup.cfg
--rw-rw-rw-   0        0        0     1219 2023-04-27 10:54:10.000000 clife_svc-1.11/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 02:54:47.636510 clife_svc-1.12/
+-rw-rw-rw-   0        0        0      420 2023-05-16 02:54:47.635459 clife_svc-1.12/PKG-INFO
+-rw-rw-rw-   0        0        0       12 2021-12-20 11:08:06.000000 clife_svc-1.12/README.md
+drwxrwxrwx   0        0        0        0 2023-05-16 02:54:47.555934 clife_svc-1.12/clife_svc/
+-rw-rw-rw-   0        0        0        2 2021-12-20 11:08:06.000000 clife_svc-1.12/clife_svc/__init__.py
+-rw-rw-rw-   0        0        0    12238 2023-04-27 10:53:11.000000 clife_svc-1.12/clife_svc/application.py
+drwxrwxrwx   0        0        0        0 2023-05-16 02:54:47.580068 clife_svc-1.12/clife_svc/config/
+-rw-rw-rw-   0        0        0        0 2023-01-13 06:18:27.000000 clife_svc-1.12/clife_svc/config/__init__.py
+-rw-rw-rw-   0        0        0     2078 2023-01-13 06:38:28.000000 clife_svc-1.12/clife_svc/config/configmap.py
+-rw-rw-rw-   0        0        0     5582 2023-04-27 09:54:37.000000 clife_svc-1.12/clife_svc/config/disconf.py
+drwxrwxrwx   0        0        0        0 2023-05-16 02:54:47.596253 clife_svc-1.12/clife_svc/errors/
+-rw-rw-rw-   0        0        0        2 2021-12-20 11:08:06.000000 clife_svc-1.12/clife_svc/errors/__init__.py
+-rw-rw-rw-   0        0        0     3589 2022-09-01 09:09:26.000000 clife_svc-1.12/clife_svc/errors/error_code.py
+drwxrwxrwx   0        0        0        0 2023-05-16 02:54:47.634456 clife_svc-1.12/clife_svc/libs/
+-rw-rw-rw-   0        0        0        2 2021-12-20 11:08:06.000000 clife_svc-1.12/clife_svc/libs/__init__.py
+-rw-rw-rw-   0        0        0      284 2021-12-23 09:51:21.000000 clife_svc-1.12/clife_svc/libs/context.py
+-rw-rw-rw-   0        0        0    14511 2023-05-15 11:07:39.000000 clife_svc-1.12/clife_svc/libs/http_request.py
+-rw-rw-rw-   0        0        0     2649 2023-05-15 11:06:18.000000 clife_svc-1.12/clife_svc/libs/log.py
+-rw-rw-rw-   0        0        0     3461 2023-01-13 06:23:00.000000 clife_svc-1.12/clife_svc/libs/mq_handler.py
+-rw-rw-rw-   0        0        0     1282 2023-01-13 07:00:07.000000 clife_svc-1.12/clife_svc/libs/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-16 02:54:47.564962 clife_svc-1.12/clife_svc.egg-info/
+-rw-rw-rw-   0        0        0      420 2023-05-16 02:54:47.000000 clife_svc-1.12/clife_svc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      535 2023-05-16 02:54:47.000000 clife_svc-1.12/clife_svc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 02:54:47.000000 clife_svc-1.12/clife_svc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       92 2023-05-16 02:54:47.000000 clife_svc-1.12/clife_svc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-16 02:54:47.000000 clife_svc-1.12/clife_svc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-16 02:54:47.636510 clife_svc-1.12/setup.cfg
+-rw-rw-rw-   0        0        0     1219 2023-05-16 02:54:25.000000 clife_svc-1.12/setup.py
```

### Comparing `clife_svc-1.11/clife_svc/application.py` & `clife_svc-1.12/clife_svc/application.py`

 * *Files identical despite different names*

### Comparing `clife_svc-1.11/clife_svc/config/configmap.py` & `clife_svc-1.12/clife_svc/config/configmap.py`

 * *Files identical despite different names*

### Comparing `clife_svc-1.11/clife_svc/config/disconf.py` & `clife_svc-1.12/clife_svc/config/disconf.py`

 * *Files identical despite different names*

### Comparing `clife_svc-1.11/clife_svc/errors/error_code.py` & `clife_svc-1.12/clife_svc/errors/error_code.py`

 * *Files identical despite different names*

### Comparing `clife_svc-1.11/clife_svc/libs/http_request.py` & `clife_svc-1.12/clife_svc/libs/http_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import time
 import random
 import string
 import asyncio
 
 import boto3
 import aiohttp
+import mimetypes
 from aiohttp.client_exceptions import ServerTimeoutError
 from qcloud_cos import CosConfig
 from qcloud_cos import CosS3Client
 
 from clife_svc.errors.error_code import ParameterException, UploadFileException, TimeoutException, DownloadFileException
 from clife_svc.libs.log import klogger, clogger
 
@@ -213,18 +214,22 @@
                             klogger.info('Upload file success: {}'.format(file_url))
                             return file_url
                     else:
                         klogger.warning('Error upload file,retry left: {}'.format(retry + 1))
                         continue
                 else:
                     key = cos_dir + '/' + file_name
+                    content_type, encoding = mimetypes.guess_type(key)
+                    content_type = content_type or 'application/octet-stream'
                     self._S3_CLIENT.upload_fileobj(
                         Fileobj=body,
                         Bucket=self.S3_BUCKET,
-                        Key=key)  # noqa
+                        Key=key,
+                        ExtraArgs={"ContentType": content_type}
+                    )  # noqa
 
                     file_url = self._S3_CLIENT.generate_presigned_url('get_object',
                                                                       Params={'Bucket': self.S3_BUCKET,
                                                                               'Key': key},
                                                                       ExpiresIn=600)
                     file_url = file_url if self.S3_BUCKET_PRIVATE else file_url.split('?')[0]
                     klogger.info('Upload file cost: {}s'.format(round(time.time() - start, 2)))
```

### Comparing `clife_svc-1.11/clife_svc/libs/log.py` & `clife_svc-1.12/clife_svc/libs/log.py`

 * *Files identical despite different names*

### Comparing `clife_svc-1.11/clife_svc/libs/mq_handler.py` & `clife_svc-1.12/clife_svc/libs/mq_handler.py`

 * *Files identical despite different names*

### Comparing `clife_svc-1.11/clife_svc/libs/utils.py` & `clife_svc-1.12/clife_svc/libs/utils.py`

 * *Files identical despite different names*

### Comparing `clife_svc-1.11/clife_svc.egg-info/SOURCES.txt` & `clife_svc-1.12/clife_svc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clife_svc-1.11/setup.py` & `clife_svc-1.12/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         if line.startswith('-e git+'):
             dependency_links.append(line.replace('-e ', ''))
         else:
             requirements.append(line)
 
 setuptools.setup(
     name='clife_svc',   # 需要打包的名字,即本模块要发布的名字
-    version='1.11',     # 版本
+    version='1.12',     # 版本
     author='andy.hu',  # 作者名
     author_email='hlp0@163.com',  # 作者邮件
     description='A module for service',   # 简要描述
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='',       # 项目地址,一般是代码托管的网站
     packages=setuptools.find_packages(),
```

