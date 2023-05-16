# Comparing `tmp/pylts-0.0.8.tar.gz` & `tmp/pylts-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylts-0.0.8.tar", max compression
+gzip compressed data, was "pylts-0.0.9.tar", max compression
```

## Comparing `pylts-0.0.8.tar` & `pylts-0.0.9.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0      291 2023-03-01 08:38:37.951816 pylts-0.0.8/README.md
--rw-r--r--   0        0        0       49 2023-03-01 08:45:28.405393 pylts-0.0.8/pylts/__init__.py
--rw-r--r--   0        0        0       32 2023-03-01 08:38:37.954814 pylts-0.0.8/pylts/__main__.py
--rw-r--r--   0        0        0    10187 2023-03-01 09:00:20.131739 pylts-0.0.8/pylts/aws.py
--rw-r--r--   0        0        0      708 2023-03-01 08:38:37.955083 pylts-0.0.8/pylts/cli.py
--rw-r--r--   0        0        0     1536 2023-03-01 08:52:47.749151 pylts-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1060 1970-01-01 00:00:00.000000 pylts-0.0.8/setup.py
--rw-r--r--   0        0        0     1216 1970-01-01 00:00:00.000000 pylts-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      293 2023-05-16 05:28:24.343767 pylts-0.0.9/README.md
+-rw-r--r--   0        0        0       54 2023-05-01 07:09:04.759465 pylts-0.0.9/pylts/__init__.py
+-rw-r--r--   0        0        0       37 2023-05-01 07:07:21.063861 pylts-0.0.9/pylts/__main__.py
+-rw-r--r--   0        0        0    10120 2023-05-01 07:12:03.629215 pylts-0.0.9/pylts/aws.py
+-rw-r--r--   0        0        0     1670 2023-05-01 08:00:44.245976 pylts-0.0.9/pylts/cli.py
+-rw-r--r--   0        0        0     1669 2023-05-16 05:26:03.799749 pylts-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1216 1970-01-01 00:00:00.000000 pylts-0.0.9/PKG-INFO
```

### Comparing `pylts-0.0.8/pylts/aws.py` & `pylts-0.0.9/pylts/aws.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,15 +94,15 @@
         title="AWS Secret Key",
         env="LITESTREAM_SECRET_ACCESS_KEY",
     )
     s3: str = Field(
         default=...,
         repr=True,
         title="s3 URL",
-        description="Should be in the format: s3://bucket/pathname",
+        description="Should be in format: s3://bucket/pathname",
         env="REPLICA_URL",
         regex=r"^s3:\/\/.*$",
         max_length=100,
     )
     folder: Path = Field(
         default=Path(__file__).parent.parent / "data",
         repr=False,
@@ -135,16 +135,15 @@
             Path: Where the database will be located locally.
         """  # noqa: E501
         self.folder.mkdir(exist_ok=True)
         return self.folder / self.db
 
     @property
     def replicate_args(self) -> list[str]:
-        """When used in the command line `litestream replicate <dbpath> <replica_url>`
-        works. As a subprocess, we itemize each item for future use.
+        """Basic args: `litestream replicate <dbpath> <replica_url>` As a subprocess, we itemize each item for future use.
 
         Examples:
             >>> from pylts import ConfigS3
             >>> from pathlib import Path
             >>> # The key, token, s3 are usually just set up in an .env file. They're included here for testing purposes. The folder however is advised to be explicitly declared
             >>> stream = ConfigS3(key="xxx", token="yyy", s3="s3://x/x.db", folder=Path().cwd() / "data")
             >>> args = stream.replicate_args
@@ -158,22 +157,21 @@
             True
             >>> args[3] == stream.s3
             True
         """  # noqa: E501
         return [
             "litestream",
             "replicate",
-            str(self.dbpath),  # path to loca
+            str(self.dbpath),  # path to local
             self.s3,  # where to replicate
         ]
 
     @property
     def restore_args(self) -> list[str]:
-        """When used in the command line `litestream restore -o <dbpath> <replica_url>`
-        works. As a subprocess, we itemize each item for future use.
+        """Basic args: `litestream restore -o <dbpath> <replica_url>`. As a subprocess, we itemize each item for future use.
 
         Examples:
             >>> from pylts import ConfigS3
             >>> from pathlib import Path
             >>> # The key, token, s3 are usually just set up in an .env file. They're included here for testing purposes. The folder however is advised to be explicitly declared
             >>> stream = ConfigS3(key="xxx", token="yyy", s3="s3://x/x.db", folder=Path().cwd() / "data")
             >>> args = stream.restore_args
@@ -197,15 +195,15 @@
             f"{str(self.dbpath)}",  # output path
             self.s3,  # source of restore
         ]
 
     def restore(self) -> Path:
         """Runs the pre-configured litestream command (`@restore_args`) to restore the
         database from the replica url to the constructed database path at `@dbpath`.
-        No need to use a timeout here since after restoration, the command terminates.
+        No need to use a timeout here since, after restoration, the command terminates.
         This is unlike `self.timed_replicate()` which is continuously executed even
         after replication.
         """
         if self.dbpath.exists():
             raise Exception(f"Remove output {self.dbpath=} before restore.")
 
         cmd = {" ".join(self.restore_args)}
