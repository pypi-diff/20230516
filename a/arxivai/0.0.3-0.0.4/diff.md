# Comparing `tmp/arxivai-0.0.3.tar.gz` & `tmp/arxivai-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arxivai-0.0.3.tar", last modified: Tue May 16 18:49:51 2023, max compression
+gzip compressed data, was "arxivai-0.0.4.tar", last modified: Tue May 16 19:10:25 2023, max compression
```

## Comparing `arxivai-0.0.3.tar` & `arxivai-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 18:49:51.252609 arxivai-0.0.3/
--rw-rw-rw-   0        0        0     1090 2023-05-16 12:09:57.000000 arxivai-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      655 2023-05-16 18:49:51.251607 arxivai-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      122 2023-05-16 12:09:49.000000 arxivai-0.0.3/README.md
--rw-rw-rw-   0        0        0      652 2023-05-16 18:49:07.000000 arxivai-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-16 18:49:51.252609 arxivai-0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-16 18:49:51.214605 arxivai-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-05-16 18:49:51.230609 arxivai-0.0.3/src/arxivai/
--rw-rw-rw-   0        0        0       24 2023-05-16 18:44:42.000000 arxivai-0.0.3/src/arxivai/__init__.py
--rw-rw-rw-   0        0        0     4365 2023-05-16 18:33:06.000000 arxivai-0.0.3/src/arxivai/arxiv_api.py
-drwxrwxrwx   0        0        0        0 2023-05-16 18:49:51.249607 arxivai-0.0.3/src/arxivai.egg-info/
--rw-rw-rw-   0        0        0      655 2023-05-16 18:49:51.000000 arxivai-0.0.3/src/arxivai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      221 2023-05-16 18:49:51.000000 arxivai-0.0.3/src/arxivai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 18:49:51.000000 arxivai-0.0.3/src/arxivai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-16 18:49:51.000000 arxivai-0.0.3/src/arxivai.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-16 19:10:25.738516 arxivai-0.0.4/
+-rw-rw-rw-   0        0        0     1090 2023-05-16 12:09:57.000000 arxivai-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      655 2023-05-16 19:10:25.737515 arxivai-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      122 2023-05-16 12:09:49.000000 arxivai-0.0.4/README.md
+-rw-rw-rw-   0        0        0      652 2023-05-16 19:09:38.000000 arxivai-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-16 19:10:25.738516 arxivai-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-16 19:10:25.708515 arxivai-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-05-16 19:10:25.716516 arxivai-0.0.4/src/arxivai/
+-rw-rw-rw-   0        0        0       24 2023-05-16 18:44:42.000000 arxivai-0.0.4/src/arxivai/__init__.py
+-rw-rw-rw-   0        0        0     4474 2023-05-16 19:09:20.000000 arxivai-0.0.4/src/arxivai/arxiv_api.py
+drwxrwxrwx   0        0        0        0 2023-05-16 19:10:25.734513 arxivai-0.0.4/src/arxivai.egg-info/
+-rw-rw-rw-   0        0        0      655 2023-05-16 19:10:25.000000 arxivai-0.0.4/src/arxivai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      221 2023-05-16 19:10:25.000000 arxivai-0.0.4/src/arxivai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 19:10:25.000000 arxivai-0.0.4/src/arxivai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-16 19:10:25.000000 arxivai-0.0.4/src/arxivai.egg-info/top_level.txt
```

### Comparing `arxivai-0.0.3/LICENSE` & `arxivai-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `arxivai-0.0.3/PKG-INFO` & `arxivai-0.0.4/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arxivai
-Version: 0.0.3
+Version: 0.0.4
 Summary: A complete arXiv API wrapper for Python.
 Author-email: Bongsang Kim <happykbs@gmail.com>
 Project-URL: Homepage, https://github.com/bongsang/arxivai-pypi
 Project-URL: Bug Tracker, https://github.com/bongsang/arxivai-pypi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `arxivai-0.0.3/pyproject.toml` & `arxivai-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   "requests",
   "beautifulsoup4",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "arxivai"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Bongsang Kim", email="happykbs@gmail.com" },
 ]
 description = "A complete arXiv API wrapper for Python."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `arxivai-0.0.3/src/arxivai/arxiv_api.py` & `arxivai-0.0.4/src/arxivai/arxiv_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,14 +65,15 @@
 
     results = []
     for entry in entries:
         result = {
             'paper_id': re.findall(regx, entry.id.text)[0],
             'title': entry.find('title').text.replace('\n', ' ').strip(),
             'authors': [author.find('name').text.strip() for author in entry.find_all('author')],
+            'category': entry.find('category')['term'],
             'abstract': entry.find('summary').text.replace('\n', ' ').strip(),
             'published': entry.find('published').text,
         }
         results.append(result)
 
     return results
 
@@ -83,14 +84,15 @@
     r = requests.get(url)
     soup = BeautifulSoup(r.text, 'lxml', parse_only=SoupStrainer('entry'))
 
     result = {
         'paper_id': re.findall(regx, soup.id.text)[0],
         'title': soup.title.text.replace('\n', ' ').strip(),
         'authors': [author.find('name').text.strip() for author in soup.find_all('author')],
+        'category': soup.find('category')['term'],
         'abstract': soup.summary.text.replace('\n', ' ').strip(),
         'published': soup.published.text,
     }
 
     return result
```

### Comparing `arxivai-0.0.3/src/arxivai.egg-info/PKG-INFO` & `arxivai-0.0.4/src/arxivai.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arxivai
-Version: 0.0.3
+Version: 0.0.4
 Summary: A complete arXiv API wrapper for Python.
 Author-email: Bongsang Kim <happykbs@gmail.com>
 Project-URL: Homepage, https://github.com/bongsang/arxivai-pypi
 Project-URL: Bug Tracker, https://github.com/bongsang/arxivai-pypi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

