# Comparing `tmp/fastq_preprocessor-2022.3.25.tar.gz` & `tmp/fastq_preprocessor-2023.5.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/jespinoz/Google/Algorithms/Packages/fastq_preprocessor/dist/tmp78ptsp3y/fastq_preprocessor-2022.3.25.tar", last modified: Fri Mar 25 19:09:55 2022, max compression
+gzip compressed data, was "fastq_preprocessor-2023.5.16.tar", last modified: Tue May 16 05:40:16 2023, max compression
```

## Comparing `fastq_preprocessor-2022.3.25.tar` & `fastq_preprocessor-2023.5.16.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 jespinoz  (3456) tigr        (63)        0 2022-03-25 19:09:55.709998 fastq_preprocessor-2022.3.25/
--rwxrwxr-x   0 jespinoz  (3456) tigr        (63)     1750 2022-01-13 21:42:58.000000 fastq_preprocessor-2022.3.25/LICENSE.txt
--rw-r--r--   0 jespinoz  (3456) tigr        (63)      151 2022-02-15 23:53:42.000000 fastq_preprocessor-2022.3.25/MANIFEST.in
--rw-r--r--   0 jespinoz  (3456) tigr        (63)      330 2022-03-25 19:09:55.709704 fastq_preprocessor-2022.3.25/PKG-INFO
--rwxrwxr-x   0 jespinoz  (3456) tigr        (63)    16608 2022-03-25 19:06:25.000000 fastq_preprocessor-2022.3.25/README.md
-drwxr-xr-x   0 jespinoz  (3456) tigr        (63)        0 2022-03-25 19:09:55.701131 fastq_preprocessor-2022.3.25/bin/
--rwxrwxr-x   0 jespinoz  (3456) tigr        (63)    22921 2022-03-25 19:08:36.000000 fastq_preprocessor-2022.3.25/bin/fastq_preprocessor
-drwxr-xr-x   0 jespinoz  (3456) tigr        (63)        0 2022-03-25 19:09:55.703347 fastq_preprocessor-2022.3.25/fastq_preprocessor/
--rwxrwxr-x   0 jespinoz  (3456) tigr        (63)     2476 2022-03-25 19:08:25.000000 fastq_preprocessor-2022.3.25/fastq_preprocessor/__init__.py
--rwxrwxr-x   0 jespinoz  (3456) tigr        (63)    22921 2022-03-25 19:08:36.000000 fastq_preprocessor-2022.3.25/fastq_preprocessor/fastq_preprocessor.py
-drwxr-xr-x   0 jespinoz  (3456) tigr        (63)        0 2022-03-25 19:09:55.709288 fastq_preprocessor-2022.3.25/fastq_preprocessor.egg-info/
--rw-r--r--   0 jespinoz  (3456) tigr        (63)      330 2022-03-25 19:09:55.000000 fastq_preprocessor-2022.3.25/fastq_preprocessor.egg-info/PKG-INFO
--rw-r--r--   0 jespinoz  (3456) tigr        (63)      346 2022-03-25 19:09:55.000000 fastq_preprocessor-2022.3.25/fastq_preprocessor.egg-info/SOURCES.txt
--rw-r--r--   0 jespinoz  (3456) tigr        (63)        1 2022-03-25 19:09:55.000000 fastq_preprocessor-2022.3.25/fastq_preprocessor.egg-info/dependency_links.txt
--rw-r--r--   0 jespinoz  (3456) tigr        (63)       80 2022-03-25 19:09:55.000000 fastq_preprocessor-2022.3.25/fastq_preprocessor.egg-info/requires.txt
--rw-r--r--   0 jespinoz  (3456) tigr        (63)       19 2022-03-25 19:09:55.000000 fastq_preprocessor-2022.3.25/fastq_preprocessor.egg-info/top_level.txt
--rw-r--r--   0 jespinoz  (3456) tigr        (63)       38 2022-03-25 19:09:55.710094 fastq_preprocessor-2022.3.25/setup.cfg
--rwxrwxr-x   0 jespinoz  (3456) tigr        (63)      943 2022-01-21 04:03:34.000000 fastq_preprocessor-2022.3.25/setup.py
+drwxr-xr-x   0 jespinoz  (3456) staff       (20)        0 2023-05-16 05:40:16.843977 fastq_preprocessor-2023.5.16/
+-rw-------   0 jespinoz  (3456) staff       (20)     1750 2020-03-27 17:41:41.000000 fastq_preprocessor-2023.5.16/LICENSE.txt
+-rw-------   0 jespinoz  (3456) staff       (20)      151 2022-02-15 23:53:42.000000 fastq_preprocessor-2023.5.16/MANIFEST.in
+-rw-r--r--   0 jespinoz  (3456) staff       (20)      302 2023-05-16 05:40:16.843531 fastq_preprocessor-2023.5.16/PKG-INFO
+-rw-------   0 jespinoz  (3456) staff       (20)    16607 2022-04-02 18:37:37.000000 fastq_preprocessor-2023.5.16/README.md
+drwxr-xr-x   0 jespinoz  (3456) staff       (20)        0 2023-05-16 05:40:16.839457 fastq_preprocessor-2023.5.16/bin/
+-rw-------   0 jespinoz  (3456) staff       (20)    23003 2023-05-16 05:37:29.000000 fastq_preprocessor-2023.5.16/bin/fastq_preprocessor
+drwxr-xr-x   0 jespinoz  (3456) staff       (20)        0 2023-05-16 05:40:16.840430 fastq_preprocessor-2023.5.16/fastq_preprocessor/
+-rw-------   0 jespinoz  (3456) staff       (20)     2476 2023-05-16 05:36:48.000000 fastq_preprocessor-2023.5.16/fastq_preprocessor/__init__.py
+-rw-------   0 jespinoz  (3456) staff       (20)    23003 2023-05-16 05:36:14.000000 fastq_preprocessor-2023.5.16/fastq_preprocessor/fastq_preprocessor.py
+drwxr-xr-x   0 jespinoz  (3456) staff       (20)        0 2023-05-16 05:40:16.843003 fastq_preprocessor-2023.5.16/fastq_preprocessor.egg-info/
+-rw-------   0 jespinoz  (3456) staff       (20)      302 2023-05-16 05:40:16.000000 fastq_preprocessor-2023.5.16/fastq_preprocessor.egg-info/PKG-INFO
+-rw-------   0 jespinoz  (3456) staff       (20)      346 2023-05-16 05:40:16.000000 fastq_preprocessor-2023.5.16/fastq_preprocessor.egg-info/SOURCES.txt
+-rw-------   0 jespinoz  (3456) staff       (20)        1 2023-05-16 05:40:16.000000 fastq_preprocessor-2023.5.16/fastq_preprocessor.egg-info/dependency_links.txt
+-rw-------   0 jespinoz  (3456) staff       (20)       80 2023-05-16 05:40:16.000000 fastq_preprocessor-2023.5.16/fastq_preprocessor.egg-info/requires.txt
+-rw-------   0 jespinoz  (3456) staff       (20)       19 2023-05-16 05:40:16.000000 fastq_preprocessor-2023.5.16/fastq_preprocessor.egg-info/top_level.txt
+-rw-r--r--   0 jespinoz  (3456) staff       (20)       38 2023-05-16 05:40:16.844250 fastq_preprocessor-2023.5.16/setup.cfg
+-rw-------   0 jespinoz  (3456) staff       (20)      943 2023-05-16 00:08:07.000000 fastq_preprocessor-2023.5.16/setup.py
```

### Comparing `fastq_preprocessor-2022.3.25/LICENSE.txt` & `fastq_preprocessor-2023.5.16/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fastq_preprocessor-2022.3.25/README.md` & `fastq_preprocessor-2023.5.16/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 `__contact__ = "jespinoz@jcvi.org, jol.espinoz@gmail.com"`
 
 `__developmental__ = True`
 
 `__license__ = "BSD-3"`
 
