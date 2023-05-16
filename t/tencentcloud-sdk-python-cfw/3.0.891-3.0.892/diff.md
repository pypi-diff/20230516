# Comparing `tmp/tencentcloud-sdk-python-cfw-3.0.891.tar.gz` & `tmp/tencentcloud-sdk-python-cfw-3.0.892.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cfw-3.0.891.tar", last modified: Mon May 15 02:37:39 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cfw-3.0.892.tar", last modified: Tue May 16 00:31:28 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cfw-3.0.891.tar` & `tencentcloud-sdk-python-cfw-3.0.892.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 02:37:39.000000 tencentcloud-sdk-python-cfw-3.0.891/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-15 02:37:39.000000 tencentcloud-sdk-python-cfw-3.0.891/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 02:37:39.000000 tencentcloud-sdk-python-cfw-3.0.891/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 02:37:39.000000 tencentcloud-sdk-python-cfw-3.0.891/tencentcloud/cfw/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 02:37:39.000000 tencentcloud-sdk-python-cfw-3.0.891/tencentcloud/cfw/v20190904/
--rw-r--r--   0 root         (0) root         (0)     1836 2023-05-15 02:37:39.000000 tencentcloud-sdk-python-cfw-3.0.891/tencentcloud/cfw/v20190904/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    65621 2023-05-15 02:37:39.000000 tencentcloud-sdk-python-cfw-3.0.891/tencentcloud/cfw/v20190904/cfw_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 02:37:39.000000 tencentcloud-sdk-python-cfw-3.0.891/tencentcloud/cfw/v20190904/__init__.py
--rw-r--r--   0 root         (0) root         (0)   215744 2023-05-15 02:37:39.000000 tencentcloud-sdk-python-cfw-3.0.891/tencentcloud/cfw/v20190904/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 02:37:39.000000 tencentcloud-sdk-python-cfw-3.0.891/tencentcloud/cfw/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-15 02:37:39.000000 tencentcloud-sdk-python-cfw-3.0.891/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 02:37:39.000000 tencentcloud-sdk-python-cfw-3.0.891/tencentcloud_sdk_python_cfw.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 02:37:39.000000 tencentcloud-sdk-python-cfw-3.0.891/tencentcloud_sdk_python_cfw.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-15 02:37:39.000000 tencentcloud-sdk-python-cfw-3.0.891/tencentcloud_sdk_python_cfw.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-15 02:37:39.000000 tencentcloud-sdk-python-cfw-3.0.891/tencentcloud_sdk_python_cfw.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-15 02:37:39.000000 tencentcloud-sdk-python-cfw-3.0.891/tencentcloud_sdk_python_cfw.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-15 02:37:39.000000 tencentcloud-sdk-python-cfw-3.0.891/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-15 02:37:39.000000 tencentcloud-sdk-python-cfw-3.0.891/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-15 02:37:39.000000 tencentcloud-sdk-python-cfw-3.0.891/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:31:28.000000 tencentcloud-sdk-python-cfw-3.0.892/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-16 00:31:28.000000 tencentcloud-sdk-python-cfw-3.0.892/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:31:28.000000 tencentcloud-sdk-python-cfw-3.0.892/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:31:28.000000 tencentcloud-sdk-python-cfw-3.0.892/tencentcloud/cfw/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:31:28.000000 tencentcloud-sdk-python-cfw-3.0.892/tencentcloud/cfw/v20190904/
+-rw-r--r--   0 root         (0) root         (0)     1836 2023-05-16 00:31:28.000000 tencentcloud-sdk-python-cfw-3.0.892/tencentcloud/cfw/v20190904/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    65621 2023-05-16 00:31:28.000000 tencentcloud-sdk-python-cfw-3.0.892/tencentcloud/cfw/v20190904/cfw_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 00:31:28.000000 tencentcloud-sdk-python-cfw-3.0.892/tencentcloud/cfw/v20190904/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   216862 2023-05-16 00:31:28.000000 tencentcloud-sdk-python-cfw-3.0.892/tencentcloud/cfw/v20190904/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 00:31:28.000000 tencentcloud-sdk-python-cfw-3.0.892/tencentcloud/cfw/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-16 00:31:28.000000 tencentcloud-sdk-python-cfw-3.0.892/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:31:28.000000 tencentcloud-sdk-python-cfw-3.0.892/tencentcloud_sdk_python_cfw.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 00:31:28.000000 tencentcloud-sdk-python-cfw-3.0.892/tencentcloud_sdk_python_cfw.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-16 00:31:28.000000 tencentcloud-sdk-python-cfw-3.0.892/tencentcloud_sdk_python_cfw.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-16 00:31:28.000000 tencentcloud-sdk-python-cfw-3.0.892/tencentcloud_sdk_python_cfw.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-16 00:31:28.000000 tencentcloud-sdk-python-cfw-3.0.892/tencentcloud_sdk_python_cfw.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-16 00:31:28.000000 tencentcloud-sdk-python-cfw-3.0.892/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-16 00:31:28.000000 tencentcloud-sdk-python-cfw-3.0.892/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-16 00:31:28.000000 tencentcloud-sdk-python-cfw-3.0.892/setup.cfg
```

### Comparing `tencentcloud-sdk-python-cfw-3.0.891/README.rst` & `tencentcloud-sdk-python-cfw-3.0.892/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cfw-3.0.891/tencentcloud/cfw/v20190904/errorcodes.py` & `tencentcloud-sdk-python-cfw-3.0.892/tencentcloud/cfw/v20190904/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cfw-3.0.891/tencentcloud/cfw/v20190904/cfw_client.py` & `tencentcloud-sdk-python-cfw-3.0.892/tencentcloud/cfw/v20190904/cfw_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cfw-3.0.891/tencentcloud/cfw/v20190904/models.py` & `tencentcloud-sdk-python-cfw-3.0.892/tencentcloud/cfw/v20190904/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -5811,14 +5811,29 @@
         :param BothWayInfo: 生成双向下发规则
 注意：此字段可能返回 null，表示取不到有效值。
         :type BothWayInfo: list of SecurityGroupBothWayInfo
         :param Direction: 方向，0：出站，1：入站，默认1
         :type Direction: int
         :param ProtocolPortType: 是否使用端口协议模板，0：否，1：是
         :type ProtocolPortType: int
