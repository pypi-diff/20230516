# Comparing `tmp/navabilitysdk-0.5.0.tar.gz` & `tmp/navabilitysdk-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "navabilitysdk-0.5.0.tar", last modified: Tue Feb 21 06:19:00 2023, max compression
+gzip compressed data, was "navabilitysdk-0.5.1.tar", last modified: Fri Feb 24 01:17:49 2023, max compression
```

## Comparing `navabilitysdk-0.5.0.tar` & `navabilitysdk-0.5.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxr-x   0 samc      (1000) samc      (1000)        0 2023-02-21 06:19:00.615092 navabilitysdk-0.5.0/
--rw-rw-r--   0 samc      (1000) samc      (1000)    11357 2022-04-26 17:04:58.000000 navabilitysdk-0.5.0/LICENSE
--rw-rw-r--   0 samc      (1000) samc      (1000)      515 2023-02-21 06:19:00.615092 navabilitysdk-0.5.0/PKG-INFO
--rw-rw-r--   0 samc      (1000) samc      (1000)     1130 2023-02-21 06:18:28.000000 navabilitysdk-0.5.0/README.md
--rw-rw-r--   0 samc      (1000) samc      (1000)       79 2023-02-21 06:19:00.615092 navabilitysdk-0.5.0/setup.cfg
--rw-rw-r--   0 samc      (1000) samc      (1000)     1346 2023-02-21 06:18:28.000000 navabilitysdk-0.5.0/setup.py
-drwxrwxr-x   0 samc      (1000) samc      (1000)        0 2023-02-21 06:19:00.611092 navabilitysdk-0.5.0/src/
-drwxrwxr-x   0 samc      (1000) samc      (1000)        0 2023-02-21 06:19:00.611092 navabilitysdk-0.5.0/src/navability/
--rw-rw-r--   0 samc      (1000) samc      (1000)        0 2022-04-26 17:04:58.000000 navabilitysdk-0.5.0/src/navability/__init__.py
-drwxrwxr-x   0 samc      (1000) samc      (1000)        0 2023-02-21 06:19:00.611092 navabilitysdk-0.5.0/src/navability/common/
--rw-rw-r--   0 samc      (1000) samc      (1000)        0 2022-04-26 17:04:58.000000 navabilitysdk-0.5.0/src/navability/common/__init__.py
--rw-rw-r--   0 samc      (1000) samc      (1000)     3947 2023-02-21 06:18:28.000000 navabilitysdk-0.5.0/src/navability/common/mutations.py
--rw-rw-r--   0 samc      (1000) samc      (1000)     9683 2023-02-21 06:18:28.000000 navabilitysdk-0.5.0/src/navability/common/queries.py
--rw-rw-r--   0 samc      (1000) samc      (1000)      189 2022-04-26 17:04:58.000000 navabilitysdk-0.5.0/src/navability/common/timestamps.py
--rw-rw-r--   0 samc      (1000) samc      (1000)       27 2022-04-26 17:04:58.000000 navabilitysdk-0.5.0/src/navability/common/versions.py
-drwxrwxr-x   0 samc      (1000) samc      (1000)        0 2023-02-21 06:19:00.615092 navabilitysdk-0.5.0/src/navability/entities/
--rw-rw-r--   0 samc      (1000) samc      (1000)      978 2023-02-21 06:18:28.000000 navabilitysdk-0.5.0/src/navability/entities/__init__.py
-drwxrwxr-x   0 samc      (1000) samc      (1000)        0 2023-02-21 06:19:00.615092 navabilitysdk-0.5.0/src/navability/entities/blob/
--rw-rw-r--   0 samc      (1000) samc      (1000)        0 2023-02-21 06:18:28.000000 navabilitysdk-0.5.0/src/navability/entities/blob/__init__.py
--rw-rw-r--   0 samc      (1000) samc      (1000)     2022 2023-02-21 06:18:28.000000 navabilitysdk-0.5.0/src/navability/entities/blob/blob.py
--rw-rw-r--   0 samc      (1000) samc      (1000)      803 2022-04-26 17:04:58.000000 navabilitysdk-0.5.0/src/navability/entities/client.py
-drwxrwxr-x   0 samc      (1000) samc      (1000)        0 2023-02-21 06:19:00.615092 navabilitysdk-0.5.0/src/navability/entities/factor/
--rw-rw-r--   0 samc      (1000) samc      (1000)        0 2022-04-26 17:04:58.000000 navabilitysdk-0.5.0/src/navability/entities/factor/__init__.py
--rw-rw-r--   0 samc      (1000) samc      (1000)     3600 2022-04-26 17:04:58.000000 navabilitysdk-0.5.0/src/navability/entities/factor/distributions.py
--rw-rw-r--   0 samc      (1000) samc      (1000)     6457 2023-02-21 06:18:28.000000 navabilitysdk-0.5.0/src/navability/entities/factor/factor.py
--rw-rw-r--   0 samc      (1000) samc      (1000)     8387 2022-04-26 17:04:58.000000 navabilitysdk-0.5.0/src/navability/entities/factor/inferencetypes.py
--rw-rw-r--   0 samc      (1000) samc      (1000)     2792 2023-02-21 06:18:28.000000 navabilitysdk-0.5.0/src/navability/entities/navabilityclient.py
--rw-rw-r--   0 samc      (1000) samc      (1000)      109 2022-04-26 17:04:58.000000 navabilitysdk-0.5.0/src/navability/entities/querydetail.py
--rw-rw-r--   0 samc      (1000) samc      (1000)      967 2022-04-26 17:04:58.000000 navabilitysdk-0.5.0/src/navability/entities/scope.py
--rw-rw-r--   0 samc      (1000) samc      (1000)      764 2022-07-06 15:11:39.000000 navabilitysdk-0.5.0/src/navability/entities/solve.py
--rw-rw-r--   0 samc      (1000) samc      (1000)     1643 2022-04-26 17:04:58.000000 navabilitysdk-0.5.0/src/navability/entities/statusmessage.py
-drwxrwxr-x   0 samc      (1000) samc      (1000)        0 2023-02-21 06:19:00.615092 navabilitysdk-0.5.0/src/navability/entities/variable/
--rw-rw-r--   0 samc      (1000) samc      (1000)        0 2022-04-26 17:04:58.000000 navabilitysdk-0.5.0/src/navability/entities/variable/__init__.py
--rw-rw-r--   0 samc      (1000) samc      (1000)     2046 2022-04-26 17:04:58.000000 navabilitysdk-0.5.0/src/navability/entities/variable/ppe.py
--rw-rw-r--   0 samc      (1000) samc      (1000)     7975 2023-02-21 06:18:28.000000 navabilitysdk-0.5.0/src/navability/entities/variable/variable.py
--rw-rw-r--   0 samc      (1000) samc      (1000)     3144 2022-07-12 18:54:00.000000 navabilitysdk-0.5.0/src/navability/entities/variable/variablenodedata.py
-drwxrwxr-x   0 samc      (1000) samc      (1000)        0 2023-02-21 06:19:00.615092 navabilitysdk-0.5.0/src/navability/services/
--rw-rw-r--   0 samc      (1000) samc      (1000)      152 2023-02-21 06:18:28.000000 navabilitysdk-0.5.0/src/navability/services/__init__.py
--rw-rw-r--   0 samc      (1000) samc      (1000)     8754 2023-02-21 06:18:28.000000 navabilitysdk-0.5.0/src/navability/services/blob.py
--rw-rw-r--   0 samc      (1000) samc      (1000)     5557 2022-07-12 18:23:55.000000 navabilitysdk-0.5.0/src/navability/services/factor.py
--rw-rw-r--   0 samc      (1000) samc      (1000)      717 2022-07-06 15:11:39.000000 navabilitysdk-0.5.0/src/navability/services/solve.py
--rw-rw-r--   0 samc      (1000) samc      (1000)     1664 2022-04-26 17:04:58.000000 navabilitysdk-0.5.0/src/navability/services/status.py
--rw-rw-r--   0 samc      (1000) samc      (1000)     2818 2022-07-12 18:23:55.000000 navabilitysdk-0.5.0/src/navability/services/utils.py
--rw-rw-r--   0 samc      (1000) samc      (1000)     8104 2023-02-21 06:18:28.000000 navabilitysdk-0.5.0/src/navability/services/variable.py
-drwxrwxr-x   0 samc      (1000) samc      (1000)        0 2023-02-21 06:19:00.615092 navabilitysdk-0.5.0/src/navabilitysdk.egg-info/
--rw-rw-r--   0 samc      (1000) samc      (1000)      515 2023-02-21 06:19:00.000000 navabilitysdk-0.5.0/src/navabilitysdk.egg-info/PKG-INFO
--rw-rw-r--   0 samc      (1000) samc      (1000)     1379 2023-02-21 06:19:00.000000 navabilitysdk-0.5.0/src/navabilitysdk.egg-info/SOURCES.txt
--rw-rw-r--   0 samc      (1000) samc      (1000)        1 2023-02-21 06:19:00.000000 navabilitysdk-0.5.0/src/navabilitysdk.egg-info/dependency_links.txt
--rw-rw-r--   0 samc      (1000) samc      (1000)      143 2023-02-21 06:19:00.000000 navabilitysdk-0.5.0/src/navabilitysdk.egg-info/requires.txt
--rw-rw-r--   0 samc      (1000) samc      (1000)       11 2023-02-21 06:19:00.000000 navabilitysdk-0.5.0/src/navabilitysdk.egg-info/top_level.txt
+drwxrwxr-x   0 dehann    (1000) dehann    (1000)        0 2023-02-24 01:17:49.772213 navabilitysdk-0.5.1/
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)    11357 2022-04-01 00:01:58.000000 navabilitysdk-0.5.1/LICENSE
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)      512 2023-02-24 01:17:49.772213 navabilitysdk-0.5.1/PKG-INFO
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)     1130 2023-02-14 05:08:08.000000 navabilitysdk-0.5.1/README.md
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)       79 2023-02-24 01:17:49.772213 navabilitysdk-0.5.1/setup.cfg
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)     1346 2023-02-23 07:42:57.000000 navabilitysdk-0.5.1/setup.py
+drwxrwxr-x   0 dehann    (1000) dehann    (1000)        0 2023-02-24 01:17:49.768212 navabilitysdk-0.5.1/src/
+drwxrwxr-x   0 dehann    (1000) dehann    (1000)        0 2023-02-24 01:17:49.768212 navabilitysdk-0.5.1/src/navability/
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)        0 2022-04-01 00:01:58.000000 navabilitysdk-0.5.1/src/navability/__init__.py
+drwxrwxr-x   0 dehann    (1000) dehann    (1000)        0 2023-02-24 01:17:49.768212 navabilitysdk-0.5.1/src/navability/common/
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)        0 2022-04-01 00:01:58.000000 navabilitysdk-0.5.1/src/navability/common/__init__.py
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)     3947 2023-02-21 02:44:09.000000 navabilitysdk-0.5.1/src/navability/common/mutations.py
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)     9683 2023-02-20 22:14:11.000000 navabilitysdk-0.5.1/src/navability/common/queries.py
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)      189 2022-04-01 00:01:58.000000 navabilitysdk-0.5.1/src/navability/common/timestamps.py
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)       27 2022-04-01 00:01:58.000000 navabilitysdk-0.5.1/src/navability/common/versions.py
+drwxrwxr-x   0 dehann    (1000) dehann    (1000)        0 2023-02-24 01:17:49.768212 navabilitysdk-0.5.1/src/navability/entities/
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)     1010 2023-02-24 00:34:43.000000 navabilitysdk-0.5.1/src/navability/entities/__init__.py
+drwxrwxr-x   0 dehann    (1000) dehann    (1000)        0 2023-02-24 01:17:49.768212 navabilitysdk-0.5.1/src/navability/entities/blob/
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)        0 2023-02-20 15:50:38.000000 navabilitysdk-0.5.1/src/navability/entities/blob/__init__.py
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)     2022 2023-02-20 22:14:11.000000 navabilitysdk-0.5.1/src/navability/entities/blob/blob.py
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)      803 2022-04-01 00:01:58.000000 navabilitysdk-0.5.1/src/navability/entities/client.py
+drwxrwxr-x   0 dehann    (1000) dehann    (1000)        0 2023-02-24 01:17:49.768212 navabilitysdk-0.5.1/src/navability/entities/factor/
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)        0 2022-04-01 00:01:58.000000 navabilitysdk-0.5.1/src/navability/entities/factor/__init__.py
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)     3600 2022-04-01 00:01:58.000000 navabilitysdk-0.5.1/src/navability/entities/factor/distributions.py
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)     6457 2023-02-21 05:26:14.000000 navabilitysdk-0.5.1/src/navability/entities/factor/factor.py
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)     8994 2023-02-23 07:42:57.000000 navabilitysdk-0.5.1/src/navability/entities/factor/inferencetypes.py
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)     2792 2023-02-20 13:35:18.000000 navabilitysdk-0.5.1/src/navability/entities/navabilityclient.py
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)      109 2022-04-01 00:01:58.000000 navabilitysdk-0.5.1/src/navability/entities/querydetail.py
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)      967 2022-04-01 00:01:58.000000 navabilitysdk-0.5.1/src/navability/entities/scope.py
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)      764 2022-07-07 20:02:22.000000 navabilitysdk-0.5.1/src/navability/entities/solve.py
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)     1643 2022-04-01 00:01:58.000000 navabilitysdk-0.5.1/src/navability/entities/statusmessage.py
+drwxrwxr-x   0 dehann    (1000) dehann    (1000)        0 2023-02-24 01:17:49.768212 navabilitysdk-0.5.1/src/navability/entities/variable/
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)        0 2022-04-01 00:01:58.000000 navabilitysdk-0.5.1/src/navability/entities/variable/__init__.py
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)     2046 2022-04-01 00:01:58.000000 navabilitysdk-0.5.1/src/navability/entities/variable/ppe.py
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)     7975 2023-02-13 22:28:36.000000 navabilitysdk-0.5.1/src/navability/entities/variable/variable.py
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)     3144 2022-07-14 05:39:17.000000 navabilitysdk-0.5.1/src/navability/entities/variable/variablenodedata.py
+drwxrwxr-x   0 dehann    (1000) dehann    (1000)        0 2023-02-24 01:17:49.772213 navabilitysdk-0.5.1/src/navability/services/
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)      152 2023-02-20 15:50:38.000000 navabilitysdk-0.5.1/src/navability/services/__init__.py
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)     8754 2023-02-21 02:44:09.000000 navabilitysdk-0.5.1/src/navability/services/blob.py
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)     5557 2022-07-07 20:02:22.000000 navabilitysdk-0.5.1/src/navability/services/factor.py
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)      717 2022-07-07 20:02:22.000000 navabilitysdk-0.5.1/src/navability/services/solve.py
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)     1664 2022-04-01 00:01:58.000000 navabilitysdk-0.5.1/src/navability/services/status.py
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)     2910 2023-02-22 23:01:10.000000 navabilitysdk-0.5.1/src/navability/services/utils.py
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)     8104 2023-02-20 15:50:38.000000 navabilitysdk-0.5.1/src/navability/services/variable.py
+drwxrwxr-x   0 dehann    (1000) dehann    (1000)        0 2023-02-24 01:17:49.772213 navabilitysdk-0.5.1/src/navabilitysdk.egg-info/
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)      512 2023-02-24 01:17:49.000000 navabilitysdk-0.5.1/src/navabilitysdk.egg-info/PKG-INFO
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)     1379 2023-02-24 01:17:49.000000 navabilitysdk-0.5.1/src/navabilitysdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)        1 2023-02-24 01:17:49.000000 navabilitysdk-0.5.1/src/navabilitysdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)      143 2023-02-24 01:17:49.000000 navabilitysdk-0.5.1/src/navabilitysdk.egg-info/requires.txt
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)       11 2023-02-24 01:17:49.000000 navabilitysdk-0.5.1/src/navabilitysdk.egg-info/top_level.txt
```

### Comparing `navabilitysdk-0.5.0/LICENSE` & `navabilitysdk-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `navabilitysdk-0.5.0/README.md` & `navabilitysdk-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `navabilitysdk-0.5.0/setup.py` & `navabilitysdk-0.5.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
         """
 ######################################
 # Python 3 is needed #
 ######################################
 """
     )
 
