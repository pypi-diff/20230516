# Comparing `tmp/licensespring-1.1.0.tar.gz` & `tmp/licensespring-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "licensespring-1.1.0.tar", max compression
+gzip compressed data, was "licensespring-1.2.0.tar", max compression
```

## Comparing `licensespring-1.1.0.tar` & `licensespring-1.2.0.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0    10869 2023-01-09 09:54:18.776091 licensespring-1.1.0/README.md
--rw-r--r--   0        0        0       37 2023-01-09 09:54:18.776567 licensespring-1.1.0/licensespring/__init__.py
--rw-r--r--   0        0        0    19949 2022-10-05 12:56:34.391176 licensespring-1.1.0/licensespring/api/__init__.py
--rw-r--r--   0        0        0     1198 2022-05-17 10:49:16.697569 licensespring-1.1.0/licensespring/api/authorization.py
--rw-r--r--   0        0        0      625 2022-05-17 10:49:16.698411 licensespring-1.1.0/licensespring/api/error.py
--rw-r--r--   0        0        0     2281 2023-01-09 09:54:18.777032 licensespring-1.1.0/licensespring/api/hardware.py
--rw-r--r--   0        0        0     1896 2022-10-28 11:45:15.353905 licensespring-1.1.0/licensespring/api/signature.py
--rw-r--r--   0        0        0      584 2023-01-09 09:54:18.778492 licensespring-1.1.0/pyproject.toml
--rw-r--r--   0        0        0    12091 2023-01-09 09:54:33.631662 licensespring-1.1.0/setup.py
--rw-r--r--   0        0        0    11515 2023-01-09 09:54:33.632278 licensespring-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    10869 2023-04-20 06:25:19.556083 licensespring-1.2.0/README.md
+-rw-r--r--   0        0        0       37 2023-05-16 07:57:47.673219 licensespring-1.2.0/licensespring/__init__.py
+-rw-r--r--   0        0        0    20560 2023-05-16 07:57:47.673219 licensespring-1.2.0/licensespring/api/__init__.py
+-rw-r--r--   0        0        0     1198 2023-04-20 06:25:19.556083 licensespring-1.2.0/licensespring/api/authorization.py
+-rw-r--r--   0        0        0      625 2023-04-20 06:25:19.556083 licensespring-1.2.0/licensespring/api/error.py
+-rw-r--r--   0        0        0     2281 2023-04-20 06:25:19.556083 licensespring-1.2.0/licensespring/api/hardware.py
+-rw-r--r--   0        0        0     1896 2023-04-20 06:25:19.556083 licensespring-1.2.0/licensespring/api/signature.py
+-rw-r--r--   0        0        0      584 2023-05-16 07:57:47.673219 licensespring-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0    11566 1970-01-01 00:00:00.000000 licensespring-1.2.0/PKG-INFO
```

### Comparing `licensespring-1.1.0/README.md` & `licensespring-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `licensespring-1.1.0/licensespring/api/__init__.py` & `licensespring-1.2.0/licensespring/api/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,14 +63,26 @@
         if username:
             data["username"] = username
         if password:
             data["password"] = password
 
         return data
 
+    def request_sso_data(
+        self, data, customer_account_code=None, id_token=None, code=None
+    ):
+        if customer_account_code:
+            data["customer_account_code"] = customer_account_code
+            if code:
+                data["code"] = code
+            elif id_token:
+                data["id_token"] = id_token
+
+        return data
+
     def request_additional_data(self, data, additional_data):
         for key, value in additional_data.items():
             if value is not None:
                 data[key] = value
         return data
 
     def request_hardware_data(
@@ -145,25 +157,34 @@
     def activate_license(
         self,
         product,
         hardware_id=None,
         license_key=None,
         username=None,
         password=None,
+        customer_account_code=None,
+        id_token=None,
+        code=None,
         app_ver=None,
         os_ver=None,
         hostname=None,
         ip=None,
         is_vm=None,
         vm_info=None,
         mac_address=None,
     ):
         data = self.request_generic_data(
             {}, product, hardware_id, license_key, username, password
         )
+        data = self.request_sso_data(
+            data,
+            customer_account_code=customer_account_code,
+            id_token=id_token,
+            code=code,
+        )
         data = self.request_hardware_data(
             data=data,
             os_ver=os_ver,
             hostname=hostname,
             ip=ip,
             mac_address=mac_address,
         )
```

