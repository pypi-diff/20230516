# Comparing `tmp/autoviz-0.1.603.tar.gz` & `tmp/autoviz-0.1.604.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoviz-0.1.603.tar", last modified: Fri May  5 14:02:25 2023, max compression
+gzip compressed data, was "autoviz-0.1.604.tar", last modified: Tue May 16 02:23:38 2023, max compression
```

## Comparing `autoviz-0.1.603.tar` & `autoviz-0.1.604.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2023-05-05 14:02:25.967815 autoviz-0.1.603/
--rwxrwxrwx   0 ram       (1000) ram       (1000)    15853 2023-05-05 14:02:25.963811 autoviz-0.1.603/PKG-INFO
--rwxrwxrwx   0 ram       (1000) ram       (1000)    13747 2023-05-05 13:59:34.000000 autoviz-0.1.603/README.md
-drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2023-05-05 14:02:25.823558 autoviz-0.1.603/autoviz/
--rwxrwxrwx   0 ram       (1000) ram       (1000)    30554 2023-04-18 12:33:51.000000 autoviz-0.1.603/autoviz/AutoViz_Class.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)    61007 2022-10-02 14:52:48.000000 autoviz-0.1.603/autoviz/AutoViz_Holo.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)    24022 2022-10-02 14:52:48.000000 autoviz-0.1.603/autoviz/AutoViz_NLP.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)   118079 2023-05-05 13:05:30.000000 autoviz-0.1.603/autoviz/AutoViz_Utils.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)     1323 2022-10-02 14:52:48.000000 autoviz-0.1.603/autoviz/__init__.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)      404 2023-05-05 12:31:56.000000 autoviz-0.1.603/autoviz/__version__.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)    24678 2023-04-18 12:53:31.000000 autoviz-0.1.603/autoviz/classify_method.py
-drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2023-05-05 14:02:25.941772 autoviz-0.1.603/autoviz.egg-info/
--rwxrwxrwx   0 ram       (1000) ram       (1000)    15853 2023-05-05 14:02:25.000000 autoviz-0.1.603/autoviz.egg-info/PKG-INFO
--rwxrwxrwx   0 ram       (1000) ram       (1000)      339 2023-05-05 14:02:25.000000 autoviz-0.1.603/autoviz.egg-info/SOURCES.txt
--rwxrwxrwx   0 ram       (1000) ram       (1000)        1 2023-05-05 14:02:25.000000 autoviz-0.1.603/autoviz.egg-info/dependency_links.txt
--rwxrwxrwx   0 ram       (1000) ram       (1000)      241 2023-05-05 14:02:25.000000 autoviz-0.1.603/autoviz.egg-info/requires.txt
--rwxrwxrwx   0 ram       (1000) ram       (1000)        8 2023-05-05 14:02:25.000000 autoviz-0.1.603/autoviz.egg-info/top_level.txt
--rwxrwxrwx   0 ram       (1000) ram       (1000)       38 2023-05-05 14:02:25.971820 autoviz-0.1.603/setup.cfg
--rwxrwxrwx   0 ram       (1000) ram       (1000)     1205 2023-05-05 13:06:48.000000 autoviz-0.1.603/setup.py
+drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2023-05-16 02:23:38.401423 autoviz-0.1.604/
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    15955 2023-05-16 02:23:38.397415 autoviz-0.1.604/PKG-INFO
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    13856 2023-05-16 02:10:32.000000 autoviz-0.1.604/README.md
+drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2023-05-16 02:23:38.273420 autoviz-0.1.604/autoviz/
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    30562 2023-05-16 01:58:53.000000 autoviz-0.1.604/autoviz/AutoViz_Class.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    60800 2023-05-15 13:55:02.000000 autoviz-0.1.604/autoviz/AutoViz_Holo.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    24022 2022-10-02 14:52:48.000000 autoviz-0.1.604/autoviz/AutoViz_NLP.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)   117958 2023-05-15 13:41:29.000000 autoviz-0.1.604/autoviz/AutoViz_Utils.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)     1323 2022-10-02 14:52:48.000000 autoviz-0.1.604/autoviz/__init__.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)      404 2023-05-16 02:18:27.000000 autoviz-0.1.604/autoviz/__version__.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    24678 2023-04-18 12:53:31.000000 autoviz-0.1.604/autoviz/classify_method.py
+drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2023-05-16 02:23:38.373421 autoviz-0.1.604/autoviz.egg-info/
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    15955 2023-05-16 02:23:37.000000 autoviz-0.1.604/autoviz.egg-info/PKG-INFO
+-rwxrwxrwx   0 ram       (1000) ram       (1000)      339 2023-05-16 02:23:37.000000 autoviz-0.1.604/autoviz.egg-info/SOURCES.txt
+-rwxrwxrwx   0 ram       (1000) ram       (1000)        1 2023-05-16 02:23:37.000000 autoviz-0.1.604/autoviz.egg-info/dependency_links.txt
+-rwxrwxrwx   0 ram       (1000) ram       (1000)      241 2023-05-16 02:23:37.000000 autoviz-0.1.604/autoviz.egg-info/requires.txt
+-rwxrwxrwx   0 ram       (1000) ram       (1000)        8 2023-05-16 02:23:37.000000 autoviz-0.1.604/autoviz.egg-info/top_level.txt
+-rwxrwxrwx   0 ram       (1000) ram       (1000)       38 2023-05-16 02:23:38.405478 autoviz-0.1.604/setup.cfg
+-rwxrwxrwx   0 ram       (1000) ram       (1000)     1205 2023-05-16 02:18:40.000000 autoviz-0.1.604/setup.py
```

### Comparing `autoviz-0.1.603/PKG-INFO` & `autoviz-0.1.604/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoviz
-Version: 0.1.603
+Version: 0.1.604
 Summary: Automatically Visualize any dataset, any size with a single line of code
 Home-page: https://github.com/AutoViML/AutoViz
 Author: Ram Seshadri
 License: Apache License 2.0
 Description: # AutoViz: The One-Line Automatic Data Visualization Library
         
         ![logo](logo.png)
