# Comparing `tmp/pref_voting-0.2.7.tar.gz` & `tmp/pref_voting-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pref_voting-0.2.7.tar", max compression
+gzip compressed data, was "pref_voting-0.2.8.tar", max compression
```

## Comparing `pref_voting-0.2.7.tar` & `pref_voting-0.2.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1068 2022-07-08 15:47:57.000000 pref_voting-0.2.7/LICENSE
--rw-r--r--   0        0        0     2756 2023-05-16 17:57:12.798243 pref_voting-0.2.7/README.md
--rw-r--r--   0        0        0       22 2023-05-16 17:57:03.098969 pref_voting-0.2.7/pref_voting/__init__.py
--rw-r--r--   0        0        0     9631 2023-05-10 11:35:26.690819 pref_voting-0.2.7/pref_voting/analysis.py
--rw-r--r--   0        0        0     1226 2023-05-10 11:42:24.592401 pref_voting-0.2.7/pref_voting/axiom.py
--rw-r--r--   0        0        0      360 2023-05-10 11:16:28.091090 pref_voting-0.2.7/pref_voting/axiom_helpers.py
--rw-r--r--   0        0        0       43 2023-04-27 22:57:52.337540 pref_voting-0.2.7/pref_voting/axioms.py
--rw-r--r--   0        0        0    23065 2023-05-10 11:22:02.837497 pref_voting-0.2.7/pref_voting/c1_methods.py
--rw-r--r--   0        0        0     8564 2023-02-15 17:29:01.299008 pref_voting-0.2.7/pref_voting/combined_methods.py
--rw-r--r--   0        0        0    11517 2023-05-10 11:58:43.699679 pref_voting-0.2.7/pref_voting/dominance_axioms.py
--rw-r--r--   0        0        0    20643 2023-05-10 11:16:22.353419 pref_voting-0.2.7/pref_voting/generate_profiles.py
--rw-r--r--   0        0        0    10484 2023-01-11 11:10:14.000000 pref_voting-0.2.7/pref_voting/generate_weighted_majority_graphs.py
--rw-r--r--   0        0        0     1806 2022-08-08 19:08:16.000000 pref_voting-0.2.7/pref_voting/helper.py
--rw-r--r--   0        0        0    73229 2023-05-10 11:16:21.455329 pref_voting-0.2.7/pref_voting/iterative_methods.py
--rw-r--r--   0        0        0    20246 2022-07-12 12:12:35.000000 pref_voting-0.2.7/pref_voting/maj_graph_ex1.png
--rw-r--r--   0        0        0    57868 2023-05-10 11:18:39.320393 pref_voting-0.2.7/pref_voting/margin_based_methods.py
--rw-r--r--   0        0        0    25681 2023-05-10 11:20:32.560828 pref_voting-0.2.7/pref_voting/other_methods.py
--rw-r--r--   0        0        0     9526 2023-05-10 11:24:57.793416 pref_voting-0.2.7/pref_voting/pr_voting_methods.py
--rw-r--r--   0        0        0    26954 2023-05-15 22:14:59.029784 pref_voting-0.2.7/pref_voting/profiles.py
--rw-r--r--   0        0        0    34203 2023-04-27 22:31:21.483788 pref_voting-0.2.7/pref_voting/profiles_with_ties.py
--rw-r--r--   0        0        0    11064 2023-05-05 16:30:25.075183 pref_voting-0.2.7/pref_voting/scoring_methods.py
--rw-r--r--   0        0        0     5381 2023-02-15 15:31:23.315651 pref_voting-0.2.7/pref_voting/voting_method.py
--rw-r--r--   0        0        0      253 2022-07-31 21:02:46.000000 pref_voting-0.2.7/pref_voting/voting_methods.py
--rw-r--r--   0        0        0    49026 2023-05-16 17:55:35.552339 pref_voting-0.2.7/pref_voting/weighted_majority_graphs.py
--rw-r--r--   0        0        0      715 2023-05-16 17:57:14.829426 pref_voting-0.2.7/pyproject.toml
--rw-r--r--   0        0        0     3731 1970-01-01 00:00:00.000000 pref_voting-0.2.7/setup.py
--rw-r--r--   0        0        0     3850 1970-01-01 00:00:00.000000 pref_voting-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0     1068 2022-07-08 15:47:57.000000 pref_voting-0.2.8/LICENSE
+-rw-r--r--   0        0        0     2756 2023-05-16 18:00:59.189933 pref_voting-0.2.8/README.md
+-rw-r--r--   0        0        0       22 2023-05-16 18:00:58.034340 pref_voting-0.2.8/pref_voting/__init__.py
+-rw-r--r--   0        0        0     9631 2023-05-10 11:35:26.690819 pref_voting-0.2.8/pref_voting/analysis.py
+-rw-r--r--   0        0        0     1226 2023-05-10 11:42:24.592401 pref_voting-0.2.8/pref_voting/axiom.py
+-rw-r--r--   0        0        0      360 2023-05-10 11:16:28.091090 pref_voting-0.2.8/pref_voting/axiom_helpers.py
+-rw-r--r--   0        0        0       43 2023-04-27 22:57:52.337540 pref_voting-0.2.8/pref_voting/axioms.py
+-rw-r--r--   0        0        0    23065 2023-05-10 11:22:02.837497 pref_voting-0.2.8/pref_voting/c1_methods.py
+-rw-r--r--   0        0        0     8564 2023-02-15 17:29:01.299008 pref_voting-0.2.8/pref_voting/combined_methods.py
+-rw-r--r--   0        0        0    11517 2023-05-10 11:58:43.699679 pref_voting-0.2.8/pref_voting/dominance_axioms.py
+-rw-r--r--   0        0        0    20643 2023-05-10 11:16:22.353419 pref_voting-0.2.8/pref_voting/generate_profiles.py
+-rw-r--r--   0        0        0    10484 2023-01-11 11:10:14.000000 pref_voting-0.2.8/pref_voting/generate_weighted_majority_graphs.py
+-rw-r--r--   0        0        0     1806 2022-08-08 19:08:16.000000 pref_voting-0.2.8/pref_voting/helper.py
+-rw-r--r--   0        0        0    73229 2023-05-10 11:16:21.455329 pref_voting-0.2.8/pref_voting/iterative_methods.py
+-rw-r--r--   0        0        0    20246 2022-07-12 12:12:35.000000 pref_voting-0.2.8/pref_voting/maj_graph_ex1.png
+-rw-r--r--   0        0        0    57868 2023-05-10 11:18:39.320393 pref_voting-0.2.8/pref_voting/margin_based_methods.py
+-rw-r--r--   0        0        0    25681 2023-05-10 11:20:32.560828 pref_voting-0.2.8/pref_voting/other_methods.py
+-rw-r--r--   0        0        0     9526 2023-05-10 11:24:57.793416 pref_voting-0.2.8/pref_voting/pr_voting_methods.py
+-rw-r--r--   0        0        0    26954 2023-05-15 22:14:59.029784 pref_voting-0.2.8/pref_voting/profiles.py
+-rw-r--r--   0        0        0    34203 2023-04-27 22:31:21.483788 pref_voting-0.2.8/pref_voting/profiles_with_ties.py
+-rw-r--r--   0        0        0    11064 2023-05-05 16:30:25.075183 pref_voting-0.2.8/pref_voting/scoring_methods.py
+-rw-r--r--   0        0        0     5381 2023-02-15 15:31:23.315651 pref_voting-0.2.8/pref_voting/voting_method.py
+-rw-r--r--   0        0        0      253 2022-07-31 21:02:46.000000 pref_voting-0.2.8/pref_voting/voting_methods.py
+-rw-r--r--   0        0        0    49214 2023-05-16 18:00:25.171109 pref_voting-0.2.8/pref_voting/weighted_majority_graphs.py
+-rw-r--r--   0        0        0      715 2023-05-16 18:00:58.624385 pref_voting-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0     3731 1970-01-01 00:00:00.000000 pref_voting-0.2.8/setup.py
+-rw-r--r--   0        0        0     3850 1970-01-01 00:00:00.000000 pref_voting-0.2.8/PKG-INFO
```

### Comparing `pref_voting-0.2.7/LICENSE` & `pref_voting-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pref_voting-0.2.7/README.md` & `pref_voting-0.2.8/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 - v0.1.25 (2023-1-11): Add condorcet_irv, condorcet_irv_put; Update documentation; add axioms.py; add display and equality to Ranking class; fix enumerate ceots functions
 - v0.1.27 (2023-2-07): Add Borda for ProfileWithTies
 - v0.2 (2023-2-15): Add Benham, add anonymize to Profile method, comment out numba to make compatible with Python 3.11, add add_unranked_candidates to ProfileWithTies
 - v0.2.1 (2023-2-15): Bug fixes
 - v0.2.3 (2023-4-2): Add plurality_with_runoff_with_explanation
 - v0.2.4 (2023-4-9): Update generate_truncated_profile so that it implements the IC probability model.
 - v0.2.6 (2023-5-10): Add axiom class, dominance axioms, and axiom_violations_data.