### Comparing `licensespring-1.1.0/licensespring/api/authorization.py` & `licensespring-1.2.0/licensespring/api/authorization.py`

 * *Files identical despite different names*

### Comparing `licensespring-1.1.0/licensespring/api/error.py` & `licensespring-1.2.0/licensespring/api/error.py`

 * *Files identical despite different names*

### Comparing `licensespring-1.1.0/licensespring/api/hardware.py` & `licensespring-1.2.0/licensespring/api/hardware.py`

 * *Files identical despite different names*

### Comparing `licensespring-1.1.0/licensespring/api/signature.py` & `licensespring-1.2.0/licensespring/api/signature.py`

 * *Files identical despite different names*

### Comparing `licensespring-1.1.0/pyproject.toml` & `licensespring-1.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "licensespring"
-version = "1.1.0"
+version = "1.2.0"
 description = "LicenseSpring Python Library"
 authors = ["Toni Sredanović <toni@licensespring.com>"]
 readme = "README.md"
 homepage = "https://licensespring.com/"
 
 [tool.poetry.dependencies]
 python = "^3.7"
```

### Comparing `licensespring-1.1.0/setup.py` & `licensespring-1.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,450 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: licensespring
+Version: 1.2.0
+Summary: LicenseSpring Python Library
+Home-page: https://licensespring.com/
+Author: Toni Sredanović
+Author-email: toni@licensespring.com
+Requires-Python: >=3.7,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: pycryptodome (>=3.14.1,<4.0.0)
+Requires-Dist: requests (>=2.27.1,<3.0.0)
+Requires-Dist: winregistry (>=1.1.1,<2.0.0)
+Description-Content-Type: text/markdown
 
-packages = \
-['licensespring', 'licensespring.api']
+# LicenseSpring Python Library
 
-package_data = \
-{'': ['*']}
+The LicenseSpring Python Library provides convenient access to the LicenseSpring API from
+applications written in the Python language.
 
