# Comparing `tmp/gleaner-0.0.2.tar.gz` & `tmp/gleaner-0.0.3.tar.gz`

## Comparing `gleaner-0.0.2.tar` & `gleaner-0.0.3.tar`

### file list

```diff
@@ -1,38 +1,35 @@
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 gleaner-0.0.2/requirements.txt
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 gleaner-0.0.2/gleaner/__about__.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 gleaner-0.0.2/gleaner/__init__.py
--rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 gleaner-0.0.2/gleaner/config.py
--rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 gleaner-0.0.2/gleaner/gleaner.py
--rw-r--r--   0        0        0     1956 2020-02-02 00:00:00.000000 gleaner-0.0.2/gleaner/utill.py
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 gleaner-0.0.2/gleaner/explorer/__init__.py
--rw-r--r--   0        0        0     5999 2020-02-02 00:00:00.000000 gleaner-0.0.2/gleaner/explorer/explorer.py
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 gleaner-0.0.2/gleaner/explorer/explorer_config.py
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 gleaner-0.0.2/gleaner/explorer/explorer_result.py
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 gleaner-0.0.2/gleaner/generator/__init__.py
--rw-r--r--   0        0        0     2906 2020-02-02 00:00:00.000000 gleaner-0.0.2/gleaner/generator/generator.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 gleaner-0.0.2/gleaner/generator/generator_config.py
--rw-r--r--   0        0        0     2669 2020-02-02 00:00:00.000000 gleaner-0.0.2/gleaner/generator/generator_parameters.py
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 gleaner-0.0.2/gleaner/model/__init__.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 gleaner-0.0.2/gleaner/model/attribute.py
--rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 gleaner-0.0.2/gleaner/model/chart_type.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 gleaner-0.0.2/gleaner/model/data_transforms.py
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 gleaner-0.0.2/gleaner/model/encodings.py
--rw-r--r--   0        0        0    13652 2020-02-02 00:00:00.000000 gleaner-0.0.2/gleaner/model/gleaner_chart.py
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 gleaner-0.0.2/gleaner/model/gleaner_dahsboard.py
--rw-r--r--   0        0        0     2673 2020-02-02 00:00:00.000000 gleaner-0.0.2/gleaner/model/task_type.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 gleaner-0.0.2/gleaner/oracle/__init__.py
--rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 gleaner-0.0.2/gleaner/oracle/oracle.py
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 gleaner-0.0.2/gleaner/oracle/oracle_result.py
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 gleaner-0.0.2/gleaner/oracle/oracle_weight.py
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 gleaner-0.0.2/gleaner/oracle/scores/__init__.py
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 gleaner-0.0.2/gleaner/oracle/scores/anova.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 gleaner-0.0.2/gleaner/oracle/scores/conciseness.py
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 gleaner-0.0.2/gleaner/oracle/scores/coverage.py
--rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 gleaner-0.0.2/gleaner/oracle/scores/diversity.py
--rw-r--r--   0        0        0     5055 2020-02-02 00:00:00.000000 gleaner-0.0.2/gleaner/oracle/scores/interestingness.py
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 gleaner-0.0.2/gleaner/oracle/scores/specificity.py
--rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 gleaner-0.0.2/.gitignore
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 gleaner-0.0.2/LICENSE
--rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 gleaner-0.0.2/README.md
--rw-r--r--   0        0        0     3222 2020-02-02 00:00:00.000000 gleaner-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 gleaner-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 gleaner-0.0.3/gleaner/__about__.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 gleaner-0.0.3/gleaner/__init__.py
+-rw-r--r--   0        0        0     3122 2020-02-02 00:00:00.000000 gleaner-0.0.3/gleaner/config.py
+-rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 gleaner-0.0.3/gleaner/gleaner.py
+-rw-r--r--   0        0        0     1956 2020-02-02 00:00:00.000000 gleaner-0.0.3/gleaner/utill.py
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 gleaner-0.0.3/gleaner/explorer/__init__.py
+-rw-r--r--   0        0        0     6734 2020-02-02 00:00:00.000000 gleaner-0.0.3/gleaner/explorer/explorer.py
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 gleaner-0.0.3/gleaner/explorer/explorer_config.py
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 gleaner-0.0.3/gleaner/explorer/explorer_result.py
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 gleaner-0.0.3/gleaner/generator/__init__.py
+-rw-r--r--   0        0        0     2906 2020-02-02 00:00:00.000000 gleaner-0.0.3/gleaner/generator/generator.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 gleaner-0.0.3/gleaner/generator/generator_config.py
+-rw-r--r--   0        0        0     2669 2020-02-02 00:00:00.000000 gleaner-0.0.3/gleaner/generator/generator_parameters.py
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 gleaner-0.0.3/gleaner/model/__init__.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 gleaner-0.0.3/gleaner/model/attribute.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 gleaner-0.0.3/gleaner/model/data_transforms.py
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 gleaner-0.0.3/gleaner/model/encodings.py
+-rw-r--r--   0        0        0    14124 2020-02-02 00:00:00.000000 gleaner-0.0.3/gleaner/model/gleaner_chart.py
+-rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 gleaner-0.0.3/gleaner/model/gleaner_dahsboard.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 gleaner-0.0.3/gleaner/oracle/__init__.py
+-rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 gleaner-0.0.3/gleaner/oracle/oracle.py
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 gleaner-0.0.3/gleaner/oracle/oracle_result.py
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 gleaner-0.0.3/gleaner/oracle/oracle_weight.py
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 gleaner-0.0.3/gleaner/oracle/scores/__init__.py
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 gleaner-0.0.3/gleaner/oracle/scores/anova.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 gleaner-0.0.3/gleaner/oracle/scores/conciseness.py
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 gleaner-0.0.3/gleaner/oracle/scores/coverage.py
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 gleaner-0.0.3/gleaner/oracle/scores/diversity.py
+-rw-r--r--   0        0        0     5097 2020-02-02 00:00:00.000000 gleaner-0.0.3/gleaner/oracle/scores/interestingness.py
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 gleaner-0.0.3/gleaner/oracle/scores/specificity.py
+-rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 gleaner-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 gleaner-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 gleaner-0.0.3/README.md
+-rw-r--r--   0        0        0     3279 2020-02-02 00:00:00.000000 gleaner-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2646 2020-02-02 00:00:00.000000 gleaner-0.0.3/PKG-INFO
```

