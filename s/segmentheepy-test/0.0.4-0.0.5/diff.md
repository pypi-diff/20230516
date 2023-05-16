# Comparing `tmp/segmentheepy_test-0.0.4-py3-none-any.whl.zip` & `tmp/segmentheepy_test-0.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 10448 bytes, number of entries: 9
--rw-rw-r--  2.0 unx        0 b- defN 23-Apr-26 09:11 segmenthee/__init__.py
--rw-rw-r--  2.0 unx    25660 b- defN 23-May-11 12:16 segmenthee/cart_api.py
--rw-rw-r--  2.0 unx      766 b- defN 23-Apr-26 09:11 segmenthee/config.py
--rw-rw-r--  2.0 unx     2023 b- defN 23-Apr-26 09:11 segmenthee/parser_api.py
--rw-rw-r--  2.0 unx     7932 b- defN 23-Apr-26 09:12 segmenthee/shop.py
--rw-rw-r--  2.0 unx      288 b- defN 23-May-11 12:28 segmentheepy_test-0.0.4.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-11 12:28 segmentheepy_test-0.0.4.dist-info/WHEEL
--rw-rw-r--  2.0 unx       11 b- defN 23-May-11 12:28 segmentheepy_test-0.0.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      725 b- defN 23-May-11 12:28 segmentheepy_test-0.0.4.dist-info/RECORD
-9 files, 37497 bytes uncompressed, 9194 bytes compressed:  75.5%
+Zip file size: 10627 bytes, number of entries: 9
+-rw-rw-r--  2.0 unx        0 b- defN 23-May-09 16:01 segmenthee/__init__.py
+-rw-rw-r--  2.0 unx    26963 b- defN 23-May-16 09:18 segmenthee/cart_api.py
+-rw-rw-r--  2.0 unx      766 b- defN 23-May-09 16:01 segmenthee/config.py
+-rw-rw-r--  2.0 unx     2023 b- defN 23-May-09 16:01 segmenthee/parser_api.py
+-rw-rw-r--  2.0 unx     7932 b- defN 23-May-09 16:02 segmenthee/shop.py
+-rw-rw-r--  2.0 unx      261 b- defN 23-May-16 09:29 segmentheepy_test-0.0.5.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-16 09:29 segmentheepy_test-0.0.5.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       11 b- defN 23-May-16 09:29 segmentheepy_test-0.0.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      725 b- defN 23-May-16 09:29 segmentheepy_test-0.0.5.dist-info/RECORD
+9 files, 38773 bytes uncompressed, 9373 bytes compressed:  75.8%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: segmenthee/parser_api.py
 Comment: 
 
 Filename: segmenthee/shop.py
 Comment: 
 
-Filename: segmentheepy_test-0.0.4.dist-info/METADATA
+Filename: segmentheepy_test-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: segmentheepy_test-0.0.4.dist-info/WHEEL
+Filename: segmentheepy_test-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: segmentheepy_test-0.0.4.dist-info/top_level.txt
+Filename: segmentheepy_test-0.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: segmentheepy_test-0.0.4.dist-info/RECORD
+Filename: segmentheepy_test-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## segmenthee/cart_api.py

