# Comparing `tmp/msmanager-0.1.0.tar.gz` & `tmp/msmanager-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msmanager-0.1.0.tar", max compression
+gzip compressed data, was "msmanager-0.1.2.tar", max compression
```

## Comparing `msmanager-0.1.0.tar` & `msmanager-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1111 2023-05-14 16:04:08.180554 msmanager-0.1.0/LICENSE
--rw-r--r--   0        0        0      267 2023-05-15 20:57:42.797028 msmanager-0.1.0/msmanager/__init__.py
--rw-r--r--   0        0        0       67 2023-05-15 21:27:48.138274 msmanager-0.1.0/msmanager/__main__.py
--rw-r--r--   0        0        0     3630 2023-05-16 16:41:14.890557 msmanager-0.1.0/msmanager/cli.py
--rw-r--r--   0        0        0     2488 2023-05-15 19:04:10.101041 msmanager-0.1.0/msmanager/config.py
--rw-r--r--   0        0        0     2793 2023-05-15 20:31:27.149266 msmanager-0.1.0/msmanager/exceptions.py
--rw-r--r--   0        0        0     3224 2023-05-16 16:35:54.115596 msmanager-0.1.0/msmanager/functions.py
--rw-r--r--   0        0        0      384 2023-05-16 16:36:36.800666 msmanager-0.1.0/msmanager/models.py
--rw-r--r--   0        0        0     2907 2023-05-15 21:23:04.177803 msmanager-0.1.0/msmanager/msm.py
--rw-r--r--   0        0        0      143 2023-05-15 19:04:10.113824 msmanager-0.1.0/msmanager/types.py
--rw-r--r--   0        0        0      533 2023-05-16 16:50:05.647919 msmanager-0.1.0/msmanager/units.py
--rw-r--r--   0        0        0      547 2023-05-16 16:49:14.197594 msmanager-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      116 2023-05-14 16:04:08.180554 msmanager-0.1.0/README.md
--rw-r--r--   0        0        0      930 1970-01-01 00:00:00.000000 msmanager-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1111 2023-05-14 16:04:08.180554 msmanager-0.1.2/LICENSE
+-rw-r--r--   0        0        0      267 2023-05-15 20:57:42.797028 msmanager-0.1.2/msmanager/__init__.py
+-rw-r--r--   0        0        0       67 2023-05-15 21:27:48.138274 msmanager-0.1.2/msmanager/__main__.py
+-rw-r--r--   0        0        0     4189 2023-05-16 17:48:34.367885 msmanager-0.1.2/msmanager/cli.py
+-rw-r--r--   0        0        0     2488 2023-05-15 19:04:10.101041 msmanager-0.1.2/msmanager/config.py
+-rw-r--r--   0        0        0     2793 2023-05-15 20:31:27.149266 msmanager-0.1.2/msmanager/exceptions.py
+-rw-r--r--   0        0        0     3224 2023-05-16 16:35:54.115596 msmanager-0.1.2/msmanager/functions.py
+-rw-r--r--   0        0        0      384 2023-05-16 16:36:36.800666 msmanager-0.1.2/msmanager/models.py
+-rw-r--r--   0        0        0     2907 2023-05-15 21:23:04.177803 msmanager-0.1.2/msmanager/msm.py
+-rw-r--r--   0        0        0      143 2023-05-15 19:04:10.113824 msmanager-0.1.2/msmanager/types.py
+-rw-r--r--   0        0        0      533 2023-05-16 17:48:52.519457 msmanager-0.1.2/msmanager/units.py
+-rw-r--r--   0        0        0      547 2023-05-16 18:10:12.484055 msmanager-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      484 2023-05-16 18:07:58.584057 msmanager-0.1.2/README.md
+-rw-r--r--   0        0        0     1284 1970-01-01 00:00:00.000000 msmanager-0.1.2/PKG-INFO
```

### Comparing `msmanager-0.1.0/LICENSE` & `msmanager-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `msmanager-0.1.0/msmanager/cli.py` & `msmanager-0.1.2/msmanager/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -59,44 +59,58 @@
         console.print("[green]>[/] Server [bold yellow]started[/]!")
     except Exception as e:
         console.print(rich_exception(e))
 
 # ? Stop Command
 @click.command("stop", help="Stop the server.")
 @click.argument("screen_name", type=str)
-def stoped(screen_name: str):
+def stoper(screen_name: str):
     try:
         msmanager.stop_server(screen_name)
         console.print("[green]>[/] Server [bold yellow]stoped[/]!")
     except Exception as e:
         console.print(rich_exception(e))
 
 # ? List Command
 @click.command("list", help="List of servers in the config.")
-def stoped():
+def lister():
     try:
         if len(msmanager.config.config.servers) != 0:
-            for server in msmanager.config.config.servers:
-                console.print(f"- [green]{repr(server.screen_name)}[/] ([green]{repr(server.executable_filepath)}[/])")
+            for idx, server in enumerate(msmanager.config.config.servers):
+                console.print(
+                    "\n\t".join(
+                        [
+                            f"({idx}) Server [green]{server.screen_name}[/]:",
+                            f"[yellow]EXECUTABLE_FILEPATH[/]: {repr(server.executable_filepath)}",
+                            f"[yellow]ARGUMENTS[/]: {repr(' '.join(server.arguments))}",
+                            f"[yellow]HOST:PORT:INPUT_PORT[/]: [green]{server.host}[/]:{server.port}:{server.input_port}"
+                        ]
+                    )
+                )
         else:
             console.print("[green]>[/] The list of servers is [bold yellow]empty[/]!")
     except Exception as e:
         console.print(rich_exception(e))
 
 # ! Main Group
 @click.group()
-@click.option("--not-check-environment", "not_check_environment", is_flag=True)
+@click.option(
+    "--not-check-environment", "not_check_environment",
+    is_flag=True,
+    help="Disables checks for GNU Screen, Java and system support."
+)
 def main(not_check_environment: bool):
     global msmanager
     msmanager = MSManager(
         check_environment=(not not_check_environment)
     )
 
 # ! Add in Group
 main.add_command(adder)
 main.add_command(remover)
 main.add_command(starter)
-main.add_command(stoped)
+main.add_command(stoper)
+main.add_command(lister)
 
 # ! Run
 def run():
     main()
```

