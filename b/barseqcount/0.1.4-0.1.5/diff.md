# Comparing `tmp/barseqcount-0.1.4.tar.gz` & `tmp/barseqcount-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "barseqcount-0.1.4.tar", last modified: Thu Feb 23 03:45:56 2023, max compression
+gzip compressed data, was "barseqcount-0.1.5.tar", last modified: Tue May 16 05:30:08 2023, max compression
```

## Comparing `barseqcount-0.1.4.tar` & `barseqcount-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0 daming    (1000) daming    (1000)        0 2023-02-23 03:45:56.448791 barseqcount-0.1.4/
--rwxrwxrwx   0 daming    (1000) daming    (1000)    35823 2022-11-18 08:14:35.000000 barseqcount-0.1.4/LICENSE
--rwxrwxrwx   0 daming    (1000) daming    (1000)     1522 2023-02-23 03:45:56.444791 barseqcount-0.1.4/PKG-INFO
--rwxrwxrwx   0 daming    (1000) daming    (1000)      960 2023-02-23 03:44:06.000000 barseqcount-0.1.4/README.md
-drwxrwxrwx   0 daming    (1000) daming    (1000)        0 2023-02-23 03:45:56.327791 barseqcount-0.1.4/barseqcount/
-drwxrwxrwx   0 daming    (1000) daming    (1000)        0 2023-02-23 03:45:56.409793 barseqcount-0.1.4/barseqcount/barseqcount.egg-info/
--rwxrwxrwx   0 daming    (1000) daming    (1000)     1522 2023-02-23 03:45:56.000000 barseqcount-0.1.4/barseqcount/barseqcount.egg-info/PKG-INFO
--rwxrwxrwx   0 daming    (1000) daming    (1000)      256 2023-02-23 03:45:56.000000 barseqcount-0.1.4/barseqcount/barseqcount.egg-info/SOURCES.txt
--rwxrwxrwx   0 daming    (1000) daming    (1000)        1 2023-02-23 03:45:56.000000 barseqcount-0.1.4/barseqcount/barseqcount.egg-info/dependency_links.txt
--rwxrwxrwx   0 daming    (1000) daming    (1000)       12 2023-02-23 03:45:56.000000 barseqcount-0.1.4/barseqcount/barseqcount.egg-info/top_level.txt
--rwxrwxrwx   0 daming    (1000) daming    (1000)    45742 2023-02-23 02:15:19.000000 barseqcount-0.1.4/barseqcount/barseqcount.py
--rwxrwxrwx   0 daming    (1000) daming    (1000)       38 2023-02-23 03:45:56.448791 barseqcount-0.1.4/setup.cfg
--rwxrwxrwx   0 daming    (1000) daming    (1000)      903 2023-02-23 02:16:13.000000 barseqcount-0.1.4/setup.py
-drwxrwxrwx   0 daming    (1000) daming    (1000)        0 2023-02-23 03:45:56.425792 barseqcount-0.1.4/tests/
--rwxrwxrwx   0 daming    (1000) daming    (1000)      529 2023-01-20 19:11:26.000000 barseqcount-0.1.4/tests/test_.py
+drwxrwxrwx   0 daming    (1000) daming    (1000)        0 2023-05-16 05:30:05.444160 barseqcount-0.1.5/
+-rwxrwxrwx   0 daming    (1000) daming    (1000)    35823 2022-11-18 08:14:35.000000 barseqcount-0.1.5/LICENSE
+-rwxrwxrwx   0 daming    (1000) daming    (1000)     1522 2023-05-16 05:30:05.441161 barseqcount-0.1.5/PKG-INFO
+-rwxrwxrwx   0 daming    (1000) daming    (1000)      960 2023-02-23 03:44:06.000000 barseqcount-0.1.5/README.md
+drwxrwxrwx   0 daming    (1000) daming    (1000)        0 2023-05-16 05:30:05.340157 barseqcount-0.1.5/barseqcount/
+drwxrwxrwx   0 daming    (1000) daming    (1000)        0 2023-05-16 05:30:05.412158 barseqcount-0.1.5/barseqcount/barseqcount.egg-info/
+-rwxrwxrwx   0 daming    (1000) daming    (1000)     1522 2023-05-16 05:30:05.000000 barseqcount-0.1.5/barseqcount/barseqcount.egg-info/PKG-INFO
+-rwxrwxrwx   0 daming    (1000) daming    (1000)      256 2023-05-16 05:30:05.000000 barseqcount-0.1.5/barseqcount/barseqcount.egg-info/SOURCES.txt
+-rwxrwxrwx   0 daming    (1000) daming    (1000)        1 2023-05-16 05:30:05.000000 barseqcount-0.1.5/barseqcount/barseqcount.egg-info/dependency_links.txt
+-rwxrwxrwx   0 daming    (1000) daming    (1000)       12 2023-05-16 05:30:05.000000 barseqcount-0.1.5/barseqcount/barseqcount.egg-info/top_level.txt
+-rwxrwxrwx   0 daming    (1000) daming    (1000)    46123 2023-05-16 03:10:24.000000 barseqcount-0.1.5/barseqcount/barseqcount.py
+-rwxrwxrwx   0 daming    (1000) daming    (1000)       38 2023-05-16 05:30:05.445160 barseqcount-0.1.5/setup.cfg
+-rwxrwxrwx   0 daming    (1000) daming    (1000)      903 2023-05-16 03:10:17.000000 barseqcount-0.1.5/setup.py
+drwxrwxrwx   0 daming    (1000) daming    (1000)        0 2023-05-16 05:30:05.426160 barseqcount-0.1.5/tests/
+-rwxrwxrwx   0 daming    (1000) daming    (1000)      529 2023-01-20 19:11:26.000000 barseqcount-0.1.5/tests/test_.py
```

### Comparing `barseqcount-0.1.4/LICENSE` & `barseqcount-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `barseqcount-0.1.4/PKG-INFO` & `barseqcount-0.1.5/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: barseqcount
-Version: 0.1.4
+Version: 0.1.5
 Summary: Analysis of DNA barcode sequencing experiments
 Home-page: https://github.com/damienmarsic/barseqcount
 Author: Damien Marsic
 Author-email: damien.marsic@aliyun.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `barseqcount-0.1.4/README.md` & `barseqcount-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `barseqcount-0.1.4/barseqcount/barseqcount.egg-info/PKG-INFO` & `barseqcount-0.1.5/barseqcount/barseqcount.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: barseqcount
-Version: 0.1.4
+Version: 0.1.5
 Summary: Analysis of DNA barcode sequencing experiments
 Home-page: https://github.com/damienmarsic/barseqcount
 Author: Damien Marsic
 Author-email: damien.marsic@aliyun.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `barseqcount-0.1.4/barseqcount/barseqcount.py` & `barseqcount-0.1.5/barseqcount/barseqcount.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
