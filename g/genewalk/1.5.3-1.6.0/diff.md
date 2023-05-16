# Comparing `tmp/genewalk-1.5.3.tar.gz` & `tmp/genewalk-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/genewalk-1.5.3.tar", last modified: Mon May 10 14:52:18 2021, max compression
+gzip compressed data, was "dist/genewalk-1.6.0.tar", last modified: Tue May 16 19:22:30 2023, max compression
```

## Comparing `genewalk-1.5.3.tar` & `genewalk-1.6.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 horizon    (501) staff       (20)        0 2021-05-10 14:52:18.000000 genewalk-1.5.3/
--rw-r--r--   0 horizon    (501) staff       (20)       66 2021-01-27 21:08:32.000000 genewalk-1.5.3/MANIFEST.in
--rw-r--r--   0 horizon    (501) staff       (20)    23325 2021-05-10 14:52:18.000000 genewalk-1.5.3/PKG-INFO
--rw-r--r--   0 horizon    (501) staff       (20)    19695 2021-02-21 02:50:54.000000 genewalk-1.5.3/README.md
-drwxr-xr-x   0 horizon    (501) staff       (20)        0 2021-05-10 14:52:18.000000 genewalk-1.5.3/doc/
--rw-r--r--   0 horizon    (501) staff       (20)      606 2019-08-30 13:54:12.000000 genewalk-1.5.3/doc/Makefile
--rw-r--r--   0 horizon    (501) staff       (20)     5562 2021-05-10 13:19:36.000000 genewalk-1.5.3/doc/conf.py
--rw-r--r--   0 horizon    (501) staff       (20)      407 2019-08-30 13:54:12.000000 genewalk-1.5.3/doc/index.rst
--rw-r--r--   0 horizon    (501) staff       (20)      812 2019-08-30 13:54:12.000000 genewalk-1.5.3/doc/make.bat
-drwxr-xr-x   0 horizon    (501) staff       (20)        0 2021-05-10 14:52:18.000000 genewalk-1.5.3/doc/modules/
--rw-r--r--   0 horizon    (501) staff       (20)     1648 2021-01-27 21:08:32.000000 genewalk-1.5.3/doc/modules/genewalk.rst
--rw-r--r--   0 horizon    (501) staff       (20)      124 2019-08-30 13:54:12.000000 genewalk-1.5.3/doc/modules/index.rst
--rw-r--r--   0 horizon    (501) staff       (20)       83 2021-01-27 21:08:32.000000 genewalk-1.5.3/doc/requirements.txt
-drwxr-xr-x   0 horizon    (501) staff       (20)        0 2021-05-10 14:52:18.000000 genewalk-1.5.3/genewalk/
--rw-r--r--   0 horizon    (501) staff       (20)      478 2021-05-10 13:19:08.000000 genewalk-1.5.3/genewalk/__init__.py
--rw-r--r--   0 horizon    (501) staff       (20)    13310 2021-02-24 03:03:19.000000 genewalk-1.5.3/genewalk/cli.py
--rw-r--r--   0 horizon    (501) staff       (20)     8303 2020-02-26 02:19:30.000000 genewalk-1.5.3/genewalk/deepwalk.py
--rw-r--r--   0 horizon    (501) staff       (20)    16017 2021-02-21 02:50:54.000000 genewalk-1.5.3/genewalk/gene_lists.py
--rw-r--r--   0 horizon    (501) staff       (20)     7237 2020-09-21 20:38:26.000000 genewalk-1.5.3/genewalk/get_indra_stmts.py
--rw-r--r--   0 horizon    (501) staff       (20)     1613 2020-02-26 02:19:30.000000 genewalk-1.5.3/genewalk/null_distributions.py
--rw-r--r--   0 horizon    (501) staff       (20)    17380 2021-05-10 13:16:56.000000 genewalk-1.5.3/genewalk/nx_mg_assembler.py
--rw-r--r--   0 horizon    (501) staff       (20)    13366 2021-02-21 02:50:54.000000 genewalk-1.5.3/genewalk/perform_statistics.py
--rw-r--r--   0 horizon    (501) staff       (20)    18257 2021-02-21 02:50:54.000000 genewalk-1.5.3/genewalk/plot.py
--rw-r--r--   0 horizon    (501) staff       (20)     5406 2021-02-21 02:50:54.000000 genewalk-1.5.3/genewalk/resources.py
--rw-r--r--   0 horizon    (501) staff       (20)      442 2021-01-27 21:08:32.000000 genewalk-1.5.3/genewalk/results_template.html
-drwxr-xr-x   0 horizon    (501) staff       (20)        0 2021-05-10 14:52:18.000000 genewalk-1.5.3/genewalk/tests/
--rw-r--r--   0 horizon    (501) staff       (20)        0 2019-08-30 13:54:12.000000 genewalk-1.5.3/genewalk/tests/__init__.py
--rw-r--r--   0 horizon    (501) staff       (20)     6255 2021-02-21 02:50:54.000000 genewalk-1.5.3/genewalk/tests/test_cli.py
--rw-r--r--   0 horizon    (501) staff       (20)      735 2020-02-26 02:19:30.000000 genewalk-1.5.3/genewalk/tests/test_deepwalk.py
--rw-r--r--   0 horizon    (501) staff       (20)     3381 2021-02-21 02:50:54.000000 genewalk-1.5.3/genewalk/tests/test_gene_lists.py
--rw-r--r--   0 horizon    (501) staff       (20)      719 2021-02-21 02:50:54.000000 genewalk-1.5.3/genewalk/tests/test_indra_assembly.py
--rw-r--r--   0 horizon    (501) staff       (20)     5185 2021-02-21 02:50:54.000000 genewalk-1.5.3/genewalk/tests/test_sif_assembler.py
--rw-r--r--   0 horizon    (501) staff       (20)      988 2021-01-27 21:08:32.000000 genewalk-1.5.3/genewalk/tests/test_visualize.py
--rw-r--r--   0 horizon    (501) staff       (20)      815 2021-02-21 02:50:54.000000 genewalk-1.5.3/genewalk/tests/util.py
-drwxr-xr-x   0 horizon    (501) staff       (20)        0 2021-05-10 14:52:18.000000 genewalk-1.5.3/genewalk.egg-info/
--rw-r--r--   0 horizon    (501) staff       (20)    23325 2021-05-10 14:52:18.000000 genewalk-1.5.3/genewalk.egg-info/PKG-INFO
--rw-r--r--   0 horizon    (501) staff       (20)      874 2021-05-10 14:52:18.000000 genewalk-1.5.3/genewalk.egg-info/SOURCES.txt
--rw-r--r--   0 horizon    (501) staff       (20)        1 2021-05-10 14:52:18.000000 genewalk-1.5.3/genewalk.egg-info/dependency_links.txt
--rw-r--r--   0 horizon    (501) staff       (20)       48 2021-05-10 14:52:18.000000 genewalk-1.5.3/genewalk.egg-info/entry_points.txt
--rw-r--r--   0 horizon    (501) staff       (20)      106 2021-05-10 14:52:18.000000 genewalk-1.5.3/genewalk.egg-info/requires.txt
--rw-r--r--   0 horizon    (501) staff       (20)        9 2021-05-10 14:52:18.000000 genewalk-1.5.3/genewalk.egg-info/top_level.txt
--rw-r--r--   0 horizon    (501) staff       (20)       79 2021-05-10 14:52:18.000000 genewalk-1.5.3/setup.cfg
--rwxr-xr-x   0 horizon    (501) staff       (20)     1657 2021-05-10 13:18:43.000000 genewalk-1.5.3/setup.py
+drwxr-xr-x   0 horizon    (501) staff       (20)        0 2023-05-16 19:22:30.000000 genewalk-1.6.0/
+-rw-r--r--   0 horizon    (501) staff       (20)       66 2021-01-27 21:08:32.000000 genewalk-1.6.0/MANIFEST.in
+-rw-r--r--   0 horizon    (501) staff       (20)    23541 2023-05-16 19:22:30.000000 genewalk-1.6.0/PKG-INFO
+-rw-r--r--   0 horizon    (501) staff       (20)    19851 2023-05-16 19:20:53.000000 genewalk-1.6.0/README.md
+drwxr-xr-x   0 horizon    (501) staff       (20)        0 2023-05-16 19:22:30.000000 genewalk-1.6.0/doc/
+-rw-r--r--   0 horizon    (501) staff       (20)      606 2019-08-30 13:54:12.000000 genewalk-1.6.0/doc/Makefile
+-rw-r--r--   0 horizon    (501) staff       (20)     5562 2023-05-16 19:20:53.000000 genewalk-1.6.0/doc/conf.py
+-rw-r--r--   0 horizon    (501) staff       (20)      407 2019-08-30 13:54:12.000000 genewalk-1.6.0/doc/index.rst
+-rw-r--r--   0 horizon    (501) staff       (20)      812 2019-08-30 13:54:12.000000 genewalk-1.6.0/doc/make.bat
+drwxr-xr-x   0 horizon    (501) staff       (20)        0 2023-05-16 19:22:30.000000 genewalk-1.6.0/doc/modules/
+-rw-r--r--   0 horizon    (501) staff       (20)     1648 2021-01-27 21:08:32.000000 genewalk-1.6.0/doc/modules/genewalk.rst
+-rw-r--r--   0 horizon    (501) staff       (20)      124 2019-08-30 13:54:12.000000 genewalk-1.6.0/doc/modules/index.rst
+-rw-r--r--   0 horizon    (501) staff       (20)       83 2021-01-27 21:08:32.000000 genewalk-1.6.0/doc/requirements.txt
+drwxr-xr-x   0 horizon    (501) staff       (20)        0 2023-05-16 19:22:30.000000 genewalk-1.6.0/genewalk/
+-rw-r--r--   0 horizon    (501) staff       (20)      478 2023-05-16 19:20:53.000000 genewalk-1.6.0/genewalk/__init__.py
+-rw-r--r--   0 horizon    (501) staff       (20)    13352 2023-05-16 19:20:53.000000 genewalk-1.6.0/genewalk/cli.py
+-rw-r--r--   0 horizon    (501) staff       (20)     8361 2023-05-16 19:20:53.000000 genewalk-1.6.0/genewalk/deepwalk.py
+-rw-r--r--   0 horizon    (501) staff       (20)    16017 2021-02-21 02:50:54.000000 genewalk-1.6.0/genewalk/gene_lists.py
+-rw-r--r--   0 horizon    (501) staff       (20)     7237 2020-09-21 20:38:26.000000 genewalk-1.6.0/genewalk/get_indra_stmts.py
+-rw-r--r--   0 horizon    (501) staff       (20)     1613 2020-02-26 02:19:30.000000 genewalk-1.6.0/genewalk/null_distributions.py
+-rw-r--r--   0 horizon    (501) staff       (20)    17380 2021-05-10 13:16:56.000000 genewalk-1.6.0/genewalk/nx_mg_assembler.py
+-rw-r--r--   0 horizon    (501) staff       (20)    13342 2023-05-16 19:20:53.000000 genewalk-1.6.0/genewalk/perform_statistics.py
+-rw-r--r--   0 horizon    (501) staff       (20)    18257 2021-02-21 02:50:54.000000 genewalk-1.6.0/genewalk/plot.py
+-rw-r--r--   0 horizon    (501) staff       (20)     5406 2021-02-21 02:50:54.000000 genewalk-1.6.0/genewalk/resources.py
+-rw-r--r--   0 horizon    (501) staff       (20)      442 2021-01-27 21:08:32.000000 genewalk-1.6.0/genewalk/results_template.html
+drwxr-xr-x   0 horizon    (501) staff       (20)        0 2023-05-16 19:22:30.000000 genewalk-1.6.0/genewalk/tests/
+-rw-r--r--   0 horizon    (501) staff       (20)        0 2019-08-30 13:54:12.000000 genewalk-1.6.0/genewalk/tests/__init__.py
+-rw-r--r--   0 horizon    (501) staff       (20)     6255 2021-02-21 02:50:54.000000 genewalk-1.6.0/genewalk/tests/test_cli.py
+-rw-r--r--   0 horizon    (501) staff       (20)      735 2020-02-26 02:19:30.000000 genewalk-1.6.0/genewalk/tests/test_deepwalk.py
+-rw-r--r--   0 horizon    (501) staff       (20)     3381 2021-02-21 02:50:54.000000 genewalk-1.6.0/genewalk/tests/test_gene_lists.py
+-rw-r--r--   0 horizon    (501) staff       (20)      719 2021-02-21 02:50:54.000000 genewalk-1.6.0/genewalk/tests/test_indra_assembly.py
+-rw-r--r--   0 horizon    (501) staff       (20)     5185 2021-02-21 02:50:54.000000 genewalk-1.6.0/genewalk/tests/test_sif_assembler.py
+-rw-r--r--   0 horizon    (501) staff       (20)      988 2021-01-27 21:08:32.000000 genewalk-1.6.0/genewalk/tests/test_visualize.py
+-rw-r--r--   0 horizon    (501) staff       (20)      815 2021-02-21 02:50:54.000000 genewalk-1.6.0/genewalk/tests/util.py
+drwxr-xr-x   0 horizon    (501) staff       (20)        0 2023-05-16 19:22:30.000000 genewalk-1.6.0/genewalk.egg-info/
+-rw-r--r--   0 horizon    (501) staff       (20)    23541 2023-05-16 19:22:30.000000 genewalk-1.6.0/genewalk.egg-info/PKG-INFO
+-rw-r--r--   0 horizon    (501) staff       (20)      874 2023-05-16 19:22:30.000000 genewalk-1.6.0/genewalk.egg-info/SOURCES.txt
+-rw-r--r--   0 horizon    (501) staff       (20)        1 2023-05-16 19:22:30.000000 genewalk-1.6.0/genewalk.egg-info/dependency_links.txt
+-rw-r--r--   0 horizon    (501) staff       (20)       48 2023-05-16 19:22:30.000000 genewalk-1.6.0/genewalk.egg-info/entry_points.txt
+-rw-r--r--   0 horizon    (501) staff       (20)      111 2023-05-16 19:22:30.000000 genewalk-1.6.0/genewalk.egg-info/requires.txt
+-rw-r--r--   0 horizon    (501) staff       (20)        9 2023-05-16 19:22:30.000000 genewalk-1.6.0/genewalk.egg-info/top_level.txt
+-rw-r--r--   0 horizon    (501) staff       (20)       79 2023-05-16 19:22:30.000000 genewalk-1.6.0/setup.cfg
+-rwxr-xr-x   0 horizon    (501) staff       (20)     1717 2023-05-16 19:20:53.000000 genewalk-1.6.0/setup.py
```

### Comparing `genewalk-1.5.3/PKG-INFO` & `genewalk-1.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: genewalk
-Version: 1.5.3
+Version: 1.6.0
 Summary: Determine gene function based on network embeddings.
 Home-page: https://github.com/churchmanlab/genewalk
 Author: Robert Ietswaart
 Author-email: robert_ietswaart@hms.harvard.edu
 License: UNKNOWN
 Description: # GeneWalk
         
         [![License](https://img.shields.io/badge/License-BSD%202--Clause-orange.svg)](https://opensource.org/licenses/BSD-2-Clause)
         [![Documentation](https://readthedocs.org/projects/genewalk/badge/?version=latest)](https://genewalk.readthedocs.io/en/latest/?badge=latest)
         [![PyPI version](https://badge.fury.io/py/genewalk.svg)](https://badge.fury.io/py/genewalk)
-        [![Python 3.6+](https://img.shields.io/pypi/pyversions/genewalk.svg)](https://www.python.org/downloads/release)
+        [![install with bioconda](https://img.shields.io/badge/install%20with-bioconda-brightgreen.svg?style=flat)](http://bioconda.github.io/recipes/genewalk/README.html)
+        [![Python 3.8+](https://img.shields.io/pypi/pyversions/genewalk.svg)](https://www.python.org/downloads)
         
         GeneWalk determines for individual genes the functions that are relevant in a
         particular biological context and experimental condition. GeneWalk quantifies
         the similarity between vector representations of a gene and annotated GO terms
         through representation learning with random walks on a condition-specific gene
         regulatory network. Similarity significance is determined through comparison
         with node similarities from randomized networks.
@@ -360,13 +361,14 @@
 Keywords: gene function,network,embedding
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Description-Content-Type: text/markdown
 Provides-Extra: indra
```

### Comparing `genewalk-1.5.3/README.md` & `genewalk-1.6.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # GeneWalk
 
 [![License](https://img.shields.io/badge/License-BSD%202--Clause-orange.svg)](https://opensource.org/licenses/BSD-2-Clause)
 [![Documentation](https://readthedocs.org/projects/genewalk/badge/?version=latest)](https://genewalk.readthedocs.io/en/latest/?badge=latest)
 [![PyPI version](https://badge.fury.io/py/genewalk.svg)](https://badge.fury.io/py/genewalk)
-[![Python 3.6+](https://img.shields.io/pypi/pyversions/genewalk.svg)](https://www.python.org/downloads/release)
+[![install with bioconda](https://img.shields.io/badge/install%20with-bioconda-brightgreen.svg?style=flat)](http://bioconda.github.io/recipes/genewalk/README.html)
+[![Python 3.8+](https://img.shields.io/pypi/pyversions/genewalk.svg)](https://www.python.org/downloads)
 
 GeneWalk determines for individual genes the functions that are relevant in a
 particular biological context and experimental condition. GeneWalk quantifies
 the similarity between vector representations of a gene and annotated GO terms
 through representation learning with random walks on a condition-specific gene
 regulatory network. Similarity significance is determined through comparison
 with node similarities from randomized networks.
```

### Comparing `genewalk-1.5.3/doc/Makefile` & `genewalk-1.6.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `genewalk-1.5.3/doc/conf.py` & `genewalk-1.6.0/doc/conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,17 +21,17 @@
 # -- Project information -----------------------------------------------------
 
 project = 'GeneWalk'
 copyright = '2019, GeneWalk Developers'
 author = 'GeneWalk Developers'
 
 # The short X.Y version
-version = '1.5'
+version = '1.6'
 # The full version, including alpha/beta/rc tags
-release = '1.5.3'
+release = '1.6.0'
 
 
 # -- General configuration ---------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
```

### Comparing `genewalk-1.5.3/doc/make.bat` & `genewalk-1.6.0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `genewalk-1.5.3/doc/modules/genewalk.rst` & `genewalk-1.6.0/doc/modules/genewalk.rst`

 * *Files identical despite different names*

### Comparing `genewalk-1.5.3/genewalk/cli.py` & `genewalk-1.6.0/genewalk/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -195,15 +195,16 @@
         genes = read_gene_list(args.genes, args.id_type, rm)
         save_pickle(genes, project_folder, 'genes')
         MG = load_network(args.network_source, args.network_file, genes,
                           resource_manager=rm)
         save_pickle(MG.graph, project_folder, 'multi_graph')
         for i in range(args.nreps_graph):
             logger.info('%s/%s' % (i + 1, args.nreps_graph))
-            DW = run_walks(MG.graph, workers=args.nproc, size=args.dim_rep)
+            DW = run_walks(MG.graph, workers=args.nproc, 
+                           vector_size=args.dim_rep)
 
             # Pickle the node vectors (embeddings) and DW object
             if args.save_dw:
                 save_pickle(DW, project_folder, 'deepwalk_%d' % (i + 1))
             nv = copy.deepcopy(DW.model.wv)
             save_pickle(nv, project_folder,
                         'deepwalk_node_vectors_%d' % (i + 1))
@@ -214,15 +215,15 @@
 
     if args.stage in ('all', 'null_distribution'):
         MG = load_pickle(project_folder, 'multi_graph')
         srd = []
         for i in range(args.nreps_null):
             logger.info('%s/%s' % (i + 1, args.nreps_null))
             RG = get_rand_graph(MG)
-            DW = run_walks(RG, workers=args.nproc, size=args.dim_rep)
+            DW = run_walks(RG, workers=args.nproc, vector_size=args.dim_rep)
 
             # Pickle the node vectors (embeddings) and DW object
             if args.save_dw:
                 save_pickle(DW, project_folder, 'deepwalk_rand_%d' % (i + 1))
             nv = copy.deepcopy(DW.model.wv)
             save_pickle(nv, project_folder, 'deepwalk_node_vectors_rand_%d'
                                             % (i + 1))
```

### Comparing `genewalk-1.5.3/genewalk/deepwalk.py` & `genewalk-1.6.0/genewalk/deepwalk.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,28 +91,28 @@
             pool.close()
             logger.debug("Joining pool...")
             pool.join()
             logger.debug("Pool closed and joined.")
         end = time.time()
         logger.info('Running random walks done in %.2fs' % (end - start))
 
-    def word2vec(self, sg=1, size=8, window=1, min_count=1, negative=5,
+    def word2vec(self, sg=1, vector_size=8, window=1, min_count=1, negative=5,
                  workers=1, sample=0):
         """Set the model based on Word2Vec
         Source: https://radimrehurek.com/gensim/models/word2vec.html
 
         Note that his function sets the model attribute if the DeepWalk object
         and doesn't return a value.
 
         Parameters
         ----------
         sg : Optional[int] {1, 0}
             Defines the training algorithm. If 1, skip-gram is employed;
             otherwise, CBOW is used. For GeneWalk this is set to 1.
-        size : Optional[int]
+        vector_size : Optional[int]
             Dimensionality of the node vectors. Default for GeneWalk is 8.
         window : Optional[int]
             a.k.a. context size. Maximum distance between the current and
             predicted word within a sentence. For GeneWalk this is set to 1
             to assess directly connected nodes only.
         min_count : Optional[int]
             Ignores all words with total frequency lower than this. For
@@ -128,15 +128,16 @@
         sample : Optional[float]
             The threshold for configuring which higher-frequency words are
             randomly downsampled, useful range is (0, 1e-5). parameter t in eq
             5 Mikolov et al. For GeneWalk this is set to 0.
         """
         logger.info('Generating node vectors...')
         start = time.time()
-        self.model = Word2Vec(sentences=self.walks, sg=sg, size=size,
+        self.model = Word2Vec(sentences=self.walks, sg=sg, 
+                              vector_size=vector_size,
                               window=window, min_count=min_count,
                               negative=negative, workers=workers,
                               sample=sample)
         end = time.time()
         logger.info('Generating node vectors done in %.2fs'
                     % (end - start))
 
@@ -219,8 +220,8 @@
         of random walks produced on the graph.
     """
     dw_args = {'walk_length': kwargs.pop('walk_length', default_walk_length),
                'niter': kwargs.pop('niter', default_niter)}
     DW = DeepWalk(graph, **dw_args)
     DW.get_walks(kwargs.get('workers', 1))
     DW.word2vec(**kwargs)
-    return DW
+    return DW
```

### Comparing `genewalk-1.5.3/genewalk/gene_lists.py` & `genewalk-1.6.0/genewalk/gene_lists.py`

 * *Files identical despite different names*

### Comparing `genewalk-1.5.3/genewalk/get_indra_stmts.py` & `genewalk-1.6.0/genewalk/get_indra_stmts.py`

 * *Files identical despite different names*

### Comparing `genewalk-1.5.3/genewalk/null_distributions.py` & `genewalk-1.6.0/genewalk/null_distributions.py`

 * *Files identical despite different names*

### Comparing `genewalk-1.5.3/genewalk/nx_mg_assembler.py` & `genewalk-1.6.0/genewalk/nx_mg_assembler.py`

 * *Files identical despite different names*

### Comparing `genewalk-1.5.3/genewalk/perform_statistics.py` & `genewalk-1.6.0/genewalk/perform_statistics.py`

 * *Files 1% similar despite different names*

```diff
@@ -230,16 +230,16 @@
             header = [self.gene_id_type] + header
 
         df = pd.DataFrame.from_records(rows, columns=header)
         df = self.global_fdr(df,alpha_fdr)
         df.drop(['pval_rep'+str(i) for i in range(len(self.nvs))],
                 axis=1, inplace=True) 
         df[self.gene_id_type] = df[self.gene_id_type].astype('category')
-        df[self.gene_id_type].cat.set_categories(df[self.gene_id_type].unique(),
-                                            inplace=True)
+        df[self.gene_id_type] = \
+        df[self.gene_id_type].cat.set_categories(df[self.gene_id_type].unique())
         df[['ncon_gene', 'ncon_go']] = \
             df[['ncon_gene', 'ncon_go']].astype('str')
         df = df.sort_values(by=[self.gene_id_type, 'global_padj', 'gene_padj',
                                 'sim', 'go_domain', 'go_name'],
                             ascending=[True, True, True, False, True, True])
         if self.gene_id_type == 'custom':
             df.drop(['hgnc_symbol','hgnc_id'],axis=1, inplace=True)
```

### Comparing `genewalk-1.5.3/genewalk/plot.py` & `genewalk-1.6.0/genewalk/plot.py`

 * *Files identical despite different names*

### Comparing `genewalk-1.5.3/genewalk/resources.py` & `genewalk-1.6.0/genewalk/resources.py`

 * *Files identical despite different names*

### Comparing `genewalk-1.5.3/genewalk/tests/test_cli.py` & `genewalk-1.6.0/genewalk/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `genewalk-1.5.3/genewalk/tests/test_deepwalk.py` & `genewalk-1.6.0/genewalk/tests/test_deepwalk.py`

 * *Files identical despite different names*

### Comparing `genewalk-1.5.3/genewalk/tests/test_gene_lists.py` & `genewalk-1.6.0/genewalk/tests/test_gene_lists.py`

 * *Files identical despite different names*

### Comparing `genewalk-1.5.3/genewalk/tests/test_indra_assembly.py` & `genewalk-1.6.0/genewalk/tests/test_indra_assembly.py`

 * *Files identical despite different names*

### Comparing `genewalk-1.5.3/genewalk/tests/test_sif_assembler.py` & `genewalk-1.6.0/genewalk/tests/test_sif_assembler.py`

 * *Files identical despite different names*

### Comparing `genewalk-1.5.3/genewalk/tests/test_visualize.py` & `genewalk-1.6.0/genewalk/tests/test_visualize.py`

 * *Files identical despite different names*

### Comparing `genewalk-1.5.3/genewalk/tests/util.py` & `genewalk-1.6.0/genewalk/tests/util.py`

 * *Files identical despite different names*

### Comparing `genewalk-1.5.3/genewalk.egg-info/PKG-INFO` & `genewalk-1.6.0/genewalk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: genewalk
-Version: 1.5.3
+Version: 1.6.0
 Summary: Determine gene function based on network embeddings.
 Home-page: https://github.com/churchmanlab/genewalk
 Author: Robert Ietswaart
 Author-email: robert_ietswaart@hms.harvard.edu
 License: UNKNOWN
 Description: # GeneWalk
         
         [![License](https://img.shields.io/badge/License-BSD%202--Clause-orange.svg)](https://opensource.org/licenses/BSD-2-Clause)
         [![Documentation](https://readthedocs.org/projects/genewalk/badge/?version=latest)](https://genewalk.readthedocs.io/en/latest/?badge=latest)
         [![PyPI version](https://badge.fury.io/py/genewalk.svg)](https://badge.fury.io/py/genewalk)
-        [![Python 3.6+](https://img.shields.io/pypi/pyversions/genewalk.svg)](https://www.python.org/downloads/release)
+        [![install with bioconda](https://img.shields.io/badge/install%20with-bioconda-brightgreen.svg?style=flat)](http://bioconda.github.io/recipes/genewalk/README.html)
+        [![Python 3.8+](https://img.shields.io/pypi/pyversions/genewalk.svg)](https://www.python.org/downloads)
         
         GeneWalk determines for individual genes the functions that are relevant in a
         particular biological context and experimental condition. GeneWalk quantifies
         the similarity between vector representations of a gene and annotated GO terms
         through representation learning with random walks on a condition-specific gene
         regulatory network. Similarity significance is determined through comparison
         with node similarities from randomized networks.
@@ -360,13 +361,14 @@
 Keywords: gene function,network,embedding
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Description-Content-Type: text/markdown
 Provides-Extra: indra
```

### Comparing `genewalk-1.5.3/genewalk.egg-info/SOURCES.txt` & `genewalk-1.6.0/genewalk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `genewalk-1.5.3/setup.py` & `genewalk-1.6.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,34 +4,35 @@
 here = path.abspath(path.dirname(__file__))
 
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 
 def main():
-    install_list = ['numpy', 'pandas', 'networkx>=2.1', 'gensim<4', 'goatools',
+    install_list = ['numpy', 'pandas', 'networkx>=2.1', 'gensim>=4.0.0', 'goatools',
                     'scipy>=1.3.0', 'matplotlib', 'seaborn', 'plotly>=4.0.0']
 
     setup(name='genewalk',
-          version='1.5.3',
+          version='1.6.0',
           description='Determine gene function based on network embeddings.',
           long_description=long_description,
           long_description_content_type='text/markdown',
           author='Robert Ietswaart',
           author_email='robert_ietswaart@hms.harvard.edu',
           url='https://github.com/churchmanlab/genewalk',
           classifiers=[
             'Development Status :: 4 - Beta',
             'Environment :: Console',
             'Intended Audience :: Science/Research',
             'License :: OSI Approved :: BSD License',
             'Operating System :: OS Independent',
-            'Programming Language :: Python :: 3.6',
-            'Programming Language :: Python :: 3.7',
             'Programming Language :: Python :: 3.8',
+            'Programming Language :: Python :: 3.9',
+            'Programming Language :: Python :: 3.10',
+            'Programming Language :: Python :: 3.11',
             'Topic :: Scientific/Engineering :: Bio-Informatics',
             ],
           keywords=['gene function', 'network', 'embedding'],
           packages=find_packages(),
           install_requires=install_list,
           extras_require={'indra': ['indra']},
           tests_require=['nose'],
```

