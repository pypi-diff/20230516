# Comparing `tmp/iosense_connect-2.1.3.tar.gz` & `tmp/iosense_connect-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\iosense_connect-2.1.3.tar", last modified: Thu May 11 06:07:42 2023, max compression
+gzip compressed data, was "dist\iosense_connect-2.1.4.tar", last modified: Tue May 16 09:02:39 2023, max compression
```

## Comparing `iosense_connect-2.1.3.tar` & `iosense_connect-2.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 06:07:42.320991 iosense_connect-2.1.3/
--rw-rw-rw-   0        0        0     1087 2023-04-28 09:03:25.000000 iosense_connect-2.1.3/LICENSE.txt
--rw-rw-rw-   0        0        0     1062 2023-05-11 06:07:42.320991 iosense_connect-2.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      690 2023-04-28 09:03:25.000000 iosense_connect-2.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-11 06:07:42.258495 iosense_connect-2.1.3/iosense_connect/
--rw-rw-rw-   0        0        0       37 2023-03-23 09:15:17.000000 iosense_connect-2.1.3/iosense_connect/__init__.py
--rw-rw-rw-   0        0        0    22553 2023-05-11 06:07:34.000000 iosense_connect-2.1.3/iosense_connect/data_access.py
-drwxrwxrwx   0        0        0        0 2023-05-11 06:07:42.320991 iosense_connect-2.1.3/iosense_connect.egg-info/
--rw-rw-rw-   0        0        0     1062 2023-05-11 06:07:41.000000 iosense_connect-2.1.3/iosense_connect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      245 2023-05-11 06:07:41.000000 iosense_connect-2.1.3/iosense_connect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 06:07:41.000000 iosense_connect-2.1.3/iosense_connect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-05-11 06:07:41.000000 iosense_connect-2.1.3/iosense_connect.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-11 06:07:42.320991 iosense_connect-2.1.3/setup.cfg
--rw-rw-rw-   0        0        0      614 2023-05-11 06:07:35.000000 iosense_connect-2.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 09:02:39.244596 iosense_connect-2.1.4/
+-rw-rw-rw-   0        0        0     1087 2023-04-28 09:03:25.000000 iosense_connect-2.1.4/LICENSE.txt
+-rw-rw-rw-   0        0        0     1062 2023-05-16 09:02:39.242421 iosense_connect-2.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      690 2023-04-28 09:03:25.000000 iosense_connect-2.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-16 09:02:39.199251 iosense_connect-2.1.4/iosense_connect/
+-rw-rw-rw-   0        0        0       37 2023-03-23 09:15:17.000000 iosense_connect-2.1.4/iosense_connect/__init__.py
+-rw-rw-rw-   0        0        0    22624 2023-05-16 08:48:38.000000 iosense_connect-2.1.4/iosense_connect/data_access.py
+drwxrwxrwx   0        0        0        0 2023-05-16 09:02:39.238157 iosense_connect-2.1.4/iosense_connect.egg-info/
+-rw-rw-rw-   0        0        0     1062 2023-05-16 09:02:38.000000 iosense_connect-2.1.4/iosense_connect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      245 2023-05-16 09:02:38.000000 iosense_connect-2.1.4/iosense_connect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 09:02:38.000000 iosense_connect-2.1.4/iosense_connect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-05-16 09:02:38.000000 iosense_connect-2.1.4/iosense_connect.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-16 09:02:39.244596 iosense_connect-2.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      614 2023-05-15 07:38:32.000000 iosense_connect-2.1.4/setup.py
```

### Comparing `iosense_connect-2.1.3/LICENSE.txt` & `iosense_connect-2.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `iosense_connect-2.1.3/PKG-INFO` & `iosense_connect-2.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iosense_connect
-Version: 2.1.3
+Version: 2.1.4
 Summary: iosense connect library
 Author: Faclon-Labs
 Author-email: reachus@faclon.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `iosense_connect-2.1.3/README.md` & `iosense_connect-2.1.4/README.md`

 * *Files identical despite different names*

### Comparing `iosense_connect-2.1.3/iosense_connect/data_access.py` & `iosense_connect-2.1.4/iosense_connect/data_access.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
         for (value1, value2) in zip(sensor_id_list, sensor_name_list):
             df_meta = pd.DataFrame(data[str(value1)])
             df_meta = df_meta.set_index('paramName').transpose()
 
             if 'm' in df_meta.columns and 'c' in df_meta.columns:
                 m = float(df_meta.iloc[0]['m'])
-                c = int(df_meta.iloc[0]['c'])
+                c = int(str(df_meta.iloc[0]['c']).replace(',',''))
                 df[str(value2)] = df[str(value2)].replace('BAD 255', '-99999').replace('-', '99999').replace(
                     'BAD undefined', '-99999').replace('BAD 0', '-99999')
                 df[str(value2)] = df[str(value2)].astype('float')
                 df[str(value2)] = (df[str(value2)] * m) + c
                 if 'min' in df_meta.columns:
                     min = int(df_meta.iloc[0]['min'])
                     df[str(value2)] = np.where(df[str(value2)] <= min, min, df[str(value2)])
@@ -495,12 +495,13 @@
                     df = DataAccess.get_caliberation(self, device_id, metadata, df,onpremise=onpremise)
                 if bands is not None:
                     df = DataAccess.time_grouping(self, df, bands,compute)
                 df = df.set_index(['time'])
                 df = df.fillna(value=np.nan)
                 df.dropna(axis=0, how='all', inplace=True)
                 df.reset_index(drop=False, inplace=True)
+                df.drop_duplicates(inplace=True)
                 if IST == False:
                     df['time'] = pd.to_datetime(df['time']) - timedelta(hours=5,minutes=30)
             return df
         except Exception as e:
             print(e)
```

### Comparing `iosense_connect-2.1.3/iosense_connect.egg-info/PKG-INFO` & `iosense_connect-2.1.4/iosense_connect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iosense-connect
-Version: 2.1.3
+Version: 2.1.4
 Summary: iosense connect library
 Author: Faclon-Labs
 Author-email: reachus@faclon.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `iosense_connect-2.1.3/setup.py` & `iosense_connect-2.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "iosense_connect",
-    version = "2.1.3",
+    version = "2.1.4",
     author = "Faclon-Labs",
     author_email = "reachus@faclon.com",
     description = "iosense connect library",
     packages = ["iosense_connect"],
     long_description = long_description,
     long_description_content_type = "text/markdown",
     classifiers = [
```