-__version__='0.1.4'
-last_update='2023-02-23'
+__version__='0.1.5'
+last_update='2023-05-16'
 author='Damien Marsic, damien.marsic@aliyun.com'
 license='GNU General Public v3 (GPLv3)'
 
 import dmbiolib as dbl
-import argparse,sys,os,itertools,regex
+import argparse,sys,os,itertools,regex#### update!
 from glob import glob
 import numpy as np
 from collections import defaultdict
 from matplotlib import pyplot as plt
 from matplotlib.backends.backend_pdf import PdfPages
 
 script=os.path.basename(__file__).split('.')[0]
@@ -74,15 +74,15 @@
         if read=='rfiles':
             x=ln.split()
             fail+=dbl.check_read_file(x[-1])
             if len(x)>2:
                 fail+='\n  Too many items per line under READ FILES! Each line must contain a prefix followed by a single file name (merged reads if paired-end sequencing), separated by space or tab!'
             if len(x)==1:
                 z=dbl.prefix([x[0]])[0]
-                x.insert(0,x[0][:z])
+                x.insert(0,z)
             if x[0] in [k[0] for k in rfiles]:
                 fail+='\n  Duplicate prefix '+x[0]+' found under READ FILES! Each line must contain a different prefix!'
             else:
                 rfiles.append(x)
         if read=='templ':
             if not templ:
                 x,y=dbl.getfasta(ln,'atgc'+dbl.ambiguous,'atgcn',False)
@@ -279,15 +279,15 @@
     if fail:
         print('\n'+fail+'\n')
         sys.exit()
     ### Check read file(s) ###
     fail=''
     print('OK\n\n  Checking read files...    ',end='')
     for j in range(len(rfiles)):
-        nr,fail=dbl.readcount(rfiles[j][1],fail)
+        nr=dbl.readcount(rfiles[j][1])
         rfiles[j].append(nr)
         if nr<100:
             fail+='\n  Number of reads in '+rfiles[j][0]+' is too low!'
         f,step=dbl.initreadfile(rfiles[j][1])
         c=0
         a=0
         b=0
