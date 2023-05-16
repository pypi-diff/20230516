# Comparing `tmp/kmerator-0.7.6b0.tar.gz` & `tmp/kmerator-0.7.7b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kmerator-0.7.6b0.tar", last modified: Mon May 15 08:37:12 2023, max compression
+gzip compressed data, was "kmerator-0.7.7b0.tar", last modified: Tue May 16 08:28:58 2023, max compression
```

## Comparing `kmerator-0.7.6b0.tar` & `kmerator-0.7.7b0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 benoit    (1017) bio2m     (1010)        0 2023-05-15 08:37:12.664667 kmerator-0.7.6b0/
--rw-r--r--   0 benoit    (1017) bio2m     (1010)      182 2023-04-17 07:20:43.000000 kmerator-0.7.6b0/MANIFEST.in
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)    13261 2023-05-15 08:37:12.660238 kmerator-0.7.6b0/PKG-INFO
--rw-r--r--   0 benoit    (1017) bio2m     (1010)    11434 2023-05-10 16:09:57.000000 kmerator-0.7.6b0/README.md
-drwxrwxr-x   0 benoit    (1017) bio2m     (1010)        0 2023-05-15 08:37:12.516152 kmerator-0.7.6b0/kmerator/
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)      115 2023-04-17 07:49:13.000000 kmerator-0.7.6b0/kmerator/__init__.py
--rwxr-xr-x   0 benoit    (1017) bio2m     (1010)      249 2023-02-16 14:55:54.000000 kmerator-0.7.6b0/kmerator/color.py
--rwxr-xr-x   0 benoit    (1017) bio2m     (1010)     2715 2023-02-17 12:04:30.000000 kmerator-0.7.6b0/kmerator/config.py
--rwxr-xr-x   0 benoit    (1017) bio2m     (1010)    19218 2023-05-10 10:26:54.000000 kmerator-0.7.6b0/kmerator/dataset.py
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)      289 2023-02-13 12:52:30.000000 kmerator-0.7.6b0/kmerator/exit.py
--rwxr-xr-x   0 benoit    (1017) bio2m     (1010)     1554 2023-05-11 09:37:25.000000 kmerator-0.7.6b0/kmerator/info.py
--rwxr-xr-x   0 benoit    (1017) bio2m     (1010)    11900 2023-03-07 20:09:49.000000 kmerator-0.7.6b0/kmerator/kmerator.py
--rw-r--r--   0 benoit    (1017) bio2m     (1010)    16939 2023-05-11 10:39:13.000000 kmerator-0.7.6b0/kmerator/kmerize.py
--rw-r--r--   0 benoit    (1017) bio2m     (1010)      757 2023-02-16 14:24:06.000000 kmerator-0.7.6b0/kmerator/longest_transcript.py
--rwxr-xr-x   0 benoit    (1017) bio2m     (1010)    10602 2023-02-28 11:49:15.000000 kmerator-0.7.6b0/kmerator/mk_geneinfo.py
--rwxr-xr-x   0 benoit    (1017) bio2m     (1010)     8671 2023-02-20 09:09:59.000000 kmerator-0.7.6b0/kmerator/mk_transcriptome.py
--rwxr-xr-x   0 benoit    (1017) bio2m     (1010)    11953 2023-05-10 16:30:50.000000 kmerator-0.7.6b0/kmerator/options.py
-drwxrwxr-x   0 benoit    (1017) bio2m     (1010)        0 2023-05-15 08:37:12.611082 kmerator-0.7.6b0/kmerator.egg-info/
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)    13261 2023-05-15 08:37:11.000000 kmerator-0.7.6b0/kmerator.egg-info/PKG-INFO
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)      481 2023-05-15 08:37:12.000000 kmerator-0.7.6b0/kmerator.egg-info/SOURCES.txt
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)        1 2023-05-15 08:37:11.000000 kmerator-0.7.6b0/kmerator.egg-info/dependency_links.txt
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)       53 2023-05-15 08:37:11.000000 kmerator-0.7.6b0/kmerator.egg-info/entry_points.txt
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)       18 2023-05-15 08:37:12.000000 kmerator-0.7.6b0/kmerator.egg-info/requires.txt
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)        9 2023-05-15 08:37:12.000000 kmerator-0.7.6b0/kmerator.egg-info/top_level.txt
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)       38 2023-05-15 08:37:12.667327 kmerator-0.7.6b0/setup.cfg
--rw-r--r--   0 benoit    (1017) bio2m     (1010)     1008 2023-02-28 16:14:06.000000 kmerator-0.7.6b0/setup.py
+drwxrwxr-x   0 benoit    (1017) bio2m     (1010)        0 2023-05-16 08:28:58.832640 kmerator-0.7.7b0/
+-rw-r--r--   0 benoit    (1017) bio2m     (1010)      182 2023-04-17 07:20:43.000000 kmerator-0.7.7b0/MANIFEST.in
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)    13261 2023-05-16 08:28:58.828371 kmerator-0.7.7b0/PKG-INFO
+-rw-r--r--   0 benoit    (1017) bio2m     (1010)    11434 2023-05-10 16:09:57.000000 kmerator-0.7.7b0/README.md
+drwxrwxr-x   0 benoit    (1017) bio2m     (1010)        0 2023-05-16 08:28:58.724654 kmerator-0.7.7b0/kmerator/
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)      115 2023-04-17 07:49:13.000000 kmerator-0.7.7b0/kmerator/__init__.py
+-rwxr-xr-x   0 benoit    (1017) bio2m     (1010)      249 2023-02-16 14:55:54.000000 kmerator-0.7.7b0/kmerator/color.py
+-rwxr-xr-x   0 benoit    (1017) bio2m     (1010)     2715 2023-02-17 12:04:30.000000 kmerator-0.7.7b0/kmerator/config.py
+-rwxr-xr-x   0 benoit    (1017) bio2m     (1010)    19683 2023-05-16 08:28:01.000000 kmerator-0.7.7b0/kmerator/dataset.py
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)      289 2023-02-13 12:52:30.000000 kmerator-0.7.7b0/kmerator/exit.py
+-rwxr-xr-x   0 benoit    (1017) bio2m     (1010)     1554 2023-05-15 12:09:40.000000 kmerator-0.7.7b0/kmerator/info.py
+-rwxr-xr-x   0 benoit    (1017) bio2m     (1010)    11941 2023-05-16 08:27:00.000000 kmerator-0.7.7b0/kmerator/kmerator.py
+-rw-r--r--   0 benoit    (1017) bio2m     (1010)    16939 2023-05-11 10:39:13.000000 kmerator-0.7.7b0/kmerator/kmerize.py
+-rw-r--r--   0 benoit    (1017) bio2m     (1010)      757 2023-02-16 14:24:06.000000 kmerator-0.7.7b0/kmerator/longest_transcript.py
+-rwxr-xr-x   0 benoit    (1017) bio2m     (1010)    10602 2023-02-28 11:49:15.000000 kmerator-0.7.7b0/kmerator/mk_geneinfo.py
+-rwxr-xr-x   0 benoit    (1017) bio2m     (1010)     8671 2023-02-20 09:09:59.000000 kmerator-0.7.7b0/kmerator/mk_transcriptome.py
+-rwxr-xr-x   0 benoit    (1017) bio2m     (1010)    12152 2023-05-16 08:26:02.000000 kmerator-0.7.7b0/kmerator/options.py
+drwxrwxr-x   0 benoit    (1017) bio2m     (1010)        0 2023-05-16 08:28:58.812392 kmerator-0.7.7b0/kmerator.egg-info/
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)    13261 2023-05-16 08:28:58.000000 kmerator-0.7.7b0/kmerator.egg-info/PKG-INFO
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)      481 2023-05-16 08:28:58.000000 kmerator-0.7.7b0/kmerator.egg-info/SOURCES.txt
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)        1 2023-05-16 08:28:58.000000 kmerator-0.7.7b0/kmerator.egg-info/dependency_links.txt
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)       53 2023-05-16 08:28:58.000000 kmerator-0.7.7b0/kmerator.egg-info/entry_points.txt
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)       18 2023-05-16 08:28:58.000000 kmerator-0.7.7b0/kmerator.egg-info/requires.txt
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)        9 2023-05-16 08:28:58.000000 kmerator-0.7.7b0/kmerator.egg-info/top_level.txt
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)       38 2023-05-16 08:28:58.835056 kmerator-0.7.7b0/setup.cfg
+-rw-r--r--   0 benoit    (1017) bio2m     (1010)     1008 2023-02-28 16:14:06.000000 kmerator-0.7.7b0/setup.py
```

### Comparing `kmerator-0.7.6b0/PKG-INFO` & `kmerator-0.7.7b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kmerator
-Version: 0.7.6b0
+Version: 0.7.7b0
 Summary: Find specific gene or transcript kmers. And more.
 Home-page: https://github.com/Transipedia/kmerator
 Author: Sébastien RIQUIER, IRMB, Montpellier
 Author-email: sebastien.riquier@ucd.ie
 License: GPLv3
 Description: # Kmerator
