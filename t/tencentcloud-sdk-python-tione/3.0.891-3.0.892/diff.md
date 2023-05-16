# Comparing `tmp/tencentcloud-sdk-python-tione-3.0.891.tar.gz` & `tmp/tencentcloud-sdk-python-tione-3.0.892.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tione-3.0.891.tar", last modified: Mon May 15 04:42:35 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tione-3.0.892.tar", last modified: Tue May 16 00:48:26 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tione-3.0.891.tar` & `tencentcloud-sdk-python-tione-3.0.892.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:42:35.000000 tencentcloud-sdk-python-tione-3.0.891/
--rw-r--r--   0 root         (0) root         (0)      743 2023-05-15 04:42:34.000000 tencentcloud-sdk-python-tione-3.0.891/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:42:35.000000 tencentcloud-sdk-python-tione-3.0.891/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-15 04:42:34.000000 tencentcloud-sdk-python-tione-3.0.891/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:42:35.000000 tencentcloud-sdk-python-tione-3.0.891/tencentcloud/tione/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 04:42:34.000000 tencentcloud-sdk-python-tione-3.0.891/tencentcloud/tione/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:42:35.000000 tencentcloud-sdk-python-tione-3.0.891/tencentcloud/tione/v20211111/
--rw-r--r--   0 root         (0) root         (0)    51024 2023-05-15 04:42:34.000000 tencentcloud-sdk-python-tione-3.0.891/tencentcloud/tione/v20211111/tione_client.py
--rw-r--r--   0 root         (0) root         (0)    11488 2023-05-15 04:42:34.000000 tencentcloud-sdk-python-tione-3.0.891/tencentcloud/tione/v20211111/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 04:42:34.000000 tencentcloud-sdk-python-tione-3.0.891/tencentcloud/tione/v20211111/__init__.py
--rw-r--r--   0 root         (0) root         (0)   334001 2023-05-15 04:42:34.000000 tencentcloud-sdk-python-tione-3.0.891/tencentcloud/tione/v20211111/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:42:35.000000 tencentcloud-sdk-python-tione-3.0.891/tencentcloud/tione/v20191022/
--rw-r--r--   0 root         (0) root         (0)    22010 2023-05-15 04:42:34.000000 tencentcloud-sdk-python-tione-3.0.891/tencentcloud/tione/v20191022/tione_client.py
--rw-r--r--   0 root         (0) root         (0)     4465 2023-05-15 04:42:34.000000 tencentcloud-sdk-python-tione-3.0.891/tencentcloud/tione/v20191022/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 04:42:34.000000 tencentcloud-sdk-python-tione-3.0.891/tencentcloud/tione/v20191022/__init__.py
--rw-r--r--   0 root         (0) root         (0)    91250 2023-05-15 04:42:34.000000 tencentcloud-sdk-python-tione-3.0.891/tencentcloud/tione/v20191022/models.py
--rw-r--r--   0 root         (0) root         (0)     1669 2023-05-15 04:42:35.000000 tencentcloud-sdk-python-tione-3.0.891/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1010 2023-05-15 04:42:34.000000 tencentcloud-sdk-python-tione-3.0.891/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-15 04:42:35.000000 tencentcloud-sdk-python-tione-3.0.891/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:42:35.000000 tencentcloud-sdk-python-tione-3.0.891/tencentcloud_sdk_python_tione.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 04:42:35.000000 tencentcloud-sdk-python-tione-3.0.891/tencentcloud_sdk_python_tione.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      633 2023-05-15 04:42:35.000000 tencentcloud-sdk-python-tione-3.0.891/tencentcloud_sdk_python_tione.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1669 2023-05-15 04:42:35.000000 tencentcloud-sdk-python-tione-3.0.891/tencentcloud_sdk_python_tione.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-15 04:42:35.000000 tencentcloud-sdk-python-tione-3.0.891/tencentcloud_sdk_python_tione.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:48:26.000000 tencentcloud-sdk-python-tione-3.0.892/
+-rw-r--r--   0 root         (0) root         (0)      743 2023-05-16 00:48:25.000000 tencentcloud-sdk-python-tione-3.0.892/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:48:26.000000 tencentcloud-sdk-python-tione-3.0.892/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-16 00:48:25.000000 tencentcloud-sdk-python-tione-3.0.892/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:48:26.000000 tencentcloud-sdk-python-tione-3.0.892/tencentcloud/tione/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 00:48:25.000000 tencentcloud-sdk-python-tione-3.0.892/tencentcloud/tione/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:48:26.000000 tencentcloud-sdk-python-tione-3.0.892/tencentcloud/tione/v20211111/
+-rw-r--r--   0 root         (0) root         (0)    51024 2023-05-16 00:48:25.000000 tencentcloud-sdk-python-tione-3.0.892/tencentcloud/tione/v20211111/tione_client.py
+-rw-r--r--   0 root         (0) root         (0)    11488 2023-05-16 00:48:25.000000 tencentcloud-sdk-python-tione-3.0.892/tencentcloud/tione/v20211111/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 00:48:25.000000 tencentcloud-sdk-python-tione-3.0.892/tencentcloud/tione/v20211111/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   334256 2023-05-16 00:48:25.000000 tencentcloud-sdk-python-tione-3.0.892/tencentcloud/tione/v20211111/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:48:26.000000 tencentcloud-sdk-python-tione-3.0.892/tencentcloud/tione/v20191022/
+-rw-r--r--   0 root         (0) root         (0)    22010 2023-05-16 00:48:25.000000 tencentcloud-sdk-python-tione-3.0.892/tencentcloud/tione/v20191022/tione_client.py
+-rw-r--r--   0 root         (0) root         (0)     4465 2023-05-16 00:48:25.000000 tencentcloud-sdk-python-tione-3.0.892/tencentcloud/tione/v20191022/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 00:48:25.000000 tencentcloud-sdk-python-tione-3.0.892/tencentcloud/tione/v20191022/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    91250 2023-05-16 00:48:25.000000 tencentcloud-sdk-python-tione-3.0.892/tencentcloud/tione/v20191022/models.py
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-05-16 00:48:26.000000 tencentcloud-sdk-python-tione-3.0.892/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-05-16 00:48:25.000000 tencentcloud-sdk-python-tione-3.0.892/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-16 00:48:26.000000 tencentcloud-sdk-python-tione-3.0.892/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:48:26.000000 tencentcloud-sdk-python-tione-3.0.892/tencentcloud_sdk_python_tione.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 00:48:26.000000 tencentcloud-sdk-python-tione-3.0.892/tencentcloud_sdk_python_tione.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      633 2023-05-16 00:48:26.000000 tencentcloud-sdk-python-tione-3.0.892/tencentcloud_sdk_python_tione.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-05-16 00:48:26.000000 tencentcloud-sdk-python-tione-3.0.892/tencentcloud_sdk_python_tione.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-16 00:48:26.000000 tencentcloud-sdk-python-tione-3.0.892/tencentcloud_sdk_python_tione.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-tione-3.0.891/README.rst` & `tencentcloud-sdk-python-tione-3.0.892/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.891/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tione-3.0.892/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tione-3.0.891/tencentcloud/tione/v20211111/tione_client.py` & `tencentcloud-sdk-python-tione-3.0.892/tencentcloud/tione/v20211111/tione_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.891/tencentcloud/tione/v20211111/errorcodes.py` & `tencentcloud-sdk-python-tione-3.0.892/tencentcloud/tione/v20211111/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.891/tencentcloud/tione/v20211111/models.py` & `tencentcloud-sdk-python-tione-3.0.892/tencentcloud/tione/v20211111/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -175,15 +175,15 @@
         :type Uin: str
         :param SubUin: 子账号uin
         :type SubUin: str
         :param Region: 地域
         :type Region: str
         :param ChargeType: 计费模式
         :type ChargeType: str
