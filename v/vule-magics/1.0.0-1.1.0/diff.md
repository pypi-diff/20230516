# Comparing `tmp/vule_magics-1.0.0.tar.gz` & `tmp/vule_magics-1.1.0.tar.gz`

## Comparing `vule_magics-1.0.0.tar` & `vule_magics-1.1.0.tar`

### file list

```diff
@@ -1,27 +1,28 @@
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 vule_magics-1.0.0/.prettierignore
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 vule_magics-1.0.0/CHANGELOG.md
--rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 vule_magics-1.0.0/RELEASE.md
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 vule_magics-1.0.0/install.json
--rw-r--r--   0        0        0     5794 2020-02-02 00:00:00.000000 vule_magics-1.0.0/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 vule_magics-1.0.0/setup.py
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 vule_magics-1.0.0/tsconfig.json
--rw-r--r--   0        0        0   217147 2020-02-02 00:00:00.000000 vule_magics-1.0.0/yarn.lock
--rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 vule_magics-1.0.0/src/index.ts
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 vule_magics-1.0.0/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 vule_magics-1.0.0/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 vule_magics-1.0.0/style/index.js
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 vule_magics-1.0.0/vule_magics/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 vule_magics-1.0.0/vule_magics/_version.py
--rw-r--r--   0        0        0     5166 2020-02-02 00:00:00.000000 vule_magics-1.0.0/vule_magics/labextension/package.json
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 vule_magics-1.0.0/vule_magics/labextension/static/568.86f8cf51e32d5a4a98cb.js
--rw-r--r--   0        0        0     3498 2020-02-02 00:00:00.000000 vule_magics-1.0.0/vule_magics/labextension/static/747.6b9eb3eb7bd07ac8fdef.js
--rw-r--r--   0        0        0     6913 2020-02-02 00:00:00.000000 vule_magics-1.0.0/vule_magics/labextension/static/remoteEntry.f3a765341d8f0e4ea124.js
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 vule_magics-1.0.0/vule_magics/labextension/static/style.js
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 vule_magics-1.0.0/vule_magics/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 vule_magics-1.0.0/vule_magics/sparksql/__init__.py
--rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 vule_magics-1.0.0/vule_magics/sparksql/sparksql.py
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 vule_magics-1.0.0/.gitignore
--rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 vule_magics-1.0.0/LICENSE
--rw-r--r--   0        0        0     2421 2020-02-02 00:00:00.000000 vule_magics-1.0.0/README.md
--rw-r--r--   0        0        0     2278 2020-02-02 00:00:00.000000 vule_magics-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     5286 2020-02-02 00:00:00.000000 vule_magics-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 vule_magics-1.1.0/.prettierignore
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 vule_magics-1.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 vule_magics-1.1.0/RELEASE.md
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 vule_magics-1.1.0/install.json
+-rw-r--r--   0        0        0     5794 2020-02-02 00:00:00.000000 vule_magics-1.1.0/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 vule_magics-1.1.0/setup.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 vule_magics-1.1.0/tsconfig.json
+-rw-r--r--   0        0        0   217147 2020-02-02 00:00:00.000000 vule_magics-1.1.0/yarn.lock
+-rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 vule_magics-1.1.0/src/index.ts
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 vule_magics-1.1.0/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 vule_magics-1.1.0/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 vule_magics-1.1.0/style/index.js
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 vule_magics-1.1.0/vule_magics/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 vule_magics-1.1.0/vule_magics/_version.py
+-rw-r--r--   0        0        0     5166 2020-02-02 00:00:00.000000 vule_magics-1.1.0/vule_magics/labextension/package.json
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 vule_magics-1.1.0/vule_magics/labextension/static/568.86f8cf51e32d5a4a98cb.js
+-rw-r--r--   0        0        0     3498 2020-02-02 00:00:00.000000 vule_magics-1.1.0/vule_magics/labextension/static/747.6b9eb3eb7bd07ac8fdef.js
+-rw-r--r--   0        0        0     6913 2020-02-02 00:00:00.000000 vule_magics-1.1.0/vule_magics/labextension/static/remoteEntry.038ab40883c4d106f12a.js
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 vule_magics-1.1.0/vule_magics/labextension/static/style.js
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 vule_magics-1.1.0/vule_magics/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 vule_magics-1.1.0/vule_magics/sparksql/__init__.py
+-rw-r--r--   0        0        0     2675 2020-02-02 00:00:00.000000 vule_magics-1.1.0/vule_magics/sparksql/sparksql.py
+-rw-r--r--   0        0        0     9861 2020-02-02 00:00:00.000000 vule_magics-1.1.0/vule_magics/sparksql/widget.py
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 vule_magics-1.1.0/.gitignore
+-rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 vule_magics-1.1.0/LICENSE
+-rw-r--r--   0        0        0     2421 2020-02-02 00:00:00.000000 vule_magics-1.1.0/README.md
+-rw-r--r--   0        0        0     2278 2020-02-02 00:00:00.000000 vule_magics-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     5286 2020-02-02 00:00:00.000000 vule_magics-1.1.0/PKG-INFO
```

