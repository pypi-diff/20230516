# Comparing `tmp/biocartograph-0.5.0.tar.gz` & `tmp/biocartograph-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biocartograph-0.5.0.tar", last modified: Mon May 15 11:33:34 2023, max compression
+gzip compressed data, was "biocartograph-0.5.1.tar", last modified: Tue May 16 13:52:00 2023, max compression
```

## Comparing `biocartograph-0.5.0.tar` & `biocartograph-0.5.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 rictjo    (1000) users      (100)        0 2023-05-15 11:33:34.206115 biocartograph-0.5.0/
--rw-r--r--   0 rictjo    (1000) users      (100)    11357 2023-01-03 14:01:46.000000 biocartograph-0.5.0/LICENSE
--rw-r--r--   0 rictjo    (1000) users      (100)     7248 2023-05-15 11:33:34.206115 biocartograph-0.5.0/PKG-INFO
--rw-r--r--   0 rictjo    (1000) users      (100)     6705 2023-04-04 06:38:15.000000 biocartograph-0.5.0/README.md
-drwxr-xr-x   0 rictjo    (1000) users      (100)        0 2023-05-15 11:33:34.204115 biocartograph-0.5.0/biocartograph.egg-info/
--rw-r--r--   0 rictjo    (1000) users      (100)     7248 2023-05-15 11:33:34.000000 biocartograph-0.5.0/biocartograph.egg-info/PKG-INFO
--rw-r--r--   0 rictjo    (1000) users      (100)      301 2023-05-15 11:33:34.000000 biocartograph-0.5.0/biocartograph.egg-info/SOURCES.txt
--rw-r--r--   0 rictjo    (1000) users      (100)        1 2023-05-15 11:33:34.000000 biocartograph-0.5.0/biocartograph.egg-info/dependency_links.txt
--rw-r--r--   0 rictjo    (1000) users      (100)       14 2023-05-15 11:33:34.000000 biocartograph-0.5.0/biocartograph.egg-info/top_level.txt
--rw-r--r--   0 rictjo    (1000) users      (100)       38 2023-05-15 11:33:34.206115 biocartograph-0.5.0/setup.cfg
--rw-r--r--   0 rictjo    (1000) users      (100)      910 2023-05-15 11:06:59.000000 biocartograph-0.5.0/setup.py
-drwxr-xr-x   0 rictjo    (1000) users      (100)        0 2023-05-15 11:33:34.203115 biocartograph-0.5.0/src/
-drwxr-xr-x   0 rictjo    (1000) users      (100)        0 2023-05-15 11:33:34.205115 biocartograph-0.5.0/src/biocartograph/
--rw-r--r--   0 rictjo    (1000) users      (100)       23 2023-03-26 08:32:40.000000 biocartograph-0.5.0/src/biocartograph/__init__.py
--rw-r--r--   0 rictjo    (1000) users      (100)    14381 2023-03-26 10:38:54.000000 biocartograph-0.5.0/src/biocartograph/enrichment.py
--rw-r--r--   0 rictjo    (1000) users      (100)    19918 2023-05-15 11:06:59.000000 biocartograph-0.5.0/src/biocartograph/quantification.py
--rw-r--r--   0 rictjo    (1000) users      (100)    25243 2023-05-15 11:06:59.000000 biocartograph-0.5.0/src/biocartograph/special.py
+drwxr-xr-x   0 rictjo    (1000) users      (100)        0 2023-05-16 13:52:00.694829 biocartograph-0.5.1/
+-rw-r--r--   0 rictjo    (1000) users      (100)    11357 2023-01-03 14:01:46.000000 biocartograph-0.5.1/LICENSE
+-rw-r--r--   0 rictjo    (1000) users      (100)     7248 2023-05-16 13:52:00.694829 biocartograph-0.5.1/PKG-INFO
+-rw-r--r--   0 rictjo    (1000) users      (100)     6705 2023-04-04 06:38:15.000000 biocartograph-0.5.1/README.md
+drwxr-xr-x   0 rictjo    (1000) users      (100)        0 2023-05-16 13:52:00.693829 biocartograph-0.5.1/biocartograph.egg-info/
+-rw-r--r--   0 rictjo    (1000) users      (100)     7248 2023-05-16 13:52:00.000000 biocartograph-0.5.1/biocartograph.egg-info/PKG-INFO
+-rw-r--r--   0 rictjo    (1000) users      (100)      301 2023-05-16 13:52:00.000000 biocartograph-0.5.1/biocartograph.egg-info/SOURCES.txt
+-rw-r--r--   0 rictjo    (1000) users      (100)        1 2023-05-16 13:52:00.000000 biocartograph-0.5.1/biocartograph.egg-info/dependency_links.txt
+-rw-r--r--   0 rictjo    (1000) users      (100)       14 2023-05-16 13:52:00.000000 biocartograph-0.5.1/biocartograph.egg-info/top_level.txt
+-rw-r--r--   0 rictjo    (1000) users      (100)       38 2023-05-16 13:52:00.694829 biocartograph-0.5.1/setup.cfg
+-rw-r--r--   0 rictjo    (1000) users      (100)      910 2023-05-16 13:50:30.000000 biocartograph-0.5.1/setup.py
+drwxr-xr-x   0 rictjo    (1000) users      (100)        0 2023-05-16 13:52:00.693829 biocartograph-0.5.1/src/
+drwxr-xr-x   0 rictjo    (1000) users      (100)        0 2023-05-16 13:52:00.694829 biocartograph-0.5.1/src/biocartograph/
+-rw-r--r--   0 rictjo    (1000) users      (100)       23 2023-03-26 08:32:40.000000 biocartograph-0.5.1/src/biocartograph/__init__.py
+-rw-r--r--   0 rictjo    (1000) users      (100)    14381 2023-03-26 10:38:54.000000 biocartograph-0.5.1/src/biocartograph/enrichment.py
+-rw-r--r--   0 rictjo    (1000) users      (100)    19937 2023-05-16 13:50:30.000000 biocartograph-0.5.1/src/biocartograph/quantification.py
+-rw-r--r--   0 rictjo    (1000) users      (100)    27027 2023-05-16 13:50:30.000000 biocartograph-0.5.1/src/biocartograph/special.py
```

### Comparing `biocartograph-0.5.0/LICENSE` & `biocartograph-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `biocartograph-0.5.0/PKG-INFO` & `biocartograph-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biocartograph
-Version: 0.5.0
+Version: 0.5.1
 Summary: Package was renamed from Biocarta v0.2.27 to Biocartograph because of an unintentional name clash
 Home-page: https://github.com/rictjo/biocarta
 Author: Richard Tjörnhammar
 Author-email: richard.tjornhammar@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `biocartograph-0.5.0/README.md` & `biocartograph-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `biocartograph-0.5.0/biocartograph.egg-info/PKG-INFO` & `biocartograph-0.5.1/biocartograph.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biocartograph
-Version: 0.5.0
+Version: 0.5.1
 Summary: Package was renamed from Biocarta v0.2.27 to Biocartograph because of an unintentional name clash
 Home-page: https://github.com/rictjo/biocarta
 Author: Richard Tjörnhammar
 Author-email: richard.tjornhammar@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `biocartograph-0.5.0/setup.py` & `biocartograph-0.5.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name         = "biocartograph",
