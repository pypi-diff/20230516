# Comparing `tmp/HawaData-0.4.0.tar.gz` & `tmp/HawaData-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HawaData-0.4.0.tar", last modified: Mon May  8 13:08:22 2023, max compression
+gzip compressed data, was "HawaData-0.4.1.tar", last modified: Tue May 16 03:27:13 2023, max compression
```

## Comparing `HawaData-0.4.0.tar` & `HawaData-0.4.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-08 13:08:22.203111 HawaData-0.4.0/
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-08 13:08:22.192704 HawaData-0.4.0/HawaData.egg-info/
--rw-r--r--   0 wangzhou   (501) staff       (20)     2278 2023-05-08 13:08:22.000000 HawaData-0.4.0/HawaData.egg-info/PKG-INFO
--rw-r--r--   0 wangzhou   (501) staff       (20)      484 2023-05-08 13:08:22.000000 HawaData-0.4.0/HawaData.egg-info/SOURCES.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)        1 2023-05-08 13:08:22.000000 HawaData-0.4.0/HawaData.egg-info/dependency_links.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)        5 2023-05-08 13:08:22.000000 HawaData-0.4.0/HawaData.egg-info/top_level.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)     2278 2023-05-08 13:08:22.202600 HawaData-0.4.0/PKG-INFO
--rw-r--r--   0 wangzhou   (501) staff       (20)      669 2022-12-02 07:10:45.000000 HawaData-0.4.0/README.md
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-08 13:08:22.193224 HawaData-0.4.0/hawa/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:39:05.000000 HawaData-0.4.0/hawa/__init__.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-08 13:08:22.195043 HawaData-0.4.0/hawa/base/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 05:35:03.000000 HawaData-0.4.0/hawa/base/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     3014 2023-05-05 08:28:22.000000 HawaData-0.4.0/hawa/base/db.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      173 2022-12-01 06:05:08.000000 HawaData-0.4.0/hawa/base/decos.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      845 2022-12-02 03:09:07.000000 HawaData-0.4.0/hawa/base/init.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-08 13:08:22.196756 HawaData-0.4.0/hawa/common/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:40:41.000000 HawaData-0.4.0/hawa/common/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     9040 2023-05-08 13:08:04.000000 HawaData-0.4.0/hawa/common/data.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     5320 2023-05-08 13:06:08.000000 HawaData-0.4.0/hawa/common/query.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     2784 2023-05-05 08:28:22.000000 HawaData-0.4.0/hawa/common/utils.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     2551 2023-03-29 04:22:37.000000 HawaData-0.4.0/hawa/config.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-08 13:08:22.198373 HawaData-0.4.0/hawa/data/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 08:59:59.000000 HawaData-0.4.0/hawa/data/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      336 2022-12-13 08:17:02.000000 HawaData-0.4.0/hawa/data/district.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      472 2022-12-28 09:14:15.000000 HawaData-0.4.0/hawa/data/school.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-08 13:08:22.200748 HawaData-0.4.0/hawa/paper/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:27:31.000000 HawaData-0.4.0/hawa/paper/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)    22995 2023-05-05 09:08:17.000000 HawaData-0.4.0/hawa/paper/health.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     5273 2023-05-05 07:06:02.000000 HawaData-0.4.0/hawa/paper/mht.py
--rw-r--r--   0 wangzhou   (501) staff       (20)       38 2023-05-08 13:08:22.203266 HawaData-0.4.0/setup.cfg
--rw-r--r--   0 wangzhou   (501) staff       (20)      879 2023-05-05 08:13:11.000000 HawaData-0.4.0/setup.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-08 13:08:22.201611 HawaData-0.4.0/test/
--rw-r--r--   0 wangzhou   (501) staff       (20)     2208 2022-12-08 07:17:34.000000 HawaData-0.4.0/test/test_query.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-16 03:27:13.575273 HawaData-0.4.1/
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-16 03:27:13.567239 HawaData-0.4.1/HawaData.egg-info/
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2306 2023-05-16 03:27:13.000000 HawaData-0.4.1/HawaData.egg-info/PKG-INFO
+-rw-r--r--   0 wangzhou   (501) staff       (20)      484 2023-05-16 03:27:13.000000 HawaData-0.4.1/HawaData.egg-info/SOURCES.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)        1 2023-05-16 03:27:13.000000 HawaData-0.4.1/HawaData.egg-info/dependency_links.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)        5 2023-05-16 03:27:13.000000 HawaData-0.4.1/HawaData.egg-info/top_level.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2306 2023-05-16 03:27:13.574974 HawaData-0.4.1/PKG-INFO
+-rw-r--r--   0 wangzhou   (501) staff       (20)      669 2022-12-02 07:10:45.000000 HawaData-0.4.1/README.md
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-16 03:27:13.567784 HawaData-0.4.1/hawa/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:39:05.000000 HawaData-0.4.1/hawa/__init__.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-16 03:27:13.569529 HawaData-0.4.1/hawa/base/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 05:35:03.000000 HawaData-0.4.1/hawa/base/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     3014 2023-05-05 08:28:22.000000 HawaData-0.4.1/hawa/base/db.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      173 2022-12-01 06:05:08.000000 HawaData-0.4.1/hawa/base/decos.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      845 2022-12-02 03:09:07.000000 HawaData-0.4.1/hawa/base/init.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-16 03:27:13.570923 HawaData-0.4.1/hawa/common/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:40:41.000000 HawaData-0.4.1/hawa/common/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     8948 2023-05-16 03:27:04.000000 HawaData-0.4.1/hawa/common/data.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     5320 2023-05-16 03:26:37.000000 HawaData-0.4.1/hawa/common/query.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2784 2023-05-05 08:28:22.000000 HawaData-0.4.1/hawa/common/utils.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2551 2023-03-29 04:22:37.000000 HawaData-0.4.1/hawa/config.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-16 03:27:13.572394 HawaData-0.4.1/hawa/data/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 08:59:59.000000 HawaData-0.4.1/hawa/data/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      336 2022-12-13 08:17:02.000000 HawaData-0.4.1/hawa/data/district.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      472 2022-12-28 09:14:15.000000 HawaData-0.4.1/hawa/data/school.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-16 03:27:13.573514 HawaData-0.4.1/hawa/paper/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:27:31.000000 HawaData-0.4.1/hawa/paper/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)    22995 2023-05-05 09:08:17.000000 HawaData-0.4.1/hawa/paper/health.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     5273 2023-05-05 07:06:02.000000 HawaData-0.4.1/hawa/paper/mht.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)       38 2023-05-16 03:27:13.575384 HawaData-0.4.1/setup.cfg
+-rw-r--r--   0 wangzhou   (501) staff       (20)      879 2023-05-05 08:13:11.000000 HawaData-0.4.1/setup.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-16 03:27:13.574246 HawaData-0.4.1/test/
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2208 2022-12-08 07:17:34.000000 HawaData-0.4.1/test/test_query.py
```

### Comparing `HawaData-0.4.0/HawaData.egg-info/PKG-INFO` & `HawaData-0.4.1/HawaData.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HawaData
-Version: 0.4.0
+Version: 0.4.1
 Summary: Use For Unified Hawa Data.
 Home-page: https://github.com/StevenLianaL/HawaData
 Author: Steven Wang
 Author-email: brightstar8284@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
