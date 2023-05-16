# Comparing `tmp/inhandtest-0.0.45.tar.gz` & `tmp/inhandtest-0.0.46.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\inhandtest-0.0.45.tar", last modified: Mon May 15 10:20:08 2023, max compression
+gzip compressed data, was "dist\inhandtest-0.0.46.tar", last modified: Tue May 16 09:07:53 2023, max compression
```

## Comparing `inhandtest-0.0.45.tar` & `inhandtest-0.0.46.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 10:20:08.000000 inhandtest-0.0.45/
--rw-rw-rw-   0        0        0      535 2023-05-15 10:20:08.000000 inhandtest-0.0.45/PKG-INFO
--rw-rw-rw-   0        0        0    12238 2023-02-27 03:43:37.000000 inhandtest-0.0.45/README.md
-drwxrwxrwx   0        0        0        0 2023-05-15 10:20:08.000000 inhandtest-0.0.45/inhandtest/
--rw-rw-rw-   0        0        0        0 2023-01-31 08:41:58.000000 inhandtest-0.0.45/inhandtest/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 10:20:08.000000 inhandtest-0.0.45/inhandtest/base_page/
--rw-rw-rw-   0        0        0      134 2023-03-15 06:05:35.000000 inhandtest-0.0.45/inhandtest/base_page/__init__.py
--rw-rw-rw-   0        0        0    38524 2023-05-15 06:31:20.000000 inhandtest-0.0.45/inhandtest/base_page/_ig_contents_locators.py
--rw-rw-rw-   0        0        0    27870 2023-05-10 08:56:15.000000 inhandtest-0.0.45/inhandtest/base_page/_ir3XX_contents_locators.py
--rw-rw-rw-   0        0        0    64964 2023-05-11 07:07:35.000000 inhandtest-0.0.45/inhandtest/base_page/_vg710_contents_locators.py
--rw-rw-rw-   0        0        0    49374 2023-05-15 08:48:06.000000 inhandtest-0.0.45/inhandtest/base_page/base_page.py
--rw-rw-rw-   0        0        0    10957 2023-05-09 09:49:30.000000 inhandtest-0.0.45/inhandtest/base_page/table_tr.py
--rw-rw-rw-   0        0        0      608 2023-03-31 07:18:06.000000 inhandtest-0.0.45/inhandtest/exception.py
--rw-rw-rw-   0        0        0     3890 2023-03-30 10:08:49.000000 inhandtest-0.0.45/inhandtest/file.py
--rw-rw-rw-   0        0        0    11861 2023-05-06 01:56:01.000000 inhandtest-0.0.45/inhandtest/inmodbus.py
--rw-rw-rw-   0        0        0     4880 2023-04-27 01:05:22.000000 inhandtest-0.0.45/inhandtest/inmongodb.py
--rw-rw-rw-   0        0        0    22049 2023-03-30 10:08:49.000000 inhandtest-0.0.45/inhandtest/inmqtt.py
--rw-rw-rw-   0        0        0    48029 2023-05-15 10:04:52.000000 inhandtest-0.0.45/inhandtest/inrequest.py
--rw-rw-rw-   0        0        0     7583 2023-05-06 07:36:44.000000 inhandtest-0.0.45/inhandtest/inserial.py
--rw-rw-rw-   0        0        0    12335 2023-04-06 06:40:29.000000 inhandtest-0.0.45/inhandtest/insocket.py
--rw-rw-rw-   0        0        0     6076 2023-05-15 10:19:14.000000 inhandtest-0.0.45/inhandtest/inssh.py
--rw-rw-rw-   0        0        0     1144 2023-03-30 10:18:47.000000 inhandtest-0.0.45/inhandtest/ip.py
--rw-rw-rw-   0        0        0    11620 2023-05-08 10:30:07.000000 inhandtest-0.0.45/inhandtest/mail.py
--rw-rw-rw-   0        0        0     1224 2023-04-28 06:53:30.000000 inhandtest-0.0.45/inhandtest/pytest_email.html
--rw-rw-rw-   0        0        0    32728 2023-05-06 01:14:17.000000 inhandtest-0.0.45/inhandtest/telnet.py
--rw-rw-rw-   0        0        0    25281 2023-05-12 08:18:46.000000 inhandtest-0.0.45/inhandtest/tools.py
--rw-rw-rw-   0        0        0      137 2023-05-15 07:42:26.000000 inhandtest-0.0.45/requirements.txt
--rw-rw-rw-   0        0        0     1450 2023-05-15 10:19:56.000000 inhandtest-0.0.45/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 09:07:53.000000 inhandtest-0.0.46/
+-rw-rw-rw-   0        0        0      535 2023-05-16 09:07:53.000000 inhandtest-0.0.46/PKG-INFO
+-rw-rw-rw-   0        0        0    12238 2023-02-27 03:43:37.000000 inhandtest-0.0.46/README.md
+drwxrwxrwx   0        0        0        0 2023-05-16 09:07:53.000000 inhandtest-0.0.46/inhandtest/
+-rw-rw-rw-   0        0        0        0 2023-01-31 08:41:58.000000 inhandtest-0.0.46/inhandtest/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 09:07:53.000000 inhandtest-0.0.46/inhandtest/base_page/
+-rw-rw-rw-   0        0        0      134 2023-03-15 06:05:35.000000 inhandtest-0.0.46/inhandtest/base_page/__init__.py
+-rw-rw-rw-   0        0        0    39712 2023-05-16 03:23:36.000000 inhandtest-0.0.46/inhandtest/base_page/_ig_contents_locators.py
+-rw-rw-rw-   0        0        0    27870 2023-05-10 08:56:15.000000 inhandtest-0.0.46/inhandtest/base_page/_ir3XX_contents_locators.py
+-rw-rw-rw-   0        0        0    64964 2023-05-11 07:07:35.000000 inhandtest-0.0.46/inhandtest/base_page/_vg710_contents_locators.py
+-rw-rw-rw-   0        0        0    49636 2023-05-16 05:53:35.000000 inhandtest-0.0.46/inhandtest/base_page/base_page.py
+-rw-rw-rw-   0        0        0    10957 2023-05-09 09:49:30.000000 inhandtest-0.0.46/inhandtest/base_page/table_tr.py
+-rw-rw-rw-   0        0        0      608 2023-03-31 07:18:06.000000 inhandtest-0.0.46/inhandtest/exception.py
+-rw-rw-rw-   0        0        0     3890 2023-03-30 10:08:49.000000 inhandtest-0.0.46/inhandtest/file.py
+-rw-rw-rw-   0        0        0    11861 2023-05-06 01:56:01.000000 inhandtest-0.0.46/inhandtest/inmodbus.py
+-rw-rw-rw-   0        0        0     4880 2023-04-27 01:05:22.000000 inhandtest-0.0.46/inhandtest/inmongodb.py
+-rw-rw-rw-   0        0        0    22049 2023-03-30 10:08:49.000000 inhandtest-0.0.46/inhandtest/inmqtt.py
+-rw-rw-rw-   0        0        0    51883 2023-05-16 09:03:39.000000 inhandtest-0.0.46/inhandtest/inrequest.py
+-rw-rw-rw-   0        0        0     7583 2023-05-06 07:36:44.000000 inhandtest-0.0.46/inhandtest/inserial.py
+-rw-rw-rw-   0        0        0    12335 2023-04-06 06:40:29.000000 inhandtest-0.0.46/inhandtest/insocket.py
+-rw-rw-rw-   0        0        0     6076 2023-05-15 10:19:14.000000 inhandtest-0.0.46/inhandtest/inssh.py
+-rw-rw-rw-   0        0        0     1144 2023-03-30 10:18:47.000000 inhandtest-0.0.46/inhandtest/ip.py
+-rw-rw-rw-   0        0        0    11620 2023-05-08 10:30:07.000000 inhandtest-0.0.46/inhandtest/mail.py
+-rw-rw-rw-   0        0        0     1224 2023-04-28 06:53:30.000000 inhandtest-0.0.46/inhandtest/pytest_email.html
+-rw-rw-rw-   0        0        0    32728 2023-05-06 01:14:17.000000 inhandtest-0.0.46/inhandtest/telnet.py
+-rw-rw-rw-   0        0        0    25281 2023-05-12 08:18:46.000000 inhandtest-0.0.46/inhandtest/tools.py
+-rw-rw-rw-   0        0        0      137 2023-05-15 07:42:26.000000 inhandtest-0.0.46/requirements.txt
+-rw-rw-rw-   0        0        0     1450 2023-05-16 09:07:33.000000 inhandtest-0.0.46/setup.py
```

### Comparing `inhandtest-0.0.45/PKG-INFO` & `inhandtest-0.0.46/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: inhandtest
-Version: 0.0.45
+Version: 0.0.46
 Summary: inhand test tools, so easy
 Home-page: https://inhandnetworks.yuque.com/irhb08/mrpu1r/qgu0imvigkm2xry9?singleDoc# 《inhandtest docs》
 Author: liwei
 Author-email: liwei@inhand.com.cn
 License: UNKNOWN
 Description: 方便inhand测试同事在自动化测试时，对通用协议或者常用工具及方法做封装，需要使用时即在线安装；
         映翰通出品，追尾必究！
