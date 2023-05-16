# Comparing `tmp/rtb_toolbox-0.1.1.tar.gz` & `tmp/rtb_toolbox-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rtb_toolbox-0.1.1.tar", max compression
+gzip compressed data, was "rtb_toolbox-0.1.2.tar", max compression
```

## Comparing `rtb_toolbox-0.1.1.tar` & `rtb_toolbox-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0        0 2023-04-14 21:56:06.455291 rtb_toolbox-0.1.1/README.md
--rw-r--r--   0        0        0      322 2023-04-14 22:14:05.543963 rtb_toolbox-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     4034 2023-04-14 21:53:58.999300 rtb_toolbox-0.1.1/src/rtb_toolbox/README.md
--rw-r--r--   0        0        0      264 2023-04-14 22:12:13.127853 rtb_toolbox-0.1.1/src/rtb_toolbox/__init__.py
--rw-r--r--   0        0        0     2298 2023-04-14 22:12:18.847856 rtb_toolbox-0.1.1/src/rtb_toolbox/forward_dynamics/__init__.py
--rw-r--r--   0        0        0     3533 2023-04-14 22:12:26.419864 rtb_toolbox-0.1.1/src/rtb_toolbox/forward_kinematics/__init__.py
--rw-r--r--   0        0        0     3097 2023-04-14 21:52:22.203974 rtb_toolbox-0.1.1/src/rtb_toolbox/frame/__init__.py
--rw-r--r--   0        0        0    33140 2023-04-14 21:54:20.903286 rtb_toolbox-0.1.1/src/rtb_toolbox/images/full_ik.png
--rw-r--r--   0        0        0    33229 2023-04-14 21:54:20.907286 rtb_toolbox-0.1.1/src/rtb_toolbox/images/partial_ik.png
--rw-r--r--   0        0        0     6569 2023-04-14 21:54:20.915286 rtb_toolbox-0.1.1/src/rtb_toolbox/images/tau1.png
--rw-r--r--   0        0        0     5005 2023-04-14 21:54:20.915286 rtb_toolbox-0.1.1/src/rtb_toolbox/images/tau2.png
--rw-r--r--   0        0        0   479230 2023-04-14 21:54:20.923286 rtb_toolbox-0.1.1/src/rtb_toolbox/images/trajectories.png
--rw-r--r--   0        0        0     7410 2023-04-14 22:12:36.779874 rtb_toolbox-0.1.1/src/rtb_toolbox/inverse_kinematics/__init__.py
--rw-r--r--   0        0        0     1673 2023-04-14 22:12:40.815878 rtb_toolbox-0.1.1/src/rtb_toolbox/link/__init__.py
--rw-r--r--   0        0        0       55 2023-04-14 21:52:22.347973 rtb_toolbox-0.1.1/src/rtb_toolbox/symbols.py
--rw-r--r--   0        0        0     1150 2023-04-14 21:52:22.231974 rtb_toolbox-0.1.1/src/rtb_toolbox/trajectory/__init__.py
--rw-r--r--   0        0        0     4732 2023-04-14 22:12:47.927885 rtb_toolbox-0.1.1/src/rtb_toolbox/utils/__init__.py
--rw-r--r--   0        0        0      790 1970-01-01 00:00:00.000000 rtb_toolbox-0.1.1/setup.py
--rw-r--r--   0        0        0      339 1970-01-01 00:00:00.000000 rtb_toolbox-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     4034 2023-04-14 22:16:46.136319 rtb_toolbox-0.1.2/README.md
+-rw-r--r--   0        0        0      322 2023-05-16 02:05:46.500976 rtb_toolbox-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4034 2023-04-14 22:17:39.372360 rtb_toolbox-0.1.2/src/rtb_toolbox/README.md
+-rw-r--r--   0        0        0      264 2023-04-14 22:12:13.127853 rtb_toolbox-0.1.2/src/rtb_toolbox/__init__.py
+-rw-r--r--   0        0        0     2298 2023-04-14 22:12:18.847856 rtb_toolbox-0.1.2/src/rtb_toolbox/forward_dynamics/__init__.py
+-rw-r--r--   0        0        0     3533 2023-05-16 02:02:18.160826 rtb_toolbox-0.1.2/src/rtb_toolbox/forward_kinematics/__init__.py
+-rw-r--r--   0        0        0     3097 2023-04-14 21:52:22.203974 rtb_toolbox-0.1.2/src/rtb_toolbox/frame/__init__.py
+-rw-r--r--   0        0        0    33140 2023-04-14 21:54:20.903286 rtb_toolbox-0.1.2/src/rtb_toolbox/images/full_ik.png
+-rw-r--r--   0        0        0    33229 2023-04-14 21:54:20.907286 rtb_toolbox-0.1.2/src/rtb_toolbox/images/partial_ik.png
+-rw-r--r--   0        0        0     6569 2023-04-14 21:54:20.915286 rtb_toolbox-0.1.2/src/rtb_toolbox/images/tau1.png
+-rw-r--r--   0        0        0     5005 2023-04-14 21:54:20.915286 rtb_toolbox-0.1.2/src/rtb_toolbox/images/tau2.png
+-rw-r--r--   0        0        0   479230 2023-04-14 21:54:20.923286 rtb_toolbox-0.1.2/src/rtb_toolbox/images/trajectories.png
+-rw-r--r--   0        0        0     7410 2023-04-14 22:12:36.779874 rtb_toolbox-0.1.2/src/rtb_toolbox/inverse_kinematics/__init__.py
+-rw-r--r--   0        0        0     1573 2023-05-16 02:04:53.020938 rtb_toolbox-0.1.2/src/rtb_toolbox/link/__init__.py
+-rw-r--r--   0        0        0      655 2023-05-16 02:04:19.044913 rtb_toolbox-0.1.2/src/rtb_toolbox/robots/puma260.py
+-rw-r--r--   0        0        0       55 2023-04-14 21:52:22.347973 rtb_toolbox-0.1.2/src/rtb_toolbox/symbols.py
+-rw-r--r--   0        0        0     1150 2023-04-14 21:52:22.231974 rtb_toolbox-0.1.2/src/rtb_toolbox/trajectory/__init__.py
+-rw-r--r--   0        0        0     4916 2023-05-16 02:04:29.872921 rtb_toolbox-0.1.2/src/rtb_toolbox/utils/__init__.py
+-rw-r--r--   0        0        0     4983 1970-01-01 00:00:00.000000 rtb_toolbox-0.1.2/setup.py
+-rw-r--r--   0        0        0     4373 1970-01-01 00:00:00.000000 rtb_toolbox-0.1.2/PKG-INFO
```

### Comparing `rtb_toolbox-0.1.1/src/rtb_toolbox/README.md` & `rtb_toolbox-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `rtb_toolbox-0.1.1/src/rtb_toolbox/forward_dynamics/__init__.py` & `rtb_toolbox-0.1.2/src/rtb_toolbox/forward_dynamics/__init__.py`

 * *Files identical despite different names*

