# Comparing `tmp/PyOdoo-0.5.7.tar.gz` & `tmp/PyOdoo-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyOdoo-0.5.7.tar", last modified: Sun Mar 19 11:00:46 2023, max compression
+gzip compressed data, was "PyOdoo-0.5.8.tar", last modified: Mon May 15 23:54:18 2023, max compression
```

## Comparing `PyOdoo-0.5.7.tar` & `PyOdoo-0.5.8.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 muflone   (1000) users      (985)        0 2023-03-19 11:00:46.799721 PyOdoo-0.5.7/
--rw-r--r--   0 muflone   (1000) users      (985)      613 2021-05-09 18:22:23.000000 PyOdoo-0.5.7/LICENSE
--rw-r--r--   0 muflone   (1000) users      (985)     1711 2023-03-19 11:00:46.799721 PyOdoo-0.5.7/PKG-INFO
-drwxr-xr-x   0 muflone   (1000) users      (985)        0 2023-03-19 11:00:46.796388 PyOdoo-0.5.7/PyOdoo.egg-info/
--rw-r--r--   0 muflone   (1000) users      (985)     1711 2023-03-19 11:00:46.000000 PyOdoo-0.5.7/PyOdoo.egg-info/PKG-INFO
--rw-r--r--   0 muflone   (1000) users      (985)      524 2023-03-19 11:00:46.000000 PyOdoo-0.5.7/PyOdoo.egg-info/SOURCES.txt
--rw-r--r--   0 muflone   (1000) users      (985)        1 2023-03-19 11:00:46.000000 PyOdoo-0.5.7/PyOdoo.egg-info/dependency_links.txt
--rw-r--r--   0 muflone   (1000) users      (985)        7 2023-03-19 11:00:46.000000 PyOdoo-0.5.7/PyOdoo.egg-info/top_level.txt
--rw-r--r--   0 muflone   (1000) users      (985)     1014 2023-02-05 04:31:04.000000 PyOdoo-0.5.7/README.md
-drwxr-xr-x   0 muflone   (1000) users      (985)        0 2023-03-19 11:00:46.796388 PyOdoo-0.5.7/pyodoo/
--rw-r--r--   0 muflone   (1000) users      (985)     1306 2023-02-05 04:31:04.000000 PyOdoo-0.5.7/pyodoo/__init__.py
--rw-r--r--   0 muflone   (1000) users      (985)     1004 2023-02-05 04:31:04.000000 PyOdoo-0.5.7/pyodoo/active_status_choice.py
--rw-r--r--   0 muflone   (1000) users      (985)      956 2023-02-05 04:31:04.000000 PyOdoo-0.5.7/pyodoo/boolean_operator.py
--rw-r--r--   0 muflone   (1000) users      (985)     1114 2023-02-05 04:31:04.000000 PyOdoo-0.5.7/pyodoo/compare_type.py
--rw-r--r--   0 muflone   (1000) users      (985)     1227 2023-03-19 10:11:36.000000 PyOdoo-0.5.7/pyodoo/constants.py
--rw-r--r--   0 muflone   (1000) users      (985)     1502 2023-02-05 04:31:04.000000 PyOdoo-0.5.7/pyodoo/filter.py
--rw-r--r--   0 muflone   (1000) users      (985)     1008 2023-02-05 04:31:04.000000 PyOdoo-0.5.7/pyodoo/message_subtype.py
-drwxr-xr-x   0 muflone   (1000) users      (985)        0 2023-03-19 11:00:46.796388 PyOdoo-0.5.7/pyodoo/samples/
--rw-r--r--   0 muflone   (1000) users      (985)        0 2022-09-23 22:59:11.000000 PyOdoo-0.5.7/pyodoo/samples/__init__.py
--rw-r--r--   0 muflone   (1000) users      (985)     1345 2023-02-05 04:31:04.000000 PyOdoo-0.5.7/pyodoo/samples/awaitable.py
--rw-r--r--   0 muflone   (1000) users      (985)     5169 2023-03-19 10:57:46.000000 PyOdoo-0.5.7/pyodoo/samples/contacts.py
--rw-r--r--   0 muflone   (1000) users      (985)     3666 2023-02-05 16:20:33.000000 PyOdoo-0.5.7/pyodoo/samples/contacts_async.py
-drwxr-xr-x   0 muflone   (1000) users      (985)        0 2023-03-19 11:00:46.796388 PyOdoo-0.5.7/pyodoo/v12/
--rw-r--r--   0 muflone   (1000) users      (985)      986 2023-02-05 04:31:04.000000 PyOdoo-0.5.7/pyodoo/v12/__init__.py
--rw-r--r--   0 muflone   (1000) users      (985)    11089 2023-02-05 18:02:47.000000 PyOdoo-0.5.7/pyodoo/v12/api.py
--rw-r--r--   0 muflone   (1000) users      (985)    32118 2023-03-19 10:22:52.000000 PyOdoo-0.5.7/pyodoo/v12/model.py
--rw-r--r--   0 muflone   (1000) users      (985)       90 2022-01-06 22:44:31.000000 PyOdoo-0.5.7/pyproject.toml
--rw-r--r--   0 muflone   (1000) users      (985)      843 2023-03-19 11:00:46.799721 PyOdoo-0.5.7/setup.cfg
-drwxr-xr-x   0 muflone   (1000) users      (985)        0 2023-03-19 11:00:46.796388 PyOdoo-0.5.7/tests/
--rw-r--r--   0 muflone   (1000) users      (985)    33963 2023-03-19 10:51:32.000000 PyOdoo-0.5.7/tests/test_contacts.py
+drwxr-xr-x   0 muflone   (1000) users      (985)        0 2023-05-15 23:54:18.495422 PyOdoo-0.5.8/
+-rw-r--r--   0 muflone   (1000) users      (985)      613 2021-05-09 18:22:23.000000 PyOdoo-0.5.8/LICENSE
+-rw-r--r--   0 muflone   (1000) users      (985)     1762 2023-05-15 23:54:18.495422 PyOdoo-0.5.8/PKG-INFO
+drwxr-xr-x   0 muflone   (1000) users      (985)        0 2023-05-15 23:54:18.492088 PyOdoo-0.5.8/PyOdoo.egg-info/
+-rw-r--r--   0 muflone   (1000) users      (985)     1762 2023-05-15 23:54:18.000000 PyOdoo-0.5.8/PyOdoo.egg-info/PKG-INFO
+-rw-r--r--   0 muflone   (1000) users      (985)      552 2023-05-15 23:54:18.000000 PyOdoo-0.5.8/PyOdoo.egg-info/SOURCES.txt
+-rw-r--r--   0 muflone   (1000) users      (985)        1 2023-05-15 23:54:18.000000 PyOdoo-0.5.8/PyOdoo.egg-info/dependency_links.txt
+-rw-r--r--   0 muflone   (1000) users      (985)        7 2023-05-15 23:54:18.000000 PyOdoo-0.5.8/PyOdoo.egg-info/top_level.txt
+-rw-r--r--   0 muflone   (1000) users      (985)     1014 2023-02-05 04:31:04.000000 PyOdoo-0.5.8/README.md
+drwxr-xr-x   0 muflone   (1000) users      (985)        0 2023-05-15 23:54:18.492088 PyOdoo-0.5.8/pyodoo/
+-rw-r--r--   0 muflone   (1000) users      (985)     1306 2023-02-05 04:31:04.000000 PyOdoo-0.5.8/pyodoo/__init__.py
+-rw-r--r--   0 muflone   (1000) users      (985)     1004 2023-02-05 04:31:04.000000 PyOdoo-0.5.8/pyodoo/active_status_choice.py
+-rw-r--r--   0 muflone   (1000) users      (985)      956 2023-02-05 04:31:04.000000 PyOdoo-0.5.8/pyodoo/boolean_operator.py
+-rw-r--r--   0 muflone   (1000) users      (985)     1365 2023-05-15 23:49:57.000000 PyOdoo-0.5.8/pyodoo/compare_type.py
+-rw-r--r--   0 muflone   (1000) users      (985)     1227 2023-05-13 15:49:56.000000 PyOdoo-0.5.8/pyodoo/constants.py
+-rw-r--r--   0 muflone   (1000) users      (985)     1502 2023-02-05 04:31:04.000000 PyOdoo-0.5.8/pyodoo/filter.py
+-rw-r--r--   0 muflone   (1000) users      (985)     1008 2023-02-05 04:31:04.000000 PyOdoo-0.5.8/pyodoo/message_subtype.py
+drwxr-xr-x   0 muflone   (1000) users      (985)        0 2023-05-15 23:54:18.492088 PyOdoo-0.5.8/pyodoo/samples/
+-rw-r--r--   0 muflone   (1000) users      (985)        0 2022-09-23 22:59:11.000000 PyOdoo-0.5.8/pyodoo/samples/__init__.py
+-rw-r--r--   0 muflone   (1000) users      (985)     1345 2023-02-05 04:31:04.000000 PyOdoo-0.5.8/pyodoo/samples/awaitable.py
+-rw-r--r--   0 muflone   (1000) users      (985)     5169 2023-03-19 10:57:46.000000 PyOdoo-0.5.8/pyodoo/samples/contacts.py
+-rw-r--r--   0 muflone   (1000) users      (985)     3666 2023-02-05 16:20:33.000000 PyOdoo-0.5.8/pyodoo/samples/contacts_async.py
+drwxr-xr-x   0 muflone   (1000) users      (985)        0 2023-05-15 23:54:18.492088 PyOdoo-0.5.8/pyodoo/v12/
+-rw-r--r--   0 muflone   (1000) users      (985)      986 2023-02-05 04:31:04.000000 PyOdoo-0.5.8/pyodoo/v12/__init__.py
+-rw-r--r--   0 muflone   (1000) users      (985)    11089 2023-02-05 18:02:47.000000 PyOdoo-0.5.8/pyodoo/v12/api.py
+-rw-r--r--   0 muflone   (1000) users      (985)    32118 2023-03-19 10:22:52.000000 PyOdoo-0.5.8/pyodoo/v12/model.py
+-rw-r--r--   0 muflone   (1000) users      (985)       90 2022-01-06 22:44:31.000000 PyOdoo-0.5.8/pyproject.toml
+-rw-r--r--   0 muflone   (1000) users      (985)      883 2023-05-15 23:54:18.495422 PyOdoo-0.5.8/setup.cfg
+drwxr-xr-x   0 muflone   (1000) users      (985)        0 2023-05-15 23:54:18.495422 PyOdoo-0.5.8/tests/
+-rw-r--r--   0 muflone   (1000) users      (985)    16600 2023-05-15 23:49:57.000000 PyOdoo-0.5.8/tests/test_compare_types.py
+-rw-r--r--   0 muflone   (1000) users      (985)    33179 2023-05-13 16:57:45.000000 PyOdoo-0.5.8/tests/test_contacts.py
```

### Comparing `PyOdoo-0.5.7/LICENSE` & `PyOdoo-0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `PyOdoo-0.5.7/PKG-INFO` & `PyOdoo-0.5.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: PyOdoo
-Version: 0.5.7
+Version: 0.5.8
 Summary: API for Odoo
 Home-page: http://www.muflone.com/pyodoo/
 Author: Fabio Castelli
 Author-email: muflone@muflone.com
 License: GPLv3+
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PyOdoo
 
 [![Travis CI Build Status](https://img.shields.io/travis/com/muflone/pyodoo/master.svg)](https://www.travis-ci.com/github/muflone/pyodoo)
```