```

### Comparing `inhandtest-0.0.45/README.md` & `inhandtest-0.0.46/README.md`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.45/inhandtest/base_page/_ig_contents_locators.py` & `inhandtest-0.0.46/inhandtest/base_page/_ig_contents_locators.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,16 @@
                                    'system': 'System', 'system_time': 'System Time', 'system_log': 'Log',
                                    'system_config': 'Configuration Management', 'system_cloud': 'InHand Cloud',
                                    'system_firmware': 'Firmware Upgrade', 'system_tools': 'Access Tools',
                                    'system_user_management': 'User Management', 'system_reboot': 'Reboot',
                                    'system_network_tools': 'Network Tools',
                                    'system_3rd_party': '3rd Party Notification',
                                    'configuration': ' Configuration', 'trigger_condition': 'Trigger Condition',
-                                   'gigabitethernet': 'Gigabitethernet',
+                                   'gigabitethernet': 'Gigabitethernet', 'flow_usage_day': 'Flow Usage Monitoring(Day)',
+                                   'flow_usage_month': 'Flow Usage Monitoring(Month)'
                                    }
         else:
             self.__locale: dict = {'network': '网络', 'network_interface': '网络接口', 'performance': '性能与存储',
                                    'cellular': '蜂窝网', 'ethernet': '以太网',
                                    'bridge': '桥接口', 'loopback': '环回接口',
                                    'network_service': '网络服务', 'dhcp': 'DHCP服务',
                                    'dns': 'DNS服务', "gps_configure": "GPS 配置", 'gps': 'GPS',
@@ -78,14 +79,15 @@
                                    'system': '系统管理', 'system_time': '系统时间', 'system_log': '系统日志',
                                    'system_config': '配置管理', 'system_cloud': '设备云平台',
                                    'system_firmware': '固件升级', 'system_tools': '管理工具',
                                    'system_user_management': '用户管理', 'system_reboot': '重启',
                                    'system_network_tools': '工具', 'system_3rd_party': '第三方软件声明',
                                    'configuration': '配置',
                                    'trigger_condition': '触发条件', 'gigabitethernet': '千兆以太网口',
+                                   'flow_usage_day': '流量使用监测（当天）', 'flow_usage_month': '流量使用监测（当月）'
                                    }
 
     def content_target(self, locale) -> Locator:
         if self.__locale.get(locale):
             locale = self.__locale.get(locale)
         return self.page.locator(f'//span[@class="ant-breadcrumb-link"]/span[text()="{locale}"]')
 
@@ -283,16 +285,30 @@
     def system_3rd_party_menu(self) -> Locator:
         return self.page.locator(f'a:has-text("{self.__locale.get("system_3rd_party")}")')
 
     @property
     def tags_menu(self) -> dict:
         return {
             'overview': {
+                'default': 'flow_usage_monitoring(day)',
                 'menu': self.overview_menu,
                 'visible_locator': [self.page.locator(f'//div[text()="{self.__locale.get("performance")}"]')],
+                'wait_locator': [self.page.locator(f'//div[text()="{self.__locale.get("performance")}"]')],
+                'flow_usage_monitoring(day)': {
+                    'menu': self.page.locator(f'div:text-is("{self.__locale.get("flow_usage_day")}")'),
+                    'attributes': {
+                        self.page.locator(f'div:text-is("{self.__locale.get("flow_usage_day")}")'): {
+                            'aria-selected': 'true'}},
+                },
+                'flow_usage_monitoring(month)': {
+                    'menu': self.page.locator(f'div:text-is("{self.__locale.get("flow_usage_month")}")'),
+                    'attributes': {
+                        self.page.locator(f'div:text-is("{self.__locale.get("flow_usage_month")}")'): {
+                            'aria-selected': 'true'}},
+                }
             },
             'network': {
                 'default': 'network_interface.cellular',
                 'menu': self.network_menu,
                 'visible_locator': [self.page.locator('//span[@class="ant-breadcrumb-link"]/a[@href="/network"]')],
                 'wait_locator': [self.content_target('cellular')],
                 'network_interface': {
```