### Comparing `gleaner-0.0.2/gleaner/config.py` & `gleaner-0.0.3/gleaner/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -74,24 +74,26 @@
         n_candidates: int = 100,
         halving_ratio: float = 0.1,
     ) -> None:
         self.robustness = robustness
         self.n_epoch = n_epoch
         self.n_candidates = n_candidates
         self.halving_ratio = halving_ratio
-
         self.df = df
+        self.init_constraints()
+
+    def give_constraints(self, constraints: list[str]):
+        self.attr_names = [m for m in self.attr_names if m not in constraints]
+        self.chart_type = [m for m in self.chart_type if m not in constraints]
+        self.agg_type = [m for m in self.agg_type if m not in constraints]
+
+    def init_constraints(self):
         self.attr_names = [
             col
-            for col in df.columns
-            if (df[col].dtype == "object" and df[col].nunique() < 10) or df[col].dtype != "object"
+            for col in self.df.columns
+            if (self.df[col].dtype == "object" and self.df[col].nunique() < 10) or self.df[col].dtype != "object"
         ]
         self.attrs: list[Attribute] = [
-            Attribute(col, "C" if df[col].dtype == "object" else "Q") for col in self.attr_names
+            Attribute(col, "C" if self.df[col].dtype == "object" else "Q") for col in self.attr_names
         ]
         self.chart_type = list(set([m[0] for m in chart_map]))
         self.agg_type = list(set([m[-1] for m in chart_map]))
-
-    def constraint(self, constraint: list[str]):
-        self.attr_names = [m for m in self.attr_names if m not in constraint]
-        self.chart_type = [m for m in self.chart_type if m not in constraint]
-        self.agg_type = [m for m in self.agg_type if m not in constraint]
```

### Comparing `gleaner-0.0.2/gleaner/gleaner.py` & `gleaner-0.0.3/gleaner/gleaner.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from dataclasses import dataclass
 import pandas as pd
 
 from gleaner.explorer import Explorer, TrainResult
 from gleaner.generator import Generator
-from gleaner.model import GleanerDashboard
+from gleaner.model import GleanerDashboard, GleanerChart
 from gleaner.config import GleanerConfig
 from gleaner.oracle import Oracle
 from gleaner.utill import display_function
 
 
 class Gleaner:
     oracle: Oracle
@@ -30,9 +30,20 @@
             train_results.append(train_result)
             display_function(epoch, train_results)
 
     def train(self, preferences: list[str]) -> list[TrainResult]:
         self.preferences = preferences
         return self.explorer.train(self.generator, self.oracle, preferences)
 
