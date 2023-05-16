# Comparing `tmp/uc_browser-0.3.3.tar.gz` & `tmp/uc_browser-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uc_browser-0.3.3.tar", max compression
+gzip compressed data, was "uc_browser-0.3.4.tar", max compression
```

## Comparing `uc_browser-0.3.3.tar` & `uc_browser-0.3.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       63 2022-10-11 19:35:12.176241 uc_browser-0.3.3/README.md
--rw-r--r--   0        0        0      503 2023-05-13 13:54:07.183297 uc_browser-0.3.3/pyproject.toml
--rw-r--r--   0        0        0        0 2022-10-11 19:35:12.176241 uc_browser-0.3.3/uc_browser/__init__.py
--rw-r--r--   0        0        0     8159 2023-01-17 19:09:01.710189 uc_browser-0.3.3/uc_browser/browser.py
--rw-r--r--   0        0        0    10590 2023-05-13 13:54:07.175297 uc_browser-0.3.3/uc_browser/browser_v2.py
--rw-r--r--   0        0        0      802 1970-01-01 00:00:00.000000 uc_browser-0.3.3/setup.py
--rw-r--r--   0        0        0      868 1970-01-01 00:00:00.000000 uc_browser-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0       63 2022-10-11 19:35:12.176241 uc_browser-0.3.4/README.md
+-rw-r--r--   0        0        0      503 2023-05-16 17:25:49.350475 uc_browser-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-10-11 19:35:12.176241 uc_browser-0.3.4/uc_browser/__init__.py
+-rw-r--r--   0        0        0     8159 2023-01-17 19:09:01.710189 uc_browser-0.3.4/uc_browser/browser.py
+-rw-r--r--   0        0        0    10611 2023-05-16 17:25:49.366476 uc_browser-0.3.4/uc_browser/browser_v2.py
+-rw-r--r--   0        0        0      802 1970-01-01 00:00:00.000000 uc_browser-0.3.4/setup.py
+-rw-r--r--   0        0        0      868 1970-01-01 00:00:00.000000 uc_browser-0.3.4/PKG-INFO
```

### Comparing `uc_browser-0.3.3/uc_browser/browser.py` & `uc_browser-0.3.4/uc_browser/browser.py`

 * *Files identical despite different names*

### Comparing `uc_browser-0.3.3/uc_browser/browser_v2.py` & `uc_browser-0.3.4/uc_browser/browser_v2.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,16 +107,16 @@
 
     def screenshot(self, filename):
         return self.driver.save_screenshot(filename)
 
     def get_href(self, xpath):
         return self.driver.find_element(By.XPATH, xpath).get_attribute('href')
 
-    def get_src(self, xpath):
-        return self.driver.find_element(By.XPATH, xpath).get_attribute('src')
+    def get_attribute(self, xpath, attribute):
+        return self.driver.find_element(By.XPATH, xpath).get_attribute(attribute)
 
     def input(self, xpath, send):
         self.driver.find_element(By.XPATH, xpath).send_keys(send)
 
     def input_like_a_human(self, xpath, send):
         element = self.driver.find_element(By.XPATH, xpath)
         for character in send:
```

### Comparing `uc_browser-0.3.3/setup.py` & `uc_browser-0.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['selenium-wire>=5.1.0,<6.0.0',
  'stem>=1.8.0,<2.0.0',
  'undetected-chromedriver>=3.1.5,<4.0.0',
  'webdriver-manager>=3.5.4,<4.0.0']
 
 setup_kwargs = {
     'name': 'uc-browser',
-    'version': '0.3.3',
+    'version': '0.3.4',
     'description': '',
     'long_description': '# browser\nModulo que implementa metodos para uso com selenium.\n',
     'author': 'Thiago Oliveira',
     'author_email': 'thiceconelo@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/ceconelo/browser',
```

### Comparing `uc_browser-0.3.3/PKG-INFO` & `uc_browser-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uc-browser
-Version: 0.3.3
+Version: 0.3.4
 Summary: 
 Home-page: https://github.com/ceconelo/browser
 License: MIT
 Author: Thiago Oliveira
 Author-email: thiceconelo@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