```

### Comparing `pylts-0.0.8/pyproject.toml` & `pylts-0.0.9/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "pylts"
 description = "Pydantic wrapper around litestreamed database specific to an AWS bucket."
-version = "0.0.8"
+version = "0.0.9"
 authors = ["Marcelino G. Veloso III <mars@veloso.one>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://mv3.dev"
 repository = "https://github.com/justmars/pylts"
 documentation = "https://justmars.github.io/pylts"
 classifiers = [
@@ -14,36 +14,44 @@
   "Development Status :: 4 - Beta",
   "Framework :: Pytest",
   "Framework :: Pydantic",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.11"
-python-dotenv = "^0.21"
-pydantic = "^1.10.4"
+python-dotenv = "^1.0"
+pydantic = "^1.10.7"
 loguru = "^0.6.0"
 click = "^8.1.3"
 
 [tool.poetry.group.dev.dependencies]
 rich = "^13.3"
-black = "^23.1.0"
-pytest = "^7.2"
+pytest = "^7.3"
 pytest-datadir = "^1.4.1"
 pytest-cov = "^2.12.1"
 pre-commit = "^2.21"
 mkdocs = "^1.4.2"
 mkdocstrings = { extras = ["python"], version = "^0.20.0" }
 mkdocs-material = "^9.0.15"
 ipython = "^8.11.0"
+ipykernel = "^6.22.0"
 
 [tool.pytest]
 minversion = "7.2"
 addopts = "-ra -q --cov=pylts tests/"
 testpaths = ["tests"]
 
+[tool.pytest.ini_options]
+minversion = "7.2"
+addopts = "-ra -q --doctest-modules --cov"
+filterwarnings = [
+  "ignore::DeprecationWarning", # DeprecationWarning: pkg_resources is deprecated as an API
+]
+testpaths = ["tests", "pylts"]
+
 [tool.ruff]
 ignore = ["F401"]
 fixable = ["F", "E", "W", "I001"]
 select = ["F", "E", "W", "I001"]
 
 [tool.black]
 target-version = ['py311']
@@ -59,16 +67,10 @@
     | _build
     | buck-out
     | build
     | dist
 )/
 '''
 
-[tool.isort]
-profile = "black"
-multi_line_output = 3
-line_length = 79
-include_trailing_comma = 'True'
-
 [build-system]
 requires = ["poetry-core>=1.3.2"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pylts-0.0.8/PKG-INFO` & `pylts-0.0.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylts
-Version: 0.0.8
+Version: 0.0.9
 Summary: Pydantic wrapper around litestreamed database specific to an AWS bucket.
 Home-page: https://mv3.dev
 License: MIT
 Author: Marcelino G. Veloso III
 Author-email: mars@veloso.one
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -13,27 +13,27 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: loguru (>=0.6.0,<0.7.0)
-Requires-Dist: pydantic (>=1.10.4,<2.0.0)
-Requires-Dist: python-dotenv (>=0.21,<0.22)
+Requires-Dist: pydantic (>=1.10.7,<2.0.0)
+Requires-Dist: python-dotenv (>=1.0,<2.0)
 Project-URL: Documentation, https://justmars.github.io/pylts
 Project-URL: Repository, https://github.com/justmars/pylts
 Description-Content-Type: text/markdown
 
 # pylts
 
 ![Github CI](https://github.com/justmars/pylts/actions/workflows/main.yml/badge.svg)
 
 Pydantic wrapper around litestreamed database specific to an AWS bucket.
 
 ## Development
 
 See [documentation](https://mv3.dev/pylts).
 
-1. Run `poetry shell`
+1. Run `poetry install`
 2. Run `poetry update`
 3. Run `pytest`
```