-    def infer(self) -> GleanerDashboard:
-        return self.explorer.infer(self.generator, self.oracle, self.preferences)
+    def infer(self, n_chart: int | None = None, fixed_charts: list[list[str | None]] = []) -> GleanerDashboard:
+        return self.explorer.infer(self.generator, self.oracle, self.preferences, n_chart, fixed_charts)
+
+    def recommend(self, dashboard: GleanerDashboard, n_results: int = 5) -> list[GleanerChart]:
+        inferred_charts = self.explorer._infer(
+            self.generator,
+            self.oracle,
+            self.preferences,
+            n_chart=len(dashboard) + 1,
+            fixed_charts=dashboard.charts,
+        )[0][:n_results]
+
+        return [d[1].charts[-1] for d in inferred_charts]
```

### Comparing `gleaner-0.0.2/gleaner/utill.py` & `gleaner-0.0.3/gleaner/utill.py`

 * *Files identical despite different names*

### Comparing `gleaner-0.0.2/gleaner/explorer/explorer.py` & `gleaner-0.0.3/gleaner/explorer/explorer.py`

 * *Files 7% similar despite different names*

```diff
@@ -49,17 +49,38 @@
     dashboard: GleanerDashboard | None = None
     result: OracleResult | None = None
 
     def __init__(self, df: pd.DataFrame, config: GleanerConfig) -> None:
         self.df = df
         self.config = config
 
-    def _infer(self, gen: Generator, oracle: Oracle, preferences: list[str]):
-        n_charts: list[float] = [gen.prior.n_charts.sample() for _ in range(self.config.n_candidates)]
+    def _infer(
+        self,
+        gen: Generator,
+        oracle: Oracle,
+        preferences: list[str],
+        n_chart: int | None = None,
+        fixed_charts: list[GleanerChart] = [],
+    ):
+        if n_chart and n_chart < len(fixed_charts):
+            raise ValueError("Number of fixed_charts should be smaller than n_chart")
+
+        n_charts: list[float] = [
+            gen.prior.n_charts.sample() if n_chart is None else n_chart for _ in range(self.config.n_candidates)
+        ]
+
+        if len(fixed_charts):
+            n_charts = [max(1, n - len(fixed_charts)) for n in n_charts]
+
         candidates: list[GleanerDashboard] = [gen.sample_dashboard(round(n_chart)) for n_chart in n_charts]
+
+        if len(fixed_charts):
+            for candidate in candidates:
+                candidate.extend(fixed_charts)
+
         results: list[OracleResult] = [oracle.get_result(dashboard, set(preferences)) for dashboard in candidates]
 
         specificity = np.array([r.specificity for r in results])
         interestingness = np.array([r.interestingness for r in results])
         coverage = np.array([r.coverage for r in results])
         diversity = np.array([r.diversity for r in results])
         conciseness = np.array([r.conciseness for r in results])
@@ -80,39 +101,47 @@
             + (conciseness - conciseness.mean()) / conciseness.std() * oracle.weight.conciseness
         )
 
         result_n_scores: list[tuple[OracleResult, GleanerDashboard, float, float]] = [
             (result, candidates[i], raw_scores[i], normalized_scores[i]) for i, result in enumerate(results)
         ]
 
+        result_n_scores.sort(key=lambda x: x[-1], reverse=True)
+
         return (
             result_n_scores,
             raw_scores,
             normalized_scores,
             specificity,
             interestingness,
             coverage,
             diversity,
             conciseness,
         )
 
-    def infer(self, gen: Generator, oracle: Oracle, preferences: list[str]) -> GleanerDashboard:
+    def infer(
+        self,
+        gen: Generator,
+        oracle: Oracle,
+        preferences: list[str],
+        n_chart: int | None = None,
+        fixed_charts: list[list[str | None]] = [],
+    ) -> GleanerDashboard:
         (
             result_n_scores,
             raw_scores,
             normalized_scores,
             specificity,
             interestingness,
             coverage,
             diversity,
             conciseness,
-        ) = self._infer(gen, oracle, preferences)
+        ) = self._infer(gen, oracle, preferences, n_chart, [GleanerChart(c, self.df) for c in fixed_charts])
 
