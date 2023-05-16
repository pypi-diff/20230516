# Comparing `tmp/postmaniac-0.9.0.tar.gz` & `tmp/postmaniac-0.9.2.tar.gz`

## Comparing `postmaniac-0.9.0.tar` & `postmaniac-0.9.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 postmaniac-0.9.0/requirements.txt
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 postmaniac-0.9.0/setup.py
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 postmaniac-0.9.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0     3018 2020-02-02 00:00:00.000000 postmaniac-0.9.0/.github/workflows/codeql.yml
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 postmaniac-0.9.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0   427725 2020-02-02 00:00:00.000000 postmaniac-0.9.0/assets/demo.gif
--rw-r--r--   0        0        0    81029 2020-02-02 00:00:00.000000 postmaniac-0.9.0/assets/long_banner.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 postmaniac-0.9.0/postmaniac/__init__.py
--rw-r--r--   0        0        0    15516 2020-02-02 00:00:00.000000 postmaniac-0.9.0/postmaniac/postmaniac.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 postmaniac-0.9.0/.gitignore
--rw-r--r--   0        0        0    34888 2020-02-02 00:00:00.000000 postmaniac-0.9.0/LICENSE.md
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 postmaniac-0.9.0/README.md
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 postmaniac-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     2260 2020-02-02 00:00:00.000000 postmaniac-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 postmaniac-0.9.2/Dockerfile
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 postmaniac-0.9.2/requirements.txt
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 postmaniac-0.9.2/setup.py
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 postmaniac-0.9.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0     3018 2020-02-02 00:00:00.000000 postmaniac-0.9.2/.github/workflows/codeql.yml
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 postmaniac-0.9.2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0   427725 2020-02-02 00:00:00.000000 postmaniac-0.9.2/assets/demo.gif
+-rw-r--r--   0        0        0    81029 2020-02-02 00:00:00.000000 postmaniac-0.9.2/assets/long_banner.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 postmaniac-0.9.2/postmaniac/__init__.py
+-rw-r--r--   0        0        0    15576 2020-02-02 00:00:00.000000 postmaniac-0.9.2/postmaniac/postmaniac.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 postmaniac-0.9.2/.gitignore
+-rw-r--r--   0        0        0    34888 2020-02-02 00:00:00.000000 postmaniac-0.9.2/LICENSE.md
+-rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 postmaniac-0.9.2/README.md
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 postmaniac-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0     2572 2020-02-02 00:00:00.000000 postmaniac-0.9.2/PKG-INFO
```

### Comparing `postmaniac-0.9.0/setup.py` & `postmaniac-0.9.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 requirements = [x.strip() for x in open("requirements.txt", "r").readlines()]
 requirements = [
     f"{line.split('#egg=')[-1]} @ {line}" if "#egg=" in line else line for line in requirements]
 
 setup(
     name='postmaniac',
-    version='0.9.0',
+    version='0.9.2',
     packages=find_packages(),
     license='GNU General Public License v3 (GPLv3)',
     license_files=('LICENSE.md'),
     author='boringthegod',
     author_email='boringthegod@tutanota.com',
     description='Postman OSINT tool to extract creds, token, username, email & more from Postman Public Workspaces.',
     url='https://github.com/boringthegod/postmaniac',
```

### Comparing `postmaniac-0.9.0/.github/ISSUE_TEMPLATE/bug_report.md` & `postmaniac-0.9.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `postmaniac-0.9.0/.github/workflows/codeql.yml` & `postmaniac-0.9.2/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `postmaniac-0.9.0/.github/workflows/python-publish.yml` & `postmaniac-0.9.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `postmaniac-0.9.0/assets/demo.gif` & `postmaniac-0.9.2/assets/demo.gif`

 * *Files identical despite different names*

### Comparing `postmaniac-0.9.0/assets/long_banner.png` & `postmaniac-0.9.2/assets/long_banner.png`

 * *Files identical despite different names*

### Comparing `postmaniac-0.9.0/postmaniac/postmaniac.py` & `postmaniac-0.9.2/postmaniac/postmaniac.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     with open("scan.txt", "w") as f:
         f.write("Rapport du scan de " + f"{args.query}")
         f.write("\n")
         f.write("\n")
 
     url = 'https://www.postman.com/_api/ws/proxy'
     headers = {
-        'User-Agent': 'postmaniac',
+        'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64; rv:102.0) Gecko/20100101 Firefox/102.0',
         'Content-Type': 'application/json',
     }
 
     data_raw = {
         "service": "search",
         "method": "POST",
         "path": "/search-all",
```

### Comparing `postmaniac-0.9.0/LICENSE.md` & `postmaniac-0.9.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `postmaniac-0.9.0/README.md` & `postmaniac-0.9.2/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -33,14 +33,26 @@
 # change the working directory to postmaniac
 $ cd postmaniac
 
 # install postmaniac
 $ python3 setup.py install
 ```
 
+### With Docker
+
+You can pull the Docker image with:
+
+```bash
+docker pull ghcr.io/boringthegod/postmaniac:latest
+```
+
+And then launch the tool **by not forgetting to specify your volume** to be able to read the file scan.txt written in output
+
+`docker run -v scan:/output ghcr.io/boringthegod/postmaniac query`
+
 # Usage
 
 postmaniac can be run from the CLI and rapidly embedded within existing python applications.
 
 ```bash
 usage: postmaniac [-h] query
```

### Comparing `postmaniac-0.9.0/pyproject.toml` & `postmaniac-0.9.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "postmaniac"
-version = "0.9.0"
+version = "0.9.2"
 description = "Postman OSINT tool to extract creds, token, username, email & more from Postman Public Workspaces."
 readme = "README.md"
 requires-python = ">=3.0"
 dependencies = [
   'colorama==0.4.6',
   'requests==2.30.0'
 ]
```

### Comparing `postmaniac-0.9.0/PKG-INFO` & `postmaniac-0.9.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: postmaniac
-Version: 0.9.0
+Version: 0.9.2
 Summary: Postman OSINT tool to extract creds, token, username, email & more from Postman Public Workspaces.
 Project-URL: Homepage, https://github.com/boringthegod/postmaniac
 Project-URL: Bug Tracker, https://github.com/boringthegod/postmaniac/issues
 Author-email: Pierre Ceberio <boringthegod@tutanota.com>
 License-File: LICENSE.md
 Keywords: cybersecurity,investigation,lespireshat,osint,pentest,postman
 Requires-Python: >=3.0
@@ -47,14 +47,26 @@
 # change the working directory to postmaniac
 $ cd postmaniac
 
 # install postmaniac
 $ python3 setup.py install
 ```
 
+### With Docker
+
+You can pull the Docker image with:
+
+```bash
+docker pull ghcr.io/boringthegod/postmaniac:latest
+```
+
+And then launch the tool **by not forgetting to specify your volume** to be able to read the file scan.txt written in output
+
+`docker run -v scan:/output ghcr.io/boringthegod/postmaniac query`
+
 # Usage
 
 postmaniac can be run from the CLI and rapidly embedded within existing python applications.
 
 ```bash
 usage: postmaniac [-h] query
```

