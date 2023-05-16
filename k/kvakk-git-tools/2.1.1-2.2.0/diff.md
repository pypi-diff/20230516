# Comparing `tmp/kvakk_git_tools-2.1.1.tar.gz` & `tmp/kvakk_git_tools-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kvakk_git_tools-2.1.1.tar", max compression
+gzip compressed data, was "kvakk_git_tools-2.2.0.tar", max compression
```

## Comparing `kvakk_git_tools-2.1.1.tar` & `kvakk_git_tools-2.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1074 2023-05-16 10:55:11.951469 kvakk_git_tools-2.1.1/LICENSE
--rw-r--r--   0        0        0     2972 2023-05-16 10:55:11.951469 kvakk_git_tools-2.1.1/README.md
--rw-r--r--   0        0        0      134 2023-05-16 10:55:11.951469 kvakk_git_tools-2.1.1/kvakk_git_tools/__init__.py
--rw-r--r--   0        0        0       64 2023-05-16 10:55:11.951469 kvakk_git_tools-2.1.1/kvakk_git_tools/recommended/gitattributes
--rw-r--r--   0        0        0      215 2023-05-16 10:55:11.951469 kvakk_git_tools-2.1.1/kvakk_git_tools/recommended/gitconfig-adm-mac
--rw-r--r--   0        0        0      515 2023-05-16 10:55:11.951469 kvakk_git_tools-2.1.1/kvakk_git_tools/recommended/gitconfig-dapla
--rw-r--r--   0        0        0      645 2023-05-16 10:55:11.951469 kvakk_git_tools-2.1.1/kvakk_git_tools/recommended/gitconfig-prod-linux
--rw-r--r--   0        0        0      472 2023-05-16 10:55:11.951469 kvakk_git_tools-2.1.1/kvakk_git_tools/recommended/gitconfig-prod-windows-citrix
--rw-r--r--   0        0        0     4656 2023-05-16 10:55:11.951469 kvakk_git_tools-2.1.1/kvakk_git_tools/recommended/gitignore
--rwxr-xr-x   0        0        0    12531 2023-05-16 10:55:11.951469 kvakk_git_tools-2.1.1/kvakk_git_tools/ssb_gitconfig.py
--rw-r--r--   0        0        0     2061 2023-05-16 10:55:11.951469 kvakk_git_tools-2.1.1/kvakk_git_tools/validate_ssb_gitconfig.py
--rw-r--r--   0        0        0     1003 2023-05-16 10:55:11.951469 kvakk_git_tools-2.1.1/pyproject.toml
--rw-r--r--   0        0        0     3466 1970-01-01 00:00:00.000000 kvakk_git_tools-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-05-16 10:55:07.785961 kvakk_git_tools-2.2.0/LICENSE
+-rw-r--r--   0        0        0     2972 2023-05-16 10:55:07.785961 kvakk_git_tools-2.2.0/README.md
+-rw-r--r--   0        0        0      134 2023-05-16 10:55:07.785961 kvakk_git_tools-2.2.0/kvakk_git_tools/__init__.py
+-rw-r--r--   0        0        0       64 2023-05-16 10:55:07.785961 kvakk_git_tools-2.2.0/kvakk_git_tools/recommended/gitattributes
+-rw-r--r--   0        0        0      215 2023-05-16 10:55:07.785961 kvakk_git_tools-2.2.0/kvakk_git_tools/recommended/gitconfig-adm-mac
+-rw-r--r--   0        0        0      515 2023-05-16 10:55:07.785961 kvakk_git_tools-2.2.0/kvakk_git_tools/recommended/gitconfig-dapla
+-rw-r--r--   0        0        0      645 2023-05-16 10:55:07.785961 kvakk_git_tools-2.2.0/kvakk_git_tools/recommended/gitconfig-prod-linux
+-rw-r--r--   0        0        0      472 2023-05-16 10:55:07.785961 kvakk_git_tools-2.2.0/kvakk_git_tools/recommended/gitconfig-prod-windows-citrix
+-rw-r--r--   0        0        0     4656 2023-05-16 10:55:07.785961 kvakk_git_tools-2.2.0/kvakk_git_tools/recommended/gitignore
+-rwxr-xr-x   0        0        0    12531 2023-05-16 10:55:07.785961 kvakk_git_tools-2.2.0/kvakk_git_tools/ssb_gitconfig.py
+-rw-r--r--   0        0        0     2061 2023-05-16 10:55:07.785961 kvakk_git_tools-2.2.0/kvakk_git_tools/validate_ssb_gitconfig.py
+-rw-r--r--   0        0        0     1003 2023-05-16 10:55:07.785961 kvakk_git_tools-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3466 1970-01-01 00:00:00.000000 kvakk_git_tools-2.2.0/PKG-INFO
```

### Comparing `kvakk_git_tools-2.1.1/LICENSE` & `kvakk_git_tools-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kvakk_git_tools-2.1.1/README.md` & `kvakk_git_tools-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `kvakk_git_tools-2.1.1/kvakk_git_tools/recommended/gitconfig-dapla` & `kvakk_git_tools-2.2.0/kvakk_git_tools/recommended/gitconfig-dapla`

 * *Files identical despite different names*

