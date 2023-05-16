# Comparing `tmp/pyvcd-0.3.0.tar.gz` & `tmp/pyvcd-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvcd-0.3.0.tar", last modified: Tue Sep 28 15:13:08 2021, max compression
+gzip compressed data, was "pyvcd-0.4.0.tar", last modified: Tue May 16 17:08:46 2023, max compression
```

## Comparing `pyvcd-0.3.0.tar` & `pyvcd-0.4.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-28 15:13:08.129150 pyvcd-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (121)       36 2021-09-28 15:13:03.000000 pyvcd-0.3.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-28 15:13:08.125150 pyvcd-0.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-28 15:13:08.125150 pyvcd-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2597 2021-09-28 15:13:03.000000 pyvcd-0.3.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (121)      114 2021-09-28 15:13:03.000000 pyvcd-0.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     2615 2021-09-28 15:13:03.000000 pyvcd-0.3.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5571 2021-09-28 15:13:03.000000 pyvcd-0.3.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1084 2021-09-28 15:13:03.000000 pyvcd-0.3.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)      208 2021-09-28 15:13:03.000000 pyvcd-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      723 2021-09-28 15:13:03.000000 pyvcd-0.3.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     4026 2021-09-28 15:13:08.129150 pyvcd-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1658 2021-09-28 15:13:03.000000 pyvcd-0.3.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-28 15:13:08.129150 pyvcd-0.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     7652 2021-09-28 15:13:03.000000 pyvcd-0.3.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     1360 2021-09-28 15:13:03.000000 pyvcd-0.3.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      266 2021-09-28 15:13:03.000000 pyvcd-0.3.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      374 2021-09-28 15:13:03.000000 pyvcd-0.3.0/docs/vcd.common.rst
--rw-r--r--   0 runner    (1001) docker     (121)      338 2021-09-28 15:13:03.000000 pyvcd-0.3.0/docs/vcd.gtkw.rst
--rw-r--r--   0 runner    (1001) docker     (121)      551 2021-09-28 15:13:03.000000 pyvcd-0.3.0/docs/vcd.reader.rst
--rw-r--r--   0 runner    (1001) docker     (121)       45 2021-09-28 15:13:03.000000 pyvcd-0.3.0/docs/vcd.rst
--rw-r--r--   0 runner    (1001) docker     (121)      375 2021-09-28 15:13:03.000000 pyvcd-0.3.0/docs/vcd.writer.rst
--rw-r--r--   0 runner    (1001) docker     (121)      328 2021-09-28 15:13:03.000000 pyvcd-0.3.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-28 15:13:08.129150 pyvcd-0.3.0/pyvcd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4026 2021-09-28 15:13:08.000000 pyvcd-0.3.0/pyvcd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      622 2021-09-28 15:13:08.000000 pyvcd-0.3.0/pyvcd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-28 15:13:08.000000 pyvcd-0.3.0/pyvcd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-28 15:13:08.000000 pyvcd-0.3.0/pyvcd.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)        4 2021-09-28 15:13:08.000000 pyvcd-0.3.0/pyvcd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      165 2021-09-28 15:13:03.000000 pyvcd-0.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1422 2021-09-28 15:13:08.129150 pyvcd-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       76 2021-09-28 15:13:03.000000 pyvcd-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-28 15:13:08.129150 pyvcd-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      234 2021-09-28 15:13:03.000000 pyvcd-0.3.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)    13333 2021-09-28 15:13:03.000000 pyvcd-0.3.0/tests/test_gtkw.py
--rw-r--r--   0 runner    (1001) docker     (121)     5327 2021-09-28 15:13:03.000000 pyvcd-0.3.0/tests/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (121)    27078 2021-09-28 15:13:03.000000 pyvcd-0.3.0/tests/test_writer.py
--rw-r--r--   0 runner    (1001) docker     (121)      177 2021-09-28 15:13:03.000000 pyvcd-0.3.0/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-28 15:13:08.129150 pyvcd-0.3.0/vcd/
--rw-r--r--   0 runner    (1001) docker     (121)      274 2021-09-28 15:13:03.000000 pyvcd-0.3.0/vcd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1859 2021-09-28 15:13:03.000000 pyvcd-0.3.0/vcd/common.py
--rw-r--r--   0 runner    (1001) docker     (121)    26265 2021-09-28 15:13:03.000000 pyvcd-0.3.0/vcd/gtkw.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-28 15:13:03.000000 pyvcd-0.3.0/vcd/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    20018 2021-09-28 15:13:03.000000 pyvcd-0.3.0/vcd/reader.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    26995 2021-09-28 15:13:03.000000 pyvcd-0.3.0/vcd/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:08:46.979321 pyvcd-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-16 17:08:33.000000 pyvcd-0.4.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:08:46.971321 pyvcd-0.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:08:46.975321 pyvcd-0.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-05-16 17:08:33.000000 pyvcd-0.4.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-16 17:08:33.000000 pyvcd-0.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-05-16 17:08:33.000000 pyvcd-0.4.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5571 2023-05-16 17:08:33.000000 pyvcd-0.4.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-16 17:08:33.000000 pyvcd-0.4.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-16 17:08:33.000000 pyvcd-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-16 17:08:33.000000 pyvcd-0.4.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-05-16 17:08:46.979321 pyvcd-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-05-16 17:08:33.000000 pyvcd-0.4.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:08:46.975321 pyvcd-0.4.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-05-16 17:08:33.000000 pyvcd-0.4.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-05-16 17:08:33.000000 pyvcd-0.4.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-16 17:08:33.000000 pyvcd-0.4.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-16 17:08:33.000000 pyvcd-0.4.0/docs/vcd.common.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-16 17:08:33.000000 pyvcd-0.4.0/docs/vcd.gtkw.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-16 17:08:33.000000 pyvcd-0.4.0/docs/vcd.reader.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-16 17:08:33.000000 pyvcd-0.4.0/docs/vcd.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-16 17:08:33.000000 pyvcd-0.4.0/docs/vcd.writer.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-16 17:08:33.000000 pyvcd-0.4.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:08:46.975321 pyvcd-0.4.0/pyvcd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-05-16 17:08:46.000000 pyvcd-0.4.0/pyvcd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-16 17:08:46.000000 pyvcd-0.4.0/pyvcd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 17:08:46.000000 pyvcd-0.4.0/pyvcd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 17:08:46.000000 pyvcd-0.4.0/pyvcd.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-16 17:08:46.000000 pyvcd-0.4.0/pyvcd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-16 17:08:33.000000 pyvcd-0.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-05-16 17:08:46.979321 pyvcd-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-16 17:08:33.000000 pyvcd-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:08:46.975321 pyvcd-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-16 17:08:33.000000 pyvcd-0.4.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13333 2023-05-16 17:08:33.000000 pyvcd-0.4.0/tests/test_gtkw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-05-16 17:08:33.000000 pyvcd-0.4.0/tests/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27078 2023-05-16 17:08:33.000000 pyvcd-0.4.0/tests/test_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-16 17:08:33.000000 pyvcd-0.4.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:08:46.979321 pyvcd-0.4.0/vcd/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-16 17:08:33.000000 pyvcd-0.4.0/vcd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-05-16 17:08:33.000000 pyvcd-0.4.0/vcd/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26270 2023-05-16 17:08:33.000000 pyvcd-0.4.0/vcd/gtkw.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 17:08:33.000000 pyvcd-0.4.0/vcd/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    20126 2023-05-16 17:08:33.000000 pyvcd-0.4.0/vcd/reader.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    26995 2023-05-16 17:08:33.000000 pyvcd-0.4.0/vcd/writer.py
```

### Comparing `pyvcd-0.3.0/.github/workflows/ci.yml` & `pyvcd-0.4.0/.github/workflows/ci.yml`

 * *Files 13% similar despite different names*

```diff
@@ -8,60 +8,74 @@
     branches: [ master ]
 
 jobs:
   build:
     runs-on: ubuntu-latest
 
     steps:
-    - uses: actions/checkout@v2
-    - run: git fetch --prune --unshallow origin +refs/tags/*:refs/tags/*
+    - uses: actions/checkout@v3
+      with:
+        fetch-depth: 0
     - name: Set up Python
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
-        python-version: '3.9'
+        python-version: '3.11'
 
     - name: Install dependencies
       run: |
         python -m pip install -U pip
-        python -m pip install setuptools_scm wheel
+        python -m pip install build setuptools_scm wheel
 
     - name: Build
       run: |
-        python setup.py sdist bdist_wheel
+        python -m build
 
     - name: Upload dist
-      uses: actions/upload-artifact@v2
+      uses: actions/upload-artifact@v3
       with:
         name: pyvcd-dist
         path: "dist/*"
 
+  publish:
+    runs-on: ubuntu-latest
+    environment:
+      name: pypi
+      url: https://pypi.org/p/pyvcd
+    permissions:
+      id-token: write
+
+    steps:
+    - name: Retrieve package
+      uses: actions/download-artifact@v3
+      with:
+        name: pyvcd-dist
+        path: "dist"
+
+    - name: Display dist files
+      run: ls -Rl
+
     # - name: Test Publish package
-    #   uses: pypa/gh-action-pypi-publish@master
+    #   uses: pypa/gh-action-pypi-publish@release/v1
     #   with:
-    #     user: __token__
-    #     password: ${{ secrets.test_pypi_password }}
-    #     repository_url: https://test.pypi.org/legacy/
+    #     repository-url: https://test.pypi.org/legacy/
 
     - name: Publish package
-      if: github.event_name == 'push' && startsWith(github.event.ref, 'refs/tags')
-      uses: pypa/gh-action-pypi-publish@master
-      with:
-        user: __token__
-        password: ${{ secrets.pypi_password }}
+      if: github.event_name == 'push' && startsWith(github.ref, 'refs/tags')
+      uses: pypa/gh-action-pypi-publish@release/v1
 
   test:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ['3.6', '3.7', '3.8', '3.9', 'pypy-3.7']
+        python-version: ['3.7', '3.8', '3.9', '3.10', '3.11', 'pypy-3.7', 'pypy-3.9']
 
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
 
     - name: Install dependencies
       run: |
         python -m pip install -U pip
         python -m pip install -e . -r requirements.txt
@@ -69,35 +83,35 @@
     - name: Test
       run: |
         make test
 
   lint:
     runs-on: ubuntu-latest
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Set up Python
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
-        python-version: '3.9'
+        python-version: '3.11'
     - name: Install dependencies
       run: |
         python -m pip install -U pip
         python -m pip install -e . -r requirements.txt
     - name: Lint
       run: |
         make lint
 
   coverage:
     runs-on: ubuntu-latest
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Set up Python
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
-        python-version: '3.9'
+        python-version: '3.11'
     - name: Install dependencies
       run: |
         python -m pip install -U pip
         python -m pip install -e . -r requirements.txt coveralls
     - name: Coverage
       env:
         COVERALLS_REPO_TOKEN: ${{ secrets.COVERALLS_REPO_TOKEN }}
```

### Comparing `pyvcd-0.3.0/CHANGELOG.rst` & `pyvcd-0.4.0/CHANGELOG.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,20 @@
 Changelog
 =========
 
+pyvcd-0.4.0 (2023-05-16)
+------------------------
+* Drop official support for EOL Python 3.6 (#25)
+* Add official support for Python 3.10 and 3.11
+* Identifiers may have parens (#21)
+* Repair typing issue in vcd.gtkw.decode_flags()
+* Repair sphinx config warnings
+* Build using `build` instead of executing setup.py
+* Repair deprecated use of license_file in setup.cfg
+
 pyvcd-0.3.0 (2021-09-28)
 ------------------------
 * Add vcd.reader module for parsing VCD files
 * Various repairs to vcd.gtkw docs
 * Update setuptools and setuptools_scm requirements
 
 pyvcd-0.2.4 (2020-12-15)
```

### Comparing `pyvcd-0.3.0/CODE_OF_CONDUCT.md` & `pyvcd-0.4.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pyvcd-0.3.0/LICENSE.txt` & `pyvcd-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyvcd-0.3.0/Makefile` & `pyvcd-0.4.0/Makefile`

 * *Files 4% similar despite different names*

```diff
@@ -48,8 +48,8 @@
 
 .PHONY: build
 build:
 	$(PYTHON) setup.py build
 
 .PHONY: dist
 dist:
-	$(PYTHON) setup.py sdist bdist_wheel
+	$(PYTHON) -m build
```

### Comparing `pyvcd-0.3.0/PKG-INFO` & `pyvcd-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: pyvcd
-Version: 0.3.0
+Version: 0.4.0
 Summary: Python VCD file support
 Home-page: http://pyvcd.readthedocs.io/en/latest/
+Download-URL: https://github.com/westerndigitalcorporation/pyvcd
 Author: Peter Grayson
 Author-email: pete@jpgrayson.net
 License: MIT
-Download-URL: https://github.com/westerndigitalcorporation/pyvcd
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 
 PyVCD
 =====
 
 The PyVCD package writes Value Change Dump (VCD) files as specified in
@@ -107,9 +107,7 @@
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
-
-
```

### Comparing `pyvcd-0.3.0/README.rst` & `pyvcd-0.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `pyvcd-0.3.0/docs/Makefile` & `pyvcd-0.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyvcd-0.3.0/docs/conf.py` & `pyvcd-0.4.0/docs/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,22 +21,22 @@
 source_suffix = '.rst'
 master_doc = 'index'
 project = 'pyvcd'
 copyright = '2021, Western Digital Corporation'
 author = 'Peter Grayson and Steven Sprouse'
 version = get_version(root='..', relative_to=__file__)
 # release = '0.0.1'
-language = None
+language = 'en'
 exclude_patterns = ['_build']
 pygments_style = 'sphinx'
 todo_include_todos = False
 
 # Options for HTML output
 html_theme = 'sphinx_rtd_theme'
-html_static_path = ['_static']
+# html_static_path = ['_static']
 htmlhelp_basename = 'pyvcddoc'
 
 # Options for LaTeX output
 
 latex_elements = {}
 latex_documents = [
     (
```

### Comparing `pyvcd-0.3.0/docs/vcd.reader.rst` & `pyvcd-0.4.0/docs/vcd.reader.rst`

 * *Files identical despite different names*

### Comparing `pyvcd-0.3.0/pyvcd.egg-info/PKG-INFO` & `pyvcd-0.4.0/pyvcd.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: pyvcd
-Version: 0.3.0
+Version: 0.4.0
 Summary: Python VCD file support
 Home-page: http://pyvcd.readthedocs.io/en/latest/
+Download-URL: https://github.com/westerndigitalcorporation/pyvcd
 Author: Peter Grayson
 Author-email: pete@jpgrayson.net
 License: MIT
-Download-URL: https://github.com/westerndigitalcorporation/pyvcd
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 
 PyVCD
 =====
 
 The PyVCD package writes Value Change Dump (VCD) files as specified in
@@ -107,9 +107,7 @@
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
-
-
```

### Comparing `pyvcd-0.3.0/pyvcd.egg-info/SOURCES.txt` & `pyvcd-0.4.0/pyvcd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyvcd-0.3.0/setup.cfg` & `pyvcd-0.4.0/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -4,39 +4,40 @@
 author_email = pete@jpgrayson.net
 description = Python VCD file support
 long_description = file: README.rst, LICENSE.txt
 long_description_content_type = text/x-rst
 url = http://pyvcd.readthedocs.io/en/latest/
 download_url = https://github.com/westerndigitalcorporation/pyvcd
 license = MIT
-license_file = LICENSE.txt
+license_files = LICENSE.txt,
 classifiers = 
 	Development Status :: 4 - Beta
 	Environment :: Console
 	Intended Audience :: Developers
 	Intended Audience :: Education
 	Intended Audience :: Science/Research
 	License :: OSI Approved :: MIT License
 	Natural Language :: English
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: Implementation :: CPython
 	Programming Language :: Python :: Implementation :: PyPy
 	Topic :: Scientific/Engineering
 	Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
 
 [options]
 include_package_data = True
 zip_safe = False
-python_requires = >= 3.6
+python_requires = >= 3.7
 packages = vcd
 
 [bdist_wheel]
 universal = 1
 
 [tool:pytest]
 addopts = --doctest-glob='*.rst'
```

### Comparing `pyvcd-0.3.0/tests/test_gtkw.py` & `pyvcd-0.4.0/tests/test_gtkw.py`

 * *Files identical despite different names*

### Comparing `pyvcd-0.3.0/tests/test_reader.py` & `pyvcd-0.4.0/tests/test_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,14 +78,20 @@
 def test_parse_var_decl_with_dotted_ref():
     tokens = tokenize(io.BytesIO(b'$var real  1  aaaaa  SomeThing.MORE_STUFF_0  $end'))
     token = next(tokens)
     assert token.var.type_ == VarType.real
     assert token.var.ref_str == 'SomeThing.MORE_STUFF_0'
 
 
+def test_parse_var_decl_with_parens_in_ref_str():
+    tokens = tokenize(io.BytesIO(b'$var integer 8 !! an(ident) $end'))
+    token = next(tokens)
+    assert token.var.ref_str == 'an(ident)'
+
+
 def test_time_change():
     tokens = tokenize(io.BytesIO(b'#1234'))
     token = next(tokens)
     assert token.time_change == 1234
 
 
 def test_scalar_change():
```

### Comparing `pyvcd-0.3.0/tests/test_writer.py` & `pyvcd-0.4.0/tests/test_writer.py`

 * *Files identical despite different names*

### Comparing `pyvcd-0.3.0/vcd/common.py` & `pyvcd-0.4.0/vcd/common.py`

 * *Files identical despite different names*

### Comparing `pyvcd-0.3.0/vcd/gtkw.py` & `pyvcd-0.4.0/vcd/gtkw.py`

 * *Files 0% similar despite different names*

```diff
@@ -660,15 +660,15 @@
     :returns: List of flag names
 
     """
     if isinstance(flags, str):
         decoded = GTKWFlag(int(flags.lstrip('@'), 16))
     else:
         decoded = GTKWFlag(flags)
-    return [flag.name for flag in GTKWFlag if flag & decoded]
+    return [str(flag.name) for flag in GTKWFlag if flag & decoded]
 
 
 def spawn_gtkwave_interactive(
     dump_path: str, save_path: str, quiet: bool = False
 ) -> None:  # pragma: no cover
     """Spawn gtkwave process in interactive mode.
```

### Comparing `pyvcd-0.3.0/vcd/reader.py` & `pyvcd-0.4.0/vcd/reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -402,14 +402,16 @@
         while (
             48 <= c <= 57  # '0' - '9'
             or 65 <= c <= 90  # 'A' - 'Z'
             or 97 <= c <= 122  # 'a' - 'z'
             or c == 95  # '_'
             or c == 36  # '$'
             or c == 46  # '.' not in spec, but seen in the wild
+            or c == 40  # '(' - produced by cva6 core
+            or c == 41  # ')' - produced by cva6 core
         ):
             identifier.append(c)
             c = self.advance(raise_on_eof=False)
 
         return bytes(identifier).decode('ascii')
 
     def take_bit_index(self) -> Union[int, Tuple[int, int]]:
```

### Comparing `pyvcd-0.3.0/vcd/writer.py` & `pyvcd-0.4.0/vcd/writer.py`

 * *Files identical despite different names*

