# Comparing `tmp/pyreemote-11.2.0.tar.gz` & `tmp/pyreemote-12.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyreemote-11.2.0.tar", last modified: Thu Apr 18 09:06:56 2019, max compression
+gzip compressed data, was "dist/pyreemote-12.1.0.tar", last modified: Wed Sep 21 10:52:49 2022, max compression
```

## Comparing `pyreemote-11.2.0.tar` & `pyreemote-12.1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 agusti    (1000) agusti    (1000)        0 2019-04-18 09:06:56.000000 pyreemote-11.2.0/
-drwxrwxr-x   0 agusti    (1000) agusti    (1000)        0 2019-04-18 09:06:56.000000 pyreemote-11.2.0/pyreemote/
--rw-rw-r--   0 agusti    (1000) agusti    (1000)       56 2019-04-18 09:05:31.000000 pyreemote-11.2.0/pyreemote/__init__.py
--rw-rw-r--   0 agusti    (1000) agusti    (1000)    19935 2019-04-18 09:04:24.000000 pyreemote-11.2.0/pyreemote/telemeasure.py
--rw-rw-r--   0 agusti    (1000) agusti    (1000)      465 2019-04-18 09:04:24.000000 pyreemote-11.2.0/setup.py
--rw-rw-r--   0 agusti    (1000) agusti    (1000)      274 2019-04-18 09:06:56.000000 pyreemote-11.2.0/PKG-INFO
--rw-rw-r--   0 agusti    (1000) agusti    (1000)       38 2019-04-18 09:06:56.000000 pyreemote-11.2.0/setup.cfg
-drwxrwxr-x   0 agusti    (1000) agusti    (1000)        0 2019-04-18 09:06:56.000000 pyreemote-11.2.0/pyreemote.egg-info/
--rw-rw-r--   0 agusti    (1000) agusti    (1000)       24 2019-04-18 09:06:56.000000 pyreemote-11.2.0/pyreemote.egg-info/requires.txt
--rw-rw-r--   0 agusti    (1000) agusti    (1000)       10 2019-04-18 09:06:56.000000 pyreemote-11.2.0/pyreemote.egg-info/top_level.txt
--rw-rw-r--   0 agusti    (1000) agusti    (1000)      274 2019-04-18 09:06:56.000000 pyreemote-11.2.0/pyreemote.egg-info/PKG-INFO
--rw-rw-r--   0 agusti    (1000) agusti    (1000)      219 2019-04-18 09:06:56.000000 pyreemote-11.2.0/pyreemote.egg-info/SOURCES.txt
--rw-rw-r--   0 agusti    (1000) agusti    (1000)        1 2019-04-18 09:06:56.000000 pyreemote-11.2.0/pyreemote.egg-info/dependency_links.txt
+drwxrwxr-x   0 afita     (1000) afita     (1000)        0 2022-09-21 10:52:49.000000 pyreemote-12.1.0/
+drwxrwxr-x   0 afita     (1000) afita     (1000)        0 2022-09-21 10:52:49.000000 pyreemote-12.1.0/pyreemote/
+-rw-rw-r--   0 afita     (1000) afita     (1000)    24369 2021-12-27 12:27:02.000000 pyreemote-12.1.0/pyreemote/telemeasure.py
+-rw-r--r--   0 afita     (1000) afita     (1000)       56 2021-12-27 12:28:11.000000 pyreemote-12.1.0/pyreemote/__init__.py
+drwxrwxr-x   0 afita     (1000) afita     (1000)        0 2022-09-21 10:52:49.000000 pyreemote-12.1.0/pyreemote.egg-info/
+-rw-r--r--   0 afita     (1000) afita     (1000)       10 2022-09-21 10:52:49.000000 pyreemote-12.1.0/pyreemote.egg-info/top_level.txt
+-rw-r--r--   0 afita     (1000) afita     (1000)      219 2022-09-21 10:52:49.000000 pyreemote-12.1.0/pyreemote.egg-info/SOURCES.txt
+-rw-r--r--   0 afita     (1000) afita     (1000)      274 2022-09-21 10:52:49.000000 pyreemote-12.1.0/pyreemote.egg-info/PKG-INFO
+-rw-r--r--   0 afita     (1000) afita     (1000)        1 2022-09-21 10:52:49.000000 pyreemote-12.1.0/pyreemote.egg-info/dependency_links.txt
+-rw-r--r--   0 afita     (1000) afita     (1000)       31 2022-09-21 10:52:49.000000 pyreemote-12.1.0/pyreemote.egg-info/requires.txt
+-rw-rw-r--   0 afita     (1000) afita     (1000)      274 2022-09-21 10:52:49.000000 pyreemote-12.1.0/PKG-INFO
+-rw-rw-r--   0 afita     (1000) afita     (1000)       38 2022-09-21 10:52:49.000000 pyreemote-12.1.0/setup.cfg
+-rw-rw-r--   0 afita     (1000) afita     (1000)      472 2021-12-27 12:27:02.000000 pyreemote-12.1.0/setup.py
```

### Comparing `pyreemote-11.2.0/pyreemote/telemeasure.py` & `pyreemote-12.1.0/pyreemote/telemeasure.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 import requests
 import iec870ree.ip
 import iec870ree.protocol
 import iec870ree_moxa.moxa
 
 TIMEZONE = timezone('Europe/Madrid')
 
+logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger(__name__)
 
 MAGNITUDES = {
     1: 'AI',
     2: 'AE',
     3: 'R1',
     4: 'R2',
@@ -45,17 +46,18 @@
         return True
     except ValueError:
         return False
 
 
 def get_season(dt):
     if dt.dst().seconds > 0:
-        return 'S'
+        season = 'S'
     else:
-        return 'W'
+        season = 'W'
+    return season
 
 
 def parse_billings(billings, contract, meter_serial, datefrom, dateto):
     res = {
         'Contract': contract,
         'DateFrom': datefrom,
         'DateTo': dateto,
@@ -88,28 +90,56 @@
             'PeriodStart': billing_period.date_start.strftime('%Y-%m-%d %H:%M:%S'),
             'QualityExcess': billing_period.ecxess_power_qual
         }
         res['Totals'].append(period)
     return res
 
 
+def parse_daily_billings(billings, meter_serial, value, datefrom, dateto, contract=1):
+    res = {
+        'Contract': contract,
+        'DateFrom': datefrom,
+        'DateTo': dateto,
+        'SerialNumber': str(meter_serial),
+        'Totals': []
+    }
+    for billing in billings:
+        period = {
+            'Tariff': 0,
+            'ai': billing[0].total,
+            'ae': billing[1].total,
+            'r1': billing[2].total,
+            'r2': billing[3].total,
+            'r3': billing[4].total,
+            'r4': billing[5].total,
+            'PeriodEnd': billing[0].datetime.strftime('%Y-%m-%d %H:%M:%S'),
+            'PeriodStart': billing[0].datetime.strftime('%Y-%m-%d %H:%M:%S'),
+            'value': value,
+        }
+        res['Totals'].append(period)
+    return res
+
+
 def parse_profiles(profiles, meter_serial, datefrom, dateto):
     res = {
         'Number': 1,
         'Absolute': False,
         'DateFrom': datefrom,
         'DateTo': dateto,
         'SerialNumber': str(meter_serial),
         'Records': []
     }
     for hour_profile in profiles:
         date = hour_profile[0].datetime
+        locdate = date
+        if locdate.tzinfo is None:
+            locdate = TIMEZONE.localize(date)
         record = {
-            'TimeInfo': date.strftime('%Y-%m-%d %H:%M:%S'),
-            'Season': get_season(TIMEZONE.localize(date)),
+            'TimeInfo': locdate.strftime('%Y-%m-%d %H:%M:%S'),
+            'Season': get_season(locdate),
             'Channels': []
         }
         for channel in hour_profile:
             if channel.address not in [7, 8]:  # Skip RES7 and RES8 registers
                 channel = {
                     'Magnitude': MAGNITUDES[channel.address],
                     'Value': channel.total,
@@ -119,112 +149,141 @@
         res['Records'].append(record)
     return res
 
 
 class ReemoteTCPIPWrapper(object):
 
     def __init__(self, ipaddr, port, link, mpoint, passwrd, datefrom, dateto,
-                 option, request, contract=None):
+                 option, request, contract=None, delay=None, wait_seconds=2):
         """
 
         :param ipaddr: Ip addres for the connection
         :param port: Port for the connection
         :param link: LinkAddress
         :param mpoint: MeasuringPointAddress
         :param passwrd: Password
         :param datefrom: Date
         :param dateto: Date
         :param option: Either "b" for Billings or "p" for Profiles
         :param request: Different types of request for the Profiles
         :param contract: List of contracts e.g:[1,3]
+        :param wait_seconds: Waiting seconds to connect
         """
         if validate(datefrom) and validate(dateto):
             self.meter_serial = None
             self.app_layer = None
             self.physical_layer = None
             self.ipaddr = ipaddr
             self.port = port
             self.link = link
             self.mpoint = mpoint
             self.passwrd = passwrd
             self.datefrom = datetime.strptime(datefrom, '%Y-%m-%dT%H:%M:%S')
             self.dateto = datetime.strptime(dateto, '%Y-%m-%dT%H:%M:%S')
             self.option = option
             self.request = request
+            self.wait_seconds = wait_seconds
             if contract:
                 if not isinstance(contract, list):
                     contract = list(contract)
                 self.contract = contract
             else:
                 self.contract = []
+            self.delay = delay
 
             if 'REEMOTE_PATH' in os.environ:
                 self.reemote = urlparse(os.environ['REEMOTE_PATH'])
             else:
                 self.reemote = 'local'
         else:
             raise ValueError(
                 'ERROR: Date format is wrong. Expected: %Y-%m-%dT%H:%M:%S'
             )
 
     def handle_file_request(self):
         output = ''
-        if self.app_layer:
-            if self.meter_serial is None:
-                resp = self.app_layer.get_info()
-                self.meter_serial = resp.content.codigo_equipo
-                print(self.meter_serial)
-            if self.option == 'b':
-                if not self.contract:
-                    self.contract = [1, 2, 3]
-                output = self.get_billings()
-            elif self.option == 'p':
-                output = self.get_profiles()
-            elif self.option == 'p4':
-                output = self.get_quarter_hour_profiles()
+        exception = False
+        error_message = ''
+        error = False
+        try:
+            if self.app_layer:
+                if self.meter_serial is None:
+                    resp = self.app_layer.get_info()
+                    self.meter_serial = resp.content.codigo_equipo
+                    print(self.meter_serial)
+                if self.option == 'b':
+                    if not self.contract:
+                        self.contract = [1, 2, 3]
+                    output = self.get_billings()
+                elif self.option == 'd':
+                    output = self.get_daily_billings()
+                elif self.option == 'p':
+                    output = self.get_profiles()
+                elif self.option == 'p4':
+                    output = self.get_quarter_hour_profiles()
+                elif self.option in ('t', 'ts'):
+                    output = self.sync_datetime()
+        except Exception as e:
+            exception_txt = '{}'.format(e)
+            exception = True
+
+        if not output:
+            error = True
+            error_message += 'No output received. '
+        if exception:
+            error_message += 'An Exception was raised: {}.'.format(exception_txt)
+
         result = {
-            'error': True if not output else False,
+            'error': error,
             'message': '',
-            'error_message': 'No output received',
+            'error_message': error_message,
         }
         if output:
             try:
                 result['message'] = output
                 result['error_message'] = ''
             except:
                 result['error'] = True
-                result['error_message'] = 'ERROR: No JSON object could be decoded'
+                result['error_message'] += 'ERROR: No JSON object could be decoded'
         return result
 
     def execute_request(self):
         if self.reemote == 'local':
-            self.establish_connection()
+            exception_txt = ''
+            try:
+                self.establish_connection()
+            except Exception as e:
+                exception = True
+                exception_txt = '{}'.format(e)
+
             if self.app_layer is not None and self.physical_layer is not None:
                 result = self.handle_file_request()
                 self.close_connection()
             else:
                 return {
                     'error': True,
                     'message': '',
-                    'error_message': "Couldn't establish connection",
+                    'error_message': "Couldn't establish connection: {}".format(exception_txt),
                 }
 
         elif self.reemote.scheme == 'http':
             logger.info('Sending request to API...')
             post_data = {
                 'ipaddr': self.ipaddr,
                 'port': self.port,
                 'link': self.link,
                 'mpoint': self.mpoint,
                 'passwrd': self.passwrd,
                 'datefrom': self.datefrom.strftime('%Y-%m-%dT%H:%M:%S'),
                 'dateto': self.dateto.strftime('%Y-%m-%dT%H:%M:%S'),
                 'option': self.option,
                 'request': self.request,
-                'contract': self.contract
+                'contract': self.contract,
+                'delay': self.delay,
+                'wait_seconds': int(self.wait_seconds),
             }
             response = requests.post(self.reemote.geturl(), data=post_data, allow_redirects=True)
             response = json.loads(response.content)
             if response['error']:
                 logger.info('Received error message from API')
                 result = {
                     'error': True,
@@ -258,14 +317,29 @@
                 values.extend(resp.content.valores)
             aux = parse_billings(values, contract, self.meter_serial,
                                  self.datefrom.strftime('%Y-%m-%d %H:%M:%S'),
                                  self.dateto.strftime('%Y-%m-%d %H:%M:%S'))
             res['Results'].append(aux)
         return res
 
+    def get_daily_billings(self):
+        logger.info('Requesting daily billings to device.')
+        res = {'Results': []}
+        values = []
+        for resp in self.app_layer.read_incremental_values(self.datefrom,
+                                                           self.dateto,
+                                                           register='daily_billings'):
+            values.append(resp.content.valores)
+        aux = parse_daily_billings(values, self.meter_serial, 'i',
+                                   self.datefrom.strftime('%Y-%m-%d %H:%M:%S'),
+                                   self.dateto.strftime('%Y-%m-%d %H:%M:%S'),
+                                   contract=1)
+        res['Results'].append(aux)
+        return res
+
     def get_profiles(self):
         logger.info('Requesting profiles to device.')
         values = []
         for resp in self.app_layer.read_incremental_values(self.datefrom,
                                                            self.dateto,
                                                            register='profiles'):
             values.append(resp.content.valores)
@@ -279,18 +353,39 @@
         for resp in self.app_layer.read_incremental_values(
                 self.datefrom, self.dateto, register='quarter_hour'):
             values.append(resp.content.valores)
         return parse_profiles(values, self.meter_serial,
                               self.datefrom.strftime('%Y-%m-%d %H:%M:%S'),
                               self.dateto.strftime('%Y-%m-%d %H:%M:%S'))
 
+    def sync_datetime(self):
+        res = {
+            'diff': 0,
+            'datetime_meter': False,
+            'current_datetime': False,
+            'updated': False,
+        }
+        logger.info('Requesting datetime to device.')
+        resp_time = self.app_layer.read_datetime()
+        current_datetime = resp_time.content.tiempo.datetime
+        datetime_meter = datetime.now(TIMEZONE)
+        diff = current_datetime - datetime_meter
+        res['diff'] = abs(diff.total_seconds())
+        res['datetime_meter'] = datetime_meter.strftime('%Y-%m-%d %H:%M:%S')
+        res['current_datetime'] = current_datetime.strftime('%Y-%m-%d %H:%M:%S')
+        if res['diff'] > self.delay and self.option == 'ts':
+            resp_update_time = self.app_layer.set_datetime()
+            if resp_update_time:
+                res['updated'] = True
+        return res
+
     def establish_connection(self):
         try:
             logger.info('Establishing connection...')
-            physical_layer = iec870ree.ip.Ip((self.ipaddr, self.port))
+            physical_layer = iec870ree.ip.Ip((self.ipaddr, self.port), self.wait_seconds)
             link_layer = iec870ree.protocol.LinkLayer(self.link, self.mpoint)
             link_layer.initialize(physical_layer)
             app_layer = iec870ree.protocol.AppLayer()
             app_layer.initialize(link_layer)
 
             physical_layer.connect()
             logger.info('Physical layer connected')
@@ -302,14 +397,15 @@
 
             self.app_layer = app_layer
             self.physical_layer = physical_layer
         except Exception as e:
             logger.info('Connection failed. Exiting process...')
             if self.connected:
                 self.close_connection()
+            raise e
 
     def close_connection(self):
         logger.info('Closing connection...')
         self.app_layer.finish_session()
         self.physical_layer.disconnect()
         logger.info('Disconnected')
 
@@ -325,28 +421,30 @@
         response = requests.get(url)
         return json.loads(response.content)
 
 
 class ReemoteMOXAWrapper(ReemoteTCPIPWrapper):
 
     def __init__(self, phone, ipaddr, port, link, mpoint, passwrd, datefrom,
-                 dateto, option, request, contract=None):
+                 dateto, option, request, contract=None, delay=None, wait_seconds=2, modem_init_str=None):
         """
         :param phone: Phone number
+        :param modem_init_str: Modem initializing string
         """
         self.phone = phone
+        self.modem_init_str = modem_init_str
         super(ReemoteMOXAWrapper, self).__init__(ipaddr, port, link, mpoint,
                                                  passwrd, datefrom, dateto,
-                                                 option, request, contract)
+                                                 option, request, contract, delay, wait_seconds)
 
     def establish_connection(self):
         try:
             logger.info('Establishing connection...')
