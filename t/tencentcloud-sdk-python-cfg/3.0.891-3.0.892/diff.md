# Comparing `tmp/tencentcloud-sdk-python-cfg-3.0.891.tar.gz` & `tmp/tencentcloud-sdk-python-cfg-3.0.892.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cfg-3.0.891.tar", last modified: Mon May 15 02:37:25 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cfg-3.0.892.tar", last modified: Tue May 16 00:31:16 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cfg-3.0.891.tar` & `tencentcloud-sdk-python-cfg-3.0.892.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 02:37:25.000000 tencentcloud-sdk-python-cfg-3.0.891/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-15 02:37:25.000000 tencentcloud-sdk-python-cfg-3.0.891/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 02:37:25.000000 tencentcloud-sdk-python-cfg-3.0.891/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-15 02:37:25.000000 tencentcloud-sdk-python-cfg-3.0.891/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 02:37:25.000000 tencentcloud-sdk-python-cfg-3.0.891/tencentcloud/cfg/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 02:37:25.000000 tencentcloud-sdk-python-cfg-3.0.891/tencentcloud/cfg/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 02:37:25.000000 tencentcloud-sdk-python-cfg-3.0.891/tencentcloud/cfg/v20210820/
--rw-r--r--   0 root         (0) root         (0)     1933 2023-05-15 02:37:25.000000 tencentcloud-sdk-python-cfg-3.0.891/tencentcloud/cfg/v20210820/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     9695 2023-05-15 02:37:25.000000 tencentcloud-sdk-python-cfg-3.0.891/tencentcloud/cfg/v20210820/cfg_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 02:37:25.000000 tencentcloud-sdk-python-cfg-3.0.891/tencentcloud/cfg/v20210820/__init__.py
--rw-r--r--   0 root         (0) root         (0)    62984 2023-05-15 02:37:25.000000 tencentcloud-sdk-python-cfg-3.0.891/tencentcloud/cfg/v20210820/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 02:37:25.000000 tencentcloud-sdk-python-cfg-3.0.891/tencentcloud_sdk_python_cfg.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 02:37:25.000000 tencentcloud-sdk-python-cfg-3.0.891/tencentcloud_sdk_python_cfg.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-15 02:37:25.000000 tencentcloud-sdk-python-cfg-3.0.891/tencentcloud_sdk_python_cfg.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-15 02:37:25.000000 tencentcloud-sdk-python-cfg-3.0.891/tencentcloud_sdk_python_cfg.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-15 02:37:25.000000 tencentcloud-sdk-python-cfg-3.0.891/tencentcloud_sdk_python_cfg.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-15 02:37:25.000000 tencentcloud-sdk-python-cfg-3.0.891/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-15 02:37:25.000000 tencentcloud-sdk-python-cfg-3.0.891/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-15 02:37:25.000000 tencentcloud-sdk-python-cfg-3.0.891/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:31:16.000000 tencentcloud-sdk-python-cfg-3.0.892/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-16 00:31:16.000000 tencentcloud-sdk-python-cfg-3.0.892/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:31:16.000000 tencentcloud-sdk-python-cfg-3.0.892/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-16 00:31:16.000000 tencentcloud-sdk-python-cfg-3.0.892/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:31:16.000000 tencentcloud-sdk-python-cfg-3.0.892/tencentcloud/cfg/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 00:31:16.000000 tencentcloud-sdk-python-cfg-3.0.892/tencentcloud/cfg/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:31:16.000000 tencentcloud-sdk-python-cfg-3.0.892/tencentcloud/cfg/v20210820/
+-rw-r--r--   0 root         (0) root         (0)     1933 2023-05-16 00:31:16.000000 tencentcloud-sdk-python-cfg-3.0.892/tencentcloud/cfg/v20210820/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     9695 2023-05-16 00:31:16.000000 tencentcloud-sdk-python-cfg-3.0.892/tencentcloud/cfg/v20210820/cfg_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 00:31:16.000000 tencentcloud-sdk-python-cfg-3.0.892/tencentcloud/cfg/v20210820/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    63461 2023-05-16 00:31:16.000000 tencentcloud-sdk-python-cfg-3.0.892/tencentcloud/cfg/v20210820/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:31:16.000000 tencentcloud-sdk-python-cfg-3.0.892/tencentcloud_sdk_python_cfg.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 00:31:16.000000 tencentcloud-sdk-python-cfg-3.0.892/tencentcloud_sdk_python_cfg.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-16 00:31:16.000000 tencentcloud-sdk-python-cfg-3.0.892/tencentcloud_sdk_python_cfg.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-16 00:31:16.000000 tencentcloud-sdk-python-cfg-3.0.892/tencentcloud_sdk_python_cfg.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-16 00:31:16.000000 tencentcloud-sdk-python-cfg-3.0.892/tencentcloud_sdk_python_cfg.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-16 00:31:16.000000 tencentcloud-sdk-python-cfg-3.0.892/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-16 00:31:16.000000 tencentcloud-sdk-python-cfg-3.0.892/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-16 00:31:16.000000 tencentcloud-sdk-python-cfg-3.0.892/setup.cfg
```

### Comparing `tencentcloud-sdk-python-cfg-3.0.891/README.rst` & `tencentcloud-sdk-python-cfg-3.0.892/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cfg-3.0.891/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cfg-3.0.892/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cfg-3.0.891/tencentcloud/cfg/v20210820/errorcodes.py` & `tencentcloud-sdk-python-cfg-3.0.892/tencentcloud/cfg/v20210820/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cfg-3.0.891/tencentcloud/cfg/v20210820/cfg_client.py` & `tencentcloud-sdk-python-cfg-3.0.892/tencentcloud/cfg/v20210820/cfg_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cfg-3.0.891/tencentcloud/cfg/v20210820/models.py` & `tencentcloud-sdk-python-cfg-3.0.892/tencentcloud/cfg/v20210820/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -733,14 +733,20 @@
         :type TaskMonitors: list of TaskMonitor
         :param TaskPolicy: 保护策略
 注意：此字段可能返回 null，表示取不到有效值。
         :type TaskPolicy: :class:`tencentcloud.cfg.v20210820.models.DescribePolicy`
         :param Tags: 标签列表
 注意：此字段可能返回 null，表示取不到有效值。
         :type Tags: list of TagWithDescribe
