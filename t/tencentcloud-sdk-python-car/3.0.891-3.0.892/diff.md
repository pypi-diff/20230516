# Comparing `tmp/tencentcloud-sdk-python-car-3.0.891.tar.gz` & `tmp/tencentcloud-sdk-python-car-3.0.892.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-car-3.0.891.tar", last modified: Mon May 15 02:36:21 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-car-3.0.892.tar", last modified: Tue May 16 00:30:09 2023, max compression
```

## Comparing `tencentcloud-sdk-python-car-3.0.891.tar` & `tencentcloud-sdk-python-car-3.0.892.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 02:36:21.000000 tencentcloud-sdk-python-car-3.0.891/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-15 02:36:21.000000 tencentcloud-sdk-python-car-3.0.891/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 02:36:21.000000 tencentcloud-sdk-python-car-3.0.891/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 02:36:21.000000 tencentcloud-sdk-python-car-3.0.891/tencentcloud/car/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 02:36:21.000000 tencentcloud-sdk-python-car-3.0.891/tencentcloud/car/v20220110/
--rw-r--r--   0 root         (0) root         (0)     1781 2023-05-15 02:36:21.000000 tencentcloud-sdk-python-car-3.0.891/tencentcloud/car/v20220110/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 02:36:21.000000 tencentcloud-sdk-python-car-3.0.891/tencentcloud/car/v20220110/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5256 2023-05-15 02:36:21.000000 tencentcloud-sdk-python-car-3.0.891/tencentcloud/car/v20220110/car_client.py
--rw-r--r--   0 root         (0) root         (0)     9309 2023-05-15 02:36:21.000000 tencentcloud-sdk-python-car-3.0.891/tencentcloud/car/v20220110/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 02:36:21.000000 tencentcloud-sdk-python-car-3.0.891/tencentcloud/car/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-15 02:36:21.000000 tencentcloud-sdk-python-car-3.0.891/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-15 02:36:21.000000 tencentcloud-sdk-python-car-3.0.891/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-15 02:36:21.000000 tencentcloud-sdk-python-car-3.0.891/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-15 02:36:21.000000 tencentcloud-sdk-python-car-3.0.891/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 02:36:21.000000 tencentcloud-sdk-python-car-3.0.891/tencentcloud_sdk_python_car.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 02:36:21.000000 tencentcloud-sdk-python-car-3.0.891/tencentcloud_sdk_python_car.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-15 02:36:21.000000 tencentcloud-sdk-python-car-3.0.891/tencentcloud_sdk_python_car.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-15 02:36:21.000000 tencentcloud-sdk-python-car-3.0.891/tencentcloud_sdk_python_car.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-15 02:36:21.000000 tencentcloud-sdk-python-car-3.0.891/tencentcloud_sdk_python_car.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:30:09.000000 tencentcloud-sdk-python-car-3.0.892/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-16 00:30:09.000000 tencentcloud-sdk-python-car-3.0.892/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:30:09.000000 tencentcloud-sdk-python-car-3.0.892/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:30:09.000000 tencentcloud-sdk-python-car-3.0.892/tencentcloud/car/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:30:09.000000 tencentcloud-sdk-python-car-3.0.892/tencentcloud/car/v20220110/
+-rw-r--r--   0 root         (0) root         (0)     1781 2023-05-16 00:30:09.000000 tencentcloud-sdk-python-car-3.0.892/tencentcloud/car/v20220110/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 00:30:09.000000 tencentcloud-sdk-python-car-3.0.892/tencentcloud/car/v20220110/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5256 2023-05-16 00:30:09.000000 tencentcloud-sdk-python-car-3.0.892/tencentcloud/car/v20220110/car_client.py
+-rw-r--r--   0 root         (0) root         (0)     9309 2023-05-16 00:30:09.000000 tencentcloud-sdk-python-car-3.0.892/tencentcloud/car/v20220110/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 00:30:09.000000 tencentcloud-sdk-python-car-3.0.892/tencentcloud/car/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-16 00:30:09.000000 tencentcloud-sdk-python-car-3.0.892/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-16 00:30:09.000000 tencentcloud-sdk-python-car-3.0.892/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-16 00:30:09.000000 tencentcloud-sdk-python-car-3.0.892/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-16 00:30:09.000000 tencentcloud-sdk-python-car-3.0.892/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:30:09.000000 tencentcloud-sdk-python-car-3.0.892/tencentcloud_sdk_python_car.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 00:30:09.000000 tencentcloud-sdk-python-car-3.0.892/tencentcloud_sdk_python_car.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-16 00:30:09.000000 tencentcloud-sdk-python-car-3.0.892/tencentcloud_sdk_python_car.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-16 00:30:09.000000 tencentcloud-sdk-python-car-3.0.892/tencentcloud_sdk_python_car.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-16 00:30:09.000000 tencentcloud-sdk-python-car-3.0.892/tencentcloud_sdk_python_car.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-car-3.0.891/README.rst` & `tencentcloud-sdk-python-car-3.0.892/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-car-3.0.891/tencentcloud/car/v20220110/errorcodes.py` & `tencentcloud-sdk-python-car-3.0.892/tencentcloud/car/v20220110/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-car-3.0.891/tencentcloud/car/v20220110/car_client.py` & `tencentcloud-sdk-python-car-3.0.892/tencentcloud/car/v20220110/car_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-car-3.0.891/tencentcloud/car/v20220110/models.py` & `tencentcloud-sdk-python-car-3.0.892/tencentcloud/car/v20220110/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-car-3.0.891/tencentcloud/__init__.py` & `tencentcloud-sdk-python-car-3.0.892/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-car-3.0.891/PKG-INFO` & `tencentcloud-sdk-python-car-3.0.892/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-car
-Version: 3.0.891
+Version: 3.0.892
 Summary: Tencent Cloud Car SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-car-3.0.891/setup.py` & `tencentcloud-sdk-python-car-3.0.892/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-car-3.0.891/tencentcloud_sdk_python_car.egg-info/PKG-INFO` & `tencentcloud-sdk-python-car-3.0.892/tencentcloud_sdk_python_car.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-car
-Version: 3.0.891
+Version: 3.0.892
 Summary: Tencent Cloud Car SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