@@ -539,14 +539,16 @@
                     continue
                 thr=x
         if read=='samples':
             if not ln in S:
                 S[ln]=set(ln.split(','))
         if read in ('gtit','etit'):
             x=ln.split()
+            if x[0].lower()=='none':
+                continue
             if len(x)==1 or not x[1].replace('.','').isdigit():
                 fail+='\n  Titer value missing: '+ln
             elif x[0] not in S:
                 fail+='\n  Unknown sample name: '+x[0]
             elif read=='gtit' and gunit and gunit!=' '.join(x[2:]):
                 fail+='\n  Genome titers must all have the same unit!'
             elif read=='etit' and eunit and eunit!=' '.join(x[2:]):
@@ -903,16 +905,16 @@
     m=[k for k in s if 'mix' in k.lower()]
     if len(m)!=1:
         m=[]
         for q in s:
             a=q.replace('_','-').replace(',','-').split('-')
             b=[k.replace('_','-').replace(',','-').split('-') for k in s if k!=q]
             for k in b:
-                for m in a:
-                    if m in k:
+                for n in a:
+                    if n in k:
                         break
                 else:
                     continue
                 break
             else:
                 m.append(q)
     if len(m)==1:
@@ -924,26 +926,26 @@
     f.write('# VARIANTS:\n\n'+'\n'.join(v)+'\n\n')
     f.write('# VARIANT MIX:\n\n'+mix+'\n\n')
     f.write('# THRESHOLD:\nInstructions: Threshold in % of equimolar distribution in the variant mix. Variants with a frequency lower than the threshold in the mix will be excluded from analysis.\n\n10\n\n')
     f.write('# SAMPLES:\n\n'+'\n'.join(s)+'\n\n')
     dna=[k for k in s if any([n in [m.lower() for m in k.replace('_','-').replace(',','-').split('-')] for n in ('dna','gdna','genome')])]
     rna=[k for k in s if any([n in [m.lower() for m in k.replace('_','-').replace(',','-').split('-')] for n in ('rna','cdna','expression')])]
     other=[k for k in s if (k not in dna and k not in rna)]
-    f.write('# GLOBAL GENOME TITERS:\nInstructions: Enter the names of all samples for which you have a global variant genome relative to host genome titer, one per line, with the name followed by the titer value and the unit, separated by tabs or blank spaces. The unit must be the same for all samples, and can be entered once (will be applied to all other samples) or more.\n\n'+'\t\tvg/cell\n'.join(dna)+'\t\tvg/cell\n\n')
-    f.write('# GLOBAL EXPRESSION TITERS:\nInstructions: Enter the names of all samples for which you have a global variant expression relative to host housekeeping gene expression level titer, one per line, with the name followed by the titer value and the unit, separated by tabs or blank spaces. The unit must be the same for all samples, and can be entered once (will be applied to all other samples) or more.\n\n'+'\t\t% control\n'.join(rna)+'\t\t% control\n\n')
+    f.write('# GLOBAL GENOME TITERS:\nInstructions: Enter the names of all samples for which you have a global variant genome relative to host genome titer, one per line, with the name followed by the titer value and the unit, separated by tabs or blank spaces. The unit must be the same for all samples, and can be entered once (will be applied to all other samples) or more. If no genome titers are available, enter "None" or delete the section from the configuration file.\n\n'+'\t\tvg/cell\n'.join(dna)+'\t\tvg/cell\n\n')
+    f.write('# GLOBAL EXPRESSION TITERS:\nInstructions: Enter the names of all samples for which you have a global variant expression relative to host housekeeping gene expression level titer, one per line, with the name followed by the titer value and the unit, separated by tabs or blank spaces. The unit must be the same for all samples, and can be entered once (will be applied to all other samples) or more. If no expression titers are available, enter "None" or delete the section from the configuration file.\n\n'+'\t\t% control\n'.join(rna)+'\t\t% control\n\n')
     f.write('# COMBINE BIOLOGICAL REPLICATES:\nInstructions: Each group of lines separated by empty lines will be a separate plot. Multiple samples within lines will be averaged. First line in each group is the figure title followed by sample identifiers (separated by space or tab). Each subsequent line: label followed by sample name(s) separated by tabs or spaces.\n\n')
     for n in (dna,rna,other):
         if not n:
             continue
         p=[k.replace('_','-').replace(',','-').split('-') for k in n]