+        :param Uuid: Uuid
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Uuid: str
+        :param Region: 地域
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Region: str
+        :param AssetGroupNameIn: 资产分组名称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AssetGroupNameIn: str
+        :param AssetGroupNameOut: 资产分组名称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AssetGroupNameOut: str
+        :param ParameterName: 模板名称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ParameterName: str
         """
         self.OrderIndex = None
         self.SourceId = None
         self.SourceType = None
         self.TargetId = None
         self.TargetType = None
         self.Protocol = None
@@ -5835,14 +5850,19 @@
         self.PublicIp = None
         self.PrivateIp = None
         self.Cidr = None
         self.ServiceTemplateId = None
         self.BothWayInfo = None
         self.Direction = None
         self.ProtocolPortType = None
+        self.Uuid = None
+        self.Region = None
+        self.AssetGroupNameIn = None
+        self.AssetGroupNameOut = None
+        self.ParameterName = None
 
 
     def _deserialize(self, params):
         self.OrderIndex = params.get("OrderIndex")
         self.SourceId = params.get("SourceId")
         self.SourceType = params.get("SourceType")
         self.TargetId = params.get("TargetId")
@@ -5866,14 +5886,19 @@
             self.BothWayInfo = []
             for item in params.get("BothWayInfo"):
                 obj = SecurityGroupBothWayInfo()
                 obj._deserialize(item)
                 self.BothWayInfo.append(obj)
         self.Direction = params.get("Direction")
         self.ProtocolPortType = params.get("ProtocolPortType")
+        self.Uuid = params.get("Uuid")
+        self.Region = params.get("Region")
+        self.AssetGroupNameIn = params.get("AssetGroupNameIn")
+        self.AssetGroupNameOut = params.get("AssetGroupNameOut")
+        self.ParameterName = params.get("ParameterName")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-cfw-3.0.891/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cfw-3.0.892/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cfw-3.0.891/tencentcloud_sdk_python_cfw.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cfw-3.0.892/tencentcloud_sdk_python_cfw.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cfw
-Version: 3.0.891
+Version: 3.0.892
 Summary: Tencent Cloud Cfw SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cfw-3.0.891/PKG-INFO` & `tencentcloud-sdk-python-cfw-3.0.892/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cfw
-Version: 3.0.891
+Version: 3.0.892
 Summary: Tencent Cloud Cfw SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cfw-3.0.891/setup.py` & `tencentcloud-sdk-python-cfw-3.0.892/setup.py`

 * *Files identical despite different names*

