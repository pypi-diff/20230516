# Comparing `tmp/SC2Spa-1.1.6.tar.gz` & `tmp/SC2Spa-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SC2Spa-1.1.6.tar", last modified: Tue Mar 21 14:02:46 2023, max compression
+gzip compressed data, was "SC2Spa-1.1.7.tar", last modified: Tue May 16 14:41:53 2023, max compression
```

## Comparing `SC2Spa-1.1.6.tar` & `SC2Spa-1.1.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-21 14:02:46.157150 SC2Spa-1.1.6/
--rwxrwxrwx   0 root         (0) root         (0)     1525 2022-11-18 16:54:51.000000 SC2Spa-1.1.6/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)     1359 2023-03-21 14:02:46.156689 SC2Spa-1.1.6/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      806 2023-01-09 13:31:30.000000 SC2Spa-1.1.6/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-21 14:02:46.152194 SC2Spa-1.1.6/SC2Spa/
--rwxrwxrwx   0 root         (0) root         (0)    12963 2023-02-13 15:19:44.000000 SC2Spa-1.1.6/SC2Spa/BM.py
--rwxrwxrwx   0 root         (0) root         (0)     8248 2022-12-06 20:19:48.000000 SC2Spa-1.1.6/SC2Spa/ME.py
--rwxrwxrwx   0 root         (0) root         (0)     3062 2022-07-12 15:41:45.000000 SC2Spa-1.1.6/SC2Spa/PP.py
--rwxrwxrwx   0 root         (0) root         (0)    49667 2023-03-21 13:45:07.000000 SC2Spa-1.1.6/SC2Spa/SI.py
--rwxrwxrwx   0 root         (0) root         (0)     4381 2023-01-08 16:28:45.000000 SC2Spa-1.1.6/SC2Spa/SVA.py
--rwxrwxrwx   0 root         (0) root         (0)    19025 2023-03-13 13:23:49.000000 SC2Spa-1.1.6/SC2Spa/Vis.py
--rwxrwxrwx   0 root         (0) root         (0)      211 2023-03-14 16:25:06.000000 SC2Spa-1.1.6/SC2Spa/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      460 2023-03-14 16:25:06.000000 SC2Spa-1.1.6/SC2Spa/__metadata__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-21 14:02:46.155672 SC2Spa-1.1.6/SC2Spa.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     1359 2023-03-21 14:02:46.000000 SC2Spa-1.1.6/SC2Spa.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      274 2023-03-21 14:02:46.000000 SC2Spa-1.1.6/SC2Spa.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-03-21 14:02:46.000000 SC2Spa-1.1.6/SC2Spa.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)        7 2023-03-21 14:02:46.000000 SC2Spa-1.1.6/SC2Spa.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)      691 2023-03-21 14:01:31.000000 SC2Spa-1.1.6/pyproject.toml
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-03-21 14:02:46.157368 SC2Spa-1.1.6/setup.cfg
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-16 14:41:53.405084 SC2Spa-1.1.7/
+-rwxrwxrwx   0 root         (0) root         (0)     1525 2022-11-18 16:54:51.000000 SC2Spa-1.1.7/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)     1359 2023-05-16 14:41:53.404491 SC2Spa-1.1.7/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      806 2023-01-09 13:31:30.000000 SC2Spa-1.1.7/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-16 14:41:53.400001 SC2Spa-1.1.7/SC2Spa/
+-rwxrwxrwx   0 root         (0) root         (0)    12963 2023-02-13 15:19:44.000000 SC2Spa-1.1.7/SC2Spa/BM.py
+-rwxrwxrwx   0 root         (0) root         (0)     8248 2022-12-06 20:19:48.000000 SC2Spa-1.1.7/SC2Spa/ME.py
+-rwxrwxrwx   0 root         (0) root         (0)     3062 2022-07-12 15:41:45.000000 SC2Spa-1.1.7/SC2Spa/PP.py
+-rwxrwxrwx   0 root         (0) root         (0)    50176 2023-05-11 15:22:04.000000 SC2Spa-1.1.7/SC2Spa/SI.py
+-rwxrwxrwx   0 root         (0) root         (0)     4381 2023-01-08 16:28:45.000000 SC2Spa-1.1.7/SC2Spa/SVA.py
+-rwxrwxrwx   0 root         (0) root         (0)    21673 2023-05-15 15:40:00.000000 SC2Spa-1.1.7/SC2Spa/Vis.py
+-rwxrwxrwx   0 root         (0) root         (0)      211 2023-03-14 16:25:06.000000 SC2Spa-1.1.7/SC2Spa/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      460 2023-03-14 16:25:06.000000 SC2Spa-1.1.7/SC2Spa/__metadata__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-16 14:41:53.403477 SC2Spa-1.1.7/SC2Spa.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     1359 2023-05-16 14:41:53.000000 SC2Spa-1.1.7/SC2Spa.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      274 2023-05-16 14:41:53.000000 SC2Spa-1.1.7/SC2Spa.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-05-16 14:41:53.000000 SC2Spa-1.1.7/SC2Spa.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)        7 2023-05-16 14:41:53.000000 SC2Spa-1.1.7/SC2Spa.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)      691 2023-05-16 14:41:37.000000 SC2Spa-1.1.7/pyproject.toml
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-05-16 14:41:53.405291 SC2Spa-1.1.7/setup.cfg
```

### Comparing `SC2Spa-1.1.6/LICENSE` & `SC2Spa-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `SC2Spa-1.1.6/PKG-INFO` & `SC2Spa-1.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SC2Spa
-Version: 1.1.6
+Version: 1.1.7
 Summary: SC2Spa: a deep learning based approach to map transcriptome to spatial origins at cellular resolution
 Author-email: "Linbu Liao, Won Lab" <linbu.liao@gmail.com>
 Project-URL: Homepage, https://github.com/linbuliao/SC2Spa
 Project-URL: Bug Tracker, https://github.com/pypa/SC2Spa/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `SC2Spa-1.1.6/README.md` & `SC2Spa-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `SC2Spa-1.1.6/SC2Spa/BM.py` & `SC2Spa-1.1.7/SC2Spa/BM.py`

 * *Files identical despite different names*