### Comparing `inhandtest-0.0.45/inhandtest/base_page/_ir3XX_contents_locators.py` & `inhandtest-0.0.46/inhandtest/base_page/_ir3XX_contents_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.45/inhandtest/base_page/_vg710_contents_locators.py` & `inhandtest-0.0.46/inhandtest/base_page/_vg710_contents_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.45/inhandtest/base_page/base_page.py` & `inhandtest-0.0.46/inhandtest/base_page/base_page.py`

 * *Files 0% similar despite different names*

```diff
@@ -769,25 +769,25 @@
                     option = filter_key[0]
                     locator = option[1].get('locator')
                     if isinstance(locator, Locator):
                         value = locator.first.inner_text() if locator.count() != 0 else 'None'
                     else:
                         value = str(locator)
                     try:
-                        expression = expect_.get(key).replace('${value}', value)
+                        expression = expect_.get(key).replace('${value}', value).replace('\n', ' ')
                         if option[1].get('param'):
                             for replace_k, replace_v in option[1].get('param').items():
                                 expression = expression.replace(replace_k, replace_v)
-                        if eval(expression):
+                        if eval(expression, {'repr': repr}):
                             logging.info(f'Check {option[0]} , {expression} is true')
                         else:
                             logging.info(f'Check {option[0]} , {expression} is false')
                             return False
                     except TypeError:
-                        logging.info(f'get inner_text failed')
+                        logging.info(f'get {key} inner_text failed')
                         return False
                 else:
                     raise KeyError(f'not support the key {key}')
         return True
 
     @allure.step("获取页面元素文本值")
     def get_text(self, keys: str or list or tuple, locators: list) -> str or dict or None:
@@ -805,23 +805,26 @@
         if keys:
             keys = [keys] if isinstance(keys, str) else keys
             for key in keys:
                 filter_key = list(filter(lambda x: x[0] == key, locators))
                 if len(filter_key) == 1:
                     option = filter_key[0]
                     locator = option[1].get('locator')
-                    if locator.count() != 0:
-                        if option[1].get('type') == 'select':
-                            value = locator.first.text_content()
-                        elif option[1].get('type') == 'fill':
-                            value = locator.first.input_value()
+                    if isinstance(locator, Locator):
+                        if locator.count() != 0:
+                            if option[1].get('type') == 'select':
+                                value = locator.first.text_content()
+                            elif option[1].get('type') == 'fill':
+                                value = locator.first.input_value()
+                            else:
+                                value = locator.first.inner_text()
                         else:
-                            value = locator.first.inner_text()
+                            raise
                     else:
-                        raise
+                        value = str(locator)
                     result[key] = value
                 else:
                     raise KeyError(f'not support the key {key}')
         if result:
             if len(result.keys()) == 1:
                 return result.get(keys[0])
             else:
@@ -874,14 +877,15 @@
         return tag_result
 
     def close(self) -> None:
         if self.__context and self.__browser and self.__playwright:
             self.__context.close()
             self.__browser.close()
             self.__playwright.stop()
+            logging.info('close browser and playwright')
 
 
 if __name__ == '__main__':
     logging.basicConfig(format='%(asctime)s %(levelname)s %(message)s', level=logging.INFO,
                         stream=sys.stdout)
     with BasePage('10.5.24.96', 'adm', '123456', 'https', 443, model='ig902') as my_page:
         # system = (
```