-    version      = "0.5.0",
+    version      = "0.5.1",
     author       = "Richard Tjörnhammar",
     author_email = "richard.tjornhammar@gmail.com",
     description  = "Package was renamed from Biocarta v0.2.27 to Biocartograph because of an unintentional name clash",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/rictjo/biocarta",
     packages = setuptools.find_packages('src'),
```

### Comparing `biocartograph-0.5.0/src/biocartograph/enrichment.py` & `biocartograph-0.5.1/src/biocartograph/enrichment.py`

 * *Files identical despite different names*

### Comparing `biocartograph-0.5.0/src/biocartograph/quantification.py` & `biocartograph-0.5.1/src/biocartograph/quantification.py`

 * *Files 0% similar despite different names*

```diff
@@ -166,19 +166,19 @@
                 else :
                     print ( item[0],'\t=\t [', str(item[1]) ,']', file=ofile )
             print ( 'PYTHON GLOBALS:\n ',
 			'\n'.join([ '\t=\t '.join([str(i) for i in item if not i is None]) for item in globals().items() if not item is None ] ),
 			file = ofile )
     #
     if bVerbose:
-        print ( "BEGIN WARNINGS : ISSUED HERE MEANS THAT SOME ITEMS WITH ZERO STANDARD DEVIATION ARE DROPPED")
+        print ( "INFORMATION : \t WARNINGS ISSUED AFTER THIS MESSAGE MEANS THAT SOME ITEMS WITH ZERO STANDARD DEVIATION WERE DROPPED\nBEGIN")
     adf = adf.iloc[ np.inf != np.abs( 1.0/np.std(adf.values,1) ) ,
                     np.inf != np.abs( 1.0/np.std(adf.values,0) ) ].copy().apply(pd.to_numeric)
