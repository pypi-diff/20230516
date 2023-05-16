# Comparing `tmp/python-zephyr-0.0.6.tar.gz` & `tmp/python-zephyr-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-zephyr-0.0.6.tar", last modified: Mon May 15 15:08:49 2023, max compression
+gzip compressed data, was "python-zephyr-0.0.7.tar", last modified: Tue May 16 14:33:11 2023, max compression
```

## Comparing `python-zephyr-0.0.6.tar` & `python-zephyr-0.0.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 15:08:49.336676 python-zephyr-0.0.6/
--rw-rw-rw-   0        0        0     1105 2023-05-15 15:00:37.000000 python-zephyr-0.0.6/LICENSE.txt
--rw-rw-rw-   0        0        0     1369 2023-05-15 15:08:49.335677 python-zephyr-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      786 2023-05-15 15:00:37.000000 python-zephyr-0.0.6/README.md
--rw-rw-rw-   0        0        0       86 2023-05-15 15:00:37.000000 python-zephyr-0.0.6/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-05-15 15:08:49.329675 python-zephyr-0.0.6/python_zephyr.egg-info/
--rw-rw-rw-   0        0        0     1369 2023-05-15 15:08:49.000000 python-zephyr-0.0.6/python_zephyr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      335 2023-05-15 15:08:49.000000 python-zephyr-0.0.6/python_zephyr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 15:08:49.000000 python-zephyr-0.0.6/python_zephyr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-15 15:08:49.000000 python-zephyr-0.0.6/python_zephyr.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-15 15:08:49.000000 python-zephyr-0.0.6/python_zephyr.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-15 15:08:49.330677 python-zephyr-0.0.6/scripts/
--rw-rw-rw-   0        0        0     1570 2023-05-15 15:00:37.000000 python-zephyr-0.0.6/scripts/tc_report_upload.py
--rw-rw-rw-   0        0        0       42 2023-05-15 15:08:49.336676 python-zephyr-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1111 2023-05-15 15:07:59.000000 python-zephyr-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-15 15:08:49.334675 python-zephyr-0.0.6/zephyr/
--rw-rw-rw-   0        0        0       22 2023-05-15 15:00:37.000000 python-zephyr-0.0.6/zephyr/__init__.py
--rw-rw-rw-   0        0        0      875 2023-05-15 15:00:37.000000 python-zephyr-0.0.6/zephyr/exceptions.py
--rw-rw-rw-   0        0        0    15600 2023-05-15 15:00:37.000000 python-zephyr-0.0.6/zephyr/interface.py
--rw-rw-rw-   0        0        0    21826 2023-05-15 15:00:37.000000 python-zephyr-0.0.6/zephyr/tc_mgmt.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:33:11.356346 python-zephyr-0.0.7/
+-rw-rw-rw-   0        0        0     1105 2023-05-15 15:00:37.000000 python-zephyr-0.0.7/LICENSE.txt
+-rw-rw-rw-   0        0        0     1369 2023-05-16 14:33:11.356346 python-zephyr-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      786 2023-05-15 15:00:37.000000 python-zephyr-0.0.7/README.md
+-rw-rw-rw-   0        0        0       86 2023-05-15 15:00:37.000000 python-zephyr-0.0.7/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-05-16 14:33:11.348346 python-zephyr-0.0.7/python_zephyr.egg-info/
+-rw-rw-rw-   0        0        0     1369 2023-05-16 14:33:11.000000 python-zephyr-0.0.7/python_zephyr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      335 2023-05-16 14:33:11.000000 python-zephyr-0.0.7/python_zephyr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 14:33:11.000000 python-zephyr-0.0.7/python_zephyr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-16 14:33:11.000000 python-zephyr-0.0.7/python_zephyr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-16 14:33:11.000000 python-zephyr-0.0.7/python_zephyr.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-16 14:33:11.349346 python-zephyr-0.0.7/scripts/
+-rw-rw-rw-   0        0        0     1570 2023-05-15 15:00:37.000000 python-zephyr-0.0.7/scripts/tc_report_upload.py
+-rw-rw-rw-   0        0        0       42 2023-05-16 14:33:11.357345 python-zephyr-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1111 2023-05-16 14:32:43.000000 python-zephyr-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:33:11.354347 python-zephyr-0.0.7/zephyr/
+-rw-rw-rw-   0        0        0       22 2023-05-15 15:00:37.000000 python-zephyr-0.0.7/zephyr/__init__.py
+-rw-rw-rw-   0        0        0      875 2023-05-15 15:00:37.000000 python-zephyr-0.0.7/zephyr/exceptions.py
+-rw-rw-rw-   0        0        0    16014 2023-05-16 14:32:43.000000 python-zephyr-0.0.7/zephyr/interface.py
+-rw-rw-rw-   0        0        0    21826 2023-05-15 15:00:37.000000 python-zephyr-0.0.7/zephyr/tc_mgmt.py
```

### Comparing `python-zephyr-0.0.6/LICENSE.txt` & `python-zephyr-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `python-zephyr-0.0.6/PKG-INFO` & `python-zephyr-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-zephyr
-Version: 0.0.6
+Version: 0.0.7
 Summary: An easy to use Zephyr Scale library for python
 Home-page: https://bitbucket.org/melectrification/python-zephyr/src/master/
 Author: Atabey Onur
 Author-email: a.onur@munichelectrification.com
 Maintainer: Atabey Onur
 Maintainer-email: a.onur@munichelectrification.com
 Classifier: Programming Language :: Python :: 3
```

