# Comparing `tmp/duy-book-1.1.0.tar.gz` & `tmp/duy-book-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duy-book-1.1.0.tar", last modified: Thu Mar  2 00:19:02 2023, max compression
+gzip compressed data, was "duy-book-1.1.2.tar", last modified: Tue May 16 03:56:18 2023, max compression
```

## Comparing `duy-book-1.1.0.tar` & `duy-book-1.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-02 00:19:02.786955 duy-book-1.1.0/
--rw-r--r--   0 root         (0) root         (0)     1074 2023-03-02 00:18:56.000000 duy-book-1.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      693 2023-03-02 00:19:02.786955 duy-book-1.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      170 2023-03-02 00:18:56.000000 duy-book-1.1.0/README.md
--rw-r--r--   0 root         (0) root         (0)      104 2023-03-02 00:18:56.000000 duy-book-1.1.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      611 2023-03-02 00:19:02.786955 duy-book-1.1.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-02 00:19:02.783955 duy-book-1.1.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-02 00:19:02.785955 duy-book-1.1.0/src/duy_book/
--rw-r--r--   0 root         (0) root         (0)      226 2023-03-02 00:18:56.000000 duy-book-1.1.0/src/duy_book/__init__.py
--rw-r--r--   0 root         (0) root         (0)      431 2023-03-02 00:18:56.000000 duy-book-1.1.0/src/duy_book/colab.py
--rw-r--r--   0 root         (0) root         (0)      320 2023-03-02 00:18:56.000000 duy-book-1.1.0/src/duy_book/cudaset.py
--rw-r--r--   0 root         (0) root         (0)     2219 2023-03-02 00:18:56.000000 duy-book-1.1.0/src/duy_book/module.py
--rw-r--r--   0 root         (0) root         (0)      151 2023-03-02 00:18:56.000000 duy-book-1.1.0/src/duy_book/random_split.py
--rw-r--r--   0 root         (0) root         (0)      238 2023-03-02 00:18:56.000000 duy-book-1.1.0/src/duy_book/ratio_split.py
--rw-r--r--   0 root         (0) root         (0)      177 2023-03-02 00:18:56.000000 duy-book-1.1.0/src/duy_book/tqdn.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-02 00:19:02.786955 duy-book-1.1.0/src/duy_book.egg-info/
--rw-r--r--   0 root         (0) root         (0)      693 2023-03-02 00:19:02.000000 duy-book-1.1.0/src/duy_book.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      358 2023-03-02 00:19:02.000000 duy-book-1.1.0/src/duy_book.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-02 00:19:02.000000 duy-book-1.1.0/src/duy_book.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-03-02 00:19:02.000000 duy-book-1.1.0/src/duy_book.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 03:56:18.377194 duy-book-1.1.2/
+-rw-r--r--   0 root         (0) root         (0)     1074 2023-05-16 03:56:09.000000 duy-book-1.1.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      656 2023-05-16 03:56:18.377194 duy-book-1.1.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      170 2023-05-16 03:56:09.000000 duy-book-1.1.2/README.md
+-rw-r--r--   0 root         (0) root         (0)      104 2023-05-16 03:56:09.000000 duy-book-1.1.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      611 2023-05-16 03:56:18.378194 duy-book-1.1.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 03:56:18.373193 duy-book-1.1.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 03:56:18.376194 duy-book-1.1.2/src/duy_book/
+-rw-r--r--   0 root         (0) root         (0)      265 2023-05-16 03:56:09.000000 duy-book-1.1.2/src/duy_book/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      431 2023-05-16 03:56:09.000000 duy-book-1.1.2/src/duy_book/colab.py
+-rw-r--r--   0 root         (0) root         (0)      320 2023-05-16 03:56:09.000000 duy-book-1.1.2/src/duy_book/cudaset.py
+-rw-r--r--   0 root         (0) root         (0)     2456 2023-05-16 03:56:09.000000 duy-book-1.1.2/src/duy_book/module.py
+-rw-r--r--   0 root         (0) root         (0)      151 2023-05-16 03:56:09.000000 duy-book-1.1.2/src/duy_book/random_split.py
+-rw-r--r--   0 root         (0) root         (0)      238 2023-05-16 03:56:09.000000 duy-book-1.1.2/src/duy_book/ratio_split.py
+-rw-r--r--   0 root         (0) root         (0)      201 2023-05-16 03:56:09.000000 duy-book-1.1.2/src/duy_book/tqdn.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 03:56:18.377194 duy-book-1.1.2/src/duy_book.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      656 2023-05-16 03:56:18.000000 duy-book-1.1.2/src/duy_book.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      358 2023-05-16 03:56:18.000000 duy-book-1.1.2/src/duy_book.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 03:56:18.000000 duy-book-1.1.2/src/duy_book.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-05-16 03:56:18.000000 duy-book-1.1.2/src/duy_book.egg-info/top_level.txt
```

### Comparing `duy-book-1.1.0/LICENSE` & `duy-book-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `duy-book-1.1.0/PKG-INFO` & `duy-book-1.1.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 Metadata-Version: 2.1
 Name: duy-book
-Version: 1.1.0
+Version: 1.1.2
 Summary: A small example package
 Home-page: https://github.com/pypa/sampleproject
 Author: Duy_abu
 Author-email: author@example.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Example Package
 This is a simple example package. You can use
 [Github-flavored Markdown](https://guides.github.com/features/mastering-markdown/)
 to write your content.
-
-
```