```

### Comparing `kmerator-0.7.6b0/README.md` & `kmerator-0.7.7b0/README.md`

 * *Files identical despite different names*

### Comparing `kmerator-0.7.6b0/kmerator/config.py` & `kmerator-0.7.7b0/kmerator/config.py`

 * *Files identical despite different names*

### Comparing `kmerator-0.7.6b0/kmerator/dataset.py` & `kmerator-0.7.7b0/kmerator/dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,14 +50,16 @@
         dataset.list()
     elif args.update_last:
         dataset.update_last()
     elif args.rm_dataset:
         dataset.remove()
     elif args.mk_dataset:
         dataset.make()
+    elif args.last_avail:
+        dataset.last_available()
     elif args.load:
         geneinfo_dict, transcriptome_dict = dataset.load()
         for type in ('gene', 'symbol', 'alias', 'transcript'):
             print(type, next(iter(geneinfo_dict[type].items())))
         print(next(iter(transcriptome_dict.items())))
         print("Assembly in geneinfo:", geneinfo_dict['assembly'])
         print("Assembly in args.assembly:", args.assembly)
@@ -89,25 +91,26 @@
         ### Is args.specie is an alternative name ?
         if self.args.specie.lower() in species:
             self.args.specie =  species[self.args.specie.lower()]
         if self.args.release == 'last' and not self.args.list_dataset:
             self.get_ebl_releases()
             self.args.release = str(max(self.ebl_releases))
         ### check if dataset is locally present and assign variable for each file
