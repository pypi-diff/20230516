# Comparing `tmp/ec2imgutils-9.0.3.tar.gz` & `tmp/ec2imgutils-9.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ec2imgutils-9.0.3.tar", last modified: Thu Sep 23 19:09:25 2021, max compression
+gzip compressed data, was "ec2imgutils-9.0.4.tar", last modified: Wed Nov  3 13:42:44 2021, max compression
```

## Comparing `ec2imgutils-9.0.3.tar` & `ec2imgutils-9.0.4.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 19:09:25.136481 ec2imgutils-9.0.3/
--rw-r--r--   0 runner    (1001) docker     (121)    35147 2021-09-23 19:09:10.000000 ec2imgutils-9.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      326 2021-09-23 19:09:10.000000 ec2imgutils-9.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1413 2021-09-23 19:09:10.000000 ec2imgutils-9.0.3/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     4871 2021-09-23 19:09:25.136481 ec2imgutils-9.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3799 2021-09-23 19:09:10.000000 ec2imgutils-9.0.3/README.md
--rwxr-xr-x   0 runner    (1001) docker     (121)     9954 2021-09-23 19:09:10.000000 ec2imgutils-9.0.3/ec2deprecateimg
--rwxr-xr-x   0 runner    (1001) docker     (121)     5515 2021-09-23 19:09:10.000000 ec2imgutils-9.0.3/ec2listimg
--rwxr-xr-x   0 runner    (1001) docker     (121)     7600 2021-09-23 19:09:10.000000 ec2imgutils-9.0.3/ec2publishimg
--rwxr-xr-x   0 runner    (1001) docker     (121)     6902 2021-09-23 19:09:10.000000 ec2imgutils-9.0.3/ec2removeimg
--rwxr-xr-x   0 runner    (1001) docker     (121)    23513 2021-09-23 19:09:10.000000 ec2imgutils-9.0.3/ec2uploadimg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 19:09:25.132481 ec2imgutils-9.0.3/lib/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 19:09:25.136481 ec2imgutils-9.0.3/lib/ec2imgutils/
--rw-r--r--   0 runner    (1001) docker     (121)        6 2021-09-23 19:09:10.000000 ec2imgutils-9.0.3/lib/ec2imgutils/VERSION
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-23 19:09:10.000000 ec2imgutils-9.0.3/lib/ec2imgutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12804 2021-09-23 19:09:10.000000 ec2imgutils-9.0.3/lib/ec2imgutils/ec2deprecateimg.py
--rw-r--r--   0 runner    (1001) docker     (121)     3528 2021-09-23 19:09:10.000000 ec2imgutils-9.0.3/lib/ec2imgutils/ec2imgutils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1116 2021-09-23 19:09:10.000000 ec2imgutils-9.0.3/lib/ec2imgutils/ec2imgutilsExceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     3820 2021-09-23 19:09:10.000000 ec2imgutils-9.0.3/lib/ec2imgutils/ec2listimg.py
--rw-r--r--   0 runner    (1001) docker     (121)     9960 2021-09-23 19:09:10.000000 ec2imgutils-9.0.3/lib/ec2imgutils/ec2publishimg.py
--rw-r--r--   0 runner    (1001) docker     (121)     7907 2021-09-23 19:09:10.000000 ec2imgutils-9.0.3/lib/ec2imgutils/ec2removeimg.py
--rw-r--r--   0 runner    (1001) docker     (121)     9656 2021-09-23 19:09:10.000000 ec2imgutils-9.0.3/lib/ec2imgutils/ec2setup.py
--rw-r--r--   0 runner    (1001) docker     (121)    44311 2021-09-23 19:09:10.000000 ec2imgutils-9.0.3/lib/ec2imgutils/ec2uploadimg.py
--rw-r--r--   0 runner    (1001) docker     (121)     9617 2021-09-23 19:09:10.000000 ec2imgutils-9.0.3/lib/ec2imgutils/ec2utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 19:09:25.136481 ec2imgutils-9.0.3/lib/ec2imgutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4871 2021-09-23 19:09:24.000000 ec2imgutils-9.0.3/lib/ec2imgutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      895 2021-09-23 19:09:25.000000 ec2imgutils-9.0.3/lib/ec2imgutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-23 19:09:24.000000 ec2imgutils-9.0.3/lib/ec2imgutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       71 2021-09-23 19:09:24.000000 ec2imgutils-9.0.3/lib/ec2imgutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2021-09-23 19:09:24.000000 ec2imgutils-9.0.3/lib/ec2imgutils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 19:09:25.132481 ec2imgutils-9.0.3/man/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 19:09:25.136481 ec2imgutils-9.0.3/man/man1/
--rw-r--r--   0 runner    (1001) docker     (121)     7704 2021-09-23 19:09:10.000000 ec2imgutils-9.0.3/man/man1/ec2deprecateimg.1
--rw-r--r--   0 runner    (1001) docker     (121)     3675 2021-09-23 19:09:10.000000 ec2imgutils-9.0.3/man/man1/ec2listimg.1
--rw-r--r--   0 runner    (1001) docker     (121)     4280 2021-09-23 19:09:10.000000 ec2imgutils-9.0.3/man/man1/ec2publishimg.1
--rw-r--r--   0 runner    (1001) docker     (121)     4065 2021-09-23 19:09:10.000000 ec2imgutils-9.0.3/man/man1/ec2removeimg.1
--rw-r--r--   0 runner    (1001) docker     (121)     8984 2021-09-23 19:09:10.000000 ec2imgutils-9.0.3/man/man1/ec2uploadimg.1
--rw-r--r--   0 runner    (1001) docker     (121)       47 2021-09-23 19:09:10.000000 ec2imgutils-9.0.3/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-09-23 19:09:10.000000 ec2imgutils-9.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      226 2021-09-23 19:09:25.136481 ec2imgutils-9.0.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     2881 2021-09-23 19:09:10.000000 ec2imgutils-9.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 19:09:25.136481 ec2imgutils-9.0.3/tests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 19:09:25.136481 ec2imgutils-9.0.3/tests/data/
--rw-r--r--   0 runner    (1001) docker     (121)      339 2021-09-23 19:09:10.000000 ec2imgutils-9.0.3/tests/data/complete.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      295 2021-09-23 19:09:10.000000 ec2imgutils-9.0.3/tests/data/invalid.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     7441 2021-09-23 19:09:10.000000 ec2imgutils-9.0.3/tests/test_ec2utilsutils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-03 13:42:44.822610 ec2imgutils-9.0.4/
+-rw-r--r--   0 runner    (1001) docker     (121)    35147 2021-11-03 13:42:33.000000 ec2imgutils-9.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      326 2021-11-03 13:42:33.000000 ec2imgutils-9.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1413 2021-11-03 13:42:33.000000 ec2imgutils-9.0.4/Makefile
+-rw-r--r--   0 runner    (1001) docker     (121)     4871 2021-11-03 13:42:44.822610 ec2imgutils-9.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3799 2021-11-03 13:42:33.000000 ec2imgutils-9.0.4/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (121)     9954 2021-11-03 13:42:33.000000 ec2imgutils-9.0.4/ec2deprecateimg
+-rwxr-xr-x   0 runner    (1001) docker     (121)     5515 2021-11-03 13:42:33.000000 ec2imgutils-9.0.4/ec2listimg
+-rwxr-xr-x   0 runner    (1001) docker     (121)     7600 2021-11-03 13:42:33.000000 ec2imgutils-9.0.4/ec2publishimg
+-rwxr-xr-x   0 runner    (1001) docker     (121)     6902 2021-11-03 13:42:33.000000 ec2imgutils-9.0.4/ec2removeimg
+-rwxr-xr-x   0 runner    (1001) docker     (121)    23513 2021-11-03 13:42:33.000000 ec2imgutils-9.0.4/ec2uploadimg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-03 13:42:44.814610 ec2imgutils-9.0.4/lib/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-03 13:42:44.818610 ec2imgutils-9.0.4/lib/ec2imgutils/
+-rw-r--r--   0 runner    (1001) docker     (121)        6 2021-11-03 13:42:33.000000 ec2imgutils-9.0.4/lib/ec2imgutils/VERSION
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-03 13:42:33.000000 ec2imgutils-9.0.4/lib/ec2imgutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12804 2021-11-03 13:42:33.000000 ec2imgutils-9.0.4/lib/ec2imgutils/ec2deprecateimg.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3528 2021-11-03 13:42:33.000000 ec2imgutils-9.0.4/lib/ec2imgutils/ec2imgutils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1116 2021-11-03 13:42:33.000000 ec2imgutils-9.0.4/lib/ec2imgutils/ec2imgutilsExceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3820 2021-11-03 13:42:33.000000 ec2imgutils-9.0.4/lib/ec2imgutils/ec2listimg.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9960 2021-11-03 13:42:33.000000 ec2imgutils-9.0.4/lib/ec2imgutils/ec2publishimg.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7907 2021-11-03 13:42:33.000000 ec2imgutils-9.0.4/lib/ec2imgutils/ec2removeimg.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9656 2021-11-03 13:42:33.000000 ec2imgutils-9.0.4/lib/ec2imgutils/ec2setup.py
+-rw-r--r--   0 runner    (1001) docker     (121)    44343 2021-11-03 13:42:33.000000 ec2imgutils-9.0.4/lib/ec2imgutils/ec2uploadimg.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9617 2021-11-03 13:42:33.000000 ec2imgutils-9.0.4/lib/ec2imgutils/ec2utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-03 13:42:44.822610 ec2imgutils-9.0.4/lib/ec2imgutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4871 2021-11-03 13:42:44.000000 ec2imgutils-9.0.4/lib/ec2imgutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      895 2021-11-03 13:42:44.000000 ec2imgutils-9.0.4/lib/ec2imgutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-03 13:42:44.000000 ec2imgutils-9.0.4/lib/ec2imgutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       71 2021-11-03 13:42:44.000000 ec2imgutils-9.0.4/lib/ec2imgutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       12 2021-11-03 13:42:44.000000 ec2imgutils-9.0.4/lib/ec2imgutils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-03 13:42:44.818610 ec2imgutils-9.0.4/man/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-03 13:42:44.822610 ec2imgutils-9.0.4/man/man1/
+-rw-r--r--   0 runner    (1001) docker     (121)     7704 2021-11-03 13:42:33.000000 ec2imgutils-9.0.4/man/man1/ec2deprecateimg.1
+-rw-r--r--   0 runner    (1001) docker     (121)     3675 2021-11-03 13:42:33.000000 ec2imgutils-9.0.4/man/man1/ec2listimg.1
+-rw-r--r--   0 runner    (1001) docker     (121)     4280 2021-11-03 13:42:33.000000 ec2imgutils-9.0.4/man/man1/ec2publishimg.1
+-rw-r--r--   0 runner    (1001) docker     (121)     4065 2021-11-03 13:42:33.000000 ec2imgutils-9.0.4/man/man1/ec2removeimg.1
+-rw-r--r--   0 runner    (1001) docker     (121)     8984 2021-11-03 13:42:33.000000 ec2imgutils-9.0.4/man/man1/ec2uploadimg.1
+-rw-r--r--   0 runner    (1001) docker     (121)       47 2021-11-03 13:42:33.000000 ec2imgutils-9.0.4/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-11-03 13:42:33.000000 ec2imgutils-9.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      226 2021-11-03 13:42:44.822610 ec2imgutils-9.0.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2881 2021-11-03 13:42:33.000000 ec2imgutils-9.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-03 13:42:44.822610 ec2imgutils-9.0.4/tests/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-03 13:42:44.822610 ec2imgutils-9.0.4/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (121)      339 2021-11-03 13:42:33.000000 ec2imgutils-9.0.4/tests/data/complete.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      295 2021-11-03 13:42:33.000000 ec2imgutils-9.0.4/tests/data/invalid.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     7441 2021-11-03 13:42:33.000000 ec2imgutils-9.0.4/tests/test_ec2utilsutils.py
```

### Comparing `ec2imgutils-9.0.3/LICENSE` & `ec2imgutils-9.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ec2imgutils-9.0.3/Makefile` & `ec2imgutils-9.0.4/Makefile`

 * *Files identical despite different names*

### Comparing `ec2imgutils-9.0.3/PKG-INFO` & `ec2imgutils-9.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ec2imgutils
-Version: 9.0.3
+Version: 9.0.4
 Summary: Command-line tools to manage images in AWS EC2
 Home-page: https://github.com/SUSE-Enceladus/ec2imgutils
 Author: SUSE Public Cloud Team
 Author-email: public-cloud-dev@susecloud.net
 License: GPLv3+
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ec2imgutils-9.0.3/README.md` & `ec2imgutils-9.0.4/README.md`

 * *Files identical despite different names*

### Comparing `ec2imgutils-9.0.3/ec2deprecateimg` & `ec2imgutils-9.0.4/ec2deprecateimg`

 * *Files identical despite different names*

### Comparing `ec2imgutils-9.0.3/ec2listimg` & `ec2imgutils-9.0.4/ec2listimg`

 * *Files identical despite different names*

### Comparing `ec2imgutils-9.0.3/ec2publishimg` & `ec2imgutils-9.0.4/ec2publishimg`

 * *Files identical despite different names*

### Comparing `ec2imgutils-9.0.3/ec2removeimg` & `ec2imgutils-9.0.4/ec2removeimg`

 * *Files identical despite different names*

### Comparing `ec2imgutils-9.0.3/ec2uploadimg` & `ec2imgutils-9.0.4/ec2uploadimg`

 * *Files identical despite different names*

### Comparing `ec2imgutils-9.0.3/lib/ec2imgutils/ec2deprecateimg.py` & `ec2imgutils-9.0.4/lib/ec2imgutils/ec2deprecateimg.py`

 * *Files identical despite different names*

### Comparing `ec2imgutils-9.0.3/lib/ec2imgutils/ec2imgutils.py` & `ec2imgutils-9.0.4/lib/ec2imgutils/ec2imgutils.py`

 * *Files identical despite different names*

### Comparing `ec2imgutils-9.0.3/lib/ec2imgutils/ec2imgutilsExceptions.py` & `ec2imgutils-9.0.4/lib/ec2imgutils/ec2imgutilsExceptions.py`

 * *Files identical despite different names*

### Comparing `ec2imgutils-9.0.3/lib/ec2imgutils/ec2listimg.py` & `ec2imgutils-9.0.4/lib/ec2imgutils/ec2listimg.py`

 * *Files identical despite different names*

### Comparing `ec2imgutils-9.0.3/lib/ec2imgutils/ec2publishimg.py` & `ec2imgutils-9.0.4/lib/ec2imgutils/ec2publishimg.py`

 * *Files identical despite different names*

### Comparing `ec2imgutils-9.0.3/lib/ec2imgutils/ec2removeimg.py` & `ec2imgutils-9.0.4/lib/ec2imgutils/ec2removeimg.py`

 * *Files identical despite different names*

### Comparing `ec2imgutils-9.0.3/lib/ec2imgutils/ec2setup.py` & `ec2imgutils-9.0.4/lib/ec2imgutils/ec2setup.py`

 * *Files identical despite different names*

### Comparing `ec2imgutils-9.0.3/lib/ec2imgutils/ec2uploadimg.py` & `ec2imgutils-9.0.4/lib/ec2imgutils/ec2uploadimg.py`

 * *Files 0% similar despite different names*

```diff
@@ -586,15 +586,16 @@
         ssh_connection = None
         timeout_counter = 1
         while not ssh_connection:
             try:
                 ssh_connection = client.connect(
                     key_filename=self.ssh_key_private_key_file,
                     username=self.inst_user_name,
-                    hostname=instance_ip
+                    hostname=instance_ip,
+                    timeout=10
                 )
             except (Exception, ConnectionResetError):
                 if self.log_level == logging.DEBUG:
                     print('. ', end=' ')
                     sys.stdout.flush()
                 time.sleep(self.default_sleep)
                 if (
```

### Comparing `ec2imgutils-9.0.3/lib/ec2imgutils/ec2utils.py` & `ec2imgutils-9.0.4/lib/ec2imgutils/ec2utils.py`

 * *Files identical despite different names*

### Comparing `ec2imgutils-9.0.3/lib/ec2imgutils.egg-info/PKG-INFO` & `ec2imgutils-9.0.4/lib/ec2imgutils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ec2imgutils
-Version: 9.0.3
+Version: 9.0.4
 Summary: Command-line tools to manage images in AWS EC2
 Home-page: https://github.com/SUSE-Enceladus/ec2imgutils
 Author: SUSE Public Cloud Team
 Author-email: public-cloud-dev@susecloud.net
 License: GPLv3+
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ec2imgutils-9.0.3/lib/ec2imgutils.egg-info/SOURCES.txt` & `ec2imgutils-9.0.4/lib/ec2imgutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ec2imgutils-9.0.3/man/man1/ec2deprecateimg.1` & `ec2imgutils-9.0.4/man/man1/ec2deprecateimg.1`

 * *Files identical despite different names*

### Comparing `ec2imgutils-9.0.3/man/man1/ec2listimg.1` & `ec2imgutils-9.0.4/man/man1/ec2listimg.1`

 * *Files identical despite different names*

### Comparing `ec2imgutils-9.0.3/man/man1/ec2publishimg.1` & `ec2imgutils-9.0.4/man/man1/ec2publishimg.1`

 * *Files identical despite different names*

### Comparing `ec2imgutils-9.0.3/man/man1/ec2removeimg.1` & `ec2imgutils-9.0.4/man/man1/ec2removeimg.1`

 * *Files identical despite different names*

### Comparing `ec2imgutils-9.0.3/man/man1/ec2uploadimg.1` & `ec2imgutils-9.0.4/man/man1/ec2uploadimg.1`

 * *Files identical despite different names*

### Comparing `ec2imgutils-9.0.3/setup.py` & `ec2imgutils-9.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `ec2imgutils-9.0.3/tests/test_ec2utilsutils.py` & `ec2imgutils-9.0.4/tests/test_ec2utilsutils.py`

 * *Files identical despite different names*

