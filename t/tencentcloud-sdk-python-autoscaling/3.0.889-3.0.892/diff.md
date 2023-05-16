# Comparing `tmp/tencentcloud-sdk-python-autoscaling-3.0.889.tar.gz` & `tmp/tencentcloud-sdk-python-autoscaling-3.0.892.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-autoscaling-3.0.889.tar", last modified: Thu May 11 02:18:28 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-autoscaling-3.0.892.tar", last modified: Tue May 16 00:28:14 2023, max compression
```

## Comparing `tencentcloud-sdk-python-autoscaling-3.0.889.tar` & `tencentcloud-sdk-python-autoscaling-3.0.892.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 02:18:28.000000 tencentcloud-sdk-python-autoscaling-3.0.889/
--rw-r--r--   0 root         (0) root         (0)      761 2023-05-11 02:18:28.000000 tencentcloud-sdk-python-autoscaling-3.0.889/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 02:18:28.000000 tencentcloud-sdk-python-autoscaling-3.0.889/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 02:18:28.000000 tencentcloud-sdk-python-autoscaling-3.0.889/tencentcloud/autoscaling/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 02:18:28.000000 tencentcloud-sdk-python-autoscaling-3.0.889/tencentcloud/autoscaling/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 02:18:28.000000 tencentcloud-sdk-python-autoscaling-3.0.889/tencentcloud/autoscaling/v20180419/
--rw-r--r--   0 root         (0) root         (0)    60187 2023-05-11 02:18:28.000000 tencentcloud-sdk-python-autoscaling-3.0.889/tencentcloud/autoscaling/v20180419/autoscaling_client.py
--rw-r--r--   0 root         (0) root         (0)    19836 2023-05-11 02:18:28.000000 tencentcloud-sdk-python-autoscaling-3.0.889/tencentcloud/autoscaling/v20180419/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 02:18:28.000000 tencentcloud-sdk-python-autoscaling-3.0.889/tencentcloud/autoscaling/v20180419/__init__.py
--rw-r--r--   0 root         (0) root         (0)   258492 2023-05-11 02:18:28.000000 tencentcloud-sdk-python-autoscaling-3.0.889/tencentcloud/autoscaling/v20180419/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-11 02:18:28.000000 tencentcloud-sdk-python-autoscaling-3.0.889/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1699 2023-05-11 02:18:28.000000 tencentcloud-sdk-python-autoscaling-3.0.889/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 02:18:28.000000 tencentcloud-sdk-python-autoscaling-3.0.889/tencentcloud_sdk_python_autoscaling.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 02:18:28.000000 tencentcloud-sdk-python-autoscaling-3.0.889/tencentcloud_sdk_python_autoscaling.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      525 2023-05-11 02:18:28.000000 tencentcloud-sdk-python-autoscaling-3.0.889/tencentcloud_sdk_python_autoscaling.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1699 2023-05-11 02:18:28.000000 tencentcloud-sdk-python-autoscaling-3.0.889/tencentcloud_sdk_python_autoscaling.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-11 02:18:28.000000 tencentcloud-sdk-python-autoscaling-3.0.889/tencentcloud_sdk_python_autoscaling.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1022 2023-05-11 02:18:28.000000 tencentcloud-sdk-python-autoscaling-3.0.889/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-11 02:18:28.000000 tencentcloud-sdk-python-autoscaling-3.0.889/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:28:14.000000 tencentcloud-sdk-python-autoscaling-3.0.892/
+-rw-r--r--   0 root         (0) root         (0)      761 2023-05-16 00:28:13.000000 tencentcloud-sdk-python-autoscaling-3.0.892/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:28:14.000000 tencentcloud-sdk-python-autoscaling-3.0.892/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:28:14.000000 tencentcloud-sdk-python-autoscaling-3.0.892/tencentcloud/autoscaling/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 00:28:13.000000 tencentcloud-sdk-python-autoscaling-3.0.892/tencentcloud/autoscaling/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:28:14.000000 tencentcloud-sdk-python-autoscaling-3.0.892/tencentcloud/autoscaling/v20180419/
+-rw-r--r--   0 root         (0) root         (0)    60396 2023-05-16 00:28:13.000000 tencentcloud-sdk-python-autoscaling-3.0.892/tencentcloud/autoscaling/v20180419/autoscaling_client.py
+-rw-r--r--   0 root         (0) root         (0)    19836 2023-05-16 00:28:13.000000 tencentcloud-sdk-python-autoscaling-3.0.892/tencentcloud/autoscaling/v20180419/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 00:28:13.000000 tencentcloud-sdk-python-autoscaling-3.0.892/tencentcloud/autoscaling/v20180419/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   258492 2023-05-16 00:28:13.000000 tencentcloud-sdk-python-autoscaling-3.0.892/tencentcloud/autoscaling/v20180419/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-16 00:28:13.000000 tencentcloud-sdk-python-autoscaling-3.0.892/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1699 2023-05-16 00:28:14.000000 tencentcloud-sdk-python-autoscaling-3.0.892/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:28:14.000000 tencentcloud-sdk-python-autoscaling-3.0.892/tencentcloud_sdk_python_autoscaling.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 00:28:13.000000 tencentcloud-sdk-python-autoscaling-3.0.892/tencentcloud_sdk_python_autoscaling.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      525 2023-05-16 00:28:14.000000 tencentcloud-sdk-python-autoscaling-3.0.892/tencentcloud_sdk_python_autoscaling.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1699 2023-05-16 00:28:13.000000 tencentcloud-sdk-python-autoscaling-3.0.892/tencentcloud_sdk_python_autoscaling.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-16 00:28:13.000000 tencentcloud-sdk-python-autoscaling-3.0.892/tencentcloud_sdk_python_autoscaling.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1022 2023-05-16 00:28:13.000000 tencentcloud-sdk-python-autoscaling-3.0.892/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-16 00:28:14.000000 tencentcloud-sdk-python-autoscaling-3.0.892/setup.cfg
```

### Comparing `tencentcloud-sdk-python-autoscaling-3.0.889/README.rst` & `tencentcloud-sdk-python-autoscaling-3.0.892/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-autoscaling-3.0.889/tencentcloud/autoscaling/v20180419/autoscaling_client.py` & `tencentcloud-sdk-python-autoscaling-3.0.892/tencentcloud/autoscaling/v20180419/autoscaling_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -333,15 +333,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DeleteAutoScalingGroup(self, request):
-        """本接口（DeleteAutoScalingGroup）用于删除指定伸缩组，删除前提是伸缩组内无实例且当前未在执行伸缩活动。
+        """本接口（DeleteAutoScalingGroup）用于删除指定伸缩组，删除前提是伸缩组内无运行中（IN_SERVICE）状态的实例且当前未在执行伸缩活动。删除伸缩组后，创建失败（CREATION_FAILED）、中止失败（TERMINATION_FAILED）、解绑失败（DETACH_FAILED）等非运行中状态的实例不会被销毁。
 
         :param request: Request instance for DeleteAutoScalingGroup.
         :type request: :class:`tencentcloud.autoscaling.v20180419.models.DeleteAutoScalingGroupRequest`
         :rtype: :class:`tencentcloud.autoscaling.v20180419.models.DeleteAutoScalingGroupResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-autoscaling-3.0.889/tencentcloud/autoscaling/v20180419/errorcodes.py` & `tencentcloud-sdk-python-autoscaling-3.0.892/tencentcloud/autoscaling/v20180419/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-autoscaling-3.0.889/tencentcloud/autoscaling/v20180419/models.py` & `tencentcloud-sdk-python-autoscaling-3.0.892/tencentcloud/autoscaling/v20180419/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-autoscaling-3.0.889/tencentcloud/__init__.py` & `tencentcloud-sdk-python-autoscaling-3.0.892/tencentcloud/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.889'
+__version__ = '3.0.892'
```

### Comparing `tencentcloud-sdk-python-autoscaling-3.0.889/PKG-INFO` & `tencentcloud-sdk-python-autoscaling-3.0.892/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-autoscaling
-Version: 3.0.889
+Version: 3.0.892
 Summary: Tencent Cloud Autoscaling SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-autoscaling-3.0.889/tencentcloud_sdk_python_autoscaling.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-autoscaling-3.0.892/tencentcloud_sdk_python_autoscaling.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-autoscaling-3.0.889/tencentcloud_sdk_python_autoscaling.egg-info/PKG-INFO` & `tencentcloud-sdk-python-autoscaling-3.0.892/tencentcloud_sdk_python_autoscaling.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-autoscaling
-Version: 3.0.889
+Version: 3.0.892
 Summary: Tencent Cloud Autoscaling SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-autoscaling-3.0.889/setup.py` & `tencentcloud-sdk-python-autoscaling-3.0.892/setup.py`

 * *Files identical despite different names*

