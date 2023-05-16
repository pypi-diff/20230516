# Comparing `tmp/jcloud-0.2.8.dev2.tar.gz` & `tmp/jcloud-0.2.9.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jcloud-0.2.8.dev2.tar", last modified: Mon May  8 14:57:54 2023, max compression
+gzip compressed data, was "jcloud-0.2.9.dev3.tar", last modified: Tue May 16 08:49:54 2023, max compression
```

## Comparing `jcloud-0.2.8.dev2.tar` & `jcloud-0.2.9.dev3.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:57:54.342459 jcloud-0.2.8.dev2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-08 14:57:48.000000 jcloud-0.2.8.dev2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-08 14:57:48.000000 jcloud-0.2.8.dev2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-05-08 14:57:54.342459 jcloud-0.2.8.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-05-08 14:57:48.000000 jcloud-0.2.8.dev2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:57:54.342459 jcloud-0.2.8.dev2/jcloud/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-08 14:57:54.000000 jcloud-0.2.8.dev2/jcloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-08 14:57:48.000000 jcloud-0.2.8.dev2/jcloud/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12612 2023-05-08 14:57:48.000000 jcloud-0.2.8.dev2/jcloud/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-08 14:57:48.000000 jcloud-0.2.8.dev2/jcloud/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     9458 2023-05-08 14:57:48.000000 jcloud-0.2.8.dev2/jcloud/env_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    21449 2023-05-08 14:57:48.000000 jcloud-0.2.8.dev2/jcloud/flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     8466 2023-05-08 14:57:48.000000 jcloud-0.2.8.dev2/jcloud/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    10350 2023-05-08 14:57:48.000000 jcloud-0.2.8.dev2/jcloud/normalize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:57:54.342459 jcloud-0.2.8.dev2/jcloud/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-05-08 14:57:48.000000 jcloud-0.2.8.dev2/jcloud/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-08 14:57:48.000000 jcloud-0.2.8.dev2/jcloud/parsers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-05-08 14:57:48.000000 jcloud-0.2.8.dev2/jcloud/parsers/custom_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-08 14:57:48.000000 jcloud-0.2.8.dev2/jcloud/parsers/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     8898 2023-05-08 14:57:48.000000 jcloud-0.2.8.dev2/jcloud/parsers/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-08 14:57:48.000000 jcloud-0.2.8.dev2/jcloud/parsers/list.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-08 14:57:48.000000 jcloud-0.2.8.dev2/jcloud/parsers/normalize.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-08 14:57:48.000000 jcloud-0.2.8.dev2/jcloud/parsers/remove.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-08 14:57:48.000000 jcloud-0.2.8.dev2/jcloud/parsers/status.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-08 14:57:48.000000 jcloud-0.2.8.dev2/jcloud/parsers/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:57:54.338459 jcloud-0.2.8.dev2/jcloud/resources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:57:54.342459 jcloud-0.2.8.dev2/jcloud/resources/project-template/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 14:57:48.000000 jcloud-0.2.8.dev2/jcloud/resources/project-template/.env
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:57:54.342459 jcloud-0.2.8.dev2/jcloud/resources/project-template/executor1/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-08 14:57:48.000000 jcloud-0.2.8.dev2/jcloud/resources/project-template/executor1/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-08 14:57:48.000000 jcloud-0.2.8.dev2/jcloud/resources/project-template/executor1/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 14:57:48.000000 jcloud-0.2.8.dev2/jcloud/resources/project-template/executor1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-08 14:57:48.000000 jcloud-0.2.8.dev2/jcloud/resources/project-template/flow.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-05-08 14:57:48.000000 jcloud-0.2.8.dev2/jcloud/survey.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:57:54.342459 jcloud-0.2.8.dev2/jcloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-05-08 14:57:54.000000 jcloud-0.2.8.dev2/jcloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-08 14:57:54.000000 jcloud-0.2.8.dev2/jcloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 14:57:54.000000 jcloud-0.2.8.dev2/jcloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-08 14:57:54.000000 jcloud-0.2.8.dev2/jcloud.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 14:57:54.000000 jcloud-0.2.8.dev2/jcloud.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-08 14:57:54.000000 jcloud-0.2.8.dev2/jcloud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-08 14:57:54.000000 jcloud-0.2.8.dev2/jcloud.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-08 14:57:48.000000 jcloud-0.2.8.dev2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 14:57:54.342459 jcloud-0.2.8.dev2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-05-08 14:57:48.000000 jcloud-0.2.8.dev2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:49:54.976805 jcloud-0.2.9.dev3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-16 08:49:50.000000 jcloud-0.2.9.dev3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-16 08:49:50.000000 jcloud-0.2.9.dev3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-05-16 08:49:54.976805 jcloud-0.2.9.dev3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-05-16 08:49:50.000000 jcloud-0.2.9.dev3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:49:54.972805 jcloud-0.2.9.dev3/jcloud/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-16 08:49:54.000000 jcloud-0.2.9.dev3/jcloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-16 08:49:50.000000 jcloud-0.2.9.dev3/jcloud/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13760 2023-05-16 08:49:50.000000 jcloud-0.2.9.dev3/jcloud/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-16 08:49:50.000000 jcloud-0.2.9.dev3/jcloud/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9458 2023-05-16 08:49:50.000000 jcloud-0.2.9.dev3/jcloud/env_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22050 2023-05-16 08:49:50.000000 jcloud-0.2.9.dev3/jcloud/flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8756 2023-05-16 08:49:50.000000 jcloud-0.2.9.dev3/jcloud/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10350 2023-05-16 08:49:50.000000 jcloud-0.2.9.dev3/jcloud/normalize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:49:54.976805 jcloud-0.2.9.dev3/jcloud/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-05-16 08:49:50.000000 jcloud-0.2.9.dev3/jcloud/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-16 08:49:50.000000 jcloud-0.2.9.dev3/jcloud/parsers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-05-16 08:49:50.000000 jcloud-0.2.9.dev3/jcloud/parsers/custom_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-16 08:49:50.000000 jcloud-0.2.9.dev3/jcloud/parsers/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8898 2023-05-16 08:49:50.000000 jcloud-0.2.9.dev3/jcloud/parsers/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-16 08:49:50.000000 jcloud-0.2.9.dev3/jcloud/parsers/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-16 08:49:50.000000 jcloud-0.2.9.dev3/jcloud/parsers/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-16 08:49:50.000000 jcloud-0.2.9.dev3/jcloud/parsers/normalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-16 08:49:50.000000 jcloud-0.2.9.dev3/jcloud/parsers/remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-16 08:49:50.000000 jcloud-0.2.9.dev3/jcloud/parsers/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-16 08:49:50.000000 jcloud-0.2.9.dev3/jcloud/parsers/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:49:54.972805 jcloud-0.2.9.dev3/jcloud/resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:49:54.976805 jcloud-0.2.9.dev3/jcloud/resources/project-template/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 08:49:50.000000 jcloud-0.2.9.dev3/jcloud/resources/project-template/.env
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:49:54.976805 jcloud-0.2.9.dev3/jcloud/resources/project-template/executor1/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-16 08:49:50.000000 jcloud-0.2.9.dev3/jcloud/resources/project-template/executor1/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-16 08:49:50.000000 jcloud-0.2.9.dev3/jcloud/resources/project-template/executor1/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 08:49:50.000000 jcloud-0.2.9.dev3/jcloud/resources/project-template/executor1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-16 08:49:50.000000 jcloud-0.2.9.dev3/jcloud/resources/project-template/flow.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-05-16 08:49:50.000000 jcloud-0.2.9.dev3/jcloud/survey.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:49:54.972805 jcloud-0.2.9.dev3/jcloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-05-16 08:49:54.000000 jcloud-0.2.9.dev3/jcloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-16 08:49:54.000000 jcloud-0.2.9.dev3/jcloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 08:49:54.000000 jcloud-0.2.9.dev3/jcloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-16 08:49:54.000000 jcloud-0.2.9.dev3/jcloud.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 08:49:54.000000 jcloud-0.2.9.dev3/jcloud.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-16 08:49:54.000000 jcloud-0.2.9.dev3/jcloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-16 08:49:54.000000 jcloud-0.2.9.dev3/jcloud.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-16 08:49:50.000000 jcloud-0.2.9.dev3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 08:49:54.976805 jcloud-0.2.9.dev3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-05-16 08:49:50.000000 jcloud-0.2.9.dev3/setup.py
```

### Comparing `jcloud-0.2.8.dev2/LICENSE` & `jcloud-0.2.9.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `jcloud-0.2.8.dev2/PKG-INFO` & `jcloud-0.2.9.dev3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jcloud
-Version: 0.2.8.dev2
+Version: 0.2.9.dev3
 Summary: Simplify deploying and managing Jina projects on Jina Cloud
 Home-page: https://github.com/jina-ai/jcloud
 Author: Jina AI
 Author-email: hello@jina.ai
 License: Apache 2.0
 Download-URL: https://github.com/jina-ai/jcloud/tags
 Project-URL: Documentation, https://jcloud.jina.ai
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: jcloud Version: 0.2.8.dev2 Summary: Simplify
+Metadata-Version: 2.1 Name: jcloud Version: 0.2.9.dev3 Summary: Simplify
 deploying and managing Jina projects on Jina Cloud Home-page: https://
 github.com/jina-ai/jcloud Author: Jina AI Author-email: hello@jina.ai License:
 Apache 2.0 Download-URL: https://github.com/jina-ai/jcloud/tags Project-URL:
 Documentation, https://jcloud.jina.ai Project-URL: Source, https://github.com/
 jina-ai/jcloud/ Project-URL: Tracker, https://github.com/jina-ai/jcloud/issues
 Keywords: jcloud neural-search serverless deployment devops mlops Platform:
 UNKNOWN Classifier: Development Status :: 5 - Production/Stable Classifier:
```

