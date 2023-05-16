# Comparing `tmp/cnv_suite-0.1.1.tar.gz` & `tmp/cnv_suite-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cnv_suite-0.1.1.tar", last modified: Thu Feb  2 21:10:55 2023, max compression
+gzip compressed data, was "cnv_suite-0.1.2.tar", last modified: Tue May 16 03:35:23 2023, max compression
```

## Comparing `cnv_suite-0.1.1.tar` & `cnv_suite-0.1.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 cmesser    (502) staff       (20)        0 2023-02-02 21:10:55.352354 cnv_suite-0.1.1/
--rw-r--r--   0 cmesser    (502) staff       (20)     1523 2022-11-07 18:37:02.000000 cnv_suite-0.1.1/LICENSE
--rw-r--r--   0 cmesser    (502) staff       (20)     3584 2023-02-02 21:10:55.351986 cnv_suite-0.1.1/PKG-INFO
--rw-r--r--   0 cmesser    (502) staff       (20)     3063 2022-06-15 21:08:47.000000 cnv_suite-0.1.1/README.md
-drwxr-xr-x   0 cmesser    (502) staff       (20)        0 2023-02-02 21:10:55.337921 cnv_suite-0.1.1/cnv_suite/
--rw-r--r--   0 cmesser    (502) staff       (20)       21 2022-06-11 22:33:05.000000 cnv_suite-0.1.1/cnv_suite/__init__.py
-drwxr-xr-x   0 cmesser    (502) staff       (20)        0 2023-02-02 21:10:55.344901 cnv_suite-0.1.1/cnv_suite/compare/
--rw-r--r--   0 cmesser    (502) staff       (20)      204 2022-11-07 21:25:17.000000 cnv_suite-0.1.1/cnv_suite/compare/__init__.py
--rw-r--r--   0 cmesser    (502) staff       (20)     4867 2022-11-07 21:28:43.000000 cnv_suite-0.1.1/cnv_suite/compare/__main__.py
--rw-r--r--   0 cmesser    (502) staff       (20)    12325 2022-11-07 21:25:24.000000 cnv_suite-0.1.1/cnv_suite/compare/acr_compare.py
--rw-r--r--   0 cmesser    (502) staff       (20)    10386 2022-11-07 21:08:00.000000 cnv_suite-0.1.1/cnv_suite/compare/comparison_validation_tools.py
--rw-r--r--   0 cmesser    (502) staff       (20)     7882 2022-06-08 20:35:34.000000 cnv_suite-0.1.1/cnv_suite/compare/plot_acr.py
-drwxr-xr-x   0 cmesser    (502) staff       (20)        0 2023-02-02 21:10:55.346799 cnv_suite-0.1.1/cnv_suite/simulate/
--rw-r--r--   0 cmesser    (502) staff       (20)       37 2022-06-01 18:24:49.000000 cnv_suite-0.1.1/cnv_suite/simulate/__init__.py
--rw-r--r--   0 cmesser    (502) staff       (20)    38556 2022-11-07 19:22:45.000000 cnv_suite-0.1.1/cnv_suite/simulate/cnv_profile.py
-drwxr-xr-x   0 cmesser    (502) staff       (20)        0 2023-02-02 21:10:55.349725 cnv_suite-0.1.1/cnv_suite/utils/
--rw-r--r--   0 cmesser    (502) staff       (20)      208 2022-06-11 22:44:13.000000 cnv_suite-0.1.1/cnv_suite/utils/__init__.py
--rw-r--r--   0 cmesser    (502) staff       (20)     9537 2022-08-26 13:30:19.000000 cnv_suite-0.1.1/cnv_suite/utils/cnv_helper_methods.py
--rw-r--r--   0 cmesser    (502) staff       (20)     4028 2022-09-28 21:32:11.000000 cnv_suite-0.1.1/cnv_suite/utils/simulation_utils.py
-drwxr-xr-x   0 cmesser    (502) staff       (20)        0 2023-02-02 21:10:55.351040 cnv_suite-0.1.1/cnv_suite/visualize/
--rw-r--r--   0 cmesser    (502) staff       (20)       32 2022-06-01 18:24:49.000000 cnv_suite-0.1.1/cnv_suite/visualize/__init__.py
--rw-r--r--   0 cmesser    (502) staff       (20)    26522 2023-02-02 21:08:47.000000 cnv_suite-0.1.1/cnv_suite/visualize/plot_cnv_profile.py
-drwxr-xr-x   0 cmesser    (502) staff       (20)        0 2023-02-02 21:10:55.340911 cnv_suite-0.1.1/cnv_suite.egg-info/
--rw-r--r--   0 cmesser    (502) staff       (20)     3584 2023-02-02 21:10:54.000000 cnv_suite-0.1.1/cnv_suite.egg-info/PKG-INFO
--rw-r--r--   0 cmesser    (502) staff       (20)      659 2023-02-02 21:10:55.000000 cnv_suite-0.1.1/cnv_suite.egg-info/SOURCES.txt
--rw-r--r--   0 cmesser    (502) staff       (20)        1 2023-02-02 21:10:54.000000 cnv_suite-0.1.1/cnv_suite.egg-info/dependency_links.txt
--rw-r--r--   0 cmesser    (502) staff       (20)      161 2023-02-02 21:10:55.000000 cnv_suite-0.1.1/cnv_suite.egg-info/entry_points.txt
--rw-r--r--   0 cmesser    (502) staff       (20)      208 2023-02-02 21:10:55.000000 cnv_suite-0.1.1/cnv_suite.egg-info/requires.txt
--rw-r--r--   0 cmesser    (502) staff       (20)       10 2023-02-02 21:10:55.000000 cnv_suite-0.1.1/cnv_suite.egg-info/top_level.txt
--rw-r--r--   0 cmesser    (502) staff       (20)       38 2023-02-02 21:10:55.352454 cnv_suite-0.1.1/setup.cfg
--rw-r--r--   0 cmesser    (502) staff       (20)     1668 2023-02-02 21:10:05.000000 cnv_suite-0.1.1/setup.py
+drwxr-xr-x   0 cmesser    (502) staff       (20)        0 2023-05-16 03:35:23.664062 cnv_suite-0.1.2/
+-rw-r--r--   0 cmesser    (502) staff       (20)     1523 2022-11-07 18:37:02.000000 cnv_suite-0.1.2/LICENSE
+-rw-r--r--   0 cmesser    (502) staff       (20)     3584 2023-05-16 03:35:23.663780 cnv_suite-0.1.2/PKG-INFO
+-rw-r--r--   0 cmesser    (502) staff       (20)     3063 2022-06-15 21:08:47.000000 cnv_suite-0.1.2/README.md
+drwxr-xr-x   0 cmesser    (502) staff       (20)        0 2023-05-16 03:35:23.650603 cnv_suite-0.1.2/cnv_suite/
+-rw-r--r--   0 cmesser    (502) staff       (20)       21 2022-06-11 22:33:05.000000 cnv_suite-0.1.2/cnv_suite/__init__.py
+drwxr-xr-x   0 cmesser    (502) staff       (20)        0 2023-05-16 03:35:23.656883 cnv_suite-0.1.2/cnv_suite/compare/
+-rw-r--r--   0 cmesser    (502) staff       (20)      204 2022-11-07 21:25:17.000000 cnv_suite-0.1.2/cnv_suite/compare/__init__.py
+-rw-r--r--   0 cmesser    (502) staff       (20)     4867 2022-11-07 21:28:43.000000 cnv_suite-0.1.2/cnv_suite/compare/__main__.py
+-rw-r--r--   0 cmesser    (502) staff       (20)    12325 2022-11-07 21:25:24.000000 cnv_suite-0.1.2/cnv_suite/compare/acr_compare.py
+-rw-r--r--   0 cmesser    (502) staff       (20)    10386 2022-11-07 21:08:00.000000 cnv_suite-0.1.2/cnv_suite/compare/comparison_validation_tools.py
+-rw-r--r--   0 cmesser    (502) staff       (20)     7882 2022-06-08 20:35:34.000000 cnv_suite-0.1.2/cnv_suite/compare/plot_acr.py
+drwxr-xr-x   0 cmesser    (502) staff       (20)        0 2023-05-16 03:35:23.658263 cnv_suite-0.1.2/cnv_suite/simulate/
+-rw-r--r--   0 cmesser    (502) staff       (20)       37 2022-06-01 18:24:49.000000 cnv_suite-0.1.2/cnv_suite/simulate/__init__.py
+-rw-r--r--   0 cmesser    (502) staff       (20)    38556 2022-11-07 19:22:45.000000 cnv_suite-0.1.2/cnv_suite/simulate/cnv_profile.py
+drwxr-xr-x   0 cmesser    (502) staff       (20)        0 2023-05-16 03:35:23.661366 cnv_suite-0.1.2/cnv_suite/utils/
+-rw-r--r--   0 cmesser    (502) staff       (20)      208 2022-06-11 22:44:13.000000 cnv_suite-0.1.2/cnv_suite/utils/__init__.py
+-rw-r--r--   0 cmesser    (502) staff       (20)     9537 2022-08-26 13:30:19.000000 cnv_suite-0.1.2/cnv_suite/utils/cnv_helper_methods.py
+-rw-r--r--   0 cmesser    (502) staff       (20)     4028 2022-09-28 21:32:11.000000 cnv_suite-0.1.2/cnv_suite/utils/simulation_utils.py
+drwxr-xr-x   0 cmesser    (502) staff       (20)        0 2023-05-16 03:35:23.662696 cnv_suite-0.1.2/cnv_suite/visualize/
+-rw-r--r--   0 cmesser    (502) staff       (20)       32 2022-06-01 18:24:49.000000 cnv_suite-0.1.2/cnv_suite/visualize/__init__.py
+-rw-r--r--   0 cmesser    (502) staff       (20)    26584 2023-05-16 03:31:48.000000 cnv_suite-0.1.2/cnv_suite/visualize/plot_cnv_profile.py
+drwxr-xr-x   0 cmesser    (502) staff       (20)        0 2023-05-16 03:35:23.653432 cnv_suite-0.1.2/cnv_suite.egg-info/
+-rw-r--r--   0 cmesser    (502) staff       (20)     3584 2023-05-16 03:35:23.000000 cnv_suite-0.1.2/cnv_suite.egg-info/PKG-INFO
+-rw-r--r--   0 cmesser    (502) staff       (20)      659 2023-05-16 03:35:23.000000 cnv_suite-0.1.2/cnv_suite.egg-info/SOURCES.txt
+-rw-r--r--   0 cmesser    (502) staff       (20)        1 2023-05-16 03:35:23.000000 cnv_suite-0.1.2/cnv_suite.egg-info/dependency_links.txt
+-rw-r--r--   0 cmesser    (502) staff       (20)      161 2023-05-16 03:35:23.000000 cnv_suite-0.1.2/cnv_suite.egg-info/entry_points.txt
+-rw-r--r--   0 cmesser    (502) staff       (20)      208 2023-05-16 03:35:23.000000 cnv_suite-0.1.2/cnv_suite.egg-info/requires.txt
+-rw-r--r--   0 cmesser    (502) staff       (20)       10 2023-05-16 03:35:23.000000 cnv_suite-0.1.2/cnv_suite.egg-info/top_level.txt
+-rw-r--r--   0 cmesser    (502) staff       (20)       38 2023-05-16 03:35:23.664165 cnv_suite-0.1.2/setup.cfg
+-rw-r--r--   0 cmesser    (502) staff       (20)     1669 2023-05-16 03:34:09.000000 cnv_suite-0.1.2/setup.py
```

### Comparing `cnv_suite-0.1.1/LICENSE` & `cnv_suite-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cnv_suite-0.1.1/PKG-INFO` & `cnv_suite-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnv_suite
-Version: 0.1.1
+Version: 0.1.2
 Summary: Copy Number tools for visualization, simulation, and comparison.
 Author: Conor Messer
 Author-email: cmesser@broadinstitute.org
 License: BSD3
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Science/Research
```

### Comparing `cnv_suite-0.1.1/README.md` & `cnv_suite-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `cnv_suite-0.1.1/cnv_suite/compare/__main__.py` & `cnv_suite-0.1.2/cnv_suite/compare/__main__.py`

 * *Files identical despite different names*