-`__version__ = "2022.1.13"`
+`__version__ = "2022.4.2"`
 
 #### Dependencies: 
 
 ##### Bioinformatics software:
 * bbmap
 * fastp
 * seqkit
```

### Comparing `fastq_preprocessor-2022.3.25/bin/fastq_preprocessor` & `fastq_preprocessor-2023.5.16/bin/fastq_preprocessor`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # Soothsayer Ecosystem
 from genopype import *
 from soothsayer_utils import *
 
 pd.options.display.max_colwidth = 100
 
 __program__ = os.path.split(sys.argv[0])[-1]
-__version__ = "2022.3.25"
+__version__ = "2023.5.16"
 
 # .............................................................................
 # Primordial
 # .............................................................................
 # Kneaddata
 def get_fastp_cmd(input_filepaths, output_filepaths, output_directory, directories, opts):
     os.environ["TMPDIR"] = directories["tmp"]
@@ -52,15 +52,15 @@
     "stats",
     "-T",
     "-j {}".format(opts.n_jobs),
     input_filepaths[0],
     input_filepaths[1],
     os.path.join(output_directory, "trimmed_1.fastq.gz"),
     os.path.join(output_directory, "trimmed_2.fastq.gz"),
-    os.path.join(output_directory, "trimmed_singletons.fastq.gz"),
+    # os.path.join(output_directory, "trimmed_singletons.fastq.gz"),
     ">",
     os.path.join(output_directory, "seqkit_stats.tsv"),
     ")",
     ]
     return cmd
 
 # Bowtie2
@@ -71,16 +71,16 @@
     "(",
     os.environ["bowtie2"],
     "-x {}".format(opts.contamination_index),
     "-p {}".format(opts.n_jobs),
     "-1 {}".format(input_filepaths[0]),
     "-2 {}".format(input_filepaths[1]),
     "--seed {}".format(opts.random_state),
-    "--un-gz {}".format(os.path.join(output_directory, "cleaned_singletons.fastq.gz")), #write unpaired reads that didn't align to <path>
-    "--al-gz {}".format(os.path.join(output_directory, "contaminated_singletons.fastq.gz")), #write unpaired reads that aligned at least once to <path>
+    # "--un-gz {}".format(os.path.join(output_directory, "cleaned_singletons.fastq.gz")), #write unpaired reads that didn't align to <path>
+    # "--al-gz {}".format(os.path.join(output_directory, "contaminated_singletons.fastq.gz")), #write unpaired reads that aligned at least once to <path>
     "--un-conc {}".format(os.path.join(output_directory, "TMP__cleaned_%.fastq")), #write pairs that didn't align concordantly to <path>
     "--al-conc {}".format(os.path.join(output_directory, "TMP__contaminated_%.fastq")),#write pairs that aligned concordantly at least once to <path>
     # "--met-file {}".format(os.path.join(output_directory, "bowtie2_metrics.txt")),
     opts.bowtie2_options,
     ">",
     "/dev/null",
     ")",
@@ -147,14 +147,15 @@
             "(",
         os.environ["bbduk.sh"],
         "zl=1", # Most likely will delete these files
         "overwrite=t",
         "threads={}".format(opts.n_jobs),
         "in1={}".format(input_filepaths[0]),
         "in2={}".format(input_filepaths[1]),
+        "ref={}".format(opts.kmer_database),
         # "refstats={}".format(os.path.join(output_directory, "bbduk_refstats.txt")),
         # "stats={}".format(os.path.join(output_directory, "bbduk_stats.txt")),
         "k={}".format(opts.kmer_size),
         "minlen={}".format(opts.minimum_read_length),
         "out1={}".format(os.path.join(output_directory, "non-kmer_hits_1.fastq.gz")),
         "out2={}".format(os.path.join(output_directory, "non-kmer_hits_2.fastq.gz")),
         "outm1={}".format(os.path.join(output_directory, "kmer_hits_1.fastq.gz")),
@@ -201,19 +202,20 @@
 python -c "import glob, pandas as pd; pd.concat(map(lambda fp: pd.read_csv(fp, sep='\t', index_col=0), glob.glob('{}')), axis=0).to_csv('{}', sep='\t')"
 """.format(
             os.path.join(directories["intermediate"],"*/seqkit_stats.tsv"),
             os.path.join(output_directory,"seqkit_stats.concatenated.tsv"),
             ),
         ]
 
-    for filepath in input_filepaths:
-        cmd += [ 
-            "ln -f -s {} {}".format(os.path.realpath(filepath), output_directory),
-            "&&",
-        ]
+    cmd += [
+    "DST={}; (for SRC in {}; do SRC=$(realpath --relative-to $DST $SRC); ln -sf $SRC $DST; done)".format(
+        output_directory,
+        " ".join(input_filepaths), 
+        )
+    ]
         
 
     return cmd[:-1]
 
 # ============
 # Run Pipeline
 # ============
```

