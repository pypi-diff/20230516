# Comparing `tmp/al2var-0.0.6.tar.gz` & `tmp/al2var-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/hendrixj/Dropbox/subDrop/devel_al2var/forPypi/dist/.tmp-c9d70512/al2var-0.0.6.tar", last modified: Mon May 15 23:30:16 2023, max compression
+gzip compressed data, was "/Users/hendrixj/Dropbox/subDrop/devel_al2var/forPypi/dist/.tmp-03wv6wl9/al2var-0.0.7.tar", last modified: Tue May 16 15:38:11 2023, max compression
```

## Comparing `al2var-0.0.6.tar` & `al2var-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 hendrixj (1692218720) 1934156310        0 2023-05-15 23:30:16.918311 al2var-0.0.6/
--rw-r--r--   0 hendrixj (1692218720) 1934156310     1122 2022-10-08 19:49:45.000000 al2var-0.0.6/LICENSE
--rw-r--r--   0 hendrixj (1692218720) 1934156310       17 2022-10-10 23:15:11.000000 al2var-0.0.6/MANIFEST.in
--rw-r--r--   0 hendrixj (1692218720) 1934156310     7024 2023-05-15 23:30:16.918516 al2var-0.0.6/PKG-INFO
--rw-r--r--   0 hendrixj (1692218720) 1934156310     6499 2023-04-19 02:14:41.000000 al2var-0.0.6/README.md
-drwxr-xr-x   0 hendrixj (1692218720) 1934156310        0 2023-05-15 23:30:16.916538 al2var-0.0.6/al2var.egg-info/
--rw-r--r--   0 hendrixj (1692218720) 1934156310     7024 2023-05-15 23:30:16.000000 al2var-0.0.6/al2var.egg-info/PKG-INFO
--rw-r--r--   0 hendrixj (1692218720) 1934156310      179 2023-05-15 23:30:16.000000 al2var-0.0.6/al2var.egg-info/SOURCES.txt
--rw-r--r--   0 hendrixj (1692218720) 1934156310        1 2023-05-15 23:30:16.000000 al2var-0.0.6/al2var.egg-info/dependency_links.txt
--rw-r--r--   0 hendrixj (1692218720) 1934156310        1 2023-05-15 23:30:16.000000 al2var-0.0.6/al2var.egg-info/top_level.txt
-drwxr-xr-x   0 hendrixj (1692218720) 1934156310        0 2023-05-15 23:30:16.917192 al2var-0.0.6/bin/
--rw-r--r--   0 hendrixj (1692218720) 1934156310    17784 2023-04-19 02:27:23.000000 al2var-0.0.6/bin/al2var
--rw-r--r--   0 hendrixj (1692218720) 1934156310       38 2023-05-15 23:30:16.919144 al2var-0.0.6/setup.cfg
--rw-r--r--   0 hendrixj (1692218720) 1934156310      824 2023-05-15 23:28:59.000000 al2var-0.0.6/setup.py
+drwxr-xr-x   0 hendrixj (1692218720) 1934156310        0 2023-05-16 15:38:11.720065 al2var-0.0.7/
+-rw-r--r--   0 hendrixj (1692218720) 1934156310     1122 2022-10-08 19:49:45.000000 al2var-0.0.7/LICENSE
+-rw-r--r--   0 hendrixj (1692218720) 1934156310       17 2022-10-10 23:15:11.000000 al2var-0.0.7/MANIFEST.in
+-rw-r--r--   0 hendrixj (1692218720) 1934156310     7142 2023-05-16 15:38:11.720238 al2var-0.0.7/PKG-INFO
+-rw-r--r--   0 hendrixj (1692218720) 1934156310     6617 2023-05-16 15:02:20.000000 al2var-0.0.7/README.md
+drwxr-xr-x   0 hendrixj (1692218720) 1934156310        0 2023-05-16 15:38:11.718500 al2var-0.0.7/al2var.egg-info/
+-rw-r--r--   0 hendrixj (1692218720) 1934156310     7142 2023-05-16 15:38:11.000000 al2var-0.0.7/al2var.egg-info/PKG-INFO
+-rw-r--r--   0 hendrixj (1692218720) 1934156310      179 2023-05-16 15:38:11.000000 al2var-0.0.7/al2var.egg-info/SOURCES.txt
+-rw-r--r--   0 hendrixj (1692218720) 1934156310        1 2023-05-16 15:38:11.000000 al2var-0.0.7/al2var.egg-info/dependency_links.txt
+-rw-r--r--   0 hendrixj (1692218720) 1934156310        1 2023-05-16 15:38:11.000000 al2var-0.0.7/al2var.egg-info/top_level.txt
+drwxr-xr-x   0 hendrixj (1692218720) 1934156310        0 2023-05-16 15:38:11.718947 al2var-0.0.7/bin/
+-rw-r--r--   0 hendrixj (1692218720) 1934156310    17784 2023-04-19 02:27:23.000000 al2var-0.0.7/bin/al2var
+-rw-r--r--   0 hendrixj (1692218720) 1934156310       38 2023-05-16 15:38:11.720784 al2var-0.0.7/setup.cfg
+-rw-r--r--   0 hendrixj (1692218720) 1934156310      824 2023-05-16 15:36:18.000000 al2var-0.0.7/setup.py
```

### Comparing `al2var-0.0.6/LICENSE` & `al2var-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `al2var-0.0.6/PKG-INFO` & `al2var-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: al2var
-Version: 0.0.6
+Version: 0.0.7
 Summary: Identify and calculate find variant rate between a bacterial genome sequence and either paired-end reads or another genome sequence
 Home-page: https://github.com/jrhendrix/al2var
 Author: Jo Hendrix
 Author-email: jrhendrix36@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -38,20 +38,30 @@
 
 
 al2var was specifically tested with
 1. python v3.7.16, bcftools v1.9, samtools v1.6, bowtie2 v2.2.5, and minimap2 v2.21
 2. python v3.10.2, bcftools v1.14, samtools v1.14, bowtie2 v2.5.1, and minimap2 v2.24
 
 
+
+
 ### Installation
+
+It is recomended by not required to install al2var in a conda environment. 
+
+Creating a possible conda environment for al2var:
+```
+conda create -n al2var python=3.10.2 bcftools=1.14 samtools=1.14 bowtie2=2.5.1 minimap2=2.24
+```
+
 al2var is available on [PyPI](https://pypi.org/project/roprokka/) and can be installed using pip.
 
 ```pip install al2var```
 
-OR clone from GitHub repository. If accessing code from GitHub, it is recommended but not required to install dependencies in a conda environment.
+OR clone from GitHub repository.
 
 ## Output
 al2var will create a directory to organize all of the generated output in various subdirectories.
 
 * Subdirectory `vcf/` harbors two files. The file ending in `000.vcf` is a sorted `vcf` that contains a record for each position in the reference sequence regardless of whether the query sequence had the same or a different genotype. If using the minimap2 mode, the genotype column will reflect the genotype of the query sequence at the mapped position. If using the bowtie2 mode, the genotype will reflect the consensus of the reads that mapped to that given position. The second file ending in `var.vcf` contains only the variants between the reference and the query sequence or input reads.
 * `report.txt` file reports on three stats: the alignment rate of the query to the reference, the number of variants between the input, and the variant rate. The variant rate is calculated from the reference length and normalized to 100kb. 
 * Subdirectory `bam/` contains the alignment information in bam format. These files can be viewed in an interactive genome browser such as IGV. These files can be automatically deleted during runtime using the `--cleanup` flag.
```