### Comparing `cnv_suite-0.1.1/cnv_suite/compare/acr_compare.py` & `cnv_suite-0.1.2/cnv_suite/compare/acr_compare.py`

 * *Files identical despite different names*

### Comparing `cnv_suite-0.1.1/cnv_suite/compare/comparison_validation_tools.py` & `cnv_suite-0.1.2/cnv_suite/compare/comparison_validation_tools.py`

 * *Files identical despite different names*

### Comparing `cnv_suite-0.1.1/cnv_suite/compare/plot_acr.py` & `cnv_suite-0.1.2/cnv_suite/compare/plot_acr.py`

 * *Files identical despite different names*

### Comparing `cnv_suite-0.1.1/cnv_suite/simulate/cnv_profile.py` & `cnv_suite-0.1.2/cnv_suite/simulate/cnv_profile.py`

 * *Files identical despite different names*

### Comparing `cnv_suite-0.1.1/cnv_suite/utils/cnv_helper_methods.py` & `cnv_suite-0.1.2/cnv_suite/utils/cnv_helper_methods.py`

 * *Files identical despite different names*

### Comparing `cnv_suite-0.1.1/cnv_suite/utils/simulation_utils.py` & `cnv_suite-0.1.2/cnv_suite/utils/simulation_utils.py`

 * *Files identical despite different names*

