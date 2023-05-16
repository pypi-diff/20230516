# Comparing `tmp/brain-loop-search-0.1.4.tar.gz` & `tmp/brain-loop-search-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brain-loop-search-0.1.4.tar", last modified: Mon May 15 02:27:41 2023, max compression
+gzip compressed data, was "brain-loop-search-0.1.5.tar", last modified: Tue May 16 05:45:36 2023, max compression
```

## Comparing `brain-loop-search-0.1.4.tar` & `brain-loop-search-0.1.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 02:27:41.194573 brain-loop-search-0.1.4/
-drwxrwxrwx   0        0        0        0 2023-05-15 02:27:41.161795 brain-loop-search-0.1.4/.github/
--rw-rw-rw-   0        0        0        6 2023-05-10 08:58:56.000000 brain-loop-search-0.1.4/.github/python-version.txt
-drwxrwxrwx   0        0        0        0 2023-05-15 02:27:41.162830 brain-loop-search-0.1.4/.github/workflows/
--rw-rw-rw-   0        0        0     1447 2023-05-10 08:58:56.000000 brain-loop-search-0.1.4/.github/workflows/static.yml
--rw-rw-rw-   0        0        0     1935 2023-05-10 08:56:44.000000 brain-loop-search-0.1.4/.gitignore
--rw-rw-rw-   0        0        0     1096 2023-04-19 10:12:56.000000 brain-loop-search-0.1.4/LICENSE
--rw-rw-rw-   0        0        0       22 2023-04-19 07:47:30.000000 brain-loop-search-0.1.4/MANIFEST.in
--rw-rw-rw-   0        0        0     4968 2023-05-15 02:27:41.193977 brain-loop-search-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     4291 2023-05-10 10:11:48.000000 brain-loop-search-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-15 02:27:41.171041 brain-loop-search-0.1.4/brain_loop_search/
--rw-rw-rw-   0        0        0      290 2023-05-10 05:16:54.000000 brain-loop-search-0.1.4/brain_loop_search/__init__.py
--rw-rw-rw-   0        0        0    10889 2023-05-10 09:11:32.000000 brain-loop-search-0.1.4/brain_loop_search/brain_utils.py
--rw-rw-rw-   0        0        0    13576 2023-05-15 02:26:42.000000 brain-loop-search-0.1.4/brain_loop_search/packing.py
--rw-rw-rw-   0        0        0    19645 2023-05-10 05:50:08.000000 brain-loop-search-0.1.4/brain_loop_search/search.py
--rw-rw-rw-   0        0        0    65506 2023-02-01 17:02:57.000000 brain-loop-search-0.1.4/brain_loop_search/structures.csv
-drwxrwxrwx   0        0        0        0 2023-05-15 02:27:41.179839 brain-loop-search-0.1.4/brain_loop_search.egg-info/
--rw-rw-rw-   0        0        0     4968 2023-05-15 02:27:40.000000 brain-loop-search-0.1.4/brain_loop_search.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      627 2023-05-15 02:27:41.000000 brain-loop-search-0.1.4/brain_loop_search.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 02:27:40.000000 brain-loop-search-0.1.4/brain_loop_search.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-05-15 02:27:40.000000 brain-loop-search-0.1.4/brain_loop_search.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-05-15 02:27:40.000000 brain-loop-search-0.1.4/brain_loop_search.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      984 2023-05-10 08:55:45.000000 brain-loop-search-0.1.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-15 02:27:41.194573 brain-loop-search-0.1.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-15 02:27:41.192382 brain-loop-search-0.1.4/test/
--rw-rw-rw-   0        0        0   144508 2023-05-10 08:22:30.000000 brain-loop-search-0.1.4/test/test.png
--rw-rw-rw-   0        0        0   143835 2023-05-10 09:11:39.000000 brain-loop-search-0.1.4/test/test2.png
--rw-rw-rw-   0        0        0     1359 2023-05-10 05:50:08.000000 brain-loop-search-0.1.4/test/test_flow.py
--rw-rw-rw-   0        0        0     2818 2023-05-04 13:57:31.000000 brain-loop-search-0.1.4/test/test_graph_packing.py
--rw-rw-rw-   0        0        0     1128 2023-05-04 13:57:31.000000 brain-loop-search-0.1.4/test/test_ontology.py
--rw-rw-rw-   0        0        0     3588 2023-05-10 05:43:45.000000 brain-loop-search-0.1.4/test/test_sssp.py
--rw-rw-rw-   0        0        0     3400 2023-05-04 13:57:31.000000 brain-loop-search-0.1.4/test/test_vertex_packing.py
--rw-rw-rw-   0        0        0     1135 2023-05-10 08:35:20.000000 brain-loop-search-0.1.4/test/test_vis.py
+drwxrwxrwx   0        0        0        0 2023-05-16 05:45:36.735617 brain-loop-search-0.1.5/
+drwxrwxrwx   0        0        0        0 2023-05-16 05:45:36.185087 brain-loop-search-0.1.5/.github/
+-rw-rw-rw-   0        0        0        6 2023-05-10 08:58:56.000000 brain-loop-search-0.1.5/.github/python-version.txt
+drwxrwxrwx   0        0        0        0 2023-05-16 05:45:36.187082 brain-loop-search-0.1.5/.github/workflows/
+-rw-rw-rw-   0        0        0     1447 2023-05-10 08:58:56.000000 brain-loop-search-0.1.5/.github/workflows/static.yml
+-rw-rw-rw-   0        0        0     1935 2023-05-10 08:56:44.000000 brain-loop-search-0.1.5/.gitignore
+-rw-rw-rw-   0        0        0     1096 2023-04-19 10:12:56.000000 brain-loop-search-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0       22 2023-04-19 07:47:30.000000 brain-loop-search-0.1.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     4968 2023-05-16 05:45:36.734620 brain-loop-search-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4291 2023-05-10 10:11:48.000000 brain-loop-search-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-16 05:45:36.258675 brain-loop-search-0.1.5/brain_loop_search/
+-rw-rw-rw-   0        0        0      290 2023-05-10 05:16:54.000000 brain-loop-search-0.1.5/brain_loop_search/__init__.py
+-rw-rw-rw-   0        0        0    10889 2023-05-10 09:11:32.000000 brain-loop-search-0.1.5/brain_loop_search/brain_utils.py
+-rw-rw-rw-   0        0        0    13783 2023-05-16 05:43:01.000000 brain-loop-search-0.1.5/brain_loop_search/packing.py
+-rw-rw-rw-   0        0        0    19645 2023-05-10 05:50:08.000000 brain-loop-search-0.1.5/brain_loop_search/search.py
+-rw-rw-rw-   0        0        0    65506 2023-02-01 17:02:57.000000 brain-loop-search-0.1.5/brain_loop_search/structures.csv
+drwxrwxrwx   0        0        0        0 2023-05-16 05:45:36.304618 brain-loop-search-0.1.5/brain_loop_search.egg-info/
+-rw-rw-rw-   0        0        0     4968 2023-05-16 05:45:35.000000 brain-loop-search-0.1.5/brain_loop_search.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      627 2023-05-16 05:45:36.000000 brain-loop-search-0.1.5/brain_loop_search.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 05:45:35.000000 brain-loop-search-0.1.5/brain_loop_search.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-05-16 05:45:35.000000 brain-loop-search-0.1.5/brain_loop_search.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-05-16 05:45:35.000000 brain-loop-search-0.1.5/brain_loop_search.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      984 2023-05-10 08:55:45.000000 brain-loop-search-0.1.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-16 05:45:36.735617 brain-loop-search-0.1.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-16 05:45:36.713867 brain-loop-search-0.1.5/test/
+-rw-rw-rw-   0        0        0   144508 2023-05-10 08:22:30.000000 brain-loop-search-0.1.5/test/test.png
+-rw-rw-rw-   0        0        0   143835 2023-05-10 09:11:39.000000 brain-loop-search-0.1.5/test/test2.png
+-rw-rw-rw-   0        0        0     1359 2023-05-10 05:50:08.000000 brain-loop-search-0.1.5/test/test_flow.py
+-rw-rw-rw-   0        0        0     2818 2023-05-04 13:57:31.000000 brain-loop-search-0.1.5/test/test_graph_packing.py
+-rw-rw-rw-   0        0        0     1128 2023-05-04 13:57:31.000000 brain-loop-search-0.1.5/test/test_ontology.py
+-rw-rw-rw-   0        0        0     3588 2023-05-10 05:43:45.000000 brain-loop-search-0.1.5/test/test_sssp.py
+-rw-rw-rw-   0        0        0     3400 2023-05-04 13:57:31.000000 brain-loop-search-0.1.5/test/test_vertex_packing.py
+-rw-rw-rw-   0        0        0     1135 2023-05-10 08:35:20.000000 brain-loop-search-0.1.5/test/test_vis.py
```

### Comparing `brain-loop-search-0.1.4/.github/workflows/static.yml` & `brain-loop-search-0.1.5/.github/workflows/static.yml`

 * *Files identical despite different names*

### Comparing `brain-loop-search-0.1.4/.gitignore` & `brain-loop-search-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `brain-loop-search-0.1.4/LICENSE` & `brain-loop-search-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `brain-loop-search-0.1.4/PKG-INFO` & `brain-loop-search-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brain-loop-search
-Version: 0.1.4
+Version: 0.1.5
 Summary: Screen loops among brain structures(or any entities comprising a graph).
 Author-email: Zuohan Zhao <zzhmark@126.com>
 License: MIT License
 Project-URL: GitHub Project, https://github.com/SEU-ALLEN-codebase/brain-loop-search
 Project-URL: Documentation, https://SEU-ALLEN-codebase.github.io/brain-loop-search
 Keywords: neuron-morphology
 Classifier: Programming Language :: Python :: 3