### Comparing `al2var-0.0.6/README.md` & `al2var-0.0.7/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -24,20 +24,30 @@
 
 
 al2var was specifically tested with
 1. python v3.7.16, bcftools v1.9, samtools v1.6, bowtie2 v2.2.5, and minimap2 v2.21
 2. python v3.10.2, bcftools v1.14, samtools v1.14, bowtie2 v2.5.1, and minimap2 v2.24
 
 
+
+
 ### Installation
+
+It is recomended by not required to install al2var in a conda environment. 
+
+Creating a possible conda environment for al2var:
+```
+conda create -n al2var python=3.10.2 bcftools=1.14 samtools=1.14 bowtie2=2.5.1 minimap2=2.24
+```
+
 al2var is available on [PyPI](https://pypi.org/project/roprokka/) and can be installed using pip.
 
 ```pip install al2var```
 
-OR clone from GitHub repository. If accessing code from GitHub, it is recommended but not required to install dependencies in a conda environment.
+OR clone from GitHub repository.
 
 ## Output
 al2var will create a directory to organize all of the generated output in various subdirectories.
 
 * Subdirectory `vcf/` harbors two files. The file ending in `000.vcf` is a sorted `vcf` that contains a record for each position in the reference sequence regardless of whether the query sequence had the same or a different genotype. If using the minimap2 mode, the genotype column will reflect the genotype of the query sequence at the mapped position. If using the bowtie2 mode, the genotype will reflect the consensus of the reads that mapped to that given position. The second file ending in `var.vcf` contains only the variants between the reference and the query sequence or input reads.
 * `report.txt` file reports on three stats: the alignment rate of the query to the reference, the number of variants between the input, and the variant rate. The variant rate is calculated from the reference length and normalized to 100kb. 
 * Subdirectory `bam/` contains the alignment information in bam format. These files can be viewed in an interactive genome browser such as IGV. These files can be automatically deleted during runtime using the `--cleanup` flag.
```

### Comparing `al2var-0.0.6/al2var.egg-info/PKG-INFO` & `al2var-0.0.7/al2var.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: al2var
-Version: 0.0.6
+Version: 0.0.7
 Summary: Identify and calculate find variant rate between a bacterial genome sequence and either paired-end reads or another genome sequence
 Home-page: https://github.com/jrhendrix/al2var
 Author: Jo Hendrix
 Author-email: jrhendrix36@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -38,20 +38,30 @@
 
 
 al2var was specifically tested with
 1. python v3.7.16, bcftools v1.9, samtools v1.6, bowtie2 v2.2.5, and minimap2 v2.21
 2. python v3.10.2, bcftools v1.14, samtools v1.14, bowtie2 v2.5.1, and minimap2 v2.24
 
 
+
+
 ### Installation
+
+It is recomended by not required to install al2var in a conda environment. 
+
+Creating a possible conda environment for al2var:
+```
+conda create -n al2var python=3.10.2 bcftools=1.14 samtools=1.14 bowtie2=2.5.1 minimap2=2.24
+```
+
 al2var is available on [PyPI](https://pypi.org/project/roprokka/) and can be installed using pip.
 
 ```pip install al2var```
 
-OR clone from GitHub repository. If accessing code from GitHub, it is recommended but not required to install dependencies in a conda environment.
+OR clone from GitHub repository.
 
 ## Output
 al2var will create a directory to organize all of the generated output in various subdirectories.
 
 * Subdirectory `vcf/` harbors two files. The file ending in `000.vcf` is a sorted `vcf` that contains a record for each position in the reference sequence regardless of whether the query sequence had the same or a different genotype. If using the minimap2 mode, the genotype column will reflect the genotype of the query sequence at the mapped position. If using the bowtie2 mode, the genotype will reflect the consensus of the reads that mapped to that given position. The second file ending in `var.vcf` contains only the variants between the reference and the query sequence or input reads.
 * `report.txt` file reports on three stats: the alignment rate of the query to the reference, the number of variants between the input, and the variant rate. The variant rate is calculated from the reference length and normalized to 100kb. 
 * Subdirectory `bam/` contains the alignment information in bam format. These files can be viewed in an interactive genome browser such as IGV. These files can be automatically deleted during runtime using the `--cleanup` flag.
```

### Comparing `al2var-0.0.6/bin/al2var` & `al2var-0.0.7/bin/al2var`

 * *Files identical despite different names*

### Comparing `al2var-0.0.6/setup.py` & `al2var-0.0.7/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="al2var",
-    version="0.0.6",
+    version="0.0.7",
     author="Jo Hendrix",
     author_email="jrhendrix36@gmail.com",
     description="Identify and calculate find variant rate between a bacterial genome sequence and either paired-end reads or another genome sequence",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jrhendrix/al2var",
     scripts=['bin/al2var'],
```