@@ -74,23 +74,22 @@
         ```
         from autoviz import AutoViz_Class
         AV = AutoViz_Class()
         dft = AV.AutoViz(filename)
         ```
         
         Feed AutoViz any input filename (in CSV, txt, or JSON format), and set `max_rows_analyzed` and `max_cols_analyzed` based on memory limitations in your environment, and watch the magic happen!
-        <p>AutoViz generates charts in multiple formats using the `chart_format` setting which can one of the following:
-        - `'png'`, `'svg'`, or `'jpg'`: Inline Matplotlib charts
-            * Save locally (`verbose=2`) or display in Jupyter Notebooks (`verbose=1`)
-            * Default AutoViz behavior
-        - `'bokeh'`: Interactive Bokeh charts in Jupyter Notebooks
-        - `'server'`: Browser-based dashboards with individual chart types
-        - `'html'`: Interactive Bokeh charts saved as HTML files under the `AutoViz_Plots` directory (working folder) or specified directory using the `save_plot_dir` setting
         
-        AutoViz takes care of the rest. You'll see charts and plots on your screen.
+        AutoViz can now create charts in multiple  formats using the `chart_format` setting:
+        - If `chart_format ='png'` or `'svg'` or `'jpg'`: Matplotlib charts are plotted inline.
+            * Can be saved locally (using `verbose=2` setting) or displayed (`verbose=1`) in Jupyter Notebooks.
+            * This is the default behavior for AutoViz.
+        - If `chart_format='bokeh'`: Interactive Bokeh charts are plotted in Jupyter Notebooks.
+        - If `chart_format='server'`, dashboards will pop up for each kind of chart on your browser.
+        - If `chart_format='html'`, interactive Bokeh charts will be created and silently saved as HTML files under the `AutoViz_Plots` directory (under working folder) or any other directory that you specify using the `save_plot_dir` setting (during input).
         
         ![var_charts](var_charts.JPG)
         
         AV.AutoViz is the main plotting function in AutoViz_Class (AV). Depending on the chart_format you choose, AutoViz will automatically call either the AutoViz_Main function or AutoViz_Holo function.
         
         # API
         Arguments for AV.AutoViz() method:
@@ -235,15 +234,15 @@
         
         # License
         AutoViz is released under the Apache License, Version 2.0. By using AutoViz, you agree to the terms and conditions specified in the license.
         
         # Tips
         <p>That covers the main aspects of AutoViz, but here are some additional tips and reminders to help you make the most of the library:</p>
         <ul>
-          <li>Make sure to regularly upgrade AutoViz to benefit from the <a href="https://github.com/AutoViML/AutoViz/blob/main/updates.md">latest features, bug fixes, and improvements</a>. You can update it using <code>pip install --upgrade autoviz</code>.</li>
+          <li>Make sure to regularly upgrade AutoViz to benefit from the <a href="https://github.com/AutoViML/AutoViz/blob/master/updates.md">latest features, bug fixes, and improvements</a>. You can update it using <code>pip install --upgrade autoviz</code>.</li>
           <li>AutoViz is highly customizable, so don't hesitate to explore and experiment with various settings, such as <code>chart_format</code>, <code>verbose</code>, and <code>max_rows_analyzed</code>. This will allow you to create visualizations that better suit your specific needs and preferences.</li>
           <li>Remember to delete the <code>AutoViz_Plots</code> directory (or any custom directory you specified) periodically if you used the <code>verbose=2</code> option, as it can accumulate a large number of saved charts over time.</li>
           <li>For further guidance or inspiration, check out the <a href="https://towardsdatascience.com/autoviz-a-new-tool-for-automated-visualization-ec9c1744a6ad">Medium article on AutoViz</a>, as well as other online resources and tutorials.</li>
           <li>If you encounter any issues, have questions, or want to suggest improvements, don't hesitate to engage with the AutoViz community through the <a href="https://github.com/AutoViML/AutoViz">GitHub repository</a> or other online platforms.</li>
         </ul>
         <p>By leveraging AutoViz's powerful and flexible features, you can streamline your data visualization process and gain valuable insights more efficiently. Happy visualizing!</p>
```

### Comparing `autoviz-0.1.603/README.md` & `autoviz-0.1.604/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -67,23 +67,22 @@
 ```
 from autoviz import AutoViz_Class
 AV = AutoViz_Class()
 dft = AV.AutoViz(filename)
 ```
 
 Feed AutoViz any input filename (in CSV, txt, or JSON format), and set `max_rows_analyzed` and `max_cols_analyzed` based on memory limitations in your environment, and watch the magic happen!
-<p>AutoViz generates charts in multiple formats using the `chart_format` setting which can one of the following:
-- `'png'`, `'svg'`, or `'jpg'`: Inline Matplotlib charts
-    * Save locally (`verbose=2`) or display in Jupyter Notebooks (`verbose=1`)
-    * Default AutoViz behavior
-- `'bokeh'`: Interactive Bokeh charts in Jupyter Notebooks
-- `'server'`: Browser-based dashboards with individual chart types
-- `'html'`: Interactive Bokeh charts saved as HTML files under the `AutoViz_Plots` directory (working folder) or specified directory using the `save_plot_dir` setting
 
-AutoViz takes care of the rest. You'll see charts and plots on your screen.
+AutoViz can now create charts in multiple  formats using the `chart_format` setting:
+- If `chart_format ='png'` or `'svg'` or `'jpg'`: Matplotlib charts are plotted inline.
+    * Can be saved locally (using `verbose=2` setting) or displayed (`verbose=1`) in Jupyter Notebooks.
+    * This is the default behavior for AutoViz.
+- If `chart_format='bokeh'`: Interactive Bokeh charts are plotted in Jupyter Notebooks.
+- If `chart_format='server'`, dashboards will pop up for each kind of chart on your browser.
+- If `chart_format='html'`, interactive Bokeh charts will be created and silently saved as HTML files under the `AutoViz_Plots` directory (under working folder) or any other directory that you specify using the `save_plot_dir` setting (during input).
 
 ![var_charts](var_charts.JPG)
 
 AV.AutoViz is the main plotting function in AutoViz_Class (AV). Depending on the chart_format you choose, AutoViz will automatically call either the AutoViz_Main function or AutoViz_Holo function.
 
 # API
 Arguments for AV.AutoViz() method:
@@ -228,15 +227,15 @@
 
 # License
 AutoViz is released under the Apache License, Version 2.0. By using AutoViz, you agree to the terms and conditions specified in the license.
 
 # Tips
 <p>That covers the main aspects of AutoViz, but here are some additional tips and reminders to help you make the most of the library:</p>
 <ul>
-  <li>Make sure to regularly upgrade AutoViz to benefit from the <a href="https://github.com/AutoViML/AutoViz/blob/main/updates.md">latest features, bug fixes, and improvements</a>. You can update it using <code>pip install --upgrade autoviz</code>.</li>
+  <li>Make sure to regularly upgrade AutoViz to benefit from the <a href="https://github.com/AutoViML/AutoViz/blob/master/updates.md">latest features, bug fixes, and improvements</a>. You can update it using <code>pip install --upgrade autoviz</code>.</li>
   <li>AutoViz is highly customizable, so don't hesitate to explore and experiment with various settings, such as <code>chart_format</code>, <code>verbose</code>, and <code>max_rows_analyzed</code>. This will allow you to create visualizations that better suit your specific needs and preferences.</li>
   <li>Remember to delete the <code>AutoViz_Plots</code> directory (or any custom directory you specified) periodically if you used the <code>verbose=2</code> option, as it can accumulate a large number of saved charts over time.</li>
   <li>For further guidance or inspiration, check out the <a href="https://towardsdatascience.com/autoviz-a-new-tool-for-automated-visualization-ec9c1744a6ad">Medium article on AutoViz</a>, as well as other online resources and tutorials.</li>
   <li>If you encounter any issues, have questions, or want to suggest improvements, don't hesitate to engage with the AutoViz community through the <a href="https://github.com/AutoViML/AutoViz">GitHub repository</a> or other online platforms.</li>
 </ul>
 <p>By leveraging AutoViz's powerful and flexible features, you can streamline your data visualization process and gain valuable insights more efficiently. Happy visualizing!</p>
