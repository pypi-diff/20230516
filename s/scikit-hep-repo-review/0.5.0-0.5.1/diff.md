# Comparing `tmp/scikit_hep_repo_review-0.5.0.tar.gz` & `tmp/scikit_hep_repo_review-0.5.1.tar.gz`

## Comparing `scikit_hep_repo_review-0.5.0.tar` & `scikit_hep_repo_review-0.5.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     2210 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.5.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.5.0/noxfile.py
--rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.5.0/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.5.0/.github/dependabot.yml
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.5.0/.github/matchers/pylint.json
--rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.5.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.5.0/docs/.nojekyll
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.5.0/docs/index.html
--rw-r--r--   0        0        0     9099 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.5.0/docs/webapp.js
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.5.0/src/scikit_hep_repo_review/__init__.py
--rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.5.0/src/scikit_hep_repo_review/__main__.py
--rw-r--r--   0        0        0     2807 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.5.0/src/scikit_hep_repo_review/ghpath.py
--rw-r--r--   0        0        0     3016 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.5.0/src/scikit_hep_repo_review/processor.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.5.0/src/scikit_hep_repo_review/py.typed
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.5.0/src/scikit_hep_repo_review/ratings/__init__.py
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.5.0/src/scikit_hep_repo_review/ratings/general.py
--rw-r--r--   0        0        0     4831 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.5.0/src/scikit_hep_repo_review/ratings/github.py
--rw-r--r--   0        0        0     3939 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.5.0/src/scikit_hep_repo_review/ratings/mypy.py
--rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.5.0/src/scikit_hep_repo_review/ratings/precommit.py
--rw-r--r--   0        0        0     5445 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.5.0/src/scikit_hep_repo_review/ratings/pyproject.py
--rw-r--r--   0        0        0     2715 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.5.0/src/scikit_hep_repo_review/ratings/ruff.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.5.0/tests/test_package.py
--rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.5.0/.gitignore
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.5.0/LICENSE
--rw-r--r--   0        0        0     4594 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.5.0/README.md
--rw-r--r--   0        0        0     3686 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     7636 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.5.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.5.1/noxfile.py
+-rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.5.1/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.5.1/.github/dependabot.yml
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.5.1/.github/matchers/pylint.json
+-rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.5.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.5.1/docs/.nojekyll
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.5.1/docs/index.html
+-rw-r--r--   0        0        0     9099 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.5.1/docs/webapp.js
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.5.1/src/scikit_hep_repo_review/__init__.py
+-rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.5.1/src/scikit_hep_repo_review/__main__.py
+-rw-r--r--   0        0        0     2807 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.5.1/src/scikit_hep_repo_review/ghpath.py
+-rw-r--r--   0        0        0     3016 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.5.1/src/scikit_hep_repo_review/processor.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.5.1/src/scikit_hep_repo_review/py.typed
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.5.1/src/scikit_hep_repo_review/ratings/__init__.py
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.5.1/src/scikit_hep_repo_review/ratings/general.py
+-rw-r--r--   0        0        0     4831 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.5.1/src/scikit_hep_repo_review/ratings/github.py
+-rw-r--r--   0        0        0     3939 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.5.1/src/scikit_hep_repo_review/ratings/mypy.py
+-rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.5.1/src/scikit_hep_repo_review/ratings/precommit.py
+-rw-r--r--   0        0        0     5445 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.5.1/src/scikit_hep_repo_review/ratings/pyproject.py
+-rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.5.1/src/scikit_hep_repo_review/ratings/ruff.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.5.1/tests/test_package.py
+-rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.5.1/.gitignore
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.5.1/LICENSE
+-rw-r--r--   0        0        0     4594 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.5.1/README.md
+-rw-r--r--   0        0        0     3686 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     7636 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.5.1/PKG-INFO
```

### Comparing `scikit_hep_repo_review-0.5.0/.pre-commit-config.yaml` & `scikit_hep_repo_review-0.5.1/.pre-commit-config.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -4,32 +4,32 @@
 
 ci:
   autoupdate_commit_msg: "chore(deps): update pre-commit hooks"
   autofix_commit_msg: "style: pre-commit fixes"
 
 repos:
   - repo: https://github.com/psf/black