```diff
@@ -25,28 +25,28 @@
     return retval
 
 #collect name from classindex
 classnames = dict()
 
 params = {
     "clickrate": 0.75,
-    "actionseparation": [0.5, 0.025],
-    "actionaffinity": [0.5, 0.025],
-    "categoryaffinity": [0.5, 0.025],
-    "carttotaltrend": [0.5, 0.025],
-    "cartcounttrend": [0.5, 0.025],
-    "avgpricemanipulation": [0.5, 0.025],
-    "lastpriceviewedtrend": [0.5, 0.025],
-    "tabcounttrend": [0.5, 0.025],
-    "redirectstrend": [0.5, 0.025],
-    "tabtypetrend": [0.5, 0.025],
-    "navigationtrend": [0.5, 0.025],
-    "referrertrend": [0.5, 0.025],
-    "pagetrend": [0.5, 0.025],
-    "sorttrend": [0.5, 0.025]
+    "actionseparation": [0.0, 0.25, 0.025],
+    "actionaffinity": [0.0, 0.25, 0.025],
+    "categoryaffinity": [0.0, 0.25, 0.025],
+    "carttotaltrend": [0.0, 0.25, 0.025],
+    "cartcounttrend": [0.0, 0.25, 0.025],
+    "avgpricemanipulation": [0.0, 0.25, 0.025],
+    "lastpriceviewedtrend": [0.0, 0.25, 0.025],
+    "tabcounttrend": [0.0, 0.25, 0.025],
+    "redirectstrend": [0.0, 0.25, 0.025],
+    "tabtypetrend": [0.0, 0.25, 0.025],
+    "navigationtrend": [0.0, 0.25, 0.025],
+    "referrertrend": [0.0, 0.25, 0.025],
+    "pagetrend": [0.0, 0.25, 0.025],
+    "sorttrend": [0.0, 0.25, 0.025]
 }
 
 MAX_CATEGORY = 6
 tabtype_dict = {'New':0, 'Existing':1}
 navigation_dict = {'NAVIGATE':0,'FORWARD':1,'BACK':2,'RELOAD':3}
 origin_dict = {"facebook":0,"google":1,"shop":2}
 sort_dict = {'default':0, 'name':1, 'price':2, 'order':3, 'relevance':4, 'date':5, 'rating':6, 'latest':7, 'discount':8, 'view':9}
@@ -132,45 +132,47 @@
 def UpdateAffinity(retval, coeffs, feature, update_index):
     if feature not in retval:
         return None
     values = retval[feature]
     featureattfacts = coeffs[feature]
     for attix in range(len(featureattfacts)):
         for act in range(len(values[0])):
+            retval["actiondifference"][attix][act] = (featureattfacts[attix] - 1) * values[attix][act]
             values[attix][act] *= featureattfacts[attix]
+        retval["actiondifference"][attix][update_index] += (featureattfacts[attix] - 1)
         values[attix][update_index] += 1 - featureattfacts[attix]
         
 def GetCoefficients(coeffs, params, delta_time):
     ''' exp(-lambda * delta_time) '''
     for key in params:
         if not isinstance(params[key],list):
             continue
-        coeffs[key][1] = np.exp(-params[key][1] * delta_time)
+        coeffs[key][-1] = np.exp(-params[key][-1] * delta_time)
 
-def CalculateUnalikeability(list):
-    n = len(list)
+def CalculateUnalikeability(arr):
+    n = len(arr)
     if n == 1:
         return 0 # may be better to return 1
     s = 0
     for i in range(n-1):
         for j in range(i+1,n):
-            if list[i] != list[j]:
+            if arr[i] != arr[j]:
                 s += 1
     u = 2*s/(n**2 - n)
     return u
 
-def CalculateAutocorrelation(list):
-    if len(list) == 1 or CalculateUnalikeability(list) == 0:
+def CalculateAutocorrelation(arr):
+    if len(arr) == 1 or CalculateUnalikeability(arr) == 0:
         return 0
     s = set()
-    for i in list:
+    for i in arr:
         s.add(i)
     enc = {value:idx for idx,value in enumerate(s)}
-    list = [enc[val] for val in list]    
-    autocorr = sm.tsa.acf(list, nlags = len(list)-1)[1:]
+    arr = [enc[val] for val in arr]
+    autocorr = sm.tsa.acf(arr, nlags =len(arr) - 1)[1:]
     return max(autocorr, key=abs)
 
 class SessionBodyEvent:
     def __init__(self, time: int):
         self.time = time
 
     def Update(self,prevstate):
@@ -225,18 +227,18 @@
             if retval["actioncount"] == 2: #initialize clickrates
                 UpdateClickrates(retval, self.time, params["clickrate"], initialize=True)
             else: #actioncount >= 3
                 UpdateClickrates(retval, self.time, params["clickrate"], initialize=False)
         else: #first action event
             GetCoefficients(self.coeffs, params, 0) #timeaffinity stays 0.0
             UpdateAffinity(retval, self.coeffs, "actionaffinity", self.classindex())
-            # arr = retval["actionaffinity"][0]
-            # for act in range(groupcount):
-            #     arr[act] *= params["actionaffinity"][0]
-            # arr[self.classindex()] += 1 - params["actionaffinity"][0]
+            #arr = retval["actionaffinity"][0]
+            #for act in range(classcount):
+            #    arr[act] *= params["actionaffinity"][0]
+            #arr[self.classindex()] += 1 - params["actionaffinity"][0]
         retval["lastactioneventtime"] = self.time
         if retval["highwatermark"] < 1:
             retval["highwatermark"] = 1
         return retval
 
 class CartModifyEvent(UserActionEvent):
     def __init__(self, time: int, delta_count: int, delta_total):
@@ -247,14 +249,16 @@
     cindex = nextclassindex()
     classnames[cindex] = "CartModifyEvent"
     
     def Update(self,prevstate):
         retval = super().Update(prevstate)
         retval["carttotal"] += self.delta_total
         retval["cartcount"] += self.delta_count
+        retval["cartdeltatotal"] = self.delta_total
+        retval["cartdeltacount"] = self.delta_count
         retval["sessionstatus"] = "CartModified"
         UpdateAttribute(retval, self.coeffs, "carttotaltrend", self.delta_total)
         UpdateAttribute(retval, self.coeffs, "cartcounttrend", self.delta_count)
         if self.delta_count != 0:
             avgprice = self.delta_total/self.delta_count
             retval["cartmodification"] = self.delta_total/self.delta_count
             UpdateAttribute(retval, self.coeffs, "avgpricemanipulation", avgprice)
@@ -497,20 +501,23 @@
 device_dict = {"mobile":0,"tablet":1,"desktop":2}
 os_dict = {"ms":0,"apple":1,"linux":2}
 lang_dict = {"hu":0}
 sessionstatus_dict = {"Browsing":0,"CartModified":1}
 
 def Update(prevstate,bodyevent,newparams=None):
     global params
+    if newparams:
+        for param in newparams:
+            if param in params:
+                params[param] = newparams[param]
     if prevstate["sessionstatus"] == "Bot":
         return prevstate
-    if newparams: # not None
-        for key in newparams:
-            if key in params:
-                params[key] = newparams[key]
+    #if restart:
+    #    return NewState(prevstate["admin_origin"], prevstate["admin_useragent"], prevstate["admin_lang"],
+    #                         bodyevent, newparams)
     return bodyevent.Update(prevstate)
 
 def NewState(origin_string, user_agent_string, lang_string, firstbodyevent, newparams=None):
     
     origin_cls = parser_api.parse_origin(origin_string)
     if origin_cls in origin_dict:
         origin = origin_dict[origin_cls]
@@ -523,14 +530,17 @@
     device = device_dict.get(device_cls,len(device_dict))
     os = os_dict.get(os_cls,len(os_dict))
 
     lang_cls = parser_api.parse_lang(lang_string)
     lang = lang_dict.get(lang_cls,len(lang_dict))
 
     original_state = {
+        "admin_origin": origin_string,
+        "admin_user_agent": user_agent_string,
+        "admin_region": lang_string,
         "sessionstart": firstbodyevent.time,
         "origin": origin,
         "device": device,
         "os": os,
         "lang":lang,
         "actioncount": 0,
         "lastbodyeventtime": None,
@@ -542,26 +552,30 @@
         "clickrate_squares": 0.0,
         "clickrate_var": 0.0,
         "z_score": 0.0,
         "sessionstatus": "Browsing",
         "clickrate": 0.0,
         "actionseparation": [0.0] * len(params["actionseparation"]),
         "actionaffinity": [[1/classcount] * classcount for _ in range(len(params["actionaffinity"]))],
+        "actiondifference": [[1 / classcount] * classcount for _ in range(len(params["actionaffinity"]))],
         "lastcategory": None,
         "categoryaffinity": [[1/MAX_CATEGORY] * MAX_CATEGORY for _ in range(len(params["categoryaffinity"]))],
         "carttotal":0.0,
         "cartcount":0,
+        "cartdeltatotal": 0.0,
+        "cartdeltacount": 0,
         "carttotaltrend": [0.0] * len(params["carttotaltrend"]),
         "cartcounttrend": [0.0] * len(params["cartcounttrend"]),
         "cartmodification": 0.0,
         "avgpricemanipulation": [0.0] * len(params["avgpricemanipulation"]),
         "couponstatus": 0,
         "lastprice": 0.0,
         "lastpriceviewedtrend": [0.0] * len(params["lastpriceviewedtrend"]),
         "tabcounttrend" : [0.0] * len(params["tabcounttrend"]),
+        #"tabcountdeltatrend": [0.0] * len(params["tabcounttrend"]),
         "redirectstrend" : [0.0] * len(params["redirectstrend"]),
         "tabtypetrend" : [0.0] * len(params["tabtypetrend"]),
         "navigationtrend": [0.0] * len(params["navigationtrend"]),
         "referrertrend": [0.0] * len(params["referrertrend"]),
         "sorttrend": [0.0] * len(params["sorttrend"]),
         "pagetrend": [0.0] * len(params["pagetrend"]),
         "producteverviewed": 0,
@@ -570,17 +584,19 @@
         "u_product": -1,
         "autocorr": 0
     }
 
     return Update(original_state,firstbodyevent,newparams)
 
 def RowOfState(state):
-    row ={k:state[k] for k in ["actioncount","origin","device","os","lang","carttotal","cartcount", "producteverviewed","couponstatus","clickrate_avg",
+    row ={k:state[k] for k in ["actioncount","origin","device","os","lang",
+                               "carttotal","cartcount","cartdeltatotal","cartdeltacount",
+                               "producteverviewed","couponstatus",
                                #"clickrate_squares",
-                               "clickrate_var","z_score", "u_product", "autocorr"]}                  
+                               "clickrate_avg","clickrate_var","z_score", "u_product", "autocorr"]}                  
     row["sessionage"] = state["lastbodyeventtime"] - state["sessionstart"]
     lastbodyeventtime = datetime.datetime.fromtimestamp(state["lastbodyeventtime"])
     row["hourofday"] = lastbodyeventtime.hour
     row["dayofweek"] = lastbodyeventtime.weekday()
     row["dayofmonth"] = lastbodyeventtime.day
     row["cartaverageprice"] = state["carttotal"]/state["cartcount"] if state["cartcount"] != 0 else 0.0
     # row["highwatermark"] = state["highwatermark"]
@@ -590,14 +606,19 @@
         row["actionseparation_" + str(i)] = arr[i]
 
     arr = state["actionaffinity"]
     for i in range(len(arr)):
         for j in range(len(arr[0])):
             row["actionaffinity_" + str(i) + "_" + classnames[j]] = arr[i][j]
 
+    arr = state["actiondifference"]
+    for i in range(len(arr)):
+        for j in range(len(arr[0])):
+            row["actiondifference_" + str(i) + "_" + classnames[j]] = arr[i][j]
+
     arr = state["categoryaffinity"]
     for i in range(len(arr)):
         for j in range(len(arr[0])):
             row["categoryaffinity_" + str(i) + "_" + str(j)] = arr[i][j]
             
     arr = state["carttotaltrend"]
     for i in range(len(arr)):
@@ -615,14 +636,18 @@
     for i in range(len(arr)):
         row["lastpriceviewedtrend_" + str(i)] = arr[i]
 
     arr = state["tabcounttrend"]
     for i in range(len(arr)):
         row["tabcounttrend_" + str(i)] = arr[i]
 
+    # arr = state["tabcountdeltatrend"]
+    # for i in range(len(arr)):
+    #     row["tabcountdeltatrend_" + str(i)] = arr[i]
+
     arr = state["redirectstrend"]
     for i in range(len(arr)):
         row["redirectstrend_" + str(i)] = arr[i]
 
     arr = state["tabtypetrend"]
     for i in range(len(arr)):
         row["tabtypetrend_" + str(i)] = arr[i]
```