### Comparing `rtb_toolbox-0.1.1/src/rtb_toolbox/forward_kinematics/__init__.py` & `rtb_toolbox-0.1.2/src/rtb_toolbox/forward_kinematics/__init__.py`

 * *Files identical despite different names*

### Comparing `rtb_toolbox-0.1.1/src/rtb_toolbox/frame/__init__.py` & `rtb_toolbox-0.1.2/src/rtb_toolbox/frame/__init__.py`

 * *Files identical despite different names*

### Comparing `rtb_toolbox-0.1.1/src/rtb_toolbox/images/full_ik.png` & `rtb_toolbox-0.1.2/src/rtb_toolbox/images/full_ik.png`

 * *Files identical despite different names*

### Comparing `rtb_toolbox-0.1.1/src/rtb_toolbox/images/partial_ik.png` & `rtb_toolbox-0.1.2/src/rtb_toolbox/images/partial_ik.png`

 * *Files identical despite different names*

### Comparing `rtb_toolbox-0.1.1/src/rtb_toolbox/images/tau1.png` & `rtb_toolbox-0.1.2/src/rtb_toolbox/images/tau1.png`

 * *Files identical despite different names*

### Comparing `rtb_toolbox-0.1.1/src/rtb_toolbox/images/tau2.png` & `rtb_toolbox-0.1.2/src/rtb_toolbox/images/tau2.png`

 * *Files identical despite different names*

