# Comparing `tmp/certbot-dns-azure-2.1.0.tar.gz` & `tmp/certbot-dns-azure-2.2.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "certbot-dns-azure-2.1.0.tar", last modified: Sun Mar  5 13:12:05 2023, max compression
+gzip compressed data, was "certbot-dns-azure-2.2.0b0.tar", last modified: Tue May 16 20:29:37 2023, max compression
```

## Comparing `certbot-dns-azure-2.1.0.tar` & `certbot-dns-azure-2.2.0b0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 13:12:05.177049 certbot-dns-azure-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    10786 2023-03-05 13:12:01.000000 certbot-dns-azure-2.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-03-05 13:12:01.000000 certbot-dns-azure-2.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-03-05 13:12:05.177049 certbot-dns-azure-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-03-05 13:12:01.000000 certbot-dns-azure-2.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 13:12:05.173049 certbot-dns-azure-2.1.0/certbot_dns_azure/
--rw-r--r--   0 runner    (1001) docker     (123)     6092 2023-03-05 13:12:01.000000 certbot-dns-azure-2.1.0/certbot_dns_azure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 13:12:05.177049 certbot-dns-azure-2.1.0/certbot_dns_azure/_internal/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-03-05 13:12:01.000000 certbot-dns-azure-2.1.0/certbot_dns_azure/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12215 2023-03-05 13:12:01.000000 certbot-dns-azure-2.1.0/certbot_dns_azure/_internal/dns_azure.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 13:12:05.173049 certbot-dns-azure-2.1.0/certbot_dns_azure.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-03-05 13:12:05.000000 certbot-dns-azure-2.1.0/certbot_dns_azure.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-03-05 13:12:05.000000 certbot-dns-azure-2.1.0/certbot_dns_azure.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-05 13:12:05.000000 certbot-dns-azure-2.1.0/certbot_dns_azure.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-05 13:12:05.000000 certbot-dns-azure-2.1.0/certbot_dns_azure.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-03-05 13:12:05.000000 certbot-dns-azure-2.1.0/certbot_dns_azure.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-05 13:12:05.000000 certbot-dns-azure-2.1.0/certbot_dns_azure.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 13:12:05.177049 certbot-dns-azure-2.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-05 13:12:01.000000 certbot-dns-azure-2.1.0/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-03-05 13:12:01.000000 certbot-dns-azure-2.1.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-03-05 13:12:01.000000 certbot-dns-azure-2.1.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5778 2023-03-05 13:12:01.000000 certbot-dns-azure-2.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-03-05 13:12:01.000000 certbot-dns-azure-2.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-03-05 13:12:01.000000 certbot-dns-azure-2.1.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-05 13:12:01.000000 certbot-dns-azure-2.1.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-05 13:12:05.177049 certbot-dns-azure-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-03-05 13:12:01.000000 certbot-dns-azure-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 13:12:05.177049 certbot-dns-azure-2.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    13430 2023-03-05 13:12:01.000000 certbot-dns-azure-2.1.0/tests/dns_azure_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:29:37.536460 certbot-dns-azure-2.2.0b0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10786 2023-05-16 20:29:34.000000 certbot-dns-azure-2.2.0b0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-16 20:29:34.000000 certbot-dns-azure-2.2.0b0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-05-16 20:29:37.536460 certbot-dns-azure-2.2.0b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-16 20:29:34.000000 certbot-dns-azure-2.2.0b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:29:37.532460 certbot-dns-azure-2.2.0b0/certbot_dns_azure/
+-rw-r--r--   0 runner    (1001) docker     (123)    10735 2023-05-16 20:29:34.000000 certbot-dns-azure-2.2.0b0/certbot_dns_azure/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:29:37.532460 certbot-dns-azure-2.2.0b0/certbot_dns_azure/_internal/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-16 20:29:34.000000 certbot-dns-azure-2.2.0b0/certbot_dns_azure/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15391 2023-05-16 20:29:34.000000 certbot-dns-azure-2.2.0b0/certbot_dns_azure/_internal/dns_azure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:29:37.532460 certbot-dns-azure-2.2.0b0/certbot_dns_azure.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-05-16 20:29:37.000000 certbot-dns-azure-2.2.0b0/certbot_dns_azure.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-16 20:29:37.000000 certbot-dns-azure-2.2.0b0/certbot_dns_azure.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 20:29:37.000000 certbot-dns-azure-2.2.0b0/certbot_dns_azure.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-16 20:29:37.000000 certbot-dns-azure-2.2.0b0/certbot_dns_azure.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-16 20:29:37.000000 certbot-dns-azure-2.2.0b0/certbot_dns_azure.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-16 20:29:37.000000 certbot-dns-azure-2.2.0b0/certbot_dns_azure.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:29:37.532460 certbot-dns-azure-2.2.0b0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-16 20:29:34.000000 certbot-dns-azure-2.2.0b0/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-16 20:29:34.000000 certbot-dns-azure-2.2.0b0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-16 20:29:34.000000 certbot-dns-azure-2.2.0b0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5778 2023-05-16 20:29:34.000000 certbot-dns-azure-2.2.0b0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-16 20:29:34.000000 certbot-dns-azure-2.2.0b0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-16 20:29:34.000000 certbot-dns-azure-2.2.0b0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-16 20:29:34.000000 certbot-dns-azure-2.2.0b0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-16 20:29:37.536460 certbot-dns-azure-2.2.0b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-05-16 20:29:34.000000 certbot-dns-azure-2.2.0b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:29:37.532460 certbot-dns-azure-2.2.0b0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    15566 2023-05-16 20:29:34.000000 certbot-dns-azure-2.2.0b0/tests/dns_azure_test.py
```

### Comparing `certbot-dns-azure-2.1.0/LICENSE.txt` & `certbot-dns-azure-2.2.0b0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `certbot-dns-azure-2.1.0/PKG-INFO` & `certbot-dns-azure-2.2.0b0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: certbot-dns-azure
-Version: 2.1.0
+Version: 2.2.0b0
 Summary: Azure DNS Authenticator plugin for Certbot
 Home-page: https://github.com/binkhq/certbot-dns-azure
 Author: Terry Cain
 Author-email: opensource@bink.com
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Security
 Classifier: Topic :: System :: Installation/Setup
 Classifier: Topic :: System :: Networking
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6
@@ -30,15 +31,15 @@
 
 # certbot-dns-azure
 
 [![Tests](https://github.com/binkhq/certbot-dns-azure/workflows/Release/badge.svg)](https://github.com/binkhq/certbot-dns-azure/actions)
 [![Python Version](https://img.shields.io/pypi/pyversions/certbot-dns-azure)](https://pypi.org/project/certbot-dns-azure/)
 [![PyPi Status](https://img.shields.io/pypi/status/certbot-dns-azure)](https://pypi.org/project/certbot-dns-azure/)
 [![Version](https://img.shields.io/pypi/v/certbot-dns-azure)](https://pypi.org/project/certbot-dns-azure/)
-[![Docs](https://readthedocs.org/projects/certbot-dns-azure/badge/?version=latest&style=flat)](https://certbot-dns-azure.readthedocs.io/en/latest/)
+[![Docs](https://readthedocs.org/projects/certbot-dns-azure/badge/?version=latest&style=flat)](https://docs.certbot-dns-azure.co.uk/en/latest/)
 
 AzureDNS Authenticator plugin for [Certbot](https://certbot.eff.org/).
 
 This plugin is built from the ground up and follows the development style and life-cycle
 of other `certbot-dns-*` plugins found in the
 [Official Certbot Repository](https://github.com/certbot/certbot). PR is open [here](https://github.com/certbot/certbot/pull/8727) though Certbot is not accepting plugin PR's at the moment.
 
@@ -51,15 +52,15 @@
 pip3 install certbot certbot-dns-azure
 ```
 
 ### Via Snap - not tested yet
 
 ```
 sudo snap install certbot --classic
-sudo snap install certbot-dns-azure
+sudo snap install --channel=stable certbot-dns-azure
 sudo snap set certbot trust-plugin-with-root=ok
 sudo snap connect certbot:plugin certbot-dns-azure
 ```
 
 ### Verification
 
 Verify:
@@ -74,10 +75,10 @@
 Interfaces: IAuthenticator, IPlugin
 Entry point: dns-azure = certbot_dns_azure.dns_azure:Authenticator
 
 ...
 ...
 ```
 
-Docs and instructions on configuration are [here](https://certbot-dns-azure.readthedocs.io/en/latest/)
+Docs and instructions on configuration are [here](https://docs.certbot-dns-azure.co.uk/en/latest/)
```

### Comparing `certbot-dns-azure-2.1.0/README.md` & `certbot-dns-azure-2.2.0b0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # certbot-dns-azure
 
 [![Tests](https://github.com/binkhq/certbot-dns-azure/workflows/Release/badge.svg)](https://github.com/binkhq/certbot-dns-azure/actions)
 [![Python Version](https://img.shields.io/pypi/pyversions/certbot-dns-azure)](https://pypi.org/project/certbot-dns-azure/)
 [![PyPi Status](https://img.shields.io/pypi/status/certbot-dns-azure)](https://pypi.org/project/certbot-dns-azure/)
 [![Version](https://img.shields.io/pypi/v/certbot-dns-azure)](https://pypi.org/project/certbot-dns-azure/)
-[![Docs](https://readthedocs.org/projects/certbot-dns-azure/badge/?version=latest&style=flat)](https://certbot-dns-azure.readthedocs.io/en/latest/)
+[![Docs](https://readthedocs.org/projects/certbot-dns-azure/badge/?version=latest&style=flat)](https://docs.certbot-dns-azure.co.uk/en/latest/)
 
 AzureDNS Authenticator plugin for [Certbot](https://certbot.eff.org/).
 
 This plugin is built from the ground up and follows the development style and life-cycle
 of other `certbot-dns-*` plugins found in the
 [Official Certbot Repository](https://github.com/certbot/certbot). PR is open [here](https://github.com/certbot/certbot/pull/8727) though Certbot is not accepting plugin PR's at the moment.
 
@@ -21,15 +21,15 @@
 pip3 install certbot certbot-dns-azure
 ```
 
 ### Via Snap - not tested yet
 
 ```
 sudo snap install certbot --classic
-sudo snap install certbot-dns-azure
+sudo snap install --channel=stable certbot-dns-azure
 sudo snap set certbot trust-plugin-with-root=ok
 sudo snap connect certbot:plugin certbot-dns-azure
 ```
 
 ### Verification
 
 Verify:
@@ -44,10 +44,10 @@
 Interfaces: IAuthenticator, IPlugin
 Entry point: dns-azure = certbot_dns_azure.dns_azure:Authenticator
 
 ...
 ...
 ```
 
-Docs and instructions on configuration are [here](https://certbot-dns-azure.readthedocs.io/en/latest/)
+Docs and instructions on configuration are [here](https://docs.certbot-dns-azure.co.uk/en/latest/)
```

### Comparing `certbot-dns-azure-2.1.0/certbot_dns_azure/_internal/dns_azure.py` & `certbot-dns-azure-2.2.0b0/certbot_dns_azure/_internal/dns_azure.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """DNS Authenticator for Azure DNS."""
 import logging
 from os import getenv
-from typing import Dict
+from typing import Dict, Tuple
 
 from azure.mgmt.dns import DnsManagementClient
 from azure.mgmt.dns.models import RecordSet, TxtRecord
 from azure.core.exceptions import HttpResponseError
+from azure.core.utils import CaseInsensitiveDict
 from azure.identity import ClientSecretCredential, ManagedIdentityCredential, CertificateCredential
 
 from certbot import errors
 from certbot.plugins import dns_common
 
 logger = logging.getLogger(__name__)
 logging.getLogger('azure').setLevel(logging.WARNING)
@@ -149,80 +150,113 @@
                 authority=aad_endpoint
             )
         elif msi_client_id:
             return ManagedIdentityCredential(client_id=msi_client_id)
         else:
             return ManagedIdentityCredential()
 
-    def _get_ids_for_domain(self, domain: str):
+    def _get_ids_for_domain(self, domain: str, validation_name: str) -> Tuple[str, str, str, str, bool]:
+        """
+        :param domain: Domain/subdomain to look up the closest parent in the config file
+        :param validation_name: DNS challenge record name, fully qualified
+
+        This returns:
+        * The Azure DNS zone for which to add records to
+        * The subscription ID for said zone
+        * The resource group for said zone
+        * The relative validation record name (or if explicitly overrided with an ID, an alternate record name)
+        * If the validation record can be deleted, if its explicitly overrided, it wont be deleted but set to `-`
+        """
+        # So if the config contains domain.io and test.domain.io
+        # and we want to renew, we'd prefer test.domain.io.
+        # Sort domains by longest first and then attempt to find the right one.
+        # This should work better, as then a.b.test.domain.io would pick domain.io irrelevant
+        # of its order in the config
+        azure_domains = sorted(self.domain_zoneid.keys(), key=lambda domain: len(domain), reverse=True)
+
         try:
-            for azure_dns_domain, resource_group in self.domain_zoneid.items():
+            for azure_dns_domain in azure_domains:
                 # Look to see if domain ends with key, to cover subdomains
                 if domain.endswith(azure_dns_domain):
-                    subscription_id = resource_group.split('/')[2]
-                    rg_name = resource_group.split('/')[4]
-                    return azure_dns_domain, subscription_id, rg_name
+                    zone_id = self.domain_zoneid[azure_dns_domain]
+
+                    try:
+                        resource = self.parse_azure_resource_id(zone_id)
+                    except ValueError as exc:
+                        raise errors.PluginError('Failed to parse resource ID for {}: {}'
+                                                 .format(domain, zone_id)) from exc
+                    subscription_id = resource.get('subscriptions')
+                    rg_name = resource.get('resourceGroups')
+                    if 'dnsZones' in resource:  # If we're manually specifying an alternate zone to use, override.
+                        azure_dns_domain = resource.get('dnsZones')
+                    relative_validation_name = self._get_relative_domain(validation_name, azure_dns_domain)
+                    can_delete = True
+                    if 'TXT' in resource:  # If we're explicitly specifing a destination record, use instead.
+                        relative_validation_name = resource.get('TXT')
+                        can_delete = False  # If we're specifying a specific record, dont delete it
+
+                    return azure_dns_domain, subscription_id, rg_name, relative_validation_name, can_delete
             else:
                 raise errors.PluginError('Domain {} does not have a valid domain to '
                                          'resource group id mapping'.format(domain))
         except IndexError:
             raise errors.PluginError('Domain {} has an invalid resource group id'.format(domain))
 
     @staticmethod
     def _get_relative_domain(fqdn: str, domain: str) -> str:
         if fqdn == domain:
             return '@'
         return fqdn.replace(domain, '').strip('.')
 
     def _perform(self, domain, validation_name, validation):
-        azure_domain, subscription_id, resource_group_name = self._get_ids_for_domain(domain)
+        azure_domain, subscription_id, resource_group_name, validation_name, _ = self._get_ids_for_domain(domain, validation_name)
         client = self._get_azure_client(subscription_id)
-        relative_validation_name = self._get_relative_domain(validation_name, azure_domain)
 
         # Check to see if there are any existing TXT validation record values
         txt_value = {validation}
         try:
             existing_rr = client.record_sets.get(
                 resource_group_name=resource_group_name,
                 zone_name=azure_domain,
-                relative_record_set_name=relative_validation_name,
+                relative_record_set_name=validation_name,
                 record_type='TXT')
             for record in existing_rr.txt_records:
                 for value in record.value:
+                    if value == '-':
+                        continue
                     txt_value.add(value)
         except HttpResponseError as err:
             if err.status_code != 404:  # Ignore RR not found
                 raise errors.PluginError('Failed to check TXT record for domain '
                                          '{}, error: {}'.format(domain, err))
 
         try:
             client.record_sets.create_or_update(
                 resource_group_name=resource_group_name,
                 zone_name=azure_domain,
-                relative_record_set_name=relative_validation_name,
+                relative_record_set_name=validation_name,
                 record_type='TXT',
                 parameters=RecordSet(ttl=self.ttl, txt_records=[TxtRecord(value=[v]) for v in txt_value])
             )
         except HttpResponseError as err:
             raise errors.PluginError('Failed to add TXT record to domain '
                                      '{}, error: {}'.format(domain, err))
 
     def _cleanup(self, domain, validation_name, validation):
         if self.credential is None:
             self._setup_credentials()
 
-        azure_domain, subscription_id, resource_group_name = self._get_ids_for_domain(domain)
-        relative_validation_name = self._get_relative_domain(validation_name, azure_domain)
+        azure_domain, subscription_id, resource_group_name, validation_name, can_delete = self._get_ids_for_domain(domain, validation_name)
         client = self._get_azure_client(subscription_id)
 
         txt_value = set()
         try:
             existing_rr = client.record_sets.get(resource_group_name=resource_group_name,
                                                  zone_name=azure_domain,
-                                                 relative_record_set_name=relative_validation_name,
+                                                 relative_record_set_name=validation_name,
                                                  record_type='TXT')
             for record in existing_rr.txt_records:
                 for value in record.value:
                     txt_value.add(value)
         except HttpResponseError as err:
             if err.status_code != 404:  # Ignore RR not found
                 raise errors.PluginError('Failed to check TXT record for domain '
@@ -231,26 +265,35 @@
         txt_value -= {validation}
 
         try:
             if txt_value:
                 client.record_sets.create_or_update(
                     resource_group_name=resource_group_name,
                     zone_name=azure_domain,
-                    relative_record_set_name=relative_validation_name,
+                    relative_record_set_name=validation_name,
                     record_type='TXT',
                     parameters=RecordSet(ttl=self.ttl,
                                          txt_records=[TxtRecord(value=[v]) for v in txt_value])
                 )
             else:
-                client.record_sets.delete(
-                    resource_group_name=resource_group_name,
-                    zone_name=azure_domain,
-                    relative_record_set_name=relative_validation_name,
-                    record_type='TXT'
-                )
+                if can_delete:
+                    client.record_sets.delete(
+                        resource_group_name=resource_group_name,
+                        zone_name=azure_domain,
+                        relative_record_set_name=validation_name,
+                        record_type='TXT'
+                    )
+                else:
+                    client.record_sets.create_or_update(  # We've manually specified a record, so dont delete, set to -
+                        resource_group_name=resource_group_name,
+                        zone_name=azure_domain,
+                        relative_record_set_name=validation_name,
+                        record_type='TXT',
+                        parameters=RecordSet(ttl=self.ttl, txt_records=[TxtRecord(value=['-'])])
+                    )
         except HttpResponseError as err:
             if err.status_code != 404:  # Ignore RR not found
                 raise errors.PluginError('Failed to remove TXT record for domain '
                                          '{}, error: {}'.format(domain, err))
 
     def _get_azure_client(self, subscription_id):
         """
@@ -258,7 +301,24 @@
 
         :param subscription_id: Azure subscription ID
         :type subscription_id: str
         :return: Azure DNS client
         :rtype: DnsManagementClient
         """
         return DnsManagementClient(self.credential, subscription_id, None, self._arm_endpoint, credential_scopes=[self._arm_endpoint + "/.default"])
+
+    @staticmethod
+    def parse_azure_resource_id(resource_id):
+        rsrc_id = resource_id
+        if rsrc_id.startswith('/'):
+            rsrc_id = rsrc_id[1:]
+
+        if rsrc_id.endswith('/'):
+            rsrc_id = rsrc_id[:-1]
+
+        if '/' not in rsrc_id:
+            raise ValueError('Invalid resource ID: {}'.format(resource_id))
+
+        parts = rsrc_id.split('/')
+        if (len(parts) % 2) != 0 or '' in parts:
+            raise ValueError('Invalid resource ID: {}'.format(resource_id))
+        return CaseInsensitiveDict(zip(parts[0::2], parts[1::2]))
```

### Comparing `certbot-dns-azure-2.1.0/certbot_dns_azure.egg-info/PKG-INFO` & `certbot-dns-azure-2.2.0b0/certbot_dns_azure.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: certbot-dns-azure
-Version: 2.1.0
+Version: 2.2.0b0
 Summary: Azure DNS Authenticator plugin for Certbot
 Home-page: https://github.com/binkhq/certbot-dns-azure
 Author: Terry Cain
 Author-email: opensource@bink.com
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Security
 Classifier: Topic :: System :: Installation/Setup
 Classifier: Topic :: System :: Networking
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6
@@ -30,15 +31,15 @@
 
 # certbot-dns-azure
 
 [![Tests](https://github.com/binkhq/certbot-dns-azure/workflows/Release/badge.svg)](https://github.com/binkhq/certbot-dns-azure/actions)
 [![Python Version](https://img.shields.io/pypi/pyversions/certbot-dns-azure)](https://pypi.org/project/certbot-dns-azure/)
 [![PyPi Status](https://img.shields.io/pypi/status/certbot-dns-azure)](https://pypi.org/project/certbot-dns-azure/)
 [![Version](https://img.shields.io/pypi/v/certbot-dns-azure)](https://pypi.org/project/certbot-dns-azure/)
-[![Docs](https://readthedocs.org/projects/certbot-dns-azure/badge/?version=latest&style=flat)](https://certbot-dns-azure.readthedocs.io/en/latest/)
+[![Docs](https://readthedocs.org/projects/certbot-dns-azure/badge/?version=latest&style=flat)](https://docs.certbot-dns-azure.co.uk/en/latest/)
 
 AzureDNS Authenticator plugin for [Certbot](https://certbot.eff.org/).
 
 This plugin is built from the ground up and follows the development style and life-cycle
 of other `certbot-dns-*` plugins found in the
 [Official Certbot Repository](https://github.com/certbot/certbot). PR is open [here](https://github.com/certbot/certbot/pull/8727) though Certbot is not accepting plugin PR's at the moment.
 
@@ -51,15 +52,15 @@
 pip3 install certbot certbot-dns-azure
 ```
 
 ### Via Snap - not tested yet
 
 ```
 sudo snap install certbot --classic
-sudo snap install certbot-dns-azure
+sudo snap install --channel=stable certbot-dns-azure
 sudo snap set certbot trust-plugin-with-root=ok
 sudo snap connect certbot:plugin certbot-dns-azure
 ```
 
 ### Verification
 
 Verify:
@@ -74,10 +75,10 @@
 Interfaces: IAuthenticator, IPlugin
 Entry point: dns-azure = certbot_dns_azure.dns_azure:Authenticator
 
 ...
 ...
 ```
 
-Docs and instructions on configuration are [here](https://certbot-dns-azure.readthedocs.io/en/latest/)
+Docs and instructions on configuration are [here](https://docs.certbot-dns-azure.co.uk/en/latest/)
```

### Comparing `certbot-dns-azure-2.1.0/certbot_dns_azure.egg-info/SOURCES.txt` & `certbot-dns-azure-2.2.0b0/certbot_dns_azure.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `certbot-dns-azure-2.1.0/docs/Makefile` & `certbot-dns-azure-2.2.0b0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `certbot-dns-azure-2.1.0/docs/conf.py` & `certbot-dns-azure-2.2.0b0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `certbot-dns-azure-2.1.0/docs/index.rst` & `certbot-dns-azure-2.2.0b0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `certbot-dns-azure-2.1.0/docs/make.bat` & `certbot-dns-azure-2.2.0b0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `certbot-dns-azure-2.1.0/setup.py` & `certbot-dns-azure-2.2.0b0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import find_packages
 from setuptools import setup
 
-version = '2.1.0'
+version = '2.2.0b0'
 
 # azure-mgmt-dns is still the old style SDK, so will change dramatically
 # when they refactor, most notably the credential parts
 install_requires = [
     'azure-identity>=1.11.0',
     'azure-mgmt-dns>=8.0.0',
     'setuptools>=41.6.0',
@@ -35,18 +35,19 @@
         'Development Status :: 5 - Production/Stable',
         'Environment :: Plugins',
         'Intended Audience :: System Administrators',
         'License :: OSI Approved :: Apache Software License',
         'Operating System :: POSIX :: Linux',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Topic :: Internet :: WWW/HTTP',
         'Topic :: Security',
         'Topic :: System :: Installation/Setup',
         'Topic :: System :: Networking',
         'Topic :: System :: Systems Administration',
         'Topic :: Utilities',
     ],
```

### Comparing `certbot-dns-azure-2.1.0/tests/dns_azure_test.py` & `certbot-dns-azure-2.2.0b0/tests/dns_azure_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,15 +16,17 @@
 
 from azure.mgmt.dns.models import RecordSet, TxtRecord
 
 MULTI_DOMAIN = [
     achallenges.KeyAuthorizationAnnotatedChallenge(
         challb=acme_util.DNS01, domain='example.com', account_key=KEY),
     achallenges.KeyAuthorizationAnnotatedChallenge(
-        challb=acme_util.DNS01, domain='example.org', account_key=KEY)
+        challb=acme_util.DNS01, domain='example.org', account_key=KEY),
+    achallenges.KeyAuthorizationAnnotatedChallenge(
+        challb=acme_util.DNS01, domain='example.net', account_key=KEY)
 ]
 SINGLE_DOMAIN = [
     achallenges.KeyAuthorizationAnnotatedChallenge(
         challb=acme_util.DNS01, domain='example.com', account_key=KEY),
 ]
 SUB_DOMAIN = [
     achallenges.KeyAuthorizationAnnotatedChallenge(
@@ -45,15 +47,17 @@
         # Setup config files
         config_files = (
             ('sp.ini', {
                 'azure_sp_client_id': '912ce44a-0156-4669-ae22-c16a17d34ca5',
                 'azure_sp_client_secret': 'E-xqXU83Y-jzTI6xe9fs2YC~mck3ZzUih9',
                 'azure_tenant_id': 'ed1090f3-ab18-4b12-816c-599af8a88cf7',
                 'azure_zone1': 'example.com:/subscriptions/c135abce-d87d-48df-936c-15596c6968a5/resourceGroups/dns1',
-                'azure_zone2': 'example.org:/subscriptions/99800903-fb14-4992-9aff-12eaf2744622/resourceGroups/dns2'
+                'azure_zone2': 'example.org:/subscriptions/99800903-fb14-4992-9aff-12eaf2744622/resourceGroups/dns2',
+                'azure_zone3': ('example.net:/subscriptions/99800903-fb14-4992-9aff-12eaf2744622/resourceGroups/dns2'
+                                '/providers/Microsoft.Network/dnsZones/example.com')
             }),
             ('sp_cert.ini', {
                 'azure_sp_client_id': '912ce44a-0156-4669-ae22-c16a17d34ca5',
                 'azure_sp_client_secret': 'E-xqXU83Y-jzTI6xe9fs2YC~mck3ZzUih9',
                 'azure_certificate_path': '/path/to/cert.pem',
                 'azure_zone1': 'example.com:/subscriptions/c135abce-d87d-48df-936c-15596c6968a5/resourceGroups/dns1',
                 'azure_zone2': 'example.org:/subscriptions/99800903-fb14-4992-9aff-12eaf2744622/resourceGroups/dns2'
@@ -91,43 +95,54 @@
         self.auth._get_azure_credentials = mock.MagicMock(return_value=self.mock_credentials)
         self.auth._get_azure_client = mock.MagicMock(return_value=self.mock_client)
 
     def test_perform_multidomain(self):
         self.mock_client.record_sets.get.return_value = RecordSet(txt_records=[])
 
         # Extract zone TXT record name and value
-        zone1_req, zone2_req = MULTI_DOMAIN
+        zone1_req, zone2_req, zone3_req = MULTI_DOMAIN
         zone1_domain_name = zone1_req.validation_domain_name(zone1_req.domain)
         zone1_relative_record = zone1_domain_name.replace('example.com', '').strip('.')
         zone1_key = zone1_req.validation(zone1_req.account_key)
         zone2_domain_name = zone2_req.validation_domain_name(zone2_req.domain)
         zone2_relative_record = zone2_domain_name.replace('example.org', '').strip('.')
         zone2_key = zone2_req.validation(zone2_req.account_key)
+        zone3_domain_name = zone3_req.validation_domain_name(zone3_req.domain)
+        zone3_relative_record = zone3_domain_name.replace('example.com', '').strip('.')
+        zone3_key = zone3_req.validation(zone3_req.account_key)
 
         self.auth.perform(MULTI_DOMAIN)
 
         # Check azure client call counts
-        self.assertEqual(self.mock_client.record_sets.get.call_count, 2)
-        self.assertEqual(self.mock_client.record_sets.create_or_update.call_count, 2)
+        self.assertEqual(self.mock_client.record_sets.get.call_count, 3)
+        self.assertEqual(self.mock_client.record_sets.create_or_update.call_count, 3)
 
         #
-        zone1_call, zone2_call = self.mock_client.record_sets.create_or_update.call_args_list
+        zone1_call, zone2_call, zone3_call = self.mock_client.record_sets.create_or_update.call_args_list
         self.assertEqual(zone1_call[1]['zone_name'], "example.com")
         self.assertEqual(zone1_call[1]['record_type'], "TXT")
         self.assertEqual(zone1_call[1]['relative_record_set_name'], zone1_relative_record)
         zone1_txt_records = zone1_call[1]['parameters'].txt_records
         self.assertEqual(len(zone1_txt_records), 1)
         self.assertEqual(zone1_txt_records[0].value[0], zone1_key)
 
         self.assertEqual(zone2_call[1]['zone_name'], "example.org")
         self.assertEqual(zone2_call[1]['relative_record_set_name'], zone2_relative_record)
         zone2_txt_records = zone2_call[1]['parameters'].txt_records
         self.assertEqual(len(zone2_txt_records), 1)
         self.assertEqual(zone2_txt_records[0].value[0], zone2_key)
 
+        # Test DNS delegation of example.net to example.com
+        self.assertEqual(zone3_req.domain, "example.net")
+        self.assertEqual(zone3_call[1]['zone_name'], "example.com")
+        self.assertEqual(zone3_call[1]['relative_record_set_name'], zone3_relative_record)
+        zone3_txt_records = zone3_call[1]['parameters'].txt_records
+        self.assertEqual(len(zone3_txt_records), 1)
+        self.assertEqual(zone3_txt_records[0].value[0], zone3_key)
+
     def test_perform_existing(self):
         self.mock_client.record_sets.get.return_value = RecordSet(txt_records=[
             TxtRecord(value=['someexistingkey'])
         ])
 
         # Extract zone TXT record name and value
         zone1_req = SINGLE_DOMAIN[0]
@@ -184,37 +199,43 @@
         self.assertEqual(len(zone1_txt_records), 1)
         self.assertEqual(zone1_txt_records[0].value[0], zone1_key)
 
     def test_cleanup_multiple(self):
         self.mock_client.record_sets.get.return_value = RecordSet(txt_records=[])
 
         # Extract zone TXT record name and value
-        zone1_req, zone2_req = MULTI_DOMAIN
+        zone1_req, zone2_req, zone3_req = MULTI_DOMAIN
         zone1_domain_name = zone1_req.validation_domain_name(zone1_req.domain)
         zone2_domain_name = zone2_req.validation_domain_name(zone2_req.domain)
+        zone3_domain_name = zone3_req.validation_domain_name(zone3_req.domain)
         zone1_relative_record = zone1_domain_name.replace('example.com', '').strip('.')
         zone2_relative_record = zone2_domain_name.replace('example.org', '').strip('.')
+        zone3_relative_record = zone3_domain_name.replace('example.com', '').strip('.')
 
         # _attempt_cleanup | pylint: disable=protected-access
         self.auth._attempt_cleanup = True
         self.auth.cleanup(MULTI_DOMAIN)
 
         # Check azure client call counts
-        self.assertEqual(self.mock_client.record_sets.get.call_count, 2)
-        self.assertEqual(self.mock_client.record_sets.delete.call_count, 2)
+        self.assertEqual(self.mock_client.record_sets.get.call_count, 3)
+        self.assertEqual(self.mock_client.record_sets.delete.call_count, 3)
 
-        zone1_call, zone2_call = self.mock_client.record_sets.delete.call_args_list
+        zone1_call, zone2_call, zone3_call = self.mock_client.record_sets.delete.call_args_list
         self.assertEqual(zone1_call[1]['zone_name'], "example.com")
         self.assertEqual(zone1_call[1]['record_type'], "TXT")
         self.assertEqual(zone1_call[1]['relative_record_set_name'], zone1_relative_record)
 
         self.assertEqual(zone2_call[1]['zone_name'], "example.org")
         self.assertEqual(zone2_call[1]['record_type'], "TXT")
         self.assertEqual(zone2_call[1]['relative_record_set_name'], zone2_relative_record)
 
+        self.assertEqual(zone3_call[1]['zone_name'], "example.com")
+        self.assertEqual(zone3_call[1]['record_type'], "TXT")
+        self.assertEqual(zone3_call[1]['relative_record_set_name'], zone3_relative_record)
+
     def test_cleanup_existing(self):
         self.mock_client.record_sets.get.return_value = RecordSet(txt_records=[
             TxtRecord(value=['someexistingkey'])
         ])
 
         # Extract zone TXT record name and value
         zone1_req = SINGLE_DOMAIN[0]
@@ -269,10 +290,22 @@
             'azure_tenant_id': 'ed1090f3-ab18-4b12-816c-599af8a88cf7',
             'azure_zone1': 'example.com',
         }, self.sp_config.azure_config)
         with self.assertRaises(errors.PluginError) as cm:
             self.auth.perform(SINGLE_DOMAIN)
         self.assertIn('DNS Zone mapping is not in the format', cm.exception.args[0])
 
+    def test_config_bad_resource_group(self):
+        # Test invalid resource group ID
+        dns_test_common.write({
+            'azure_sp_client_id': '912ce44a-0156-4669-ae22-c16a17d34ca5',
+            'azure_sp_client_secret': 'E-xqXU83Y-jzTI6xe9fs2YC~mck3ZzUih9',
+            'azure_tenant_id': 'ed1090f3-ab18-4b12-816c-599af8a88cf7',
+            'azure_zone1': 'example.com:/subscriptions/c135abce-d87d-48df-936c-15596c6968a5/invalid',
+        }, self.sp_config.azure_config)
+        with self.assertRaises(errors.PluginError) as cm:
+            self.auth.perform(SINGLE_DOMAIN)
+        self.assertIn('Failed to parse resource ID for example.com', cm.exception.args[0])
+
 
 if __name__ == "__main__":
     unittest.main()  # pragma: no cover
```

