# Comparing `tmp/PyComplexHeatmap-1.4.2.tar.gz` & `tmp/PyComplexHeatmap-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyComplexHeatmap-1.4.2.tar", last modified: Sun May  7 03:26:15 2023, max compression
+gzip compressed data, was "PyComplexHeatmap-1.4.3.tar", last modified: Mon May 15 23:22:54 2023, max compression
```

## Comparing `PyComplexHeatmap-1.4.2.tar` & `PyComplexHeatmap-1.4.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 wding     (8051) wding    (17694)        0 2023-05-07 03:26:15.502252 PyComplexHeatmap-1.4.2/
--rw-rw-r--   0 wding     (8051) wding    (17694)     1067 2023-05-05 16:24:49.000000 PyComplexHeatmap-1.4.2/LICENSE
--rw-rw-r--   0 wding     (8051) wding    (17694)      105 2023-05-05 16:24:49.000000 PyComplexHeatmap-1.4.2/MANIFEST.in
--rw-rw-r--   0 wding     (8051) wding    (17694)    11704 2023-05-07 03:26:15.487258 PyComplexHeatmap-1.4.2/PKG-INFO
-drwxrwxr-x   0 wding     (8051) wding    (17694)        0 2023-05-07 03:26:15.460256 PyComplexHeatmap-1.4.2/PyComplexHeatmap/
--rw-rw-r--   0 wding     (8051) wding    (17694)      375 2023-05-07 03:25:44.000000 PyComplexHeatmap-1.4.2/PyComplexHeatmap/__init__.py
--rw-rw-r--   0 wding     (8051) wding    (17694)    65607 2023-05-07 01:41:34.000000 PyComplexHeatmap-1.4.2/PyComplexHeatmap/annotations.py
--rw-rw-r--   0 wding     (8051) wding    (17694)    70631 2023-05-05 16:24:49.000000 PyComplexHeatmap-1.4.2/PyComplexHeatmap/clustermap.py
--rw-rw-r--   0 wding     (8051) wding    (17694)     5495 2023-05-05 16:24:49.000000 PyComplexHeatmap-1.4.2/PyComplexHeatmap/colors.py
--rw-rw-r--   0 wding     (8051) wding    (17694)    21247 2023-05-05 16:24:49.000000 PyComplexHeatmap-1.4.2/PyComplexHeatmap/dotHeatmap.py
--rw-rw-r--   0 wding     (8051) wding    (17694)     6766 2023-05-05 16:24:49.000000 PyComplexHeatmap-1.4.2/PyComplexHeatmap/example.py
--rw-rw-r--   0 wding     (8051) wding    (17694)    17814 2023-05-05 16:24:49.000000 PyComplexHeatmap-1.4.2/PyComplexHeatmap/oncoPrint.py
--rw-rw-r--   0 wding     (8051) wding    (17694)     6753 2023-05-05 16:24:49.000000 PyComplexHeatmap-1.4.2/PyComplexHeatmap/tools.py
--rw-rw-r--   0 wding     (8051) wding    (17694)    25817 2023-05-06 22:12:59.000000 PyComplexHeatmap-1.4.2/PyComplexHeatmap/utils.py
-drwxrwxr-x   0 wding     (8051) wding    (17694)        0 2023-05-07 03:26:15.486256 PyComplexHeatmap-1.4.2/PyComplexHeatmap.egg-info/
--rw-rw-r--   0 wding     (8051) wding    (17694)    11704 2023-05-07 03:26:15.000000 PyComplexHeatmap-1.4.2/PyComplexHeatmap.egg-info/PKG-INFO
--rw-rw-r--   0 wding     (8051) wding    (17694)      473 2023-05-07 03:26:15.000000 PyComplexHeatmap-1.4.2/PyComplexHeatmap.egg-info/SOURCES.txt
--rw-rw-r--   0 wding     (8051) wding    (17694)        1 2023-05-07 03:26:15.000000 PyComplexHeatmap-1.4.2/PyComplexHeatmap.egg-info/dependency_links.txt
--rw-rw-r--   0 wding     (8051) wding    (17694)       17 2023-05-07 03:26:15.000000 PyComplexHeatmap-1.4.2/PyComplexHeatmap.egg-info/top_level.txt
--rw-rw-r--   0 wding     (8051) wding    (17694)    11095 2023-05-05 17:28:56.000000 PyComplexHeatmap-1.4.2/README.md
--rw-rw-r--   0 wding     (8051) wding    (17694)      672 2023-05-07 03:25:35.000000 PyComplexHeatmap-1.4.2/pyproject.toml
--rw-rw-r--   0 wding     (8051) wding    (17694)       38 2023-05-07 03:26:15.502256 PyComplexHeatmap-1.4.2/setup.cfg
--rw-rw-r--   0 wding     (8051) wding    (17694)     1044 2023-05-07 03:25:27.000000 PyComplexHeatmap-1.4.2/setup.py
+drwxr-xr-x   0 wding      (503) staff       (20)        0 2023-05-15 23:22:54.785860 PyComplexHeatmap-1.4.3/
+-rw-r--r--   0 wding      (503) staff       (20)     1067 2023-05-08 23:39:01.000000 PyComplexHeatmap-1.4.3/LICENSE
+-rw-r--r--   0 wding      (503) staff       (20)      105 2023-05-08 23:39:01.000000 PyComplexHeatmap-1.4.3/MANIFEST.in
+-rw-r--r--   0 wding      (503) staff       (20)    11704 2023-05-15 23:22:54.785353 PyComplexHeatmap-1.4.3/PKG-INFO
+drwxr-xr-x   0 wding      (503) staff       (20)        0 2023-05-15 23:22:54.782393 PyComplexHeatmap-1.4.3/PyComplexHeatmap/
+-rw-r--r--   0 wding      (503) staff       (20)      387 2023-05-15 23:22:07.000000 PyComplexHeatmap-1.4.3/PyComplexHeatmap/__init__.py
+-rw-r--r--   0 wding      (503) staff       (20)    65863 2023-05-12 20:49:25.000000 PyComplexHeatmap-1.4.3/PyComplexHeatmap/annotations.py
+-rw-r--r--   0 wding      (503) staff       (20)    70857 2023-05-13 05:04:42.000000 PyComplexHeatmap-1.4.3/PyComplexHeatmap/clustermap.py
+-rw-r--r--   0 wding      (503) staff       (20)     5430 2023-05-15 19:27:29.000000 PyComplexHeatmap-1.4.3/PyComplexHeatmap/colors.py
+-rw-r--r--   0 wding      (503) staff       (20)    21247 2023-05-08 23:39:01.000000 PyComplexHeatmap-1.4.3/PyComplexHeatmap/dotHeatmap.py
+-rw-r--r--   0 wding      (503) staff       (20)     6766 2023-05-08 23:39:01.000000 PyComplexHeatmap-1.4.3/PyComplexHeatmap/example.py
+-rw-r--r--   0 wding      (503) staff       (20)    17814 2023-05-08 23:39:01.000000 PyComplexHeatmap-1.4.3/PyComplexHeatmap/oncoPrint.py
+-rw-r--r--   0 wding      (503) staff       (20)     6753 2023-05-08 23:39:01.000000 PyComplexHeatmap-1.4.3/PyComplexHeatmap/tools.py
+-rw-r--r--   0 wding      (503) staff       (20)    26408 2023-05-15 19:27:56.000000 PyComplexHeatmap-1.4.3/PyComplexHeatmap/utils.py
+drwxr-xr-x   0 wding      (503) staff       (20)        0 2023-05-15 23:22:54.784769 PyComplexHeatmap-1.4.3/PyComplexHeatmap.egg-info/
+-rw-r--r--   0 wding      (503) staff       (20)    11704 2023-05-15 23:22:54.000000 PyComplexHeatmap-1.4.3/PyComplexHeatmap.egg-info/PKG-INFO
+-rw-r--r--   0 wding      (503) staff       (20)      473 2023-05-15 23:22:54.000000 PyComplexHeatmap-1.4.3/PyComplexHeatmap.egg-info/SOURCES.txt
+-rw-r--r--   0 wding      (503) staff       (20)        1 2023-05-15 23:22:54.000000 PyComplexHeatmap-1.4.3/PyComplexHeatmap.egg-info/dependency_links.txt
+-rw-r--r--   0 wding      (503) staff       (20)       17 2023-05-15 23:22:54.000000 PyComplexHeatmap-1.4.3/PyComplexHeatmap.egg-info/top_level.txt
+-rw-r--r--   0 wding      (503) staff       (20)    11095 2023-05-08 23:39:01.000000 PyComplexHeatmap-1.4.3/README.md
+-rw-r--r--   0 wding      (503) staff       (20)      672 2023-05-15 23:22:21.000000 PyComplexHeatmap-1.4.3/pyproject.toml
+-rw-r--r--   0 wding      (503) staff       (20)       38 2023-05-15 23:22:54.786080 PyComplexHeatmap-1.4.3/setup.cfg
+-rw-r--r--   0 wding      (503) staff       (20)     1044 2023-05-15 23:22:27.000000 PyComplexHeatmap-1.4.3/setup.py
```

### Comparing `PyComplexHeatmap-1.4.2/LICENSE` & `PyComplexHeatmap-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.4.2/PKG-INFO` & `PyComplexHeatmap-1.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyComplexHeatmap
-Version: 1.4.2
+Version: 1.4.3
 Summary: A python package to plot complex heatmap
 Home-page: https://github.com/DingWB/PyComplexHeatmap
 Author: Wubin Ding
 Author-email: Wubin Ding <ding.wu.bin.gm@gmail.com>
 Project-URL: Homepage, https://github.com/DingWB/PyComplexHeatmap
 Project-URL: Bug Tracker, https://github.com/DingWB/PyComplexHeatmap/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `PyComplexHeatmap-1.4.2/PyComplexHeatmap/annotations.py` & `PyComplexHeatmap-1.4.3/PyComplexHeatmap/annotations.py`

 * *Files 0% similar despite different names*

