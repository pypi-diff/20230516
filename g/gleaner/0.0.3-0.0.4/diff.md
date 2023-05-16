# Comparing `tmp/gleaner-0.0.3.tar.gz` & `tmp/gleaner-0.0.4.tar.gz`

## Comparing `gleaner-0.0.3.tar` & `gleaner-0.0.4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 gleaner-0.0.3/gleaner/__about__.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 gleaner-0.0.3/gleaner/__init__.py
--rw-r--r--   0        0        0     3122 2020-02-02 00:00:00.000000 gleaner-0.0.3/gleaner/config.py
--rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 gleaner-0.0.3/gleaner/gleaner.py
--rw-r--r--   0        0        0     1956 2020-02-02 00:00:00.000000 gleaner-0.0.3/gleaner/utill.py
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 gleaner-0.0.3/gleaner/explorer/__init__.py
--rw-r--r--   0        0        0     6734 2020-02-02 00:00:00.000000 gleaner-0.0.3/gleaner/explorer/explorer.py
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 gleaner-0.0.3/gleaner/explorer/explorer_config.py
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 gleaner-0.0.3/gleaner/explorer/explorer_result.py
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 gleaner-0.0.3/gleaner/generator/__init__.py
--rw-r--r--   0        0        0     2906 2020-02-02 00:00:00.000000 gleaner-0.0.3/gleaner/generator/generator.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 gleaner-0.0.3/gleaner/generator/generator_config.py
--rw-r--r--   0        0        0     2669 2020-02-02 00:00:00.000000 gleaner-0.0.3/gleaner/generator/generator_parameters.py
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 gleaner-0.0.3/gleaner/model/__init__.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 gleaner-0.0.3/gleaner/model/attribute.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 gleaner-0.0.3/gleaner/model/data_transforms.py
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 gleaner-0.0.3/gleaner/model/encodings.py
--rw-r--r--   0        0        0    14124 2020-02-02 00:00:00.000000 gleaner-0.0.3/gleaner/model/gleaner_chart.py
--rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 gleaner-0.0.3/gleaner/model/gleaner_dahsboard.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 gleaner-0.0.3/gleaner/oracle/__init__.py
--rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 gleaner-0.0.3/gleaner/oracle/oracle.py
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 gleaner-0.0.3/gleaner/oracle/oracle_result.py
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 gleaner-0.0.3/gleaner/oracle/oracle_weight.py
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 gleaner-0.0.3/gleaner/oracle/scores/__init__.py
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 gleaner-0.0.3/gleaner/oracle/scores/anova.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 gleaner-0.0.3/gleaner/oracle/scores/conciseness.py
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 gleaner-0.0.3/gleaner/oracle/scores/coverage.py
--rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 gleaner-0.0.3/gleaner/oracle/scores/diversity.py
--rw-r--r--   0        0        0     5097 2020-02-02 00:00:00.000000 gleaner-0.0.3/gleaner/oracle/scores/interestingness.py
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 gleaner-0.0.3/gleaner/oracle/scores/specificity.py
--rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 gleaner-0.0.3/.gitignore
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 gleaner-0.0.3/LICENSE
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 gleaner-0.0.3/README.md
--rw-r--r--   0        0        0     3279 2020-02-02 00:00:00.000000 gleaner-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2646 2020-02-02 00:00:00.000000 gleaner-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 gleaner-0.0.4/gleaner/__about__.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 gleaner-0.0.4/gleaner/__init__.py
+-rw-r--r--   0        0        0     3121 2020-02-02 00:00:00.000000 gleaner-0.0.4/gleaner/config.py
+-rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 gleaner-0.0.4/gleaner/gleaner.py
+-rw-r--r--   0        0        0     1956 2020-02-02 00:00:00.000000 gleaner-0.0.4/gleaner/utill.py
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 gleaner-0.0.4/gleaner/explorer/__init__.py
+-rw-r--r--   0        0        0     6830 2020-02-02 00:00:00.000000 gleaner-0.0.4/gleaner/explorer/explorer.py
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 gleaner-0.0.4/gleaner/explorer/explorer_config.py
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 gleaner-0.0.4/gleaner/explorer/explorer_result.py
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 gleaner-0.0.4/gleaner/generator/__init__.py
+-rw-r--r--   0        0        0     2906 2020-02-02 00:00:00.000000 gleaner-0.0.4/gleaner/generator/generator.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 gleaner-0.0.4/gleaner/generator/generator_config.py
+-rw-r--r--   0        0        0     2669 2020-02-02 00:00:00.000000 gleaner-0.0.4/gleaner/generator/generator_parameters.py
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 gleaner-0.0.4/gleaner/model/__init__.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 gleaner-0.0.4/gleaner/model/attribute.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 gleaner-0.0.4/gleaner/model/data_transforms.py
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 gleaner-0.0.4/gleaner/model/encodings.py
+-rw-r--r--   0        0        0    14124 2020-02-02 00:00:00.000000 gleaner-0.0.4/gleaner/model/gleaner_chart.py
+-rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 gleaner-0.0.4/gleaner/model/gleaner_dahsboard.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 gleaner-0.0.4/gleaner/oracle/__init__.py
+-rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 gleaner-0.0.4/gleaner/oracle/oracle.py
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 gleaner-0.0.4/gleaner/oracle/oracle_result.py
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 gleaner-0.0.4/gleaner/oracle/oracle_weight.py
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 gleaner-0.0.4/gleaner/oracle/scores/__init__.py
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 gleaner-0.0.4/gleaner/oracle/scores/anova.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 gleaner-0.0.4/gleaner/oracle/scores/conciseness.py
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 gleaner-0.0.4/gleaner/oracle/scores/coverage.py
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 gleaner-0.0.4/gleaner/oracle/scores/diversity.py
+-rw-r--r--   0        0        0     5097 2020-02-02 00:00:00.000000 gleaner-0.0.4/gleaner/oracle/scores/interestingness.py
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 gleaner-0.0.4/gleaner/oracle/scores/specificity.py
+-rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 gleaner-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 gleaner-0.0.4/LICENSE
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 gleaner-0.0.4/README.md
+-rw-r--r--   0        0        0     3279 2020-02-02 00:00:00.000000 gleaner-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2646 2020-02-02 00:00:00.000000 gleaner-0.0.4/PKG-INFO
```

### Comparing `gleaner-0.0.3/gleaner/config.py` & `gleaner-0.0.4/gleaner/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,15 @@
     n_candidates: int
     halving_ratio: float
 
     def __init__(
         self,
         df: pd.DataFrame,
         robustness: int = 150,
-        n_epoch: int = 50,
+        n_epoch: int = 5,
         n_candidates: int = 100,
         halving_ratio: float = 0.1,
     ) -> None:
         self.robustness = robustness
         self.n_epoch = n_epoch
         self.n_candidates = n_candidates
         self.halving_ratio = halving_ratio
