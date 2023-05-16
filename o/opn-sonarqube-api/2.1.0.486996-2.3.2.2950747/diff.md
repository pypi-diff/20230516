# Comparing `tmp/opn_sonarqube_api-2.1.0.486996.tar.gz` & `tmp/opn_sonarqube_api-2.3.2.2950747.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/opn_sonarqube_api-2.1.0.486996.tar", last modified: Thu Sep 10 14:37:52 2020, max compression
+gzip compressed data, was "dist/opn_sonarqube_api-2.3.2.2950747.tar", last modified: Tue May 16 10:16:02 2023, max compression
```

## Comparing `opn_sonarqube_api-2.1.0.486996.tar` & `opn_sonarqube_api-2.3.2.2950747.tar`

### file list

```diff
@@ -1,42 +1,44 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-10 14:37:52.000000 opn_sonarqube_api-2.1.0.486996/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-10 14:37:52.000000 opn_sonarqube_api-2.1.0.486996/sonarqube_api/
--rw-rw-rw-   0 root         (0) root         (0)       96 2020-09-10 14:36:31.000000 opn_sonarqube_api-2.1.0.486996/sonarqube_api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      174 2020-09-10 14:36:31.000000 opn_sonarqube_api-2.1.0.486996/sonarqube_api/utils.py
--rw-rw-rw-   0 root         (0) root         (0)      204 2020-09-10 14:36:31.000000 opn_sonarqube_api-2.1.0.486996/sonarqube_api/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)    17756 2020-09-10 14:36:31.000000 opn_sonarqube_api-2.1.0.486996/sonarqube_api/sonar.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-10 14:37:52.000000 opn_sonarqube_api-2.1.0.486996/sonarqube_api/sonarapi/
--rw-rw-rw-   0 root         (0) root         (0)       36 2020-09-10 14:36:31.000000 opn_sonarqube_api-2.1.0.486996/sonarqube_api/sonarapi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      586 2020-09-10 14:36:31.000000 opn_sonarqube_api-2.1.0.486996/sonarqube_api/sonarapi/authentication.py
--rw-rw-rw-   0 root         (0) root         (0)      469 2020-09-10 14:36:31.000000 opn_sonarqube_api-2.1.0.486996/sonarqube_api/sonarapi/users.py
--rw-rw-rw-   0 root         (0) root         (0)     1891 2020-09-10 14:36:31.000000 opn_sonarqube_api-2.1.0.486996/sonarqube_api/sonarapi/user_token.py
--rw-rw-rw-   0 root         (0) root         (0)     1193 2020-09-10 14:36:31.000000 opn_sonarqube_api-2.1.0.486996/sonarqube_api/sonarapi/settings.py
--rw-rw-rw-   0 root         (0) root         (0)     3294 2020-09-10 14:36:31.000000 opn_sonarqube_api-2.1.0.486996/sonarqube_api/sonarapi/rules.py
--rw-rw-rw-   0 root         (0) root         (0)     9729 2020-09-10 14:36:31.000000 opn_sonarqube_api-2.1.0.486996/sonarqube_api/sonarapi/permissions.py
--rw-rw-rw-   0 root         (0) root         (0)      743 2020-09-10 14:36:31.000000 opn_sonarqube_api-2.1.0.486996/sonarqube_api/sonarapi/components.py
--rw-rw-rw-   0 root         (0) root         (0)     4868 2020-09-10 14:36:31.000000 opn_sonarqube_api-2.1.0.486996/sonarqube_api/sonarapi/resources.py
--rw-rw-rw-   0 root         (0) root         (0)     1309 2020-09-10 14:36:31.000000 opn_sonarqube_api-2.1.0.486996/sonarqube_api/sonarapi/metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     7523 2020-09-10 14:36:31.000000 opn_sonarqube_api-2.1.0.486996/sonarqube_api/sonarapi/qualitygates.py
--rw-rw-rw-   0 root         (0) root         (0)     2566 2020-09-10 14:36:31.000000 opn_sonarqube_api-2.1.0.486996/sonarqube_api/sonarapi/groups.py
--rw-rw-rw-   0 root         (0) root         (0)     6505 2020-09-10 14:36:31.000000 opn_sonarqube_api-2.1.0.486996/sonarqube_api/sonarapi/qualityprofiles.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-10 14:37:52.000000 opn_sonarqube_api-2.1.0.486996/sonarqube_api/cmd/
--rw-rw-rw-   0 root         (0) root         (0)       33 2020-09-10 14:36:31.000000 opn_sonarqube_api-2.1.0.486996/sonarqube_api/cmd/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5675 2020-09-10 14:36:31.000000 opn_sonarqube_api-2.1.0.486996/sonarqube_api/cmd/export_rules.py
--rw-rw-rw-   0 root         (0) root         (0)     5331 2020-09-10 14:36:31.000000 opn_sonarqube_api-2.1.0.486996/sonarqube_api/cmd/migrate_rules.py
--rw-rw-rw-   0 root         (0) root         (0)     3248 2020-09-10 14:36:31.000000 opn_sonarqube_api-2.1.0.486996/sonarqube_api/cmd/activate_rules.py
--rw-rw-rw-   0 root         (0) root         (0)     3015 2020-09-10 14:36:31.000000 opn_sonarqube_api-2.1.0.486996/sonarqube_api/api.py
--rw-r--r--   0 root         (0) root         (0)     5923 2020-09-10 14:37:52.000000 opn_sonarqube_api-2.1.0.486996/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      238 2020-09-10 14:36:31.000000 opn_sonarqube_api-2.1.0.486996/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)     4135 2020-09-10 14:36:31.000000 opn_sonarqube_api-2.1.0.486996/README.rst
--rw-rw-rw-   0 root         (0) root         (0)       67 2020-09-10 14:36:31.000000 opn_sonarqube_api-2.1.0.486996/DESCRIPTION.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-10 14:37:52.000000 opn_sonarqube_api-2.1.0.486996/tests/
--rw-rw-rw-   0 root         (0) root         (0)       24 2020-09-10 14:36:31.000000 opn_sonarqube_api-2.1.0.486996/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15993 2020-09-10 14:36:31.000000 opn_sonarqube_api-2.1.0.486996/tests/test_api.py
--rw-rw-rw-   0 root         (0) root         (0)     2353 2020-09-10 14:37:52.000000 opn_sonarqube_api-2.1.0.486996/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-10 14:37:52.000000 opn_sonarqube_api-2.1.0.486996/opn_sonarqube_api.egg-info/
--rw-r--r--   0 root         (0) root         (0)       20 2020-09-10 14:37:52.000000 opn_sonarqube_api-2.1.0.486996/opn_sonarqube_api.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2020-09-10 14:37:52.000000 opn_sonarqube_api-2.1.0.486996/opn_sonarqube_api.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     5923 2020-09-10 14:37:52.000000 opn_sonarqube_api-2.1.0.486996/opn_sonarqube_api.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      208 2020-09-10 14:37:52.000000 opn_sonarqube_api-2.1.0.486996/opn_sonarqube_api.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       14 2020-09-10 14:37:52.000000 opn_sonarqube_api-2.1.0.486996/opn_sonarqube_api.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1058 2020-09-10 14:37:52.000000 opn_sonarqube_api-2.1.0.486996/opn_sonarqube_api.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       38 2020-09-10 14:37:52.000000 opn_sonarqube_api-2.1.0.486996/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 10:16:02.000000 opn_sonarqube_api-2.3.2.2950747/
+-rw-rw-rw-   0 root         (0) root         (0)      238 2023-05-16 10:15:22.000000 opn_sonarqube_api-2.3.2.2950747/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-16 10:16:02.000000 opn_sonarqube_api-2.3.2.2950747/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 10:16:02.000000 opn_sonarqube_api-2.3.2.2950747/sonarqube_api/
+-rw-rw-rw-   0 root         (0) root         (0)     3862 2023-05-16 10:15:22.000000 opn_sonarqube_api-2.3.2.2950747/sonarqube_api/api.py
+-rw-rw-rw-   0 root         (0) root         (0)      204 2023-05-16 10:15:22.000000 opn_sonarqube_api-2.3.2.2950747/sonarqube_api/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)      174 2023-05-16 10:15:22.000000 opn_sonarqube_api-2.3.2.2950747/sonarqube_api/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    18515 2023-05-16 10:15:22.000000 opn_sonarqube_api-2.3.2.2950747/sonarqube_api/sonar.py
+-rw-rw-rw-   0 root         (0) root         (0)       96 2023-05-16 10:15:22.000000 opn_sonarqube_api-2.3.2.2950747/sonarqube_api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 10:16:02.000000 opn_sonarqube_api-2.3.2.2950747/sonarqube_api/cmd/
+-rw-rw-rw-   0 root         (0) root         (0)     5675 2023-05-16 10:15:22.000000 opn_sonarqube_api-2.3.2.2950747/sonarqube_api/cmd/export_rules.py
+-rw-rw-rw-   0 root         (0) root         (0)     5331 2023-05-16 10:15:22.000000 opn_sonarqube_api-2.3.2.2950747/sonarqube_api/cmd/migrate_rules.py
+-rw-rw-rw-   0 root         (0) root         (0)       33 2023-05-16 10:15:22.000000 opn_sonarqube_api-2.3.2.2950747/sonarqube_api/cmd/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3248 2023-05-16 10:15:22.000000 opn_sonarqube_api-2.3.2.2950747/sonarqube_api/cmd/activate_rules.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 10:16:02.000000 opn_sonarqube_api-2.3.2.2950747/sonarqube_api/sonarapi/
+-rw-rw-rw-   0 root         (0) root         (0)     3294 2023-05-16 10:15:22.000000 opn_sonarqube_api-2.3.2.2950747/sonarqube_api/sonarapi/rules.py
+-rw-rw-rw-   0 root         (0) root         (0)      764 2023-05-16 10:15:22.000000 opn_sonarqube_api-2.3.2.2950747/sonarqube_api/sonarapi/projects.py
+-rw-rw-rw-   0 root         (0) root         (0)     1193 2023-05-16 10:15:22.000000 opn_sonarqube_api-2.3.2.2950747/sonarqube_api/sonarapi/settings.py
+-rw-rw-rw-   0 root         (0) root         (0)     6268 2023-05-16 10:15:22.000000 opn_sonarqube_api-2.3.2.2950747/sonarqube_api/sonarapi/qualityprofiles.py
+-rw-rw-rw-   0 root         (0) root         (0)     1309 2023-05-16 10:15:22.000000 opn_sonarqube_api-2.3.2.2950747/sonarqube_api/sonarapi/metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)      586 2023-05-16 10:15:22.000000 opn_sonarqube_api-2.3.2.2950747/sonarqube_api/sonarapi/authentication.py
+-rw-rw-rw-   0 root         (0) root         (0)      743 2023-05-16 10:15:22.000000 opn_sonarqube_api-2.3.2.2950747/sonarqube_api/sonarapi/components.py
+-rw-rw-rw-   0 root         (0) root         (0)     9702 2023-05-16 10:15:22.000000 opn_sonarqube_api-2.3.2.2950747/sonarqube_api/sonarapi/permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)     4868 2023-05-16 10:15:22.000000 opn_sonarqube_api-2.3.2.2950747/sonarqube_api/sonarapi/resources.py
+-rw-rw-rw-   0 root         (0) root         (0)      469 2023-05-16 10:15:22.000000 opn_sonarqube_api-2.3.2.2950747/sonarqube_api/sonarapi/users.py
+-rw-rw-rw-   0 root         (0) root         (0)       36 2023-05-16 10:15:22.000000 opn_sonarqube_api-2.3.2.2950747/sonarqube_api/sonarapi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7502 2023-05-16 10:15:22.000000 opn_sonarqube_api-2.3.2.2950747/sonarqube_api/sonarapi/qualitygates.py
+-rw-rw-rw-   0 root         (0) root         (0)     2562 2023-05-16 10:15:22.000000 opn_sonarqube_api-2.3.2.2950747/sonarqube_api/sonarapi/groups.py
+-rw-rw-rw-   0 root         (0) root         (0)      719 2023-05-16 10:15:22.000000 opn_sonarqube_api-2.3.2.2950747/sonarqube_api/sonarapi/branches.py
+-rw-rw-rw-   0 root         (0) root         (0)     1891 2023-05-16 10:15:22.000000 opn_sonarqube_api-2.3.2.2950747/sonarqube_api/sonarapi/user_token.py
+-rw-r--r--   0 root         (0) root         (0)     5918 2023-05-16 10:16:02.000000 opn_sonarqube_api-2.3.2.2950747/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4135 2023-05-16 10:15:22.000000 opn_sonarqube_api-2.3.2.2950747/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 10:16:02.000000 opn_sonarqube_api-2.3.2.2950747/opn_sonarqube_api.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5918 2023-05-16 10:16:02.000000 opn_sonarqube_api-2.3.2.2950747/opn_sonarqube_api.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1128 2023-05-16 10:16:02.000000 opn_sonarqube_api-2.3.2.2950747/opn_sonarqube_api.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-05-16 10:16:02.000000 opn_sonarqube_api-2.3.2.2950747/opn_sonarqube_api.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-05-16 10:16:02.000000 opn_sonarqube_api-2.3.2.2950747/opn_sonarqube_api.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)      208 2023-05-16 10:16:02.000000 opn_sonarqube_api-2.3.2.2950747/opn_sonarqube_api.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 10:16:02.000000 opn_sonarqube_api-2.3.2.2950747/opn_sonarqube_api.egg-info/dependency_links.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 10:16:02.000000 opn_sonarqube_api-2.3.2.2950747/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-05-16 10:15:22.000000 opn_sonarqube_api-2.3.2.2950747/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15993 2023-05-16 10:15:22.000000 opn_sonarqube_api-2.3.2.2950747/tests/test_api.py
+-rw-rw-rw-   0 root         (0) root         (0)       67 2023-05-16 10:15:22.000000 opn_sonarqube_api-2.3.2.2950747/DESCRIPTION.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2348 2023-05-16 10:16:02.000000 opn_sonarqube_api-2.3.2.2950747/setup.py
```

### Comparing `opn_sonarqube_api-2.1.0.486996/sonarqube_api/sonar.py` & `opn_sonarqube_api-2.3.2.2950747/sonarqube_api/sonar.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 from .sonarapi.qualityprofiles import SonarAPIQualityProfile
 from .sonarapi.resources import SonarAPIResources
 from .sonarapi.rules import SonarAPIRules
 from .sonarapi.settings import SonarAPISettings
 from .sonarapi.user_token import SonarAPIUserToken
 from .sonarapi.users import SonarAPIUser
 from .sonarapi.components import SonarAPIComponents