```diff
@@ -234,14 +234,19 @@
                  majority=True, text_kws=None, height=None, legend=True,
                  legend_kws=None, **plot_kws):
         self.add_text = add_text
         self.majority = majority
         self.text_kws = text_kws if not text_kws is None else {}
         self.plot_kws = plot_kws
         # print(self.plot_kws)
+        legend_kws = legend_kws if not legend_kws is None else {}
+        if 'vmax' in plot_kws:
+            legend_kws.setdefault('vmax', plot_kws.get('vmax'))
+        if 'vmin' in plot_kws:
+            legend_kws.setdefault('vmin', plot_kws.get('vmin'))
         super().__init__(df=df, cmap=cmap, colors=colors,
                          height=height, legend=legend, legend_kws=legend_kws, **plot_kws)
 
     def _set_default_plot_kws(self, plot_kws):
         self.plot_kws = {} if plot_kws is None else plot_kws
         self.plot_kws.setdefault('zorder', 10)
         self.text_kws.setdefault('zorder', 16)
```

### Comparing `PyComplexHeatmap-1.4.2/PyComplexHeatmap/clustermap.py` & `PyComplexHeatmap-1.4.3/PyComplexHeatmap/clustermap.py`

 * *Files 0% similar despite different names*

```diff
@@ -999,19 +999,21 @@
             #index=self.dendrogram_row.dendrogram['ivl']).to_frame(name='cluster')
 
         elif isinstance(self.row_split, (pd.Series, pd.DataFrame)):
             if isinstance(self.row_split, pd.Series):
                 self.row_split = self.row_split.to_frame(name=self.row_split.name)
             cols = self.row_split.columns.tolist()
             row_clusters = self.row_split.groupby(cols).apply(lambda x: x.index.tolist())
-            if self.row_split_order is None:
+            if len(cols)==1 and self.row_split_order is None:
                 # calculate row_split_order using the mean across all samples in this group of
                 # values of mean values across all samples
                 self.row_split_order = row_clusters.apply(lambda x: self.data2d.loc[x].mean(axis=1).mean())\
                     .sort_values(ascending=False).index.tolist()
+            else:
+                self.row_split_order=row_clusters.sort_index().index.tolist()
             self.row_clusters = row_clusters.loc[self.row_split_order].to_dict()
         elif not self.row_cluster:
             self.row_order = [self.data2d.index.tolist()]
             return None
         else:
             raise TypeError("row_split must be integar or dataframe or series")
 
@@ -1046,19 +1048,21 @@
             #index=self.dendrogram_col.dendrogram['ivl']).to_frame(name='cluster')
 
         elif isinstance(self.col_split, (pd.Series, pd.DataFrame)):
             if isinstance(self.col_split, pd.Series):
                 self.col_split = self.col_split.to_frame(name=self.col_split.name)
             cols = self.col_split.columns.tolist()
             col_clusters = self.col_split.groupby(cols).apply(lambda x: x.index.tolist())
-            if self.col_split_order is None:
+            if len(cols)==1 and self.col_split_order is None:
                 # calculate col_split_order using the mean across all samples in this group of
                 # values of mean values across all samples
                 self.col_split_order = col_clusters.apply(lambda x: self.data2d.loc[:,x].mean().mean())\
                     .sort_values(ascending=False).index.tolist()
+            else:
+                self.col_split_order=col_clusters.sort_index().index.tolist()
             self.col_clusters = col_clusters.loc[self.col_split_order].to_dict()
         elif not self.col_cluster:
             self.col_order = [self.data2d.columns.tolist()]
             return None
         else:
             raise TypeError("row_split must be integar or dataframe or series")
```