-        expl_idx = np.argmax(normalized_scores)
-        return result_n_scores[expl_idx][1]
+        return result_n_scores[0][1]
 
     def _train(self, gen: Generator, oracle: Oracle, preferences: list[str]) -> TrainResult:
         (
             result_n_scores,
             raw_scores,
             normalized_scores,
             specificity,
```

### Comparing `gleaner-0.0.2/gleaner/generator/generator.py` & `gleaner-0.0.3/gleaner/generator/generator.py`

 * *Files identical despite different names*

### Comparing `gleaner-0.0.2/gleaner/generator/generator_parameters.py` & `gleaner-0.0.3/gleaner/generator/generator_parameters.py`

 * *Files identical despite different names*

### Comparing `gleaner-0.0.2/gleaner/model/data_transforms.py` & `gleaner-0.0.3/gleaner/model/data_transforms.py`

 * *Files identical despite different names*

### Comparing `gleaner-0.0.2/gleaner/model/gleaner_chart.py` & `gleaner-0.0.3/gleaner/model/gleaner_chart.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,61 @@
 # type: ignore
+from ast import literal_eval
 from typing import Literal, Optional, Set, Union
 import altair as alt
 import pandas as pd
 import json
 
 from gleaner.model import (
     Aggregation,
     Binning,
     Encodings,
     Attribute,
 )
 
 
-chart_hash = {}
+chart_hash: dict[str, "GleanerChart"] = {}
+
+
+def get_gleaner_chart_from_key(key: str) -> "GleanerChart":
+    chart = chart_hash.get(key)
+    if not chart:
+        raise Exception("Chart not found")
+    return chart
 
 
 def get_gleaner_chart(sample: list[Attribute | str | None], df):
-    chart = chart_hash.get(tuple([s.name if isinstance(s, Attribute) else s for s in sample]))
+    chart = chart_hash.get(str([s.name if isinstance(s, Attribute) else s for s in sample]))
     return chart if chart else GleanerChart(sample, df)
 
 
 class GleanerChart:
     sample: list[Union["Attribute", str, None]]
+    key: str
     index: Optional[int]
     sub_df: pd.DataFrame
     attrs: list["Attribute"]
 
     filters: Optional[list[tuple[str, str, str]]] = None
     binnings: Optional[list["Binning"]] = None
     aggregation: Optional["Aggregation"] = None
     chart_type: str = None
     encoding: Optional["Encodings"] = None
 
     def __init__(self, result: list, df: pd.DataFrame) -> None:
         chart_type, x, y, z, agg_type = result
+        self.key = str(
+            [
+                chart_type,
+                x.name if x else None,
+                y.name if y else None,
+                z.name if z else None,
+                agg_type,
+            ]
+        )
         self.attrs = [x, y, z] if z else [x, y] if y else [x]
         self.sample = result
         for i in range(len(self.attrs)):
             self.sample[i + 1] = self.attrs[i].name
 
         self.sub_df = df[[x.name, y.name, z.name] if z else [x.name, y.name] if y else [x.name]]
         self.chart_type = chart_type
```

### Comparing `gleaner-0.0.2/gleaner/model/gleaner_dahsboard.py` & `gleaner-0.0.3/gleaner/model/gleaner_dahsboard.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,14 +7,20 @@
 @dataclass
 class GleanerDashboard:
     charts: list[GleanerChart]
 
     def __len__(self):
         return len(self.charts)
 
+    def append(self, chart: GleanerChart):
+        self.charts.append(chart)
+
+    def extend(self, charts: list[GleanerChart]):
+        self.charts = charts + self.charts
+
     def display(self, width: int = 150, height: int = 150, num_cols: int = 4):
         if self.charts is None:
             return None
         altairs = [chart.display().properties(width=width, height=height) for chart in self.charts]
         rows: list[alt.HConcatChart] = [
             alt.hconcat(*altairs[i : i + num_cols]).resolve_scale(color="independent")
             for i in range(0, len(altairs), num_cols)
```

### Comparing `gleaner-0.0.2/gleaner/oracle/oracle.py` & `gleaner-0.0.3/gleaner/oracle/oracle.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,18 +6,19 @@
 from gleaner.oracle import OracleResult, OracleWeight
 from gleaner.oracle.scores import (
     get_coverage_from_nodes,
     get_diversity_from_nodes,
     get_interestingness,
     get_specificity_from_nodes,
     get_conciseness_from_nodes,
+    get_statistic_features,
 )
 
 if TYPE_CHECKING:
-    from gleaner.model import GleanerDashboard
+    from gleaner.model import GleanerDashboard, GleanerChart
 
 
 class Oracle:
     df: pd.DataFrame
 
     def __init__(self, df) -> None:
         self.df = df
@@ -30,14 +31,17 @@
             coverage=get_coverage_from_nodes(nodes, self.df),
             diversity=get_diversity_from_nodes(nodes, preferences),
             interestingness=get_interestingness(nodes),
             specificity=get_specificity_from_nodes(nodes, preferences),
             conciseness=get_conciseness_from_nodes(nodes, self.df),
         )
 
+    def get_statistics_from_chart(self, chart: "GleanerChart") -> dict[str, list[str | None]]:
+        return get_statistic_features(chart)
+
     def update(
         self,
         specificity: float | None = None,
         interestingness: float | None = None,
         coverage: float | None = None,
         diversity: float | None = None,
         conciseness: float | None = None,
```

### Comparing `gleaner-0.0.2/gleaner/oracle/oracle_result.py` & `gleaner-0.0.3/gleaner/oracle/oracle_result.py`

 * *Files identical despite different names*

### Comparing `gleaner-0.0.2/gleaner/oracle/scores/anova.py` & `gleaner-0.0.3/gleaner/oracle/scores/anova.py`

 * *Files identical despite different names*

### Comparing `gleaner-0.0.2/gleaner/oracle/scores/diversity.py` & `gleaner-0.0.3/gleaner/oracle/scores/diversity.py`

 * *Files identical despite different names*

### Comparing `gleaner-0.0.2/gleaner/oracle/scores/interestingness.py` & `gleaner-0.0.3/gleaner/oracle/scores/interestingness.py`

 * *Files 8% similar despite different names*

```diff
@@ -62,35 +62,35 @@
 def has_significance_qn(df: pd.DataFrame, attr_q: str, attr_n: str) -> str | None:
     n = df[attr_n].to_numpy()
     q = df[attr_q].to_numpy()
     f, p = f_oneway(n, q)
     return "has_significance" if p < 0.05 else None
 
 
-hashmap = {}
+hashmap: dict[str, list[str | None]] = {}
 df_hash_map = {}
 
 
 def mean(l):
     return sum(l) / len(l)
 
 
-def get_statistic_features(node: "GleanerChart") -> list[list[str | None]]:
+def get_statistic_features(node: "GleanerChart") -> dict[str, list[str | None]]:
     attr_combinations: list[tuple[Attribute, ...]] = [
         *list(combinations(node.attrs, 1)),
         *list(combinations(node.attrs, 2)),
     ]
-    features = []
+    features = {}
     for comb in attr_combinations:
-        key = ""
-        if node.filters is not None:
-            for f in node.filters:
-                key += f"{str((f[0], f[1]))}/"
+        # if node.filters is not None:
+        #     for f in node.filters:
+        #         key += f"{str((f[0], f[1]))}/"
+
         target_attrs = [attr.name for attr in comb]
-        key += f"{target_attrs}"
+        key = "/".join(target_attrs)
 
         try:
             if key not in hashmap:
                 df_notnull = df_hash_map[key] if key in df_hash_map else node.sub_df.dropna()
                 if len(comb) == 1 and comb[0].type == "Q":
                     hashmap[key] = [
                         has_outliers_q(df_notnull, comb[0].name),
@@ -109,15 +109,15 @@
                         has_outliers_qq(df_notnull, comb[0].name, comb[1].name),
                     ]
                 elif len(comb) == 2 and comb[0].type == "C" and comb[1].type == "C":
                     hashmap[key] = [
                         has_correlation_nn(df_notnull, comb[0].name, comb[1].name),
                         has_outliers_nn(df_notnull, comb[0].name, comb[1].name),
                     ]
-            features.append(hashmap[key])
+            features[key] = hashmap[key]
         except Exception as e:
             print(f"Error in {key} with {comb} and {node.filters}")
             raise e
 
     return features
 
 
@@ -127,8 +127,8 @@
 
 
 def get_interestingness(
     nodes: list["GleanerChart"],
 ) -> float:
     node_features = [get_statistic_features(node) for node in nodes]
 
-    return mean([feature_to_interestingness(feature) for feature in node_features])
+    return mean([feature_to_interestingness(list(feature.values())) for feature in node_features])
```

### Comparing `gleaner-0.0.2/.gitignore` & `gleaner-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `gleaner-0.0.2/LICENSE` & `gleaner-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gleaner-0.0.2/README.md` & `gleaner-0.0.3/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,30 @@
 # Gleaner: Multi-Criteria Optimization for Automatic Dashboard Design
 ![figure](https://user-images.githubusercontent.com/2310571/236782548-6976a025-f97e-443f-8e07-50e5d442890e.png)
 
 ***Gleaner*** is an automatic dashboard design system that optimizes the design in terms of four design criteria, namely Specificity, Interestingness, Diversity, and Coverage. With these criteria, Gleaner not only optimizes for the expressiveness and interestingness of a single visualization but also improves the diversity and coverage of the dashboard as a whole. Users are able to express their intent for desired dashboard design to Gleaner, including specifying preferred or constrained attributes and adjusting the weight of the Oracle. This flexibility in expressing intent enables Gleaner to design dashboards that are well-aligned with the user's own analytic goals leading to more effective and efficient data exploration and analysis.
 
+## Installation
+```
+pip install gleaner
+```
+
+## Usage Example
+* Detailed documentations are under construction!
+
+```python
+from gleaner import Gleaner
+gl = Gleaner(df)
+gl.train(["rect", "count", "Creative_Type"])
+gl.infer().display()
+```
 
-## Demo for Standalone Python Library
+## Demo for Gleaner Library
 
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/Jason-Choi/Gleaner/main?labpath=demo.ipynb)
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/12_Wm74nT2_X9zJlV0PJ0SeEVhyOc0eUf)
 
 ## Demo for Web-based Interface
 
 TBA
 
 ## Development
```

### Comparing `gleaner-0.0.2/pyproject.toml` & `gleaner-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,17 @@
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
     "pandas",
     "numpy",
     "altair",
     "scikit-learn",
+    "ipython",
+    "fastapi",
+    "uvicorn"
 ]
 
 [project.urls]
 Documentation = "https://github.com/jason-choi/gleaner"
 Issues = "https://github.com/jason-choi/gleaner/issues"
 Source = "https://github.com/jason-choi/gleaner"
 
@@ -161,11 +164,12 @@
 [tool.hatch.build.targets.sdist]
 exclude = [
   "/.github",
   "/__pycache__",
   "/.ipynb_checkpoints",
   "/docs",
   "/*.ipynb",
+  "/client"
 ]
 
 [tool.hatch.build.targets.wheel]
-packages = ["gleaner"]
+packages = ["gleaner"]
```

### Comparing `gleaner-0.0.2/PKG-INFO` & `gleaner-0.0.3/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gleaner
-Version: 0.0.2
+Version: 0.0.3
 Summary: Gleaner: Multi-Criteria Optimization for Automatic Dashboard Design
 Project-URL: Documentation, https://github.com/jason-choi/gleaner
 Project-URL: Issues, https://github.com/jason-choi/gleaner/issues
 Project-URL: Source, https://github.com/jason-choi/gleaner
 Author-email: Jason Choi <jasonchoi3@g.skku.edu>
 License-Expression: MIT
 License-File: LICENSE
@@ -12,28 +12,45 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
 Requires-Dist: altair
+Requires-Dist: fastapi
+Requires-Dist: ipython
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: scikit-learn
+Requires-Dist: uvicorn
 Description-Content-Type: text/markdown
 
 # Gleaner: Multi-Criteria Optimization for Automatic Dashboard Design
 ![figure](https://user-images.githubusercontent.com/2310571/236782548-6976a025-f97e-443f-8e07-50e5d442890e.png)
 
 ***Gleaner*** is an automatic dashboard design system that optimizes the design in terms of four design criteria, namely Specificity, Interestingness, Diversity, and Coverage. With these criteria, Gleaner not only optimizes for the expressiveness and interestingness of a single visualization but also improves the diversity and coverage of the dashboard as a whole. Users are able to express their intent for desired dashboard design to Gleaner, including specifying preferred or constrained attributes and adjusting the weight of the Oracle. This flexibility in expressing intent enables Gleaner to design dashboards that are well-aligned with the user's own analytic goals leading to more effective and efficient data exploration and analysis.
 
+## Installation
+```
+pip install gleaner
+```
+
+## Usage Example
+* Detailed documentations are under construction!
+
+```python
+from gleaner import Gleaner
+gl = Gleaner(df)
+gl.train(["rect", "count", "Creative_Type"])
+gl.infer().display()
+```
 
-## Demo for Standalone Python Library
+## Demo for Gleaner Library
 
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/Jason-Choi/Gleaner/main?labpath=demo.ipynb)
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/12_Wm74nT2_X9zJlV0PJ0SeEVhyOc0eUf)
 
 ## Demo for Web-based Interface
 
 TBA
 
 ## Development
```