### Comparing `msmanager-0.1.0/msmanager/config.py` & `msmanager-0.1.2/msmanager/config.py`

 * *Files identical despite different names*

### Comparing `msmanager-0.1.0/msmanager/exceptions.py` & `msmanager-0.1.2/msmanager/exceptions.py`

 * *Files identical despite different names*

### Comparing `msmanager-0.1.0/msmanager/functions.py` & `msmanager-0.1.2/msmanager/functions.py`

 * *Files identical despite different names*

### Comparing `msmanager-0.1.0/msmanager/msm.py` & `msmanager-0.1.2/msmanager/msm.py`

 * *Files identical despite different names*

### Comparing `msmanager-0.1.0/msmanager/units.py` & `msmanager-0.1.2/msmanager/units.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 from platformdirs import user_config_dir
 
 # ! Metadata
 __name__ = "msmanager"
-__version__ = "0.1.1"
+__version__ = "0.1.2"
 __author__ = "RCR"
 __email__ = "semina054@gmail.com"
 __url__ = "https://github.com/RCR-OOP/msmanager"
 
 # ! Constants
 SUPPORT_PLATFORMS = [
     "windows-amd64", "windows-x86_64", "linux-x86_64"
```

### Comparing `msmanager-0.1.0/pyproject.toml` & `msmanager-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "msmanager"
-version = "0.1.0"
+version = "0.1.2"
 description = "Manager for managing Mindusrty servers."
 authors = ["Romanin <semina054@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "msmanager"}]
 
 [tool.poetry.dependencies]
```

