# Comparing `tmp/tencentcloud-sdk-python-waf-3.0.889.tar.gz` & `tmp/tencentcloud-sdk-python-waf-3.0.891.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-waf-3.0.889.tar", last modified: Thu May 11 03:29:00 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-waf-3.0.891.tar", last modified: Mon May 15 04:56:06 2023, max compression
```

## Comparing `tencentcloud-sdk-python-waf-3.0.889.tar` & `tencentcloud-sdk-python-waf-3.0.891.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 03:29:00.000000 tencentcloud-sdk-python-waf-3.0.889/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-11 03:29:00.000000 tencentcloud-sdk-python-waf-3.0.889/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 03:29:00.000000 tencentcloud-sdk-python-waf-3.0.889/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 03:29:00.000000 tencentcloud-sdk-python-waf-3.0.889/tencentcloud/waf/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 03:29:00.000000 tencentcloud-sdk-python-waf-3.0.889/tencentcloud/waf/v20180125/
--rw-r--r--   0 root         (0) root         (0)    46563 2023-05-11 03:29:00.000000 tencentcloud-sdk-python-waf-3.0.889/tencentcloud/waf/v20180125/waf_client.py
--rw-r--r--   0 root         (0) root         (0)     2513 2023-05-11 03:29:00.000000 tencentcloud-sdk-python-waf-3.0.889/tencentcloud/waf/v20180125/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 03:29:00.000000 tencentcloud-sdk-python-waf-3.0.889/tencentcloud/waf/v20180125/__init__.py
--rw-r--r--   0 root         (0) root         (0)   180125 2023-05-11 03:29:00.000000 tencentcloud-sdk-python-waf-3.0.889/tencentcloud/waf/v20180125/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 03:29:00.000000 tencentcloud-sdk-python-waf-3.0.889/tencentcloud/waf/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-11 03:29:00.000000 tencentcloud-sdk-python-waf-3.0.889/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-11 03:29:00.000000 tencentcloud-sdk-python-waf-3.0.889/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-11 03:29:00.000000 tencentcloud-sdk-python-waf-3.0.889/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-11 03:29:00.000000 tencentcloud-sdk-python-waf-3.0.889/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 03:29:00.000000 tencentcloud-sdk-python-waf-3.0.889/tencentcloud_sdk_python_waf.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 03:29:00.000000 tencentcloud-sdk-python-waf-3.0.889/tencentcloud_sdk_python_waf.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-11 03:29:00.000000 tencentcloud-sdk-python-waf-3.0.889/tencentcloud_sdk_python_waf.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-11 03:29:00.000000 tencentcloud-sdk-python-waf-3.0.889/tencentcloud_sdk_python_waf.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-11 03:29:00.000000 tencentcloud-sdk-python-waf-3.0.889/tencentcloud_sdk_python_waf.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:56:06.000000 tencentcloud-sdk-python-waf-3.0.891/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-15 04:56:06.000000 tencentcloud-sdk-python-waf-3.0.891/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:56:06.000000 tencentcloud-sdk-python-waf-3.0.891/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:56:06.000000 tencentcloud-sdk-python-waf-3.0.891/tencentcloud/waf/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:56:06.000000 tencentcloud-sdk-python-waf-3.0.891/tencentcloud/waf/v20180125/
+-rw-r--r--   0 root         (0) root         (0)    46563 2023-05-15 04:56:06.000000 tencentcloud-sdk-python-waf-3.0.891/tencentcloud/waf/v20180125/waf_client.py
+-rw-r--r--   0 root         (0) root         (0)     2513 2023-05-15 04:56:06.000000 tencentcloud-sdk-python-waf-3.0.891/tencentcloud/waf/v20180125/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 04:56:06.000000 tencentcloud-sdk-python-waf-3.0.891/tencentcloud/waf/v20180125/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   180125 2023-05-15 04:56:06.000000 tencentcloud-sdk-python-waf-3.0.891/tencentcloud/waf/v20180125/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 04:56:06.000000 tencentcloud-sdk-python-waf-3.0.891/tencentcloud/waf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-15 04:56:06.000000 tencentcloud-sdk-python-waf-3.0.891/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-15 04:56:06.000000 tencentcloud-sdk-python-waf-3.0.891/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-15 04:56:06.000000 tencentcloud-sdk-python-waf-3.0.891/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-15 04:56:06.000000 tencentcloud-sdk-python-waf-3.0.891/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:56:06.000000 tencentcloud-sdk-python-waf-3.0.891/tencentcloud_sdk_python_waf.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 04:56:06.000000 tencentcloud-sdk-python-waf-3.0.891/tencentcloud_sdk_python_waf.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-15 04:56:06.000000 tencentcloud-sdk-python-waf-3.0.891/tencentcloud_sdk_python_waf.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-15 04:56:06.000000 tencentcloud-sdk-python-waf-3.0.891/tencentcloud_sdk_python_waf.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-15 04:56:06.000000 tencentcloud-sdk-python-waf-3.0.891/tencentcloud_sdk_python_waf.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-waf-3.0.889/README.rst` & `tencentcloud-sdk-python-waf-3.0.891/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-waf-3.0.889/tencentcloud/waf/v20180125/waf_client.py` & `tencentcloud-sdk-python-waf-3.0.891/tencentcloud/waf/v20180125/waf_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-waf-3.0.889/tencentcloud/waf/v20180125/errorcodes.py` & `tencentcloud-sdk-python-waf-3.0.891/tencentcloud/waf/v20180125/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-waf-3.0.889/tencentcloud/waf/v20180125/models.py` & `tencentcloud-sdk-python-waf-3.0.891/tencentcloud/waf/v20180125/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-waf-3.0.889/tencentcloud/__init__.py` & `tencentcloud-sdk-python-waf-3.0.891/tencentcloud/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.889'
+__version__ = '3.0.891'
```

### Comparing `tencentcloud-sdk-python-waf-3.0.889/PKG-INFO` & `tencentcloud-sdk-python-waf-3.0.891/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-waf
-Version: 3.0.889
+Version: 3.0.891
 Summary: Tencent Cloud Waf SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-waf-3.0.889/setup.py` & `tencentcloud-sdk-python-waf-3.0.891/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-waf-3.0.889/tencentcloud_sdk_python_waf.egg-info/PKG-INFO` & `tencentcloud-sdk-python-waf-3.0.891/tencentcloud_sdk_python_waf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-waf
-Version: 3.0.889
+Version: 3.0.891
 Summary: Tencent Cloud Waf SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

