# Comparing `tmp/arxivai-0.0.4.tar.gz` & `tmp/arxivai-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arxivai-0.0.4.tar", last modified: Tue May 16 19:10:25 2023, max compression
+gzip compressed data, was "arxivai-0.0.5.tar", last modified: Tue May 16 19:27:26 2023, max compression
```

## Comparing `arxivai-0.0.4.tar` & `arxivai-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 19:10:25.738516 arxivai-0.0.4/
--rw-rw-rw-   0        0        0     1090 2023-05-16 12:09:57.000000 arxivai-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      655 2023-05-16 19:10:25.737515 arxivai-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      122 2023-05-16 12:09:49.000000 arxivai-0.0.4/README.md
--rw-rw-rw-   0        0        0      652 2023-05-16 19:09:38.000000 arxivai-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-16 19:10:25.738516 arxivai-0.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-16 19:10:25.708515 arxivai-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-05-16 19:10:25.716516 arxivai-0.0.4/src/arxivai/
--rw-rw-rw-   0        0        0       24 2023-05-16 18:44:42.000000 arxivai-0.0.4/src/arxivai/__init__.py
--rw-rw-rw-   0        0        0     4474 2023-05-16 19:09:20.000000 arxivai-0.0.4/src/arxivai/arxiv_api.py
-drwxrwxrwx   0        0        0        0 2023-05-16 19:10:25.734513 arxivai-0.0.4/src/arxivai.egg-info/
--rw-rw-rw-   0        0        0      655 2023-05-16 19:10:25.000000 arxivai-0.0.4/src/arxivai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      221 2023-05-16 19:10:25.000000 arxivai-0.0.4/src/arxivai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 19:10:25.000000 arxivai-0.0.4/src/arxivai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-16 19:10:25.000000 arxivai-0.0.4/src/arxivai.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-16 19:27:26.430919 arxivai-0.0.5/
+-rw-rw-rw-   0        0        0     1090 2023-05-16 12:09:57.000000 arxivai-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      655 2023-05-16 19:27:26.430919 arxivai-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      122 2023-05-16 12:09:49.000000 arxivai-0.0.5/README.md
+-rw-rw-rw-   0        0        0      652 2023-05-16 19:26:59.000000 arxivai-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-16 19:27:26.431920 arxivai-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-16 19:27:26.401924 arxivai-0.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-05-16 19:27:26.409923 arxivai-0.0.5/src/arxivai/
+-rw-rw-rw-   0        0        0       24 2023-05-16 18:44:42.000000 arxivai-0.0.5/src/arxivai/__init__.py
+-rw-rw-rw-   0        0        0     4481 2023-05-16 19:26:44.000000 arxivai-0.0.5/src/arxivai/arxiv_api.py
+drwxrwxrwx   0        0        0        0 2023-05-16 19:27:26.428920 arxivai-0.0.5/src/arxivai.egg-info/
+-rw-rw-rw-   0        0        0      655 2023-05-16 19:27:26.000000 arxivai-0.0.5/src/arxivai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      221 2023-05-16 19:27:26.000000 arxivai-0.0.5/src/arxivai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 19:27:26.000000 arxivai-0.0.5/src/arxivai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-16 19:27:26.000000 arxivai-0.0.5/src/arxivai.egg-info/top_level.txt
```

### Comparing `arxivai-0.0.4/LICENSE` & `arxivai-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `arxivai-0.0.4/PKG-INFO` & `arxivai-0.0.5/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arxivai
-Version: 0.0.4
+Version: 0.0.5
 Summary: A complete arXiv API wrapper for Python.
 Author-email: Bongsang Kim <happykbs@gmail.com>
 Project-URL: Homepage, https://github.com/bongsang/arxivai-pypi
 Project-URL: Bug Tracker, https://github.com/bongsang/arxivai-pypi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `arxivai-0.0.4/pyproject.toml` & `arxivai-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   "requests",
   "beautifulsoup4",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "arxivai"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Bongsang Kim", email="happykbs@gmail.com" },
 ]
 description = "A complete arXiv API wrapper for Python."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `arxivai-0.0.4/src/arxivai/arxiv_api.py` & `arxivai-0.0.5/src/arxivai/arxiv_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import requests
 from bs4 import BeautifulSoup, SoupStrainer
 
 regx = re.compile(r'(?<=/)\d+\.?\w+')
 """Extract arXiv paper id from url. ex) http://arxiv.org/abs/2001.04189v3 -> 2001.04189v3"""
 
-def query(q, prefix='ti', start=0, max_results=100, sort_by='relevance', sort_order='descending'):
+def search(q, prefix='all', start=0, max_results=100, sort_by='relevance', sort_order='descending'):
     """Query the arXiv API.
     https://info.arxiv.org/help/api/user-manual.html#_query_interface
 
     Parameters
     ----------
     prefix	explanation
         ti	Title
@@ -75,15 +75,15 @@
         }
         results.append(result)
 
     return results
 
 
 
-def get(id):
+def fetch(id):
     url = f'http://export.arxiv.org/api/query?id_list={id}'
     r = requests.get(url)
     soup = BeautifulSoup(r.text, 'lxml', parse_only=SoupStrainer('entry'))
 
     result = {
         'paper_id': re.findall(regx, soup.id.text)[0],
         'title': soup.title.text.replace('\n', ' ').strip(),
@@ -93,10 +93,10 @@
         'published': soup.published.text,
     }
 
     return result
 
 
 if __name__ == '__main__':
-    print(query('style GAN'))
-    # print(get('1810.03787'))
+    # print(search('style GAN'))
+    print(fetch('2106.12423'))
```

### Comparing `arxivai-0.0.4/src/arxivai.egg-info/PKG-INFO` & `arxivai-0.0.5/src/arxivai.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arxivai
-Version: 0.0.4
+Version: 0.0.5
 Summary: A complete arXiv API wrapper for Python.
 Author-email: Bongsang Kim <happykbs@gmail.com>
 Project-URL: Homepage, https://github.com/bongsang/arxivai-pypi
 Project-URL: Bug Tracker, https://github.com/bongsang/arxivai-pypi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