-_version = "0.5.0"
+_version = "0.5.1"
 
 setup(
     name="navabilitysdk",
     version=_version,
     license="Apache-2.0",
     author="NavAbility",
     author_email="info@navability.io",
```

### Comparing `navabilitysdk-0.5.0/src/navability/common/mutations.py` & `navabilitysdk-0.5.1/src/navability/common/mutations.py`

 * *Files identical despite different names*

### Comparing `navabilitysdk-0.5.0/src/navability/common/queries.py` & `navabilitysdk-0.5.1/src/navability/common/queries.py`

 * *Files identical despite different names*

### Comparing `navabilitysdk-0.5.0/src/navability/entities/__init__.py` & `navabilitysdk-0.5.1/src/navability/entities/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,17 +14,19 @@
     LinearRelative,
     Mixture,
     Point2Point2Range,
     Pose2AprilTag4Corners,
     Pose2Point2BearingRange,
     Pose2Point2Range,
     Pose2Pose2,
+    Pose3Pose3,
     Prior,
     PriorPoint2,
     PriorPose2,
+    PriorPose3,
 )
 from .navabilityclient import (
     NavAbilityClient,
     NavAbilityHttpsClient,
     NavAbilityWebsocketClient,
 )
 from .querydetail import QueryDetail
```

### Comparing `navabilitysdk-0.5.0/src/navability/entities/blob/blob.py` & `navabilitysdk-0.5.1/src/navability/entities/blob/blob.py`

 * *Files identical despite different names*

### Comparing `navabilitysdk-0.5.0/src/navability/entities/client.py` & `navabilitysdk-0.5.1/src/navability/entities/client.py`

 * *Files identical despite different names*

### Comparing `navabilitysdk-0.5.0/src/navability/entities/factor/distributions.py` & `navabilitysdk-0.5.1/src/navability/entities/factor/distributions.py`

 * *Files identical despite different names*

### Comparing `navabilitysdk-0.5.0/src/navability/entities/factor/factor.py` & `navabilitysdk-0.5.1/src/navability/entities/factor/factor.py`

 * *Files identical despite different names*

### Comparing `navabilitysdk-0.5.0/src/navability/entities/factor/inferencetypes.py` & `navabilitysdk-0.5.1/src/navability/entities/factor/inferencetypes.py`

 * *Files 4% similar despite different names*

```diff
@@ -92,14 +92,31 @@
 
     def dumps(self):
         return ZSchema().dumps(self)
 
     # TODO: Deserializing this.
 
 