+from .sonarapi.projects import SonarAPIProjects
+from .sonarapi.branches import SonarAPIBranches
 
 
 class SonarAPI(object):
     """
     Adapter for SonarQube's web service API.
     """
     # Default host is local
@@ -40,14 +42,16 @@
         self._qualityprofile = SonarAPIQualityProfile(api=self.api)
         self._resources = SonarAPIResources(api=self.api)
         self._rules = SonarAPIRules(api=self.api)
         self._settings = SonarAPISettings(api=self.api)
         self._qgates = SonarAPIQGates(api=self.api)
         self._authentication = SonarAPIAuthentication(api=self.api)
         self._components = SonarAPIComponents(api=self.api)
+        self._projects = SonarAPIProjects(api=self.api)
+        self._branches = SonarAPIBranches(api=self.api)
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
     # #
     # #  API
     # #
 
@@ -465,7 +469,27 @@
         """
         get projets list.
 
         :param query: query to send
         :return: request response
         """
         return self._components.search_project(query, ps, facets, f)
+
+    def search_projects(self, query):
+        """
+        search project
+
+        :param query: Limit search to:
+            component names that contain the supplied string
+            component keys that contain the supplied string
+        :return: request response
+        """
+        return self._projects.search(query)
+
+    def branches_list(self, project):
+        """
+        get project branches
+
+        :param project: List the branches of a project.
+        :return: request response
+        """
+        return self._branches.get(project)
```

### Comparing `opn_sonarqube_api-2.1.0.486996/sonarqube_api/sonarapi/authentication.py` & `opn_sonarqube_api-2.3.2.2950747/sonarqube_api/sonarapi/authentication.py`

 * *Files identical despite different names*

### Comparing `opn_sonarqube_api-2.1.0.486996/sonarqube_api/sonarapi/user_token.py` & `opn_sonarqube_api-2.3.2.2950747/sonarqube_api/sonarapi/user_token.py`

 * *Files identical despite different names*

### Comparing `opn_sonarqube_api-2.1.0.486996/sonarqube_api/sonarapi/settings.py` & `opn_sonarqube_api-2.3.2.2950747/sonarqube_api/sonarapi/settings.py`

 * *Files identical despite different names*

### Comparing `opn_sonarqube_api-2.1.0.486996/sonarqube_api/sonarapi/rules.py` & `opn_sonarqube_api-2.3.2.2950747/sonarqube_api/sonarapi/rules.py`

 * *Files identical despite different names*

### Comparing `opn_sonarqube_api-2.1.0.486996/sonarqube_api/sonarapi/permissions.py` & `opn_sonarqube_api-2.3.2.2950747/sonarqube_api/sonarapi/permissions.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         """
         # Build main data to post
         data = {
             'q': template_name
         }
 
         # Make call (might raise exception) and return
-        res = self._api._make_call('post', self.PERMISSIONS_TEMPLATE_LIST_ENDPOINT, data=data)
+        res = self._api._make_call('get', self.PERMISSIONS_TEMPLATE_LIST_ENDPOINT, data=data)
         return res if res.status_code == 204 else json.loads(res.content)
 
     def delete_template(self, template_id):
         """
         Delete template id.
 
         :param template_id: id of the template to delete
