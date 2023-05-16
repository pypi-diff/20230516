# Comparing `tmp/vizad-0.0.2.tar.gz` & `tmp/vizad-0.0.3.tar.gz`

## Comparing `vizad-0.0.2.tar` & `vizad-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 vizad-0.0.2/.DS_Store
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 vizad-0.0.2/.idea/.gitignore
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 vizad-0.0.2/.idea/eda.iml
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 vizad-0.0.2/.idea/misc.xml
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 vizad-0.0.2/.idea/modules.xml
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 vizad-0.0.2/.idea/vcs.xml
--rw-r--r--   0        0        0     2572 2020-02-02 00:00:00.000000 vizad-0.0.2/.idea/workspace.xml
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 vizad-0.0.2/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 vizad-0.0.2/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 vizad-0.0.2/src/.DS_Store
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 vizad-0.0.2/src/vizad/.DS_Store
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vizad-0.0.2/src/vizad/__init__.py
--rw-r--r--   0        0        0     5706 2020-02-02 00:00:00.000000 vizad-0.0.2/src/vizad/bivariate.py
--rw-r--r--   0        0        0     7875 2020-02-02 00:00:00.000000 vizad-0.0.2/src/vizad/univariate.py
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 vizad-0.0.2/LICENSE
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 vizad-0.0.2/README.md
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 vizad-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 vizad-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 vizad-0.0.3/.DS_Store
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 vizad-0.0.3/.idea/.gitignore
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 vizad-0.0.3/.idea/eda.iml
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 vizad-0.0.3/.idea/misc.xml
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 vizad-0.0.3/.idea/modules.xml
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 vizad-0.0.3/.idea/vcs.xml
+-rw-r--r--   0        0        0     2750 2020-02-02 00:00:00.000000 vizad-0.0.3/.idea/workspace.xml
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 vizad-0.0.3/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 vizad-0.0.3/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 vizad-0.0.3/src/.DS_Store
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 vizad-0.0.3/src/vizad/.DS_Store
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vizad-0.0.3/src/vizad/__init__.py
+-rw-r--r--   0        0        0     5706 2020-02-02 00:00:00.000000 vizad-0.0.3/src/vizad/bivariate.py
+-rw-r--r--   0        0        0     7581 2020-02-02 00:00:00.000000 vizad-0.0.3/src/vizad/univariate.py
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 vizad-0.0.3/LICENSE
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 vizad-0.0.3/README.md
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 vizad-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 vizad-0.0.3/PKG-INFO
```

### Comparing `vizad-0.0.2/.DS_Store` & `vizad-0.0.3/src/.DS_Store`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 00000000: 0000 0001 4275 6431 0000 1000 0000 0800  ....Bud1........
 00000010: 0000 1000 0000 0209 0000 0000 0000 0000  ................
 00000020: 0000 0000 0000 0000 0000 0000 0000 0800  ................
 00000030: 0000 0800 0000 0000 0000 0000 0000 0000  ................
 00000040: 0000 0000 0000 0002 0000 0000 0000 0004  ................
-00000050: 0000 0001 0000 1000 7363 626f 6f6c 0100  ........scbool..
-00000060: 0000 0500 0000 0000 0000 0000 0000 0000  ................
+00000050: 0000 0001 0000 1000 0064 6277 7370 626c  .........dbwspbl
+00000060: 6f62 0000 0000 0000 0000 0000 0000 0000  ob..............
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -26,33 +26,33 @@
 00000190: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000200: 0000 0000 0000 0000 0000 0004 0000 0003  ................
-00000210: 0073 0072 0063 6664 7363 626f 6f6c 0100  .s.r.cfdscbool..
-00000220: 0000 0500 7600 6900 7a00 6100 6462 7773  ....v.i.z.a.dbws
-00000230: 7062 6c6f 6200 0000 b862 706c 6973 7430  pblob....bplist0
-00000240: 30d6 0102 0304 0506 0708 0708 0b08 5d53  0.............]S
-00000250: 686f 7753 7461 7475 7342 6172 5b53 686f  howStatusBar[Sho
-00000260: 7754 6f6f 6c62 6172 5b53 686f 7754 6162  wToolbar[ShowTab
-00000270: 5669 6577 5f10 1443 6f6e 7461 696e 6572  View_..Container
-00000280: 5368 6f77 5369 6465 6261 725c 5769 6e64  ShowSidebar\Wind
-00000290: 6f77 426f 756e 6473 5b53 686f 7753 6964  owBounds[ShowSid
-000002a0: 6562 6172 0809 0809 5f10 187b 7b35 3438  ebar...._..{{548
-000002b0: 2c20 3136 397d 2c20 7b39 3230 2c20 3433  , 169}, {920, 43
-000002c0: 367d 7d09 0815 232f 3b52 5f6b 6c6d 6e6f  6}}...#/;R_klmno
-000002d0: 8a00 0000 0000 0001 0100 0000 0000 0000  ................
-000002e0: 0d00 0000 0000 0000 0000 0000 0000 0000  ................
-000002f0: 8b00 0000 0500 7600 6900 7a00 6100 6466  ......v.i.z.a.df
-00000300: 6473 6362 6f6f 6c00 0000 0005 0076 0069  dscbool......v.i
-00000310: 007a 0061 0064 7653 726e 6c6f 6e67 0000  .z.a.dvSrnlong..
-00000320: 0001 0000 0000 0000 0000 0000 0000 0000  ................
+00000200: 0000 0000 0000 0000 0000 0004 0000 0005  ................
+00000210: 0076 0069 007a 0061 0064 6277 7370 626c  .v.i.z.a.dbwspbl
+00000220: 6f62 0000 00b8 6270 6c69 7374 3030 d601  ob....bplist00..
+00000230: 0203 0405 0607 0807 080b 085d 5368 6f77  ...........]Show
+00000240: 5374 6174 7573 4261 725b 5368 6f77 546f  StatusBar[ShowTo
+00000250: 6f6c 6261 725b 5368 6f77 5461 6256 6965  olbar[ShowTabVie
+00000260: 775f 1014 436f 6e74 6169 6e65 7253 686f  w_..ContainerSho
+00000270: 7753 6964 6562 6172 5c57 696e 646f 7742  wSidebar\WindowB
+00000280: 6f75 6e64 735b 5368 6f77 5369 6465 6261  ounds[ShowSideba
+00000290: 7208 0908 095f 1018 7b7b 3433 362c 2033  r...._..{{436, 3
+000002a0: 3736 7d2c 207b 3932 302c 2034 3336 7d7d  76}, {920, 436}}
+000002b0: 0908 1523 2f3b 525f 6b6c 6d6e 6f8a 0000  ...#/;R_klmno...
+000002c0: 0000 0000 0101 0000 0000 0000 000d 0000  ................
+000002d0: 0000 0000 0000 0000 0000 0000 008b 0000  ................
+000002e0: 0005 0076 0069 007a 0061 0064 6473 636c  ...v.i.z.a.ddscl
+000002f0: 626f 6f6c 0000 0000 0500 7600 6900 7a00  bool......v.i.z.
+00000300: 6100 6466 6473 6362 6f6f 6c00 0000 0005  a.dfdscbool.....
+00000310: 0076 0069 007a 0061 0064 7653 726e 6c6f  .v.i.z.a.dvSrnlo
+00000320: 6e67 0000 0001 0000 0000 0000 0000 0000  ng..............
 00000330: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000340: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000350: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000360: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000370: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000380: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000390: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `vizad-0.0.2/.idea/workspace.xml` & `vizad-0.0.3/.idea/workspace.xml`

 * *Files 3% similar despite different names*

#### Comparing `vizad-0.0.2/.idea/workspace.xml` & `vizad-0.0.3/.idea/workspace.xml`

```diff
@@ -13,14 +13,17 @@
   <component name="FileTemplateManagerImpl">
     <option name="RECENT_TEMPLATES">
       <list>
         <option value="Python Script"/>
       </list>
     </option>
   </component>
