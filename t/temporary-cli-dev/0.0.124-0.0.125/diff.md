# Comparing `tmp/temporary-cli-dev-0.0.124.tar.gz` & `tmp/temporary-cli-dev-0.0.125.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "temporary-cli-dev-0.0.124.tar", last modified: Tue May 16 21:23:09 2023, max compression
+gzip compressed data, was "temporary-cli-dev-0.0.125.tar", last modified: Tue May 16 21:32:37 2023, max compression
```

## Comparing `temporary-cli-dev-0.0.124.tar` & `temporary-cli-dev-0.0.125.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 winikatesl   (501) staff       (20)        0 2023-05-16 21:23:09.860374 temporary-cli-dev-0.0.124/
--rw-r--r--   0 winikatesl   (501) staff       (20)    11345 2023-05-11 19:56:12.000000 temporary-cli-dev-0.0.124/LICENSE
--rw-r--r--   0 winikatesl   (501) staff       (20)      211 2023-05-11 19:56:12.000000 temporary-cli-dev-0.0.124/MANIFEST.in
--rw-r--r--   0 winikatesl   (501) staff       (20)     1345 2023-05-16 21:23:09.860565 temporary-cli-dev-0.0.124/PKG-INFO
--rw-r--r--   0 winikatesl   (501) staff       (20)      344 2023-05-12 23:05:23.000000 temporary-cli-dev-0.0.124/README.rst
--rw-r--r--   0 winikatesl   (501) staff       (20)       67 2023-05-16 21:23:09.861487 temporary-cli-dev-0.0.124/setup.cfg
--rw-r--r--   0 winikatesl   (501) staff       (20)     2200 2023-05-16 21:06:35.000000 temporary-cli-dev-0.0.124/setup.py
-drwxr-xr-x   0 winikatesl   (501) staff       (20)        0 2023-05-16 21:23:09.859854 temporary-cli-dev-0.0.124/temporary_cli_dev.egg-info/
--rw-r--r--   0 winikatesl   (501) staff       (20)      752 2023-05-16 21:23:09.000000 temporary-cli-dev-0.0.124/temporary_cli_dev.egg-info/SOURCES.txt
-drwxr-xr-x   0 winikatesl   (501) staff       (20)        0 2023-05-16 21:23:09.834065 temporary-cli-dev-0.0.124/tests/
--rw-r--r--   0 winikatesl   (501) staff       (20)      838 2023-05-11 19:56:12.000000 temporary-cli-dev-0.0.124/tests/test_cli.py
-drwxr-xr-x   0 winikatesl   (501) staff       (20)        0 2023-05-16 21:23:09.835157 temporary-cli-dev-0.0.124/wavefront_cli/
--rw-r--r--   0 winikatesl   (501) staff       (20)       64 2023-05-16 21:23:08.000000 temporary-cli-dev-0.0.124/wavefront_cli/__init__.py
--rw-r--r--   0 winikatesl   (501) staff       (20)     2256 2023-05-16 21:05:03.000000 temporary-cli-dev-0.0.124/wavefront_cli/cli.py
-drwxr-xr-x   0 winikatesl   (501) staff       (20)        0 2023-05-16 21:23:09.846636 temporary-cli-dev-0.0.124/wavefront_cli/commands/
--rw-r--r--   0 winikatesl   (501) staff       (20)      277 2023-05-11 19:56:12.000000 temporary-cli-dev-0.0.124/wavefront_cli/commands/__init__.py
--rw-r--r--   0 winikatesl   (501) staff       (20)      496 2023-05-11 19:56:12.000000 temporary-cli-dev-0.0.124/wavefront_cli/commands/base.py
--rw-r--r--   0 winikatesl   (501) staff       (20)      421 2023-05-11 19:56:12.000000 temporary-cli-dev-0.0.124/wavefront_cli/commands/configure.py
--rw-r--r--   0 winikatesl   (501) staff       (20)      423 2023-05-11 19:56:12.000000 temporary-cli-dev-0.0.124/wavefront_cli/commands/hello.py
--rw-r--r--   0 winikatesl   (501) staff       (20)     9085 2023-05-16 21:20:43.000000 temporary-cli-dev-0.0.124/wavefront_cli/commands/install.py
--rw-r--r--   0 winikatesl   (501) staff       (20)     1642 2023-05-11 19:56:12.000000 temporary-cli-dev-0.0.124/wavefront_cli/commands/integration.py
-drwxr-xr-x   0 winikatesl   (501) staff       (20)        0 2023-05-16 21:23:09.850083 temporary-cli-dev-0.0.124/wavefront_cli/integrations/
--rw-r--r--   0 winikatesl   (501) staff       (20)      246 2023-05-11 19:56:12.000000 temporary-cli-dev-0.0.124/wavefront_cli/integrations/__init__.py
--rw-r--r--   0 winikatesl   (501) staff       (20)     1426 2023-05-11 19:56:12.000000 temporary-cli-dev-0.0.124/wavefront_cli/integrations/base.py
--rw-r--r--   0 winikatesl   (501) staff       (20)     1499 2023-05-11 19:56:12.000000 temporary-cli-dev-0.0.124/wavefront_cli/integrations/example.py
--rw-r--r--   0 winikatesl   (501) staff       (20)     2992 2023-05-11 19:56:12.000000 temporary-cli-dev-0.0.124/wavefront_cli/integrations/statsd.py
--rw-r--r--   0 winikatesl   (501) staff       (20)     2223 2023-05-11 19:56:12.000000 temporary-cli-dev-0.0.124/wavefront_cli/integrations/wavefront.py
-drwxr-xr-x   0 winikatesl   (501) staff       (20)        0 2023-05-16 21:23:09.858983 temporary-cli-dev-0.0.124/wavefront_cli/lib/
--rw-r--r--   0 winikatesl   (501) staff       (20)      349 2023-05-11 19:56:12.000000 temporary-cli-dev-0.0.124/wavefront_cli/lib/__init__.py
--rw-r--r--   0 winikatesl   (501) staff       (20)     3889 2023-05-11 19:56:12.000000 temporary-cli-dev-0.0.124/wavefront_cli/lib/agent.py
--rw-r--r--   0 winikatesl   (501) staff       (20)     1511 2023-05-11 19:56:12.000000 temporary-cli-dev-0.0.124/wavefront_cli/lib/api.py
--rw-r--r--   0 winikatesl   (501) staff       (20)     2431 2023-05-11 19:56:12.000000 temporary-cli-dev-0.0.124/wavefront_cli/lib/auth.py
--rw-r--r--   0 winikatesl   (501) staff       (20)     2064 2023-05-11 19:56:12.000000 temporary-cli-dev-0.0.124/wavefront_cli/lib/aws.py
--rw-r--r--   0 winikatesl   (501) staff       (20)     1313 2023-05-11 19:56:12.000000 temporary-cli-dev-0.0.124/wavefront_cli/lib/message.py
--rw-r--r--   0 winikatesl   (501) staff       (20)     4104 2023-05-11 19:56:12.000000 temporary-cli-dev-0.0.124/wavefront_cli/lib/proxy.py
--rw-r--r--   0 winikatesl   (501) staff       (20)     1889 2023-05-11 19:56:12.000000 temporary-cli-dev-0.0.124/wavefront_cli/lib/system.py
--rw-r--r--   0 winikatesl   (501) staff       (20)      692 2023-05-11 19:56:12.000000 temporary-cli-dev-0.0.124/wavefront_cli/lib/util.py
+drwxr-xr-x   0 winikatesl   (501) staff       (20)        0 2023-05-16 21:32:37.956316 temporary-cli-dev-0.0.125/
+-rw-r--r--   0 winikatesl   (501) staff       (20)    11345 2023-05-11 19:56:12.000000 temporary-cli-dev-0.0.125/LICENSE
+-rw-r--r--   0 winikatesl   (501) staff       (20)      211 2023-05-11 19:56:12.000000 temporary-cli-dev-0.0.125/MANIFEST.in
+-rw-r--r--   0 winikatesl   (501) staff       (20)     1345 2023-05-16 21:32:37.956500 temporary-cli-dev-0.0.125/PKG-INFO
+-rw-r--r--   0 winikatesl   (501) staff       (20)      344 2023-05-12 23:05:23.000000 temporary-cli-dev-0.0.125/README.rst
+-rw-r--r--   0 winikatesl   (501) staff       (20)       67 2023-05-16 21:32:37.957479 temporary-cli-dev-0.0.125/setup.cfg
+-rw-r--r--   0 winikatesl   (501) staff       (20)     2200 2023-05-16 21:06:35.000000 temporary-cli-dev-0.0.125/setup.py
+drwxr-xr-x   0 winikatesl   (501) staff       (20)        0 2023-05-16 21:32:37.955833 temporary-cli-dev-0.0.125/temporary_cli_dev.egg-info/
+-rw-r--r--   0 winikatesl   (501) staff       (20)      752 2023-05-16 21:32:37.000000 temporary-cli-dev-0.0.125/temporary_cli_dev.egg-info/SOURCES.txt
+drwxr-xr-x   0 winikatesl   (501) staff       (20)        0 2023-05-16 21:32:37.929184 temporary-cli-dev-0.0.125/tests/
+-rw-r--r--   0 winikatesl   (501) staff       (20)      838 2023-05-11 19:56:12.000000 temporary-cli-dev-0.0.125/tests/test_cli.py
+drwxr-xr-x   0 winikatesl   (501) staff       (20)        0 2023-05-16 21:32:37.930316 temporary-cli-dev-0.0.125/wavefront_cli/
+-rw-r--r--   0 winikatesl   (501) staff       (20)       64 2023-05-16 21:32:31.000000 temporary-cli-dev-0.0.125/wavefront_cli/__init__.py
+-rw-r--r--   0 winikatesl   (501) staff       (20)     2256 2023-05-16 21:05:03.000000 temporary-cli-dev-0.0.125/wavefront_cli/cli.py
+drwxr-xr-x   0 winikatesl   (501) staff       (20)        0 2023-05-16 21:32:37.940127 temporary-cli-dev-0.0.125/wavefront_cli/commands/
+-rw-r--r--   0 winikatesl   (501) staff       (20)      277 2023-05-11 19:56:12.000000 temporary-cli-dev-0.0.125/wavefront_cli/commands/__init__.py
+-rw-r--r--   0 winikatesl   (501) staff       (20)      496 2023-05-11 19:56:12.000000 temporary-cli-dev-0.0.125/wavefront_cli/commands/base.py
+-rw-r--r--   0 winikatesl   (501) staff       (20)      421 2023-05-11 19:56:12.000000 temporary-cli-dev-0.0.125/wavefront_cli/commands/configure.py
+-rw-r--r--   0 winikatesl   (501) staff       (20)      423 2023-05-11 19:56:12.000000 temporary-cli-dev-0.0.125/wavefront_cli/commands/hello.py
+-rw-r--r--   0 winikatesl   (501) staff       (20)     9085 2023-05-16 21:32:26.000000 temporary-cli-dev-0.0.125/wavefront_cli/commands/install.py
+-rw-r--r--   0 winikatesl   (501) staff       (20)     1642 2023-05-11 19:56:12.000000 temporary-cli-dev-0.0.125/wavefront_cli/commands/integration.py
+drwxr-xr-x   0 winikatesl   (501) staff       (20)        0 2023-05-16 21:32:37.945343 temporary-cli-dev-0.0.125/wavefront_cli/integrations/
+-rw-r--r--   0 winikatesl   (501) staff       (20)      246 2023-05-11 19:56:12.000000 temporary-cli-dev-0.0.125/wavefront_cli/integrations/__init__.py
+-rw-r--r--   0 winikatesl   (501) staff       (20)     1426 2023-05-11 19:56:12.000000 temporary-cli-dev-0.0.125/wavefront_cli/integrations/base.py
+-rw-r--r--   0 winikatesl   (501) staff       (20)     1499 2023-05-11 19:56:12.000000 temporary-cli-dev-0.0.125/wavefront_cli/integrations/example.py
+-rw-r--r--   0 winikatesl   (501) staff       (20)     2992 2023-05-11 19:56:12.000000 temporary-cli-dev-0.0.125/wavefront_cli/integrations/statsd.py
+-rw-r--r--   0 winikatesl   (501) staff       (20)     2223 2023-05-11 19:56:12.000000 temporary-cli-dev-0.0.125/wavefront_cli/integrations/wavefront.py
+drwxr-xr-x   0 winikatesl   (501) staff       (20)        0 2023-05-16 21:32:37.954746 temporary-cli-dev-0.0.125/wavefront_cli/lib/
+-rw-r--r--   0 winikatesl   (501) staff       (20)      349 2023-05-11 19:56:12.000000 temporary-cli-dev-0.0.125/wavefront_cli/lib/__init__.py
+-rw-r--r--   0 winikatesl   (501) staff       (20)     3889 2023-05-11 19:56:12.000000 temporary-cli-dev-0.0.125/wavefront_cli/lib/agent.py
+-rw-r--r--   0 winikatesl   (501) staff       (20)     1511 2023-05-11 19:56:12.000000 temporary-cli-dev-0.0.125/wavefront_cli/lib/api.py
+-rw-r--r--   0 winikatesl   (501) staff       (20)     2431 2023-05-11 19:56:12.000000 temporary-cli-dev-0.0.125/wavefront_cli/lib/auth.py
+-rw-r--r--   0 winikatesl   (501) staff       (20)     2064 2023-05-11 19:56:12.000000 temporary-cli-dev-0.0.125/wavefront_cli/lib/aws.py
+-rw-r--r--   0 winikatesl   (501) staff       (20)     1313 2023-05-11 19:56:12.000000 temporary-cli-dev-0.0.125/wavefront_cli/lib/message.py
+-rw-r--r--   0 winikatesl   (501) staff       (20)     4104 2023-05-11 19:56:12.000000 temporary-cli-dev-0.0.125/wavefront_cli/lib/proxy.py
+-rw-r--r--   0 winikatesl   (501) staff       (20)     1889 2023-05-11 19:56:12.000000 temporary-cli-dev-0.0.125/wavefront_cli/lib/system.py
+-rw-r--r--   0 winikatesl   (501) staff       (20)      692 2023-05-11 19:56:12.000000 temporary-cli-dev-0.0.125/wavefront_cli/lib/util.py
```

### Comparing `temporary-cli-dev-0.0.124/LICENSE` & `temporary-cli-dev-0.0.125/LICENSE`

 * *Files identical despite different names*

### Comparing `temporary-cli-dev-0.0.124/PKG-INFO` & `temporary-cli-dev-0.0.125/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: temporary-cli-dev
-Version: 0.0.124
+Version: 0.0.125
 Summary: ---
 Home-page: https://github.com/wavefrontHQ/wavefront-cli
 Author: ----
 Author-email: foo@example.com
 License: UNLICENSE
 Keywords: lib,cli
 Classifier: Intended Audience :: Developers