```

### Comparing `brain-loop-search-0.1.4/README.md` & `brain-loop-search-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `brain-loop-search-0.1.4/brain_loop_search/brain_utils.py` & `brain-loop-search-0.1.5/brain_loop_search/brain_utils.py`

 * *Files identical despite different names*

### Comparing `brain-loop-search-0.1.4/brain_loop_search/packing.py` & `brain-loop-search-0.1.5/brain_loop_search/packing.py`

 * *Files 2% similar despite different names*

```diff
@@ -243,17 +243,19 @@
 
     def __init__(self, adj_mat: pd.DataFrame, ontology: Ontology):
         """
         :param adj_mat: the adjacent matrix in pandas dataframe, the projection is from rows to columns.
         :param ontology: a derivation of the abstract class `Ontology`.
         """
         # check adjacent matrix
-        assert ontology.check_include(adj_mat.index), f"rows contain unrecognizable ID "
-        assert ontology.check_include(adj_mat.columns), f"columns contain unrecognizable ID "
-        self._init_mat = adj_mat
+        assert ontology.check_include(adj_mat.index), f"rows contain unrecognizable ID"
+        assert ontology.check_include(adj_mat.columns), f"columns contain unrecognizable ID"
+        self._mat = adj_mat.to_numpy()
+        self._rows = adj_mat.index
+        self._cols = adj_mat.columns
         self._ont = ontology
 
     def pack(self, new_rows: typing.Iterable, new_cols: typing.Iterable, def_val: float = -1,
              superior_as_complement: bool = False, aggr_func=lambda x: 1 / (1 / x).sum()):
         """
         Specifying new rows and columns (usually generated by feeding the original to VertexPacker, but you can
         provide your own list, long as it's within the ontology),
@@ -278,35 +280,39 @@
         assert new_rows.is_unique, "new row items are not unique"
         assert new_cols.is_unique, "new column items are not unique"
 
         new_mat = np.ones([len(new_rows), len(new_cols)]) * def_val
 
         def vertex_map_gen(all_vert, new_vert):
             # prefilter
-            packer = VertexPacker(all_vert, self._ont)
+            packer = VertexPacker(all_vert.unique(), self._ont)
             packer.filter_by_descendants_of(new_vert, include_parents=True)
             needed_vert = packer.stash()
             # map
             map = []
             for v in new_vert:
                 packer = VertexPacker(needed_vert, self._ont)
                 packer.filter_by_descendants_of([v], include_parents=True)
                 nodes = packer.stash()
                 if not superior_as_complement:  # filter the sub nodes in this mode
                     packer = VertexPacker(nodes, self._ont)
                     packer.filter_sub()
                     nodes = packer.stash()
-                map.append(nodes)
+                map.append(np.where(all_vert.isin(nodes)))
             return map
 
-        row_map = vertex_map_gen(self._init_mat.index, new_rows)
-        col_map = vertex_map_gen(self._init_mat.columns, new_cols)
+        row_map = vertex_map_gen(self._rows, new_rows)
+        col_map = vertex_map_gen(self._cols, new_cols)
 
         # calculate the edges in the new matrix
-        for i, (row, fro_nodes) in enumerate(zip(new_rows, row_map)):
-            if len(fro_nodes) == 0:
+        for i, (row, fro_ind) in enumerate(zip(new_rows, row_map)):
+            if len(fro_ind) == 0:
                 continue
-            for j, (col, to_nodes) in enumerate(zip(new_cols, col_map)):
-                if row == col or len(to_nodes) == 0:
+            for j, (col, to_ind) in enumerate(zip(new_cols, col_map)):
+                if row == col or len(to_ind) == 0:
                     continue
-                new_mat[i, j] = aggr_func(self._init_mat.loc[fro_nodes, to_nodes].to_numpy())
+                dat = self._mat[fro_ind][:,to_ind].reshape(-1)
+                dat = dat[dat != def_val]
+                if len(dat) == 0:
+                    continue
+                new_mat[i, j] = aggr_func(dat)
         return pd.DataFrame(new_mat, index=new_rows, columns=new_cols)
```

