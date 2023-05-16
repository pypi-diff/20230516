# Comparing `tmp/arxivai-0.0.6.tar.gz` & `tmp/arxivai-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arxivai-0.0.6.tar", last modified: Tue May 16 19:55:39 2023, max compression
+gzip compressed data, was "arxivai-0.0.7.tar", last modified: Tue May 16 21:50:24 2023, max compression
```

## Comparing `arxivai-0.0.6.tar` & `arxivai-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 19:55:39.650754 arxivai-0.0.6/
--rw-rw-rw-   0        0        0     1090 2023-05-16 12:09:57.000000 arxivai-0.0.6/LICENSE
--rw-rw-rw-   0        0        0      655 2023-05-16 19:55:39.649750 arxivai-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      122 2023-05-16 12:09:49.000000 arxivai-0.0.6/README.md
--rw-rw-rw-   0        0        0      652 2023-05-16 19:55:09.000000 arxivai-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-16 19:55:39.651751 arxivai-0.0.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-16 19:55:39.619757 arxivai-0.0.6/src/
-drwxrwxrwx   0        0        0        0 2023-05-16 19:55:39.627754 arxivai-0.0.6/src/arxivai/
--rw-rw-rw-   0        0        0       24 2023-05-16 18:44:42.000000 arxivai-0.0.6/src/arxivai/__init__.py
--rw-rw-rw-   0        0        0     4509 2023-05-16 19:54:43.000000 arxivai-0.0.6/src/arxivai/arxiv_api.py
-drwxrwxrwx   0        0        0        0 2023-05-16 19:55:39.647754 arxivai-0.0.6/src/arxivai.egg-info/
--rw-rw-rw-   0        0        0      655 2023-05-16 19:55:39.000000 arxivai-0.0.6/src/arxivai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      221 2023-05-16 19:55:39.000000 arxivai-0.0.6/src/arxivai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 19:55:39.000000 arxivai-0.0.6/src/arxivai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-16 19:55:39.000000 arxivai-0.0.6/src/arxivai.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-16 21:50:24.459787 arxivai-0.0.7/
+-rw-rw-rw-   0        0        0     1090 2023-05-16 12:09:57.000000 arxivai-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0      655 2023-05-16 21:50:24.458787 arxivai-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      122 2023-05-16 12:09:49.000000 arxivai-0.0.7/README.md
+-rw-rw-rw-   0        0        0      679 2023-05-16 20:26:19.000000 arxivai-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-16 21:50:24.459787 arxivai-0.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-16 21:50:24.427787 arxivai-0.0.7/src/
+drwxrwxrwx   0        0        0        0 2023-05-16 21:50:24.438785 arxivai-0.0.7/src/arxivai/
+-rw-rw-rw-   0        0        0       24 2023-05-16 18:44:42.000000 arxivai-0.0.7/src/arxivai/__init__.py
+-rw-rw-rw-   0        0        0     4421 2023-05-16 20:22:48.000000 arxivai-0.0.7/src/arxivai/arxiv_api.py
+-rw-rw-rw-   0        0        0      629 2023-05-16 21:49:58.000000 arxivai-0.0.7/src/arxivai/arxiv_pdf.py
+drwxrwxrwx   0        0        0        0 2023-05-16 21:50:24.456790 arxivai-0.0.7/src/arxivai.egg-info/
+-rw-rw-rw-   0        0        0      655 2023-05-16 21:50:24.000000 arxivai-0.0.7/src/arxivai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2023-05-16 21:50:24.000000 arxivai-0.0.7/src/arxivai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 21:50:24.000000 arxivai-0.0.7/src/arxivai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-16 21:50:24.000000 arxivai-0.0.7/src/arxivai.egg-info/top_level.txt
```

### Comparing `arxivai-0.0.6/LICENSE` & `arxivai-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `arxivai-0.0.6/PKG-INFO` & `arxivai-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arxivai
-Version: 0.0.6
+Version: 0.0.7
 Summary: A complete arXiv API wrapper for Python.
 Author-email: Bongsang Kim <happykbs@gmail.com>
 Project-URL: Homepage, https://github.com/bongsang/arxivai-pypi
 Project-URL: Bug Tracker, https://github.com/bongsang/arxivai-pypi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `arxivai-0.0.6/pyproject.toml` & `arxivai-0.0.7/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 [build-system]
 requires = [
   "setuptools",
   "requests",
   "beautifulsoup4",
+  "google-cloud-storage",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "arxivai"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Bongsang Kim", email="happykbs@gmail.com" },
 ]
 description = "A complete arXiv API wrapper for Python."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `arxivai-0.0.6/src/arxivai/arxiv_api.py` & `arxivai-0.0.7/src/arxivai/arxiv_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,28 +75,22 @@
         }
         results.append(result)
 
     return results
 
 
 
-def fetch(id):
-    url = f'http://export.arxiv.org/api/query?id_list={id}'
+def fetch(arxiv_id):
+    url = f'http://export.arxiv.org/api/query?id_list={arxiv_id}'
     r = requests.get(url)
     soup = BeautifulSoup(r.text, 'lxml', parse_only=SoupStrainer('entry'))
 
     result = {
         'paper_id': re.findall(regx, soup.id.text)[0],
         'title': soup.title.text.replace('\n', ' ').strip(),
         'authors': [author.find('name').text.strip() for author in soup.find_all('author')],
         'category': soup.find('category')['term'],
         'abstract': soup.summary.text.replace('\n', ' ').strip(),
         'published': soup.published.text.split('T')[0],
     }
 
     return result
-
-
-if __name__ == '__main__':
-    print(search('style GAN'))
-    # print(fetch('2106.12423'))
-
```

### Comparing `arxivai-0.0.6/src/arxivai.egg-info/PKG-INFO` & `arxivai-0.0.7/src/arxivai.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arxivai
-Version: 0.0.6
+Version: 0.0.7
 Summary: A complete arXiv API wrapper for Python.
 Author-email: Bongsang Kim <happykbs@gmail.com>
 Project-URL: Homepage, https://github.com/bongsang/arxivai-pypi
 Project-URL: Bug Tracker, https://github.com/bongsang/arxivai-pypi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