### Comparing `PyComplexHeatmap-1.4.2/PyComplexHeatmap/colors.py` & `PyComplexHeatmap-1.4.3/PyComplexHeatmap/colors.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 # -*- coding: utf-8 -*-
 # !/usr/bin/env python3
 import matplotlib
 import matplotlib.pylab as plt
 from matplotlib.colors import LinearSegmentedColormap,ListedColormap,CSS4_COLORS
 import random
 from .utils import _calculate_luminance
-plt.rcParams['figure.dpi'] = 100
-plt.rcParams['savefig.dpi']=300
 
 def define_cmap():
     all_cmaps=matplotlib.pyplot.colormaps()
     if 'binarize' not in all_cmaps:
         c = LinearSegmentedColormap.from_list('binarize', [(0, 'lightgray'), (1, 'black')])
         plt.register_cmap(cmap=c)
     if 'exp1' not in all_cmaps:
```

### Comparing `PyComplexHeatmap-1.4.2/PyComplexHeatmap/dotHeatmap.py` & `PyComplexHeatmap-1.4.3/PyComplexHeatmap/dotHeatmap.py`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.4.2/PyComplexHeatmap/example.py` & `PyComplexHeatmap-1.4.3/PyComplexHeatmap/example.py`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.4.2/PyComplexHeatmap/oncoPrint.py` & `PyComplexHeatmap-1.4.3/PyComplexHeatmap/oncoPrint.py`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.4.2/PyComplexHeatmap/tools.py` & `PyComplexHeatmap-1.4.3/PyComplexHeatmap/tools.py`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.4.2/PyComplexHeatmap/utils.py` & `PyComplexHeatmap-1.4.3/PyComplexHeatmap/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,34 @@
 import matplotlib
 import matplotlib.pylab as plt
 from matplotlib.colors import LinearSegmentedColormap
 import matplotlib.lines as mlines
 import matplotlib.patches as mpatches
 mm2inch=1/25.4
 # =============================================================================