### Comparing `fastq_preprocessor-2022.3.25/fastq_preprocessor/__init__.py` & `fastq_preprocessor-2023.5.16/fastq_preprocessor/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 #
 # THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 #
 # =======
 # Version
 # =======
-__version__= "2022.3.25"
+__version__= "2023.5.16"
 __author__ = "Josh L. Espinoza"
 __email__ = "jespinoz@jcvi.org, jol.espinoz@gmail.com"
 __url__ = "https://github.com/jolespin/fastq_preprocessor"
 __cite__ = "https://github.com/jolespin/fastq_preprocessor"
 __license__ = "BSD-3"
 __developmental__ = True
 __all__ = []
```

### Comparing `fastq_preprocessor-2022.3.25/fastq_preprocessor/fastq_preprocessor.py` & `fastq_preprocessor-2023.5.16/fastq_preprocessor/fastq_preprocessor.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # Soothsayer Ecosystem
 from genopype import *
 from soothsayer_utils import *
 
 pd.options.display.max_colwidth = 100
 
 __program__ = os.path.split(sys.argv[0])[-1]
-__version__ = "2022.3.25"
+__version__ = "2023.5.16"
 
 # .............................................................................
 # Primordial
 # .............................................................................
 # Kneaddata
 def get_fastp_cmd(input_filepaths, output_filepaths, output_directory, directories, opts):
     os.environ["TMPDIR"] = directories["tmp"]