### Comparing `kvakk_git_tools-2.1.1/kvakk_git_tools/recommended/gitconfig-prod-linux` & `kvakk_git_tools-2.2.0/kvakk_git_tools/recommended/gitconfig-prod-linux`

 * *Files identical despite different names*

### Comparing `kvakk_git_tools-2.1.1/kvakk_git_tools/recommended/gitignore` & `kvakk_git_tools-2.2.0/kvakk_git_tools/recommended/gitignore`

 * *Files identical despite different names*

### Comparing `kvakk_git_tools-2.1.1/kvakk_git_tools/ssb_gitconfig.py` & `kvakk_git_tools-2.2.0/kvakk_git_tools/ssb_gitconfig.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 https://github.com/statisticsnorway/kvakk-git-tools.git. The script clones this
 repo and selects the base git config based on the detected platform.
 
 If there is an existing .gitconfig file, it is backed up, and the name and email
 address are extracted from it and reused.
 """
 
-__version__ = "2.1.1"
+__version__ = "2.2.0"
 
 import argparse
 import getpass
 import os
 import platform
 import shutil
 import stat
@@ -215,15 +215,15 @@
     temp_dir = Path.home() / "temp-ssb-gitconfig"
     config_dir = temp_dir / "kvakk-git-tools" / "kvakk_git_tools" / "recommended"
     dst = Path().home() / ".gitconfig"
     src = config_dir / f"gitconfig-{pl.name().value}"
     if test:
         src = config_dir / "gitconfig-dapla"
 
-    options = ["--branch", "2.1.1"]
+    options = ["--branch", "2.2.0"]
     prod_zone_windows = pl.name() is PlatformName.PROD_WINDOWS_CITRIX
     prod_zone_linux = pl.name() is PlatformName.PROD_LINUX
     if prod_zone_windows or prod_zone_linux:
         options = ["-c", "http.sslVerify=False"]
 
     cmd = (
         ["git"]
@@ -231,15 +231,15 @@
         + options
     )
     print("Get recommended gitconfigs by cloning repo...")
 
     # Fix for python < 3.7, using stdout.
     # Use capture_output=true instead of stdout when python >= 3.7
     with TempDir(temp_dir):
-        subprocess.run(cmd, cwd=temp_dir, stderr=subprocess.DEVNULL, check=True)
+        subprocess.run(cmd, cwd=temp_dir, stdout=subprocess.DEVNULL, check=True)
         dst.write_bytes(src.read_bytes())
 
         # Replace template username with real username
         if pl.name() is PlatformName.PROD_WINDOWS_CITRIX:
             windows_username = getpass.getuser()
             replace_text_in_file("username", windows_username, dst)
```

### Comparing `kvakk_git_tools-2.1.1/kvakk_git_tools/validate_ssb_gitconfig.py` & `kvakk_git_tools-2.2.0/kvakk_git_tools/validate_ssb_gitconfig.py`

 * *Files identical despite different names*

### Comparing `kvakk_git_tools-2.1.1/pyproject.toml` & `kvakk_git_tools-2.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kvakk-git-tools"
-version = "2.1.1"
+version = "2.2.0"
 description = "Recommended git config and git scripts for Statistics Norway."
 authors = ["Arne Sørli <81353974+arneso-ssb@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "kvakk_git_tools" }]
 
 [tool.poetry.scripts]
```

### Comparing `kvakk_git_tools-2.1.1/PKG-INFO` & `kvakk_git_tools-2.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kvakk-git-tools
-Version: 2.1.1
+Version: 2.2.0
 Summary: Recommended git config and git scripts for Statistics Norway.
 License: MIT
 Author: Arne Sørli
 Author-email: 81353974+arneso-ssb@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

