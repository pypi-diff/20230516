# Comparing `tmp/fvalues-0.0.3.tar.gz` & `tmp/fvalues-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fvalues-0.0.3.tar", last modified: Wed Jan 25 13:02:20 2023, max compression
+gzip compressed data, was "fvalues-0.0.4.tar", last modified: Tue May 16 13:21:58 2023, max compression
```

## Comparing `fvalues-0.0.3.tar` & `fvalues-0.0.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-01-25 13:02:20.073968 fvalues-0.0.3/
--rw-rw-r--   0 alex      (1000) alex      (1000)       97 2022-12-15 22:36:26.000000 fvalues-0.0.3/.flake8
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-01-25 13:02:20.069968 fvalues-0.0.3/.github/
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-01-25 13:02:20.069968 fvalues-0.0.3/.github/workflows/
--rw-rw-r--   0 alex      (1000) alex      (1000)     1091 2023-01-25 12:57:52.000000 fvalues-0.0.3/.github/workflows/tests.yml
--rw-rw-r--   0 alex      (1000) alex      (1000)      142 2022-12-16 01:45:37.000000 fvalues-0.0.3/.gitignore
--rw-rw-r--   0 alex      (1000) alex      (1000)      842 2022-12-20 12:50:02.000000 fvalues-0.0.3/.pre-commit-config.yaml
--rw-rw-r--   0 alex      (1000) alex      (1000)   362354 2023-01-25 12:57:52.000000 fvalues-0.0.3/ICE.jpeg
--rw-rw-r--   0 alex      (1000) alex      (1000)     1062 2022-11-16 09:43:50.000000 fvalues-0.0.3/LICENSE.md
--rw-rw-r--   0 alex      (1000) alex      (1000)     4656 2023-01-25 13:02:20.073968 fvalues-0.0.3/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)     4091 2023-01-25 12:57:52.000000 fvalues-0.0.3/README.md
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-01-25 13:02:20.069968 fvalues-0.0.3/fvalues/
--rw-rw-r--   0 alex      (1000) alex      (1000)      339 2022-12-16 05:28:05.000000 fvalues-0.0.3/fvalues/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    13527 2023-01-25 12:57:52.000000 fvalues-0.0.3/fvalues/f.py
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-12-05 11:03:08.000000 fvalues-0.0.3/fvalues/py.typed
--rw-rw-r--   0 alex      (1000) alex      (1000)       22 2023-01-25 13:02:20.000000 fvalues-0.0.3/fvalues/version.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-01-25 13:02:20.073968 fvalues-0.0.3/fvalues.egg-info/
--rw-rw-r--   0 alex      (1000) alex      (1000)     4656 2023-01-25 13:02:20.000000 fvalues-0.0.3/fvalues.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)      392 2023-01-25 13:02:20.000000 fvalues-0.0.3/fvalues.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-01-25 13:02:20.000000 fvalues-0.0.3/fvalues.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       74 2023-01-25 13:02:20.000000 fvalues-0.0.3/fvalues.egg-info/requires.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        8 2023-01-25 13:02:20.000000 fvalues-0.0.3/fvalues.egg-info/top_level.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)      367 2022-12-16 01:16:35.000000 fvalues-0.0.3/mypy.ini
--rw-rw-r--   0 alex      (1000) alex      (1000)      331 2022-12-15 22:32:40.000000 fvalues-0.0.3/pyproject.toml
--rwxrwxr-x   0 alex      (1000) alex      (1000)      596 2022-12-20 12:53:52.000000 fvalues-0.0.3/release.sh
--rw-rw-r--   0 alex      (1000) alex      (1000)      878 2023-01-25 13:02:20.073968 fvalues-0.0.3/setup.cfg
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-01-25 13:02:20.073968 fvalues-0.0.3/tests/
--rw-rw-r--   0 alex      (1000) alex      (1000)     8715 2023-01-25 12:57:52.000000 fvalues-0.0.3/tests/test_f.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      100 2022-12-17 01:13:11.000000 fvalues-0.0.3/tox.ini
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-16 13:21:58.684094 fvalues-0.0.4/
+-rw-rw-r--   0 alex      (1000) alex      (1000)       97 2022-12-15 22:36:26.000000 fvalues-0.0.4/.flake8
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-16 13:21:58.680094 fvalues-0.0.4/.github/
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-16 13:21:58.684094 fvalues-0.0.4/.github/workflows/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1091 2023-01-25 12:57:52.000000 fvalues-0.0.4/.github/workflows/tests.yml
+-rw-rw-r--   0 alex      (1000) alex      (1000)      142 2022-12-16 01:45:37.000000 fvalues-0.0.4/.gitignore
+-rw-rw-r--   0 alex      (1000) alex      (1000)      841 2023-05-16 13:20:01.000000 fvalues-0.0.4/.pre-commit-config.yaml
+-rw-rw-r--   0 alex      (1000) alex      (1000)   362354 2023-01-25 12:57:52.000000 fvalues-0.0.4/ICE.jpeg
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1062 2022-11-16 09:43:50.000000 fvalues-0.0.4/LICENSE.md
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4656 2023-05-16 13:21:58.684094 fvalues-0.0.4/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4091 2023-01-25 12:57:52.000000 fvalues-0.0.4/README.md
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-16 13:21:58.684094 fvalues-0.0.4/fvalues/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      339 2022-12-16 05:28:05.000000 fvalues-0.0.4/fvalues/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    14347 2023-05-16 13:20:01.000000 fvalues-0.0.4/fvalues/f.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-12-05 11:03:08.000000 fvalues-0.0.4/fvalues/py.typed
+-rw-rw-r--   0 alex      (1000) alex      (1000)       22 2023-05-16 13:21:58.000000 fvalues-0.0.4/fvalues/version.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-16 13:21:58.684094 fvalues-0.0.4/fvalues.egg-info/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4656 2023-05-16 13:21:58.000000 fvalues-0.0.4/fvalues.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)      392 2023-05-16 13:21:58.000000 fvalues-0.0.4/fvalues.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-05-16 13:21:58.000000 fvalues-0.0.4/fvalues.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       74 2023-05-16 13:21:58.000000 fvalues-0.0.4/fvalues.egg-info/requires.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        8 2023-05-16 13:21:58.000000 fvalues-0.0.4/fvalues.egg-info/top_level.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)      367 2022-12-16 01:16:35.000000 fvalues-0.0.4/mypy.ini
+-rw-rw-r--   0 alex      (1000) alex      (1000)      331 2022-12-15 22:32:40.000000 fvalues-0.0.4/pyproject.toml
+-rwxrwxr-x   0 alex      (1000) alex      (1000)      596 2022-12-20 12:53:52.000000 fvalues-0.0.4/release.sh
+-rw-rw-r--   0 alex      (1000) alex      (1000)      878 2023-05-16 13:21:58.684094 fvalues-0.0.4/setup.cfg
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-16 13:21:58.684094 fvalues-0.0.4/tests/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9660 2023-05-16 13:20:01.000000 fvalues-0.0.4/tests/test_f.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      100 2022-12-17 01:13:11.000000 fvalues-0.0.4/tox.ini
```

### Comparing `fvalues-0.0.3/.github/workflows/tests.yml` & `fvalues-0.0.4/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `fvalues-0.0.3/.pre-commit-config.yaml` & `fvalues-0.0.4/.pre-commit-config.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -12,20 +12,20 @@
       - id: trailing-whitespace
   - repo: https://github.com/asottile/reorder_python_imports
     rev: v3.9.0
     hooks:
       - id: reorder-python-imports
         args: [--py39-plus]
   - repo: https://github.com/psf/black
-    rev: 22.12.0
+    rev: 23.1.0
     hooks:
       - id: black
   - repo: https://github.com/PyCQA/flake8
     rev: 6.0.0
     hooks:
       - id: flake8
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v0.991
+    rev: v1.0.1
     hooks:
       - id: mypy
         additional_dependencies: [pytest]
         args: [--config-file, mypy.ini]
```

