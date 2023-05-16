# Comparing `tmp/genopype-2023.4.13.tar.gz` & `tmp/genopype-2023.5.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genopype-2023.4.13.tar", last modified: Fri Apr 14 00:02:36 2023, max compression
+gzip compressed data, was "genopype-2023.5.15.tar", last modified: Tue May 16 04:17:12 2023, max compression
```

## Comparing `genopype-2023.4.13.tar` & `genopype-2023.5.15.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 jespinoz  (3456) staff       (20)        0 2023-04-14 00:02:36.920054 genopype-2023.4.13/
--rw-------   0 jespinoz  (3456) staff       (20)     1524 2023-03-22 04:17:10.000000 genopype-2023.4.13/LICENSE
--rw-------   0 jespinoz  (3456) staff       (20)     2023 2023-04-13 20:32:03.000000 genopype-2023.4.13/LICENSE.txt
--rw-------   0 jespinoz  (3456) staff       (20)      193 2023-04-13 20:32:03.000000 genopype-2023.4.13/MANIFEST.in
--rw-r--r--   0 jespinoz  (3456) staff       (20)      278 2023-04-14 00:02:36.919658 genopype-2023.4.13/PKG-INFO
--rw-------   0 jespinoz  (3456) staff       (20)     7261 2023-04-13 20:32:03.000000 genopype-2023.4.13/README.md
-drwxr-xr-x   0 jespinoz  (3456) staff       (20)        0 2023-04-14 00:02:36.916243 genopype-2023.4.13/genopype/
--rw-------   0 jespinoz  (3456) staff       (20)     2769 2023-04-14 00:01:29.000000 genopype-2023.4.13/genopype/__init__.py
--rw-------   0 jespinoz  (3456) staff       (20)    38712 2023-04-14 00:00:38.000000 genopype-2023.4.13/genopype/genopype.py
-drwxr-xr-x   0 jespinoz  (3456) staff       (20)        0 2023-04-14 00:02:36.919114 genopype-2023.4.13/genopype.egg-info/
--rw-------   0 jespinoz  (3456) staff       (20)      278 2023-04-14 00:02:36.000000 genopype-2023.4.13/genopype.egg-info/PKG-INFO
--rw-------   0 jespinoz  (3456) staff       (20)      251 2023-04-14 00:02:36.000000 genopype-2023.4.13/genopype.egg-info/SOURCES.txt
--rw-------   0 jespinoz  (3456) staff       (20)        1 2023-04-14 00:02:36.000000 genopype-2023.4.13/genopype.egg-info/dependency_links.txt
--rw-------   0 jespinoz  (3456) staff       (20)       34 2023-04-14 00:02:36.000000 genopype-2023.4.13/genopype.egg-info/requires.txt
--rw-------   0 jespinoz  (3456) staff       (20)        9 2023-04-14 00:02:36.000000 genopype-2023.4.13/genopype.egg-info/top_level.txt
--rw-r--r--   0 jespinoz  (3456) staff       (20)       38 2023-04-14 00:02:36.920177 genopype-2023.4.13/setup.cfg
--rw-------   0 jespinoz  (3456) staff       (20)      718 2023-04-13 20:32:03.000000 genopype-2023.4.13/setup.py
+drwxr-xr-x   0 jespinoz  (3456) staff       (20)        0 2023-05-16 04:17:12.064089 genopype-2023.5.15/
+-rw-------   0 jespinoz  (3456) staff       (20)     1524 2023-04-14 00:08:41.000000 genopype-2023.5.15/LICENSE
+-rw-------   0 jespinoz  (3456) staff       (20)     2023 2023-04-14 00:08:45.000000 genopype-2023.5.15/LICENSE.txt
+-rw-------   0 jespinoz  (3456) staff       (20)      193 2023-04-14 00:08:45.000000 genopype-2023.5.15/MANIFEST.in
+-rw-r--r--   0 jespinoz  (3456) staff       (20)      278 2023-05-16 04:17:12.063711 genopype-2023.5.15/PKG-INFO
+-rw-------   0 jespinoz  (3456) staff       (20)     7261 2023-04-14 00:08:45.000000 genopype-2023.5.15/README.md
+drwxr-xr-x   0 jespinoz  (3456) staff       (20)        0 2023-05-16 04:17:12.060295 genopype-2023.5.15/genopype/
+-rw-------   0 jespinoz  (3456) staff       (20)     2769 2023-05-16 04:13:22.000000 genopype-2023.5.15/genopype/__init__.py
+-rw-------   0 jespinoz  (3456) staff       (20)    38720 2023-05-16 04:13:06.000000 genopype-2023.5.15/genopype/genopype.py
+drwxr-xr-x   0 jespinoz  (3456) staff       (20)        0 2023-05-16 04:17:12.063212 genopype-2023.5.15/genopype.egg-info/
+-rw-------   0 jespinoz  (3456) staff       (20)      278 2023-05-16 04:17:11.000000 genopype-2023.5.15/genopype.egg-info/PKG-INFO
+-rw-------   0 jespinoz  (3456) staff       (20)      251 2023-05-16 04:17:11.000000 genopype-2023.5.15/genopype.egg-info/SOURCES.txt
+-rw-------   0 jespinoz  (3456) staff       (20)        1 2023-05-16 04:17:11.000000 genopype-2023.5.15/genopype.egg-info/dependency_links.txt
+-rw-------   0 jespinoz  (3456) staff       (20)       34 2023-05-16 04:17:11.000000 genopype-2023.5.15/genopype.egg-info/requires.txt
+-rw-------   0 jespinoz  (3456) staff       (20)        9 2023-05-16 04:17:11.000000 genopype-2023.5.15/genopype.egg-info/top_level.txt
+-rw-r--r--   0 jespinoz  (3456) staff       (20)       38 2023-05-16 04:17:12.064215 genopype-2023.5.15/setup.cfg
+-rw-------   0 jespinoz  (3456) staff       (20)      718 2023-04-14 00:08:45.000000 genopype-2023.5.15/setup.py
```

### Comparing `genopype-2023.4.13/LICENSE` & `genopype-2023.5.15/LICENSE`

 * *Files identical despite different names*

### Comparing `genopype-2023.4.13/LICENSE.txt` & `genopype-2023.5.15/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `genopype-2023.4.13/README.md` & `genopype-2023.5.15/README.md`

 * *Files identical despite different names*

