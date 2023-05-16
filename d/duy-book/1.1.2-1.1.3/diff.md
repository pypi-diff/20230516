# Comparing `tmp/duy-book-1.1.2.tar.gz` & `tmp/duy-book-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duy-book-1.1.2.tar", last modified: Tue May 16 03:56:18 2023, max compression
+gzip compressed data, was "duy-book-1.1.3.tar", last modified: Tue May 16 04:04:34 2023, max compression
```

## Comparing `duy-book-1.1.2.tar` & `duy-book-1.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 03:56:18.377194 duy-book-1.1.2/
--rw-r--r--   0 root         (0) root         (0)     1074 2023-05-16 03:56:09.000000 duy-book-1.1.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)      656 2023-05-16 03:56:18.377194 duy-book-1.1.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      170 2023-05-16 03:56:09.000000 duy-book-1.1.2/README.md
--rw-r--r--   0 root         (0) root         (0)      104 2023-05-16 03:56:09.000000 duy-book-1.1.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      611 2023-05-16 03:56:18.378194 duy-book-1.1.2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 03:56:18.373193 duy-book-1.1.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 03:56:18.376194 duy-book-1.1.2/src/duy_book/
--rw-r--r--   0 root         (0) root         (0)      265 2023-05-16 03:56:09.000000 duy-book-1.1.2/src/duy_book/__init__.py
--rw-r--r--   0 root         (0) root         (0)      431 2023-05-16 03:56:09.000000 duy-book-1.1.2/src/duy_book/colab.py
--rw-r--r--   0 root         (0) root         (0)      320 2023-05-16 03:56:09.000000 duy-book-1.1.2/src/duy_book/cudaset.py
--rw-r--r--   0 root         (0) root         (0)     2456 2023-05-16 03:56:09.000000 duy-book-1.1.2/src/duy_book/module.py
--rw-r--r--   0 root         (0) root         (0)      151 2023-05-16 03:56:09.000000 duy-book-1.1.2/src/duy_book/random_split.py
--rw-r--r--   0 root         (0) root         (0)      238 2023-05-16 03:56:09.000000 duy-book-1.1.2/src/duy_book/ratio_split.py
--rw-r--r--   0 root         (0) root         (0)      201 2023-05-16 03:56:09.000000 duy-book-1.1.2/src/duy_book/tqdn.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 03:56:18.377194 duy-book-1.1.2/src/duy_book.egg-info/
--rw-r--r--   0 root         (0) root         (0)      656 2023-05-16 03:56:18.000000 duy-book-1.1.2/src/duy_book.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      358 2023-05-16 03:56:18.000000 duy-book-1.1.2/src/duy_book.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 03:56:18.000000 duy-book-1.1.2/src/duy_book.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-05-16 03:56:18.000000 duy-book-1.1.2/src/duy_book.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 04:04:34.286638 duy-book-1.1.3/
+-rw-r--r--   0 root         (0) root         (0)     1074 2023-05-16 04:04:20.000000 duy-book-1.1.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      656 2023-05-16 04:04:34.286638 duy-book-1.1.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      170 2023-05-16 04:04:20.000000 duy-book-1.1.3/README.md
+-rw-r--r--   0 root         (0) root         (0)      104 2023-05-16 04:04:20.000000 duy-book-1.1.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      611 2023-05-16 04:04:34.287638 duy-book-1.1.3/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 04:04:34.281638 duy-book-1.1.3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 04:04:34.284638 duy-book-1.1.3/src/duy_book/
+-rw-r--r--   0 root         (0) root         (0)      265 2023-05-16 04:04:20.000000 duy-book-1.1.3/src/duy_book/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      431 2023-05-16 04:04:20.000000 duy-book-1.1.3/src/duy_book/colab.py
+-rw-r--r--   0 root         (0) root         (0)      320 2023-05-16 04:04:20.000000 duy-book-1.1.3/src/duy_book/cudaset.py
+-rw-r--r--   0 root         (0) root         (0)     2488 2023-05-16 04:04:20.000000 duy-book-1.1.3/src/duy_book/module.py
+-rw-r--r--   0 root         (0) root         (0)      151 2023-05-16 04:04:20.000000 duy-book-1.1.3/src/duy_book/random_split.py
+-rw-r--r--   0 root         (0) root         (0)      238 2023-05-16 04:04:20.000000 duy-book-1.1.3/src/duy_book/ratio_split.py
+-rw-r--r--   0 root         (0) root         (0)      201 2023-05-16 04:04:20.000000 duy-book-1.1.3/src/duy_book/tqdn.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 04:04:34.285638 duy-book-1.1.3/src/duy_book.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      656 2023-05-16 04:04:33.000000 duy-book-1.1.3/src/duy_book.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      358 2023-05-16 04:04:33.000000 duy-book-1.1.3/src/duy_book.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 04:04:33.000000 duy-book-1.1.3/src/duy_book.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-05-16 04:04:33.000000 duy-book-1.1.3/src/duy_book.egg-info/top_level.txt
```

### Comparing `duy-book-1.1.2/LICENSE` & `duy-book-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `duy-book-1.1.2/PKG-INFO` & `duy-book-1.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duy-book
-Version: 1.1.2
+Version: 1.1.3
 Summary: A small example package
 Home-page: https://github.com/pypa/sampleproject
 Author: Duy_abu
 Author-email: author@example.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `duy-book-1.1.2/setup.cfg` & `duy-book-1.1.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = duy-book
-version = 1.1.2
+version = 1.1.3
 author = Duy_abu
 author_email = author@example.com
 description = A small example package
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/pypa/sampleproject
 project_urls =
```

### Comparing `duy-book-1.1.2/src/duy_book/module.py` & `duy-book-1.1.3/src/duy_book/module.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import torch
 import torch.nn as nn
 import torch.optim as optim
 import torch.nn.functional as F
 import torch.optim.lr_scheduler as sched
 from torchsummary import summary
+import matplotlib.pyplot as plt
 from tqdm.notebook import tqdm
 from .colab import ColabOutput
 from .tqdn import tqdn
 
 class Module(nn.Module):
   def forward(self, input):
     return self.module.forward(input)
```

### Comparing `duy-book-1.1.2/src/duy_book.egg-info/PKG-INFO` & `duy-book-1.1.3/src/duy_book.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duy-book
-Version: 1.1.2
+Version: 1.1.3
 Summary: A small example package
 Home-page: https://github.com/pypa/sampleproject
 Author: Duy_abu
 Author-email: author@example.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