@@ -101,21 +101,20 @@
     def list_groups_of_template(self, template_id):
         """
         get permission template's groups.
 
         :param template_id: id of the template to update
         :return: request response
         """
-        # Build main data to post
-        data = {
-            'templateId': template_id,
-        }
+        # Build main data to get
+        text="?templateId"
+        combined=text+"="+template_id
 
         # Make call (might raise exception) and return
-        res = self._api._make_call('post', self.PERMISSIONS_TEMPLATE_GROUPS, data=data)
+        res = self._api._get_call(self.PERMISSIONS_TEMPLATE_GROUPS, params=combined)
         return res if res.status_code == 204 else json.loads(res.content)
 
     def add_group_to_template(self, template_id, group_name, permission):
         """
         update permission template.
 
         :param template_id: id of the template to update
@@ -200,15 +199,15 @@
         # Build main data to post
         data = {
             'q': user_name,
             'ps': 100
         }
 
         # Make call (might raise exception) and return
-        res = self._api._make_call('post', self.PERMISSIONS_SEARCH_USER, data=data)
+        res = self._api._make_call('get', self.PERMISSIONS_SEARCH_USER, data=data)
         return res if res.status_code == 204 else json.loads(res.content)
 
     def add_permission_to_group(self, group_name, permission):
         """
         update group's permission.
 
         :param group_name: name of the group to associate
