# Comparing `tmp/pyreemote-12.1.0.tar.gz` & `tmp/pyreemote-12.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyreemote-12.1.0.tar", last modified: Wed Sep 21 10:52:49 2022, max compression
+gzip compressed data, was "dist/pyreemote-12.2.0.tar", last modified: Tue May 16 14:20:51 2023, max compression
```

## Comparing `pyreemote-12.1.0.tar` & `pyreemote-12.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 afita     (1000) afita     (1000)        0 2022-09-21 10:52:49.000000 pyreemote-12.1.0/
-drwxrwxr-x   0 afita     (1000) afita     (1000)        0 2022-09-21 10:52:49.000000 pyreemote-12.1.0/pyreemote/
--rw-rw-r--   0 afita     (1000) afita     (1000)    24369 2021-12-27 12:27:02.000000 pyreemote-12.1.0/pyreemote/telemeasure.py
--rw-r--r--   0 afita     (1000) afita     (1000)       56 2021-12-27 12:28:11.000000 pyreemote-12.1.0/pyreemote/__init__.py
-drwxrwxr-x   0 afita     (1000) afita     (1000)        0 2022-09-21 10:52:49.000000 pyreemote-12.1.0/pyreemote.egg-info/
--rw-r--r--   0 afita     (1000) afita     (1000)       10 2022-09-21 10:52:49.000000 pyreemote-12.1.0/pyreemote.egg-info/top_level.txt
--rw-r--r--   0 afita     (1000) afita     (1000)      219 2022-09-21 10:52:49.000000 pyreemote-12.1.0/pyreemote.egg-info/SOURCES.txt
--rw-r--r--   0 afita     (1000) afita     (1000)      274 2022-09-21 10:52:49.000000 pyreemote-12.1.0/pyreemote.egg-info/PKG-INFO
--rw-r--r--   0 afita     (1000) afita     (1000)        1 2022-09-21 10:52:49.000000 pyreemote-12.1.0/pyreemote.egg-info/dependency_links.txt
--rw-r--r--   0 afita     (1000) afita     (1000)       31 2022-09-21 10:52:49.000000 pyreemote-12.1.0/pyreemote.egg-info/requires.txt
--rw-rw-r--   0 afita     (1000) afita     (1000)      274 2022-09-21 10:52:49.000000 pyreemote-12.1.0/PKG-INFO
--rw-rw-r--   0 afita     (1000) afita     (1000)       38 2022-09-21 10:52:49.000000 pyreemote-12.1.0/setup.cfg
--rw-rw-r--   0 afita     (1000) afita     (1000)      472 2021-12-27 12:27:02.000000 pyreemote-12.1.0/setup.py
+drwxrwxr-x   0 afita     (1000) afita     (1000)        0 2023-05-16 14:20:51.000000 pyreemote-12.2.0/
+drwxrwxr-x   0 afita     (1000) afita     (1000)        0 2023-05-16 14:20:51.000000 pyreemote-12.2.0/pyreemote/
+-rw-rw-r--   0 afita     (1000) afita     (1000)    26702 2023-05-16 14:17:38.000000 pyreemote-12.2.0/pyreemote/telemeasure.py
+-rw-r--r--   0 afita     (1000) afita     (1000)       56 2023-05-16 14:18:53.000000 pyreemote-12.2.0/pyreemote/__init__.py
+drwxrwxr-x   0 afita     (1000) afita     (1000)        0 2023-05-16 14:20:51.000000 pyreemote-12.2.0/pyreemote.egg-info/
+-rw-r--r--   0 afita     (1000) afita     (1000)       10 2023-05-16 14:20:51.000000 pyreemote-12.2.0/pyreemote.egg-info/top_level.txt
+-rw-r--r--   0 afita     (1000) afita     (1000)      219 2023-05-16 14:20:51.000000 pyreemote-12.2.0/pyreemote.egg-info/SOURCES.txt
+-rw-r--r--   0 afita     (1000) afita     (1000)      274 2023-05-16 14:20:51.000000 pyreemote-12.2.0/pyreemote.egg-info/PKG-INFO
+-rw-r--r--   0 afita     (1000) afita     (1000)        1 2023-05-16 14:20:51.000000 pyreemote-12.2.0/pyreemote.egg-info/dependency_links.txt
+-rw-r--r--   0 afita     (1000) afita     (1000)       49 2023-05-16 14:20:51.000000 pyreemote-12.2.0/pyreemote.egg-info/requires.txt
+-rw-rw-r--   0 afita     (1000) afita     (1000)      274 2023-05-16 14:20:51.000000 pyreemote-12.2.0/PKG-INFO
+-rw-rw-r--   0 afita     (1000) afita     (1000)       38 2023-05-16 14:20:51.000000 pyreemote-12.2.0/setup.cfg
+-rw-rw-r--   0 afita     (1000) afita     (1000)      501 2023-05-16 14:17:38.000000 pyreemote-12.2.0/setup.py
```

### Comparing `pyreemote-12.1.0/pyreemote/telemeasure.py` & `pyreemote-12.2.0/pyreemote/telemeasure.py`

 * *Files 6% similar despite different names*

```diff
@@ -146,14 +146,78 @@
                     'Quality': channel.quality
                 }
                 record['Channels'].append(channel)
         res['Records'].append(record)
     return res
 
 