### Comparing `vule_magics-1.0.0/RELEASE.md` & `vule_magics-1.1.0/RELEASE.md`

 * *Files identical despite different names*

### Comparing `vule_magics-1.0.0/package.json` & `vule_magics-1.1.0/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'version'": "'1.1.0'"}*

```diff
@@ -163,9 +163,9 @@
         "rules": {
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "1.0.0"
+    "version": "1.1.0"
 }
```

### Comparing `vule_magics-1.0.0/tsconfig.json` & `vule_magics-1.1.0/tsconfig.json`

 * *Files identical despite different names*

### Comparing `vule_magics-1.0.0/yarn.lock` & `vule_magics-1.1.0/yarn.lock`

 * *Files identical despite different names*

### Comparing `vule_magics-1.0.0/src/index.ts` & `vule_magics-1.1.0/src/index.ts`

 * *Files 4% similar despite different names*

```diff
@@ -67,14 +67,15 @@
   ): void {
     const current_mode = cellEditor.getOption('mode') as string;
     // console.log('current_mode:', current_mode);
 
     if (current_mode === 'null') {
       if (retry) {
         // putting at the end of execution queue to allow the CodeMirror mode to be updated
+        // this will be invoked as soon as possible
         setTimeout(() => this.highlight(cellEditor, false, mode), 0);
       }
       return;
     }
     // console.log('current_mode:', current_mode);
     cellEditor.setOption('mode', mode);
   }
```

### Comparing `vule_magics-1.0.0/vule_magics/labextension/package.json` & `vule_magics-1.1.0/vule_magics/labextension/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9785879629629629%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.038ab40883c4d106f12a.js'}}",*

 * * "'version'": "'1.1.0'"}*

```diff
@@ -96,15 +96,15 @@
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/vule24/vule-jupyter-extensions",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.f3a765341d8f0e4ea124.js",
+            "load": "static/remoteEntry.038ab40883c4d106f12a.js",
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
-    "version": "1.0.0"
+    "version": "1.1.0"
 }
```

### Comparing `vule_magics-1.0.0/vule_magics/labextension/static/568.86f8cf51e32d5a4a98cb.js` & `vule_magics-1.1.0/vule_magics/labextension/static/568.86f8cf51e32d5a4a98cb.js`

 * *Files identical despite different names*

### Comparing `vule_magics-1.0.0/vule_magics/labextension/static/747.6b9eb3eb7bd07ac8fdef.js` & `vule_magics-1.1.0/vule_magics/labextension/static/747.6b9eb3eb7bd07ac8fdef.js`

 * *Files identical despite different names*