@@ -246,16 +245,14 @@
     def search_permission_for_group(self, group_name):
         """
         list groups permission.
 
         :param group_name: name of the group to associate
         :return: request response
         """
-        # Build main data to post
-        data = {
-            'q': group_name,
-            'ps': 100
-        }
+        # Build main data to get
+        text="?ps=100&q"
+        combined=text+"="+group_name
 
         # Make call (might raise exception) and return
-        res = self._api._make_call('post', self.PERMISSIONS_SEARCH_GROUP, data=data)
+        res = self._api._get_call(self.PERMISSIONS_SEARCH_GROUP, params=combined)
         return res if res.status_code == 204 else json.loads(res.content)
```

### Comparing `opn_sonarqube_api-2.1.0.486996/sonarqube_api/sonarapi/components.py` & `opn_sonarqube_api-2.3.2.2950747/sonarqube_api/sonarapi/components.py`

 * *Files identical despite different names*

### Comparing `opn_sonarqube_api-2.1.0.486996/sonarqube_api/sonarapi/resources.py` & `opn_sonarqube_api-2.3.2.2950747/sonarqube_api/sonarapi/resources.py`

 * *Files identical despite different names*

### Comparing `opn_sonarqube_api-2.1.0.486996/sonarqube_api/sonarapi/metrics.py` & `opn_sonarqube_api-2.3.2.2950747/sonarqube_api/sonarapi/metrics.py`

 * *Files identical despite different names*

### Comparing `opn_sonarqube_api-2.1.0.486996/sonarqube_api/sonarapi/qualitygates.py` & `opn_sonarqube_api-2.3.2.2950747/sonarqube_api/sonarapi/qualitygates.py`

 * *Files 10% similar despite different names*

```diff
@@ -51,32 +51,32 @@
     def list(self):
         """
         list quality gates.
 
         :return: request response
         """
         # Make call (might raise exception) and return
-        res = self._api._make_call('get', self.LIST_ENDPOINT)
+        res = self._api._get_call(self.LIST_ENDPOINT)
         return res if res.status_code == 204 else json.loads(res.content)
 
     def show(self, id=None, name=None):
         """
         get quality gate details, using id or name (id is prior is both are set)
 
         :param id: id of the quality gate
         :param name: name of the quality gate
         :return: request response
         """