+        :param TaskPlanId: 关联的演练计划ID
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TaskPlanId: int
+        :param TaskPlanTitle: 关联的演练计划名称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TaskPlanTitle: str
         """
         self.TaskId = None
         self.TaskTitle = None
         self.TaskDescription = None
         self.TaskTag = None
         self.TaskStatus = None
         self.TaskStatusType = None
@@ -755,14 +761,16 @@
         self.TaskMode = None
         self.TaskPauseDuration = None
         self.TaskOwnerUin = None
         self.TaskRegionId = None
         self.TaskMonitors = None
         self.TaskPolicy = None
         self.Tags = None
+        self.TaskPlanId = None
+        self.TaskPlanTitle = None
 
 
     def _deserialize(self, params):
         self.TaskId = params.get("TaskId")
         self.TaskTitle = params.get("TaskTitle")
         self.TaskDescription = params.get("TaskDescription")
         self.TaskTag = params.get("TaskTag")
@@ -796,14 +804,16 @@
             self.TaskPolicy._deserialize(params.get("TaskPolicy"))
         if params.get("Tags") is not None:
             self.Tags = []
             for item in params.get("Tags"):
                 obj = TagWithDescribe()
                 obj._deserialize(item)
                 self.Tags.append(obj)
+        self.TaskPlanId = params.get("TaskPlanId")
+        self.TaskPlanTitle = params.get("TaskPlanTitle")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-cfg-3.0.891/tencentcloud_sdk_python_cfg.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cfg-3.0.892/tencentcloud_sdk_python_cfg.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cfg
-Version: 3.0.891
+Version: 3.0.892
 Summary: Tencent Cloud Cfg SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cfg-3.0.891/PKG-INFO` & `tencentcloud-sdk-python-cfg-3.0.892/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cfg
-Version: 3.0.891
+Version: 3.0.892
 Summary: Tencent Cloud Cfg SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cfg-3.0.891/setup.py` & `tencentcloud-sdk-python-cfg-3.0.892/setup.py`

 * *Files identical despite different names*