### Comparing `inhandtest-0.0.45/inhandtest/base_page/table_tr.py` & `inhandtest-0.0.46/inhandtest/base_page/table_tr.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.45/inhandtest/exception.py` & `inhandtest-0.0.46/inhandtest/exception.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.45/inhandtest/file.py` & `inhandtest-0.0.46/inhandtest/file.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.45/inhandtest/inmodbus.py` & `inhandtest-0.0.46/inhandtest/inmodbus.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.45/inhandtest/inmongodb.py` & `inhandtest-0.0.46/inhandtest/inmongodb.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.45/inhandtest/inmqtt.py` & `inhandtest-0.0.46/inhandtest/inmqtt.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.45/inhandtest/inrequest.py` & `inhandtest-0.0.46/inhandtest/inrequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,87 @@
 import time
 from typing import List
 import urllib3
 import requests
 from inhandtest.exception import ParameterValueError, UsernameOrPasswordError, TimeOutError, UpgradeFailedError, \
     ResourceNotFoundError
 from inhandtest.file import file_hash
-from inhandtest.tools import dict_in, dict_merge, replace_str, DotDict
+from inhandtest.tools import dict_in, dict_merge, replace_str, DotDict, loop_inspector
+
+
+class DnInterface:
+    def __init__(self, username, password, host='c.inhand.com.cn'):
+        """
+        :param username  平台用户名
+        :param password  平台密码
+        :param host: 'c.inhand.com.cn'
+        """
+        self.host = host
+        self.username = username
+        self.api = InRequest(self.host, username, password, 'dn4')
+
+    def add_device(self, sn: str, mac: str, model: str) -> None:
+        """添加设备，
+
+        :param sn: 设备序列号
+        :param mac: 设备mac地址
+        :param model: 设备型号 IR6XX_EVDO  IR300
+        :return:
+        """
+
+        def get_model_id(model_name: str) -> str:
+            models = self.api.send_request('api/models', method='get', param={'limit': 0, 'verbose': 1}).json().get(
+                'result')
+            for model_ in models:
+                if model_.get('name').upper() == model_name.upper():
+                    return model_.get('_id')
+            else:
+                raise ResourceNotFoundError(f"the model {model_name} not found")
+
+        for i in range(3):
+            response = self.api.send_request('api/devices', method='get',
+                                             param={"verbose": 100, "limit": 10, "cursor": 0,
+                                                    'serial_number': sn, 'plc_id': 0})
+            if response.json().get('total') == 0:
+                body = {"deviceConfig": {"maxHeartbeatLost": 6, "heartbeatInterval": 120, "heartbeatTimeout": 10,
+                                         "resendLogin": 60}, "siteName": "", "siteId": None, "name": sn,
+                        "businessState": "0", "modelId": get_model_id(model), "model": model.upper(),
+                        "serialNumber": sn, "mac": mac.upper(), "mobileNumber": "", "plcId": 0,
+                        "config": {"timeout": "300000", "ackTimeout": "120000", "ackRetries": "3", "sync": "2"}}
+                self.api.send_request('api/devices', 'post', param={"create_site": 0}, body=body)
+                logging.info(f"the {sn} device add success")
+            else:
+                break
+
+    @loop_inspector('device online')
+    def assert_device_online(self, sn: str, timeout=120, interval=5) -> int:
+        """ 校验设备基本状态
+
+        :param sn: 序列号
+        :param timeout: 校验信息，最大超时时间
+        :param interval: 校验信息，校验间隔时间
+        :return: True or False
+        """
+        response = self.api.send_request('api/devices', method='get',
+                                         param={"verbose": 100, "limit": 10, "cursor": 0,
+                                                'serial_number': sn, 'plc_id': 0})
+        if response.json().get('total') == 1:
+            device_id = response.json().get('result')[0].get('_id')
+            response = self.api.send_request(f'api/devices/{device_id}', method='get', param={"verbose": 100}).json()
+            return response.get('result').get('online')
+        else:
+            return 0
+
+    def delete_device(self, sn):
+        response = self.api.send_request('api/devices', method='get',
+                                         param={"verbose": 100, "limit": 10, "cursor": 0,
+                                                'serial_number': sn, 'plc_id': 0}).json()
+        if response.get('total') == 1:
+            self.api.send_request(f'api/devices/{response.get("result")[0].get("_id")}', method='delete')
+            logging.info(f"the {sn} device delete success")
 
 
 class DmInterface:
 
     def __init__(self, username, password, host='iot.inhand.com.cn'):
         """
         :param username  平台用户名
@@ -97,15 +169,15 @@
 
     def add_device(self, sn: str) -> None:
         """添加设备，
 
         :param sn: 设备序列号
         :return:
         """
-        while True:
+        for i in range(5):
             response = self.api.send_request('api/devices', method='get',
                                              param={"verbose": 100, "limit": 10, "cursor": 0,
                                                     'serial_number': sn})
             if response.json().get('total') == 0:
                 self.api.send_request('api/devices', 'post',
                                       body={"name": sn + str(int(time.time())), "serialNumber": sn})
                 logging.info(f"the {sn} device add success")
@@ -200,20 +272,21 @@
         if response.json().get('total') == 1 and response.json().get('result')[0].get('online') == 1:
             device_id = response.json().get('result')[0].get('_id')
             device_name = response.json().get('result')[0].get('name')
             for i in range(0, 3):
                 try:
                     task_state = self.api.send_request('api2/tasks/run', 'post',
                                                        body={'name': "GET RUNNING CONFIG", 'objectId': device_id,
-                                                             'priority': 30, 'objectName': device_name, 'timeout': 30000,
+                                                             'priority': 30, 'objectName': device_name,
+                                                             'timeout': 30000,
                                                              'type': "4"}).json().get('result').get('state')
                     assert task_state == 3, "GET RUNNING CONFIG task status error!"
                     break
                 except Exception as e:
-                    logging.error(f'get running config task status reason is {e}, try {i+2} again')
+                    logging.error(f'get running config task status reason is {e}, try {i + 2} again')
             else:
                 raise Exception(f'device {sn} get running config task status failed')
             config_content = self.api.send_request(f'api/devices/{device_id}/config', 'get').json().get('result').get(
                 'content')
             if config:
                 assert set(config.split('\n')).issubset(set(config_content.split('\n'))), f'config {config} not exist'
         else:
@@ -643,15 +716,15 @@
     def add_device(self, sn: str, mac_or_imei: str) -> None:
         """添加设备，
 
         :param sn: 设备序列号
         :param mac_or_imei: 添加设备时需要依赖设备的mac地址或者IMEI号，去生产库查询该设备是否是映翰通设备
         :return:
         """
-        while True:
+        for i in range(5):
             validated_field = self.api.send_request(f'api/v1/serialnumber/{sn}/validate', method='post').json().get(
                 'result').get('validatedField')
             if not list(filter(lambda x: x.get('id'), self.device_state([sn]))):
                 self.api.send_request('api/v1/devices', 'post',
                                       body={"name": sn + str(int(time.time())), "serialNumber": sn, 'oid': self.me.oid,
                                             validated_field: mac_or_imei})
                 logging.info(f"the {sn} device add success")
@@ -720,15 +793,15 @@
 
     def __init__(self, host: str, username: str, password: str, type_='device', protocol='https', port=443):
         """支持设备，平台登录及操作API, 自动识别地址
 
         :param host:  主机地址，如果是平台的就填写平台server，如果是设备就填写设备的地址
         :param username:  用户名
         :param password: 密码