### Comparing `brain-loop-search-0.1.4/brain_loop_search/search.py` & `brain-loop-search-0.1.5/brain_loop_search/search.py`

 * *Files identical despite different names*

### Comparing `brain-loop-search-0.1.4/brain_loop_search/structures.csv` & `brain-loop-search-0.1.5/brain_loop_search/structures.csv`

 * *Files identical despite different names*

### Comparing `brain-loop-search-0.1.4/brain_loop_search.egg-info/PKG-INFO` & `brain-loop-search-0.1.5/brain_loop_search.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brain-loop-search
-Version: 0.1.4
+Version: 0.1.5
 Summary: Screen loops among brain structures(or any entities comprising a graph).
 Author-email: Zuohan Zhao <zzhmark@126.com>
 License: MIT License
 Project-URL: GitHub Project, https://github.com/SEU-ALLEN-codebase/brain-loop-search
 Project-URL: Documentation, https://SEU-ALLEN-codebase.github.io/brain-loop-search
 Keywords: neuron-morphology
 Classifier: Programming Language :: Python :: 3
```

### Comparing `brain-loop-search-0.1.4/brain_loop_search.egg-info/SOURCES.txt` & `brain-loop-search-0.1.5/brain_loop_search.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `brain-loop-search-0.1.4/pyproject.toml` & `brain-loop-search-0.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `brain-loop-search-0.1.4/test/test.png` & `brain-loop-search-0.1.5/test/test.png`

 * *Files identical despite different names*

### Comparing `brain-loop-search-0.1.4/test/test2.png` & `brain-loop-search-0.1.5/test/test2.png`

 * *Files identical despite different names*

### Comparing `brain-loop-search-0.1.4/test/test_flow.py` & `brain-loop-search-0.1.5/test/test_flow.py`

 * *Files identical despite different names*

### Comparing `brain-loop-search-0.1.4/test/test_graph_packing.py` & `brain-loop-search-0.1.5/test/test_graph_packing.py`

 * *Files identical despite different names*

### Comparing `brain-loop-search-0.1.4/test/test_ontology.py` & `brain-loop-search-0.1.5/test/test_ontology.py`

 * *Files identical despite different names*

### Comparing `brain-loop-search-0.1.4/test/test_sssp.py` & `brain-loop-search-0.1.5/test/test_sssp.py`

 * *Files identical despite different names*

### Comparing `brain-loop-search-0.1.4/test/test_vertex_packing.py` & `brain-loop-search-0.1.5/test/test_vertex_packing.py`

 * *Files identical despite different names*

### Comparing `brain-loop-search-0.1.4/test/test_vis.py` & `brain-loop-search-0.1.5/test/test_vis.py`

 * *Files identical despite different names*