+def parse_instant_values(values, meter_serial):
+    res = {
+        "totals": parse_instant_totals(values[0].valores),
+        "powers": parse_instant_powers(values[1].valores),
+        "iv": parse_iv(values[2].valores),
+        "meter_serial": meter_serial
+    }
+    return res
+
+
+def parse_instant_totals(totalizer):
+    return {
+        "ae": totalizer.ae,
+        "ae_val": totalizer.ae_val,
+        "ai": totalizer.ai,
+        "ai_val": totalizer.ai_val,
+        "r1": totalizer.r1,
+        "r1_val": totalizer.r1_val,
+        "r2": totalizer.r2,
+        "r2_val": totalizer.r2_val,
+        "r3": totalizer.r3,
+        "r3_val": totalizer.r3_val,
+        "r4": totalizer.r4,
+        "r4_val": totalizer.r4_val,
+        "measure_date": totalizer.measure_date.datetime.strftime('%Y-%m-%d %H:%M:%S')
+    }
+
+
+def parse_instant_powers(powers):
+    res = {
+        'records': [],
+        'measure_date': False
+    }
+    for i in range(0, len(powers)-1):
+        record = {
+            "fase": powers[i].fase,
+            "potencia_activa": powers[i].potencia_activa,
+            "potencia_reactiva": powers[i].potencia_reactiva,
+            "factor_potencia": powers[i].factor_potencia,
+            "is_exporting_activa": powers[i].is_exporting_activa,
+            "is_exporting_reactiva": powers[i].is_exporting_reactiva,
+            "valid": powers[i].valid
+        }
+        res['records'].append(record)
+    res['measure_date'] = powers[len(powers)-1].datetime.strftime('%Y-%m-%d %H:%M:%S')
+    return res
+
+
+def parse_iv(ivs):
+    res = {
+        'records': [],
+        'measure_date': False
+    }
+    for i in range(0, len(ivs)-1):
+        record = {
+            "phase": ivs[i].phase,
+            "I": ivs[i].I,
+            "V": ivs[i].V,
+            "valid": ivs[i].valid
+        }
+        res['records'].append(record)
+    res['measure_date'] = ivs[len(ivs)-1].datetime.strftime('%Y-%m-%d %H:%M:%S')
+    return res
+
 class ReemoteTCPIPWrapper(object):
 
     def __init__(self, ipaddr, port, link, mpoint, passwrd, datefrom, dateto,
                  option, request, contract=None, delay=None, wait_seconds=2):
         """
 
         :param ipaddr: Ip addres for the connection
@@ -218,14 +282,16 @@
                     output = self.get_daily_billings()
                 elif self.option == 'p':
                     output = self.get_profiles()
                 elif self.option == 'p4':
                     output = self.get_quarter_hour_profiles()
                 elif self.option in ('t', 'ts'):
                     output = self.sync_datetime()
+                elif self.option == 'iv':
+                    output = self.get_instant_values()
         except Exception as e:
             exception_txt = '{}'.format(e)
             exception = True
 
         if not output:
             error = True
             error_message += 'No output received. '
@@ -374,14 +440,20 @@
         res['current_datetime'] = current_datetime.strftime('%Y-%m-%d %H:%M:%S')
         if res['diff'] > self.delay and self.option == 'ts':
             resp_update_time = self.app_layer.set_datetime()
             if resp_update_time:
                 res['updated'] = True
         return res
 
+    def get_instant_values(self):
+        logger.info('Requesting instant values to device')
+        instant_objects = ['totalizadores', 'potencias', 'I_V']
+        resp = self.app_layer.ext_read_instant_values(objects=instant_objects)
+        return parse_instant_values(resp.content.valores, self.meter_serial)
+
     def establish_connection(self):
         try:
             logger.info('Establishing connection...')
             physical_layer = iec870ree.ip.Ip((self.ipaddr, self.port), self.wait_seconds)
             link_layer = iec870ree.protocol.LinkLayer(self.link, self.mpoint)
             link_layer.initialize(physical_layer)
             app_layer = iec870ree.protocol.AppLayer()
```