-        :param ResourceGroupId: 包年包月资源组id
+        :param ResourceGroupId: 包年包月资源组ID
 注意：此字段可能返回 null，表示取不到有效值。
         :type ResourceGroupId: str
         :param ResourceGroupName: 包年包月资源组名称
 注意：此字段可能返回 null，表示取不到有效值。
         :type ResourceGroupName: str
         :param ResourceConfigInfo: 资源配置
         :type ResourceConfigInfo: :class:`tencentcloud.tione.v20211111.models.ResourceConfigInfo`
@@ -240,15 +240,15 @@
         :type LatestInstanceId: str
         :param Remark: 备注
 注意：此字段可能返回 null，表示取不到有效值。
         :type Remark: str
         :param FailureReason: 失败原因
 注意：此字段可能返回 null，表示取不到有效值。
         :type FailureReason: str
-        :param BillingInfo: 计费金额信息，eg：2.00元/小时 (for后付费)
+        :param BillingInfo: 计费金额信息，eg：2.00元/小时 (for 按量计费)
 注意：此字段可能返回 null，表示取不到有效值。
         :type BillingInfo: str
         :param PodList: 运行中的Pod的名字
 注意：此字段可能返回 null，表示取不到有效值。
         :type PodList: list of str
         :param ModelInferenceCodeInfo: 模型推理代码信息
 注意：此字段可能返回 null，表示取不到有效值。