-        x=[[k[i] for i in range(len(k)) if len(set([m[i] for m in p]))>1] for k in p]
-        w=[[k[i] for i in range(len(k)) if all([m[i].isdigit() for m in p])] for k in p]
+        x=[[k[-i] for i in range(len(k)) if len(set([m[max(-i,-len(m))] for m in p]))>1] for k in p]
+        w=[[k[-i] for i in range(len(k)) if all([m[max(-i,-len(m))].isdigit() for m in p])] for k in p]
         q=min([len(k) for k in w])
         if not q:
-            w=[[k[i] for i in range(len(k)) if all([m[i][-1].isdigit() for m in x])] for k in x]
+            w=[[k[-i] for i in range(len(k)) if all([m[max(-i,-len(m))][-1].isdigit() for m in x])] for k in x]
             q=min([len(k) for k in w])
         if q:
             w=[k[-1] for k in w]
         x=[[x[i][j] for j in range(len(x[i])) if x[i][j]!=w[i]] for i in range(len(x))]
         y=''
         if n==dna:
             y='Genome'
@@ -952,14 +954,16 @@
         z=sorted(set(['-'.join(k) for k in x]))
         if w[0]:
             w=sorted(set(w))
         else:
             w=[]
         if len(w)==x.count(z[0].split('-')):
             y+='\t'+'\t'.join(w)
+        if not y:
+            continue
         f.write(y+'\n')
         for m in z:
             f.write(m+'\t'+'\t'.join(sorted([n[i] for i in range(len(n)) if all([q in p[i] for q in m.split('-')])]))+'\n')
         f.write('\n')
     f.write('# X-AXIS:\nInstructions: either variants or samples can be on the x-axis.\n\nVariants\n\n')
     f.write('# SHOW INDIVIDUAL DATA POINTS:\nInstructions: on bar plots of combined data, superimpose individual data points (points / circles / stars / none).\n\npoints\n\n')
     f.write('# SHOW ERROR BARS:\nInstructions: display error bars on bar plots of combined data (Range / Standard error / Standard deviation / None).\n\nNone\n\n')
@@ -967,34 +971,34 @@
     f.write('# HEAT MAP COLOR MAPS:\nInstructions: list color maps to be used in heat maps, one per line for global variant enrichment and biodistribution (default or leave empty for default color maps, or any compatible color map such as seismic, bwr, hot, RdBu or their reversed versions with _r appended).\n\ndefault\ndefault\n\n')
     f.write('=== END OF CONFIGURATION FILE ===')
     f.close()
     print('\n  Edit the file '+fname+' before running '+script+' '+args.command+' again !\n\n')
 
 def countconf(fname,args):
     z=script+' '+args.command
-    f,dirname,rfiles=dbl.conf_start(fname,z)
-    f.write('# PROJECT NAME\nInstructions: Project name to be used as prefix in output file name.\n\n')
-    f.write(dirname+'\n\n')
-    f.write('# READ FILE(S)\nInstructions: List prefix (to be used as sample name in output files if multiple read files are present, will be created automatically if missing) and read file names, one file (single-end or merged paired-end data) per line, separated by space or tab.\n\n')
+    content,dirname,rfiles=dbl.conf_start(z)
+    content+='# PROJECT NAME\nInstructions: Project name to be used as prefix in output file name.\n\n'
+    content+=dirname+'\n\n'
+    content+='# READ FILE(S)\nInstructions: List prefix (to be used as sample name in output files if multiple read files are present, will be created automatically if missing) and read file names, one file (single-end or merged paired-end data) per line, separated by space or tab.\n\n'
     y=[k for k in rfiles if k.count(' ')==2]
     x=[k for k in rfiles if k not in y]
     if not x and y:
         print('\n  Only unmerged paired-end read files found in the current directory! Please merge before using '+script+'!\n')
         sys.exit()
-    f.write('\n'.join(x)+'\n\n')
-    f.write('# TEMPLATE SEQUENCE\nInstructions: Name of the file, in FASTA format, containing the PCR template sequence, with the barcode shown as a stretch of N. Alternatively, paste the sequence itself. Primer binding regions must be included.\n\n')
+    content+='\n'.join(x)+'\n\n'
+    content+='# TEMPLATE SEQUENCE\nInstructions: Name of the file, in FASTA format, containing the PCR template sequence, with the barcode shown as a stretch of N. Alternatively, paste the sequence itself. Primer binding regions must be included.\n\n'
     x=glob('*.f*a')
     y='\n'
     if len(x)==1:
         y=x[0]+2*y
