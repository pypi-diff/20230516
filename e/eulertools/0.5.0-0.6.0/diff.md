# Comparing `tmp/eulertools-0.5.0.tar.gz` & `tmp/eulertools-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eulertools-0.5.0.tar", max compression
+gzip compressed data, was "eulertools-0.6.0.tar", max compression
```

## Comparing `eulertools-0.5.0.tar` & `eulertools-0.6.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     7652 2023-05-09 19:41:34.782813 eulertools-0.5.0/LICENSE.txt
--rw-r--r--   0        0        0      976 2023-05-09 19:41:34.788663 eulertools-0.5.0/README.rst
--rw-r--r--   0        0        0     2694 2023-05-15 10:13:58.333719 eulertools-0.5.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-09 19:41:34.789309 eulertools-0.5.0/src/eulertools/__init__.py
--rw-r--r--   0        0        0       22 2023-05-15 10:13:58.336742 eulertools-0.5.0/src/eulertools/__version__.py
--rw-r--r--   0        0        0     2879 2023-05-15 10:13:22.829230 eulertools-0.5.0/src/eulertools/compare.py
--rw-r--r--   0        0        0     1007 2023-05-15 10:13:22.829663 eulertools-0.5.0/src/eulertools/generate.py
--rw-r--r--   0        0        0     3234 2023-05-12 18:56:00.902083 eulertools-0.5.0/src/eulertools/main.py
--rw-r--r--   0        0        0     3067 2023-05-15 10:13:22.830141 eulertools-0.5.0/src/eulertools/run.py
--rw-r--r--   0        0        0      627 2023-05-15 10:13:22.830519 eulertools-0.5.0/src/eulertools/statement.py
--rw-r--r--   0        0        0     2586 2023-05-15 10:13:22.830923 eulertools-0.5.0/src/eulertools/time.py
--rw-r--r--   0        0        0     6485 2023-05-15 10:13:22.831296 eulertools-0.5.0/src/eulertools/utils.py
--rw-r--r--   0        0        0     1817 1970-01-01 00:00:00.000000 eulertools-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     7652 2023-05-09 19:41:34.782813 eulertools-0.6.0/LICENSE.txt
+-rw-r--r--   0        0        0      976 2023-05-09 19:41:34.788663 eulertools-0.6.0/README.rst
+-rw-r--r--   0        0        0     2694 2023-05-15 21:09:48.261023 eulertools-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-09 19:41:34.789309 eulertools-0.6.0/src/eulertools/__init__.py
+-rw-r--r--   0        0        0       22 2023-05-15 21:09:32.056049 eulertools-0.6.0/src/eulertools/__version__.py
+-rw-r--r--   0        0        0     2881 2023-05-15 13:24:16.965570 eulertools-0.6.0/src/eulertools/compare.py
+-rw-r--r--   0        0        0     1007 2023-05-15 10:13:22.829663 eulertools-0.6.0/src/eulertools/generate.py
+-rw-r--r--   0        0        0     3234 2023-05-12 18:56:00.902083 eulertools-0.6.0/src/eulertools/main.py
+-rw-r--r--   0        0        0     3175 2023-05-15 13:31:53.522885 eulertools-0.6.0/src/eulertools/run.py
+-rw-r--r--   0        0        0      627 2023-05-15 10:13:22.830519 eulertools-0.6.0/src/eulertools/statement.py
+-rw-r--r--   0        0        0     2586 2023-05-15 13:30:41.006142 eulertools-0.6.0/src/eulertools/time.py
+-rw-r--r--   0        0        0     6485 2023-05-15 10:13:22.831296 eulertools-0.6.0/src/eulertools/utils.py
+-rw-r--r--   0        0        0     1817 1970-01-01 00:00:00.000000 eulertools-0.6.0/PKG-INFO
```

### Comparing `eulertools-0.5.0/LICENSE.txt` & `eulertools-0.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `eulertools-0.5.0/README.rst` & `eulertools-0.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `eulertools-0.5.0/pyproject.toml` & `eulertools-0.6.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -98,15 +98,15 @@
 [tool.coverage.report]
 show_missing = true
 skip_covered = true
 skip_empty = true
 
 [tool.poetry]
 name = "eulertools"
