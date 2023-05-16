# Comparing `tmp/tencentcloud-sdk-python-ecdn-3.0.890.tar.gz` & `tmp/tencentcloud-sdk-python-ecdn-3.0.892.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ecdn-3.0.890.tar", last modified: Fri May 12 02:09:40 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ecdn-3.0.892.tar", last modified: Tue May 16 00:35:56 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ecdn-3.0.890.tar` & `tencentcloud-sdk-python-ecdn-3.0.892.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 02:09:40.000000 tencentcloud-sdk-python-ecdn-3.0.890/
--rw-r--r--   0 root         (0) root         (0)      740 2023-05-12 02:09:40.000000 tencentcloud-sdk-python-ecdn-3.0.890/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 02:09:40.000000 tencentcloud-sdk-python-ecdn-3.0.890/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 02:09:40.000000 tencentcloud-sdk-python-ecdn-3.0.890/tencentcloud/ecdn/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 02:09:40.000000 tencentcloud-sdk-python-ecdn-3.0.890/tencentcloud/ecdn/v20191012/
--rw-r--r--   0 root         (0) root         (0)    20260 2023-05-12 02:09:40.000000 tencentcloud-sdk-python-ecdn-3.0.890/tencentcloud/ecdn/v20191012/ecdn_client.py
--rw-r--r--   0 root         (0) root         (0)     9084 2023-05-12 02:09:40.000000 tencentcloud-sdk-python-ecdn-3.0.890/tencentcloud/ecdn/v20191012/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-12 02:09:40.000000 tencentcloud-sdk-python-ecdn-3.0.890/tencentcloud/ecdn/v20191012/__init__.py
--rw-r--r--   0 root         (0) root         (0)    80852 2023-05-12 02:09:40.000000 tencentcloud-sdk-python-ecdn-3.0.890/tencentcloud/ecdn/v20191012/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-12 02:09:40.000000 tencentcloud-sdk-python-ecdn-3.0.890/tencentcloud/ecdn/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-12 02:09:40.000000 tencentcloud-sdk-python-ecdn-3.0.890/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1664 2023-05-12 02:09:40.000000 tencentcloud-sdk-python-ecdn-3.0.890/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1008 2023-05-12 02:09:40.000000 tencentcloud-sdk-python-ecdn-3.0.890/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-12 02:09:40.000000 tencentcloud-sdk-python-ecdn-3.0.890/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 02:09:40.000000 tencentcloud-sdk-python-ecdn-3.0.890/tencentcloud_sdk_python_ecdn.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-12 02:09:40.000000 tencentcloud-sdk-python-ecdn-3.0.890/tencentcloud_sdk_python_ecdn.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-05-12 02:09:40.000000 tencentcloud-sdk-python-ecdn-3.0.890/tencentcloud_sdk_python_ecdn.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-05-12 02:09:40.000000 tencentcloud-sdk-python-ecdn-3.0.890/tencentcloud_sdk_python_ecdn.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-12 02:09:40.000000 tencentcloud-sdk-python-ecdn-3.0.890/tencentcloud_sdk_python_ecdn.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:35:56.000000 tencentcloud-sdk-python-ecdn-3.0.892/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-05-16 00:35:56.000000 tencentcloud-sdk-python-ecdn-3.0.892/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:35:56.000000 tencentcloud-sdk-python-ecdn-3.0.892/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:35:56.000000 tencentcloud-sdk-python-ecdn-3.0.892/tencentcloud/ecdn/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:35:56.000000 tencentcloud-sdk-python-ecdn-3.0.892/tencentcloud/ecdn/v20191012/
+-rw-r--r--   0 root         (0) root         (0)    20260 2023-05-16 00:35:56.000000 tencentcloud-sdk-python-ecdn-3.0.892/tencentcloud/ecdn/v20191012/ecdn_client.py
+-rw-r--r--   0 root         (0) root         (0)     9084 2023-05-16 00:35:56.000000 tencentcloud-sdk-python-ecdn-3.0.892/tencentcloud/ecdn/v20191012/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 00:35:56.000000 tencentcloud-sdk-python-ecdn-3.0.892/tencentcloud/ecdn/v20191012/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    80852 2023-05-16 00:35:56.000000 tencentcloud-sdk-python-ecdn-3.0.892/tencentcloud/ecdn/v20191012/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 00:35:56.000000 tencentcloud-sdk-python-ecdn-3.0.892/tencentcloud/ecdn/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-16 00:35:56.000000 tencentcloud-sdk-python-ecdn-3.0.892/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-05-16 00:35:56.000000 tencentcloud-sdk-python-ecdn-3.0.892/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-05-16 00:35:56.000000 tencentcloud-sdk-python-ecdn-3.0.892/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-16 00:35:56.000000 tencentcloud-sdk-python-ecdn-3.0.892/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:35:56.000000 tencentcloud-sdk-python-ecdn-3.0.892/tencentcloud_sdk_python_ecdn.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 00:35:56.000000 tencentcloud-sdk-python-ecdn-3.0.892/tencentcloud_sdk_python_ecdn.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-05-16 00:35:56.000000 tencentcloud-sdk-python-ecdn-3.0.892/tencentcloud_sdk_python_ecdn.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-05-16 00:35:56.000000 tencentcloud-sdk-python-ecdn-3.0.892/tencentcloud_sdk_python_ecdn.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-16 00:35:56.000000 tencentcloud-sdk-python-ecdn-3.0.892/tencentcloud_sdk_python_ecdn.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-ecdn-3.0.890/README.rst` & `tencentcloud-sdk-python-ecdn-3.0.892/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ecdn-3.0.890/tencentcloud/ecdn/v20191012/ecdn_client.py` & `tencentcloud-sdk-python-ecdn-3.0.892/tencentcloud/ecdn/v20191012/ecdn_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ecdn-3.0.890/tencentcloud/ecdn/v20191012/errorcodes.py` & `tencentcloud-sdk-python-ecdn-3.0.892/tencentcloud/ecdn/v20191012/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ecdn-3.0.890/tencentcloud/ecdn/v20191012/models.py` & `tencentcloud-sdk-python-ecdn-3.0.892/tencentcloud/ecdn/v20191012/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ecdn-3.0.890/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ecdn-3.0.892/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.890'
+__version__ = '3.0.892'
```

### Comparing `tencentcloud-sdk-python-ecdn-3.0.890/PKG-INFO` & `tencentcloud-sdk-python-ecdn-3.0.892/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ecdn
-Version: 3.0.890
+Version: 3.0.892
 Summary: Tencent Cloud Ecdn SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ecdn-3.0.890/setup.py` & `tencentcloud-sdk-python-ecdn-3.0.892/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ecdn-3.0.890/tencentcloud_sdk_python_ecdn.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ecdn-3.0.892/tencentcloud_sdk_python_ecdn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ecdn
-Version: 3.0.890
+Version: 3.0.892
 Summary: Tencent Cloud Ecdn SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```