```

### Comparing `temporary-cli-dev-0.0.124/setup.py` & `temporary-cli-dev-0.0.125/setup.py`

 * *Files identical despite different names*

### Comparing `temporary-cli-dev-0.0.124/temporary_cli_dev.egg-info/SOURCES.txt` & `temporary-cli-dev-0.0.125/temporary_cli_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `temporary-cli-dev-0.0.124/tests/test_cli.py` & `temporary-cli-dev-0.0.125/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `temporary-cli-dev-0.0.124/wavefront_cli/cli.py` & `temporary-cli-dev-0.0.125/wavefront_cli/cli.py`

 * *Files identical despite different names*

### Comparing `temporary-cli-dev-0.0.124/wavefront_cli/commands/install.py` & `temporary-cli-dev-0.0.125/wavefront_cli/commands/install.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     """Manage agent installation."""
 
     def run(self):
         """Install wavefront proxy/statsd/telegraf."""
         # pylint: disable=too-many-branches
         # pylint: disable=too-many-locals
         # pylint: disable=too-many-statements
-        agent_name = "_telegraf"
+        agent_name = "telegraf"
         lib.message.print_welcome()
         # pylint: disable=pointless-string-statement
         '''
         wave install
             [--proxy]
                 [--wavefront-url=<wavefront_url>]
                 [--api-token=<api_token>]
@@ -168,15 +168,15 @@
             if agent_tags:
                 tags = lib.util.cskv_to_dict(agent_tags)
                 if not lib.agent.tag_telegraf_config('cli user tags', tags):
                     sys.exit(1)
 
             # check if user 'telegraf' has read permission for config path if
             # not change owner of telegraf path to 'telegraf' user recursively
-            uid = pwd.getpwnam(agent_name).pw_uid
+            uid = pwd.getpwnam("_telegraf").pw_uid
             path = '/etc/telegraf'
 
             if not uid == os.stat(path).st_uid:
                 os.chown(path, uid, -1)
                 for root, dirs, files in os.walk(path):
                     for name in dirs:
                         os.chown(os.path.join(root, name), uid, -1)
```

### Comparing `temporary-cli-dev-0.0.124/wavefront_cli/commands/integration.py` & `temporary-cli-dev-0.0.125/wavefront_cli/commands/integration.py`

 * *Files identical despite different names*

### Comparing `temporary-cli-dev-0.0.124/wavefront_cli/integrations/base.py` & `temporary-cli-dev-0.0.125/wavefront_cli/integrations/base.py`

 * *Files identical despite different names*

### Comparing `temporary-cli-dev-0.0.124/wavefront_cli/integrations/example.py` & `temporary-cli-dev-0.0.125/wavefront_cli/integrations/example.py`

 * *Files identical despite different names*

### Comparing `temporary-cli-dev-0.0.124/wavefront_cli/integrations/statsd.py` & `temporary-cli-dev-0.0.125/wavefront_cli/integrations/statsd.py`

 * *Files identical despite different names*

### Comparing `temporary-cli-dev-0.0.124/wavefront_cli/integrations/wavefront.py` & `temporary-cli-dev-0.0.125/wavefront_cli/integrations/wavefront.py`

 * *Files identical despite different names*

### Comparing `temporary-cli-dev-0.0.124/wavefront_cli/lib/agent.py` & `temporary-cli-dev-0.0.125/wavefront_cli/lib/agent.py`

 * *Files identical despite different names*

### Comparing `temporary-cli-dev-0.0.124/wavefront_cli/lib/api.py` & `temporary-cli-dev-0.0.125/wavefront_cli/lib/api.py`

 * *Files identical despite different names*

### Comparing `temporary-cli-dev-0.0.124/wavefront_cli/lib/auth.py` & `temporary-cli-dev-0.0.125/wavefront_cli/lib/auth.py`

 * *Files identical despite different names*

### Comparing `temporary-cli-dev-0.0.124/wavefront_cli/lib/aws.py` & `temporary-cli-dev-0.0.125/wavefront_cli/lib/aws.py`

 * *Files identical despite different names*

### Comparing `temporary-cli-dev-0.0.124/wavefront_cli/lib/message.py` & `temporary-cli-dev-0.0.125/wavefront_cli/lib/message.py`

 * *Files identical despite different names*

### Comparing `temporary-cli-dev-0.0.124/wavefront_cli/lib/proxy.py` & `temporary-cli-dev-0.0.125/wavefront_cli/lib/proxy.py`

 * *Files identical despite different names*

### Comparing `temporary-cli-dev-0.0.124/wavefront_cli/lib/system.py` & `temporary-cli-dev-0.0.125/wavefront_cli/lib/system.py`

 * *Files identical despite different names*

### Comparing `temporary-cli-dev-0.0.124/wavefront_cli/lib/util.py` & `temporary-cli-dev-0.0.125/wavefront_cli/lib/util.py`

 * *Files identical despite different names*