### Comparing `vule_magics-1.0.0/vule_magics/labextension/static/remoteEntry.f3a765341d8f0e4ea124.js` & `vule_magics-1.1.0/vule_magics/labextension/static/remoteEntry.038ab40883c4d106f12a.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, a, i, u, l, s, f, d, c, p, h, v, g, m, b, y, w, S = {
+    var e, r, t, n, o, a, i, u, l, s, f, d, c, p, h, v, b, g, m, y, w, S = {
             348: (e, r, t) => {
                 var n = {
                         "./index": () => t.e(568).then((() => () => t(568))),
                         "./extension": () => t.e(568).then((() => () => t(568))),
                         "./style": () => t.e(747).then((() => () => t(747)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
@@ -106,15 +106,15 @@
                     var o = a[e] = a[e] || {},
                         u = o[r];
                     (!u || !u.loaded && (1 != !u.eager ? n : i > u.from)) && (o[r] = {
                         get: () => k.e(568).then((() => () => k(568))),
                         from: i,
                         eager: !1
                     })
-                })("vule-magics", "1.0.0"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                })("vule-magics", "1.1.0"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         k.g.importScripts && (e = k.g.location + "");
         var r = k.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -212,38 +212,38 @@
         var o = e[r];
         return (r = Object.keys(o).reduce(((e, r) => !a(t, r) || e && !n(e, r) ? e : r), 0)) && o[r]
     }, c = (e, r, t, n) => {
         var a = e[t];
         return "No satisfying version (" + o(n) + ") of shared module " + t + " found in shared scope " + r + ".\nAvailable versions: " + Object.keys(a).map((e => e + " from " + a[e].from)).join(", ")
     }, p = (e, r, t, n) => {
         "undefined" != typeof console && console.warn && console.warn(c(e, r, t, n))
-    }, h = e => (e.loaded = 1, e.get()), g = (v = e => function(r, t, n, o) {
+    }, h = e => (e.loaded = 1, e.get()), b = (v = e => function(r, t, n, o) {
         var a = k.I(r);
         return a && a.then ? a.then(e.bind(e, r, k.S[r], t, n, o)) : e(r, k.S[r], t, n, o)
-    })(((e, r, t, n) => (i(e, t), h(d(r, t, n) || p(r, e, t, n) || u(r, t))))), m = v(((e, r, t, n) => (i(e, t), f(r, 0, t, n)))), b = {}, y = {
-        123: () => m("default", "@jupyterlab/notebook", [1, 3, 6, 3]),
-        191: () => g("default", "@jupyterlab/cells", [1, 3, 6, 3])
+    })(((e, r, t, n) => (i(e, t), h(d(r, t, n) || p(r, e, t, n) || u(r, t))))), g = v(((e, r, t, n) => (i(e, t), f(r, 0, t, n)))), m = {}, y = {
+        123: () => g("default", "@jupyterlab/notebook", [1, 3, 6, 3]),
+        191: () => b("default", "@jupyterlab/cells", [1, 3, 6, 3])
     }, w = {
         568: [123, 191]
     }, k.f.consumes = (e, r) => {
         k.o(w, e) && w[e].forEach((e => {
-            if (k.o(b, e)) return r.push(b[e]);
+            if (k.o(m, e)) return r.push(m[e]);
             var t = r => {
-                    b[e] = 0, k.m[e] = t => {
+                    m[e] = 0, k.m[e] = t => {
                         delete k.c[e], t.exports = r()
                     }
                 },
                 n = r => {
-                    delete b[e], k.m[e] = t => {
+                    delete m[e], k.m[e] = t => {
                         throw delete k.c[e], r
                     }
                 };
             try {
                 var o = y[e]();
-                o.then ? r.push(b[e] = o.then(t).catch(n)) : t(o)
+                o.then ? r.push(m[e] = o.then(t).catch(n)) : t(o)
             } catch (e) {
                 n(e)
             }
         }))
     }, (() => {
         var e = {
             466: 0
```

### Comparing `vule_magics-1.0.0/vule_magics/labextension/static/third-party-licenses.json` & `vule_magics-1.1.0/vule_magics/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `vule_magics-1.0.0/vule_magics/sparksql/sparksql.py` & `vule_magics-1.1.0/vule_magics/sparksql/sparksql.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,66 +1,75 @@
 from __future__ import print_function
-from IPython.core.magic import Magics, magics_class, cell_magic, needs_local_scope
+from IPython.core.magic import Magics, magics_class, cell_magic, line_magic
 from IPython.core.magic_arguments import argument, magic_arguments, parse_argstring
-from IPython.display import display, clear_output
+from IPython import display
 from pyspark.sql import SparkSession
 from pyspark.sql.dataframe import DataFrame
 from string import Formatter
+import numpy as np
+
+from .widget import generate_output_widget, generate_classic_table
 
 
 @magics_class
 class SparkSQL(Magics):
 
     @property
     def spark(self):
         return SparkSession._instantiatedSession
 
-
     @magic_arguments()
     @argument('dataframe', metavar='DF', type=str, nargs='?')
-    @argument('-n', '--num-rows', type=int, default=20)
+    @argument('-n', '--num-rows', type=int, default=100)
+    @argument('-c', '--classic', action='store_true', default=False)
     @cell_magic
     def sql(self, line, cell):
-        self._create_temp_view_for_available_dataframe()
-        if cell is None:
-            query_str = self._format_params(line)
-            return self.spark.sql(query_str)
+        self.create_temp_view_for_available_dataframe()
+        
+        args = parse_argstring(self.sql, line)
+        query_str = self.format_fillin_pyvar(cell)
+        
+        sdf = self.spark.sql(query_str)
+        if args.dataframe:
+            self.shell.user_ns.update({args.dataframe: sdf})
+        if not args.classic:
+            return generate_output_widget(sdf, num_rows=args.num_rows, export_table_name=args.dataframe or None)
         else:
-            args = parse_argstring(self.sql, line)
-            query_str = self._format_params(cell)
-            df = self.spark.sql(query_str)
-            if args.dataframe:
-                self.shell.user_ns.update({args.dataframe: df})
-            else:
-                display(df.limit(args.num_rows).toPandas())
-            clear_output(wait=True)
+            return generate_classic_table(sdf, num_rows=args.num_rows)
+
 
 
     @magic_arguments()
+    @argument('dataframe', metavar='DF', type=str, nargs='?')
     @argument('-n', '--num-rows', type=int, default=20)
-    @cell_magic
+    @argument('-c', '--classic', action='store_true', default=False)
+    @line_magic
     def show(self, line):
         args = parse_argstring(self.sql, line)
-        df = self.shell.user_ns.get(args.dataframe, None)
+        sdf = self.shell.user_ns.get(args.dataframe, None)
         try:
-            display(df.limit(args.num_rows).toPandas())
-            clear_output(wait=True)
+            if not args.classic:
+                return generate_output_widget(sdf, num_rows=args.num_rows, export_table_name=args.dataframe)
+            else:
+                return generate_classic_table(sdf, num_rows=args.num_rows)
         except AttributeError as err:
             display(err)
             print("Input dataframe is not existed")
 
 
-    def _create_temp_view_for_available_dataframe(self):
+    def create_temp_view_for_available_dataframe(self):
         for k, v in self.shell.user_ns.items():
             v.createOrReplaceTempView(k) if isinstance(v, DataFrame) else None
 
-    def _format_params(self, source):
-        params = [fn for _, fn, _, _ in Formatter().parse(source) if fn is not None]
+    def format_fillin_pyvar(self, source):
+        params = [fn for _, fn, _, _ in Formatter().parse(source) if fn]
         params_values = {}
         for param in params:
             value = self.shell.user_ns.get(param, None)
             if not value:
-                continue
+                raise NameError("name '{}' is not defined".format(param))
             params_values.update({param: value})
         return source.format(**params_values)
+    
+
```

### Comparing `vule_magics-1.0.0/.gitignore` & `vule_magics-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `vule_magics-1.0.0/LICENSE` & `vule_magics-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vule_magics-1.0.0/README.md` & `vule_magics-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `vule_magics-1.0.0/pyproject.toml` & `vule_magics-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vule_magics-1.0.0/PKG-INFO` & `vule_magics-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vule_magics
-Version: 1.0.0
+Version: 1.1.0
 Summary: JupyterLab MagicCommands Extension
 Project-URL: Homepage, https://github.com/vule24/vule-jupyter-extensions
 Project-URL: Bug Tracker, https://github.com/vule24/vule-jupyter-extensions/issues
 Project-URL: Repository, https://github.com/vule24/vule-jupyter-extensions.git
 Author-email: Vu Le <ltnv24@gmail.com>
 License: BSD 3-Clause License
```