-        self.dataset_ok = self.dataset_here()
+        if args.datadir:
+            self.dataset_ok = self.dataset_here()
 
 
     def get_ebl_releases(self):
         """ get avalaible releases on Ensembl, limited to 90 """
         try:
             r = requests.get(self.base_url)
         except requests.exceptions.ConnectionError:
             ### If no connection to Ensembl, suggest to use last local Release
-            print(f"{YELLOW} Error connecting to Ensembl.{ENDCOL}")                
-            local_releases = self.get_local_releases()                    
+            print(f"{YELLOW} Error connecting to Ensembl.{ENDCOL}")
+            local_releases = self.get_local_releases()
             if not local_releases:
                 print(f"{YELLOW} No dataset found in {self.args.datadir!r}, exit.")
                 exit.gracefully(self.args)
             ask = 'y'
             if not self.args.yes:
                 ask = input(f" {YELLOW}Last local Release found in datasets is {max(local_releases)}. Continue with it? (Yn): {ENDCOL}") or 'y'
             if ask.lower() == 'y':
@@ -176,15 +179,14 @@
             self.build()
         ### Load transcriptome
         with open(self.transcriptome_pkl, 'rb') as fic:
             transcriptome_dict = pickle.load(fic)
         return transcriptome_dict
 
 
-
     def dataset_here(self):
         """
         - Check if dataset is present in datadir
         - assign files names to matching variables
         """
         attended  = ['transcriptome_pkl', 'transcriptome_jf', 'geneinfo_pkl', 'report_md']
         found = 0
@@ -383,38 +385,45 @@
             else:
                 sys.exit("Aborted by user.")
         else:
             print(f"The last release for {self.args.specie} is {last_ebl_release}, nothing to do.")
         exit.gracefully(self.args)
 
 
+    def last_available(self):
+        # ~ self.get_ebl_releases()
+        print(max(self.ebl_releases))
+        exit.gracefully(self.args)
+
+
 def usage():
     parser = argparse.ArgumentParser()
+    exclusive = parser.add_mutually_exclusive_group(required=True)
     ### OPTION
     parser.add_argument('-S', '--specie',
                         help=(
                             "indicate a specie referenced in Ensembl, to help, follow the link "
                             "https://rest.ensembl.org/documentation/info/species. You can use "
                             "the 'name', the 'display_name' or any 'aliases'. For example human, "
                             "homo_sapiens or homsap are valid (default: human)."
                             ),
                         default='human',
                         )
     parser.add_argument('-r', '--release',
                         help="release of transcriptome (default: last).",
                         default="last",
                         )
