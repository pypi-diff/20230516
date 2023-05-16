# Comparing `tmp/tencentcloud-sdk-python-mrs-3.0.890.tar.gz` & `tmp/tencentcloud-sdk-python-mrs-3.0.892.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-mrs-3.0.890.tar", last modified: Fri May 12 03:10:25 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-mrs-3.0.892.tar", last modified: Tue May 16 00:41:28 2023, max compression
```

## Comparing `tencentcloud-sdk-python-mrs-3.0.890.tar` & `tencentcloud-sdk-python-mrs-3.0.892.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 03:10:25.000000 tencentcloud-sdk-python-mrs-3.0.890/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 03:10:25.000000 tencentcloud-sdk-python-mrs-3.0.890/tencentcloud_sdk_python_mrs.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-12 03:10:25.000000 tencentcloud-sdk-python-mrs-3.0.890/tencentcloud_sdk_python_mrs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-12 03:10:25.000000 tencentcloud-sdk-python-mrs-3.0.890/tencentcloud_sdk_python_mrs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-12 03:10:25.000000 tencentcloud-sdk-python-mrs-3.0.890/tencentcloud_sdk_python_mrs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-12 03:10:25.000000 tencentcloud-sdk-python-mrs-3.0.890/tencentcloud_sdk_python_mrs.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-12 03:10:25.000000 tencentcloud-sdk-python-mrs-3.0.890/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 03:10:25.000000 tencentcloud-sdk-python-mrs-3.0.890/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-12 03:10:25.000000 tencentcloud-sdk-python-mrs-3.0.890/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 03:10:25.000000 tencentcloud-sdk-python-mrs-3.0.890/tencentcloud/mrs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 03:10:25.000000 tencentcloud-sdk-python-mrs-3.0.890/tencentcloud/mrs/v20200910/
--rw-r--r--   0 root         (0) root         (0)     4657 2023-05-12 03:10:25.000000 tencentcloud-sdk-python-mrs-3.0.890/tencentcloud/mrs/v20200910/mrs_client.py
--rw-r--r--   0 root         (0) root         (0)     3011 2023-05-12 03:10:25.000000 tencentcloud-sdk-python-mrs-3.0.890/tencentcloud/mrs/v20200910/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-12 03:10:25.000000 tencentcloud-sdk-python-mrs-3.0.890/tencentcloud/mrs/v20200910/__init__.py
--rw-r--r--   0 root         (0) root         (0)   360378 2023-05-12 03:10:25.000000 tencentcloud-sdk-python-mrs-3.0.890/tencentcloud/mrs/v20200910/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-12 03:10:25.000000 tencentcloud-sdk-python-mrs-3.0.890/tencentcloud/mrs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-12 03:10:25.000000 tencentcloud-sdk-python-mrs-3.0.890/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-12 03:10:25.000000 tencentcloud-sdk-python-mrs-3.0.890/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-12 03:10:25.000000 tencentcloud-sdk-python-mrs-3.0.890/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:41:28.000000 tencentcloud-sdk-python-mrs-3.0.892/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:41:28.000000 tencentcloud-sdk-python-mrs-3.0.892/tencentcloud_sdk_python_mrs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 00:41:28.000000 tencentcloud-sdk-python-mrs-3.0.892/tencentcloud_sdk_python_mrs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-16 00:41:28.000000 tencentcloud-sdk-python-mrs-3.0.892/tencentcloud_sdk_python_mrs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-16 00:41:28.000000 tencentcloud-sdk-python-mrs-3.0.892/tencentcloud_sdk_python_mrs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-16 00:41:28.000000 tencentcloud-sdk-python-mrs-3.0.892/tencentcloud_sdk_python_mrs.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-16 00:41:28.000000 tencentcloud-sdk-python-mrs-3.0.892/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:41:28.000000 tencentcloud-sdk-python-mrs-3.0.892/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-16 00:41:28.000000 tencentcloud-sdk-python-mrs-3.0.892/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:41:28.000000 tencentcloud-sdk-python-mrs-3.0.892/tencentcloud/mrs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:41:28.000000 tencentcloud-sdk-python-mrs-3.0.892/tencentcloud/mrs/v20200910/
+-rw-r--r--   0 root         (0) root         (0)     4657 2023-05-16 00:41:28.000000 tencentcloud-sdk-python-mrs-3.0.892/tencentcloud/mrs/v20200910/mrs_client.py
+-rw-r--r--   0 root         (0) root         (0)     3011 2023-05-16 00:41:28.000000 tencentcloud-sdk-python-mrs-3.0.892/tencentcloud/mrs/v20200910/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 00:41:28.000000 tencentcloud-sdk-python-mrs-3.0.892/tencentcloud/mrs/v20200910/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   360378 2023-05-16 00:41:28.000000 tencentcloud-sdk-python-mrs-3.0.892/tencentcloud/mrs/v20200910/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 00:41:28.000000 tencentcloud-sdk-python-mrs-3.0.892/tencentcloud/mrs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-16 00:41:28.000000 tencentcloud-sdk-python-mrs-3.0.892/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-16 00:41:28.000000 tencentcloud-sdk-python-mrs-3.0.892/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-16 00:41:28.000000 tencentcloud-sdk-python-mrs-3.0.892/setup.cfg
```

### Comparing `tencentcloud-sdk-python-mrs-3.0.890/tencentcloud_sdk_python_mrs.egg-info/PKG-INFO` & `tencentcloud-sdk-python-mrs-3.0.892/tencentcloud_sdk_python_mrs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-mrs
-Version: 3.0.890
+Version: 3.0.892
 Summary: Tencent Cloud Mrs SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-mrs-3.0.890/README.rst` & `tencentcloud-sdk-python-mrs-3.0.892/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mrs-3.0.890/tencentcloud/__init__.py` & `tencentcloud-sdk-python-mrs-3.0.892/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-mrs-3.0.890/tencentcloud/mrs/v20200910/mrs_client.py` & `tencentcloud-sdk-python-mrs-3.0.892/tencentcloud/mrs/v20200910/mrs_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mrs-3.0.890/tencentcloud/mrs/v20200910/errorcodes.py` & `tencentcloud-sdk-python-mrs-3.0.892/tencentcloud/mrs/v20200910/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mrs-3.0.890/tencentcloud/mrs/v20200910/models.py` & `tencentcloud-sdk-python-mrs-3.0.892/tencentcloud/mrs/v20200910/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -3599,15 +3599,15 @@
 注意：当 IsUsedClassify 为True 时，表示使用收费的报告分类服务，将会产生额外的费用，具体收费标准参见 [购买指南的产品价格](https://cloud.tencent.com/document/product/1314/54264)。
         :type IsUsedClassify: bool
         :param UserType: 后付费的用户类型，新客户传1，老客户可不传或传 0。2022 年 12 月 15 新增了计费项，在此时间之前已经通过商务指定优惠价格的大客户，请不传这个字段或传 0，如果传 1 会导致以前获得的折扣价格失效。在 2022 年 12 月 15 日之后，通过商务指定优惠价格的大客户请传 1。
         :type UserType: int
         :param ReportTypeVersion: 可选。用于指定不同报告使用的结构化引擎版本，不同版本返回的JSON 数据结果不兼容。若不指定版本号，就默认用旧的版本号。
 （1）检验报告 11，默认使用 V2，最高支持 V3。
 （2）病理报告 15，默认使用 V1，最高支持 V2。
-（3）入院记录29、出院记录 28、病理记录 216、病程记录 217、门诊记录 210，默认使用 V1，最高支持 V2。
+（3）入院记录29、出院记录 28、病历记录 216、病程记录 217、门诊记录 210，默认使用 V1，最高支持 V2。
         :type ReportTypeVersion: list of ReportTypeVersion
         """
         self.ImageInfoList = None
         self.HandleParam = None
         self.Type = None
         self.IsUsedClassify = None
         self.UserType = None
@@ -8196,15 +8196,15 @@
 注意：当 IsUsedClassify 为True 时，表示使用收费的报告分类服务，将会产生额外的费用，具体收费标准参见 [购买指南的产品价格](https://cloud.tencent.com/document/product/1314/54264)。
         :type IsUsedClassify: bool
         :param UserType: 后付费的用户类型，新客户传1，老客户可不传或传 0。2022 年 12 月 15 新增了计费项，在此时间之前已经通过商务指定优惠价格的大客户，请不传这个字段或传 0，如果传 1 会导致以前获得的折扣价格失效。在 2022 年 12 月 15 日之后，通过商务指定优惠价格的大客户请传 1。
         :type UserType: int
         :param ReportTypeVersion: 可选。用于指定不同报告使用的结构化引擎版本，不同版本返回的JSON 数据结果不兼容。若不指定版本号，就默认用旧的版本号。
 （1）检验报告 11，默认使用 V2，最高支持 V3。
 （2）病理报告 15，默认使用 V1，最高支持 V2。
-（3）入院记录29、出院记录 28、病理记录 216、病程记录 217、门诊记录 210，默认使用 V1，最高支持 V2。
+（3）入院记录29、出院记录 28、病历记录 216、病程记录 217、门诊记录 210，默认使用 V1，最高支持 V2。
         :type ReportTypeVersion: list of ReportTypeVersion
         """
         self.Text = None
         self.Type = None
         self.IsUsedClassify = None
         self.UserType = None
         self.ReportTypeVersion = None
```

### Comparing `tencentcloud-sdk-python-mrs-3.0.890/PKG-INFO` & `tencentcloud-sdk-python-mrs-3.0.892/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-mrs
-Version: 3.0.890
+Version: 3.0.892
 Summary: Tencent Cloud Mrs SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-mrs-3.0.890/setup.py` & `tencentcloud-sdk-python-mrs-3.0.892/setup.py`

 * *Files identical despite different names*