-        # Build main data to post
+        # Build main data to get
         params = {
             'id' if id is not None else 'name': id if id is not None else name
         }
 
         # Make call (might raise exception) and return
-        res = self._api._make_call('get', self.DETAIL_ENDPOINT, params=params)
+        res = self._api._get_call(self.DETAIL_ENDPOINT, params=params)
         return res if res.status_code == 204 else json.loads(res.content)
 
     def create(self, name):
         """
         create a new empty quality agte
 
         :param name: name of the quality gate
@@ -109,47 +109,42 @@
         # Make call (return nothing)
         self._api._make_call('post', self.DESTROY_ENDPOINT, data=data)
 
     def select(self, gateId, projectId):
         """
         assign a quality gate to a project
 
-        :param gateId: id of the quality gate
-        :param projectid: id of the project
+        :param gateId: id of the quality gate (DEPRECATED -> switch to gateName)
+        :param projectKey: id of the project
         :return: 204 no content
         """
-        # Build main data to post
+        # Build main data to get
         data = {
             'gateId': gateId,
-            'projectId': projectId
+            'projectKey': projectId
         }
 
         # Make call (return nothing)
-        self._api._make_call('post', self.SELECT_ENDPOINT, data=data)
+        self._api._get_call(self.SELECT_ENDPOINT, params=data)
 
     def search_project(self, gateId, query, ps=50, selected='all'):
         """
         get projets list.
 
-        :param gateId: Id of the qualitygate
+        :param gateId: Id of the qualitygate (DEPRECATED -> switch to gateName)
         :param query: query to send
         :param ps: pageSize
         :param selected: all/selected/deselected
         :return: request response
         """
-        # Build main data to post
-        query = {
-            'query': query,
-            'ps': ps,
-            'selected': selected,
-            'gateId': gateId
-        }
-
+        # Build main data to get
+        combined="?gateId="+gateId+"&ps="+ps+"&selected="+selected+"&q="+query
+        
         # Make call (might raise exception) and return
-        res = self._api._make_call('post', self.SEARCH_ENDPOINT, params=query)
+        res = self._api._get_call(self.SEARCH_ENDPOINT, params=combined)
         return res if res.status_code == 204 else json.loads(res.content)
 
     def get_for_project(self, project, organization='default-organization'):
         """
         get qg summary for a project
 
         :param project: project to use
@@ -159,15 +154,15 @@
         # Build main data to post
         data = {
             'project': project,
             'organization': organization
         }
 
         # Make call (might raise exception) and return
-        res = self._api._make_call('post', self.PROJECT_ENDPOINT, data=data)
+        res = self._api._get_call(self.PROJECT_ENDPOINT, params=data)
         return res if res.status_code == 204 else json.loads(res.content)
 
     def create_condition(self, gateid, metric, op, error):
         """
         create a condition for a quality gate
 
         :param gateid: id of the quality gate
```

### Comparing `opn_sonarqube_api-2.1.0.486996/sonarqube_api/sonarapi/groups.py` & `opn_sonarqube_api-2.3.2.2950747/sonarqube_api/sonarapi/groups.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,21 +32,20 @@
     def search_group(self, group_name):
         """
         Search group with specified name.
 
         :param group_name: name of the group
         :return: request response
         """
-        # Build main data to post
-        data = {
-            'q': group_name
-        }
+        # Build main data to get
+        text="?q"
+        combined=text+"="+group_name
 
         # Make call (might raise exception) and return
-        res = self._api._make_call('post', self.GROUP_LIST_ENDPOINT, data=data)
+        res = self._api._get_call(self.GROUP_LIST_ENDPOINT, params=combined)
         return res if res.status_code == 204 else json.loads(res.content)
 
     def delete_group(self, group_id):
         """
         Delete group id.
 
         :param group_id: id of the group