-install_requires = \
-['pycryptodome>=3.14.1,<4.0.0',
- 'requests>=2.27.1,<3.0.0',
- 'winregistry>=1.1.1,<2.0.0']
-
-setup_kwargs = {
-    'name': 'licensespring',
-    'version': '1.1.0',
-    'description': 'LicenseSpring Python Library',
-    'long_description': '# LicenseSpring Python Library\n\nThe LicenseSpring Python Library provides convenient access to the LicenseSpring API from\napplications written in the Python language.\n\n## Installation\n\nInstall `licensespring` library:\n\n```\npip install licensespring\n```\n\nRequires: Python >=3.7\n\n## Hardware (Device) IDs\n\nThis library provides preconfigured hardware identity providers:\n- `HardwareIdProvider` (default)\n- `PlatformIdProvider`\n\nYou can set the desired hardware identity provider when initializing the APIClient:\n```python\napi_client = APIClient(api_key="_your_api_key_", shared_key="_your_shared_key_", hardware_id_provider=PlatformIdProvider)\n```\n\nIt also supports their customization and creation of your own hardware id provider.\n\n### HardwareIdProvider\n\n Uses [uuid.getnode()](https://docs.python.org/3/library/uuid.html#uuid.getnode) to generate unique ID per device as described:\n\n> Get the hardware address as a 48-bit positive integer. The first time this runs, it may launch a separate program, which could be quite slow. If all attempts to obtain the hardware address fail, we choose a random 48-bit number with the multicast bit (least significant bit of the first octet) set to 1 as recommended in RFC 4122. “Hardware address” means the MAC address of a network interface. On a machine with multiple network interfaces, universally administered MAC addresses (i.e. where the second least significant bit of the first octet is unset) will be preferred over locally administered MAC addresses, but with no other ordering guarantees.\n\nAll of the methods exposed by `HardwareIdProvider`:\n```python\nclass HardwareIdProvider:\n    def get_id(self):\n        return str(uuid.getnode())\n\n    def get_os_ver(self):\n        return platform.platform()\n\n    def get_hostname(self):\n        return platform.node()\n\n    def get_ip(self):\n        return socket.gethostbyname(self.get_hostname())\n\n    def get_is_vm(self):\n        return False\n\n    def get_vm_info(self):\n        return None\n\n    def get_mac_address(self):\n        return ":".join(("%012X" % uuid.getnode())[i : i + 2] for i in range(0, 12, 2))\n\n    def get_request_id(self):\n        return str(uuid.uuid4())\n```\n\n### PlatformIdProvider\n\nUses [sys.platform](https://docs.python.org/3/library/sys.html#sys.platform) and OS queries to find the raw GUID of the device.\n\nExtends the `HardwareIdProvider` and overwrites only the `get_id` method:\n```python\nclass PlatformIdProvider(HardwareIdProvider):\n    def get_id(self):\n        id = None\n\n        if sys.platform == \'darwin\':\n            id = execute("ioreg -d2 -c IOPlatformExpertDevice | awk -F\\\\\\" \'/IOPlatformUUID/{print $(NF-1)}\'")\n\n        if sys.platform == \'win32\' or sys.platform == \'cygwin\' or sys.platform == \'msys\':\n            id = read_win_registry(\'HKEY_LOCAL_MACHINE\\\\SOFTWARE\\\\Microsoft\\\\Cryptography\', \'MachineGuid\')\n            if not id:\n                id = execute(\'wmic csproduct get uuid\').split(\'\\n\')[2].strip()\n\n        if sys.platform.startswith(\'linux\'):\n            id = read_file(\'/var/lib/dbus/machine-id\')\n            if not id:\n                id = read_file(\'/etc/machine-id\')\n\n        if sys.platform.startswith(\'openbsd\') or sys.platform.startswith(\'freebsd\'):\n            id = read_file(\'/etc/hostid\')\n            if not id:\n                id = execute(\'kenv -q smbios.system.uuid\')\n\n        if not id:\n            id = super().get_id()\n\n        return id\n```\n\n### Customization\n\nExtend any of the preconfigured hardware identity providers, overwrite the methods you want and provide it when initializing the APIClient:\n```python\nclass CustomHardwareIdProvider(HardwareIdProvider):\n    def get_id(self):\n        return "_my_id_"\n\napi_client = APIClient(api_key="_your_api_key_", shared_key="_your_shared_key_", hardware_id_provider=CustomHardwareIdProvider)\n```\n\n## APIClient Usage Examples\n\n### Set app version\n```python\nimport licensespring\n\nlicensespring.app_version = "MyApp 1.0.0"\n```\n\n### Create APIClient\n```python\nfrom licensespring.api import APIClient\n\napi_client = APIClient(api_key="_your_api_key_", shared_key="_your_shared_key_")\n```\n\n### Activate key based license\n```python\nproduct = "lkprod1"\nlicense_key = "GPB7-279T-6MNK-CQLK"\nlicense_data = api_client.activate_license(product=product, license_key=license_key)\n\nprint(license_data)\n```\n\n### Activate user based license\n```python\nproduct = "uprod1"\nusername = "user1@email.com"\npassword = "nq64k1!@"\n\nlicense_data = api_client.activate_license(\n    product=product, username=username, password=password\n)\n\nprint(license_data)\n```\n\n### Deactivate key based license\n```python\nproduct = "lkprod1"\nlicense_key = "GPUB-J4PH-CGNK-C7LK"\nis_deactivated = api_client.deactivate_license(product=product, license_key=license_key)\n\nprint(is_deactivated)\n```\n\n### Deactivate user based license\n```python\nproduct = "uprod1"\nusername = "user1@email.com"\npassword = "nq64k1!@"\n\nlicense_data = api_client.deactivate_license(\n    product=product, username=username, password=password\n)\n\nprint(license_data)\n```\n\n### Check key based license\n```python\nproduct = "lkprod1"\nlicense_key = "GPBQ-DZCP-E9SK-CQLK"\n\nlicense_data = api_client.check_license(product=product, license_key=license_key)\n\nprint(license_data)\n```\n\n### Check user based license\n```python\nproduct = "uprod1"\nusername = "user2@email.com"\npassword = "1l48y#!b"\n\nlicense_data = api_client.check_license(product=product, username=username)\n\nprint(license_data)\n```\n\n### Add consumption\n```python\nproduct = "lkprod1"\nlicense_key = "GPSU-QTKQ-HSSK-C9LK"\n\n# Add 1 consumption\nconsumption_data = api_client.add_consumption(\n    product=product, license_key=license_key\n)\n\n# Add 3 consumptions\nconsumption_data = api_client.add_consumption(\n    product=product, license_key=license_key, consumptions=3\n)\n\n# Add 1 consumption, allow overages and define max overages\nconsumption_data = api_client.add_consumption(\n    product=product, license_key=license_key, allow_overages=True, max_overages=10\n)\n\nprint(consumption_data)\n```\n\n### Add feature consumption\n```python\nproduct = "lkprod1"\nlicense_key = "GPTJ-LSYZ-USEK-C8LK"\nfeature = "lkprod1cf1"\n\n# Add 1 consumption\nfeature_consumption_data = api_client.add_feature_consumption(\n    product=product, license_key=license_key, feature=feature\n)\n\n# Add 3 consumptions\nfeature_consumption_data = api_client.add_feature_consumption(\n    product=product, license_key=license_key, feature=feature, consumptions=3\n)\n\nprint(feature_consumption_data)\n```\n\n### Trial key\n```python\nproduct = "lkprod2"\n\ntrial_license_data = api_client.trial_key(product=product)\n\nprint(trial_license_data)\n```\n\n### Product details\n```python\nproduct = "lkprod1"\n\nproduct_data = api_client.product_details(product=product)\n\nprint(product_data)\n```\n\n### Track device variables\n```python\nproduct = "lkprod1"\nlicense_key = "GPUB-SZF9-AB2K-C7LK"\nvariables = {"variable_1_key": "variable_1_value", "variable_2_key": "variable_2_value"}\n\nis_tracked = api_client.track_device_variables(product=product, license_key=license_key, variables=variables)\n\nprint(is_tracked)\n```\n\n### Get device variables\n```python\nproduct = "lkprod1"\nlicense_key = "GPUB-SZF9-AB2K-C7LK"\n\ndevice_variables = api_client.get_device_variables(product=product, license_key=license_key)\n\nprint(device_variables)\n```\n\n### Floating borrow\n```python\nproduct = "lkprod1"\nlicense_key = "GPUC-NGWU-3NJK-C7LK"\n\n# Borrow for 2 hours\nborrowed_until = (datetime.utcnow() + timedelta(hours=2)).isoformat()\nfloating_borrow_data = api_client.floating_borrow(product=product, license_key=license_key, borrowed_until=borrowed_until)\n\nprint(floating_borrow_data)\n```\n\n### Floating release\n```python\nproduct = "lkprod1"\nlicense_key = "GPUC-NGWU-3NJK-C7LK"\n\nis_released = api_client.floating_release(product=product, license_key=license_key)\n\nprint(is_released)\n```\n\n### Change password\n```python\nusername = "user4@email.com"\npassword = "_old_password_"\nnew_password = "_new_password_"\n\nis_password_changed = api_client.change_password(username=username, password=password, new_password=new_password)\n\nprint(is_password_changed)\n```\n\n### Versions\n```python\nproduct = "lkprod1"\nlicense_key = "GPB7-279T-6MNK-CQLK"\n\n# Get versions for all environments\nversions_data = api_client.versions(product=product, license_key=license_key)\n\n# Get versions for mac environment\nmac_versions_data = api_client.versions(\n    product=product, license_key=license_key, env="mac"\n)\n\nprint(versions_data)\n```\n\n### Installation file\n```python\nproduct = "lkprod1"\nlicense_key = "GPB7-279T-6MNK-CQLK"\n\n# Get the latest installation file\ninstallation_file_data = api_client.installation_file(\n    product=product, license_key=license_key\n)\n\n# Get the latest installation file for linux environment\ninstallation_file_data = api_client.installation_file(\n    product=product, license_key=license_key, env="linux"\n)\n\n# Get the latest installation file for version 1.0.0\ninstallation_file_data = api_client.installation_file(\n    product=product, license_key=license_key, version="1.0.0"\n)\n\nprint(installation_file_data)\n```\n\n### Customer license users\n```python\nproduct = "uprod1"\ncustomer = \'c1@c.com\'\n\ncustomer_license_users_data = api_client.customer_license_users(\n    product=product, customer=customer\n)\n\nprint(customer_license_users_data)\n```\n\n### SSO URL\n```python\nproduct = "uprod1"\ncustomer_account_code = "ccorp"\n\nsso_url_data = api_client.sso_url(\n    product=product, customer_account_code=customer_account_code\n)\n\nprint(sso_url_data)\n```\n\n\n### SSO URL with `code` response type\n```python\nproduct = "uprod1"\ncustomer_account_code = "ccorp"\n\nsso_url_data = api_client.sso_url(\n    product=product,\n    customer_account_code=customer_account_code,\n    response_type="code",\n)\n\nprint(sso_url_data)\n```\n\n### Activate offline\n```python\nproduct = "lkprod1"\nlicense_key = "GPY7-VHX9-MDSK-C3LK"\n\n# Generate data for offline activation\nactivate_offline_data = api_client.activate_offline_dump(\n    product=product, license_key=license_key\n)\n\n# Write to file\nwith open(\'activate_offline.req\', mode=\'w\') as f:\n    print(activate_offline_data, file=f)\n\n# Activate offline\nlicense_data = api_client.activate_offline(data=activate_offline_data)\n\nprint(license_data)\n```\n\n### Activate offline load\n```python\n# Read from file\nwith open(\'./ls_activation.lic\') as file:\n    ls_activation_data = file.read()\n\nlicense_data = api_client.activate_offline_load(ls_activation_data)\n\nprint(license_data)\n```\n\n### Deactivate offline\n```python\nproduct = "lkprod1"\nlicense_key = "GPYC-X5J2-L5SK-C3LK"\n\n# Generate data for offline deactivation\ndeactivate_offline_data = api_client.deactivate_offline_dump(\n    product=product, license_key=license_key\n)\n\n# Write to file\nwith open(\'deactivate_offline.req\', mode=\'w\') as f:\n    print(deactivate_offline_data, file=f)\n\n# Deactivate offline\nis_deactivated = api_client.deactivate_offline(data=deactivate_offline_data)\n\nprint(is_deactiavted)\n```\n',
-    'author': 'Toni Sredanović',
-    'author_email': 'toni@licensespring.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://licensespring.com/',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
-}
+## Installation
 
