# Comparing `tmp/port_forward_manager-3.0.8.tar.gz` & `tmp/port_forward_manager-3.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "port_forward_manager-3.0.8.tar", max compression
+gzip compressed data, was "port_forward_manager-3.0.9.tar", max compression
```

## Comparing `port_forward_manager-3.0.8.tar` & `port_forward_manager-3.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     2346 2022-11-11 17:11:29.313063 port_forward_manager-3.0.8/README.md
--rw-r--r--   0        0        0        0 2022-10-29 11:51:07.229275 port_forward_manager-3.0.8/port_forward_manager/__init__.py
--rw-r--r--   0        0        0     8275 2023-03-26 18:06:46.836138 port_forward_manager-3.0.8/port_forward_manager/cli.py
--rw-r--r--   0        0        0     2112 2023-02-22 15:03:51.449016 port_forward_manager-3.0.8/port_forward_manager/cli_autocomplete.py
--rw-r--r--   0        0        0     3200 2022-12-13 00:00:26.203547 port_forward_manager-3.0.8/port_forward_manager/cli_group.py
--rw-r--r--   0        0        0     7287 2023-02-23 11:38:08.463573 port_forward_manager-3.0.8/port_forward_manager/cli_schema.py
--rw-r--r--   0        0        0     9216 2023-02-23 10:17:19.690244 port_forward_manager-3.0.8/port_forward_manager/cli_session.py
--rw-r--r--   0        0        0     3177 2023-03-25 14:57:03.284196 port_forward_manager-3.0.8/port_forward_manager/cli_ssh_group.py
--rw-r--r--   0        0        0      788 2022-12-13 14:22:32.914417 port_forward_manager-3.0.8/port_forward_manager/database.py
--rw-r--r--   0        0        0     6468 2023-02-23 11:55:41.057803 port_forward_manager-3.0.8/port_forward_manager/forward_sessions.py
--rw-r--r--   0        0        0     9054 2023-03-26 18:04:58.039893 port_forward_manager-3.0.8/port_forward_manager/models.py
--rw-r--r--   0        0        0     1912 2023-03-25 18:39:04.860321 port_forward_manager-3.0.8/port_forward_manager/tools.py
--rw-r--r--   0        0        0      790 2023-03-26 18:07:39.287560 port_forward_manager-3.0.8/pyproject.toml
--rw-r--r--   0        0        0     3343 1970-01-01 00:00:00.000000 port_forward_manager-3.0.8/PKG-INFO
+-rw-r--r--   0        0        0     2346 2022-11-11 17:11:29.313063 port_forward_manager-3.0.9/README.md
+-rw-r--r--   0        0        0        0 2022-10-29 11:51:07.229275 port_forward_manager-3.0.9/port_forward_manager/__init__.py
+-rw-r--r--   0        0        0     8275 2023-03-26 18:06:46.836138 port_forward_manager-3.0.9/port_forward_manager/cli.py
+-rw-r--r--   0        0        0     2112 2023-02-22 15:03:51.449016 port_forward_manager-3.0.9/port_forward_manager/cli_autocomplete.py
+-rw-r--r--   0        0        0     3200 2022-12-13 00:00:26.203547 port_forward_manager-3.0.9/port_forward_manager/cli_group.py
+-rw-r--r--   0        0        0     7287 2023-02-23 11:38:08.463573 port_forward_manager-3.0.9/port_forward_manager/cli_schema.py
+-rw-r--r--   0        0        0     9216 2023-02-23 10:17:19.690244 port_forward_manager-3.0.9/port_forward_manager/cli_session.py
+-rw-r--r--   0        0        0     3187 2023-03-26 18:17:47.080654 port_forward_manager-3.0.9/port_forward_manager/cli_ssh_group.py
+-rw-r--r--   0        0        0      788 2022-12-13 14:22:32.914417 port_forward_manager-3.0.9/port_forward_manager/database.py
+-rw-r--r--   0        0        0     6468 2023-02-23 11:55:41.057803 port_forward_manager-3.0.9/port_forward_manager/forward_sessions.py
+-rw-r--r--   0        0        0     9054 2023-03-26 18:04:58.039893 port_forward_manager-3.0.9/port_forward_manager/models.py
+-rw-r--r--   0        0        0     1912 2023-03-25 18:39:04.860321 port_forward_manager-3.0.9/port_forward_manager/tools.py
+-rw-r--r--   0        0        0      790 2023-03-26 18:18:36.626189 port_forward_manager-3.0.9/pyproject.toml
+-rw-r--r--   0        0        0     3343 1970-01-01 00:00:00.000000 port_forward_manager-3.0.9/PKG-INFO
```

### Comparing `port_forward_manager-3.0.8/README.md` & `port_forward_manager-3.0.9/README.md`

 * *Files identical despite different names*

### Comparing `port_forward_manager-3.0.8/port_forward_manager/cli.py` & `port_forward_manager-3.0.9/port_forward_manager/cli.py`

 * *Files identical despite different names*

### Comparing `port_forward_manager-3.0.8/port_forward_manager/cli_autocomplete.py` & `port_forward_manager-3.0.9/port_forward_manager/cli_autocomplete.py`

 * *Files identical despite different names*

### Comparing `port_forward_manager-3.0.8/port_forward_manager/cli_group.py` & `port_forward_manager-3.0.9/port_forward_manager/cli_group.py`

 * *Files identical despite different names*

### Comparing `port_forward_manager-3.0.8/port_forward_manager/cli_schema.py` & `port_forward_manager-3.0.9/port_forward_manager/cli_schema.py`

 * *Files identical despite different names*

### Comparing `port_forward_manager-3.0.8/port_forward_manager/cli_session.py` & `port_forward_manager-3.0.9/port_forward_manager/cli_session.py`

 * *Files identical despite different names*

### Comparing `port_forward_manager-3.0.8/port_forward_manager/cli_ssh_group.py` & `port_forward_manager-3.0.9/port_forward_manager/cli_ssh_group.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
     return table
 
 
 @app.command()
 def index(name=typer.Argument(None, help='Group name criteria to search')):
     """
-    List groups
+    List SSH groups
     """
     table = prepare_group_table()
     for group in models.SSHGroup.index(name):
         row = [
             str(group.id),
             group.schema.name,
             group.group_name,
@@ -43,15 +43,15 @@
 
 
 @app.command()
 def create(schema_id=typer.Argument(..., help='Schema ID'),
            name=typer.Argument(..., help='Group unique name'),
            label=typer.Argument(..., help='Group label')):
     """
-    Create a group
+    Create SSH group
     """
     schema = models.Schema.find_by_id(schema_id)
     if not schema:
         print(f"Group '{schema_id}' doesn't exist")
         exit(401)
 
     ssh_group = models.SSHGroup(group_name=name, label=label)
@@ -69,15 +69,15 @@
 
 
 @app.command()
 def update(group_id=typer.Argument(..., help="Group ID"),
            name=typer.Option(None, help='Group unique name'),
            label=typer.Option(None, help='Group label')):
     """
-    Update a group
+    Update SSH group
     """
     group = models.SSHGroup.find_by_id(group_id)
     if not group:
         print("Group ID not found")
         exit(401)
 
     if name:
@@ -95,15 +95,15 @@
         message = template.format(type(ex).__name__, ex.args)
         print(message)
 
 
 @app.command()
 def delete(group_id: int = typer.Argument(None, help='Group name'),
            force: bool = typer.Option(False, '-f', help="Force delete")):
-    """Delete session"""
+    """Delete SSH group"""
 
     group = models.SSHGroup.find_by_id(group_id)
     if group is None:
         print(f"Group '{group_id}' not found")
         exit()
 
     if force or Confirm.ask(f"Are you sure you want to delete '{group.label}'?"):
```

### Comparing `port_forward_manager-3.0.8/port_forward_manager/database.py` & `port_forward_manager-3.0.9/port_forward_manager/database.py`

 * *Files identical despite different names*

### Comparing `port_forward_manager-3.0.8/port_forward_manager/forward_sessions.py` & `port_forward_manager-3.0.9/port_forward_manager/forward_sessions.py`

 * *Files identical despite different names*

### Comparing `port_forward_manager-3.0.8/port_forward_manager/models.py` & `port_forward_manager-3.0.9/port_forward_manager/models.py`

 * *Files identical despite different names*

### Comparing `port_forward_manager-3.0.8/port_forward_manager/tools.py` & `port_forward_manager-3.0.9/port_forward_manager/tools.py`

 * *Files identical despite different names*

### Comparing `port_forward_manager-3.0.8/pyproject.toml` & `port_forward_manager-3.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name = "port-forward-managercat "
 [tool.poetry]
 name = "port-forward-manager"
-version = "3.0.8"
+version = "3.0.9"
 description = "Port forwarding manager"
 authors = ["Vladimiro Casinha <vcasinha@kjoo.net>"]
 repository = "https://github.com/kxiros/port-forward-manager"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python="^3.10"
```

### Comparing `port_forward_manager-3.0.8/PKG-INFO` & `port_forward_manager-3.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: port-forward-manager
-Version: 3.0.8
+Version: 3.0.9
 Summary: Port forwarding manager
 Home-page: https://github.com/kxiros/port-forward-manager
 Author: Vladimiro Casinha
 Author-email: vcasinha@kjoo.net
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