-version = "0.5.0"
+version = "0.6.0"
 description = "Multilanguage competitive coding toolbox"
 authors = [
     "Stephanos Kuma <stephanos@kuma.ai>",
 ]
 
 license = "LGPL-3.0+"
 readme = "README.rst"
```

### Comparing `eulertools-0.5.0/src/eulertools/compare.py` & `eulertools-0.6.0/src/eulertools/compare.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
             ["problem", *(f"{problem}/{key}" for problem, key in self.keyed_problems)],
             *(self.get_language_timings(language) for language in self.languages),
         ]
         self.print_table(self.transpose(matrix))
 
     def print_table(self, matrix: list[list[str]]) -> None:
         if len(matrix) == 1:
-            raise ValueError("No data to print")
+            raise RuntimeError("No data to print")
         n = len(self.languages) + 1
         spacing = ["─" * self.pad_length for _ in range(n)]
         top = "┌" + "┬".join(spacing) + "┐"
         mid = "├" + "┼".join(spacing) + "┤"
         btm = "└" + "┴".join(spacing) + "┘"
         print(top)
         for i, row in enumerate(matrix):
```

### Comparing `eulertools-0.5.0/src/eulertools/generate.py` & `eulertools-0.6.0/src/eulertools/generate.py`

 * *Files identical despite different names*

### Comparing `eulertools-0.5.0/src/eulertools/main.py` & `eulertools-0.6.0/src/eulertools/main.py`

 * *Files identical despite different names*

### Comparing `eulertools-0.5.0/src/eulertools/run.py` & `eulertools-0.6.0/src/eulertools/run.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,26 +18,30 @@
         self.problems = problems
         self.mode = mode
         self.times = times
         self.verbosity = verbosity
 
     def run(self) -> dict[Language, dict[str, dict[int, list[int]]]]:
         output: dict[Language, dict[str, dict[int, list[int]]]] = {}
+        success = True
         for language, problem in product(self.languages, self.problems):
-            timings = self.run_single_problem(language, problem)
-            if timings is not None:
+            run_success, timings = self.run_single_problem(language, problem)
+            if run_success is not None:
+                success = success and run_success
                 output.setdefault(language, {})[problem] = timings
+        if not success:
+            raise RuntimeError("Some tests failed")
         return output
 
     def run_single_problem(
         self, language: Language, problem: str
-    ) -> dict[int, list[int]] | None:
+    ) -> tuple[bool | None, dict[int, list[int]]]:
         solution = get_solution(language, problem)
         if not solution.exists():
-            return None
+            return None, {}
         raw_output = subprocess.run(
             [language.runner, problem, str(self.times)],  # noqa: S603
             capture_output=True,
         )
         output = raw_output.stdout.decode()
         if self.verbosity > 3:
             print(output)
@@ -70,10 +74,8 @@
             elif value != expected_answers[key]:
                 success = False
                 print(
                     f"🔴 Running {language.name}/{problem}/{key}... expected: {expected_answers[key]}, got: {value}"
                 )
             elif self.mode != Modes.TIMING:
                 print(f"🟢 Running {language.name}/{problem}/{key}... {value}")
-        if not success:
-            raise ValueError("Running failed. Aborting...")
-        return timings
+        return success, timings
```

### Comparing `eulertools-0.5.0/src/eulertools/statement.py` & `eulertools-0.6.0/src/eulertools/statement.py`

 * *Files identical despite different names*

### Comparing `eulertools-0.5.0/src/eulertools/time.py` & `eulertools-0.6.0/src/eulertools/time.py`

 * *Files identical despite different names*

### Comparing `eulertools-0.5.0/src/eulertools/utils.py` & `eulertools-0.6.0/src/eulertools/utils.py`

 * *Files identical despite different names*

### Comparing `eulertools-0.5.0/PKG-INFO` & `eulertools-0.6.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eulertools
-Version: 0.5.0
+Version: 0.6.0
 Summary: Multilanguage competitive coding toolbox
 Home-page: https://eulertools.readthedocs.io/en/latest/
 License: LGPL-3.0+
 Keywords: leetcode,topcoder,project_euler
 Author: Stephanos Kuma
 Author-email: stephanos@kuma.ai
 Requires-Python: >=3.11,<4.0
```