+Install `licensespring` library:
+
+```
+pip install licensespring
+```
+
+Requires: Python >=3.7
+
+## Hardware (Device) IDs
+
+This library provides preconfigured hardware identity providers:
+- `HardwareIdProvider` (default)
+- `PlatformIdProvider`
+
+You can set the desired hardware identity provider when initializing the APIClient:
+```python
+api_client = APIClient(api_key="_your_api_key_", shared_key="_your_shared_key_", hardware_id_provider=PlatformIdProvider)
+```
+
+It also supports their customization and creation of your own hardware id provider.
+
+### HardwareIdProvider
+
+ Uses [uuid.getnode()](https://docs.python.org/3/library/uuid.html#uuid.getnode) to generate unique ID per device as described:
+
+> Get the hardware address as a 48-bit positive integer. The first time this runs, it may launch a separate program, which could be quite slow. If all attempts to obtain the hardware address fail, we choose a random 48-bit number with the multicast bit (least significant bit of the first octet) set to 1 as recommended in RFC 4122. “Hardware address” means the MAC address of a network interface. On a machine with multiple network interfaces, universally administered MAC addresses (i.e. where the second least significant bit of the first octet is unset) will be preferred over locally administered MAC addresses, but with no other ordering guarantees.
+
+All of the methods exposed by `HardwareIdProvider`:
+```python
+class HardwareIdProvider:
+    def get_id(self):
+        return str(uuid.getnode())
+
+    def get_os_ver(self):
+        return platform.platform()
+
+    def get_hostname(self):
+        return platform.node()
+
+    def get_ip(self):
+        return socket.gethostbyname(self.get_hostname())
+
+    def get_is_vm(self):
+        return False
+
+    def get_vm_info(self):
+        return None
+
+    def get_mac_address(self):
+        return ":".join(("%012X" % uuid.getnode())[i : i + 2] for i in range(0, 12, 2))
+
+    def get_request_id(self):
+        return str(uuid.uuid4())
+```
+
+### PlatformIdProvider
+
+Uses [sys.platform](https://docs.python.org/3/library/sys.html#sys.platform) and OS queries to find the raw GUID of the device.
+
+Extends the `HardwareIdProvider` and overwrites only the `get_id` method:
+```python
+class PlatformIdProvider(HardwareIdProvider):
+    def get_id(self):
+        id = None
+
+        if sys.platform == 'darwin':
+            id = execute("ioreg -d2 -c IOPlatformExpertDevice | awk -F\\\" '/IOPlatformUUID/{print $(NF-1)}'")
+
+        if sys.platform == 'win32' or sys.platform == 'cygwin' or sys.platform == 'msys':
+            id = read_win_registry('HKEY_LOCAL_MACHINE\\SOFTWARE\\Microsoft\\Cryptography', 'MachineGuid')
+            if not id:
+                id = execute('wmic csproduct get uuid').split('\n')[2].strip()
+
+        if sys.platform.startswith('linux'):
+            id = read_file('/var/lib/dbus/machine-id')
+            if not id:
+                id = read_file('/etc/machine-id')
+
+        if sys.platform.startswith('openbsd') or sys.platform.startswith('freebsd'):
+            id = read_file('/etc/hostid')
+            if not id:
+                id = execute('kenv -q smbios.system.uuid')
+
+        if not id:
+            id = super().get_id()
+
+        return id
+```
+
+### Customization
+
+Extend any of the preconfigured hardware identity providers, overwrite the methods you want and provide it when initializing the APIClient:
+```python
+class CustomHardwareIdProvider(HardwareIdProvider):
+    def get_id(self):
+        return "_my_id_"
+
+api_client = APIClient(api_key="_your_api_key_", shared_key="_your_shared_key_", hardware_id_provider=CustomHardwareIdProvider)
+```
+
+## APIClient Usage Examples
+
+### Set app version
+```python
+import licensespring
+
+licensespring.app_version = "MyApp 1.0.0"
+```
+
+### Create APIClient
+```python
+from licensespring.api import APIClient
+
+api_client = APIClient(api_key="_your_api_key_", shared_key="_your_shared_key_")
+```
+
+### Activate key based license
+```python
+product = "lkprod1"
+license_key = "GPB7-279T-6MNK-CQLK"
+license_data = api_client.activate_license(product=product, license_key=license_key)
+
+print(license_data)
+```
+
+### Activate user based license
+```python
+product = "uprod1"
+username = "user1@email.com"
+password = "nq64k1!@"
+
+license_data = api_client.activate_license(
+    product=product, username=username, password=password
+)
+
+print(license_data)
+```
+
+### Deactivate key based license
+```python
+product = "lkprod1"
+license_key = "GPUB-J4PH-CGNK-C7LK"
+is_deactivated = api_client.deactivate_license(product=product, license_key=license_key)
+
+print(is_deactivated)
+```
+
+### Deactivate user based license
+```python
+product = "uprod1"
+username = "user1@email.com"
+password = "nq64k1!@"
+
+license_data = api_client.deactivate_license(
+    product=product, username=username, password=password
+)
+
+print(license_data)
+```
+
+### Check key based license
+```python
+product = "lkprod1"
+license_key = "GPBQ-DZCP-E9SK-CQLK"
+
+license_data = api_client.check_license(product=product, license_key=license_key)
+
+print(license_data)
+```
+
+### Check user based license
+```python
+product = "uprod1"
+username = "user2@email.com"
+password = "1l48y#!b"
+
+license_data = api_client.check_license(product=product, username=username)
+
+print(license_data)
+```
+
+### Add consumption
+```python
+product = "lkprod1"
+license_key = "GPSU-QTKQ-HSSK-C9LK"
+
+# Add 1 consumption
+consumption_data = api_client.add_consumption(
+    product=product, license_key=license_key
+)
+
+# Add 3 consumptions
+consumption_data = api_client.add_consumption(
+    product=product, license_key=license_key, consumptions=3
+)
+
+# Add 1 consumption, allow overages and define max overages
+consumption_data = api_client.add_consumption(
+    product=product, license_key=license_key, allow_overages=True, max_overages=10
+)
+
+print(consumption_data)
+```
+
+### Add feature consumption
+```python
+product = "lkprod1"
+license_key = "GPTJ-LSYZ-USEK-C8LK"
+feature = "lkprod1cf1"
+
+# Add 1 consumption
+feature_consumption_data = api_client.add_feature_consumption(
+    product=product, license_key=license_key, feature=feature
+)
+
+# Add 3 consumptions
+feature_consumption_data = api_client.add_feature_consumption(
+    product=product, license_key=license_key, feature=feature, consumptions=3
+)
+
+print(feature_consumption_data)
+```
+
+### Trial key
+```python
+product = "lkprod2"
+
+trial_license_data = api_client.trial_key(product=product)
+
+print(trial_license_data)
+```
+
+### Product details
+```python
+product = "lkprod1"
+
+product_data = api_client.product_details(product=product)
+
+print(product_data)
+```
+
+### Track device variables
+```python
+product = "lkprod1"
+license_key = "GPUB-SZF9-AB2K-C7LK"
+variables = {"variable_1_key": "variable_1_value", "variable_2_key": "variable_2_value"}
+
+is_tracked = api_client.track_device_variables(product=product, license_key=license_key, variables=variables)
+
+print(is_tracked)
+```
+
+### Get device variables
+```python
+product = "lkprod1"
+license_key = "GPUB-SZF9-AB2K-C7LK"
+
+device_variables = api_client.get_device_variables(product=product, license_key=license_key)
+
+print(device_variables)
+```
+
+### Floating borrow
+```python
+product = "lkprod1"
+license_key = "GPUC-NGWU-3NJK-C7LK"
+
+# Borrow for 2 hours
+borrowed_until = (datetime.utcnow() + timedelta(hours=2)).isoformat()
+floating_borrow_data = api_client.floating_borrow(product=product, license_key=license_key, borrowed_until=borrowed_until)
+
+print(floating_borrow_data)
+```
+
+### Floating release
+```python
+product = "lkprod1"
+license_key = "GPUC-NGWU-3NJK-C7LK"
+
+is_released = api_client.floating_release(product=product, license_key=license_key)
+
+print(is_released)
+```
+
+### Change password
+```python
+username = "user4@email.com"
+password = "_old_password_"
+new_password = "_new_password_"
+
+is_password_changed = api_client.change_password(username=username, password=password, new_password=new_password)
+
+print(is_password_changed)
+```
+
+### Versions
+```python
+product = "lkprod1"
+license_key = "GPB7-279T-6MNK-CQLK"
+
+# Get versions for all environments
+versions_data = api_client.versions(product=product, license_key=license_key)
+
+# Get versions for mac environment
+mac_versions_data = api_client.versions(
+    product=product, license_key=license_key, env="mac"
+)
+
+print(versions_data)
+```
+
+### Installation file
+```python
+product = "lkprod1"
+license_key = "GPB7-279T-6MNK-CQLK"
+
+# Get the latest installation file
+installation_file_data = api_client.installation_file(
+    product=product, license_key=license_key
+)
+
+# Get the latest installation file for linux environment
+installation_file_data = api_client.installation_file(
+    product=product, license_key=license_key, env="linux"
+)
+
+# Get the latest installation file for version 1.0.0
+installation_file_data = api_client.installation_file(
+    product=product, license_key=license_key, version="1.0.0"
+)
+
+print(installation_file_data)
+```
+
+### Customer license users
+```python
+product = "uprod1"
+customer = 'c1@c.com'
+
+customer_license_users_data = api_client.customer_license_users(
+    product=product, customer=customer
+)
+
+print(customer_license_users_data)
+```
+
+### SSO URL
+```python
+product = "uprod1"
+customer_account_code = "ccorp"
+
+sso_url_data = api_client.sso_url(
+    product=product, customer_account_code=customer_account_code
+)
+
+print(sso_url_data)
+```
+
+
+### SSO URL with `code` response type
+```python
+product = "uprod1"
+customer_account_code = "ccorp"
+
+sso_url_data = api_client.sso_url(
+    product=product,
+    customer_account_code=customer_account_code,
+    response_type="code",
+)
+
+print(sso_url_data)
+```
+
+### Activate offline
+```python
+product = "lkprod1"
+license_key = "GPY7-VHX9-MDSK-C3LK"
+
+# Generate data for offline activation
+activate_offline_data = api_client.activate_offline_dump(
+    product=product, license_key=license_key
+)
+
+# Write to file
+with open('activate_offline.req', mode='w') as f:
+    print(activate_offline_data, file=f)
+
+# Activate offline
+license_data = api_client.activate_offline(data=activate_offline_data)
+
+print(license_data)
+```
+
+### Activate offline load
+```python
+# Read from file
+with open('./ls_activation.lic') as file:
+    ls_activation_data = file.read()
+
+license_data = api_client.activate_offline_load(ls_activation_data)
+
+print(license_data)
+```
+
+### Deactivate offline
+```python
+product = "lkprod1"
+license_key = "GPYC-X5J2-L5SK-C3LK"
+
+# Generate data for offline deactivation
+deactivate_offline_data = api_client.deactivate_offline_dump(
+    product=product, license_key=license_key
+)
+
+# Write to file
+with open('deactivate_offline.req', mode='w') as f:
+    print(deactivate_offline_data, file=f)
+
+# Deactivate offline
+is_deactivated = api_client.deactivate_offline(data=deactivate_offline_data)
+
+print(is_deactiavted)
+```
 
-setup(**setup_kwargs)
```