### Comparing `cnv_suite-0.1.1/cnv_suite/visualize/plot_cnv_profile.py` & `cnv_suite-0.1.2/cnv_suite/visualize/plot_cnv_profile.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,17 +101,16 @@
     :param title: Title of plot
     :param fig_names: Title for each subplot (one for each row)
     """
     fig = plotly.subplots.make_subplots(rows=len(fig_list), cols=1,
                                         shared_xaxes=True, subplot_titles=fig_names,
                                         vertical_spacing=0.15/len(fig_list), **kwargs)
 
-    for i in range(len(fig_list)):
-        for t in fig_list[i].data:
-            fig.add_trace(t, row=i+1, col=1)
+    for i, sub_figure in enumerate(fig_list):
+        fig.add_traces(sub_figure.data, rows=i + 1, cols=1)
         fig.update_yaxes(fig_list[i].layout.yaxis, row=i+1, col=1)
 
     # Add chromosome background back in
     add_background(fig, csize.keys(), csize)
 
     # update height based on subplot number
     fig.update_layout(height=len(fig_list)*height_per_sample + 50,
@@ -353,19 +352,19 @@
     chrom_ticks = []
     patch_color = 'white'
 
     is_plotly_figure = isinstance(ax, go.Figure) and not ((plotly_row is None) or (plotly_col is None))
     for chrom in chr_order:
         if type(ax) == go.Figure:
             if is_plotly_figure:
-                ax.add_vrect(base_start, base_start + csize[chrom], fillcolor=patch_color,
-                             opacity=0.1, layer='below', line_width=0, row=plotly_row, col=plotly_col)
+                ax.add_shape(x0=base_start, x1=base_start + csize[chrom], y0=0, y1=1, fillcolor=patch_color,
+                             opacity=0.1, layer='below', line_width=0, yref= 'y domain', row=plotly_row, col=plotly_col)
             else:
-                ax.add_vrect(base_start, base_start + csize[chrom], fillcolor=patch_color,
-                              opacity=0.1, layer='below', line_width=0)
+                ax.add_shape(x0=base_start, x1=base_start + csize[chrom], y0=0, y1=1, fillcolor=patch_color,
+                             opacity=0.1, layer='below', line_width=0, yref= 'y domain')
         else:
             p = patches.Rectangle((base_start, -0.2), csize[chrom], height, fill=True, facecolor=patch_color,
                                   edgecolor=None, alpha=.1)  # Background
 
             if is_plotly_figure:
                 ax.add_patch(p, row=plotly_row, col=plotly_col)
             else:
```

### Comparing `cnv_suite-0.1.1/cnv_suite.egg-info/PKG-INFO` & `cnv_suite-0.1.2/cnv_suite.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnv-suite
-Version: 0.1.1
+Version: 0.1.2
 Summary: Copy Number tools for visualization, simulation, and comparison.
 Author: Conor Messer
 Author-email: cmesser@broadinstitute.org
 License: BSD3
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Science/Research
```

### Comparing `cnv_suite-0.1.1/cnv_suite.egg-info/SOURCES.txt` & `cnv_suite-0.1.2/cnv_suite.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cnv_suite-0.1.1/setup.py` & `cnv_suite-0.1.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='cnv_suite',
-    version="0.1.1",
+    version="0.1.2",
     packages=['cnv_suite.compare', 'cnv_suite.simulate', 'cnv_suite.utils', 'cnv_suite.visualize', 'cnv_suite'],
     entry_points={
         'console_scripts': [
             'simulate = cnv_suite.simulate.cnv_profile:main',
             'visualize = cnv_suite.visualize.plot_cnv_profile:main',
             'compare = cnv_suite.compare.__main__:main'
         ]
@@ -43,8 +43,8 @@
         "Development Status :: 4 - Beta",
         "Programming Language :: Python :: 3",
         "Intended Audience :: Science/Research",
         "Topic :: Scientific/Engineering :: Bio-Informatics",
         "License :: OSI Approved :: BSD License"
     ],
     license="BSD3"
-)
+)
```

