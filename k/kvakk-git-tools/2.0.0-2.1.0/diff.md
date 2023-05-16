# Comparing `tmp/kvakk_git_tools-2.0.0.tar.gz` & `tmp/kvakk_git_tools-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kvakk_git_tools-2.0.0.tar", max compression
+gzip compressed data, was "kvakk_git_tools-2.1.0.tar", max compression
```

## Comparing `kvakk_git_tools-2.0.0.tar` & `kvakk_git_tools-2.1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1074 2023-05-16 07:37:32.216724 kvakk_git_tools-2.0.0/LICENSE
--rw-r--r--   0        0        0     2279 2023-05-16 07:37:32.216724 kvakk_git_tools-2.0.0/README.md
--rw-r--r--   0        0        0      134 2023-05-16 07:37:32.216724 kvakk_git_tools-2.0.0/kvakk_git_tools/__init__.py
--rw-r--r--   0        0        0       64 2023-05-16 07:37:32.216724 kvakk_git_tools-2.0.0/kvakk_git_tools/recommended/gitattributes
--rw-r--r--   0        0        0      215 2023-05-16 07:37:32.216724 kvakk_git_tools-2.0.0/kvakk_git_tools/recommended/gitconfig-adm-mac
--rw-r--r--   0        0        0      515 2023-05-16 07:37:32.216724 kvakk_git_tools-2.0.0/kvakk_git_tools/recommended/gitconfig-dapla
--rw-r--r--   0        0        0      645 2023-05-16 07:37:32.220724 kvakk_git_tools-2.0.0/kvakk_git_tools/recommended/gitconfig-prod-linux
--rw-r--r--   0        0        0      472 2023-05-16 07:37:32.220724 kvakk_git_tools-2.0.0/kvakk_git_tools/recommended/gitconfig-prod-windows-citrix
--rw-r--r--   0        0        0     4656 2023-05-16 07:37:32.220724 kvakk_git_tools-2.0.0/kvakk_git_tools/recommended/gitignore
--rwxr-xr-x   0        0        0    10623 2023-05-16 07:37:32.220724 kvakk_git_tools-2.0.0/kvakk_git_tools/ssb_gitconfig.py
--rw-r--r--   0        0        0     2061 2023-05-16 07:37:32.220724 kvakk_git_tools-2.0.0/kvakk_git_tools/validate_ssb_gitconfig.py
--rw-r--r--   0        0        0      985 2023-05-16 07:37:32.220724 kvakk_git_tools-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     2773 1970-01-01 00:00:00.000000 kvakk_git_tools-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-05-16 10:14:58.907124 kvakk_git_tools-2.1.0/LICENSE
+-rw-r--r--   0        0        0     2972 2023-05-16 10:14:58.907124 kvakk_git_tools-2.1.0/README.md
+-rw-r--r--   0        0        0      134 2023-05-16 10:14:58.907124 kvakk_git_tools-2.1.0/kvakk_git_tools/__init__.py
+-rw-r--r--   0        0        0       64 2023-05-16 10:14:58.907124 kvakk_git_tools-2.1.0/kvakk_git_tools/recommended/gitattributes
+-rw-r--r--   0        0        0      215 2023-05-16 10:14:58.907124 kvakk_git_tools-2.1.0/kvakk_git_tools/recommended/gitconfig-adm-mac
+-rw-r--r--   0        0        0      515 2023-05-16 10:14:58.907124 kvakk_git_tools-2.1.0/kvakk_git_tools/recommended/gitconfig-dapla
+-rw-r--r--   0        0        0      645 2023-05-16 10:14:58.907124 kvakk_git_tools-2.1.0/kvakk_git_tools/recommended/gitconfig-prod-linux
+-rw-r--r--   0        0        0      472 2023-05-16 10:14:58.907124 kvakk_git_tools-2.1.0/kvakk_git_tools/recommended/gitconfig-prod-windows-citrix
+-rw-r--r--   0        0        0     4656 2023-05-16 10:14:58.907124 kvakk_git_tools-2.1.0/kvakk_git_tools/recommended/gitignore
+-rwxr-xr-x   0        0        0    12528 2023-05-16 10:14:58.907124 kvakk_git_tools-2.1.0/kvakk_git_tools/ssb_gitconfig.py
+-rw-r--r--   0        0        0     2061 2023-05-16 10:14:58.907124 kvakk_git_tools-2.1.0/kvakk_git_tools/validate_ssb_gitconfig.py
+-rw-r--r--   0        0        0     1003 2023-05-16 10:14:58.911124 kvakk_git_tools-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3466 1970-01-01 00:00:00.000000 kvakk_git_tools-2.1.0/PKG-INFO
```

### Comparing `kvakk_git_tools-2.0.0/LICENSE` & `kvakk_git_tools-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kvakk_git_tools-2.0.0/README.md` & `kvakk_git_tools-2.1.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -8,44 +8,44 @@
 
 Initially the repo will contain a collection of git configurations for the different
 environments. But the aim is to make a common script, setting up the recommended
 git config for all SSB platforms, based on the detected environment.
 
 ## Status
 