### Comparing `fvalues-0.0.3/ICE.jpeg` & `fvalues-0.0.4/ICE.jpeg`

 * *Files identical despite different names*

### Comparing `fvalues-0.0.3/LICENSE.md` & `fvalues-0.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `fvalues-0.0.3/PKG-INFO` & `fvalues-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fvalues
-Version: 0.0.3
+Version: 0.0.4
 Summary: Keep track of components in strings, especially formatted values in f-strings.
 Home-page: https://github.com/oughtinc/fvalues
 Author: Alex Hall
 Author-email: alex.mojaki@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `fvalues-0.0.3/README.md` & `fvalues-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `fvalues-0.0.3/fvalues/f.py` & `fvalues-0.0.4/fvalues/f.py`

 * *Files 3% similar despite different names*

```diff
@@ -300,14 +300,38 @@
 
             if iterable_source:
                 parts.append(FValue(f"{iterable_source}[{i}]", item, str(item)))
             else:
                 parts.append(item)
         return F(str(self).join(map(str, iterable)), tuple(parts))
 
+    def preserved_join(self, iterable: Iterable[str]) -> "F":
+        """Join strings while preserving regular strings.
+
+        Normally, joined strings will all become FValues. However, sometimes we want
+        to preserve them as regular strings instead of FValues. This function allows
+        for that option.
+        """
+        joined = ""
+        parts = []
+        for substring in iterable:
+            joined += substring
+            parts.append(substring)
+
+            # avoid polluting parts when joining with empty string
+            if str(self) != "":
+                joined += self
+                parts.append(self)
+
+        if len(parts) > 0 and str(self) != "":  # pop the last joiner
+            joined = joined[: -len(self)]
+            parts.pop()
+
+        return F(joined, parts=tuple(parts))
+
 
 def get_frame() -> FrameType:
     """
     Return the frame which is calling the function which is calling this.
     """
     return inspect.currentframe().f_back.f_back  # type: ignore
