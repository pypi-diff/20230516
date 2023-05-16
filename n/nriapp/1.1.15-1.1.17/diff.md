# Comparing `tmp/nriapp-1.1.15.tar.gz` & `tmp/nriapp-1.1.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nriapp-1.1.15.tar", last modified: Sat May  6 05:26:31 2023, max compression
+gzip compressed data, was "nriapp-1.1.17.tar", last modified: Tue May 16 13:40:04 2023, max compression
```

## Comparing `nriapp-1.1.15.tar` & `nriapp-1.1.17.tar`

### file list

```diff
@@ -1,38 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 05:26:31.263397 nriapp-1.1.15/
--rw-rw-rw-   0        0        0     1084 2023-02-12 09:09:41.000000 nriapp-1.1.15/LICENSE
--rw-rw-rw-   0        0        0       57 2023-03-02 17:29:56.000000 nriapp-1.1.15/MANIFEST.in
--rw-rw-rw-   0        0        0      273 2023-05-06 05:26:31.263397 nriapp-1.1.15/PKG-INFO
--rw-rw-rw-   0        0        0        7 2023-02-12 09:19:02.000000 nriapp-1.1.15/README
--rw-rw-rw-   0        0        0      344 2023-05-06 05:25:35.000000 nriapp-1.1.15/requirements.txt
--rw-rw-rw-   0        0        0       86 2023-05-06 05:26:31.263397 nriapp-1.1.15/setup.cfg
--rw-rw-rw-   0        0        0     1108 2023-05-06 05:25:51.000000 nriapp-1.1.15/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-06 05:26:31.122997 nriapp-1.1.15/src/
-drwxrwxrwx   0        0        0        0 2023-05-06 05:26:31.185397 nriapp-1.1.15/src/nriapp/
--rw-rw-rw-   0        0        0        2 2023-04-19 13:47:32.000000 nriapp-1.1.15/src/nriapp/__init__.py
--rw-rw-rw-   0        0        0     3672 2023-02-02 00:29:38.000000 nriapp-1.1.15/src/nriapp/changelog.txt
-drwxrwxrwx   0        0        0        0 2023-05-06 05:26:31.200997 nriapp-1.1.15/src/nriapp/config/
--rw-rw-rw-   0        0        0        2 2023-03-02 07:59:35.000000 nriapp-1.1.15/src/nriapp/config/__init__.py
--rw-rw-rw-   0        0        0       55 2023-03-02 07:59:35.000000 nriapp-1.1.15/src/nriapp/config/config.py
-drwxrwxrwx   0        0        0        0 2023-05-06 05:26:31.232197 nriapp-1.1.15/src/nriapp/core/
--rw-rw-rw-   0        0        0        0 2023-04-19 13:47:32.000000 nriapp-1.1.15/src/nriapp/core/__init__.py
--rw-rw-rw-   0        0        0     1520 2023-04-19 13:47:32.000000 nriapp-1.1.15/src/nriapp/core/abuseipdbapi.py
--rw-rw-rw-   0        0        0    17188 2023-05-05 05:36:38.000000 nriapp-1.1.15/src/nriapp/core/dataexplorer.py
--rw-rw-rw-   0        0        0    30935 2023-05-02 03:08:50.000000 nriapp-1.1.15/src/nriapp/core/msgraphapi.py
--rw-rw-rw-   0        0        0   101629 2023-04-30 17:20:44.000000 nriapp-1.1.15/src/nriapp/core/mssentinelapi.py
--rw-rw-rw-   0        0        0     6076 2023-04-19 13:47:32.000000 nriapp-1.1.15/src/nriapp/core/multifactor.py
--rw-rw-rw-   0        0        0      640 2023-04-19 13:47:32.000000 nriapp-1.1.15/src/nriapp/core/vtquery.py
-drwxrwxrwx   0        0        0        0 2023-05-06 05:26:31.263397 nriapp-1.1.15/src/nriapp/helper/
--rw-rw-rw-   0        0        0        2 2023-04-19 13:47:32.000000 nriapp-1.1.15/src/nriapp/helper/__init__.py
--rw-rw-rw-   0        0        0     5696 2023-04-19 13:47:32.000000 nriapp-1.1.15/src/nriapp/helper/doc.py
--rw-rw-rw-   0        0        0      246 2023-04-19 13:47:32.000000 nriapp-1.1.15/src/nriapp/helper/excel.py
--rw-rw-rw-   0        0        0     8397 2023-04-29 03:04:07.000000 nriapp-1.1.15/src/nriapp/helper/login.py
--rw-rw-rw-   0        0        0     2443 2023-04-19 13:47:32.000000 nriapp-1.1.15/src/nriapp/helper/pylog.py
--rw-rw-rw-   0        0        0     1247 2023-04-19 13:47:32.000000 nriapp-1.1.15/src/nriapp/helper/requestheader.py
--rw-rw-rw-   0        0        0       92 2023-04-19 13:47:32.000000 nriapp-1.1.15/src/nriapp/helper/visualization.py
-drwxrwxrwx   0        0        0        0 2023-05-06 05:26:31.169797 nriapp-1.1.15/src/nriapp/nriapp.egg-info/
--rw-rw-rw-   0        0        0      273 2023-05-06 05:26:30.000000 nriapp-1.1.15/src/nriapp/nriapp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1024 2023-05-06 05:26:30.000000 nriapp-1.1.15/src/nriapp/nriapp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 05:26:30.000000 nriapp-1.1.15/src/nriapp/nriapp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-05-06 05:26:30.000000 nriapp-1.1.15/src/nriapp/nriapp.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       20 2023-05-06 05:26:30.000000 nriapp-1.1.15/src/nriapp/nriapp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    36761 2023-04-29 10:16:03.000000 nriapp-1.1.15/src/nriapp/nriapp.py
+drwxrwxrwx   0        0        0        0 2023-05-16 13:40:04.289182 nriapp-1.1.17/
+-rw-rw-rw-   0        0        0     1084 2023-02-12 09:09:41.000000 nriapp-1.1.17/LICENSE
+-rw-rw-rw-   0        0        0       57 2023-03-02 17:29:56.000000 nriapp-1.1.17/MANIFEST.in
+-rw-rw-rw-   0        0        0      273 2023-05-16 13:40:04.289182 nriapp-1.1.17/PKG-INFO
+-rw-rw-rw-   0        0        0        7 2023-02-12 09:19:02.000000 nriapp-1.1.17/README
+-rw-rw-rw-   0        0        0      344 2023-05-06 05:28:38.000000 nriapp-1.1.17/requirements.txt
+-rw-rw-rw-   0        0        0       86 2023-05-16 13:40:04.304782 nriapp-1.1.17/setup.cfg
+-rw-rw-rw-   0        0        0     1108 2023-05-16 13:39:55.000000 nriapp-1.1.17/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 13:40:04.242382 nriapp-1.1.17/src/
+drwxrwxrwx   0        0        0        0 2023-05-16 13:40:04.273582 nriapp-1.1.17/src/nriapp/
+-rw-rw-rw-   0        0        0        2 2023-04-19 13:47:32.000000 nriapp-1.1.17/src/nriapp/__init__.py
+-rw-rw-rw-   0        0        0     3672 2023-02-02 00:29:38.000000 nriapp-1.1.17/src/nriapp/changelog.txt
+drwxrwxrwx   0        0        0        0 2023-05-16 13:40:04.273582 nriapp-1.1.17/src/nriapp/config/
+-rw-rw-rw-   0        0        0        2 2023-03-02 07:59:35.000000 nriapp-1.1.17/src/nriapp/config/__init__.py
+-rw-rw-rw-   0        0        0       55 2023-03-02 07:59:35.000000 nriapp-1.1.17/src/nriapp/config/config.py
+drwxrwxrwx   0        0        0        0 2023-05-16 13:40:04.289182 nriapp-1.1.17/src/nriapp/core/
+-rw-rw-rw-   0        0        0        0 2023-04-19 13:47:32.000000 nriapp-1.1.17/src/nriapp/core/__init__.py
+-rw-rw-rw-   0        0        0     1520 2023-04-19 13:47:32.000000 nriapp-1.1.17/src/nriapp/core/abuseipdbapi.py
+-rw-rw-rw-   0        0        0    20524 2023-05-16 04:22:17.000000 nriapp-1.1.17/src/nriapp/core/dataexplorer.py
+-rw-rw-rw-   0        0        0    30935 2023-05-02 03:08:50.000000 nriapp-1.1.17/src/nriapp/core/msgraphapi.py
+-rw-rw-rw-   0        0        0   104956 2023-05-16 05:49:17.000000 nriapp-1.1.17/src/nriapp/core/mssentinelapi.py
+-rw-rw-rw-   0        0        0     6076 2023-04-19 13:47:32.000000 nriapp-1.1.17/src/nriapp/core/multifactor.py
+-rw-rw-rw-   0        0        0      640 2023-04-19 13:47:32.000000 nriapp-1.1.17/src/nriapp/core/vtquery.py
+drwxrwxrwx   0        0        0        0 2023-05-16 13:40:04.289182 nriapp-1.1.17/src/nriapp/helper/
+-rw-rw-rw-   0        0        0        2 2023-04-19 13:47:32.000000 nriapp-1.1.17/src/nriapp/helper/__init__.py
+-rw-rw-rw-   0        0        0     5696 2023-04-19 13:47:32.000000 nriapp-1.1.17/src/nriapp/helper/doc.py
+-rw-rw-rw-   0        0        0      246 2023-04-19 13:47:32.000000 nriapp-1.1.17/src/nriapp/helper/excel.py
+-rw-rw-rw-   0        0        0     8397 2023-04-29 03:04:07.000000 nriapp-1.1.17/src/nriapp/helper/login.py
+-rw-rw-rw-   0        0        0     2443 2023-04-19 13:47:32.000000 nriapp-1.1.17/src/nriapp/helper/pylog.py
+-rw-rw-rw-   0        0        0     1247 2023-04-19 13:47:32.000000 nriapp-1.1.17/src/nriapp/helper/requestheader.py
+drwxrwxrwx   0        0        0        0 2023-05-16 13:40:04.257982 nriapp-1.1.17/src/nriapp/nriapp.egg-info/
+-rw-rw-rw-   0        0        0      273 2023-05-16 13:40:03.000000 nriapp-1.1.17/src/nriapp/nriapp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      820 2023-05-16 13:40:04.000000 nriapp-1.1.17/src/nriapp/nriapp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 13:40:03.000000 nriapp-1.1.17/src/nriapp/nriapp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-05-16 13:40:03.000000 nriapp-1.1.17/src/nriapp/nriapp.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       20 2023-05-16 13:40:03.000000 nriapp-1.1.17/src/nriapp/nriapp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    38172 2023-05-16 13:34:30.000000 nriapp-1.1.17/src/nriapp/nriapp.py
```

### Comparing `nriapp-1.1.15/LICENSE` & `nriapp-1.1.17/LICENSE`

 * *Files identical despite different names*

### Comparing `nriapp-1.1.15/setup.py` & `nriapp-1.1.17/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 #with open('requirements.txt') as f:
 #    requirements = f.read().splitlines()
 
 
 setup(
    name='nriapp',
-   version='1.1.15',
+   version='1.1.17',
    description='This is an internal tool for crawling MS 365 Defender web with NRI',
     license='MIT',
    author='Llallum Victoria',
    author_email='llallumvictoria@gmail.com',
 #   packages=find_packages('src'),
    package_dir = {'':'src/nriapp'},
```

### Comparing `nriapp-1.1.15/src/nriapp/changelog.txt` & `nriapp-1.1.17/src/nriapp/changelog.txt`

 * *Files identical despite different names*

### Comparing `nriapp-1.1.15/src/nriapp/core/abuseipdbapi.py` & `nriapp-1.1.17/src/nriapp/core/abuseipdbapi.py`

 * *Files identical despite different names*

### Comparing `nriapp-1.1.15/src/nriapp/core/dataexplorer.py` & `nriapp-1.1.17/src/nriapp/core/dataexplorer.py`

 * *Files 8% similar despite different names*

```diff
@@ -105,15 +105,15 @@
         with open(path, "w") as file:
             for item in data:
                 file.write(json.dumps(item) + "\n")
         if data:
             ingestion_props = IngestionProperties(database=database,table=table,data_format=DataFormat.MULTIJSON, ingestion_mapping_reference="RawEventMapping")
             self.client_ingest.ingest_from_file(path, ingestion_properties=ingestion_props)
         os.remove(path)
-        return data
+        return [i["IncidentId"] for i in data]
 
     def check_ingest_mfastats_tag(self, database="Incidents", table="Authentication"):
         tag = date.today().strftime("%Y-%m-%d")
         
         current_tags = ''' Authentication
         | extend tags = tostring(extent_tags())
         | distinct tags
@@ -249,14 +249,31 @@
             for item in data:
                 file.write(json.dumps(item) + "\n")
         if data:
             ingestion_props = IngestionProperties(database=database,table=table,data_format=DataFormat.MULTIJSON, ingestion_mapping_reference="ManagedDevicesMapping", ingest_if_not_exists=[tag],ingest_by_tags=[tag], drop_by_tags=[tag]) 
             self.client_ingest.ingest_from_file(path, ingestion_properties=ingestion_props)
         os.remove(path)
 
+    def check_defender_agents_tag(self, database="Incidents", table="DefenderAgents"):
+        tag = date.today().strftime("%Y-%m-%d")
+        current_tags = '''
+        DefenderAgents
+        | extend tags = tostring(extent_tags())
+        | distinct tags
+        | extend item = parse_json(tags)
+        | mv-expand tag = item
+        | project trim_start("ingest-by:", tostring(tag))
+        '''
+        response = self.client_query.execute(database, current_tags)        
+        tags = [i[0] for i in response.primary_results[0].raw_rows]
+        for i in tags:
+
+            if tag == i:
+                return True
+        return False
 
     def ingest_defender_agents(self, path, database="Incidents", table="DefenderAgents"):
         tag = date.today().strftime("%Y-%m-%d")
 
         ingestion_props =  IngestionProperties(database=database,table=table,data_format=DataFormat.CSV, ingestion_mapping_reference="DefenderAgents_mapping", additional_properties={'ignoreFirstRecord': 'true'},  ingest_if_not_exists=[tag],ingest_by_tags=[tag], drop_by_tags=[tag]) 
         result = self.client_ingest.ingest_from_file(path, ingestion_properties=ingestion_props)
         os.remove(path)
@@ -289,15 +306,15 @@
         if data:
             ingestion_props = IngestionProperties(database=database,table=table,data_format=DataFormat.MULTIJSON, ingestion_mapping_reference="SignInLogsMapping") 
             self.client_ingest.ingest_from_file(path, ingestion_properties=ingestion_props)
         os.remove(path)
 
     def get_latest_av_engines(self):
 
-        defender_updates = "https://www.microsoft.com/en-us/wdsi/defenderupdates"
+        defender_updates = "https://www.microsoft.com/en-us/wdsi/defenderupdates/"
         
         response = requests.get(defender_updates, headers={"User-Agent" : "PostmanRuntime/7.32.2"})
         soup = BeautifulSoup(response.content, 'html.parser')
 
         ul_tag = soup.find("ul", {"class" : "c-list list-bottom-margin"})
         version_info = {}
         for i in ul_tag.find_all("li"):
@@ -369,7 +386,71 @@
                 file.write(json.dumps(item) + "\n")
         if data:
             ingestion_props = IngestionProperties(database=database,table=table,data_format=DataFormat.MULTIJSON, ingestion_mapping_reference="CompliancePolicyMapping")
             self.client_ingest.ingest_from_file(path, ingestion_properties=ingestion_props)
         os.remove(path)    
 
 
+    def ingest_device_inventory(self, data, database="Incidents", table="DeviceInventory"):
+        tag = date.today().strftime("%Y-%m-%d")
+
+        path = os.path.join(desktop, "devices_inventory.tmp")
+        with open(path, "w") as file:
+            for item in data:
+                file.write(json.dumps(item) + "\n")
+        if data:
+            ingestion_props = IngestionProperties(database=database,table=table,data_format=DataFormat.MULTIJSON, ingestion_mapping_reference="DeviceInventoryMapping", ingest_if_not_exists=[tag],ingest_by_tags=[tag], drop_by_tags=[tag])
+            self.client_ingest.ingest_from_file(path, ingestion_properties=ingestion_props)
+        os.remove(path)
+
+    def check_device_inventory_tag(self, database="Incidents", table="DeviceInventory"):
+        tag = date.today().strftime("%Y-%m-%d")
+
+        current_tags = '''
+        DeviceInventory
+        | extend tags = tostring(extent_tags())
+        | distinct tags
+        | extend item = parse_json(tags)
+        | mv-expand tag = item
+        | project trim_start("ingest-by:", tostring(tag))
+        '''
+        response = self.client_query.execute(database, current_tags)        
+        tags = [i[0] for i in response.primary_results[0].raw_rows]
+        for i in tags:
+            if tag == i:
+                return True
+        return False
+
+
+    def check_raw_audit_list(self, database="Incidents", table="RawAuditHistory"):
+        latest_id = '''
+        RawAuditHistory
+        | extend Items = parse_json(Items)
+        | project id=toint(Items.auditId)
+        '''
+        response = self.client_query.execute(database, latest_id)        
+#        audit_id = response.primary_results[0].raw_rows[0]
+        audit_id = [i[0] for i in response.primary_results[0].raw_rows]
+
+        if audit_id:
+            return audit_id
+        else:
+            return
+
+    def ingest_raw_audit_history(self, data, database="Incidents", table="RawAuditHistory"):
+
+        audit_id = self.check_raw_audit_list()
+
+        for i in data[:]:
+            if i["auditId"] in audit_id:
+                data.remove(i)
+
+        path = os.path.join(desktop, "raw_audit_history.tmp")
+        with open(path, "w") as file:
+            for item in data:
+                file.write(json.dumps(item) + "\n")
+        if data:
+            ingestion_props = IngestionProperties(database=database,table=table,data_format=DataFormat.MULTIJSON, ingestion_mapping_reference="RawAuditHistoryMapping")
+            self.client_ingest.ingest_from_file(path, ingestion_properties=ingestion_props)
+        os.remove(path)
+
+
```

### Comparing `nriapp-1.1.15/src/nriapp/core/msgraphapi.py` & `nriapp-1.1.17/src/nriapp/core/msgraphapi.py`

 * *Files identical despite different names*

### Comparing `nriapp-1.1.15/src/nriapp/core/mssentinelapi.py` & `nriapp-1.1.17/src/nriapp/core/mssentinelapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,16 @@
             try:
                 if params:
                     dbgPrint.info("Sending GET request")
                     response = self._session.get(arg, headers=headers, params=params, verify=False)
                     if response.status_code == 440:
                         login.Login().delete_session()
                         login.Login(self.email).login()
-                        self.load_session()
+#                       self.load_session()
+                        break
                     elif response.status_code == 200:
                         break
                     elif response.status_code == 500:
                         message = json.loads(response.text)
                         dbgPrint.error(message["Message"])
                         sys.exit()
                     elif response.status_code == 504:
@@ -139,26 +140,21 @@
             if response.status_code == 440:
                 self.load_session()
                 response = self.tryrequest(incident_alerts, json=json_data)
 
         incident_list.extend(json.loads(response.text))
 
         if len(json.loads(response.text)) == pageSize:
-            items = self.get_incidents(incidentId,pageIndex=pageIndex+1,lookBackInDays = 180, pageSize = 3000)
-            return items
+            self.get_incidents(incidentId,pageIndex=pageIndex+1,lookBackInDays = 180, pageSize = 3000, incident_list=incident_list)
         else:
-            if incidentId:
-                temp = []
-                for a in incidentId:
-                    incident = [i for i in incident_list if i["IncidentId"] == a]
-                    if incident:
-                        temp.append(incident[0])
-                return temp
-            else:                      
-                return incident_list
+            incident_list.extend(json.loads(response.text))
+
+        return incident_list
+
+
 
     def search_incident(self, query, pageSize=3):
         incident_search = 'https://security.microsoft.com/apiproxy/mtp/incidentSearch'
 
         params = {
             'term': query,
             'pageSize': pageSize
@@ -1749,21 +1745,99 @@
         
         # Determination - 0 - 69 True Positive
         # Classification - 0 - 20 Others
         # Feedback 
 
         return audit
 
-    def get_all_audit_logs(self, incidents):
+    def get_audit_history_raw(self, incidentId):    
+
+        classifications = {
+            20 : "True Positive",
+            10 : "False Positive",
+            30 : "Informational, Expected Activity",
+            0  : "Not set"
+            }
+
+        determinations = {
+            140 : "Line of Business Application", 
+            130 : "Confirmed Activity",
+            120 : "Not Enough Data to Validata",
+            110 : "Not Malicious",
+            100 : "Malicious User Activity",
+            90  : "Phishing",
+            80  : "Compromised Account",
+            70  : "Multi Stage Attack",
+            60  : "Other",
+            50  : "Unwanted Software",
+            40  : "Security Testing",
+            20  : "Malware",
+            0   : "Not set"
+            }
 
-        id = [i["IncidentId"] for i in incidents]
+        audit_history = "https://security.microsoft.com/apiproxy/mtp/auditHistory/AuditHistory"
 
+        params = {
+            'entityType' : 'IncidentEntity',
+            'id'         : incidentId,
+            'pageIndex'  : 1,
+            'pageSize'   : 100
+            }
+        response = self.tryrequest(audit_history, params=params)
+        while(response.status_code !=200):
+            if response.status_code == 440:
+                self.load_session()
+                response = self.tryrequest(audit_history, params=params)
+
+        sorted_list = sorted(json.loads(response.text), key=lambda x: x["auditId"])
+        return sorted_list
+
+    def get_all_audit_logs_raw(self, lookBackInDays=30, new_list=[]):
+        
+        incident_list = []
+
+        self.get_incidents(lookBackInDays=lookBackInDays, incident_list=incident_list)
+
+#        utc_now = datetime.utcnow().replace(tzinfo=pytz.UTC)
+
+#        t_lower = datetime.strptime(min, "%Y-%m-%dT%H:%M:%SZ")
+#        t_lower = t_lower.replace(minute=0, second=0, microsecond=0)
+
+#        for i in incident_list[:]:
+#            if (utc_now - parser.parse(i["FirstEventTime"])).days > 30:
+#                incident_list.remove(i)
+#        active = incident_list[:]
+
+#        for i in incident_list[:]:
+#            if i["Status"] != 2:
+#                incident_list.remove(i)
+
+#        incident_list.extend(new_list)
+#        incident_list = list(set(incident_list))
+
+        id_list = [i["IncidentId"] for i in incident_list]       # Active and In-progress tickets
+        id_list.extend(new_list)                                 # Updated tickets that were ingested previously
+        id_list = list(set(id_list))
+
+        start = time.time()
+        audit_history_raw = []
+        for i in id_list:
+            audit = self.get_audit_history_raw(i)
+            audit_history_raw.extend(audit)
+            dbgPrint.info(i)
+
+        end = time.time()
+        dbgPrint.success("Job done (Elapsed time {value}).", value=end-start)  
+        return audit_history_raw
+
+    def get_all_audit_logs(self, incidents):
+   
         audit_history = []
         
-        for i in id:
+        for i in incidents:
             audit_logs = self.get_audit_history(i)
             audit_logs["id"] = i
             audit_history.append(audit_logs)
             dbgPrint.info(len(audit_history))
         return audit_history
 
     def get_file_info(self, hash):
@@ -1782,25 +1856,45 @@
         if len(hash) != 40:
             info.update({"sha256" : hash.lower()})
         else:
             info.update({"sha1" : hash.lower()})
         
         return info
 
-    def get_device_info(self, senseMachineId):
+    def get_device_inventory(self, pageIndex=1):
 
-        machine_info = "https://security.microsoft.com/apiproxy/mtp/getMachine/machines"
+        device_totals = "https://security.microsoft.com/apiproxy/mtp/k8s/machines"
 
         params = {
-            "machineId"         : senseMachineId,
-            "idType"            : "SenseMachineId",
-            "readFromCache"     : "true",
-            "lookingBackIndays" : 180
+            "lookingBackIndays" : 30,
+            "deviceCategories"  : "IoT,Unknown,Endpoint,NetworkDevice",
+            "pageIndex" : pageIndex,
+            "pageSize" : 200,
+            "sortByField" : "riskscore",
+            "sortOrder" : "Descending"
             }
 
-        response = self.tryrequest(machine_info, params=params)
+        response = self.tryrequest(device_totals, params=params)
+        while(response.status_code != 200):
+            if response.status_code == 440:
+                self.load_session()
+                response = self.tryrequest(device_totals, params=params)
 
         info = json.loads(response.text)
 
         return info
         
+    def get_all_device_inventory(self):
+
+        device_inventory = []
+        pageIndex=1
+        result = self.get_device_inventory(pageIndex)
+
+        while(len(result)==200):
+            device_inventory.extend(result)
+            dbgPrint.info(len(device_inventory))
+            pageIndex=pageIndex+1
+            result = self.get_device_inventory(pageIndex)
+
+        device_inventory.extend(result)
 
+        return device_inventory
```

### Comparing `nriapp-1.1.15/src/nriapp/core/multifactor.py` & `nriapp-1.1.17/src/nriapp/core/multifactor.py`

 * *Files identical despite different names*

### Comparing `nriapp-1.1.15/src/nriapp/core/vtquery.py` & `nriapp-1.1.17/src/nriapp/core/vtquery.py`

 * *Files identical despite different names*

### Comparing `nriapp-1.1.15/src/nriapp/helper/doc.py` & `nriapp-1.1.17/src/nriapp/helper/doc.py`

 * *Files identical despite different names*

### Comparing `nriapp-1.1.15/src/nriapp/helper/login.py` & `nriapp-1.1.17/src/nriapp/helper/login.py`

 * *Files identical despite different names*

### Comparing `nriapp-1.1.15/src/nriapp/helper/pylog.py` & `nriapp-1.1.17/src/nriapp/helper/pylog.py`

 * *Files identical despite different names*

### Comparing `nriapp-1.1.15/src/nriapp/helper/requestheader.py` & `nriapp-1.1.17/src/nriapp/helper/requestheader.py`

 * *Files identical despite different names*

### Comparing `nriapp-1.1.15/src/nriapp/nriapp.egg-info/SOURCES.txt` & `nriapp-1.1.17/src/nriapp/nriapp.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -23,13 +23,8 @@
 src/nriapp/core/vtquery.py
 src/nriapp/helper/__init__.py
 src/nriapp/helper/doc.py
 src/nriapp/helper/excel.py
 src/nriapp/helper/login.py
 src/nriapp/helper/pylog.py
 src/nriapp/helper/requestheader.py
-src/nriapp/helper/visualization.py
-src/nriapp/nriapp.egg-info/PKG-INFO
-src/nriapp/nriapp.egg-info/SOURCES.txt
-src/nriapp/nriapp.egg-info/dependency_links.txt
-src/nriapp/nriapp.egg-info/entry_points.txt
-src/nriapp/nriapp.egg-info/top_level.txt
+src/nriapp/nriapp.egg-info/SOURCES.txt
```

### Comparing `nriapp-1.1.15/src/nriapp/nriapp.py` & `nriapp-1.1.17/src/nriapp/nriapp.py`

 * *Files 2% similar despite different names*

```diff
@@ -489,28 +489,66 @@
             elif impacted["mailboxes"]:
                 for a in impacted["mailboxes"]:
                     for x,y in a.items():
                         if x == "userPrincipalName":
                             if y["companyName"] not in company:
                                 company.append(y["companyName"])
 
-         
+    def get_audit_logs(self, incident_id):
+        start = time.time()
+        audit = self.sentinel.get_audit_history_raw(incident_id)
+        end = time.time()
+        dbgPrint.success("Job done (Elapsed time {value}).", value=end-start)        
+
+        dataexplorer = adx.DataIngestion()
+        dataexplorer.ingest_raw_audit_history(data=audit)
+
+
+
     def get_timely_report(self, lookBackInDays, duration=5):
         
         t_end = time.time() + 60 * duration
         dataexplorer = adx.DataIngestion()
 
         utc_timezone = pytz.UTC
 
         while time.time() < t_end:
     #        incidents_cpy = incidents[:]
+            
+#            self.get_audit_logs()
+
+            dbgPrint.debug("Fetching incidents data")
+            incidents = self.sentinel.get_incidents(incidentId=0, 
+                                                    alertStatus=['New','InProgress', 'Resolved'] , 
+                                                    severity=[256,128,64,32], 
+                                                    pageIndex=1, 
+                                                    lookBackInDays=lookBackInDays, 
+                                                    pageSize=3000, 
+                                                    ) #sourceFilter=[16384, 1048576], titleFilter=["eDiscovery"]      #16384 == MCAS incidents 512 = eDiscovery
+            dbgPrint.debug("Ingesting data")
+            audit = dataexplorer.ingest_events(data=incidents)
+            dbgPrint.debug("Fetching audit logs of incidents")
+
+            audit_logs = self.sentinel.get_all_audit_logs(audit)
+            dbgPrint.debug("Ingesting data")
+            dataexplorer.ingest_audit_logs(data=audit_logs)
+            del audit_logs[:]
+            del incidents[:]
+
+            raw_audit_logs = self.sentinel.get_all_audit_logs_raw(new_list=audit)
+            dataexplorer.ingest_raw_audit_history(data=raw_audit_logs)
+
             if dataexplorer.get_latest_compliance_ingestion_time():
                 policy = self.msgraph.get_compliance_policy()
                 dataexplorer.ingest_compliance_policy(data=policy) 
 
+            if not dataexplorer.check_device_inventory_tag():
+                device_overview = self.sentinel.get_all_device_inventory()
+                dataexplorer.ingest_device_inventory(device_overview)
+
             av_engines = dataexplorer.get_latest_av_engines()
             recent_date = dataexplorer.check_latest_av_engines()
             if not recent_date:
                 dataexplorer.ingest_latest_av_engine(data=av_engines)
 
             elif utc_timezone.localize(parser.parse(av_engines["ReleaseDateUtc"])) > parser.parse(recent_date):
                 dataexplorer.ingest_latest_av_engine(data=av_engines)
@@ -546,49 +584,27 @@
             if not dataexplorer.check_ingest_users_tag():
                 dbgPrint.debug("Fetching all users info")      
                 all_users = self.msgraph.get_all_users()
                 dbgPrint.debug("Ingesting data")  
                 dataexplorer.ingest_users(data=all_users)
                 del all_users[:]
 
-            defender_agents = self.msgraph.get_defender_agents()
-            dataexplorer.ingest_defender_agents(path=defender_agents)
-            dbgPrint.debug("Fetching incidents data")
-            incidents = self.sentinel.get_incidents(incidentId=0, 
-                                                    alertStatus=['New','InProgress', 'Resolved'] , 
-                                                    severity=[256,128,64,32], 
-                                                    pageIndex=1, 
-                                                    lookBackInDays=lookBackInDays, 
-                                                    pageSize=3000, 
-                                                    ) #sourceFilter=[16384, 1048576], titleFilter=["eDiscovery"]      #16384 == MCAS incidents 512 = eDiscovery
-            dbgPrint.debug("Ingesting data")
-            audit = dataexplorer.ingest_events(data=incidents)
-            dbgPrint.debug("Fetching audit logs of incidents")
-            audit_logs = self.sentinel.get_all_audit_logs(audit)
-            dbgPrint.debug("Ingesting data")
-            dataexplorer.ingest_audit_logs(data=audit_logs)
-            del audit_logs[:]
-            del incidents[:]
+            if not dataexplorer.check_defender_agents_tag():
+                defender_agents = self.msgraph.get_defender_agents()
+                dataexplorer.ingest_defender_agents(path=defender_agents)
+
             dbgPrint.debug("Sleeping for 3 mins")
             time.sleep(3 * 60)
 
 
 
-
-
-
 #        user_list = []
 #        mfa_users_list = self.mfa.query_all_users(mfa_list=user_list, page=1)
 #        dataexplorer.ingest_mfastats(data=mfa_users_list)
         
-
-
-
-        pass
-   
     
     def get_full_report_backend(self, incident, lookBackInDays=30, open_doc=False):
         doc = WordDoc()
         ip_list = []
         hash_list = []
         recipient = []
         q = queue.Queue()
@@ -618,22 +634,28 @@
         doc.traverse(self.sentinel.get_audit_history(incident["IncidentId"]))
         doc.save(self.output + "\\" + str(incident["IncidentId"]) + ".docx")
         if open_doc:
             os.startfile(self.output + "\\" + str(incident["IncidentId"]) + ".docx")
 
     def get_full_report(self, id=None, lookBackInDays=30, start_index=0, end_index=0):
 
-        all_data = {}
-        incidents = self.sentinel.get_incidents(incidentId=id, 
+        all_data = {}        
+        incident_list = self.sentinel.get_incidents(incidentId=id, 
                                                 alertStatus=['New','InProgress', 'Resolved'] , 
                                                 severity=[256,128,64,32], 
                                                 pageIndex=1, 
                                                 lookBackInDays=lookBackInDays, 
                                                 pageSize=3000, 
                                                 sourceFilter=[16384, 1048576], titleFilter=["eDiscovery"])       #16384 == MCAS incidents 512 = eDiscovery
+        if id:
+            incidents = []
+            for a in id:
+                incident = [i for i in incident_list if i["IncidentId"] == a]
+                if incident:
+                    incidents.append(incident[0])
 
         sorted_incidents = sorted(incidents, key=lambda x: x["IncidentId"], reverse=True)
         if sorted_incidents:
             start = sorted_incidents[0]["IncidentId"]
             end = sorted_incidents[len(sorted_incidents)-1]["IncidentId"]
         else:
             dbgPrint.error("Out of range. You may change the lockBackInDays or the incident might be aggragated to other incidents.")
@@ -668,70 +690,67 @@
             if val == 2:
                 dbgPrint.enable("core.mssentinelapi")
             elif val == 3:
                 dbgPrint.enable("core.msgraphapi")
             elif val == 4:
                 dbgPrint.enable("core.multifactor")
             elif val == 5:
-                dbgPrint.enable("helper.login")
-            elif val == 6:
                 dbgPrint.enable("core.dataexplorer")
-            elif val == 7:
+            elif val == 6:
                 dbgPrint.enable(__name__)
                 dbgPrint.enable("core.mssentinelapi")
                 dbgPrint.enable("core.msgraphapi")
                 dbgPrint.enable("helper.login")
+                dbgPrint.enable("core.dataexplorer")
             else:
-                dbgPrint.error("Unknown value")
-                sys.exit()
-        if args.get("clear"):
-            pass
-#        if args.get("resetmfa"):
-#            self.mfa.reset_session(self.email)
-        if args.get("user"):
-            self.__init__(args)
-            user_info = self.msgraph.check_mfa_status(args.get("user"))
+                dbgPrint.error("Unknown verbose level")
+                sys.exit(1)
+#        if args.get("user"):
+#            self.__init__(args)
+#            user_info = self.msgraph.check_mfa_status(args.get("user"))
 #            if user_info:
 #                printTable(user_info)
 #            user_info = self.msgraph.search_user(args.get("user"))
-        elif args.get("incidentId"):
+        if args.get("incidentId"):
             self.__init__(args)
             start = time.time()
 #            dbgPrint.info("Processing {value}", value=args.get("incidentId"))
             self.get_full_report(args.get("incidentId"), lookBackInDays=args.get("daysago") if args.get("daysago") else 30)
             end = time.time()
             dbgPrint.success("Job done (Elapsed time {value}).", value=end-start)
 #        elif args.get("all"):
 #            start = time.time()
 #            dbgPrint.info("Processing all incidents")
 #            self.get_full_report(lookBackInDays=args.get("daysago") if args.get("daysago") else 30)
 #            end = time.time()
 #            dbgPrint.success("Job done (Elapsed time {value}).", value=end-start)
+        elif args.get("audit"):
+            self.get_audit_logs(args["audit"])
         elif args.get("range"):
             start = time.time()
             dbgPrint.info("Processing Incidents with range")
             start_index = args["range"][0]
             end_index = 0
             if len(args["range"]) > 1 and len(args["range"]) < 3:
                 end_index = args["range"][1]
             if (start_index == end_index) or (start_index < end_index):
                 dbgPrint.error("The starting index must be higher than ending index")
                 sys.exit(1)
             self.get_full_report(lookBackInDays=args.get("daysago") if args.get("daysago") else 30, start_index=start_index, end_index=end_index)
             end = time.time()
             dbgPrint.success("Job done (Elapsed time {value}).", value=end-start)
         elif args.get("timely"):
-            if int(args["timely"]) >= 5:
+            if int(args["timely"]):
                 self.get_timely_report(lookBackInDays=args.get("daysago") if args.get("daysago") else 30, duration= int(args["timely"]))
         return
 
     #------------------------------------------------------
 
 def parse_argument():
-
+        
     parser = argparse.ArgumentParser(
         prog = 'ChromeDriver',
         description  = 'This tool is used to retrieve all the necessary informaation of the incident',
         epilog = '',
         formatter_class=argparse.RawTextHelpFormatter
         )
 #    group = parser.add_mutually_exclusive_group(required=True)
@@ -751,25 +770,29 @@
 #    parser.add_argument('-r', '--reset', help="Reset the session and restart", action="store_true")
     parser.add_argument('-e', '--email', help="Set email address.")
 #    parser.add_argument('-u', '--user', help = "Fetch user info")
     parser.add_argument('-o', '--output', help = "Set output folder.")
 #    parser.add_argument('-c','--clear', help = "Clear cache", action="store_true")
     parser.add_argument('-d', '--daysago', help="Look back in days. Default=30")
 
-    parser.add_argument('-rm', '--resetmfa', help="Reset MFA Session", action='store_true')
+#    parser.add_argument('-rm', '--resetmfa', help="Reset MFA Session", action='store_true')
  
     parser.add_argument('-c', '--companytags',help="CSV of company tags <Tag> <Company> <Country> to identify which country does a user belong.")
 
     parser.add_argument('-r', '--range', nargs='+', type=int, help="Specify the range in a reverse order, \n"
                                                                    "wherein the start is the higher limit and end is lower limit.\n"
                                                                    "Lower limit is optional. If not provided, the default value will be zero.\n"
                                                                    "Example: \n"
                                                                    "-r 13700 13000")
 
-    parser.add_argument('-t', '--timely', nargs='?', default=5, help="Fetching and ingesting data to Azure Data Explorer and can be use to run with specific time duration, minimum of 5 mins")
+    parser.add_argument('-t', '--timely', nargs='?', help="Fetching and ingesting data to Azure Data Explorer and can be use to run with specific time duration, minimum of 5 mins")
+
+#    parser.add_argument('-f', '--force', nargs='+', help="Force ingest the incident data by using Incident ID and will automatically update the ingested data in Azure Data Explorer")
+
+    parser.add_argument('-a', '--audit', type=int, help="For Aadit history of each incidents. The input should be incident ID. The only use case of this if the data is not be able to ingest automatically, you could use this flag.")
 
     args = parser.parse_args()
 
 #    if args.incidentId and args.all:
 #        parser.error("Required only one between -id/--incidentId and -a/--all.")
 
     if len(sys.argv)==1:
```