-The `ssb-gitconfig.py` script works and is tested on the following platforms:
+The `ssb_gitconfig.py` script works and is tested on the following platforms:
 
 - Dapla
 - Production zone, Linux (including Jupyter)
 - Production zone, Windows (Citrix)
 
 ## Directories
 
 The `existing` directory contains configurations collected from existing environments
 before any recommendations are implemented. The `recommended` directory contains the
 recommended config files for the different environments.
 
-The `ssb-gitconfig` directory is the root directory for the script that should
+The `ssb_gitconfig` directory is the root directory for the script that should
 set the ssb recommended git config based on the detected environment. It is a
 work in progress and not finished yet.
 
 ## Usage
 
 Linux and Mac OS:
 
 ```shell
 git clone https://github.com/statisticsnorway/kvakk-git-tools.git
-kvakk-git-tools/ssb-gitconfig/src/ssb-gitconfig.py
+kvakk-git-tools/kvakk_git_tools/ssb_gitconfig.py
 ```
 
 Windows:
 
 ```shell
 git clone https://github.com/statisticsnorway/kvakk-git-tools.git
-python kvakk-git-tools\ssb-gitconfig\src\ssb-gitconfig.py
+python kvakk-git-tools\kvakk_git_tools\ssb_gitconfig.py
 ```
 
 ## Developer guide
 
 ### Initial setup
 
 The Poetry tool is used for dependency management. Install poetry as described on the
@@ -68,9 +68,25 @@
 ### Linting
 
 You can do local linting with the following commands:
 
 ```shell
 poetry run flake8
 poetry run mypy .
-poetry run pylint ssb-gitconfig/ssb-gitconfig.py
+poetry run pylint kvakk_git_tools/*.py
 ```