+def set_default_style():
+    from matplotlib import rcParams
+    D={
+        'font.family':['sans serif'], #'serif',
+        # 'mathtext.fontset':'dejavuserif',
+        'font.sans-serif':['Arial'],
+        'pdf.fonttype':42,
+
+        # Remove legend frame
+        'legend.frameon': True,
+
+        # Savefig
+        'figure.dpi': 100,
+        'savefig.bbox': 'tight',
+        'savefig.dpi':300,
+        'savefig.pad_inches': 0.05
+    }
+    
+    rcParams.update(D)
+# =============================================================================
 def _check_mask(data, mask):
     """
 
     Ensure that data and mask are compatible and add missing values and infinite values.
     Values will be plotted for cells where ``mask`` is ``False``.
     ``data`` is expected to be a DataFrame; ``mask`` can be an array or
     a DataFrame.
@@ -369,14 +389,15 @@
     Returns
     -------
     cbar: axes of legend
 
     """
     label='' if label is None else label
     cbar_kws={} if kws is None else kws.copy()
+    cbar_kws.setdefault('label',label)
     # cbar_kws.setdefault("aspect",3)
     cbar_kws.setdefault("orientation","vertical")
     # cbar_kws.setdefault("use_gridspec", True)
     # cbar_kws.setdefault("location", "bottom")
     cbar_kws.setdefault("fraction", 1)
     cbar_kws.setdefault("shrink", 1)
     cbar_kws.setdefault("pad", 0)