### Comparing `PyOdoo-0.5.7/PyOdoo.egg-info/PKG-INFO` & `PyOdoo-0.5.8/PyOdoo.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: PyOdoo
-Version: 0.5.7
+Version: 0.5.8
 Summary: API for Odoo
 Home-page: http://www.muflone.com/pyodoo/
 Author: Fabio Castelli
 Author-email: muflone@muflone.com
 License: GPLv3+
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PyOdoo
 
 [![Travis CI Build Status](https://img.shields.io/travis/com/muflone/pyodoo/master.svg)](https://www.travis-ci.com/github/muflone/pyodoo)
```

### Comparing `PyOdoo-0.5.7/README.md` & `PyOdoo-0.5.8/README.md`

 * *Files identical despite different names*

### Comparing `PyOdoo-0.5.7/pyodoo/__init__.py` & `PyOdoo-0.5.8/pyodoo/__init__.py`

 * *Files identical despite different names*

### Comparing `PyOdoo-0.5.7/pyodoo/active_status_choice.py` & `PyOdoo-0.5.8/pyodoo/active_status_choice.py`

 * *Files identical despite different names*

### Comparing `PyOdoo-0.5.7/pyodoo/boolean_operator.py` & `PyOdoo-0.5.8/pyodoo/boolean_operator.py`

 * *Files identical despite different names*

### Comparing `PyOdoo-0.5.7/pyodoo/compare_type.py` & `PyOdoo-0.5.8/pyodoo/compare_type.py`

 * *Files 15% similar despite different names*

```diff
@@ -28,7 +28,17 @@
     GREATER_EQ = '>='
     LOWER = '<'
     LOWER_EQ = '<='
     IN = 'in'
     NOT_IN = 'not in'
     CONTAINS = 'ilike'
     CONTAINS_NOT = 'not ilike'
+    NOT_CONTAINS = 'not ilike'
+    LIKE = 'like'
+    NOT_LIKE = 'not like'
+    ILIKE = 'ilike'
+    NOT_ILIKE = 'not ilike'
+    RAW_LIKE = '=like'
+    RAW_ILIKE = '=ilike'
+    UNSET_OR_EQUAL = '=?'
+    CHILD_OF = 'child_of'
+    PARENT_OF = 'parent_of'
```

### Comparing `PyOdoo-0.5.7/pyodoo/constants.py` & `PyOdoo-0.5.8/pyodoo/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 #  GNU General Public License for more details.
 #
 #  You should have received a copy of the GNU General Public License
 #  along with this program.  If not, see <https://www.gnu.org/licenses/>.
 ##
 
 APP_NAME = 'PyOdoo'
-APP_VERSION = '0.5.7'
+APP_VERSION = '0.5.8'
 APP_DESCRIPTION = 'API for Odoo'
 APP_DOMAIN = 'pyodoo'
 APP_ID = f'{APP_DOMAIN}.muflone.com'
 APP_AUTHOR = 'Fabio Castelli'
 APP_AUTHOR_EMAIL = 'muflone@muflone.com'
 APP_COPYRIGHT = f'Copyright 2021-2023 {APP_AUTHOR}'
 URL_AUTHOR = 'http://www.muflone.com/'
```

### Comparing `PyOdoo-0.5.7/pyodoo/filter.py` & `PyOdoo-0.5.8/pyodoo/filter.py`

 * *Files identical despite different names*

### Comparing `PyOdoo-0.5.7/pyodoo/message_subtype.py` & `PyOdoo-0.5.8/pyodoo/message_subtype.py`

 * *Files identical despite different names*

### Comparing `PyOdoo-0.5.7/pyodoo/samples/awaitable.py` & `PyOdoo-0.5.8/pyodoo/samples/awaitable.py`

 * *Files identical despite different names*

### Comparing `PyOdoo-0.5.7/pyodoo/samples/contacts.py` & `PyOdoo-0.5.8/pyodoo/samples/contacts.py`

 * *Files identical despite different names*

### Comparing `PyOdoo-0.5.7/pyodoo/samples/contacts_async.py` & `PyOdoo-0.5.8/pyodoo/samples/contacts_async.py`

 * *Files identical despite different names*

### Comparing `PyOdoo-0.5.7/pyodoo/v12/__init__.py` & `PyOdoo-0.5.8/pyodoo/v12/__init__.py`

 * *Files identical despite different names*

### Comparing `PyOdoo-0.5.7/pyodoo/v12/api.py` & `PyOdoo-0.5.8/pyodoo/v12/api.py`

 * *Files identical despite different names*

### Comparing `PyOdoo-0.5.7/pyodoo/v12/model.py` & `PyOdoo-0.5.8/pyodoo/v12/model.py`

 * *Files identical despite different names*

### Comparing `PyOdoo-0.5.7/setup.cfg` & `PyOdoo-0.5.8/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 	Development Status :: 1 - Planning
 	Intended Audience :: Developers
 	License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Topic :: Software Development :: Libraries :: Python Modules
 
 [options]
 packages = 
 	pyodoo
 	pyodoo.v12
 include_package_data = False
```

### Comparing `PyOdoo-0.5.7/tests/test_contacts.py` & `PyOdoo-0.5.8/tests/test_contacts.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,39 +25,24 @@
                     BooleanOperator,
                     CompareType,
                     Filter,
                     MessageSubType)
 from pyodoo.constants import APP_AUTHOR_EMAIL, APP_NAME, APP_VERSION
 from pyodoo.v12 import Model
 
+import utility
+
 
 class TestCaseContacts(unittest.TestCase):
     @classmethod
     def setUpClass(cls):
         """
         Model object preparation
         """
-        # Get the free public server credentials
-        try:
-            info = xmlrpc.client.ServerProxy(
-                uri='https://demo.odoo.com/start').start()
-        except xmlrpc.client.Fault:
-            # Sometimes the free public server start page is not available
-            # Use a specif instance (this may be very mutable)
-            info = {'host': 'https://demo4.odoo.com',
-                    'database': 'demo_160_1676157153',
-                    'user': 'admin',
-                    'password': 'admin'}
-        cls.model = Model(model_name='res.partner',
-                          endpoint=info['host'],
-                          database=info['database'],
-                          username=info['user'],
-                          password=info['password'],
-                          language='en_US',
-                          authenticate=False)
+        cls.model = utility.get_model_from_demo(model_name='res.partner')
 
     def test_01_authenticate(self) -> None:
         """
         Check the authentication
         """
         results = self.model.authenticate()
         # Check if the user ID is not None
```