### Comparing `duy-book-1.1.0/setup.cfg` & `duy-book-1.1.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = duy-book
-version = 1.1.0
+version = 1.1.2
 author = Duy_abu
 author_email = author@example.com
 description = A small example package
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/pypa/sampleproject
 project_urls =
```

### Comparing `duy-book-1.1.0/src/duy_book/module.py` & `duy-book-1.1.2/src/duy_book/module.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,46 @@
 import torch
 import torch.nn as nn
 import torch.optim as optim
 import torch.nn.functional as F
 import torch.optim.lr_scheduler as sched
+from torchsummary import summary
 from tqdm.notebook import tqdm
 from .colab import ColabOutput
 from .tqdn import tqdn
 
 class Module(nn.Module):
   def forward(self, input):
     return self.module.forward(input)
   
   def init(self, optimizer=optim.Adam, lr=1e-3, scheduler=sched.CosineAnnealingLR, T_max=100):
     self.cuda()
     self.optimizer = optimizer(self.parameters(), lr)
     self.scheduler = scheduler(self.optimizer, T_max)
     return self
   
+  def summary(self, input_size, batch_size=-1):
+    for param in self.parameters():
+      device = str(param.device).split(':')[0]
+      return summary(self, input_size, batch_size, device)
+  
   def test(self, loader):
     self.eval()
     accuracy = 0
     with torch.no_grad():
-      progress = tqdm(loader)
-      for images, labels in progress:
+      for bar, (images, labels) in tqdn(loader, desc='Testing\t'):
         predict = self(images).argmax(1)
         accuracy += (predict == labels).sum().item()
         accuracy /= len(loader.dataset)
-        progress.set_postfix_str('Accuracy is {:%}'.format(accuracy))
+        bar.set_postfix_str('Accuracy is {:%}'.format(accuracy))
   
   def fit(self, epochs:int, loaders:list, losser=F.cross_entropy):
     colab = ColabOutput()
     losses = [[], [], []]
-    for bar, epoch in tqdn(range(epochs)):
+    for bar, epoch in tqdn(range(epochs), desc='Training'):
       for param_group in self.optimizer.param_groups:
         bar.set_postfix_str(f'lr:{param_group["lr"]}')
         break
 
       self.train()
       for images, labels in loaders[0]:
         self.optimizer.zero_grad()
```

### Comparing `duy-book-1.1.0/src/duy_book.egg-info/PKG-INFO` & `duy-book-1.1.2/src/duy_book.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 Metadata-Version: 2.1
 Name: duy-book
-Version: 1.1.0
+Version: 1.1.2
 Summary: A small example package
 Home-page: https://github.com/pypa/sampleproject
 Author: Duy_abu
 Author-email: author@example.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Example Package
 This is a simple example package. You can use
 [Github-flavored Markdown](https://guides.github.com/features/mastering-markdown/)
 to write your content.
-
-
```

