# Comparing `tmp/ProTstab2-1.0.1.tar.gz` & `tmp/ProTstab2-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ProTstab2-1.0.1.tar", last modified: Tue May 16 07:19:18 2023, max compression
+gzip compressed data, was "ProTstab2-1.0.2.tar", last modified: Tue May 16 08:07:10 2023, max compression
```

## Comparing `ProTstab2-1.0.1.tar` & `ProTstab2-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 07:19:18.199281 ProTstab2-1.0.1/
--rw-rw-rw-   0        0        0    35823 2023-05-15 09:13:01.000000 ProTstab2-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     2679 2023-05-16 07:19:18.199281 ProTstab2-1.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-16 07:19:18.192783 ProTstab2-1.0.1/ProTstab2/
--rw-rw-rw-   0        0        0     6087 2023-05-16 06:02:46.000000 ProTstab2-1.0.1/ProTstab2/__init__.py
--rw-rw-rw-   0        0        0     6192 2023-05-16 06:02:46.000000 ProTstab2-1.0.1/ProTstab2/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-16 07:19:18.198282 ProTstab2-1.0.1/ProTstab2.egg-info/
--rw-rw-rw-   0        0        0     2679 2023-05-16 07:19:18.000000 ProTstab2-1.0.1/ProTstab2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      231 2023-05-16 07:19:18.000000 ProTstab2-1.0.1/ProTstab2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 07:19:18.000000 ProTstab2-1.0.1/ProTstab2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       98 2023-05-16 07:19:18.000000 ProTstab2-1.0.1/ProTstab2.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-16 07:19:18.000000 ProTstab2-1.0.1/ProTstab2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2161 2023-05-16 06:21:35.000000 ProTstab2-1.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-16 07:19:18.199281 ProTstab2-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1057 2023-05-16 07:18:57.000000 ProTstab2-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 08:07:10.982064 ProTstab2-1.0.2/
+-rw-rw-rw-   0        0        0    35823 2023-05-15 09:13:01.000000 ProTstab2-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     2679 2023-05-16 08:07:10.981063 ProTstab2-1.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-16 08:07:10.974059 ProTstab2-1.0.2/ProTstab2/
+-rw-rw-rw-   0        0        0     6089 2023-05-16 08:04:29.000000 ProTstab2-1.0.2/ProTstab2/__init__.py
+-rw-rw-rw-   0        0        0     6192 2023-05-16 06:02:46.000000 ProTstab2-1.0.2/ProTstab2/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-16 08:07:10.980063 ProTstab2-1.0.2/ProTstab2.egg-info/
+-rw-rw-rw-   0        0        0     2679 2023-05-16 08:07:10.000000 ProTstab2-1.0.2/ProTstab2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      231 2023-05-16 08:07:10.000000 ProTstab2-1.0.2/ProTstab2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 08:07:10.000000 ProTstab2-1.0.2/ProTstab2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       98 2023-05-16 08:07:10.000000 ProTstab2-1.0.2/ProTstab2.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-16 08:07:10.000000 ProTstab2-1.0.2/ProTstab2.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2161 2023-05-16 06:21:35.000000 ProTstab2-1.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-16 08:07:10.982064 ProTstab2-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1057 2023-05-16 08:06:55.000000 ProTstab2-1.0.2/setup.py
```

### Comparing `ProTstab2-1.0.1/LICENSE` & `ProTstab2-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ProTstab2-1.0.1/PKG-INFO` & `ProTstab2-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ProTstab2
-Version: 1.0.1
+Version: 1.0.2
 Summary: Protein prediction package
 Home-page: http://8.133.174.28:8989/DeepTP/
 Author: Jianjun Zhao
 Author-email: 20204227057@stu.suda.edu.cn
 License: MIT
 Platform: all
 Classifier: Intended Audience :: Developers
```

### Comparing `ProTstab2-1.0.1/ProTstab2/__init__.py` & `ProTstab2-1.0.2/ProTstab2/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         self._exists(self.csv_name, self.csv_name_zip)
 
     def load_models(self):
         with open(os.path.join(self.base_model_path, self.features_model_name), 'rb') as f:
             self.get_model = pickle.load(f)
         new_model = tf.keras.models.load_model(os.path.join(self.base_model_path, self.deep_tp_model_name),
                                                custom_objects={'Attention': Attention})
-        new_model.summary()
+        # new_model.summary()
         self.new_model = new_model
 
         test_data = pd.read_csv(os.path.join(self.base_model_path, self.csv_name), index_col=0)
         test_data = test_data[test_data['Sequence'].str.len() <= 1500]
         test_data_x = test_data.drop(['uniprot_id', 'Sequence', 'temp'], axis=1).select_dtypes(exclude=['object'])
         self.test_data_x = test_data_x
```

### Comparing `ProTstab2-1.0.1/ProTstab2/utils.py` & `ProTstab2-1.0.2/ProTstab2/utils.py`

 * *Files identical despite different names*

### Comparing `ProTstab2-1.0.1/ProTstab2.egg-info/PKG-INFO` & `ProTstab2-1.0.2/ProTstab2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ProTstab2
-Version: 1.0.1
+Version: 1.0.2
 Summary: Protein prediction package
 Home-page: http://8.133.174.28:8989/DeepTP/
 Author: Jianjun Zhao
 Author-email: 20204227057@stu.suda.edu.cn
 License: MIT
 Platform: all
 Classifier: Intended Audience :: Developers
```

### Comparing `ProTstab2-1.0.1/README.md` & `ProTstab2-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `ProTstab2-1.0.1/setup.py` & `ProTstab2-1.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import find_packages
 
 with open("README.md", "r", encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='ProTstab2',  # 包名
-    version='1.0.1',  # 版本号
+    version='1.0.2',  # 版本号
     description='Protein prediction package',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Jianjun Zhao',
     author_email='20204227057@stu.suda.edu.cn',
     url='http://8.133.174.28:8989/DeepTP/',
     install_requires=[
```