@@ -80,7 +80,8 @@
 - 0.3.3 performance improvement by grade
 - 0.3.4 up to py3.11
 - 0.3.5 fix engine encoding
 - 0.3.6 update sqlarchemy to 2+
 - 0.3.7 update pandas to 2+
 - 0.3.8 fix loss data
 - 0.4.0 add case project_id
+- 0.4.1 fix miss grade data
```

### Comparing `HawaData-0.4.0/PKG-INFO` & `HawaData-0.4.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HawaData
-Version: 0.4.0
+Version: 0.4.1
 Summary: Use For Unified Hawa Data.
 Home-page: https://github.com/StevenLianaL/HawaData
 Author: Steven Wang
 Author-email: brightstar8284@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
@@ -80,7 +80,8 @@
 - 0.3.3 performance improvement by grade
 - 0.3.4 up to py3.11
 - 0.3.5 fix engine encoding
 - 0.3.6 update sqlarchemy to 2+
 - 0.3.7 update pandas to 2+
 - 0.3.8 fix loss data
 - 0.4.0 add case project_id
+- 0.4.1 fix miss grade data
```

### Comparing `HawaData-0.4.0/README.md` & `HawaData-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `HawaData-0.4.0/hawa/base/db.py` & `HawaData-0.4.1/hawa/base/db.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.4.0/hawa/base/init.py` & `HawaData-0.4.1/hawa/base/init.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.4.0/hawa/common/data.py` & `HawaData-0.4.1/hawa/common/data.py`

 * *Files 4% similar despite different names*

```diff
@@ -212,19 +212,19 @@
 
     def get_last_year_miss(self, grade: int):
         key = f'{project.REDIS_PREFIX}{self.last_year_num}:data'
         data = json.loads(self.redis.conn.get(key))
         try:
             grade_data = data[str(grade)]
         except KeyError:
-            temp_key = f'{project.REDIS_PREFIX}{self.last_year_num - 1}:data'
-            temp_cache_data = self.redis.conn.get(temp_key)
-            if temp_cache_data:
-                temp_data = json.loads(temp_cache_data)
-                grade_data = temp_data[str(grade - 1)]
+            for i in range(1, grade):
+                temp_grade = grade - i
+                grade_data = data.get(str(temp_grade))
+                if grade_data:
+                    break
             else:
                 grade_data = data[str(3)]
 
         grade_data['people']['grade'] = f"{grade}年级"
         for k, v in grade_data['code'].items():
             grade_data['code'][k]['grade'] = grade
         return grade_data
```

### Comparing `HawaData-0.4.0/hawa/common/query.py` & `HawaData-0.4.1/hawa/common/query.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.4.0/hawa/common/utils.py` & `HawaData-0.4.1/hawa/common/utils.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.4.0/hawa/config.py` & `HawaData-0.4.1/hawa/config.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.4.0/hawa/paper/health.py` & `HawaData-0.4.1/hawa/paper/health.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.4.0/hawa/paper/mht.py` & `HawaData-0.4.1/hawa/paper/mht.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.4.0/setup.py` & `HawaData-0.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.4.0/test/test_query.py` & `HawaData-0.4.1/test/test_query.py`

 * *Files identical despite different names*

