# Comparing `tmp/python-dotenv-vault-0.5.2.tar.gz` & `tmp/python-dotenv-vault-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-dotenv-vault-0.5.2.tar", last modified: Fri May  5 05:53:39 2023, max compression
+gzip compressed data, was "python-dotenv-vault-0.6.0.tar", last modified: Tue May 16 04:39:03 2023, max compression
```

## Comparing `python-dotenv-vault-0.5.2.tar` & `python-dotenv-vault-0.6.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:39.558388 python-dotenv-vault-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-05 05:53:21.000000 python-dotenv-vault-0.5.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-05 05:53:21.000000 python-dotenv-vault-0.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-05 05:53:21.000000 python-dotenv-vault-0.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7333 2023-05-05 05:53:39.558388 python-dotenv-vault-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-05-05 05:53:21.000000 python-dotenv-vault-0.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-05 05:53:21.000000 python-dotenv-vault-0.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 05:53:39.558388 python-dotenv-vault-0.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-05 05:53:21.000000 python-dotenv-vault-0.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:39.558388 python-dotenv-vault-0.5.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:39.558388 python-dotenv-vault-0.5.2/src/dotenv_vault/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-05 05:53:21.000000 python-dotenv-vault-0.5.2/src/dotenv_vault/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-05 05:53:21.000000 python-dotenv-vault-0.5.2/src/dotenv_vault/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-05-05 05:53:21.000000 python-dotenv-vault-0.5.2/src/dotenv_vault/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-05-05 05:53:21.000000 python-dotenv-vault-0.5.2/src/dotenv_vault/test_vault.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:39.558388 python-dotenv-vault-0.5.2/src/python_dotenv_vault.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7333 2023-05-05 05:53:39.000000 python-dotenv-vault-0.5.2/src/python_dotenv_vault.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-05 05:53:39.000000 python-dotenv-vault-0.5.2/src/python_dotenv_vault.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 05:53:39.000000 python-dotenv-vault-0.5.2/src/python_dotenv_vault.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-05 05:53:39.000000 python-dotenv-vault-0.5.2/src/python_dotenv_vault.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-05 05:53:39.000000 python-dotenv-vault-0.5.2/src/python_dotenv_vault.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:39:03.167764 python-dotenv-vault-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-05-16 04:38:44.000000 python-dotenv-vault-0.6.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-16 04:38:44.000000 python-dotenv-vault-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-16 04:38:44.000000 python-dotenv-vault-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7454 2023-05-16 04:39:03.167764 python-dotenv-vault-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-05-16 04:38:44.000000 python-dotenv-vault-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-16 04:38:44.000000 python-dotenv-vault-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 04:39:03.167764 python-dotenv-vault-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-16 04:38:44.000000 python-dotenv-vault-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:39:03.163764 python-dotenv-vault-0.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:39:03.163764 python-dotenv-vault-0.6.0/src/dotenv_vault/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-16 04:38:44.000000 python-dotenv-vault-0.6.0/src/dotenv_vault/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-16 04:38:44.000000 python-dotenv-vault-0.6.0/src/dotenv_vault/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5293 2023-05-16 04:38:44.000000 python-dotenv-vault-0.6.0/src/dotenv_vault/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-05-16 04:38:44.000000 python-dotenv-vault-0.6.0/src/dotenv_vault/test_vault.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:39:03.163764 python-dotenv-vault-0.6.0/src/python_dotenv_vault.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7454 2023-05-16 04:39:03.000000 python-dotenv-vault-0.6.0/src/python_dotenv_vault.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-16 04:39:03.000000 python-dotenv-vault-0.6.0/src/python_dotenv_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 04:39:03.000000 python-dotenv-vault-0.6.0/src/python_dotenv_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-16 04:39:03.000000 python-dotenv-vault-0.6.0/src/python_dotenv_vault.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-16 04:39:03.000000 python-dotenv-vault-0.6.0/src/python_dotenv_vault.egg-info/top_level.txt
```

### Comparing `python-dotenv-vault-0.5.2/CHANGELOG.md` & `python-dotenv-vault-0.6.0/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 # Changelog
 
 All notable changes to this project will be documented in this file. See [standard-version](https://github.com/conventional-changelog/standard-version) for commit guidelines.
 
 ## [Unreleased](https://github.com/dotenv-org/python-dotenv-vault/compare/v0.5.1...master)
 
+## 0.6.0
+
+### Changed
+
+- Fix environment variable load [#12](https://github.com/dotenv-org/python-dotenv-vault/pull/12)
+
 ## 0.5.1
 
 ### Changed
 
 - Fix error reference [#10](https://github.com/dotenv-org/python-dotenv-vault/pull/10)
 
 ## 0.5.0
```

### Comparing `python-dotenv-vault-0.5.2/LICENSE` & `python-dotenv-vault-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-dotenv-vault-0.5.2/PKG-INFO` & `python-dotenv-vault-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-dotenv-vault
-Version: 0.5.2
+Version: 0.6.0
 Summary: Decrypt .env.vault file.
 Home-page: https://github.com/dotenv-org/python-dotenv-vault
 Author: dotenv
 Author-email: mot@dotenv.org
 License: MIT
 Keywords: environment,environment variables,deployments,settings,env,dotenv,configurations,python,dotenv-vault
 Description-Content-Type: text/markdown
@@ -170,14 +170,20 @@
 
 # Changelog
 
 All notable changes to this project will be documented in this file. See [standard-version](https://github.com/conventional-changelog/standard-version) for commit guidelines.
 
 ## [Unreleased](https://github.com/dotenv-org/python-dotenv-vault/compare/v0.5.1...master)
 
+## 0.6.0
+
+### Changed
+
+- Fix environment variable load [#12](https://github.com/dotenv-org/python-dotenv-vault/pull/12)
+
 ## 0.5.1
 
 ### Changed
 
 - Fix error reference [#10](https://github.com/dotenv-org/python-dotenv-vault/pull/10)
 
 ## 0.5.0
```

### Comparing `python-dotenv-vault-0.5.2/README.md` & `python-dotenv-vault-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `python-dotenv-vault-0.5.2/setup.py` & `python-dotenv-vault-0.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `python-dotenv-vault-0.5.2/src/dotenv_vault/main.py` & `python-dotenv-vault-0.6.0/src/dotenv_vault/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import dotenv.main as dotenv
 
 
 def load_dotenv(
     dotenv_path: Union[str, os.PathLike, None] = None,
     stream: Optional[IO[str]] = None,
     verbose: bool = False,
-    override: bool = False,
+    override: bool = True,
     interpolate: bool = True,
     encoding: Optional[str] = "utf-8",
 ) -> bool:
     """This function will read your encrypted env file and load it
     into the environment for this process.
 
     Call this function as close as possible to the start of your
@@ -38,15 +38,14 @@
     overrides existing environment settings or not is determined by
     the `override` flag.
 
     """
     if "DOTENV_KEY" in os.environ:
         vault_stream = parse_vault(open(".env.vault"))
         return dotenv.load_dotenv(
-            dotenv_path=".env.vault",
             stream=vault_stream,
             verbose=verbose,
             override=override,
             interpolate=interpolate
         )
     else:
         return dotenv.load_dotenv(
```

### Comparing `python-dotenv-vault-0.5.2/src/dotenv_vault/test_vault.py` & `python-dotenv-vault-0.6.0/src/dotenv_vault/test_vault.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from io import StringIO
 import os
 import unittest
 
-from dotenv.main import DotEnv
+from dotenv.main import load_dotenv
 
 import dotenv_vault.main as vault
 
 class TestParsing(unittest.TestCase):
     TEST_KEYS = [
         # OK.
         ["dotenv://:key_0dec82bea24ada79a983dcc11b431e28838eae59a07a8f983247c7ca9027a925@dotenv.local/vault/.env.vault?environment=development",
@@ -36,24 +36,28 @@
             except Exception as exc:
                 self.assertFalse(should_pass)
             finally:
                 os.unsetenv("DOTENV_KEY")
                 if old_dotenv_key:
                     os.environ["DOTENV_KEY"] = old_dotenv_key
 
-    PARSE_TEST_KEY = "dotenv://:key_0dec82bea24ada79a983dcc11b431e28838eae59a07a8f983247c7ca9027a925@dotenv.local/vault/.env.vault?environment=development"
+    PARSE_TEST_KEY = "dotenv://:key_ff6456d445b08c289eec891ba1944e3ae09b00b33387d046624214aff27173d5@dotenv.org/vault/.env.vault?environment=production"
 
-    PARSE_TEST_VAULT = """# .env.vault (generated with npx dotenv-vault local build)
-                        DOTENV_VAULT_DEVELOPMENT="H2A2wOUZU+bjKH3kTpeua9iIhtK/q7/VpAn+LLVNnms+CtQ/cwXqiw=="
-                        """
+    PARSE_TEST_VAULT = """
+    DOTENV_VAULT=vlt_993de4634508b7d119adc8010781346341a142250aa1df5a20ad53bf0d9d8992
+    DOTENV_VAULT_DEVELOPMENT="BINHFMl8zRRSt5cLMe9BNHDdsH1D5zX45tRrL05WYYbXCuBDsLF2YiAT7VKDdrbk1eg/X5n4FKO76lE1UQ5QTA=="
+    DOTENV_VAULT_CI="nWcJP28Z7w16aBuh9sg/zFACTqWcBXgJnykPNDkF7RqjOwESQDFSO5cymC4="
+    DOTENV_VAULT_STAGING="uGHOx986lAWGU9s5mN5+b0jl0HAvNj4Mqs/zwN7Bl8UeV+C6hBg5JuKdi2AGGLka5g=="
+    DOTENV_VAULT_PRODUCTION="YpDpGGf+eqiOPibziIQQbw4gBW/zfOBR6jow5B1UHYTTu6Kak6xy+qP/vXZWaPp4HOh2/Nu7gRK2CWfrbtk="
+    """
                 
     def test_vault_parsing(self):
         old_dotenv_key = os.environ.get("DOTENV_KEY")
         os.environ["DOTENV_KEY"] = self.PARSE_TEST_KEY
         try:
             stream = vault.parse_vault(StringIO(self.PARSE_TEST_VAULT))
-            dotenv = DotEnv(dotenv_path=".env.vault", stream=stream)
-            self.assertEqual(dotenv.dict().get("HELLO"), "world")
+            load_dotenv(stream=stream, override=True)
+            self.assertEqual(os.environ.get("HELLO"), "Production")
         finally:
             os.unsetenv("DOTENV_KEY")
             if old_dotenv_key:
                 os.environ["DOTENV_KEY"] = old_dotenv_key
```

### Comparing `python-dotenv-vault-0.5.2/src/python_dotenv_vault.egg-info/PKG-INFO` & `python-dotenv-vault-0.6.0/src/python_dotenv_vault.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-dotenv-vault
-Version: 0.5.2
+Version: 0.6.0
 Summary: Decrypt .env.vault file.
 Home-page: https://github.com/dotenv-org/python-dotenv-vault
 Author: dotenv
 Author-email: mot@dotenv.org
 License: MIT
 Keywords: environment,environment variables,deployments,settings,env,dotenv,configurations,python,dotenv-vault
 Description-Content-Type: text/markdown
@@ -170,14 +170,20 @@
 
 # Changelog
 
 All notable changes to this project will be documented in this file. See [standard-version](https://github.com/conventional-changelog/standard-version) for commit guidelines.
 
 ## [Unreleased](https://github.com/dotenv-org/python-dotenv-vault/compare/v0.5.1...master)
 
+## 0.6.0
+
+### Changed
+
+- Fix environment variable load [#12](https://github.com/dotenv-org/python-dotenv-vault/pull/12)
+
 ## 0.5.1
 
 ### Changed
 
 - Fix error reference [#10](https://github.com/dotenv-org/python-dotenv-vault/pull/10)
 
 ## 0.5.0
```