### Comparing `python-zephyr-0.0.6/README.md` & `python-zephyr-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `python-zephyr-0.0.6/python_zephyr.egg-info/PKG-INFO` & `python-zephyr-0.0.7/python_zephyr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-zephyr
-Version: 0.0.6
+Version: 0.0.7
 Summary: An easy to use Zephyr Scale library for python
 Home-page: https://bitbucket.org/melectrification/python-zephyr/src/master/
 Author: Atabey Onur
 Author-email: a.onur@munichelectrification.com
 Maintainer: Atabey Onur
 Maintainer-email: a.onur@munichelectrification.com
 Classifier: Programming Language :: Python :: 3
```

### Comparing `python-zephyr-0.0.6/scripts/tc_report_upload.py` & `python-zephyr-0.0.7/scripts/tc_report_upload.py`

 * *Files identical despite different names*

### Comparing `python-zephyr-0.0.6/setup.py` & `python-zephyr-0.0.7/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 with open(os.path.join(HERE, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 packages = find_packages(".")
 
 setup(
     name="python-zephyr",
-    version="0.0.6",
+    version="0.0.7",
     description="An easy to use Zephyr Scale library for python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     scripts=list(filter(os.path.isfile, (os.path.join("scripts/", f) for f in os.listdir("scripts/")))),
     author="Atabey Onur",
     author_email="a.onur@munichelectrification.com",
     maintainer="Atabey Onur",
```

### Comparing `python-zephyr-0.0.6/zephyr/exceptions.py` & `python-zephyr-0.0.7/zephyr/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-zephyr-0.0.6/zephyr/interface.py` & `python-zephyr-0.0.7/zephyr/interface.py`

 * *Files 4% similar despite different names*

```diff
@@ -332,14 +332,43 @@
                     folders.extend(data["values"])
                     time.sleep(timeout_s)
             found_ids = [folder["id"] for folder in folders if parent_id == folder["parentId"]]
             return found_ids
         else:
             return None
 
+    def get_all_children_folder_ids(
+        self,
+        parent_id: int = None,
+        folder_type: Literal["TEST_CASE", "TEST_PLAN", "TEST_CYCLE"] = "TEST_CASE",
+    ):
+        """
+        Recursively gets all children folder ids for a given parent folder id
+        :param parent_id:
+            id of the parent folder to search in
+        :param folder_type:
+            type of the folder to look for
+        :param timeout_s:
+            wait time between individual requests to Zephyr API
+        :return:
+            ids of all the children folders
+        """
+        next_children_ids = []
+        # check if we have children
+        found_children_ids = self.get_children_folder_ids(folder_type=folder_type, parent_id=parent_id)
+        if len(found_children_ids) > 0:  # if so...
+            for folder_id in found_children_ids:  # get their children invdividually
+                next_children_ids.extend(
+                    self.get_all_children_folder_ids(parent_id=folder_id, folder_type=folder_type)
+                )  # and do recursion into all their children
+            for next_id in next_children_ids:
+                if next_id not in found_children_ids:  # avoid adding duplicates to the found children
+                    found_children_ids.append(next_id)
+        return found_children_ids
+
     def get_environments(self, project_key: str = None, timeout_s: float = 1.0):
         """
         Gets all available test environments for a given project_key
         :param project_key:
             key of the project to search in (e.g. "BMC")
         :param timeout_s:
             wait time between individual requests to Zephyr API
@@ -417,22 +446,8 @@
         else:
             return None
 
 
 if __name__ == "__main__":
     with open("mytoken.txt", "r") as f:
         token = f.read()
-
-    zi = ZephyrInterface(token)
-    myFolderId = zi.get_folder_id(project_key="BMC", folder_name="2.6.5_ESS State Machine")
-    print("2.6.5_ESS State Machine folder Id: " + str(myFolderId))
-    myFolderId = zi.get_folder_id(project_key="BMC", folder_name="bolognasc")
-    print("All bolognasc folder Ids: " + str(myFolderId))
-    myFolderId = zi.get_folder_id(project_key="BMC", folder_name="Gtest")
-    print("GtestFolderId: " + str(myFolderId))
-    myFolderId = zi.get_folder_id(project_key="BMC", folder_name="bolognasc", parent_id=myFolderId)
-    print("bolognasc Folder Id within Gtest: " + str(myFolderId))
-    myChildrenIds = zi.get_children_folder_ids(folder_type="TEST_CASE", parent_id=myFolderId)
-    print("All children folder Ids of bolognasc Folder Id within Gtest: " + str(myChildrenIds))
-    print(zi.get_project_id("BMC"))
-    myStatuses = zi.get_statuses(project_key="BMC", status_type="TEST_EXECUTION")
-    print(myStatuses[0]["id"])
+    # room for some tests here
```

### Comparing `python-zephyr-0.0.6/zephyr/tc_mgmt.py` & `python-zephyr-0.0.7/zephyr/tc_mgmt.py`

 * *Files identical despite different names*