-        :param type_: device|iot|ics|star|iscada|iwos  区分平台和设备
+        :param type_: device|iot|ics|star|iscada|iwos|dn4  区分平台和设备
         :param protocol: 协议，当前只支持http https
         :param port: 端口
         """
         self.protocol = protocol
         self.host = host
         self.username = username
         self.password = password
@@ -745,15 +818,15 @@
         """
         if path.startswith('/'):
             return self.protocol + '://' + self.host + ':' + str(self.port) + path
         else:
             return self.protocol + '://' + self.host + ':' + str(self.port) + '/' + path
 
     def __login(self):
-        if self.type_ in ('iot', 'ics', 'iwos'):
+        if self.type_ in ('iot', 'ics', 'iwos', 'dn4'):
             self.headers = {"Content-Type": "application/x-www-form-urlencoded"}
             param = {
                 'client_id': '17953450251798098136',
                 'client_secret': '08E9EC6793345759456CB8BAE52615F3',
                 'grant_type': 'password',
                 'type': 'account',
                 'autoLogin': 'true',
@@ -885,16 +958,18 @@
             else:
                 raise ValueError('expect param type error！')
         return res
 
 
 if __name__ == "__main__":
     logging.basicConfig(format='%(asctime)s %(levelname)s %(message)s', level=logging.INFO, stream=sys.stdout)
-    testApi = StarInterface('liwei@inhand.com.cn', '123456', 'star.nezha.inhand.dev')
-    print(testApi.me.oid)
+    # testApi = StarInterface('liwei@inhand.com.cn', '123456', 'star.nezha.inhand.dev')
+    api = DnInterface('smoke@inhand.com.cn', 'smoke@inhand', 'c.inhand.com.cn', )
+    api.add_device('RL6152315576161', '00:18:05:29:12:AB', 'IR6XX_EVDO')
+    api.delete_device('RL6152315576161')
     # testApi.remote_maintenance_online('RF3052213006490', )
     # testApi.add_device({'RF3052213006490': 'IR305'})
     # print(testApi.web_remote_online('RF3052213006490'))
     # testApi.device_exist('VG7512022009918')
     # testApi.get_config_online('VG7512022009918', 'hello\r\nword')
     # testApi.send_config_online('VG7512022009918', 'hello\nword')
     # testApi.send_openvpn_config('RF3022206089272')
```

### Comparing `inhandtest-0.0.45/inhandtest/inserial.py` & `inhandtest-0.0.46/inhandtest/inserial.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.45/inhandtest/insocket.py` & `inhandtest-0.0.46/inhandtest/insocket.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.45/inhandtest/inssh.py` & `inhandtest-0.0.46/inhandtest/inssh.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.45/inhandtest/ip.py` & `inhandtest-0.0.46/inhandtest/ip.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.45/inhandtest/mail.py` & `inhandtest-0.0.46/inhandtest/mail.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.45/inhandtest/pytest_email.html` & `inhandtest-0.0.46/inhandtest/pytest_email.html`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.45/inhandtest/telnet.py` & `inhandtest-0.0.46/inhandtest/telnet.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.45/inhandtest/tools.py` & `inhandtest-0.0.46/inhandtest/tools.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.45/setup.py` & `inhandtest-0.0.46/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 setup
 
 """
 from distutils.core import setup
 
 setup(
     name='inhandtest',
-    version='0.0.45',
+    version='0.0.46',
     author='liwei',
     author_email='liwei@inhand.com.cn',
     description='inhand test tools, so easy',
     maintainer='liwei',
     maintainer_email='liwei@inhand.com.cn',
     # py_modules=['inhandtest.tools', 'inhandtest.telnet', 'inhandtest.inmodbus', 'inhandtest.inmqtt', 'inhandtest.file',
     #             'inhandtest.inrequest', 'inhandtest.inssh', 'inhandtest.base_page'],
```

