# Comparing `tmp/shbin-0.1.2.tar.gz` & `tmp/shbin-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shbin-0.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "shbin-0.1.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `shbin-0.1.2.tar` & `shbin-0.1.3.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     4887 2023-05-16 19:56:37.006983 shbin-0.1.2/README.md
--rw-r--r--   0        0        0     1081 2023-05-16 19:56:37.006983 shbin-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     7827 2023-05-16 19:56:37.006983 shbin-0.1.2/shbin.py
--rw-r--r--   0        0        0     5728 1970-01-01 00:00:00.000000 shbin-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     4901 2023-05-16 20:03:37.038733 shbin-0.1.3/README.md
+-rw-r--r--   0        0        0     1081 2023-05-16 20:03:37.038733 shbin-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     7827 2023-05-16 20:03:37.038733 shbin-0.1.3/shbin.py
+-rw-r--r--   0        0        0     5742 1970-01-01 00:00:00.000000 shbin-0.1.3/PKG-INFO
```

### Comparing `shbin-0.1.2/README.md` & `shbin-0.1.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -92,17 +92,17 @@
 
 ```console
 port install file
 ```
 
 # Setup
 
-Create a [new fine-grained personal token](https://github.com/settings/personal-access-tokens/new) on Github for your "pastebin" repository (under your user or your organization ownership), with the following permissions: 
+Create a [new fine-grained personal token](https://github.com/settings/personal-access-tokens/new) on Github for your "pastebin" repository (under your user or your organization ownership), with read and write permissions on "contents: 
 
-![image](https://user-images.githubusercontent.com/2355719/238744990-94388e54-4cf3-4e01-8276-0675059d0cda.png)
+![image](https://user-images.githubusercontent.com/2355719/238758491-9d15e7e6-e4b7-43c8-a321-b65c968fc7e0.png)
 
 - Then set the environment variables in your preferred place:
     
   ```
   export SHBIN_GITHUB_TOKEN="<your personal token>"
   export SHBIN_REPO="<user_or_org>/<repo>"   # example "Shiphero/pastebin"   
    ```
```

### Comparing `shbin-0.1.2/pyproject.toml` & `shbin-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `shbin-0.1.2/shbin.py` & `shbin-0.1.3/shbin.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
   -m <message>, --message=<message>                 Commit message
   -d <target-dir>, --target-dir=<target-dir>        Optional (sub)directory to upload file/s. 
   --namespace=<namespace>                           Base namespace to upload. Default to
                                                     SHBIN_NAMESPACE envvar or "{user}/". 
   -p, --url-link-to-pages                           Reformat the url to link to Github pages. 
 """
 
-__version__ = "0.1.2"
+__version__ = "0.1.3"
 
 
 class FakePath:
     """
     A wrapper on a PurePath object (ie it doesn’t actually access a filesystem)
     with an explicity content in bytes.
     """
```

### Comparing `shbin-0.1.2/PKG-INFO` & `shbin-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shbin
-Version: 0.1.2
+Version: 0.1.3
 Summary: Turns a Github repo into a pastebin.
 Author-email: Alvar Maciel <alvar.maciel@shiphero.com>, Martín Gaitán <marting@shiphero.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
@@ -115,17 +115,17 @@
 
 ```console
 port install file
 ```
 
 # Setup
 
-Create a [new fine-grained personal token](https://github.com/settings/personal-access-tokens/new) on Github for your "pastebin" repository (under your user or your organization ownership), with the following permissions: 
+Create a [new fine-grained personal token](https://github.com/settings/personal-access-tokens/new) on Github for your "pastebin" repository (under your user or your organization ownership), with read and write permissions on "contents: 
 
-![image](https://user-images.githubusercontent.com/2355719/238744990-94388e54-4cf3-4e01-8276-0675059d0cda.png)
+![image](https://user-images.githubusercontent.com/2355719/238758491-9d15e7e6-e4b7-43c8-a321-b65c968fc7e0.png)
 
 - Then set the environment variables in your preferred place:
     
   ```
   export SHBIN_GITHUB_TOKEN="<your personal token>"
   export SHBIN_REPO="<user_or_org>/<repo>"   # example "Shiphero/pastebin"   
    ```
```