-- v0.2.7 (2023-5-16): Add description function to Majority Graphs.
+- v0.2.8 (2023-5-16): Add description function to Majority Graphs.
 
 ## Questions?
 
 Feel free to [send me an email](https://pacuit.org/) if you have questions about the project.
 
 ## License
```

### Comparing `pref_voting-0.2.7/pref_voting/analysis.py` & `pref_voting-0.2.8/pref_voting/analysis.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.2.7/pref_voting/axiom.py` & `pref_voting-0.2.8/pref_voting/axiom.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.2.7/pref_voting/c1_methods.py` & `pref_voting-0.2.8/pref_voting/c1_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.2.7/pref_voting/combined_methods.py` & `pref_voting-0.2.8/pref_voting/combined_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.2.7/pref_voting/dominance_axioms.py` & `pref_voting-0.2.8/pref_voting/dominance_axioms.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.2.7/pref_voting/generate_profiles.py` & `pref_voting-0.2.8/pref_voting/generate_profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.2.7/pref_voting/generate_weighted_majority_graphs.py` & `pref_voting-0.2.8/pref_voting/generate_weighted_majority_graphs.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.2.7/pref_voting/helper.py` & `pref_voting-0.2.8/pref_voting/helper.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.2.7/pref_voting/iterative_methods.py` & `pref_voting-0.2.8/pref_voting/iterative_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.2.7/pref_voting/maj_graph_ex1.png` & `pref_voting-0.2.8/pref_voting/maj_graph_ex1.png`

 * *Files identical despite different names*

### Comparing `pref_voting-0.2.7/pref_voting/margin_based_methods.py` & `pref_voting-0.2.8/pref_voting/margin_based_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.2.7/pref_voting/other_methods.py` & `pref_voting-0.2.8/pref_voting/other_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.2.7/pref_voting/pr_voting_methods.py` & `pref_voting-0.2.8/pref_voting/pr_voting_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.2.7/pref_voting/profiles.py` & `pref_voting-0.2.8/pref_voting/profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.2.7/pref_voting/profiles_with_ties.py` & `pref_voting-0.2.8/pref_voting/profiles_with_ties.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.2.7/pref_voting/scoring_methods.py` & `pref_voting-0.2.8/pref_voting/scoring_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.2.7/pref_voting/voting_method.py` & `pref_voting-0.2.8/pref_voting/voting_method.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.2.7/pref_voting/weighted_majority_graphs.py` & `pref_voting-0.2.8/pref_voting/weighted_majority_graphs.py`

 * *Files 1% similar despite different names*

```diff
@@ -584,14 +584,20 @@
                 new_edges.append((e[0], e[1], new_margin))
 
             else:
                 new_edges.append((e[0], e[1], new_margin))
 
         return MarginGraph(self.candidates, new_edges, cmap=self.cmap)
 
+    def description(self): 
+        """
+        Returns a string describing the Margin Graph.
+        """
+        return f"MarginGraph({self.candidates}, {self.edges}, cmap={self.cmap})"
+
     def display(self, curr_cands=None, cmap=None):
         """Display a margin graph (restricted to ``curr_cands``) using networkx.draw.
 
         :param cmap: the candidate map to use (overrides the cmap associated with this majority graph)
         :type cmap: dict[int,str], optional
         :param curr_cands: list of candidates
         :type curr_cands: list[int], optional
```

### Comparing `pref_voting-0.2.7/pyproject.toml` & `pref_voting-0.2.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 name = "pref_voting"
-version = "0.2.7"
+version = "0.2.8"
 description = "pref_voting is a Python packaging that contains tools to reason about election profiles and margin graphs, and implementations of a variety of preferential voting methods."
 authors = ["Eric Pacuit <epacuit@umd.edu>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/voting-tools/pref_voting"
 repository = "https://github.com/voting-tools/pref_voting"
```

### Comparing `pref_voting-0.2.7/setup.py` & `pref_voting-0.2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,17 +12,17 @@
  'networkx>=3.0,<4.0',
  'random2>=1.0.1,<2.0.0',
  'scipy>=1.0.0,<2.0.0',
  'tabulate>=0.9.0,<0.10.0']
 
 setup_kwargs = {
     'name': 'pref-voting',
-    'version': '0.2.7',
+    'version': '0.2.8',
     'description': 'pref_voting is a Python packaging that contains tools to reason about election profiles and margin graphs, and implementations of a variety of preferential voting methods.',
-    'long_description': 'pref_voting\n==========\n\n## Installation\n\nWith pip package manager:\n\n```bash\npip install pref_voting\n```\n## Documentation\n\nOnline documentation is available at [https://pref_voting.readthedocs.io](https://pref_voting.readthedocs.io).\n\n## Profiles and Voting Methods\n\nA profile (of linear orders over the candidates) is created by initializing a Profile class object.  This needs a list of rankings (each ranking is a tuple of numbers), the number of candidates, and a list giving the number of each ranking in the profile:\n\n```python\nfrom pref_voting.profiles import Profile\n\nrankings = [(0, 1, 2, 3), (2, 3, 1, 0), (3, 1, 2, 0), (1, 2, 0, 3), (1, 3, 2, 0)]\nrcounts = [5, 3, 2, 4, 3]\n\nprof = Profile(rankings, rcounts=rcounts)\n```\n\nThe function generate_profile is used to generate a profile for a given number of candidates and voters:  \n```python\nfrom pref_voting.generate_profiles import generate_profile\n\n# generate a profile using the Impartial Culture probability model\nprof = generate_profile(3, 4) # prof is a Profile object\n\n# generate a profile using the Impartial Anonymous Culture probability model\nprof = generate_profile(3, 4, probmod = "IAC") # prof is a Profile object \n```\n\n```python\nfrom pref_voting.profiles import Profile\nfrom pref_voting.voting_methods import *\n\nprof = Profile(rankings, num_cands, rcounts=rcounts)\nprint(f"{split_cycle.name} winners:  {split_cycle(prof)}")\nsplit_cycle.display(prof)\n\n```\n\n## Versions\n\n- v0.1.10 (2022-08-09): **Initial release** \n- v0.1.13 (2022-11-05): Minor updates and bug fixes \n- v0.1.14 (2022-12-19): Add plurality_scores to ProfileWithTies; add generate ceots function; bug fixes \n- v0.1.23 (2022-12-27): Add instant_runoff_for_truncated_linear_orders and functions to truncate overvotes in a ProfileWithTies, add smith_irv_put, document analysis functions\n- v0.1.25 (2023-1-11): Add condorcet_irv, condorcet_irv_put; Update documentation; add axioms.py; add display and equality to Ranking class; fix enumerate ceots functions\n- v0.1.27 (2023-2-07): Add Borda for ProfileWithTies\n- v0.2 (2023-2-15): Add Benham, add anonymize to Profile method, comment out numba to make compatible with Python 3.11, add add_unranked_candidates to ProfileWithTies\n- v0.2.1 (2023-2-15): Bug fixes\n- v0.2.3 (2023-4-2): Add plurality_with_runoff_with_explanation\n- v0.2.4 (2023-4-9): Update generate_truncated_profile so that it implements the IC probability model.\n- v0.2.6 (2023-5-10): Add axiom class, dominance axioms, and axiom_violations_data.\n- v0.2.7 (2023-5-16): Add description function to Majority Graphs.\n\n## Questions?\n\nFeel free to [send me an email](https://pacuit.org/) if you have questions about the project.\n\n## License\n\n[MIT](https://github.com/jontingvold/pyrankvote/blob/master/LICENSE.txt)\n',
+    'long_description': 'pref_voting\n==========\n\n## Installation\n\nWith pip package manager:\n\n```bash\npip install pref_voting\n```\n## Documentation\n\nOnline documentation is available at [https://pref_voting.readthedocs.io](https://pref_voting.readthedocs.io).\n\n## Profiles and Voting Methods\n\nA profile (of linear orders over the candidates) is created by initializing a Profile class object.  This needs a list of rankings (each ranking is a tuple of numbers), the number of candidates, and a list giving the number of each ranking in the profile:\n\n```python\nfrom pref_voting.profiles import Profile\n\nrankings = [(0, 1, 2, 3), (2, 3, 1, 0), (3, 1, 2, 0), (1, 2, 0, 3), (1, 3, 2, 0)]\nrcounts = [5, 3, 2, 4, 3]\n\nprof = Profile(rankings, rcounts=rcounts)\n```\n\nThe function generate_profile is used to generate a profile for a given number of candidates and voters:  \n```python\nfrom pref_voting.generate_profiles import generate_profile\n\n# generate a profile using the Impartial Culture probability model\nprof = generate_profile(3, 4) # prof is a Profile object\n\n# generate a profile using the Impartial Anonymous Culture probability model\nprof = generate_profile(3, 4, probmod = "IAC") # prof is a Profile object \n```\n\n```python\nfrom pref_voting.profiles import Profile\nfrom pref_voting.voting_methods import *\n\nprof = Profile(rankings, num_cands, rcounts=rcounts)\nprint(f"{split_cycle.name} winners:  {split_cycle(prof)}")\nsplit_cycle.display(prof)\n\n```\n\n## Versions\n\n- v0.1.10 (2022-08-09): **Initial release** \n- v0.1.13 (2022-11-05): Minor updates and bug fixes \n- v0.1.14 (2022-12-19): Add plurality_scores to ProfileWithTies; add generate ceots function; bug fixes \n- v0.1.23 (2022-12-27): Add instant_runoff_for_truncated_linear_orders and functions to truncate overvotes in a ProfileWithTies, add smith_irv_put, document analysis functions\n- v0.1.25 (2023-1-11): Add condorcet_irv, condorcet_irv_put; Update documentation; add axioms.py; add display and equality to Ranking class; fix enumerate ceots functions\n- v0.1.27 (2023-2-07): Add Borda for ProfileWithTies\n- v0.2 (2023-2-15): Add Benham, add anonymize to Profile method, comment out numba to make compatible with Python 3.11, add add_unranked_candidates to ProfileWithTies\n- v0.2.1 (2023-2-15): Bug fixes\n- v0.2.3 (2023-4-2): Add plurality_with_runoff_with_explanation\n- v0.2.4 (2023-4-9): Update generate_truncated_profile so that it implements the IC probability model.\n- v0.2.6 (2023-5-10): Add axiom class, dominance axioms, and axiom_violations_data.\n- v0.2.8 (2023-5-16): Add description function to Majority Graphs.\n\n## Questions?\n\nFeel free to [send me an email](https://pacuit.org/) if you have questions about the project.\n\n## License\n\n[MIT](https://github.com/jontingvold/pyrankvote/blob/master/LICENSE.txt)\n',
     'author': 'Eric Pacuit',
     'author_email': 'epacuit@umd.edu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/voting-tools/pref_voting',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `pref_voting-0.2.7/PKG-INFO` & `pref_voting-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pref-voting
-Version: 0.2.7
+Version: 0.2.8
 Summary: pref_voting is a Python packaging that contains tools to reason about election profiles and margin graphs, and implementations of a variety of preferential voting methods.
 Home-page: https://github.com/voting-tools/pref_voting
 License: MIT
 Author: Eric Pacuit
 Author-email: epacuit@umd.edu
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -80,15 +80,15 @@
 - v0.1.25 (2023-1-11): Add condorcet_irv, condorcet_irv_put; Update documentation; add axioms.py; add display and equality to Ranking class; fix enumerate ceots functions
 - v0.1.27 (2023-2-07): Add Borda for ProfileWithTies
 - v0.2 (2023-2-15): Add Benham, add anonymize to Profile method, comment out numba to make compatible with Python 3.11, add add_unranked_candidates to ProfileWithTies
 - v0.2.1 (2023-2-15): Bug fixes
 - v0.2.3 (2023-4-2): Add plurality_with_runoff_with_explanation
 - v0.2.4 (2023-4-9): Update generate_truncated_profile so that it implements the IC probability model.
 - v0.2.6 (2023-5-10): Add axiom class, dominance axioms, and axiom_violations_data.
-- v0.2.7 (2023-5-16): Add description function to Majority Graphs.
+- v0.2.8 (2023-5-16): Add description function to Majority Graphs.
 
 ## Questions?
 
 Feel free to [send me an email](https://pacuit.org/) if you have questions about the project.
 
 ## License
```