-            ip_layer = iec870ree.ip.Ip((self.ipaddr, self.port))
-            moxa_layer = iec870ree_moxa.moxa.Moxa(self.phone, ip_layer)
+            ip_layer = iec870ree.ip.Ip((self.ipaddr, self.port), self.wait_seconds)
+            moxa_layer = iec870ree_moxa.moxa.Moxa(self.phone, ip_layer, self.modem_init_str)
             link_layer = iec870ree.protocol.LinkLayer(self.link, self.mpoint)
             link_layer.initialize(moxa_layer)
             app_layer = iec870ree.protocol.AppLayer()
             app_layer.initialize(link_layer)
 
             moxa_layer.connect()
             logger.info('MOXA physical layer connected')
@@ -358,26 +456,33 @@
 
             self.app_layer = app_layer
             self.physical_layer = moxa_layer
         except Exception as e:
             logger.info('Connection failed. Exiting process...')
             if self.connected:
                 self.close_connection()
+            raise e
 
     def execute_request(self):
         if self.reemote == 'local':
-            self.establish_connection()
+            exception_txt = ''
+            try:
+                self.establish_connection()
+            except Exception as e:
+                exception = True
+                exception_txt = '{}'.format(e)
+
             if self.app_layer is not None and self.physical_layer is not None:
                 result = self.handle_file_request()
                 self.close_connection()
             else:
                 return {
                     'error': True,
                     'message': '',
-                    'error_message': "Couldn't establish connection",
+                    'error_message': "Couldn't establish connection: {}".format(exception_txt),
                 }
 
         elif self.reemote.scheme == 'http':
             logger.info('Sending request to API...')
             post_data = {
                 'phone': self.phone,
                 'ipaddr': self.ipaddr,
@@ -385,15 +490,18 @@
                 'link': self.link,
                 'mpoint': self.mpoint,
                 'passwrd': self.passwrd,
                 'datefrom': self.datefrom.strftime('%Y-%m-%dT%H:%M:%S'),
                 'dateto': self.dateto.strftime('%Y-%m-%dT%H:%M:%S'),
                 'option': self.option,
                 'request': self.request,
-                'contract': self.contract
+                'modem_init_str': self.modem_init_str,
+                'contract': self.contract,
+                'delay': self.delay,
+                'wait_seconds': self.wait_seconds
             }
             response = requests.post(self.reemote.geturl(), data=post_data, allow_redirects=True)
             response = json.loads(response.content)
             if response['error']:
                 logger.info('Received error message from API')
                 result = {
                     'error': True,
@@ -416,27 +524,28 @@
 
         return result
 
 
 class ReemoteModemWrapper(object):
 
     def __init__(self, phone, port, link, mpoint, passwrd, datefrom, dateto,
-                 option, request, contract=None):
+                 option, request, contract=None, delay=None, wait_seconds=2):
         """
 
         :param phone: Phone number of the modem
         :param port: Port for the connection
         :param link: LinkAddress
         :param mpoint: MeasuringPointAddress
         :param passwrd: Password
         :param datefrom: Date
         :param dateto: Date
         :param option: Either "b" for Billings or "p" for Profiles
         :param request: Different types of request for the Profiles
         :param contract: List of contracts e.g:[1,3]
+        :param wait_seconds: Waiting seconds to connect
         """
         if validate(datefrom) and validate(dateto):
             self.phone = phone
             self.port = port
             self.link = link
             self.mpoint = mpoint
             self.passwrd = passwrd
@@ -446,14 +555,15 @@
             self.request = request
             if contract:
                 if not isinstance(contract, list):
                     contract = list(contract)
                 self.contract = contract
             else:
                 self.contract = None
+            self.delay = delay
 
             if 'REEMOTE_PATH' in os.environ:
                 if os.environ['REEMOTE_PATH'] == 'local':
                     self.reemote = 'local'
                 else:
                     self.reemote = urlparse(os.environ['REEMOTE_PATH'])
             else:
@@ -480,15 +590,17 @@
                 'link_address': self.link,
                 'mpoint': self.mpoint,
                 'passwrd': self.passwrd,
                 'datefrom': self.datefrom,
                 'dateto': self.dateto,
                 'option': self.option,
                 'request': self.request,
-                'contract': self.contract
+                'contract': self.contract,
+                'delay': self.delay,
+                'wait_seconds': self.wait_seconds
             }
             response = requests.post(self.reemote.geturl(), data=post_data)
             if response['error']:
                 result = {
                     'error': True,
                     'message': response['message'],
                     'error_message': response['errors'],
```