-    f.write(y)
-    f.write("# PRIMERS/BARCODES\nInstructions: List all primers (name followed by sequence), whether barcoded or not, one per line (forward and reverse PCR primers used to amplify the template, as well as primers used to generate the template). Barcodes only (without primer sequence) can be entered instead, if no ambiguity. If no primer information is entered, the exact consensus read sequence must be entered in the template sequence section above, with all barcodes indicated by stretches of N, and barcodes should be grouped (each grpup surrounded by empty lines) by their corresponding region in the order the barcoded regions appear in the read sequence. Barcodes from the reverse strand need to be followed by a - sign (their reverse-complement will then be used).\n\n\n")
-    f.write("# DEFINITIONS\nInstructions: Each line contains a sample/variant name followed by one or more barcode name(s), separated by a space or tab. Barcodes from different regions indicate that the sample is defined by a combination of barcodes from those regions. Multiple barcodes from the same region are allowed and indicate that a sample/variant is represented by more than one barcoode. All primers/barcodes must have a different name. In case of more than one sample/conditions is defined by a barcode or barcode combination, use a separator (- or _ or ,) between them.\n\n\n")
-    f.write('# PROBE LENGTH\nInstructions: Minimum length in nt of sequences used as probes to locate barcodes (integer between 1 and 50.\n\n5\n\n')
-    dbl.conf_end(f,fname,z)
+    content+=y
+    content+="# PRIMERS/BARCODES\nInstructions: List all primers (name followed by sequence), whether barcoded or not, one per line (forward and reverse PCR primers used to amplify the template, as well as primers used to generate the template). Barcodes only (without primer sequence) can be entered instead, if no ambiguity. If no primer information is entered, the exact consensus read sequence must be entered in the template sequence section above, with all barcodes indicated by stretches of N, and barcodes should be grouped (each grpup surrounded by empty lines) by their corresponding region in the order the barcoded regions appear in the read sequence. Barcodes from the reverse strand need to be followed by a - sign (their reverse-complement will then be used).\n\n\n"
+    content+="# DEFINITIONS\nInstructions: Each line contains a sample/variant name followed by one or more barcode name(s), separated by a space or tab. Barcodes from different regions indicate that the sample is defined by a combination of barcodes from those regions. Multiple barcodes from the same region are allowed and indicate that a sample/variant is represented by more than one barcoode. All primers/barcodes must have a different name. In case of more than one sample/conditions is defined by a barcode or barcode combination, use a separator (- or _ or ,) between them.\n\n\n"
+    content+='# PROBE LENGTH\nInstructions: Minimum length in nt of sequences used as probes to locate barcodes (integer between 1 and 50.\n\n5\n\n'
+    dbl.conf_end(fname,content,z)
 
 def find_bc(l,templ,bcr,cl,ctempl,cbcr):
     X={}
     p=0
     ec=[0,0,0]
     for i in bcr:
         a=bcr[i][-3]
@@ -1027,17 +1031,17 @@
                 continue
         X={}
         break
     return X,p,ec
 
 def fb(l,templ,i,bcr):
     r=''
-    x=[k.start()+i-bcr[i][-3] for k in regex.finditer(templ[bcr[i][-3]:i],l,overlapped=True)]
+    x=[k.start()+i-bcr[i][-3] for k in regex.finditer(templ[bcr[i][-3]:i],l,overlapped=True)]### update !!!
     if x:
-        y=[k.start() for k in regex.finditer(templ[bcr[i][-2]:bcr[i][-1]],l,overlapped=True)]
+        y=[k.start() for k in regex.finditer(templ[bcr[i][-2]:bcr[i][-1]],l,overlapped=True)]### update !!!
         z=[(n,m) for n in x for m in y if m>n and m-n==bcr[i][0]]
         if z:
             if len(z)==1:
                 z=z[0]
             else:
                 q=min([abs(k[0]-i) for k in z])
                 w=[k for k in z if abs(k[0]-i)==q]
```

### Comparing `barseqcount-0.1.4/setup.py` & `barseqcount-0.1.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setuptools.setup(
     name="barseqcount",
-    version="0.1.4",
+    version="0.1.5",
     author="Damien Marsic",
     author_email="damien.marsic@aliyun.com",
     description="Analysis of DNA barcode sequencing experiments",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/damienmarsic/barseqcount",
     package_dir={'': 'barseqcount'},
```

### Comparing `barseqcount-0.1.4/tests/test_.py` & `barseqcount-0.1.5/tests/test_.py`

 * *Files identical despite different names*