```

### Comparing `autoviz-0.1.603/autoviz/AutoViz_Class.py` & `autoviz-0.1.604/autoviz/AutoViz_Class.py`

 * *Files 0% similar despite different names*

```diff
@@ -260,15 +260,15 @@
         ####  If verbose=2, it will print messages but will not display charts,  #####
         ####  it will simply save them.                                          #####
         ##############################################################################
         """
         if isinstance(depVar, list):
             print('Since AutoViz cannot visualize multi-label targets, choosing first item in targets: %s' %depVar[0])
             depVar = depVar[0]
-
+        
         ####################################################################################
         if chart_format.lower() in ['bokeh','server','bokeh_server','bokeh-server', 'html']:
             dft = AutoViz_Holo(filename, sep, depVar, dfte, header, verbose,
                         lowess,chart_format,max_rows_analyzed,
                             max_cols_analyzed, save_plot_dir)
         else:
             dft = self.AutoViz_Main(filename, sep, depVar, dfte, header, verbose,
@@ -280,15 +280,15 @@
                             lowess=False,chart_format='svg',max_rows_analyzed=150000,
                                 max_cols_analyzed=30, save_plot_dir=None):
         """
         ##############################################################################
         ##### AUTOVIZ_MAIN PERFORMS AUTO VISUALIZATION OF ANY DATA USING MATPLOTLIB ##
         ##############################################################################
         """
-        corr_limit = 0.7  ### This is needed to remove variables correlated above this limit
+        corr_limit = 0.8  ### This is needed to remove variables correlated above this limit
         ######### create a directory to save all plots generated by autoviz ############
         ############    THis is where you save the figures in a target directory #######
         
         if not depVar is None:
             if isinstance(depVar, list):
                 target_dir = depVar[0]
             elif isinstance(depVar, str):
```

### Comparing `autoviz-0.1.603/autoviz/AutoViz_Holo.py` & `autoviz-0.1.604/autoviz/AutoViz_Holo.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,14 +159,15 @@
         print('Not able to read or load file. Please check your inputs and try again...')
         return None
     #################   This is where the differentiated HoloViews code begins ####
     ls_objects = []
     imgdata_list = list()
     height_size = 400
     width_size = 500
+    
     ##########    Now start drawing the Bokeh Plots ###############################
     if len(nums) > 0:
         if problem_type == 'Clustering':
             #### There is no need to do a scatter plot with a dep variable when no dependent variable is given
             print('No scatter plots with depVar when no depVar is given.')
         else:
             drawobj1 = draw_scatters_hv(dfin,nums,chart_format,problem_type,
@@ -276,48 +277,49 @@
 #####################################################################################################
 def draw_kdeplot_hv(dfin, cats, nums, chart_format, problem_type, dep, ls_objects, mk_dir, verbose=0):
     dft = copy.deepcopy(dfin)
     image_count = 0
     imgdata_list = list()
     N = len(nums)
     cols = 2
+    plot_name = 'kde_plots'
     width_size = 600
     height_size = 400
-    plot_name = 'kde_plots'
     ########################################################################################
+    def return_dynamic_objects(dfout, dep, title='Distribution of Target variable'):
+        width_size = 600
+        height_size = 400
+        pdf1 = pd.DataFrame(dfout[dep].value_counts().reset_index())
+        pdf2 = pd.DataFrame(dfout[dep].value_counts(1).reset_index())
+        drawobj41 = pdf1.hvplot(kind='bar', color='lightblue', title=title).opts(
+                        height=height_size, width=width_size,xrotation=70)
+        drawobj42 = pdf2.hvplot(kind='bar', color='lightgreen', title=title)
+        return (drawobj41+drawobj42)
+
     if problem_type.endswith('Classification'):
         colors = cycle('brycgkbyrcmgkbyrcmgkbyrcmgkbyr')
-        pdf1 = pd.DataFrame(dfin[dep].value_counts().reset_index())
-        pdf2 = pd.DataFrame(dfin[dep].value_counts(1).reset_index())
-        drawobj41 = pdf1.hvplot(kind='bar', color='r', title='Distribution of Target variable').opts(
-                        height=height_size, width=width_size,xrotation=70)
-        drawobj42 = pdf2.hvplot(kind='bar', color='g', title='Percent Distribution of Target variable').opts(
-                        )
-        dmap = hv.DynamicMap((drawobj41+drawobj42).opts(shared_axes=False).opts(title='Histogram and KDE of Target = %s' %dep)).opts(
+        dmap = hv.DynamicMap(return_dynamic_objects(dfin, dep, title='Percent Distribution of Target variable'
+                        ).opts(shared_axes=False).opts(title='Histogram and KDE of Target = %s' %dep)).opts(
                             height=height_size, width=width_size)
         dmap.opts(framewise=True,axiswise=True) ## both must be True for your charts to have dynamically varying axes!
         hv_all = pn.pane.HoloViews(dmap)#, sizing_mode="stretch_both")
-        ls_objects.append(drawobj41)
-        ls_objects.append(drawobj42)
+        #ls_objects.append(drawobj41)
+        #ls_objects.append(drawobj42)
     else:
         if not isinstance(dep, list):
             ### it means dep is a string ###
             if dep == '':
                 ### there is no target variable to draw ######
                 return ls_objects
             else:
-                drawobj41 = dfin[dep].hvplot(kind='bar', color='r', title='Histogram of Target variable').opts(
-                                height=height_size,width=width_size,color='lightgreen', xrotation=70)
-                drawobj42 = dfin[dep].hvplot(kind='kde', color='g', title='KDE Plot of Target variable').opts(
-                                height=height_size,width=width_size,color='lightblue')
-                dmap = hv.DynamicMap((drawobj41+drawobj42)).opts(title='Histogram and KDE of Target = %s' %dep, width=width_size)
+                dmap = hv.DynamicMap(return_dynamic_objects(dfin, dep, title=f'Histogram and KDE of Target = {dep}')).opts(width=width_size)
                 dmap.opts(framewise=True,axiswise=True) ## both must be True for your charts to have dynamically varying axes!
                 hv_all = pn.pane.HoloViews(dmap)
-                ls_objects.append(drawobj41)
-                ls_objects.append(drawobj42)
+                #ls_objects.append(drawobj41)
+                #ls_objects.append(drawobj42)
     #### In this case we are using multiple objects in panel ###
     ##### Save all the chart objects here ##############
     if verbose == 2:
         imgdata_list = append_panels(hv_all, imgdata_list, chart_format)
         image_count += 1
     if chart_format.lower() in ['server', 'bokeh_server', 'bokeh-server']:
         ### If you want it on a server, you use drawobj.show()
```

### Comparing `autoviz-0.1.603/autoviz/AutoViz_NLP.py` & `autoviz-0.1.604/autoviz/AutoViz_NLP.py`

 * *Files identical despite different names*

### Comparing `autoviz-0.1.603/autoviz/AutoViz_Utils.py` & `autoviz-0.1.604/autoviz/AutoViz_Utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -682,16 +682,14 @@
         dft = dft[:]
         try:
             dft.index = pd.to_datetime(dft.pop(datevars[0]),infer_datetime_format=True)
             timeseries_flag = True
         except:
             if verbose >= 1 and len(datevars) > 0:
                 print('No date vars could be found or %s could not be indexed.' %datevars)
-            elif verbose >= 1 and len(datevars) == 0:
-                print('No date vars could be found in data set')
             timeseries_flag = False
     # Add a column: the color depends on target variable but you can use whatever function
     imgdata_list = list()
     if modeltype.endswith('Classification'):
         ########## This is for Classification problems only ###########
         if dft[dep].dtype == object or dft[dep].dtype == np.int64:
             dft[dep] = dft[dep].factorize()[0]
```

### Comparing `autoviz-0.1.603/autoviz/__init__.py` & `autoviz-0.1.604/autoviz/__init__.py`

 * *Files identical despite different names*

### Comparing `autoviz-0.1.603/autoviz/classify_method.py` & `autoviz-0.1.604/autoviz/classify_method.py`

 * *Files identical despite different names*

### Comparing `autoviz-0.1.603/autoviz.egg-info/PKG-INFO` & `autoviz-0.1.604/autoviz.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoviz
-Version: 0.1.603
+Version: 0.1.604
 Summary: Automatically Visualize any dataset, any size with a single line of code
 Home-page: https://github.com/AutoViML/AutoViz
 Author: Ram Seshadri
 License: Apache License 2.0
 Description: # AutoViz: The One-Line Automatic Data Visualization Library
         
         ![logo](logo.png)
@@ -74,23 +74,22 @@
         ```
         from autoviz import AutoViz_Class
         AV = AutoViz_Class()
         dft = AV.AutoViz(filename)
         ```
         
         Feed AutoViz any input filename (in CSV, txt, or JSON format), and set `max_rows_analyzed` and `max_cols_analyzed` based on memory limitations in your environment, and watch the magic happen!
-        <p>AutoViz generates charts in multiple formats using the `chart_format` setting which can one of the following:
-        - `'png'`, `'svg'`, or `'jpg'`: Inline Matplotlib charts
-            * Save locally (`verbose=2`) or display in Jupyter Notebooks (`verbose=1`)
-            * Default AutoViz behavior
-        - `'bokeh'`: Interactive Bokeh charts in Jupyter Notebooks
-        - `'server'`: Browser-based dashboards with individual chart types
-        - `'html'`: Interactive Bokeh charts saved as HTML files under the `AutoViz_Plots` directory (working folder) or specified directory using the `save_plot_dir` setting
         
-        AutoViz takes care of the rest. You'll see charts and plots on your screen.
+        AutoViz can now create charts in multiple  formats using the `chart_format` setting:
+        - If `chart_format ='png'` or `'svg'` or `'jpg'`: Matplotlib charts are plotted inline.
+            * Can be saved locally (using `verbose=2` setting) or displayed (`verbose=1`) in Jupyter Notebooks.
+            * This is the default behavior for AutoViz.
+        - If `chart_format='bokeh'`: Interactive Bokeh charts are plotted in Jupyter Notebooks.
+        - If `chart_format='server'`, dashboards will pop up for each kind of chart on your browser.
+        - If `chart_format='html'`, interactive Bokeh charts will be created and silently saved as HTML files under the `AutoViz_Plots` directory (under working folder) or any other directory that you specify using the `save_plot_dir` setting (during input).
         
         ![var_charts](var_charts.JPG)
         
         AV.AutoViz is the main plotting function in AutoViz_Class (AV). Depending on the chart_format you choose, AutoViz will automatically call either the AutoViz_Main function or AutoViz_Holo function.
         
         # API
         Arguments for AV.AutoViz() method:
@@ -235,15 +234,15 @@
         
         # License
         AutoViz is released under the Apache License, Version 2.0. By using AutoViz, you agree to the terms and conditions specified in the license.
         
         # Tips
         <p>That covers the main aspects of AutoViz, but here are some additional tips and reminders to help you make the most of the library:</p>
         <ul>
-          <li>Make sure to regularly upgrade AutoViz to benefit from the <a href="https://github.com/AutoViML/AutoViz/blob/main/updates.md">latest features, bug fixes, and improvements</a>. You can update it using <code>pip install --upgrade autoviz</code>.</li>
+          <li>Make sure to regularly upgrade AutoViz to benefit from the <a href="https://github.com/AutoViML/AutoViz/blob/master/updates.md">latest features, bug fixes, and improvements</a>. You can update it using <code>pip install --upgrade autoviz</code>.</li>
           <li>AutoViz is highly customizable, so don't hesitate to explore and experiment with various settings, such as <code>chart_format</code>, <code>verbose</code>, and <code>max_rows_analyzed</code>. This will allow you to create visualizations that better suit your specific needs and preferences.</li>
           <li>Remember to delete the <code>AutoViz_Plots</code> directory (or any custom directory you specified) periodically if you used the <code>verbose=2</code> option, as it can accumulate a large number of saved charts over time.</li>
           <li>For further guidance or inspiration, check out the <a href="https://towardsdatascience.com/autoviz-a-new-tool-for-automated-visualization-ec9c1744a6ad">Medium article on AutoViz</a>, as well as other online resources and tutorials.</li>
           <li>If you encounter any issues, have questions, or want to suggest improvements, don't hesitate to engage with the AutoViz community through the <a href="https://github.com/AutoViML/AutoViz">GitHub repository</a> or other online platforms.</li>
         </ul>
         <p>By leveraging AutoViz's powerful and flexible features, you can streamline your data visualization process and gain valuable insights more efficiently. Happy visualizing!</p>
```

### Comparing `autoviz-0.1.603/setup.py` & `autoviz-0.1.604/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="autoviz",
-    version="0.1.603",
+    version="0.1.604",
     author="Ram Seshadri",
     # author_email="author@example.com",
     description="Automatically Visualize any dataset, any size with a single line of code",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='Apache License 2.0',
     url="https://github.com/AutoViML/AutoViz",
@@ -25,15 +25,15 @@
         "pyamg",
         "matplotlib>=3.3.3",
         "seaborn>=0.11.1",
         "scikit-learn",
         "statsmodels",
         "nltk",
         "textblob",
-        "holoviews>=1.14.6",
+        "holoviews~=1.14.9",
         "bokeh>=2.4.2",
         "hvplot>=0.7.3",
         "panel>=0.12.6",
         "xgboost>=0.82",
         "fsspec>=0.8.3",
         "typing-extensions>=4.1.1",
     ],
```