-    rev: 23.1.0
+    rev: 23.3.0
     hooks:
       - id: black-jupyter
 
   - repo: https://github.com/asottile/blacken-docs
     rev: 1.13.0
     hooks:
       - id: blacken-docs
         additional_dependencies: [black==23.1.0]
 
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: "v0.0.251"
+    rev: "v0.0.267"
     hooks:
       - id: ruff
         args: ["--fix", "--show-fixes"]
 
   - repo: https://github.com/pre-commit/mirrors-prettier
-    rev: "v3.0.0-alpha.4"
+    rev: "v3.0.0-alpha.9-for-vscode"
     hooks:
       - id: prettier
         types_or: [yaml, markdown, html, css, scss, javascript, json]
 
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.4.0
     hooks:
@@ -50,28 +50,28 @@
     rev: v1.10.0
     hooks:
       - id: rst-backticks
       - id: rst-directive-colons
       - id: rst-inline-touching-normal
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.0.1
+    rev: v1.3.0
     hooks:
       - id: mypy
         files: src
         args: []
         additional_dependencies:
           - click
           - rich
           - types-PyYAML
           - tomli;python_version<"3.11"
           - markdown-it-py
 
   - repo: https://github.com/codespell-project/codespell
-    rev: v2.2.2
+    rev: v2.2.4
     hooks:
       - id: codespell
         args: ["-Lhist,absense"]
 
   - repo: https://github.com/shellcheck-py/shellcheck-py
     rev: v0.9.0.2
     hooks:
```

### Comparing `scikit_hep_repo_review-0.5.0/noxfile.py` & `scikit_hep_repo_review-0.5.1/noxfile.py`

 * *Files identical despite different names*

### Comparing `scikit_hep_repo_review-0.5.0/.github/CONTRIBUTING.md` & `scikit_hep_repo_review-0.5.1/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `scikit_hep_repo_review-0.5.0/.github/matchers/pylint.json` & `scikit_hep_repo_review-0.5.1/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `scikit_hep_repo_review-0.5.0/.github/workflows/ci.yml` & `scikit_hep_repo_review-0.5.1/.github/workflows/ci.yml`

 * *Files 5% similar despite different names*

```diff
@@ -72,11 +72,22 @@
       - uses: actions/upload-artifact@v3
         with:
           path: dist
 
       - name: Check products
         run: pipx run twine check dist/*
 
-      - uses: pypa/gh-action-pypi-publish@v1.6.4
-        if: github.event_name == 'release' && github.event.action == 'published'
+  publish:
+    name: Publish
+    needs: [dist]
+    environment: pypi
+    permissions:
+      id-token: write
+    runs-on: ubuntu-latest
+    if: github.event_name == 'release' && github.event.action == 'published'
+    steps:
+      - uses: actions/download-artifact@v3
         with:
-          password: ${{ secrets.pypi_password }}
+          name: artifact
+          path: dist
+
+      - uses: pypa/gh-action-pypi-publish@release/v1
```

### Comparing `scikit_hep_repo_review-0.5.0/docs/index.html` & `scikit_hep_repo_review-0.5.1/docs/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
   <head>
     <meta
       charset="utf-8"
       name="viewport"
       content="initial-scale=1, width=device-width"
     />
     <script
-      src="https://cdn.jsdelivr.net/pyodide/v0.22.1/full/pyodide.js"
+      src="https://cdn.jsdelivr.net/pyodide/v0.23.1/full/pyodide.js"
       crossorigin
     ></script>
     <!-- Production -->
     <script
       src="https://unpkg.com/react@18/umd/react.production.min.js"
       crossorigin
     ></script>
```

### Comparing `scikit_hep_repo_review-0.5.0/docs/webapp.js` & `scikit_hep_repo_review-0.5.1/docs/webapp.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -163,15 +163,15 @@
 
 async function prepare_pyodide() {
     const pyodide = await loadPyodide();
 
     await pyodide.loadPackage("micropip");
     await pyodide.runPythonAsync(`
         import micropip
-        await micropip.install(["scikit_hep_repo_review==0.4.2"])
+        await micropip.install(["scikit_hep_repo_review==0.5.0"])
     `);
     return pyodide;
 }
 
 const pyodide_promise = prepare_pyodide();
 
 function MyThemeProvider(props) {
```

### Comparing `scikit_hep_repo_review-0.5.0/src/scikit_hep_repo_review/__main__.py` & `scikit_hep_repo_review-0.5.1/src/scikit_hep_repo_review/__main__.py`

 * *Files identical despite different names*

### Comparing `scikit_hep_repo_review-0.5.0/src/scikit_hep_repo_review/ghpath.py` & `scikit_hep_repo_review-0.5.1/src/scikit_hep_repo_review/ghpath.py`

 * *Files identical despite different names*

### Comparing `scikit_hep_repo_review-0.5.0/src/scikit_hep_repo_review/processor.py` & `scikit_hep_repo_review-0.5.1/src/scikit_hep_repo_review/processor.py`

 * *Files identical despite different names*

### Comparing `scikit_hep_repo_review-0.5.0/src/scikit_hep_repo_review/ratings/general.py` & `scikit_hep_repo_review-0.5.1/src/scikit_hep_repo_review/ratings/general.py`

 * *Files identical despite different names*

### Comparing `scikit_hep_repo_review-0.5.0/src/scikit_hep_repo_review/ratings/github.py` & `scikit_hep_repo_review-0.5.1/src/scikit_hep_repo_review/ratings/github.py`

 * *Files identical despite different names*

### Comparing `scikit_hep_repo_review-0.5.0/src/scikit_hep_repo_review/ratings/mypy.py` & `scikit_hep_repo_review-0.5.1/src/scikit_hep_repo_review/ratings/mypy.py`

 * *Files identical despite different names*

### Comparing `scikit_hep_repo_review-0.5.0/src/scikit_hep_repo_review/ratings/precommit.py` & `scikit_hep_repo_review-0.5.1/src/scikit_hep_repo_review/ratings/precommit.py`

 * *Files identical despite different names*

### Comparing `scikit_hep_repo_review-0.5.0/src/scikit_hep_repo_review/ratings/pyproject.py` & `scikit_hep_repo_review-0.5.1/src/scikit_hep_repo_review/ratings/pyproject.py`

 * *Files identical despite different names*

### Comparing `scikit_hep_repo_review-0.5.0/src/scikit_hep_repo_review/ratings/ruff.py` & `scikit_hep_repo_review-0.5.1/src/scikit_hep_repo_review/ratings/ruff.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,14 +46,16 @@
             case _:
                 return False
 
 
 class R003(Ruff):
     "src directory specified if used"
 
+    requires = {"R001"}
+
     @staticmethod
     def check(pyproject: dict[str, Any], package: Traversable) -> bool | None:
         """
         Must specify `src` directory if it exists.
         ```toml
         src = ["src"]
         ```
```

### Comparing `scikit_hep_repo_review-0.5.0/.gitignore` & `scikit_hep_repo_review-0.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `scikit_hep_repo_review-0.5.0/LICENSE` & `scikit_hep_repo_review-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit_hep_repo_review-0.5.0/README.md` & `scikit_hep_repo_review-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `scikit_hep_repo_review-0.5.0/pyproject.toml` & `scikit_hep_repo_review-0.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scikit_hep_repo_review-0.5.0/PKG-INFO` & `scikit_hep_repo_review-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit_hep_repo_review
-Version: 0.5.0
+Version: 0.5.1
 Summary: Review repos for compliance to the Scikit-HEP developer guidelines
 Project-URL: homepage, https://github.com/Scikit-HEP/repo-review
 Project-URL: webpage, https://scikit-hep.github.io/repo-review
 Author-email: Henry Schreiner <henryfs@princeton.edu>
 Maintainer-email: The Scikit-HEP admins <scikit-hep-admins@googlegroups.com>
 License: BSD 3-Clause License
```