+@dataclass
+class PriorPose3(InferenceType):
+    Z: Distribution
+
+    def __repr__(self):
+        return f"<{self.__class__.__name__}(Z={str(self.Z)})>"
+
+    def dump(self):
+        return ZSchema().dump(self)
+
+    def dumps(self):
+        return ZSchema().dumps(self)
+
+    # TODO: Deserializing this.
+
+
+
 """
 Create a prior factor for a Point2 with a distribution Z representing (x,y) prior
 information, e.g. `FullNormal([0.0, 0.0.0], diag([0.01, 0.01]))`.
 """
 
 
 @dataclass
@@ -130,14 +147,30 @@
     Z: Distribution
 
     def __repr__(self):
         return f"<{self.__class__.__name__}(Z={str(self.Z)})>"
 
     def dump(self):
         return ZSchema().dump(self)
+
+    def dumps(self):
+        return ZSchema().dumps(self)
+
+    # TODO: Deserializing this.
+
+
+@dataclass
+class Pose3Pose3(InferenceType):
+    Z: Distribution
+
+    def __repr__(self):
+        return f"<{self.__class__.__name__}(Z={str(self.Z)})>"
+
+    def dump(self):
+        return ZSchema().dump(self)
 
     def dumps(self):
         return ZSchema().dumps(self)
 
     # TODO: Deserializing this.