-    if bVerbose:
-        print ( "END STD WARNINGS")
+    if bVerbose :
+        print ( "END")
     #
     comp_df = None
     if not jdf is None :
         if not ( alignment_label is None ) :
             if bVerbose :
                 print ( "CONDUCTING COMPOSITIONAL ANALYSIS" )
             comp_df = biox.calculate_compositions ( adf , jdf, label = alignment_label , bAddPies=bAddPies )
```

### Comparing `biocartograph-0.5.0/src/biocartograph/special.py` & `biocartograph-0.5.1/src/biocartograph/special.py`

 * *Files 4% similar despite different names*

```diff
@@ -474,53 +474,83 @@
     for i in range( len(drsp) ) :
         if drsp[i] == '.' or drsp[i] == '..' :
             continue
         if len(drsp[:i+1])>0 :
             thisdir = '/'.join(drsp[:i+1])
             l = set( os.listdir ( '/'.join(thisdir.split('/')[:-1]) ) )
             if not thisdir.split('/')[-1] in l :
-                os.mkdir( thisdir )
+                try:
+                    os.mkdir( thisdir )
+                except:
+                    print ( "WOULD NOT CREATE DIRECTORY:",thisdir,"\n\t\t(WILL PRETEND IT EXISTS ANYWAY)")
 
 #
 def quick_check_solution(header_str:str = '../results/DMHMSY_Tue_May__2_10_57_05_2023_' ) :
     file 	= header_str + 'soldf_f.tsv'
     df		= pd.read_csv(file,sep='\t',index_col=0 )
     print ( df.iloc[:,np.argmax(df.iloc[1,:].values)]   )
 
 
 def generate_atlas_files ( header_str:str ,
                 fcfile:str = 'clustering/final_consensus.tsv' ,
 		nnfile:str = 'distance/nearest_neighbors.tsv' ,
                 umfile:str = 'UMAP/UMAP.tsv' ,
                 ccfile:str = 'UMAP/cluster_centers.tsv' ,
-		pofile:str = 'UMAP/UMAP_polygons.tsv' , nNN:int=20 ,
+		pofile:str = 'UMAP/UMAP_polygons.tsv' ,
+                pcadir:str = 'PCA/',
+                evadir:str = 'evaluation/',
+                nNN:int=20 ,
                 additional_directories:list[str] = ['data','enrichment','evaluation','graph','PCA','UMAP',
-					'svg','svg/heatmap','svg/bubble','svg/treemap','html','html/clustering_DV']) :
+					'svg'  , 'svg/heatmap','svg/bubble','svg/treemap','svg/fountain',
+                                        'html' , 'html']) :
     #
     # START ATLAS GEN
     sep = '\t'
+    #
+    hdir_str = header_str
+    if hdir_str[-1] == '_' :
+        hdir_str =  hdir_str[:-1] + '/'
+    #
     df_sol_     = pd.read_csv( header_str + 'resdf_f.tsv' , sep=sep , index_col=0 ) # SHOULD BE ASSERTED
     df_pca_     = pd.read_csv( header_str + 'pcas_df.tsv' , sep=sep , index_col=0 ) # SHOULD BE ASSERTED