```

### Comparing `opn_sonarqube_api-2.1.0.486996/sonarqube_api/sonarapi/qualityprofiles.py` & `opn_sonarqube_api-2.3.2.2950747/sonarqube_api/sonarapi/qualityprofiles.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,176 +1,169 @@
-import json
-import re
-
-class SonarAPIQualityProfile(object):
-    PROJECTS_ENDPOINT = '/api/qualityprofiles/projects'
-    RULES_ACTIVATION_ENDPOINT = '/api/qualityprofiles/activate_rule'
-    CREATE_QUALITY_PROFILE_ENDPOINT = '/api/qualityprofiles/create'
-    SEARCH_QUALITY_PROFILE_ENDPOINT = '/api/qualityprofiles/search'
-    ADD_PROJECT_TO_QUALITY_PROFILE_ENDPOINT = '/api/qualityprofiles/add_project'
-    RESTORE_QUALITY_PROFILE_FROM_XML_ENDPOINT = '/api/qualityprofiles/restore'
-    DELETE_QUALITY_PROFILE_ENDPOINT = '/api/qualityprofiles/delete'
-
-    def __init__(self, api=None):
-        self._api = api
-
-    def project(self, key, query, ps=50, selected='all'):
-        """
-        get projets list.
-
-        :param key: Id of the qualityprofile
-        :param query: query to send
-        :param ps: pageSize
-        :param selected: all/selected/deselected
-        :return: request response
-        """
-        # Build main data to post
-        query = {
-            'query': query,
-            'ps': ps,
-            'selected': selected,
-            'key': key
-        }
-
-        # Make call (might raise exception) and return
-        res = self._api._make_call('post', self.PROJECTS_ENDPOINT, params=query)
-        return res if res.status_code == 204 else json.loads(res.content)
-
-    def restore_quality_profile_from_xml(self, backup, project_name):
-        """
-        Create a quality profile with rules from a xml file
-
-        :param project_name: name of the project, used to name the profile
-        :param backup: contents of xml file to config quality profile
-        :return:
-        """
-
-        # Retrieve the language in the xml
-        r = re.search('<language>(.*)</language>', backup)
-        if r is not None:
-            language = r.group(1)
-        else:
-            print('error no language set in xml')
-
-        # Replace the profile name by the project name
-        backup = re.sub(r"<name>(.*?)</name>", r"<name>" + project_name + "</name>", backup)
-
-        # Check if the qg exists already, and if so, deletes it
-        existing_qp = self.search_quality_profile(project_name)
-        if existing_qp is not None and existing_qp["profiles"] is not None:
-            for profile in existing_qp["profiles"]:
-                if profile['name'] == project_name and profile['language'] == language:
-                    self.delete_quality_profile(project_name, language)
-
-        # Make call (might raise exception) and return
-        res = self._api._make_call('post', self.RESTORE_QUALITY_PROFILE_FROM_XML_ENDPOINT, files=dict(backup=backup))
-        return res if res.status_code == 204 else json.loads(res.content)
-
-    def search_quality_profile(self, profile_name):
-        """
-
-        :param profile_name:
-        :return:
-        """
-
-        data = {
-            'profileName': profile_name
-        }
-
-        # Make call (might raise exception) and return
-        res = self._api._make_call('get', self.SEARCH_QUALITY_PROFILE_ENDPOINT, data)
-        return res if res.status_code == 204 else json.loads(res.content)
-
-    def delete_quality_profile(self, profile_name, language):
-        """
-
-        :param profileName:
-        :return:
-        """
-
-        data = {
-            'profileName': profile_name,
-            'language': language
-        }
-
-        # Make call (return nothing)
-        self._api._make_call('post', self.DELETE_QUALITY_PROFILE_ENDPOINT, data)
-
-    def create_quality_profile(self, key, name, language, languagename,
-                               isinherited=False, isdefault=False, organization="default-organization"):
-        """
-        Create a quality profile
-
-        :param key:
-        :param name: name of the profile
-        :param language: language used (java, C#...)
-        :param languagename: language name (may be different from the language)
-        :param isinherited: profile inherited
-        :param isdefault: default rules
-        :param organization:
-        :return: request response
-        """
-
-        data = {
-            'key': key,
-            'name': name,
-            'language': language,
-            'languageName': languagename,
-            'isInherited': isinherited,
-            'isDefault': isdefault,
-            'organization': organization
-        }
-
-        # Make call (might raise exception) and return
-        res = self._api._make_call('post', self.CREATE_QUALITY_PROFILE_ENDPOINT, data=data)
-        return res if res.status_code == 204 else json.loads(res.content)
-
-    def add_project_to_quality_profile(self, profile_key, project_key):
-        """
-        Adds the project to the quality profile
-
-        :param profile_key: key of the profile
-        :param project_key: key of the project
-        :return: request response
-        """
-
-        data = {
-            'profileKey': profile_key,
-            'projectKey': project_key
-        }
-
-        # Make call (might raise exception) and return no content
-        self._api._make_call('post', self.ADD_PROJECT_TO_QUALITY_PROFILE_ENDPOINT, data=data)
-
-    def activate_rule(self, key, profile_key, reset=False, severity=None,
-                      **params):
-        """
-        Activate a rule for a given quality profile.
-
-        :param key: key of the rule
-        :param profile_key: key of the profile
-        :param reset: reset severity and params to default
-        :param severity: severity of rule for given profile
-        :param params: customized parameters for the rule
-        :return: request response
-        """
-        # Build main data to post
-        data = {
-            'rule_key': key,
-            'profile_key': profile_key,
-            'reset': reset and 'true' or 'false'
-        }
-
-        if not reset:
-            # No reset, Add severity if given (if not default will be used?)
-            if severity:
-                data['severity'] = severity.upper()
-
-            # Add params if we have any
-            # Note: sort by key to allow checking easily
-            params = ';'.join('{}={}'.format(k, v) for k, v in sorted(params.items()) if v)
-            if params:
-                data['params'] = params
-
-        # Make call (might raise exception) and return
-        res = self._api._make_call('post', self.RULES_ACTIVATION_ENDPOINT, data=data)
-        return res if res.status_code == 204 else json.loads(res.content)
+import json
+import re
+
+class SonarAPIQualityProfile(object):
+    PROJECTS_ENDPOINT = '/api/qualityprofiles/projects'
+    RULES_ACTIVATION_ENDPOINT = '/api/qualityprofiles/activate_rule'
+    CREATE_QUALITY_PROFILE_ENDPOINT = '/api/qualityprofiles/create'
+    SEARCH_QUALITY_PROFILE_ENDPOINT = '/api/qualityprofiles/search'
+    ADD_PROJECT_TO_QUALITY_PROFILE_ENDPOINT = '/api/qualityprofiles/add_project'
+    RESTORE_QUALITY_PROFILE_FROM_XML_ENDPOINT = '/api/qualityprofiles/restore'
+    DELETE_QUALITY_PROFILE_ENDPOINT = '/api/qualityprofiles/delete'
+
+    def __init__(self, api=None):
+        self._api = api
+
+    def project(self, key, query, ps=50, selected='all'):
+        """
+        get projets list.
+
+        :param key: Id of the qualityprofile
+        :param query: query to send
+        :param ps: pageSize
+        :param selected: all/selected/deselected
+        :return: request response
+        """
+        # Build main data to get
+        combined="?key="+key+"&ps="+ps+"&selected="+selected+"&q="+query
+
+        # Make call (might raise exception) and return
+        res = self._api._get_call(self.PROJECTS_ENDPOINT, params=combined)
+        return res if res.status_code == 204 else json.loads(res.content)
+
+    def restore_quality_profile_from_xml(self, backup, project_name):
+        """
+        Create a quality profile with rules from a xml file
+
+        :param project_name: name of the project, used to name the profile
+        :param backup: contents of xml file to config quality profile
+        :return:
+        """
+
+        # Retrieve the language in the xml
+        r = re.search('<language>(.*)</language>', backup)
+        if r is not None:
+            language = r.group(1)
+        else:
+            print('error no language set in xml')
+
+        # Replace the profile name by the project name
+        backup = re.sub(r"<name>(.*?)</name>", r"<name>" + project_name + "</name>", backup)
+
+        # Check if the qg exists already, and if so, deletes it
+        existing_qp = self.search_quality_profile(project_name)
+        if existing_qp is not None and existing_qp["profiles"] is not None:
+            for profile in existing_qp["profiles"]:
+                if profile['name'] == project_name and profile['language'] == language:
+                    self.delete_quality_profile(project_name, language)
+
+        # Make call (might raise exception) and return
+        res = self._api._make_call('post', self.RESTORE_QUALITY_PROFILE_FROM_XML_ENDPOINT, files=dict(backup=backup))
+        return res if res.status_code == 204 else json.loads(res.content)
+
+    def search_quality_profile(self, profile_name):
+        """
+
+        :param profile_name:
+        :return:
+        """   
+        text="?qualityProfile"
+        combined=text+"="+profile_name
+
+        # Make call (might raise exception) and return
+        res = self._api._get_call(self.SEARCH_QUALITY_PROFILE_ENDPOINT, params=combined)
+        return res if res.status_code == 204 else json.loads(res.content)
+
+    def delete_quality_profile(self, profile_name, language):
+        """
+
+        :param profileName:
+        :return:
+        """
+
+        data = {
+            'profileName': profile_name,
+            'language': language
+        }
+
+        # Make call (return nothing)
+        self._api._make_call('post', self.DELETE_QUALITY_PROFILE_ENDPOINT, data)
+
+    def create_quality_profile(self, key, name, language, languagename,
+                               isinherited=False, isdefault=False, organization="default-organization"):
+        """
+        Create a quality profile
+
+        :param key:
+        :param name: name of the profile
+        :param language: language used (java, C#...)
+        :param languagename: language name (may be different from the language)
+        :param isinherited: profile inherited
+        :param isdefault: default rules
+        :param organization:
+        :return: request response
+        """
+
+        data = {
+            'key': key,
+            'name': name,
+            'language': language,
+            'languageName': languagename,
+            'isInherited': isinherited,
+            'isDefault': isdefault,
+            'organization': organization
+        }
+
+        # Make call (might raise exception) and return
+        res = self._api._make_call('post', self.CREATE_QUALITY_PROFILE_ENDPOINT, data=data)
+        return res if res.status_code == 204 else json.loads(res.content)
+
+    def add_project_to_quality_profile(self, profile_key, project_key):
+        """
+        Adds the project to the quality profile
+
+        :param profile_key: key of the profile
+        :param project_key: key of the project
+        :return: request response
+        """
+
+        data = {
+            'profileKey': profile_key,
+            'projectKey': project_key
+        }
+
+        # Make call (might raise exception) and return no content
+        self._api._make_call('post', self.ADD_PROJECT_TO_QUALITY_PROFILE_ENDPOINT, data=data)
+
+    def activate_rule(self, key, profile_key, reset=False, severity=None,
+                      **params):
+        """
+        Activate a rule for a given quality profile.
+
+        :param key: key of the rule
+        :param profile_key: key of the profile
+        :param reset: reset severity and params to default
+        :param severity: severity of rule for given profile
+        :param params: customized parameters for the rule
+        :return: request response
+        """
+        # Build main data to post
+        data = {
+            'rule_key': key,
+            'profile_key': profile_key,
+            'reset': reset and 'true' or 'false'
+        }
+
+        if not reset:
+            # No reset, Add severity if given (if not default will be used?)
+            if severity:
+                data['severity'] = severity.upper()
+
+            # Add params if we have any
+            # Note: sort by key to allow checking easily
+            params = ';'.join('{}={}'.format(k, v) for k, v in sorted(params.items()) if v)
+            if params:
+                data['params'] = params
+
+        # Make call (might raise exception) and return
+        res = self._api._make_call('post', self.RULES_ACTIVATION_ENDPOINT, data=data)
+        return res if res.status_code == 204 else json.loads(res.content)
```

### Comparing `opn_sonarqube_api-2.1.0.486996/sonarqube_api/cmd/export_rules.py` & `opn_sonarqube_api-2.3.2.2950747/sonarqube_api/cmd/export_rules.py`

 * *Files identical despite different names*

### Comparing `opn_sonarqube_api-2.1.0.486996/sonarqube_api/cmd/migrate_rules.py` & `opn_sonarqube_api-2.3.2.2950747/sonarqube_api/cmd/migrate_rules.py`

 * *Files identical despite different names*

### Comparing `opn_sonarqube_api-2.1.0.486996/sonarqube_api/cmd/activate_rules.py` & `opn_sonarqube_api-2.3.2.2950747/sonarqube_api/cmd/activate_rules.py`

 * *Files identical despite different names*

### Comparing `opn_sonarqube_api-2.1.0.486996/sonarqube_api/api.py` & `opn_sonarqube_api-2.3.2.2950747/sonarqube_api/api.py`

 * *Files 22% similar despite different names*

```diff
@@ -81,7 +81,33 @@
         elif res.status_code < 500:
             # Other 4xx, generic client error
             raise ClientError(res.reason)
 
         else:
             # 5xx is server error
             raise ServerError(res.reason)