## Comparing `segmentheepy_test-0.0.4.dist-info/RECORD` & `segmentheepy_test-0.0.5.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 segmenthee/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-segmenthee/cart_api.py,sha256=ExPwGSJ5oy2C_OyXiEmRz72Jt6F9ZpYvBOOm2a9o7r0,25660
+segmenthee/cart_api.py,sha256=u5A4u-30q9o3LNQfCxHIpAXHDrxYYl55lKDj8vQ49_8,26963
 segmenthee/config.py,sha256=lXea6JINCK44eZP38JaQOlfgVerzFx0e9wDxObuw54c,766
 segmenthee/parser_api.py,sha256=TB-Q8roqNAV_wwYSrdJYchNoC3zTGRKI0die0sN-K-8,2023
 segmenthee/shop.py,sha256=RlKZfL1vebVw6JOxUthPfzgzkcU7MaAYE96Wc4EYDJQ,7932
-segmentheepy_test-0.0.4.dist-info/METADATA,sha256=NhMAS2iF_jTov3JZLu4KjF2raOWe0Emuk7k5TuzeGOw,288
-segmentheepy_test-0.0.4.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-segmentheepy_test-0.0.4.dist-info/top_level.txt,sha256=ESnfgSm7LAnmWZiJ4HDmTbd5B0AemZ20M9sFA5X59IU,11
-segmentheepy_test-0.0.4.dist-info/RECORD,,
+segmentheepy_test-0.0.5.dist-info/METADATA,sha256=Ynhs5_g3V8hMWDGN6c_bZUBEMTDZXVO5pom1UY5J8_o,261
+segmentheepy_test-0.0.5.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+segmentheepy_test-0.0.5.dist-info/top_level.txt,sha256=ESnfgSm7LAnmWZiJ4HDmTbd5B0AemZ20M9sFA5X59IU,11
+segmentheepy_test-0.0.5.dist-info/RECORD,,
```