```

### Comparing `gleaner-0.0.3/gleaner/gleaner.py` & `gleaner-0.0.4/gleaner/gleaner.py`

 * *Files identical despite different names*

### Comparing `gleaner-0.0.3/gleaner/utill.py` & `gleaner-0.0.4/gleaner/utill.py`

 * *Files identical despite different names*

### Comparing `gleaner-0.0.3/gleaner/explorer/explorer.py` & `gleaner-0.0.4/gleaner/explorer/explorer.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,15 +90,19 @@
             + interestingness * oracle.weight.interestingness
             + coverage * oracle.weight.coverage
             + diversity * oracle.weight.diversity
             + conciseness * oracle.weight.conciseness
         )
 
         normalized_scores = (
-            (specificity - specificity.mean()) / specificity.std() * oracle.weight.specificity
+            (
+                0
+                if len(preferences) == 0
+                else (specificity - specificity.mean()) / specificity.std() * oracle.weight.specificity
+            )
             + (interestingness - interestingness.mean()) / interestingness.std() * oracle.weight.interestingness
             + (coverage - coverage.mean()) / coverage.std() * oracle.weight.coverage
             + (diversity - diversity.mean()) / diversity.std() * oracle.weight.diversity
             + (conciseness - conciseness.mean()) / conciseness.std() * oracle.weight.conciseness
         )
 
         result_n_scores: list[tuple[OracleResult, GleanerDashboard, float, float]] = [
```

### Comparing `gleaner-0.0.3/gleaner/generator/generator.py` & `gleaner-0.0.4/gleaner/generator/generator.py`

 * *Files identical despite different names*

### Comparing `gleaner-0.0.3/gleaner/generator/generator_parameters.py` & `gleaner-0.0.4/gleaner/generator/generator_parameters.py`

 * *Files identical despite different names*

### Comparing `gleaner-0.0.3/gleaner/model/data_transforms.py` & `gleaner-0.0.4/gleaner/model/data_transforms.py`

 * *Files identical despite different names*

### Comparing `gleaner-0.0.3/gleaner/model/gleaner_chart.py` & `gleaner-0.0.4/gleaner/model/gleaner_chart.py`

 * *Files identical despite different names*

### Comparing `gleaner-0.0.3/gleaner/model/gleaner_dahsboard.py` & `gleaner-0.0.4/gleaner/model/gleaner_dahsboard.py`

 * *Files identical despite different names*

### Comparing `gleaner-0.0.3/gleaner/oracle/oracle.py` & `gleaner-0.0.4/gleaner/oracle/oracle.py`

 * *Files identical despite different names*

### Comparing `gleaner-0.0.3/gleaner/oracle/oracle_result.py` & `gleaner-0.0.4/gleaner/oracle/oracle_result.py`

 * *Files identical despite different names*

### Comparing `gleaner-0.0.3/gleaner/oracle/scores/anova.py` & `gleaner-0.0.4/gleaner/oracle/scores/anova.py`

 * *Files identical despite different names*

### Comparing `gleaner-0.0.3/gleaner/oracle/scores/diversity.py` & `gleaner-0.0.4/gleaner/oracle/scores/diversity.py`

 * *Files identical despite different names*

### Comparing `gleaner-0.0.3/gleaner/oracle/scores/interestingness.py` & `gleaner-0.0.4/gleaner/oracle/scores/interestingness.py`

 * *Files identical despite different names*

### Comparing `gleaner-0.0.3/.gitignore` & `gleaner-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `gleaner-0.0.3/LICENSE` & `gleaner-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gleaner-0.0.3/README.md` & `gleaner-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `gleaner-0.0.3/pyproject.toml` & `gleaner-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gleaner-0.0.3/PKG-INFO` & `gleaner-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gleaner
-Version: 0.0.3
+Version: 0.0.4
 Summary: Gleaner: Multi-Criteria Optimization for Automatic Dashboard Design
 Project-URL: Documentation, https://github.com/jason-choi/gleaner
 Project-URL: Issues, https://github.com/jason-choi/gleaner/issues
 Project-URL: Source, https://github.com/jason-choi/gleaner
 Author-email: Jason Choi <jasonchoi3@g.skku.edu>
 License-Expression: MIT
 License-File: LICENSE
```