+
+    def _get_call(self, endpoint, params):
+        """
+        Specifically make the get call to the service, queryset and data,
+        using the initial session.
+
+        :param endpoint: relative url to make the call
+        :param params: queryset or body
+        :return: response
+        """
+        url = self.get_url(endpoint)
+        combined=url+params
+
+        res = requests.get(combined, auth=self._session.auth)
+
+        if res.status_code < 300:
+            return res
+        elif res.status_code == 400:
+            msg = ', '.join(e['msg'] for e in res.json()['errors'])
+            raise ValidationError(msg)
+        elif res.status_code in (401, 403):
+            raise AuthError(res.reason)
+        elif res.status_code < 500:
+            raise ClientError(res.reason)
+        else:
+            raise ServerError(res.reason)
```

### Comparing `opn_sonarqube_api-2.1.0.486996/PKG-INFO` & `opn_sonarqube_api-2.3.2.2950747/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 1.1
 Name: opn_sonarqube_api
-Version: 2.1.0.486996
+Version: 2.3.2.2950747
 Summary: Open SonarQube API Handler
 Home-page: UNKNOWN
 Author: open sas
-Author-email: sebastien.bettinger@open-groupe.com
+Author-email: boost-support@open-groupe.com
 License: MIT
 Description: ====================
         Python SonarQube API
         ====================
         
         .. image:: https://img.shields.io/github/license/kako-nawao/python-sonarqube-api.svg
             :target: http://www.opensource.org/licenses/MIT