@@ -386,15 +407,15 @@
     cax.set_ylim([vmin,vmax])
     cbar_kws.setdefault("ticks",[vmin,(vmax+vmin)/2,vmax])
     m = plt.cm.ScalarMappable(
         norm=matplotlib.colors.Normalize(vmin=vmin, vmax=vmax),
         cmap=cmap)
     cax.yaxis.set_label_position(label_side)
     cax.yaxis.set_ticks_position(label_side)
-    cbar=ax.figure.colorbar(m,cax=cax,label=label,**cbar_kws) #use_gridspec=True
+    cbar=ax.figure.colorbar(m,cax=cax,**cbar_kws) #use_gridspec=True
     # cbar.outline.set_color('white')
     # cbar.outline.set_linewidth(2)
     # cbar.dividers.set_color('red')
     # cbar.dividers.set_linewidth(2)
     # ax.figure.tight_layout(rect=[cax.get_position().x0, 0, cax.get_position().x1, 1],h_pad=0,w_pad=0) #
     # cax.spines['top'].set_visible(False)
     # cax.spines['bottom'].set_visible(False)
@@ -629,8 +650,10 @@
         y = y - f - h_gap
         i+=1
     if legend_side=='right':
         boundry=ax1.get_position().y1+max_width / ax.figure.get_window_extent().width
     else:
         boundry = ax1.get_position().y0 - max_width / ax.figure.get_window_extent().width
     return legend_axes,cbars,boundry
-# =============================================================================
+# =============================================================================
+
+set_default_style()
```

### Comparing `PyComplexHeatmap-1.4.2/PyComplexHeatmap.egg-info/PKG-INFO` & `PyComplexHeatmap-1.4.3/PyComplexHeatmap.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyComplexHeatmap
-Version: 1.4.2
+Version: 1.4.3
 Summary: A python package to plot complex heatmap
 Home-page: https://github.com/DingWB/PyComplexHeatmap
 Author: Wubin Ding
 Author-email: Wubin Ding <ding.wu.bin.gm@gmail.com>
 Project-URL: Homepage, https://github.com/DingWB/PyComplexHeatmap
 Project-URL: Bug Tracker, https://github.com/DingWB/PyComplexHeatmap/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `PyComplexHeatmap-1.4.2/README.md` & `PyComplexHeatmap-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.4.2/pyproject.toml` & `PyComplexHeatmap-1.4.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0","matplotlib>=3.5.1","numpy>=1.20.3","pandas>=1.4.1", "scipy"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "PyComplexHeatmap"
-version = "1.4.2"
+version = "1.4.3"
 authors = [
   { name="Wubin Ding", email="ding.wu.bin.gm@gmail.com" },
 ]
 description = "A python package to plot complex heatmap"
 readme = "README.md"
 requires-python = ">=3.0"
 classifiers = [
```

### Comparing `PyComplexHeatmap-1.4.2/setup.py` & `PyComplexHeatmap-1.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 # print(long_description)
 
 #release new version
 setup(
    name='PyComplexHeatmap',
-   version='1.4.2',
+   version='1.4.3',
    description='A Python package to plot complex heatmap',
    # long_description="#PyComplexHeatmap\n##Documentation:https://dingwb.github.io/PyComplexHeatmap/build/html/index.html",
    # long_description_content_type='text/markdown',
    author='Wubin Ding',
    author_email='ding.wu.bin.gm@gmail.com',
    url="https://github.com/DingWB/PyComplexHeatmap",
    packages=['PyComplexHeatmap'], #src
```