### Comparing `jcloud-0.2.8.dev2/README.md` & `jcloud-0.2.9.dev3/README.md`

 * *Files identical despite different names*

### Comparing `jcloud-0.2.8.dev2/jcloud/__main__.py` & `jcloud-0.2.9.dev3/jcloud/__main__.py`

 * *Files identical despite different names*

### Comparing `jcloud-0.2.8.dev2/jcloud/api.py` & `jcloud-0.2.9.dev3/jcloud/api.py`

 * *Files 16% similar despite different names*

```diff
@@ -33,116 +33,106 @@
 def normalize(args):
     flow_normalize(path=args.path, verbose=args.verbose, output_path=args.output)
 
 
 @asyncify
 async def status(args):
     from rich import box
-    from rich.align import Align
     from rich.console import Console
     from rich.json import JSON
     from rich.syntax import Syntax
     from rich.table import Table
 
-    from .helper import CustomHighlighter
+    from .helper import CustomHighlighter, add_table_row_fn, center_align
 
     _t = Table(
         'Attribute',
         'Value',
         show_header=False,
         box=box.ROUNDED,
         highlight=True,
         show_lines=True,
     )
 
-    def _add_row_fn(key, value):
-        return lambda: _t.add_row(Align(f'[bold]{key}', vertical='middle'), value)
-
-    def _center_align(value):
-        return Align(f'[bold]{value}[/bold]', align='center')
-
     console = Console(highlighter=CustomHighlighter())
     with console.status(f'[bold]Fetching status of [green]{args.flow}[/green] ...'):
         _result = await CloudFlow(flow_id=args.flow).status
         if not _result:
             console.print(
                 f'[red]Something went wrong while fetching the details for {args.flow} ![/red]. Please retry after sometime.'
             )
         else:
             _other_rows = []
             for k, v in _result.items():
                 if k == 'id':
-                    _id_row = _add_row_fn(
-                        'ID', Align(f'[bold]{v}[/bold]', align='center')
-                    )
+                    _id_row = add_table_row_fn(_t, 'ID', center_align(v))
 
                 elif k == 'status':
                     for _k, _v in v.items():
                         if _k == 'phase':
                             # Show Phase
-                            _phase_row = _add_row_fn('Phase', _center_align(_v))
+                            _phase_row = add_table_row_fn(_t, 'Phase', center_align(_v))
 
                         elif _k == 'endpoints' and _v:
                             # Show Endpoints and Dashboards
                             _other_rows.append(
-                                _add_row_fn("Endpoint(s)", JSON(jsonify(_v)))
+                                add_table_row_fn(_t, 'Endpoint(s)', JSON(jsonify(_v)))
                             )
 
                         elif _k == 'dashboards' and _v:
                             # Show Dashboard
                             if _v.get('grafana'):
                                 _other_rows.append(
-                                    _add_row_fn(
+                                    add_table_row_fn(
+                                        _t,
                                         'Grafana Dashboard',
-                                        _center_align(_v.get('grafana')),
+                                        center_align(_v.get('grafana')),
                                     )
                                 )
                             else:
                                 _other_rows.append(
-                                    _add_row_fn(
-                                        'Dashboards',
-                                        _v,
-                                    )
+                                    add_table_row_fn(_t, 'Dashboards', _v)
                                 )
 
                         elif _k == 'conditions' and args.verbose:
                             # Show Conditions only if verbose
                             _other_rows.append(
-                                _add_row_fn('Details', JSON(jsonify(_v)))
+                                add_table_row_fn(_t, 'Details', JSON(jsonify(_v)))
                             )
 
                         elif _k == 'version' and args.verbose:
                             # Show Jina version only if verbose
                             _other_rows.append(
-                                _add_row_fn("Jina Version", _center_align(_v))
+                                add_table_row_fn(_t, 'Jina Version', center_align(_v))
                             )
 
                 elif k == 'spec' and v is not None:
                     v = Syntax(
                         yamlify(v),
                         'yaml',
                         theme='monokai',
                         line_numbers=1,
                         code_width=60,
                     )
-                    _other_rows.append(_add_row_fn('Spec', v))
+                    _other_rows.append(add_table_row_fn(_t, 'Spec', v))
 
                 elif k == 'CPH' and v:
                     _other_rows.append(
-                        _add_row_fn("Credits Per Hour", JSON(jsonify(v)))
+                        add_table_row_fn(_t, 'Credits Per Hour', JSON(jsonify(v)))
                     )
 
                 elif k == 'error' and v:
-                    _other_rows.append(_add_row_fn(k, f'[red]{v}[red]'))
+                    _other_rows.append(add_table_row_fn(_t, k, f'[red]{v}[red]'))
 
                 elif k in ('ctime', 'utime'):
                     _other_rows.append(
-                        _add_row_fn(
+                        add_table_row_fn(
+                            _t,
                             'Created' if k == 'ctime' else 'Updated',
-                            _center_align(cleanup_dt(v)),
+                            center_align(cleanup_dt(v)),
                         ),
                     )
 
             for fn in [_id_row, _phase_row, *_other_rows]:
                 fn()
             console.print(_t)
 
@@ -403,7 +393,55 @@
 @asyncify
 async def recreate(args):
     from rich import print
 
     print(f'Recreating deleted Flow [green]{args.flow}[/green]')
 
     await CloudFlow(flow_id=args.flow).recreate()
+
+
+@asyncify
+async def logs(args):
+    from rich import print
+    from rich import box
+    from rich.console import Console
+    from rich.syntax import Syntax
+    from rich.table import Table
+
+    from .helper import add_table_row_fn, center_align
+
+    _t = Table(
+        'Attribute',
+        'Value',
+        show_header=False,
+        box=box.ROUNDED,
+        show_lines=True,
+    )
+
+    name = 'gateway' if args.gateway else f'executor {args.executor}'
+    print(f'Fetching the logs for {name} of the Flow: [green]{args.flow}[/green]')
+
+    if args.gateway:
+        logs = await CloudFlow(flow_id=args.flow).logs()
+    else:
+        logs = await CloudFlow(flow_id=args.flow).logs(args.executor)
+
+    console = Console()
+    for pod, pod_logs in logs.items():
+        with console.status(f'[bold]Displaying logs of pod [green]{pod}[/green]...'):
+            _pod_id_row = add_table_row_fn(_t, 'POD_ID', center_align(pod))
+
+            _pod_logs_lines = '\n'.join(pod_logs.split('\n'))
+            _pod_logs_row = add_table_row_fn(
+                _t,
+                'Logs',
+                Syntax(
+                    _pod_logs_lines,
+                    lexer='vctreestatus',
+                    line_numbers=1,
+                    code_width=90,
+                ),
+            )
+
+            for fn in [_pod_id_row, _pod_logs_row]:
+                fn()
+            console.print(_t)
```