-    parser.add_argument('-d', '--datadir',
+    exclusive.add_argument('-d', '--datadir',
                         help=(
                             "Directory where kmerator file are stored. Files are:"
                             "\n - fasta file of modified transcriptome (fa)"
                             "\n - jellyfish of this transcriptome (jf)"
                             "\n - metadata file like gene-symbols or aliases, "
                             ),
-                        required = True,
+                        # ~ required = True,
                         )
     parser.add_argument('-l', '--list-dataset', '--datasets',
                         action="store_true",
                         help="list local releases",
                        )
     parser.add_argument('--debug',
                         action="store_true",
@@ -446,14 +455,18 @@
                         help="builds a new dataset if a new version is found on Ensembl",
                        )
     parser.add_argument('-k', '--kmer-length',
                         type=int,
                         help="kmer length (default: 31)",
                         default=31,
                        )
+    exclusive.add_argument('--last-avail', '--last-available',
+                        action='store_true',
+                        help="last release available on Ensembl",
+                       )
     parser.add_argument('--keep',
                         action='store_true',
                         help=("keep kmerator transcriptome as fasta format."
                             ),
                         )
     parser.add_argument('-y', '--yes',
                         action='store_true',
```

### Comparing `kmerator-0.7.6b0/kmerator/info.py` & `kmerator-0.7.7b0/kmerator/info.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 Genral informations on to the program.
 """
 
 APPNAME = "kmerator"
 SHORTDESC = "Find specific gene or transcript kmers. And more."
 LICENCE = "GPL3"
-VERSION = "0.7.6-beta"
+VERSION = "0.7.7-beta"
 AUTHOR = 'Sébastien RIQUIER, IRMB, Montpellier'
 AUTHOR_EMAIL = "sebastien.riquier@ucd.ie"
 CONTIBUTORS = [
     'Chloe BESSIERE chloe.bessiere@inserm.fr>'
     'Benoit GUIBERT <benoit.guibert@inserm.fr>',
 ]
 DOC = f"""
```

### Comparing `kmerator-0.7.6b0/kmerator/kmerator.py` & `kmerator-0.7.7b0/kmerator/kmerator.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,14 +48,15 @@
     ### check files of the dataset (download if needed)
     dataset = Dataset(args)
 
     ### Handle dataset options: '--list-dataset', '--rm-dataset'
     if args.list_dataset: dataset.list()
     if args.rm_dataset: dataset.remove()
     if args.mk_dataset: dataset.make()
+    if args.last_avail: dataset.last_available()
     if args.update_dataset: dataset.update_last()
 
 
     ### load kmerator geneinfo file as dict
     print(f" 🧬 Load dataset {args.release!r}.")
 
     ### Important objects
@@ -67,18 +68,18 @@
 
     ### load transcriptome if --selection option is set
     if args.selection:
         ### create shared objects among multiple processes with Manager()
         transcriptome_dict = dataset.load_transcriptome()
 
     ### load geneinfo
-    geneinfo_dict = dataset.load_geneinfo()    
+    geneinfo_dict = dataset.load_geneinfo()
     ### Find transcripts according the selection
     find_items(args, items, report, geneinfo_dict)
-    
+
     ### get specific kmers (using multithreading)
     print(f" 🧬 Extract specific kmers, please wait..")
     SpecificKmers(args, report, items, transcriptome_dict, geneinfo_dict)
 
     ### Concatene results
     print(f" 🧬 Build finals results and report")
     merged_results(args)
```

### Comparing `kmerator-0.7.6b0/kmerator/kmerize.py` & `kmerator-0.7.7b0/kmerator/kmerize.py`

 * *Files identical despite different names*

### Comparing `kmerator-0.7.6b0/kmerator/longest_transcript.py` & `kmerator-0.7.7b0/kmerator/longest_transcript.py`

 * *Files identical despite different names*

### Comparing `kmerator-0.7.6b0/kmerator/mk_geneinfo.py` & `kmerator-0.7.7b0/kmerator/mk_geneinfo.py`

 * *Files identical despite different names*

### Comparing `kmerator-0.7.6b0/kmerator/mk_transcriptome.py` & `kmerator-0.7.7b0/kmerator/mk_transcriptome.py`

 * *Files identical despite different names*

### Comparing `kmerator-0.7.6b0/kmerator/options.py` & `kmerator-0.7.7b0/kmerator/options.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,14 +151,18 @@
                         action='store_true',
                         help="remove a dataset, according with --specie and --release options",
                       )
     exclusive.add_argument('--mk-dataset',
                         action='store_true',
                         help="make a dataset, according with --specie and --release options",
                       )
+    exclusive.add_argument('--last-avail', '--last-available',
+                        action='store_true',
+                        help="last release available on Ensembl",
+                       )
     exclusive.add_argument('-u', '--update-dataset',
                         action="store_true",
                         help="builds a new dataset if a new version is found on Ensembl",
                        )
     parser.add_argument('-v', '--version',
                         action='version',
                         version=f'{parser.prog} v{info.VERSION}',
```

### Comparing `kmerator-0.7.6b0/kmerator.egg-info/PKG-INFO` & `kmerator-0.7.7b0/kmerator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kmerator
-Version: 0.7.6b0
+Version: 0.7.7b0
 Summary: Find specific gene or transcript kmers. And more.
 Home-page: https://github.com/Transipedia/kmerator
 Author: Sébastien RIQUIER, IRMB, Montpellier
 Author-email: sebastien.riquier@ucd.ie
 License: GPLv3
 Description: # Kmerator
```

### Comparing `kmerator-0.7.6b0/setup.py` & `kmerator-0.7.7b0/setup.py`

 * *Files identical despite different names*