```

### Comparing `opn_sonarqube_api-2.1.0.486996/README.rst` & `opn_sonarqube_api-2.3.2.2950747/README.rst`

 * *Files identical despite different names*

### Comparing `opn_sonarqube_api-2.1.0.486996/tests/test_api.py` & `opn_sonarqube_api-2.3.2.2950747/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `opn_sonarqube_api-2.1.0.486996/setup.py` & `opn_sonarqube_api-2.3.2.2950747/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,20 +16,20 @@
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='opn_sonarqube_api',
 
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='2.1.0.486996',
+    version='2.3.2.2950747',
 
     description='Open SonarQube API Handler',
     long_description=long_description,
     author='open sas',
-    author_email='sebastien.bettinger@open-groupe.com',
+    author_email='boost-support@open-groupe.com',
     license='MIT',
 
     # See https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Environment :: Plugins',
         'Intended Audience :: Developers',
```

### Comparing `opn_sonarqube_api-2.1.0.486996/opn_sonarqube_api.egg-info/PKG-INFO` & `opn_sonarqube_api-2.3.2.2950747/opn_sonarqube_api.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 1.1
 Name: opn-sonarqube-api
-Version: 2.1.0.486996
+Version: 2.3.2.2950747
 Summary: Open SonarQube API Handler
 Home-page: UNKNOWN
 Author: open sas
-Author-email: sebastien.bettinger@open-groupe.com
+Author-email: boost-support@open-groupe.com
 License: MIT
 Description: ====================
         Python SonarQube API
         ====================
         
         .. image:: https://img.shields.io/github/license/kako-nawao/python-sonarqube-api.svg
             :target: http://www.opensource.org/licenses/MIT
```

### Comparing `opn_sonarqube_api-2.1.0.486996/opn_sonarqube_api.egg-info/SOURCES.txt` & `opn_sonarqube_api-2.3.2.2950747/opn_sonarqube_api.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -15,18 +15,20 @@
 sonarqube_api/utils.py
 sonarqube_api/cmd/__init__.py
 sonarqube_api/cmd/activate_rules.py
 sonarqube_api/cmd/export_rules.py
 sonarqube_api/cmd/migrate_rules.py
 sonarqube_api/sonarapi/__init__.py
 sonarqube_api/sonarapi/authentication.py
+sonarqube_api/sonarapi/branches.py
 sonarqube_api/sonarapi/components.py
 sonarqube_api/sonarapi/groups.py
 sonarqube_api/sonarapi/metrics.py
 sonarqube_api/sonarapi/permissions.py
+sonarqube_api/sonarapi/projects.py
 sonarqube_api/sonarapi/qualitygates.py
 sonarqube_api/sonarapi/qualityprofiles.py
 sonarqube_api/sonarapi/resources.py
 sonarqube_api/sonarapi/rules.py
 sonarqube_api/sonarapi/settings.py
 sonarqube_api/sonarapi/user_token.py
 sonarqube_api/sonarapi/users.py
```