+
+### Bumping version
+
+Use `make` to bump the _patch_, _minor_ version or _major_ version before creating a pull request to the `main` GIT
+branch.
+
+You can use either `bump-version-patch`, `bump-version-minor`, or `bump-version-major`.
+Bumping must be done with a clean git working space, and automatically commits with the new version number.
+
+Then just run `git push origin --tags` to push the changes and trigger the release process.
+
+### Building and releasing
+
+Before merging your changes into the `main` branch, make sure you have bumped the version like outlined above.
+
+An automatic release process will build _kvakk-git-tools_ and release a new version of the package to **pypi.org** automatically.
```

### Comparing `kvakk_git_tools-2.0.0/kvakk_git_tools/recommended/gitconfig-dapla` & `kvakk_git_tools-2.1.0/kvakk_git_tools/recommended/gitconfig-dapla`

 * *Files identical despite different names*

### Comparing `kvakk_git_tools-2.0.0/kvakk_git_tools/recommended/gitconfig-prod-linux` & `kvakk_git_tools-2.1.0/kvakk_git_tools/recommended/gitconfig-prod-linux`

 * *Files identical despite different names*

### Comparing `kvakk_git_tools-2.0.0/kvakk_git_tools/recommended/gitignore` & `kvakk_git_tools-2.1.0/kvakk_git_tools/recommended/gitignore`

 * *Files identical despite different names*

### Comparing `kvakk_git_tools-2.0.0/kvakk_git_tools/ssb_gitconfig.py` & `kvakk_git_tools-2.1.0/kvakk_git_tools/ssb_gitconfig.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,29 +5,31 @@
 https://github.com/statisticsnorway/kvakk-git-tools.git. The script clones this
 repo and selects the base git config based on the detected platform.
 
 If there is an existing .gitconfig file, it is backed up, and the name and email
 address are extracted from it and reused.
 """
 
-__version__ = "1.0.4"
+__version__ = "2.1.0"
 
 import argparse
 import getpass
 import os
 import platform
 import shutil
 import stat
 import subprocess
 import sys
 from datetime import datetime
 from enum import Enum
 from pathlib import Path
 from typing import Optional, Tuple
 
+import pkg_resources
+
 
 def ping(host: str) -> bool:
     """Returns True if host responds to a ping request."""
     # Option for the number of packets is different on Windows and Linux
     ping_param = "-n" if platform.system() == "Windows" else "-c"
 
     # Timeout is -w <milliseconds> on Windows, and -W <seconds> on Linux
@@ -213,15 +215,15 @@
     temp_dir = Path.home() / "temp-ssb-gitconfig"
     config_dir = temp_dir / "kvakk-git-tools" / "kvakk_git_tools" / "recommended"
     dst = Path().home() / ".gitconfig"
     src = config_dir / f"gitconfig-{pl.name().value}"
     if test:
         src = config_dir / "gitconfig-dapla"
 
-    options = ["--branch", "v2.0.0"]
+    options = ["--branch", "2.1.0"]
     prod_zone_windows = pl.name() is PlatformName.PROD_WINDOWS_CITRIX
     prod_zone_linux = pl.name() is PlatformName.PROD_LINUX
     if prod_zone_windows or prod_zone_linux:
         options = ["-c", "http.sslVerify=False"]
 
     cmd = (
         ["git"]
@@ -290,26 +292,83 @@
     if (
         sys.version_info.major == 3 and sys.version_info.minor < 6
     ) or sys.version_info.major < 3:
         print("This script requires python version >= 3.6")
         sys.exit(1)
 
 
+def kvakk_git_tools_package_installed() -> bool:
+    """Checks if the kvakk_git_tools package is installed on the system.
+
+    Returns:
+        bool: True if the package is installed, False otherwise.
+    """
+    try:
+        pkg_resources.get_distribution("kvakk_git_tools")
+        return True
+    except pkg_resources.DistributionNotFound:
+        return False
+
+
+def enable_additional_package_arguments(
+    parser: argparse.ArgumentParser, enable: bool
+) -> None:
+    """Enables packages specific arguments in the given ArgumentParser object.
+
+    Args:
+        parser (argparse.ArgumentParser): The ArgumentParser object.
+        enable (bool): Indicates whether to enable the additional arguments.
+    """
+    if enable:
+        parser.add_argument(
+            "--validate",
+            action="store_true",
+            help="Validates SSB gitconfig for your current platform",
+        )
+
+
+def parse_optional_validation_argument(validate: bool):
+    """Parses the optional validation argument and performs SSB Git configuration validation.
+
+    Args:
+        validate (bool): Indicates whether to perform the validation.
+    """
+    if validate:
+        from kvakk_git_tools.validate_ssb_gitconfig import validate_git_config
+
+        if validate_git_config():
+            print("Git configuration follows SSB recommendations.")
+            exit(0)
+        else:
+            print(
+                "WARNING: Git configuration does not follow SSB recommendations."
+                "\nThis can lead to sensitive information being pushed to Git."
+                "\nYou can fix this by running: 'kvakk-git-tools' in your terminal."
+            )
+            exit(1)
+
+
 def run() -> None:
     check_python_version()
 
     parser = argparse.ArgumentParser(description=sys.modules[__name__].__doc__)
     parser.add_argument(
         "--test", action="store_true", help="used when testing the script"
     )
     parser.add_argument(
         "--version", action="store_true", help="print he version number of the script"
     )
+    package_installed = kvakk_git_tools_package_installed()
+    enable_additional_package_arguments(parser, package_installed)
+
     args = parser.parse_args()
 
+    if package_installed:
+        parse_optional_validation_argument(args.validate)
+
     if args.version:
         print(f"ssb_gitconfig version: {__version__}")
     else:
         main(args.test)
 
 
 if __name__ == "__main__":
```

### Comparing `kvakk_git_tools-2.0.0/kvakk_git_tools/validate_ssb_gitconfig.py` & `kvakk_git_tools-2.1.0/kvakk_git_tools/validate_ssb_gitconfig.py`

 * *Files identical despite different names*

### Comparing `kvakk_git_tools-2.0.0/pyproject.toml` & `kvakk_git_tools-2.1.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kvakk-git-tools"
-version = "2.0.0"
+version = "2.1.0"
 description = "Recommended git config and git scripts for Statistics Norway."
 authors = ["Arne Sørli <81353974+arneso-ssb@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "kvakk_git_tools" }]
 
 [tool.poetry.scripts]
@@ -22,14 +22,15 @@
 flake8-docstrings = "^1.6.0"
 isort = "^5.10.1"
 mypy = "^0.991"
 pre-commit = "^2.20.0"
 pre-commit-hooks = "^4.3.0"
 pylint = "^2.15.3"
 bump2version = "*"
+pytest = "^7.3.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 profile = "black"
```

### Comparing `kvakk_git_tools-2.0.0/PKG-INFO` & `kvakk_git_tools-2.1.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kvakk-git-tools
-Version: 2.0.0
+Version: 2.1.0
 Summary: Recommended git config and git scripts for Statistics Norway.
 License: MIT
 Author: Arne Sørli
 Author-email: 81353974+arneso-ssb@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -22,44 +22,44 @@
 
 Initially the repo will contain a collection of git configurations for the different
 environments. But the aim is to make a common script, setting up the recommended
 git config for all SSB platforms, based on the detected environment.
 
 ## Status
 
-The `ssb-gitconfig.py` script works and is tested on the following platforms:
+The `ssb_gitconfig.py` script works and is tested on the following platforms:
 
 - Dapla
 - Production zone, Linux (including Jupyter)
 - Production zone, Windows (Citrix)
 
 ## Directories
 
 The `existing` directory contains configurations collected from existing environments
 before any recommendations are implemented. The `recommended` directory contains the
 recommended config files for the different environments.
 
-The `ssb-gitconfig` directory is the root directory for the script that should
+The `ssb_gitconfig` directory is the root directory for the script that should
 set the ssb recommended git config based on the detected environment. It is a
 work in progress and not finished yet.
 
 ## Usage
 
 Linux and Mac OS:
 
 ```shell
 git clone https://github.com/statisticsnorway/kvakk-git-tools.git
-kvakk-git-tools/ssb-gitconfig/src/ssb-gitconfig.py
+kvakk-git-tools/kvakk_git_tools/ssb_gitconfig.py
 ```
 
 Windows:
 
 ```shell
 git clone https://github.com/statisticsnorway/kvakk-git-tools.git
-python kvakk-git-tools\ssb-gitconfig\src\ssb-gitconfig.py
+python kvakk-git-tools\kvakk_git_tools\ssb_gitconfig.py
 ```
 
 ## Developer guide
 
 ### Initial setup
 
 The Poetry tool is used for dependency management. Install poetry as described on the
@@ -82,10 +82,26 @@
 ### Linting
 
 You can do local linting with the following commands:
 
 ```shell
 poetry run flake8
 poetry run mypy .
-poetry run pylint ssb-gitconfig/ssb-gitconfig.py
+poetry run pylint kvakk_git_tools/*.py
 ```
 
+### Bumping version
+
+Use `make` to bump the _patch_, _minor_ version or _major_ version before creating a pull request to the `main` GIT
+branch.
+
+You can use either `bump-version-patch`, `bump-version-minor`, or `bump-version-major`.
+Bumping must be done with a clean git working space, and automatically commits with the new version number.
+
+Then just run `git push origin --tags` to push the changes and trigger the release process.
+
+### Building and releasing
+
+Before merging your changes into the `main` branch, make sure you have bumped the version like outlined above.
+
+An automatic release process will build _kvakk-git-tools_ and release a new version of the package to **pypi.org** automatically.
+
```