### Comparing `jcloud-0.2.8.dev2/jcloud/constants.py` & `jcloud-0.2.9.dev3/jcloud/constants.py`

 * *Files identical despite different names*

### Comparing `jcloud-0.2.8.dev2/jcloud/env_helper.py` & `jcloud-0.2.9.dev3/jcloud/env_helper.py`

 * *Files identical despite different names*

### Comparing `jcloud-0.2.8.dev2/jcloud/flow.py` & `jcloud-0.2.9.dev3/jcloud/flow.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,26 +37,33 @@
 ):
     if response.status != expected_status:
         if response.status == HTTPStatus.UNAUTHORIZED:
             _exit_error(
                 'You are not logged in, please login using [b]jcloud login[/b] first.'
             )
         elif response.status == HTTPStatus.FORBIDDEN:
-            print(
-                f'Got an error from the server: [red]{json_response.get("error")}[/red]'
+            print_server_resposne(json_response['error'])
+            _exit_error(
+                f'Please make sure your account is activated and funded or that you own the requested flow.'
             )
-            _exit_error(f'Please make sure your account is activated and funded.')
+        elif response.status == HTTPStatus.NOT_FOUND:
+            print_server_resposne(json_response['error'])
+            _exit_error(f'Please make sure the requested resource exists.')
         else:
             _exit_error(
                 f'Bad response: expecting [b]{expected_status}[/b], got [b]{response.status}[/b] from server.\n'
                 f'{json.dumps(json_response, indent=1)}'
             )
 
 
-def _exit_error(text):
+def print_server_resposne(error_message: str):
+    print(f'Got an error from the server: [red]{error_message}[/red]')
+
+
+def _exit_error(text: str):
     print(f'[red]{text}[/red]')
     exit(1)
 
 
 @dataclass
 class CloudFlow:
     path: Optional[str] = None
@@ -356,70 +363,81 @@
                 ) as response:
                     response.raise_for_status()
                     return jcloud_logs_from_response(
                         self.flow_id, await response.json()
                     )
         except aiohttp.ClientResponseError as e:
             if e.status == HTTPStatus.UNAUTHORIZED:
+                _exit_error('Please login using [b]jc login[/b].')
+            if e.status == HTTPStatus.FORBIDDEN:
                 _exit_error(
                     f'You are not authorized to access the Flow [b]{self.flow_id}[/b]'
                 )
-            if e.status == HTTPStatus.FORBIDDEN:
-                _exit_error('Please login using [b]jc login[/b].')
 
     @property
     async def status(self) -> Dict:
-        try:
-            async with get_aiohttp_session() as session:
-                async with session.get(
-                    url=f'{FLOWS_API}/{self.flow_id}', headers=self.auth_header
-                ) as response:
-                    response.raise_for_status()
-                    return await response.json()
-        except aiohttp.ClientResponseError as e:
-            if e.status == HTTPStatus.UNAUTHORIZED:
-                _exit_error(
-                    f'You are not authorized to access the Flow [b]{self.flow_id}[/b]'
+        async with get_aiohttp_session() as session:
+            async with session.get(
+                url=f'{FLOWS_API}/{self.flow_id}', headers=self.auth_header
+            ) as response:
+                json_response = await response.json()
+                _exit_if_response_error(
+                    response,
+                    expected_status=HTTPStatus.OK,
+                    json_response=json_response,
                 )
-            if e.status == HTTPStatus.FORBIDDEN:
-                _exit_error('Please login using [b]jc login[/b].')
+                return await response.json()
+
+    async def logs(self, executor_name: Optional[str] = None) -> Dict:
+        _base_url = f'{FLOWS_API}/{self.flow_id}'
+        if executor_name:
+            _url = f'{_base_url}/executors/{executor_name}'
+        else:
+            _url = f'{_base_url}/gateway'
+        async with get_aiohttp_session() as session:
+            async with session.get(
+                url=f'{_url}/logs', headers=self.auth_header
+            ) as response:
+                json_response = await response.json()
+                _exit_if_response_error(
+                    response,
+                    expected_status=HTTPStatus.OK,
+                    json_response=json_response,
+                )
+                return json_response['logs']
 
     async def list_all(
         self,
         phase: Optional[str] = None,
         name: Optional[str] = None,
         labels: Dict[str, str] = None,
     ) -> Dict:
-        try:
-            async with get_aiohttp_session() as session:
-                _args = dict(url=FLOWS_API, headers=self.auth_header)
-                _args['params'] = {}
+        async with get_aiohttp_session() as session:
+            _args = dict(url=FLOWS_API, headers=self.auth_header)
+            _args['params'] = {}
 
-                if phase is not None and phase != 'All':
-                    _args['params'].update({'phase': phase})
-                if name is not None:
-                    _args['params'].update({'name': name})
-                if labels is not None:
-                    _args['params'].update({'labels': labels})
-                async with session.get(**_args) as response:
-                    response.raise_for_status()
-                    _results = await response.json()
-                    if not _results:
-                        print(
-                            f'\nYou don\'t have any Flows deployed with status [green]{phase}[/green]. '
-                            f'Please pass a different [i]--status[/i] or use [i]jc deploy[/i] to deploy a new Flow'
-                        )
-                    return _results
-        except aiohttp.ClientResponseError as e:
-            if e.status in (HTTPStatus.UNAUTHORIZED, HTTPStatus.FORBIDDEN):
-                _exit_error('Please login using [b]jc login[/b].')
-            elif e.status == HTTPStatus.NOT_FOUND:
-                print(
-                    '\nYou don\'t have any Flows deployed. Please use [b]jc deploy[/b]'
+            if phase is not None and phase != 'All':
+                _args['params'].update({'phase': phase})
+            if name is not None:
+                _args['params'].update({'name': name})
+            if labels is not None:
+                _args['params'].update({'labels': labels})
+            async with session.get(**_args) as response:
+                _results = await response.json()
+                if not _results:
+                    print(
+                        f'\nYou don\'t have any Flows deployed with status [green]{phase}[/green]. '
+                        f'Please pass a different [i]--status[/i] or use [i]jc deploy[/i] to deploy a new Flow'
+                    )
+                _exit_if_response_error(
+                    response,
+                    expected_status=HTTPStatus.OK,
+                    json_response=_results,
                 )
+                return _results
 
     async def _fetch_until(
         self,
         intermediate: List[Phase],
         desired: Phase = Phase.Serving,
     ) -> Tuple[Optional[Dict[str, str]], Optional[str]]:
         _wait_seconds = 0
@@ -494,15 +512,16 @@
                 intermediate=[
                     Phase.Empty,
                     Phase.Pending,
                     Phase.Starting,
                 ],
                 desired=Phase.Serving,
             )
-            pbar.console.print(self)
+            if 'JCLOUD_HIDE_SUCCESS_MSG' not in os.environ:
+                pbar.console.print(self)
             pbar.update(pb_task, description='Finishing', advance=1)
 
         if 'JCLOUD_NO_SURVEY' not in os.environ:
             # ask feedback
             from .survey import Survey
 
             Survey().count().ask(threshold=3)
```

### Comparing `jcloud-0.2.8.dev2/jcloud/helper.py` & `jcloud-0.2.9.dev3/jcloud/helper.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,17 @@
 import aiohttp
 import pkg_resources
 import yaml
 from dateutil import tz
 from hubble.executor.helper import is_valid_docker_uri, is_valid_sandbox_uri
 from packaging.version import Version
 from rich import print
+from rich.align import Align
 from rich.highlighter import ReprHighlighter
+from rich.table import Table
 from rich.panel import Panel
 
 __windows__ = sys.platform == 'win32'
 
 
 def _version_check(package: str = None, github_repo: str = None):
     try:
@@ -189,14 +191,22 @@
 
 class CustomHighlighter(ReprHighlighter):
     highlights = ReprHighlighter.highlights + [
         r"(?P<url>(grpc|grpcs)://[-0-9a-zA-Z$_+!`(),.?/;:&=%#]*)"
     ]
 
 
+def add_table_row_fn(table: Table, key: str, value: str):
+    return lambda: table.add_row(Align(f'[bold]{key}', vertical='middle'), value)
+
+
+def center_align(value: str):
+    return Align(f'[bold]{value}[/bold]', align='center')
+
+
 def remove_prefix(s: str, prefix: str):
     return s[len(prefix) :] if s.startswith(prefix) else s
 
 
 def jsonify(data: Union[Dict, List]) -> str:
     return (
         json.dumps(data, indent=2, sort_keys=True)
```

### Comparing `jcloud-0.2.8.dev2/jcloud/normalize.py` & `jcloud-0.2.9.dev3/jcloud/normalize.py`

 * *Files identical despite different names*

### Comparing `jcloud-0.2.8.dev2/jcloud/parsers/__init__.py` & `jcloud-0.2.9.dev3/jcloud/parsers/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     from .deploy import set_deploy_parser
     from .helper import _chf
     from .list import set_list_parser
     from .remove import set_remove_parser
     from .status import set_status_parser
     from .normalize import set_normalize_parser
     from .update import set_update_parser
+    from .logs import set_logs_parser
     from .custom_actions import (
         set_restart_parser,
         set_pause_parser,
         set_resume_parser,
         set_scale_parser,
         set_recreate_parser,
     )
@@ -117,19 +118,35 @@
             'resume',
             help='Resume a paused Flow',
             formatter_class=_chf,
         )
     )
 
     set_scale_parser(
-        sp.add_parser('scale', help='Scale executor of Flow', formatter_class=_chf)
+        sp.add_parser(
+            'scale',
+            help='Scale executor of Flow',
+            formatter_class=_chf,
+        )
     )
 
     set_recreate_parser(
-        sp.add_parser('recreate', help='Recreate deleted Flow', formatter_class=_chf)
+        sp.add_parser(
+            'recreate',
+            help='Recreate deleted Flow',
+            formatter_class=_chf,
+        )
+    )
+
+    set_logs_parser(
+        sp.add_parser(
+            'logs',
+            help='Get the logs of an executor/gateway pod',
+            formatter_class=_chf,
+        )
     )
 
     sp.add_parser(
         'survey',
         help='Tell us your experience and help us improve.',
         formatter_class=_chf,
     )