### Comparing `genopype-2023.4.13/genopype/__init__.py` & `genopype-2023.5.15/genopype/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 #
 # THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 #
 # =======
 # Version
 # =======
-__version__= "2023.4.13"
+__version__= "2023.5.15"
 __author__ = "Josh L. Espinoza"
 __email__ = "jespinoz@jcvi.org, jol.espinoz@gmail.com"
 __url__ = "https://github.com/jolespin/genopype"
 __cite__ = "https://github.com/jolespin/genopype"
 __license__ = "BSD-3"
 __developmental__ = True
 __all__ = ["Command","ExecutablePipeline","DisplayablePath", "get_directory_tree", "get_directory_size",  "check_filename", "format_filename", "create_directory", "validate_file_existence"]
```

### Comparing `genopype-2023.4.13/genopype/genopype.py` & `genopype-2023.5.15/genopype/genopype.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,21 +71,21 @@
         else:
             # path = os.path.realpath(path)
             paths_expanded.append(path)
     for path in paths_expanded:
         # Get the absolute path
         # path = os.path.realpath(path)
         # Get the path to the symlink target
-        if os.path.islink(path):
-            path = os.readlink(path)
+        # if os.path.islink(path):
+        #     path = os.readlink(path)
         assert os.path.exists(path), "The following path does not exist: {}".format(path)
         # original_path = None
         # symlink = None
-        if os.path.islink(path):
-            path = os.readlink(path)
+        # if os.path.islink(path):
+        #     path = os.readlink(path)
         if not os.path.isdir(path):
             size_bytes = os.path.getsize(path)
 
             if path not in whitelist_empty_files:
                 # print(path, whitelist_empty_files)
                 assert size_bytes >= minimum_filesize, "The following file appears to be empty ({} bytes): {}".format(size_bytes, path)
             else:
```

### Comparing `genopype-2023.4.13/setup.py` & `genopype-2023.5.15/setup.py`

 * *Files identical despite different names*

