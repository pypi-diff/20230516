# Comparing `tmp/yotpy-0.0.84.tar.gz` & `tmp/yotpy-0.0.85.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yotpy-0.0.84.tar", last modified: Thu Apr 20 21:49:41 2023, max compression
+gzip compressed data, was "yotpy-0.0.85.tar", last modified: Tue May 16 00:42:07 2023, max compression
```

## Comparing `yotpy-0.0.84.tar` & `yotpy-0.0.85.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      893 2023-04-12 23:14:08.203084 yotpy-0.0.84/.github/workflows/static.yml
--rw-r--r--   0        0        0      316 2023-04-12 22:41:53.693273 yotpy-0.0.84/.gitignore
--rw-r--r--   0        0        0     1085 2023-04-11 18:17:34.364138 yotpy-0.0.84/LICENSE
--rw-r--r--   0        0        0      378 2023-04-20 14:56:17.136904 yotpy-0.0.84/README.md
--rw-r--r--   0        0        0      136 2023-04-12 22:59:50.105965 yotpy-0.0.84/docs/index.html
--rw-r--r--   0        0        0   178839 2023-04-12 22:59:50.175644 yotpy-0.0.84/docs/search.js
--rw-r--r--   0        0        0   491392 2023-04-12 22:59:50.101919 yotpy-0.0.84/docs/yotpy.html
--rw-r--r--   0        0        0      830 2023-04-13 22:15:48.351075 yotpy-0.0.84/pyproject.toml
--rw-r--r--   0        0        0      318 2023-04-20 21:49:25.507206 yotpy-0.0.84/yotpy/__init__.py
--rw-r--r--   0        0        0    32314 2023-04-20 21:46:46.147254 yotpy-0.0.84/yotpy/core.py
--rw-r--r--   0        0        0     1953 2023-04-13 22:27:49.518980 yotpy-0.0.84/yotpy/exceptions.py
--rw-r--r--   0        0        0     1109 1970-01-01 00:00:00.000000 yotpy-0.0.84/PKG-INFO
+-rw-r--r--   0        0        0      893 2023-04-12 23:14:08.203084 yotpy-0.0.85/.github/workflows/static.yml
+-rw-r--r--   0        0        0      316 2023-04-12 22:41:53.693273 yotpy-0.0.85/.gitignore
+-rw-r--r--   0        0        0     1085 2023-04-11 18:17:34.364138 yotpy-0.0.85/LICENSE
+-rw-r--r--   0        0        0      378 2023-04-20 14:56:17.136904 yotpy-0.0.85/README.md
+-rw-r--r--   0        0        0      136 2023-04-12 22:59:50.105965 yotpy-0.0.85/docs/index.html
+-rw-r--r--   0        0        0   178839 2023-04-12 22:59:50.175644 yotpy-0.0.85/docs/search.js
+-rw-r--r--   0        0        0   491392 2023-04-12 22:59:50.101919 yotpy-0.0.85/docs/yotpy.html
+-rw-r--r--   0        0        0      830 2023-04-13 22:15:48.351075 yotpy-0.0.85/pyproject.toml
+-rw-r--r--   0        0        0      318 2023-05-16 00:40:49.101718 yotpy-0.0.85/yotpy/__init__.py
+-rw-r--r--   0        0        0    32578 2023-05-16 00:40:41.423561 yotpy-0.0.85/yotpy/core.py
+-rw-r--r--   0        0        0     1953 2023-04-13 22:27:49.518980 yotpy-0.0.85/yotpy/exceptions.py
+-rw-r--r--   0        0        0     1109 1970-01-01 00:00:00.000000 yotpy-0.0.85/PKG-INFO
```

### Comparing `yotpy-0.0.84/.github/workflows/static.yml` & `yotpy-0.0.85/.github/workflows/static.yml`

 * *Files identical despite different names*

### Comparing `yotpy-0.0.84/LICENSE` & `yotpy-0.0.85/LICENSE`

 * *Files identical despite different names*

### Comparing `yotpy-0.0.84/docs/search.js` & `yotpy-0.0.85/docs/search.js`

 * *Files identical despite different names*

### Comparing `yotpy-0.0.84/docs/yotpy.html` & `yotpy-0.0.85/docs/yotpy.html`

 * *Files identical despite different names*

### Comparing `yotpy-0.0.84/pyproject.toml` & `yotpy-0.0.85/pyproject.toml`

 * *Files identical despite different names*

### Comparing `yotpy-0.0.84/yotpy/core.py` & `yotpy-0.0.85/yotpy/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -281,65 +281,67 @@
         # Flatten the JSON object into a list of dictionaries using the flatten method.
         for item in JSONTransformer.flatten_list(json_list, sep, exclude, include):
             rows.append(item)
             headers.update(item.keys())
         return rows, headers
 
     @staticmethod