+    df_pca_s    = pd.read_csv( header_str + 'pcaw_df.tsv' , sep=sep , index_col=0 ) # SHOULD BE ASSERTED
+    if 'str' in str(type(pcadir)) :
+        if pcadir[-1] != '/' :
+            pcadir += '/'
+        create_directory ( hdir_str + pcadir )
+        df_pca_ .to_csv( hdir_str + pcadir + 'pca_analytes_df.tsv' )
+        df_pca_s.to_csv( hdir_str + pcadir +  'pca_samples_df.tsv' )
+    #
+    if 'str' in str(type(evadir)) :
+        if evadir[-1] != '/' :
+            evadir += '/'
+        create_directory ( hdir_str + evadir )
+        e1df = pd.read_csv( header_str + 'soldf_f.tsv' , sep=sep , index_col=0 )
+        e1df .to_csv( hdir_str + evadir + 'solution_analytes.tsv' ,sep=sep )
+        del e1df
+        e2df = pd.read_csv( header_str + 'soldf_s.tsv' , sep=sep , index_col=0 )
+        e2df .to_csv( hdir_str + evadir + 'solution_samples.tsv' , sep=sep )
+        del e2df
+        c1df = pd.read_csv( header_str + 'composition.tsv'  , sep=sep , index_col=0 )
+        c1df .to_csv( hdir_str + evadir + 'composition.tsv' , sep=sep )
+        del c1df
+    #
     common_idx  = sorted( list( set( df_sol_.index.values ) & set( df_pca_.index.values )))
     df_sol_     = df_sol_.loc[ common_idx,: ]
     df_pca_     = df_pca_.loc[ common_idx,: ]
     #
     df		= df_sol_
     minmax      = lambda x: np.array( [ np.min(x,0) , np.max(x,0) ] )
     scale       = minmax ( df.loc[:,[c for c in df if 'UMAP.' in c ]].values )
     dfs         = ( df .loc[:,[c for c in df if 'UMAP.' in c ]] - scale[0]) / (scale[1]-scale[0])
     dfs.columns = [ str(c) + '.scaled' for c in dfs.columns ]
     df          = pd.concat([df.T,dfs.T]).T
     all_hulls   = generate_hulls( df , hid = '.scaled' ,
                         bPlottered=False )
     #
-    hdir_str = header_str
-    if hdir_str[-1] == '_' :
-        hdir_str =  hdir_str[:-1] + '/'
-    #
     create_directory ( hdir_str + '/'.join( fcfile.split('/')[:-1]) )
     final_consensus_df = df_sol_.loc[:,['cids.max']].rename(columns={'cids.max':'cluster'}).copy()
     final_consensus_df .index.name = 'gene'
     final_consensus_df .to_csv( hdir_str + fcfile, sep=sep )
     #
     create_directory ( hdir_str + '/'.join( umfile.split('/')[:-1]) )
     udf = df.loc[:,[c for c in df.columns if 'UMAP' in c ] ]
@@ -543,14 +573,23 @@
     nninfo  = generate_neighbor_distance_information(  df_pca_ , lab = 'PCA' ,
 			 iex = -1 , nNN = nNN , sep = '\t' )
     o_f = open( hdir_str + nnfile,'w')
     print ( nninfo , file=o_f )
     o_f .close()
     for dir in additional_directories :
         create_directory ( hdir_str + dir )
+    #
+    # CHECK FOR ENRICHMENTS
+    hdr_dir   = '/'.join( header_str.split('/')[:-1] )
+    id_tag    = header_str.split('/')[-1]
+    import os
+    enr_files = [ l for l in set(os.listdir(hdr_dir)) if id_tag in l and ('treemap' in l or 'GFA' in l or 'enrichment' in l ) ]
+    if len(enr_files) > 0 :
+        for f in enr_files :
+            os.system('cp ' + hdr_dir + '/' + f + ' ' +  hdir_str + 'enrichment/' + f )
 
 
 if __name__ == '__main__':
     #
     reformat_results_and_print_gmtfile_pcfile(header_str = '../results/DMHMSY_Fri_Mar_17_14_37_07_2023_' )
     reformat_results_and_print_gmtfile_pcfile(header_str = '../results/DMHMSY_Fri_Mar_17_16_00_47_2023_' )
     #
```