```

### Comparing `jcloud-0.2.8.dev2/jcloud/parsers/base.py` & `jcloud-0.2.9.dev3/jcloud/parsers/base.py`

 * *Files identical despite different names*

### Comparing `jcloud-0.2.8.dev2/jcloud/parsers/custom_actions.py` & `jcloud-0.2.9.dev3/jcloud/parsers/custom_actions.py`

 * *Files identical despite different names*

### Comparing `jcloud-0.2.8.dev2/jcloud/parsers/helper.py` & `jcloud-0.2.9.dev3/jcloud/parsers/helper.py`

 * *Files identical despite different names*

### Comparing `jcloud-0.2.8.dev2/jcloud/parsers/list.py` & `jcloud-0.2.9.dev3/jcloud/parsers/list.py`

 * *Files identical despite different names*

### Comparing `jcloud-0.2.8.dev2/jcloud/parsers/normalize.py` & `jcloud-0.2.9.dev3/jcloud/parsers/normalize.py`

 * *Files identical despite different names*

### Comparing `jcloud-0.2.8.dev2/jcloud/parsers/remove.py` & `jcloud-0.2.9.dev3/jcloud/parsers/remove.py`

 * *Files identical despite different names*

### Comparing `jcloud-0.2.8.dev2/jcloud/survey.py` & `jcloud-0.2.9.dev3/jcloud/survey.py`

 * *Files identical despite different names*

### Comparing `jcloud-0.2.8.dev2/jcloud.egg-info/PKG-INFO` & `jcloud-0.2.9.dev3/jcloud.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jcloud
-Version: 0.2.8.dev2
+Version: 0.2.9.dev3
 Summary: Simplify deploying and managing Jina projects on Jina Cloud
 Home-page: https://github.com/jina-ai/jcloud
 Author: Jina AI
 Author-email: hello@jina.ai
 License: Apache 2.0
 Download-URL: https://github.com/jina-ai/jcloud/tags
 Project-URL: Documentation, https://jcloud.jina.ai
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: jcloud Version: 0.2.8.dev2 Summary: Simplify
+Metadata-Version: 2.1 Name: jcloud Version: 0.2.9.dev3 Summary: Simplify
 deploying and managing Jina projects on Jina Cloud Home-page: https://
 github.com/jina-ai/jcloud Author: Jina AI Author-email: hello@jina.ai License:
 Apache 2.0 Download-URL: https://github.com/jina-ai/jcloud/tags Project-URL:
 Documentation, https://jcloud.jina.ai Project-URL: Source, https://github.com/
 jina-ai/jcloud/ Project-URL: Tracker, https://github.com/jina-ai/jcloud/issues
 Keywords: jcloud neural-search serverless deployment devops mlops Platform:
 UNKNOWN Classifier: Development Status :: 5 - Production/Stable Classifier:
```

### Comparing `jcloud-0.2.8.dev2/jcloud.egg-info/SOURCES.txt` & `jcloud-0.2.9.dev3/jcloud.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 jcloud.egg-info/top_level.txt
 jcloud/parsers/__init__.py
 jcloud/parsers/base.py
 jcloud/parsers/custom_actions.py
 jcloud/parsers/deploy.py
 jcloud/parsers/helper.py
 jcloud/parsers/list.py
+jcloud/parsers/logs.py
 jcloud/parsers/normalize.py
 jcloud/parsers/remove.py
 jcloud/parsers/status.py
 jcloud/parsers/update.py
 jcloud/resources/project-template/.env
 jcloud/resources/project-template/flow.yml
 jcloud/resources/project-template/executor1/config.yml
```

### Comparing `jcloud-0.2.8.dev2/setup.py` & `jcloud-0.2.9.dev3/setup.py`

 * *Files identical despite different names*