### Comparing `SC2Spa-1.1.6/SC2Spa/ME.py` & `SC2Spa-1.1.7/SC2Spa/ME.py`

 * *Files identical despite different names*

### Comparing `SC2Spa-1.1.6/SC2Spa/PP.py` & `SC2Spa-1.1.7/SC2Spa/PP.py`

 * *Files identical despite different names*

### Comparing `SC2Spa-1.1.6/SC2Spa/SI.py` & `SC2Spa-1.1.7/SC2Spa/SI.py`

 * *Files 1% similar despite different names*

```diff
@@ -286,14 +286,16 @@
     WD_cutoff
         genes with Wasserstein distance lower than the cutoff will be selected
 
     Returns
     -------
     JGs
         A list that contains the select genes
+    WDs
+        A table contains
     '''
     adata_ref.var_names = adata_ref.var_names.str.upper()
     adata_query.var_names = adata_query.var_names.str.upper()
 
     adata_ref.var_names_make_unique()
     adata_query.var_names_make_unique()
 
@@ -779,14 +781,21 @@
         Number of the nearest neighbors of a bead or cell. This parameter is for
         the KNN algorithm
     dis_cutoff
         Limit for the distance between a single cell and a ST bead. In the process
          of fine mapping. Only the cells within the cutoff will be retained.
     FM
         Perform fine mapping and reconstruct ST data at single cell resolution if True
+    n_layer_cell
+        Number of cells in layers for sampling single cells for a ST bead.
+    cell_radius
+        Radius of a cell. For example, n_layer_cell=[1, 4] and cell_radius=5 means sampling 1 cell
+         from cells within 5 to a bead and at most 4 cells from cells between 5 and 15 to the bead.
+         It is at most 4 cells because a cell can be sampled more than once to deal with the case
+         that a bead has fewer cells than the user specified.
     seed
         seed for reconstructing the single-cell ST data
     '''
 
     # Extract values
     X_ref, X_query, Y_ref = PP_Mapping(adata_ref, adata_query, JGs = JGs,
                                        sparse = sparse, WD_cutoff = WD_cutoff)
```

### Comparing `SC2Spa-1.1.6/SC2Spa/SVA.py` & `SC2Spa-1.1.7/SC2Spa/SVA.py`

 * *Files identical despite different names*

### Comparing `SC2Spa-1.1.6/SC2Spa/Vis.py` & `SC2Spa-1.1.7/SC2Spa/Vis.py`

 * *Files 8% similar despite different names*