```

### Comparing `navabilitysdk-0.5.0/src/navability/entities/navabilityclient.py` & `navabilitysdk-0.5.1/src/navability/entities/navabilityclient.py`

 * *Files identical despite different names*

### Comparing `navabilitysdk-0.5.0/src/navability/entities/scope.py` & `navabilitysdk-0.5.1/src/navability/entities/scope.py`

 * *Files identical despite different names*

### Comparing `navabilitysdk-0.5.0/src/navability/entities/solve.py` & `navabilitysdk-0.5.1/src/navability/entities/solve.py`

 * *Files identical despite different names*

### Comparing `navabilitysdk-0.5.0/src/navability/entities/statusmessage.py` & `navabilitysdk-0.5.1/src/navability/entities/statusmessage.py`

 * *Files identical despite different names*

### Comparing `navabilitysdk-0.5.0/src/navability/entities/variable/ppe.py` & `navabilitysdk-0.5.1/src/navability/entities/variable/ppe.py`

 * *Files identical despite different names*

### Comparing `navabilitysdk-0.5.0/src/navability/entities/variable/variable.py` & `navabilitysdk-0.5.1/src/navability/entities/variable/variable.py`

 * *Files identical despite different names*

### Comparing `navabilitysdk-0.5.0/src/navability/entities/variable/variablenodedata.py` & `navabilitysdk-0.5.1/src/navability/entities/variable/variablenodedata.py`

 * *Files identical despite different names*

### Comparing `navabilitysdk-0.5.0/src/navability/services/blob.py` & `navabilitysdk-0.5.1/src/navability/services/blob.py`

 * *Files identical despite different names*

### Comparing `navabilitysdk-0.5.0/src/navability/services/factor.py` & `navabilitysdk-0.5.1/src/navability/services/factor.py`

 * *Files identical despite different names*

### Comparing `navabilitysdk-0.5.0/src/navability/services/solve.py` & `navabilitysdk-0.5.1/src/navability/services/solve.py`

 * *Files identical despite different names*

### Comparing `navabilitysdk-0.5.0/src/navability/services/status.py` & `navabilitysdk-0.5.1/src/navability/services/status.py`

 * *Files identical despite different names*

### Comparing `navabilitysdk-0.5.0/src/navability/services/utils.py` & `navabilitysdk-0.5.1/src/navability/services/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -54,17 +54,20 @@
     except Exception:
         return
 
 
 def MapVizApp(client, variableStartsWith=None):
     geometry_vis_link = f"https://app.navability.io/cloud/map/?userId={client.userId}&robotStartsWith={client.robotId}&sessionStartsWith={client.sessionId}"  # noqa: E501, B950
     if variableStartsWith is None:
+        # reset the filter
         geometry_vis_link = geometry_vis_link + "&variableStartsWith"
+    else:
         if 0 < len(variableStartsWith):
-            geometry_vis_link = geometry_vis_link + "=" + variableStartsWith
+            # this defines a filter
+            geometry_vis_link = geometry_vis_link + "&variableStartsWith=" + variableStartsWith
     print(geometry_vis_link)
     try:
         return md(
             f"""[![Navigate to Factor Graph](http://www.navability.io/wp-content/uploads/2022/03/geometric_map.png)]({geometry_vis_link})"""  # noqa: E501, B950
         )
     except Exception:
         return
```

### Comparing `navabilitysdk-0.5.0/src/navability/services/variable.py` & `navabilitysdk-0.5.1/src/navability/services/variable.py`

 * *Files identical despite different names*

### Comparing `navabilitysdk-0.5.0/src/navabilitysdk.egg-info/SOURCES.txt` & `navabilitysdk-0.5.1/src/navabilitysdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