+  <component name="Git.Settings">
+    <option name="RECENT_GIT_ROOT_PATH" value="$PROJECT_DIR$/vizad"/>
+  </component>
   <component name="ProjectId" id="2PHYrtu9pshRERE8VxkqaXyEh03"/>
   <component name="ProjectViewState">
     <option name="hideEmptyMiddlePackages" value="true"/>
     <option name="showLibraryContents" value="true"/>
   </component>
   <component name="PropertiesComponent">{
   &quot;keyToString&quot;: {
@@ -42,14 +45,15 @@
       <created>1683115676288</created>
       <option name="number" value="Default"/>
       <option name="presentableId" value="Default"/>
       <updated>1683115676288</updated>
       <workItem from="1683115692344" duration="4031000"/>
       <workItem from="1683527910982" duration="7548000"/>
       <workItem from="1683537804084" duration="668000"/>
+      <workItem from="1683569514961" duration="598000"/>
     </task>
     <servers/>
   </component>
   <component name="TypeScriptGeneratedFilesManager">
     <option name="version" value="3"/>
   </component>
 </project>
```

### Comparing `vizad-0.0.2/.idea/inspectionProfiles/Project_Default.xml` & `vizad-0.0.3/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `vizad-0.0.2/src/vizad/.DS_Store` & `vizad-0.0.3/src/vizad/.DS_Store`

 * *Files identical despite different names*

### Comparing `vizad-0.0.2/src/vizad/bivariate.py` & `vizad-0.0.3/src/vizad/bivariate.py`

 * *Files identical despite different names*

### Comparing `vizad-0.0.2/src/vizad/univariate.py` & `vizad-0.0.3/src/vizad/univariate.py`

 * *Files 3% similar despite different names*

```diff
@@ -76,18 +76,21 @@
         
         # remove the excess axes
         excess_plots = subplot_rows*subplot_cols - numcols_len
         if excess_plots > 0:
             for i in range(numcols_len,subplot_rows*subplot_cols):
                 fig.delaxes(axes[i//subplot_cols,i%subplot_cols])
         plt.tight_layout()
+    # add suptitle
+    fig.suptitle("Univariate Analysis: Numeric Features",fontsize=20)
+    plt.tight_layout()
 
 
 
-def plot_univariate_categorical(df, catcols_name, subplot_cols=3, kind="count"):
+def plot_univariate_categorical(df, catcols_name, subplot_cols=3, kind="count",figsize=(10,10)):
     """
     This function takes a pandas dataframe and a list of column names containing
     categorical values and plots univariate distribution of each column. The user
     can choose the kind of plot to be displayed using the 'kind' parameter. The
     function returns a matplotlib figure object.
 
     Parameters:
@@ -97,35 +100,41 @@
     catcols_name : list of str
         The list of column names containing categorical values.
     subplot_cols : int (default=3)
         The number of subplots columns to display.
     kind : str (default='count')
         The kind of plot to be displayed. Possible values are 'count', and
         'proportion'.
+    figsize : tuple (default=(10,10))
 
     Returns:
     --------
     None
     """
     catcols_len = len(catcols_name)
     subplot_rows = 1
     # handle edge case when subplot_cols > numcols_len
     if subplot_cols >= catcols_len:
         subplot_cols = catcols_len
     else:
         subplot_rows = int(np.ceil(catcols_len / subplot_cols))
-    fig, axes = plt.subplots(subplot_rows, subplot_cols, figsize=(subplot_cols * 3, subplot_rows * 3))
+    fig, axes = plt.subplots(subplot_rows, 
+                             subplot_cols, 
+                             figsize=(max(subplot_cols*3,figsize[0]),max(subplot_rows*3,figsize[1])))
 
 
     # if subplot_rows == 1 or subplot_cols==1 then the axes object will be a 1D array
     # so we need to handle this case differently
     if (subplot_rows == 1) | (subplot_cols == 1):
         for i in range(catcols_len):
             if kind == "count":
-                sns.countplot(x=catcols_name[i], data=df, ax=axes[i])
+                sns.countplot(y=catcols_name[i], 
+                              data=df, 
+                              ax=axes[i],
+                              order=df[catcols_name[i]].value_counts().index)
             elif kind == "proportion":
                 # compute the proportions using value_counts(normalize=True)
                 data = df[catcols_name[i]].value_counts(normalize=True).reset_index()
 
                 # plot the piechart using matplotlib pie function
                 axes[i].pie(x=data[catcols_name[i]], labels=data["index"],
                             autopct="%.2f%%")
@@ -138,15 +147,18 @@
         if excess_plots > 0:
             for i in range(catcols_len, subplot_rows * subplot_cols):
                 fig.delaxes(axes[i])
         plt.tight_layout()
     else:  # if subplot_rows > 1 then the axes object will be a 2D array
         for i in range(catcols_len):
             if kind == "count":
-                sns.countplot(x=catcols_name[i], data=df, ax=axes[i // subplot_cols, i % subplot_cols])
+                sns.countplot(y=catcols_name[i], 
+                              data=df, 
+                              ax=axes[i // subplot_cols, i % subplot_cols],
+                              order=df[catcols_name[i]].value_counts().index)
             elif kind == "proportion":
                 # compute the proportions using value_counts(normalize=True)
                 data = df[catcols_name[i]].value_counts(normalize=True).reset_index()
 
                 # plot the piechart using matplotlib pie function
                 axes[i // subplot_cols, i % subplot_cols].pie(x=data[catcols_name[i]], labels=data["index"],
                                                               autopct="%.2f%%")
@@ -154,24 +166,12 @@
             else:
                 raise ValueError("kind parameter can only take values 'count', or 'proportion'")
         excess_plots = subplot_rows * subplot_cols - catcols_len
         if excess_plots > 0:
             for i in range(catcols_len, subplot_rows * subplot_cols):
                 fig.delaxes(axes[i // subplot_cols, i % subplot_cols])
         plt.tight_layout()
+    # add suptitle
+    fig.suptitle("Univariate Analysis: Categorical Features", fontsize=20)
+    plt.tight_layout()
 
-    # for i in range(catcols_len):
-    #     if kind == "count":
-    #         sns.countplot(x=catcols_name[i], data=df, ax=axes[i // subplot_cols, i % subplot_cols])
-    #     elif kind == "proportion":
-    #         # compute the proportions using value_counts(normalize=True)
-    #         data = df[catcols_name[i]].value_counts(normalize=True).reset_index()
-
-    #         # plot the piechart using matplotlib pie function
-    #         axes[i // subplot_cols, i % subplot_cols].pie(x=data[catcols_name[i]], labels=data["index"],
-    #                                                       autopct="%.2f%%")
-    #         axes[i // subplot_cols, i % subplot_cols].set_title(catcols_name[i])
-    # excess_plots = subplot_rows * subplot_cols - catcols_len
-    # if excess_plots > 0:
-    #     for i in range(catcols_len, subplot_rows * subplot_cols):
-    #         fig.delaxes(axes[i // subplot_cols, i % subplot_cols])
-    # plt.tight_layout()
+
```

### Comparing `vizad-0.0.2/LICENSE` & `vizad-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vizad-0.0.2/pyproject.toml` & `vizad-0.0.3/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "vizad"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
     {name = "Balaji Sundararaman", email = "bala@python4u.in"},
 ]
 description = "A simple visualization library for univariate and bivariate analysis"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `vizad-0.0.2/PKG-INFO` & `vizad-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vizad
-Version: 0.0.2
+Version: 0.0.3
 Summary: A simple visualization library for univariate and bivariate analysis
 Project-URL: Homepage, https://github.com/bala-srm/eda
 Project-URL: Bug Tracker, https://github.com/bala-srm/eda/issues
 Author-email: Balaji Sundararaman <bala@python4u.in>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

