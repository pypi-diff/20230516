# Comparing `tmp/tencentcloud-sdk-python-tiia-3.0.891.tar.gz` & `tmp/tencentcloud-sdk-python-tiia-3.0.892.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tiia-3.0.891.tar", last modified: Mon May 15 04:42:27 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tiia-3.0.892.tar", last modified: Tue May 16 00:48:19 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tiia-3.0.891.tar` & `tencentcloud-sdk-python-tiia-3.0.892.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:42:27.000000 tencentcloud-sdk-python-tiia-3.0.891/
--rw-r--r--   0 root         (0) root         (0)      740 2023-05-15 04:42:26.000000 tencentcloud-sdk-python-tiia-3.0.891/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:42:27.000000 tencentcloud-sdk-python-tiia-3.0.891/tencentcloud_sdk_python_tiia.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 04:42:27.000000 tencentcloud-sdk-python-tiia-3.0.891/tencentcloud_sdk_python_tiia.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-05-15 04:42:27.000000 tencentcloud-sdk-python-tiia-3.0.891/tencentcloud_sdk_python_tiia.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-05-15 04:42:27.000000 tencentcloud-sdk-python-tiia-3.0.891/tencentcloud_sdk_python_tiia.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-15 04:42:27.000000 tencentcloud-sdk-python-tiia-3.0.891/tencentcloud_sdk_python_tiia.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:42:27.000000 tencentcloud-sdk-python-tiia-3.0.891/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-15 04:42:26.000000 tencentcloud-sdk-python-tiia-3.0.891/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:42:27.000000 tencentcloud-sdk-python-tiia-3.0.891/tencentcloud/tiia/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:42:27.000000 tencentcloud-sdk-python-tiia-3.0.891/tencentcloud/tiia/v20190529/
--rw-r--r--   0 root         (0) root         (0)    32444 2023-05-15 04:42:26.000000 tencentcloud-sdk-python-tiia-3.0.891/tencentcloud/tiia/v20190529/tiia_client.py
--rw-r--r--   0 root         (0) root         (0)     7113 2023-05-15 04:42:26.000000 tencentcloud-sdk-python-tiia-3.0.891/tencentcloud/tiia/v20190529/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 04:42:26.000000 tencentcloud-sdk-python-tiia-3.0.891/tencentcloud/tiia/v20190529/__init__.py
--rw-r--r--   0 root         (0) root         (0)   102357 2023-05-15 04:42:26.000000 tencentcloud-sdk-python-tiia-3.0.891/tencentcloud/tiia/v20190529/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 04:42:26.000000 tencentcloud-sdk-python-tiia-3.0.891/tencentcloud/tiia/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1664 2023-05-15 04:42:27.000000 tencentcloud-sdk-python-tiia-3.0.891/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1008 2023-05-15 04:42:26.000000 tencentcloud-sdk-python-tiia-3.0.891/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-15 04:42:27.000000 tencentcloud-sdk-python-tiia-3.0.891/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:48:19.000000 tencentcloud-sdk-python-tiia-3.0.892/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-05-16 00:48:19.000000 tencentcloud-sdk-python-tiia-3.0.892/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:48:19.000000 tencentcloud-sdk-python-tiia-3.0.892/tencentcloud_sdk_python_tiia.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 00:48:19.000000 tencentcloud-sdk-python-tiia-3.0.892/tencentcloud_sdk_python_tiia.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-05-16 00:48:19.000000 tencentcloud-sdk-python-tiia-3.0.892/tencentcloud_sdk_python_tiia.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-05-16 00:48:19.000000 tencentcloud-sdk-python-tiia-3.0.892/tencentcloud_sdk_python_tiia.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-16 00:48:19.000000 tencentcloud-sdk-python-tiia-3.0.892/tencentcloud_sdk_python_tiia.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:48:19.000000 tencentcloud-sdk-python-tiia-3.0.892/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-16 00:48:19.000000 tencentcloud-sdk-python-tiia-3.0.892/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:48:19.000000 tencentcloud-sdk-python-tiia-3.0.892/tencentcloud/tiia/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:48:19.000000 tencentcloud-sdk-python-tiia-3.0.892/tencentcloud/tiia/v20190529/
+-rw-r--r--   0 root         (0) root         (0)    32444 2023-05-16 00:48:19.000000 tencentcloud-sdk-python-tiia-3.0.892/tencentcloud/tiia/v20190529/tiia_client.py
+-rw-r--r--   0 root         (0) root         (0)     7113 2023-05-16 00:48:19.000000 tencentcloud-sdk-python-tiia-3.0.892/tencentcloud/tiia/v20190529/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 00:48:19.000000 tencentcloud-sdk-python-tiia-3.0.892/tencentcloud/tiia/v20190529/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   102357 2023-05-16 00:48:19.000000 tencentcloud-sdk-python-tiia-3.0.892/tencentcloud/tiia/v20190529/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 00:48:19.000000 tencentcloud-sdk-python-tiia-3.0.892/tencentcloud/tiia/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-05-16 00:48:19.000000 tencentcloud-sdk-python-tiia-3.0.892/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-05-16 00:48:19.000000 tencentcloud-sdk-python-tiia-3.0.892/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-16 00:48:19.000000 tencentcloud-sdk-python-tiia-3.0.892/setup.cfg
```

### Comparing `tencentcloud-sdk-python-tiia-3.0.891/README.rst` & `tencentcloud-sdk-python-tiia-3.0.892/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tiia-3.0.891/tencentcloud_sdk_python_tiia.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tiia-3.0.892/tencentcloud_sdk_python_tiia.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tiia
-Version: 3.0.891
+Version: 3.0.892
 Summary: Tencent Cloud Tiia SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tiia-3.0.891/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tiia-3.0.892/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.891'
+__version__ = '3.0.892'
```

### Comparing `tencentcloud-sdk-python-tiia-3.0.891/tencentcloud/tiia/v20190529/tiia_client.py` & `tencentcloud-sdk-python-tiia-3.0.892/tencentcloud/tiia/v20190529/tiia_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tiia-3.0.891/tencentcloud/tiia/v20190529/errorcodes.py` & `tencentcloud-sdk-python-tiia-3.0.892/tencentcloud/tiia/v20190529/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tiia-3.0.891/tencentcloud/tiia/v20190529/models.py` & `tencentcloud-sdk-python-tiia-3.0.892/tencentcloud/tiia/v20190529/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tiia-3.0.891/PKG-INFO` & `tencentcloud-sdk-python-tiia-3.0.892/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tiia
-Version: 3.0.891
+Version: 3.0.892
 Summary: Tencent Cloud Tiia SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tiia-3.0.891/setup.py` & `tencentcloud-sdk-python-tiia-3.0.892/setup.py`

 * *Files identical despite different names*