```

### Comparing `fvalues-0.0.3/fvalues.egg-info/PKG-INFO` & `fvalues-0.0.4/fvalues.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fvalues
-Version: 0.0.3
+Version: 0.0.4
 Summary: Keep track of components in strings, especially formatted values in f-strings.
 Home-page: https://github.com/oughtinc/fvalues
 Author: Alex Hall
 Author-email: alex.mojaki@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `fvalues-0.0.3/release.sh` & `fvalues-0.0.4/release.sh`

 * *Files identical despite different names*

### Comparing `fvalues-0.0.3/setup.cfg` & `fvalues-0.0.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `fvalues-0.0.3/tests/test_f.py` & `fvalues-0.0.4/tests/test_f.py`

 * *Files 6% similar despite different names*

```diff
@@ -284,14 +284,57 @@
 def test_join_bad_source():
     strings = ["a", "b", "c"]
     s = F.join(F(","), strings)
     assert s == "a,b,c"
     assert s.parts == s.flatten().parts == ("a", ",", "b", ",", "c")
 
 
+def test_preserved_join_empty():
+    s = F(" ").preserved_join([])
+    assert s == F("", parts=("",))
+
+
+def test_preserved_join_list():
+    b = 2
+    s = F(" ").preserved_join(["a", F(f"b={b}"), "c"])
+    assert s == "a b=2 c"
+    assert s.parts == (
+        "a",
+        " ",
+        F(f"b={b}", parts=("b=", FValue(source="b", value=2, formatted="2"))),
+        " ",
+        "c",
+    )
+    assert s.flatten().parts == (
+        "a",
+        " ",
+        "b=",
+        FValue(source="b", value=2, formatted="2"),
+        " ",
+        "c",
+    )
+
+
+def test_preserved_join_empty_string():
+    b = 2
+    s = F("").preserved_join(["a", F(f"b={b}"), "c"])
+    assert s == "ab=2c"
+    assert s.parts == (
+        "a",
+        F(f"b={b}", parts=("b=", FValue(source="b", value=2, formatted="2"))),
+        "c",
+    )
+    assert s.flatten().parts == (
+        "a",
+        "b=",
+        FValue(source="b", value=2, formatted="2"),
+        "c",
+    )
+
+
 def test_deserialization():
     # pyyaml deserialization reconstructs F with multiple arguments:
     # https://github.com/yaml/pyyaml/blob/957ae4d/lib/yaml/constructor.py#L591
     # make sure that there is no error resulting from this
     cls = F
     args = ["test_str"]
     kwds: Dict[str, Any] = {}
```

