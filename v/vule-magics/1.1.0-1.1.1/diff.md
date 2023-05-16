# Comparing `tmp/vule_magics-1.1.0.tar.gz` & `tmp/vule_magics-1.1.1.tar.gz`

## Comparing `vule_magics-1.1.0.tar` & `vule_magics-1.1.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 vule_magics-1.1.0/.prettierignore
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 vule_magics-1.1.0/CHANGELOG.md
--rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 vule_magics-1.1.0/RELEASE.md
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 vule_magics-1.1.0/install.json
--rw-r--r--   0        0        0     5794 2020-02-02 00:00:00.000000 vule_magics-1.1.0/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 vule_magics-1.1.0/setup.py
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 vule_magics-1.1.0/tsconfig.json
--rw-r--r--   0        0        0   217147 2020-02-02 00:00:00.000000 vule_magics-1.1.0/yarn.lock
--rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 vule_magics-1.1.0/src/index.ts
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 vule_magics-1.1.0/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 vule_magics-1.1.0/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 vule_magics-1.1.0/style/index.js
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 vule_magics-1.1.0/vule_magics/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 vule_magics-1.1.0/vule_magics/_version.py
--rw-r--r--   0        0        0     5166 2020-02-02 00:00:00.000000 vule_magics-1.1.0/vule_magics/labextension/package.json
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 vule_magics-1.1.0/vule_magics/labextension/static/568.86f8cf51e32d5a4a98cb.js
--rw-r--r--   0        0        0     3498 2020-02-02 00:00:00.000000 vule_magics-1.1.0/vule_magics/labextension/static/747.6b9eb3eb7bd07ac8fdef.js
--rw-r--r--   0        0        0     6913 2020-02-02 00:00:00.000000 vule_magics-1.1.0/vule_magics/labextension/static/remoteEntry.038ab40883c4d106f12a.js
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 vule_magics-1.1.0/vule_magics/labextension/static/style.js
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 vule_magics-1.1.0/vule_magics/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 vule_magics-1.1.0/vule_magics/sparksql/__init__.py
--rw-r--r--   0        0        0     2675 2020-02-02 00:00:00.000000 vule_magics-1.1.0/vule_magics/sparksql/sparksql.py
--rw-r--r--   0        0        0     9861 2020-02-02 00:00:00.000000 vule_magics-1.1.0/vule_magics/sparksql/widget.py
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 vule_magics-1.1.0/.gitignore
--rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 vule_magics-1.1.0/LICENSE
--rw-r--r--   0        0        0     2421 2020-02-02 00:00:00.000000 vule_magics-1.1.0/README.md
--rw-r--r--   0        0        0     2278 2020-02-02 00:00:00.000000 vule_magics-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     5286 2020-02-02 00:00:00.000000 vule_magics-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 vule_magics-1.1.1/.prettierignore
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 vule_magics-1.1.1/CHANGELOG.md
+-rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 vule_magics-1.1.1/RELEASE.md
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 vule_magics-1.1.1/install.json
+-rw-r--r--   0        0        0     5794 2020-02-02 00:00:00.000000 vule_magics-1.1.1/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 vule_magics-1.1.1/setup.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 vule_magics-1.1.1/tsconfig.json
+-rw-r--r--   0        0        0   217147 2020-02-02 00:00:00.000000 vule_magics-1.1.1/yarn.lock
+-rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 vule_magics-1.1.1/src/index.ts
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 vule_magics-1.1.1/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 vule_magics-1.1.1/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 vule_magics-1.1.1/style/index.js
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 vule_magics-1.1.1/vule_magics/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 vule_magics-1.1.1/vule_magics/_version.py
+-rw-r--r--   0        0        0     5166 2020-02-02 00:00:00.000000 vule_magics-1.1.1/vule_magics/labextension/package.json
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 vule_magics-1.1.1/vule_magics/labextension/static/568.86f8cf51e32d5a4a98cb.js
+-rw-r--r--   0        0        0     3498 2020-02-02 00:00:00.000000 vule_magics-1.1.1/vule_magics/labextension/static/747.6b9eb3eb7bd07ac8fdef.js
+-rw-r--r--   0        0        0     6913 2020-02-02 00:00:00.000000 vule_magics-1.1.1/vule_magics/labextension/static/remoteEntry.146740570c7e2dc00ed3.js
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 vule_magics-1.1.1/vule_magics/labextension/static/style.js
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 vule_magics-1.1.1/vule_magics/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 vule_magics-1.1.1/vule_magics/sparksql/__init__.py
+-rw-r--r--   0        0        0     2675 2020-02-02 00:00:00.000000 vule_magics-1.1.1/vule_magics/sparksql/sparksql.py
+-rw-r--r--   0        0        0     9873 2020-02-02 00:00:00.000000 vule_magics-1.1.1/vule_magics/sparksql/widget.py
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 vule_magics-1.1.1/.gitignore
+-rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 vule_magics-1.1.1/LICENSE
+-rw-r--r--   0        0        0     2421 2020-02-02 00:00:00.000000 vule_magics-1.1.1/README.md
+-rw-r--r--   0        0        0     2278 2020-02-02 00:00:00.000000 vule_magics-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     5286 2020-02-02 00:00:00.000000 vule_magics-1.1.1/PKG-INFO
```

### Comparing `vule_magics-1.1.0/RELEASE.md` & `vule_magics-1.1.1/RELEASE.md`

 * *Files identical despite different names*

### Comparing `vule_magics-1.1.0/package.json` & `vule_magics-1.1.1/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'version'": "'1.1.1'"}*