```diff
@@ -302,14 +302,16 @@
         Fine mapping result should be stored in `adata.obs['FM']` if `FM==True`
         Coordinate Information should be stored in `adata.obsm[coords_name]`
         Reconstruction info should be stored in adata.obs['Recon_scST']
     CT
         The cell type to be drawn. it must be one category in `adata.obs[c_name]`
     ax
         matplotlib ax where the figure is plotted
+    coords_name
+        Coordinate Information should be stored in `adata.obsm[coords_name]`
     s
         size of beads in the figure
     FM
         Draw finely mapped beads or cells if True.
     scST
         Draw reconstructed single-cell ST data if True.
     figsize
@@ -419,14 +421,96 @@
 
         plt.savefig(root + save + '_' + CT + '.png',
                     dpi=128, bbox_inches='tight')
 
     plt.show()
 
 
+def DrawCT3(adata: anndata.AnnData, CT_list: list, coords_name='spatial_mapping', s=3,
+            FM=True, scST=False, c_name='cell_type_med_resolution', legend=False,
+            root='Transfer1/FM_Valid3/', figsize=(10, 10), save=None):
+    '''
+    Display original locations or predicted locations of beads/cells of selected types.
+    Beads/cells are colored according to anatomy/cell type.
+    A figure will be saved to `root+save+'.png'`
+    The legend of the figure will be saved to `root + save + '_legend.png'`
+
+    Parameters
+    ---------
+    adata
+        anndata file.
+        Cell type information should be stored in `adata.obs[c_name]
+        Fine mapping result should be stored in `adata.obs['FM']` if `FM==True`
+        Coordinate Information should be stored in `adata.obsm[coords_name]`
+        Reconstruction info should be stored in adata.obs['Recon_scST']
+    CT_list
+        A list that contains the cell types to be shown. the cell types must
+        exist in `adata.obs[c_name]`
+    c_name
+        Name of cell type column in adata.obs
+    s
+        size of beads in the figure
+    legend
+        Draw legend in the figure if True
+
+    Returns
+    -------
+    None
+
+    '''
+
+    if (scST):
+        adata = adata[adata.obs['Recon_scST']]
+    elif (FM):
+        adata = adata[adata.obs['FM']]
+
+    adata_t = adata[adata.obs[c_name].apply(lambda x: x in CT_list)]
+
+    color_dic = {}
+    cts = sorted(adata_t.obs[c_name].unique())
+    for i, ct in enumerate(cts):
+        color_dic[ct] = i
+
+    color = list(map(lambda x: color_dic[x], adata_t.obs[c_name]))
+
+    if (figsize != None):
+        plt.figure(figsize=figsize)
+
+    coord = adata_t.obsm[coords_name]
+
+    scatter = plt.scatter(coord[:, 0], \
+                          coord[:, 1], \
+                          s=s, \
+                          c=color, \
+                          cmap=plt.get_cmap('Paired'))
+    plt.grid(False)
+    plt.axis('off')
+
+    if (legend):
+        plt.legend(handles=scatter.legend_elements()[0],
+                   labels=cts)
+
+    if ((save != None)):
+
+        if not os.path.exists(root):
+            os.makedirs(root)
+        plt.savefig(root + save + '.png',
+                    dpi=128, bbox_inches='tight')
+    plt.show()
+
+    ##Extract handles
+    handles = scatter.legend_elements()[0]
+
+    plt.legend(handles=scatter.legend_elements()[0],
+               labels=cts)
+    plt.savefig(root + save + '_legend.png', bbox_inches='tight')
+
+    plt.show()
+
+
 def Superimpose(adata:anndata.AnnData, coords_name='spatial', G1='APOE', G2='NRGN',
                 s = 2, C1 = 'Reds', C2 = 'Blues', figsize = (10, 10),
                 alpha1=0.5, alpha2=0.7, save_root = 'figures/BME/', save=True):
     '''
     Show the spatial gene expressions of two genes and their superimposed images
 
     The figures will be saved as if `save==True`:
```

### Comparing `SC2Spa-1.1.6/SC2Spa.egg-info/PKG-INFO` & `SC2Spa-1.1.7/SC2Spa.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SC2Spa
-Version: 1.1.6
+Version: 1.1.7
 Summary: SC2Spa: a deep learning based approach to map transcriptome to spatial origins at cellular resolution
 Author-email: "Linbu Liao, Won Lab" <linbu.liao@gmail.com>
 Project-URL: Homepage, https://github.com/linbuliao/SC2Spa
 Project-URL: Bug Tracker, https://github.com/pypa/SC2Spa/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `SC2Spa-1.1.6/pyproject.toml` & `SC2Spa-1.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "SC2Spa"
-version = "1.1.6"
+version = "1.1.7"
 authors = [
   { name="Linbu Liao, Won Lab", email="linbu.liao@gmail.com" },
 ]
 description = "SC2Spa: a deep learning based approach to map transcriptome to spatial origins at cellular resolution"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