-    def to_csv_stringio(headers: set, rows: list[dict]) -> StringIO:
+    def to_csv_stringio(headers: set, rows: list[dict], delimiter=',') -> StringIO:
         """
         Convert a list of rows into a CSV formatted StringIO object.
 
         This method takes a list of rows (dictionaries) and a set of headers, and writes them into
         a CSV formatted StringIO object. It can be used to create a CSV file-like object without
         creating an actual file on the filesystem.
 
         Args:
             headers (set): A set of headers to use for the CSV data.
             rows (list[dict]): A list of rows to convert into a CSV formatted StringIO object.
+            delimiter (str, optional): The delimiter to use for the CSV data. Defaults to ','.
 
         Returns:
             StringIO: A CSV formatted StringIO object.
         """
         # Create a StringIO object to write the CSV data to.
         csv_stringio = StringIO()
         # Create a csv writer and write the rows to the StringIO object.
-        writer = DictWriter(csv_stringio, fieldnames=headers)
+        writer = DictWriter(csv_stringio, fieldnames=headers, delimiter=delimiter)
         writer.writeheader()
         writer.writerows(rows)
 
         # Reset the StringIO object's position to the beginning
         csv_stringio.seek(0)
 
         return csv_stringio
 
     @staticmethod
-    def to_csv_bytesio(headers: set, rows: list[dict]) -> BytesIO:
+    def to_csv_bytesio(headers: set, rows: list[dict], delimiter=',') -> BytesIO:
         """
         Convert a list of rows into a CSV formatted BytesIO object.
 
         This method takes a list of rows (dictionaries) and a set of headers, and writes them into
         a CSV formatted BytesIO object. It can be used to create a CSV file-like object without
         creating an actual file on the filesystem.
 
         Args:
             headers (set): A set of headers to use for the CSV data.
             rows (list[dict]): A list of rows to convert into a CSV formatted BytesIO object.
+            delimiter (str, optional): The delimiter to use for the CSV data. Defaults to ','.
 
         Returns:
             BytesIO: A CSV formatted BytesIO object.
         """
         # Create a BytesIO object to write the CSV data to.
         csv_bytesio = BytesIO()
         
         # Wrap the BytesIO object with a TextIOWrapper using utf-8-sig encoding.
         csv_textio = TextIOWrapper(csv_bytesio, encoding='utf-8-sig')
 
         # Create a csv writer and write the rows to the wrapped BytesIO object.
-        writer = DictWriter(csv_textio, fieldnames=headers)
+        writer = DictWriter(csv_textio, fieldnames=headers, delimiter=delimiter)
         writer.writeheader()
         writer.writerows(rows)
 
         # Flush the TextIOWrapper to ensure all data is written to the underlying BytesIO object
         csv_textio.flush()
 
         csv_bytesio = csv_textio.detach()
```

### Comparing `yotpy-0.0.84/yotpy/exceptions.py` & `yotpy-0.0.85/yotpy/exceptions.py`

 * *Files identical despite different names*

### Comparing `yotpy-0.0.84/PKG-INFO` & `yotpy-0.0.85/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yotpy
-Version: 0.0.84
+Version: 0.0.85
 Summary: Yotpy: An easy-to-use Python wrapper for the Yotpo web API.
 Home-page: https://github.com/wlk-dev/yotpy
 License: MIT
 Keywords: yotpo, api, wrapper, python, data, transformation, client, integration, review, ecommerce
 Author: William Koelling
 Author-email: william.koelling@gmail.com
 Description-Content-Type: text/markdown
```