### Comparing `rtb_toolbox-0.1.1/src/rtb_toolbox/images/trajectories.png` & `rtb_toolbox-0.1.2/src/rtb_toolbox/images/trajectories.png`

 * *Files identical despite different names*

### Comparing `rtb_toolbox-0.1.1/src/rtb_toolbox/inverse_kinematics/__init__.py` & `rtb_toolbox-0.1.2/src/rtb_toolbox/inverse_kinematics/__init__.py`

 * *Files identical despite different names*

### Comparing `rtb_toolbox-0.1.1/src/rtb_toolbox/link/__init__.py` & `rtb_toolbox-0.1.2/src/rtb_toolbox/link/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from rtb_toolbox.utils import compute_link_transformation, np
 
-
 class Link:
     def __init__(
             self,
             dhp=None,
             generalized_coordinate=None,
             offset=0,
             mass=None,
@@ -33,23 +32,18 @@
 
         if generalized_coordinate is None:
             if link_type == 'R':
                 self.generalized_coordinate = dhp[0]
             elif link_type == 'P':
                 self.generalized_coordinate = dhp[1]
 
-        if link_type == 'R':
-            self.dhp[0] += offset
-        else:
-            self.dhp[1] += offset
-
         self.mass = mass
         self.transformation_matrix = transformation_matrix
 
         if transformation_matrix is None:
             self.transformation_matrix = compute_link_transformation(dhp)
 
     def update(self):
-        self.transformation_matrix = compute_link_transformation(self.dhp)
+        self.transformation_matrix = compute_link_transformation(self.dhp, self.offset)
 
     def get_transformation_matrix(self):
         return self.transformation_matrix
```

### Comparing `rtb_toolbox-0.1.1/src/rtb_toolbox/trajectory/__init__.py` & `rtb_toolbox-0.1.2/src/rtb_toolbox/trajectory/__init__.py`

 * *Files identical despite different names*

### Comparing `rtb_toolbox-0.1.1/src/rtb_toolbox/utils/__init__.py` & `rtb_toolbox-0.1.2/src/rtb_toolbox/utils/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,20 +127,26 @@
         theta = np.arccos((np.trace(R) - 1) / 2.0)
 
         return np.r_[np.c_[l3, np.dot(
             np.eye(3) - l3 / 2.0 + (1.0 / theta - 1.0 / np.tan(theta / 2.0) / 2) * np.dot(l3, l3) / theta,
             p)], [[0, 0, 0, 0]]]
 
 
-def compute_link_transformation(dhp):
+def compute_link_transformation(dhp, offset=0, link_type='R'):
     rz = z_rotation_matrix(dhp[0])
     tz = translation_matrix(0, 0, dhp[1])
     tx = translation_matrix(dhp[2], 0, 0)
     rx = x_rotation_matrix(dhp[3])
 
+    if offset != 0:
+        if link_type == 'R':
+            rz @= z_rotation_matrix(offset)
+        else:
+            tz @= translation_matrix(0, 0, offset)
+
     return rz @ tz @ tx @ rx
 
 
 def compute_homogeneous_transformation(links, start, end):
     if end == 0:
         return sp.eye(4)
```