@@ -52,15 +52,15 @@
     "stats",
     "-T",
     "-j {}".format(opts.n_jobs),
     input_filepaths[0],
     input_filepaths[1],
     os.path.join(output_directory, "trimmed_1.fastq.gz"),
     os.path.join(output_directory, "trimmed_2.fastq.gz"),
-    os.path.join(output_directory, "trimmed_singletons.fastq.gz"),
+    # os.path.join(output_directory, "trimmed_singletons.fastq.gz"),
     ">",
     os.path.join(output_directory, "seqkit_stats.tsv"),
     ")",
     ]
     return cmd
 
 # Bowtie2
@@ -71,16 +71,16 @@
     "(",
     os.environ["bowtie2"],
     "-x {}".format(opts.contamination_index),
     "-p {}".format(opts.n_jobs),
     "-1 {}".format(input_filepaths[0]),
     "-2 {}".format(input_filepaths[1]),
     "--seed {}".format(opts.random_state),
-    "--un-gz {}".format(os.path.join(output_directory, "cleaned_singletons.fastq.gz")), #write unpaired reads that didn't align to <path>
-    "--al-gz {}".format(os.path.join(output_directory, "contaminated_singletons.fastq.gz")), #write unpaired reads that aligned at least once to <path>
+    # "--un-gz {}".format(os.path.join(output_directory, "cleaned_singletons.fastq.gz")), #write unpaired reads that didn't align to <path>
+    # "--al-gz {}".format(os.path.join(output_directory, "contaminated_singletons.fastq.gz")), #write unpaired reads that aligned at least once to <path>
     "--un-conc {}".format(os.path.join(output_directory, "TMP__cleaned_%.fastq")), #write pairs that didn't align concordantly to <path>
     "--al-conc {}".format(os.path.join(output_directory, "TMP__contaminated_%.fastq")),#write pairs that aligned concordantly at least once to <path>
     # "--met-file {}".format(os.path.join(output_directory, "bowtie2_metrics.txt")),
     opts.bowtie2_options,
     ">",
     "/dev/null",
     ")",
@@ -147,14 +147,15 @@
             "(",
         os.environ["bbduk.sh"],
         "zl=1", # Most likely will delete these files
         "overwrite=t",
         "threads={}".format(opts.n_jobs),
         "in1={}".format(input_filepaths[0]),
         "in2={}".format(input_filepaths[1]),
+        "ref={}".format(opts.kmer_database),
         # "refstats={}".format(os.path.join(output_directory, "bbduk_refstats.txt")),
         # "stats={}".format(os.path.join(output_directory, "bbduk_stats.txt")),
         "k={}".format(opts.kmer_size),
         "minlen={}".format(opts.minimum_read_length),
         "out1={}".format(os.path.join(output_directory, "non-kmer_hits_1.fastq.gz")),
         "out2={}".format(os.path.join(output_directory, "non-kmer_hits_2.fastq.gz")),
         "outm1={}".format(os.path.join(output_directory, "kmer_hits_1.fastq.gz")),
@@ -201,19 +202,20 @@
 python -c "import glob, pandas as pd; pd.concat(map(lambda fp: pd.read_csv(fp, sep='\t', index_col=0), glob.glob('{}')), axis=0).to_csv('{}', sep='\t')"
 """.format(
             os.path.join(directories["intermediate"],"*/seqkit_stats.tsv"),
             os.path.join(output_directory,"seqkit_stats.concatenated.tsv"),
             ),
         ]
 
-    for filepath in input_filepaths:
-        cmd += [ 
-            "ln -f -s {} {}".format(os.path.realpath(filepath), output_directory),
-            "&&",
-        ]
+    cmd += [
+    "DST={}; (for SRC in {}; do SRC=$(realpath --relative-to $DST $SRC); ln -sf $SRC $DST; done)".format(
+        output_directory,
+        " ".join(input_filepaths), 
+        )
+    ]
         
 
     return cmd[:-1]
 
 # ============
 # Run Pipeline
 # ============
```

### Comparing `fastq_preprocessor-2022.3.25/setup.py` & `fastq_preprocessor-2023.5.16/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,16 +14,16 @@
       description='Fast short read fastq preprocessor with optional contamination removal',
       url='https://github.com/jolespin/fastq_preprocessor',
       author='Josh L. Espinoza',
       author_email='jespinoz@jcvi.org',
       license='BSD-3',
       packages=["fastq_preprocessor"],
       install_requires=[
-      "genopype >=2020.3.27",
-      "soothsayer_utils >=2022.1.19",
+      "genopype >=2023.4.13",
+      "soothsayer_utils >=2022.6.24",
       "pandas >=0.24",
       "numpy",
       "tqdm",
       "scandir",
       ],
     include_package_data=True,
      scripts=["bin/fastq_preprocessor"],
```