@@ -5153,32 +5153,37 @@
         :type EnableDistributed: str
         :param MinBlockSizePt: TORCH_SCRIPT、MMDETECTION、DETECTRON2、HUGGINGFACE格式在进行优化时切分子图的最小算子数目，一般无需进行改动，默认为3
 注意：此字段可能返回 null，表示取不到有效值。
         :type MinBlockSizePt: str
         :param MinBlockSizeTf: FROZEN_GRAPH、SAVED_MODEL格式在进行优化时切分子图的最小算子数目，一般无需进行改动，默认为10
 注意：此字段可能返回 null，表示取不到有效值。
         :type MinBlockSizeTf: str
+        :param PipelineArgs: Stable Diffusion 模型优化参数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type PipelineArgs: str
         """
         self.MaxNNZ = None
         self.SlotNum = None
         self.CpuCachePercentage = None
         self.GpuCachePercentage = None
         self.EnableDistributed = None
         self.MinBlockSizePt = None
         self.MinBlockSizeTf = None
+        self.PipelineArgs = None
 
 
     def _deserialize(self, params):
         self.MaxNNZ = params.get("MaxNNZ")
         self.SlotNum = params.get("SlotNum")
         self.CpuCachePercentage = params.get("CpuCachePercentage")
         self.GpuCachePercentage = params.get("GpuCachePercentage")
         self.EnableDistributed = params.get("EnableDistributed")
         self.MinBlockSizePt = params.get("MinBlockSizePt")
         self.MinBlockSizeTf = params.get("MinBlockSizeTf")
+        self.PipelineArgs = params.get("PipelineArgs")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-tione-3.0.891/tencentcloud/tione/v20191022/tione_client.py` & `tencentcloud-sdk-python-tione-3.0.892/tencentcloud/tione/v20191022/tione_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.891/tencentcloud/tione/v20191022/errorcodes.py` & `tencentcloud-sdk-python-tione-3.0.892/tencentcloud/tione/v20191022/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.891/tencentcloud/tione/v20191022/models.py` & `tencentcloud-sdk-python-tione-3.0.892/tencentcloud/tione/v20191022/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.891/PKG-INFO` & `tencentcloud-sdk-python-tione-3.0.892/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tione
-Version: 3.0.891
+Version: 3.0.892
 Summary: Tencent Cloud Tione SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tione-3.0.891/setup.py` & `tencentcloud-sdk-python-tione-3.0.892/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.891/tencentcloud_sdk_python_tione.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-tione-3.0.892/tencentcloud_sdk_python_tione.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.891/tencentcloud_sdk_python_tione.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tione-3.0.892/tencentcloud_sdk_python_tione.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tione
-Version: 3.0.891
+Version: 3.0.892
 Summary: Tencent Cloud Tione SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