```diff
@@ -163,9 +163,9 @@
         "rules": {
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "1.1.0"
+    "version": "1.1.1"
 }
```

### Comparing `vule_magics-1.1.0/tsconfig.json` & `vule_magics-1.1.1/tsconfig.json`

 * *Files identical despite different names*

### Comparing `vule_magics-1.1.0/yarn.lock` & `vule_magics-1.1.1/yarn.lock`

 * *Files identical despite different names*

### Comparing `vule_magics-1.1.0/src/index.ts` & `vule_magics-1.1.1/src/index.ts`

 * *Files identical despite different names*

### Comparing `vule_magics-1.1.0/vule_magics/labextension/package.json` & `vule_magics-1.1.1/vule_magics/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9785879629629629%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.146740570c7e2dc00ed3.js'}}",*

 * * "'version'": "'1.1.1'"}*

```diff
@@ -96,15 +96,15 @@
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/vule24/vule-jupyter-extensions",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.038ab40883c4d106f12a.js",
+            "load": "static/remoteEntry.146740570c7e2dc00ed3.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "vule_magics/labextension"
     },
     "keywords": [
         "jupyter",
@@ -168,9 +168,9 @@
         "rules": {
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "1.1.0"
+    "version": "1.1.1"
 }
```

### Comparing `vule_magics-1.1.0/vule_magics/labextension/static/568.86f8cf51e32d5a4a98cb.js` & `vule_magics-1.1.1/vule_magics/labextension/static/568.86f8cf51e32d5a4a98cb.js`

 * *Files identical despite different names*

### Comparing `vule_magics-1.1.0/vule_magics/labextension/static/747.6b9eb3eb7bd07ac8fdef.js` & `vule_magics-1.1.1/vule_magics/labextension/static/747.6b9eb3eb7bd07ac8fdef.js`

 * *Files identical despite different names*

### Comparing `vule_magics-1.1.0/vule_magics/labextension/static/remoteEntry.038ab40883c4d106f12a.js` & `vule_magics-1.1.1/vule_magics/labextension/static/remoteEntry.146740570c7e2dc00ed3.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -106,15 +106,15 @@
                     var o = a[e] = a[e] || {},
                         u = o[r];
                     (!u || !u.loaded && (1 != !u.eager ? n : i > u.from)) && (o[r] = {
                         get: () => k.e(568).then((() => () => k(568))),
                         from: i,
                         eager: !1
                     })
-                })("vule-magics", "1.1.0"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                })("vule-magics", "1.1.1"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         k.g.importScripts && (e = k.g.location + "");
         var r = k.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
```

### Comparing `vule_magics-1.1.0/vule_magics/labextension/static/third-party-licenses.json` & `vule_magics-1.1.1/vule_magics/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `vule_magics-1.1.0/vule_magics/sparksql/__init__.py` & `vule_magics-1.1.1/vule_magics/sparksql/__init__.py`

 * *Files identical despite different names*

### Comparing `vule_magics-1.1.0/vule_magics/sparksql/sparksql.py` & `vule_magics-1.1.1/vule_magics/sparksql/sparksql.py`

 * *Files identical despite different names*

### Comparing `vule_magics-1.1.0/vule_magics/sparksql/widget.py` & `vule_magics-1.1.1/vule_magics/sparksql/widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,16 +99,16 @@
         lines = theme_file.read_text().split('\n')
         for line in lines:
             if '"theme"' in line.strip():
                 if "JupyterLab Light" in line.strip():
                     state['template'] = None
                 else:
                     state['template'] = 'plotly_dark'
-    except Exception() as err:
-        print(err)
+    except Exception as err:
+        state['template'] = None
     
     
     # elements
     layout_btn_render_type = w.Layout(
         width='50px',
         margin='1px 2px 2px 2px')
```

### Comparing `vule_magics-1.1.0/.gitignore` & `vule_magics-1.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `vule_magics-1.1.0/LICENSE` & `vule_magics-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vule_magics-1.1.0/README.md` & `vule_magics-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `vule_magics-1.1.0/pyproject.toml` & `vule_magics-1.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vule_magics-1.1.0/PKG-INFO` & `vule_magics-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vule_magics
-Version: 1.1.0
+Version: 1.1.1
 Summary: JupyterLab MagicCommands Extension
 Project-URL: Homepage, https://github.com/vule24/vule-jupyter-extensions
 Project-URL: Bug Tracker, https://github.com/vule24/vule-jupyter-extensions/issues
 Project-URL: Repository, https://github.com/vule24/vule-jupyter-extensions.git
 Author-email: Vu Le <ltnv24@gmail.com>
 License: BSD 3-Clause License
```

