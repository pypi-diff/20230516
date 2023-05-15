# Comparing `tmp/ibeam-0.4.3.tar.gz` & `tmp/ibeam-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ibeam-0.4.3.tar", last modified: Tue Aug  9 08:39:14 2022, max compression
+gzip compressed data, was "dist\ibeam-0.4.4.tar", last modified: Mon May 15 23:30:34 2023, max compression
```

## Comparing `ibeam-0.4.3.tar` & `ibeam-0.4.4.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxrwxrwx   0        0        0        0 2022-08-09 08:39:14.000000 ibeam-0.4.3/
--rw-rw-rw-   0        0        0    11562 2020-10-15 10:25:32.000000 ibeam-0.4.3/LICENSE
--rw-rw-rw-   0        0        0    18598 2022-08-09 08:39:14.000000 ibeam-0.4.3/PKG-INFO
--rw-rw-rw-   0        0        0    17908 2022-07-02 18:21:50.000000 ibeam-0.4.3/README.md
-drwxrwxrwx   0        0        0        0 2022-08-09 08:39:14.000000 ibeam-0.4.3/ibeam/
--rw-rw-rw-   0        0        0       74 2022-08-09 08:38:16.000000 ibeam-0.4.3/ibeam/__init__.py
--rw-rw-rw-   0        0        0      349 2021-06-21 13:45:43.000000 ibeam-0.4.3/ibeam/config.py
--rw-rw-rw-   0        0        0     3814 2022-04-07 12:15:07.000000 ibeam-0.4.3/ibeam/ibeam_starter.py
-drwxrwxrwx   0        0        0        0 2022-08-09 08:39:14.000000 ibeam-0.4.3/ibeam/src/
--rw-rw-rw-   0        0        0        0 2020-10-09 05:29:20.000000 ibeam-0.4.3/ibeam/src/__init__.py
--rw-rw-rw-   0        0        0    14002 2022-04-07 12:15:07.000000 ibeam-0.4.3/ibeam/src/authenticate.py
--rw-rw-rw-   0        0        0    15616 2022-07-02 18:21:50.000000 ibeam-0.4.3/ibeam/src/gateway_client.py
--rw-rw-rw-   0        0        0     1696 2022-06-27 14:32:23.000000 ibeam-0.4.3/ibeam/src/health_server.py
--rw-rw-rw-   0        0        0     7539 2022-04-07 12:15:07.000000 ibeam-0.4.3/ibeam/src/http_handler.py
--rw-rw-rw-   0        0        0     1315 2022-04-07 12:15:07.000000 ibeam-0.4.3/ibeam/src/inputs_handler.py
--rw-rw-rw-   0        0        0     1668 2022-04-07 12:15:07.000000 ibeam-0.4.3/ibeam/src/logs.py
--rw-rw-rw-   0        0        0     1821 2021-06-21 13:45:43.000000 ibeam-0.4.3/ibeam/src/process_utils.py
-drwxrwxrwx   0        0        0        0 2022-08-09 08:39:14.000000 ibeam-0.4.3/ibeam/src/two_fa_handlers/
--rw-rw-rw-   0        0        0        0 2022-08-09 08:38:04.000000 ibeam-0.4.3/ibeam/src/two_fa_handlers/__init__.py
--rw-rw-rw-   0        0        0     2941 2021-06-21 13:45:43.000000 ibeam-0.4.3/ibeam/src/two_fa_handlers/external_request_handler.py
--rw-rw-rw-   0        0        0     4831 2022-04-07 12:15:07.000000 ibeam-0.4.3/ibeam/src/two_fa_handlers/google_msg_handler.py
--rw-rw-rw-   0        0        0      264 2021-06-21 13:45:43.000000 ibeam-0.4.3/ibeam/src/two_fa_handlers/two_fa_handler.py
--rw-rw-rw-   0        0        0     2483 2021-06-21 13:45:43.000000 ibeam-0.4.3/ibeam/src/two_fa_selector.py
--rw-rw-rw-   0        0        0     5556 2022-07-02 18:21:50.000000 ibeam-0.4.3/ibeam/src/var.py
-drwxrwxrwx   0        0        0        0 2022-08-09 08:39:14.000000 ibeam-0.4.3/ibeam.egg-info/
--rw-rw-rw-   0        0        0    18598 2022-08-09 08:39:13.000000 ibeam-0.4.3/ibeam.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      669 2022-08-09 08:39:13.000000 ibeam-0.4.3/ibeam.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-09 08:39:13.000000 ibeam-0.4.3/ibeam.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       97 2022-08-09 08:39:13.000000 ibeam-0.4.3/ibeam.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2022-08-09 08:39:13.000000 ibeam-0.4.3/ibeam.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2022-08-09 08:39:14.000000 ibeam-0.4.3/setup.cfg
--rw-rw-rw-   0        0        0     1378 2022-04-07 12:19:21.000000 ibeam-0.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 23:30:34.000000 ibeam-0.4.4/
+-rw-rw-rw-   0        0        0    11562 2020-10-15 10:25:32.000000 ibeam-0.4.4/LICENSE
+-rw-rw-rw-   0        0        0    10486 2023-05-15 23:30:34.000000 ibeam-0.4.4/PKG-INFO
+-rw-rw-rw-   0        0        0     9800 2022-08-31 12:47:22.000000 ibeam-0.4.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-15 23:30:34.000000 ibeam-0.4.4/ibeam/
+-rw-rw-rw-   0        0        0       74 2023-05-15 18:50:41.000000 ibeam-0.4.4/ibeam/__init__.py
+-rw-rw-rw-   0        0        0      349 2021-06-21 13:45:43.000000 ibeam-0.4.4/ibeam/config.py
+-rw-rw-rw-   0        0        0     3850 2023-05-04 18:30:06.000000 ibeam-0.4.4/ibeam/ibeam_starter.py
+drwxrwxrwx   0        0        0        0 2023-05-15 23:30:34.000000 ibeam-0.4.4/ibeam/src/
+-rw-rw-rw-   0        0        0        0 2020-10-09 05:29:20.000000 ibeam-0.4.4/ibeam/src/__init__.py
+-rw-rw-rw-   0        0        0    19816 2023-05-09 19:20:47.000000 ibeam-0.4.4/ibeam/src/authenticate.py
+-rw-rw-rw-   0        0        0    15614 2023-05-04 18:33:34.000000 ibeam-0.4.4/ibeam/src/gateway_client.py
+-rw-rw-rw-   0        0        0     1696 2022-06-27 14:32:23.000000 ibeam-0.4.4/ibeam/src/health_server.py
+-rw-rw-rw-   0        0        0     7805 2023-05-04 18:33:34.000000 ibeam-0.4.4/ibeam/src/http_handler.py
+-rw-rw-rw-   0        0        0     1314 2023-05-04 18:33:34.000000 ibeam-0.4.4/ibeam/src/inputs_handler.py
+-rw-rw-rw-   0        0        0     1668 2022-04-07 12:15:07.000000 ibeam-0.4.4/ibeam/src/logs.py
+-rw-rw-rw-   0        0        0     1851 2023-05-04 18:30:58.000000 ibeam-0.4.4/ibeam/src/process_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-15 23:30:34.000000 ibeam-0.4.4/ibeam/src/two_fa_handlers/
+-rw-rw-rw-   0        0        0        0 2022-08-09 08:38:04.000000 ibeam-0.4.4/ibeam/src/two_fa_handlers/__init__.py
+-rw-rw-rw-   0        0        0     2941 2021-06-21 13:45:43.000000 ibeam-0.4.4/ibeam/src/two_fa_handlers/external_request_handler.py
+-rw-rw-rw-   0        0        0     5387 2023-05-04 18:33:34.000000 ibeam-0.4.4/ibeam/src/two_fa_handlers/google_msg_handler.py
+-rw-rw-rw-   0        0        0     2975 2023-05-03 22:42:05.000000 ibeam-0.4.4/ibeam/src/two_fa_handlers/notification_resend_handler.py
+-rw-rw-rw-   0        0        0      264 2021-06-21 13:45:43.000000 ibeam-0.4.4/ibeam/src/two_fa_handlers/two_fa_handler.py
+-rw-rw-rw-   0        0        0     2682 2023-04-01 23:25:13.000000 ibeam-0.4.4/ibeam/src/two_fa_selector.py
+-rw-rw-rw-   0        0        0     6087 2023-05-03 22:26:29.000000 ibeam-0.4.4/ibeam/src/var.py
+drwxrwxrwx   0        0        0        0 2023-05-15 23:30:34.000000 ibeam-0.4.4/ibeam.egg-info/
+-rw-rw-rw-   0        0        0    10486 2023-05-15 23:30:32.000000 ibeam-0.4.4/ibeam.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      726 2023-05-15 23:30:33.000000 ibeam-0.4.4/ibeam.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 23:30:32.000000 ibeam-0.4.4/ibeam.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       97 2023-05-15 23:30:32.000000 ibeam-0.4.4/ibeam.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-15 23:30:32.000000 ibeam-0.4.4/ibeam.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-05-15 23:30:34.000000 ibeam-0.4.4/setup.cfg
+-rw-rw-rw-   0        0        0     1378 2022-04-07 12:19:21.000000 ibeam-0.4.4/setup.py
```

### Comparing `ibeam-0.4.3/LICENSE` & `ibeam-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ibeam-0.4.3/ibeam/ibeam_starter.py` & `ibeam-0.4.4/ibeam/ibeam_starter.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 
     client = GatewayClient(http_handler=http_handler,
                            inputs_handler=inputs_handler,
                            two_fa_handler=two_fa_handler,
                            gateway_dir=gateway_dir,
                            driver_path=driver_path)
 
-    _LOGGER.debug(f'{var.all_variables}')
+    _LOGGER.info(f'Environment variable configuration:\n{var.all_variables}')
 
     if args.start:
         pid = client.try_starting()
         success = pid is not None
         if success:
             _LOGGER.info(f'Gateway running with pid: {pid}')
         else:
```

### Comparing `ibeam-0.4.3/ibeam/src/authenticate.py` & `ibeam-0.4.4/ibeam/src/authenticate.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,51 +1,63 @@
 import logging
 import os
-import re
 import sys
 import time
 import traceback
-import urllib.parse
 from datetime import datetime
 from pathlib import Path
 import tempfile
-from typing import Union
+from typing import Union, Optional
 
 from cryptography.fernet import Fernet
 from pyvirtualdisplay import Display
 from selenium import webdriver
 from selenium.common.exceptions import WebDriverException, StaleElementReferenceException, TimeoutException
 from selenium.webdriver.common.by import By
 from selenium.webdriver.common.keys import Keys
 from selenium.webdriver.support import expected_conditions as EC
 from selenium.webdriver.support.wait import WebDriverWait
+from selenium.webdriver.support.ui import Select
 
 import ibeam
 from ibeam.src import var
 from ibeam.src.two_fa_handlers.two_fa_handler import TwoFaHandler
 
 _LOGGER = logging.getLogger('ibeam.' + Path(__file__).stem)
 
 _DRIVER_NAMES = {}
 _FAILED_ATTEMPTS = 0
 
+_VERSIONS = {
+    1: {
+        'USER_NAME_EL': 'user_name',
+        'ERROR_EL': 'alert alert-danger margin-top-10'
+    },
+    2: {
+        'USER_NAME_EL': 'username',
+        'ERROR_EL': 'xyz-errormessage'
+    }
+}
 
-def new_chrome_driver(driver_path, name: str = 'default', headless: bool = True):
+
+def new_chrome_driver(driver_path, name: str = 'default', headless: bool = True, incognito: bool = True):
     """Creates a new chrome driver."""
 
     global _DRIVER_NAMES
 
     _DRIVER_NAMES[name] = True  # just to ensure the name is in the dict
     driver_index = list(_DRIVER_NAMES.keys()).index(name)  # order of insertion dictates the driver_index
 
     options = webdriver.ChromeOptions()
     if headless:
         options.add_argument('--headless')
         options.add_argument('--disable-gpu')
     options.add_argument('--no-sandbox')
+    if incognito:
+        options.add_argument("--incognito")  # this allows 2FA method to be selected every time
     options.add_argument('--ignore-ssl-errors=yes')
     options.add_argument('--ignore-certificate-errors')
     options.add_argument(f'--remote-debugging-port={9222 + driver_index}')
     options.add_argument('--useAutomationExtension=false')
     options.add_argument('--disable-extensions')
     options.add_argument('--dns-prefetch-disable')
     options.add_argument(f'--user-data-dir={tempfile.gettempdir()}/ibeam-chrome-{name}')
@@ -106,29 +118,105 @@
         return
 
     now = datetime.now().strftime('%Y-%m-%d_%H-%M-%S')
     outputs_path = Path(var.OUTPUTS_DIR)
     screenshot_name = f'ibeam__{ibeam.__version__}__{now}{postfix}.png'
 
     try:
+        required_width = driver.execute_script('return document.body.parentNode.scrollWidth')
+        required_height = driver.execute_script('return document.body.parentNode.scrollHeight')
+        driver.set_window_size(required_width, required_height)
+
         outputs_path.mkdir(exist_ok=True)
         screenshot_filepath = os.path.join(var.OUTPUTS_DIR, screenshot_name)
 
         # a little hack to prevent overwriting screenshots saved in the same second
         if os.path.exists(screenshot_filepath):
             save_screenshot(driver, postfix + '_')
             return
 
-        _LOGGER.debug(
+        _LOGGER.info(
             f'Saving screenshot to {screenshot_filepath}. Make sure to cover your credentials if you share it with others.')
         driver.get_screenshot_as_file(screenshot_filepath)
     except Exception as e:
         _LOGGER.exception(f"Exception while saving screenshot: {str(e)} for screenshot: {screenshot_name}")
 
 
+def identify_trigger(trigger, elements) -> Optional[str]:
+    if trigger.get_attribute('id') == elements['TWO_FA_EL_ID']:
+        return elements['TWO_FA_EL_ID']
+
+    if trigger.get_attribute('id') == elements['TWO_FA_SELECT_EL_ID']:
+        return elements['TWO_FA_SELECT_EL_ID']
+
+    if elements['ERROR_EL'] in trigger.get_attribute('class'):
+        return elements['ERROR_EL']
+
+    if elements['TWO_FA_NOTIFICATION_EL'] in trigger.get_attribute('class'):
+        return elements['TWO_FA_NOTIFICATION_EL']
+
+    if elements['IBKEY_PROMO_EL_CLASS'] in trigger.get_attribute('class'):
+        return elements['IBKEY_PROMO_EL_CLASS']
+
+    if trigger.text == elements['SUCCESS_EL_TEXT']:
+        return elements['SUCCESS_EL_TEXT']
+
+    raise RuntimeError(f'Trigger found but cannot be identified: {trigger} :: {trigger.get_attribute("outerHTML")}')
+
+
+def check_version(driver) -> int:
+    """ Check for the IBRK website version. Currently, there are various versions shown to users and we want to know which one we are operating on.
+
+    Versions:
+
+    * 1 = available until March 2023
+    * 2 = available from March 2023
+    """
+
+    try:
+        user_name_present = EC.presence_of_element_located((By.NAME, 'user_name'))
+        WebDriverWait(driver, 5).until(user_name_present)
+        return 1
+    except TimeoutException as e:
+        pass
+
+    try:
+        user_name_present = EC.presence_of_element_located((By.NAME, 'username'))
+        WebDriverWait(driver, 5).until(user_name_present)
+        return 2
+    except TimeoutException as e:
+        pass
+
+    _LOGGER.warning(f'Cannot determine the version of IBKR website, assuming version 1')
+
+    return 1
+
+
+def create_elements(versions: dict):
+    elements = {}
+    elements['USER_NAME_EL'] = versions['USER_NAME_EL']
+    elements['PASSWORD_EL'] = var.PASSWORD_EL
+    elements['SUBMIT_EL'] = var.SUBMIT_EL
+    elements['ERROR_EL'] = versions['ERROR_EL']
+    elements['SUCCESS_EL_TEXT'] = var.SUCCESS_EL_TEXT
+    elements['IBKEY_PROMO_EL_CLASS'] = var.IBKEY_PROMO_EL_CLASS
+    elements['TWO_FA_EL_ID'] = var.TWO_FA_EL_ID
+    elements['TWO_FA_NOTIFICATION_EL'] = var.TWO_FA_NOTIFICATION_EL
+    elements['TWO_FA_INPUT_EL_ID'] = var.TWO_FA_INPUT_EL_ID
+    elements['TWO_FA_SELECT_EL_ID'] = var.TWO_FA_SELECT_EL_ID
+
+    if var.USER_NAME_EL is not None:
+        elements['USER_NAME_EL'] = var.USER_NAME_EL
+
+    if var.ERROR_EL is not None:
+        elements['ERROR_EL'] = var.ERROR_EL
+
+    return elements
+
+
 def authenticate_gateway(driver_path,
                          account,
                          password,
                          key: str = None,
                          base_url: str = None,
                          two_fa_handler: TwoFaHandler = None) -> (bool, bool):
     """
@@ -143,127 +231,175 @@
     :rtype: (bool, bool)
     """
     base_url = base_url if base_url is not None else var.GATEWAY_BASE_URL
     display = None
     success = False
     driver = None
     try:
-        _LOGGER.debug(f'Loading auth webpage at {base_url + var.ROUTE_AUTH}')
+        _LOGGER.info(f'Loading auth webpage at {base_url + var.ROUTE_AUTH}')
         if sys.platform == 'linux':
             display = Display(visible=0, size=(800, 600))
             display.start()
 
         driver = start_driver(base_url, driver_path)
         if driver is None:
             return False, False
 
         driver.get(base_url + var.ROUTE_AUTH)
-        
+
+        website_version = check_version(driver)
+
+        elements = create_elements(_VERSIONS[website_version])
+
         # wait for the page to load
-        user_name_present = EC.presence_of_element_located((By.ID, var.USER_NAME_EL_ID))
+        user_name_present = EC.presence_of_element_located((By.NAME, elements['USER_NAME_EL']))
         WebDriverWait(driver, 15).until(user_name_present)
-        _LOGGER.debug('Gateway auth webpage loaded')
+        _LOGGER.info('Gateway auth webpage loaded')
 
         immediate_attempts = 0
 
         while immediate_attempts < max(var.MAX_IMMEDIATE_ATTEMPTS, 1):
             immediate_attempts += 1
-            _LOGGER.debug(f'Login attempt number {immediate_attempts}')
+            _LOGGER.info(f'Login attempt number {immediate_attempts}')
 
             # time.sleep(300)
 
             # input credentials
-            user_name_el = driver.find_element_by_id(var.USER_NAME_EL_ID)
-            password_el = driver.find_element_by_id(var.PASSWORD_EL_ID)
+            user_name_el = driver.find_element_by_name(elements['USER_NAME_EL'])
+            password_el = driver.find_element_by_name(elements['PASSWORD_EL'])
             user_name_el.send_keys(account)
 
             if key is None:
                 password_el.send_keys(password)
             else:
                 password_el.send_keys(Fernet(key).decrypt(password.encode('utf-8')).decode("utf-8"))
 
             password_el.send_keys(Keys.TAB)
 
             # small buffer to prevent race-condition on client side
             time.sleep(5)
             # submit the form
-            _LOGGER.debug('Submitting the form')
-            submit_form_el = driver.find_element_by_id(var.SUBMIT_EL_ID)
+            _LOGGER.info('Submitting the form')
+            submit_form_el = driver.find_element_by_css_selector(elements['SUBMIT_EL'])
             submit_form_el.click()
 
             # observe results - either success or 2FA request
             success_present = text_to_be_present_in_element([(By.TAG_NAME, 'pre'), (By.TAG_NAME, 'body')],
-                                                            var.SUCCESS_EL_TEXT)
-            two_factor_input_present = EC.visibility_of_element_located((By.ID, var.TWO_FA_EL_ID))
-            error_displayed = EC.visibility_of_element_located((By.ID, var.ERROR_EL_ID))
-            ibkey_promo_skip_clickable = EC.element_to_be_clickable((By.CLASS_NAME, var.IBKEY_PROMO_EL_CLASS))
+                                                            elements['SUCCESS_EL_TEXT'])
+            two_factor_input_present = EC.visibility_of_element_located((By.ID, elements['TWO_FA_EL_ID']))
 
-            trigger = WebDriverWait(driver, var.OAUTH_TIMEOUT).until(
-                any_of(success_present, two_factor_input_present, error_displayed, ibkey_promo_skip_clickable))
+            two_factor_select_present = EC.visibility_of_element_located((By.ID, elements['TWO_FA_SELECT_EL_ID']))
+
+            two_factor_notification = EC.visibility_of_element_located((By.CLASS_NAME, elements['TWO_FA_NOTIFICATION_EL']))
 
-            trigger_id = trigger.get_attribute('id')
+            error_displayed = EC.visibility_of_element_located((By.CSS_SELECTOR, '.' + elements['ERROR_EL'].replace(' ', '.')))
+            ibkey_promo_skip_clickable = EC.element_to_be_clickable((By.CLASS_NAME, elements['IBKEY_PROMO_EL_CLASS']))
+
+            trigger = WebDriverWait(driver, var.OAUTH_TIMEOUT).until(
+                any_of(success_present,
+                       two_factor_input_present,
+                       two_factor_select_present,
+                       two_factor_notification,
+                       error_displayed,
+                       ibkey_promo_skip_clickable))
+
+            trigger_identifier = identify_trigger(trigger, elements)
+            _LOGGER.debug(f'trigger: {trigger_identifier}')
+
+            if trigger_identifier == elements['TWO_FA_SELECT_EL_ID']:
+                _LOGGER.info(f'Required to select a 2FA method.')
+                select_el = driver.find_element_by_id(elements['TWO_FA_SELECT_EL_ID'])
+                select = Select(select_el)
+                select.select_by_visible_text(var.TWO_FA_SELECT_TARGET)
+
+                trigger = WebDriverWait(driver, var.OAUTH_TIMEOUT).until(
+                    any_of(success_present,
+                           two_factor_input_present,
+                           two_factor_notification,
+                           error_displayed,
+                           ibkey_promo_skip_clickable))
+
+                _LOGGER.info(f'2FA method "{var.TWO_FA_SELECT_TARGET}" selected successfully.')
+
+                trigger_identifier = identify_trigger(trigger, elements)
+                _LOGGER.debug(f'trigger: {trigger_identifier}')
+
+            if trigger_identifier == elements['TWO_FA_NOTIFICATION_EL']:
+                _LOGGER.info(f'Credentials correct, but Gateway requires notification two-factor authentication.')
+
+                if two_fa_handler is not None:
+                    two_fa_success = two_fa_handler.get_two_fa_code(driver)
+                    if not two_fa_success:
+                        driver.refresh()
+                        continue  # attempt a direct retry
+
+                trigger = WebDriverWait(driver, var.OAUTH_TIMEOUT).until(
+                    any_of(success_present, ibkey_promo_skip_clickable, error_displayed))
+                trigger_identifier = identify_trigger(trigger, elements)
 
             # handle 2FA
-            if trigger_id == var.TWO_FA_EL_ID:
+            if trigger_identifier == elements['TWO_FA_EL_ID']:
                 _LOGGER.info(f'Credentials correct, but Gateway requires two-factor authentication.')
                 if two_fa_handler is None:
                     _LOGGER.critical(
                         f'######## ATTENTION! ######## No 2FA handler found. You may define your own 2FA handler or use built-in handlers. See documentation for more: https://github.com/Voyz/ibeam/wiki/Two-Factor-Authentication')
                     return False, True
 
                 two_fa_code = handle_two_fa(two_fa_handler)
 
                 if two_fa_code is None:
                     _LOGGER.warning(f'No 2FA code returned. Aborting authentication.')
                 else:
-                    two_fa_el = driver.find_elements_by_id(var.TWO_FA_INPUT_EL_ID)
+                    two_fa_el = driver.find_elements_by_id(elements['TWO_FA_INPUT_EL_ID'])
                     WebDriverWait(driver, var.OAUTH_TIMEOUT).until(
-                        EC.element_to_be_clickable((By.ID, var.TWO_FA_INPUT_EL_ID)))
+                        EC.element_to_be_clickable((By.ID, elements['TWO_FA_INPUT_EL_ID'])))
                     two_fa_el[0].send_keys(two_fa_code)
 
-                    _LOGGER.debug('Submitting the 2FA form')
-                    submit_form_el = driver.find_element_by_id(var.SUBMIT_EL_ID)
+                    _LOGGER.info('Submitting the 2FA form')
+                    submit_form_el = driver.find_element_by_css_selector(elements['SUBMIT_EL'])
                     WebDriverWait(driver, var.OAUTH_TIMEOUT).until(
-                        EC.element_to_be_clickable((By.ID, var.SUBMIT_EL_ID)))
+                        EC.element_to_be_clickable((By.CSS_SELECTOR, elements['SUBMIT_EL'])))
                     submit_form_el.click()
 
                     trigger = WebDriverWait(driver, var.OAUTH_TIMEOUT).until(
                         any_of(success_present, ibkey_promo_skip_clickable, error_displayed))
-                    trigger_id = trigger.get_attribute('id')
-            
+                    trigger_identifier = identify_trigger(trigger, elements)
+
             trigger_class = trigger.get_attribute('class')
 
-            if trigger_class == var.IBKEY_PROMO_EL_CLASS:
-                _LOGGER.debug('Handling IB-Key promo display...')
+            if elements['IBKEY_PROMO_EL_CLASS'] in trigger_class:
+                _LOGGER.info('Handling IB-Key promo display...')
                 trigger.click()
-                WebDriverWait(driver, 10).until(success_present)
+                trigger = WebDriverWait(driver, 10).until(any_of(success_present, error_displayed))
+                trigger_identifier = identify_trigger(trigger, elements)
 
-            if trigger_id == var.ERROR_EL_ID:
+            if trigger_identifier == elements['ERROR_EL']:
                 _LOGGER.error(f'Error displayed by the login webpage: {trigger.text}')
                 save_screenshot(driver, '__failed_attempt')
 
                 # try to prevent having the account locked-out
                 if trigger.text == 'failed' or trigger.text == 'Invalid username password combination' and var.MAX_FAILED_AUTH > 0:
                     global _FAILED_ATTEMPTS
                     _FAILED_ATTEMPTS += 1
                     if _FAILED_ATTEMPTS >= var.MAX_FAILED_AUTH:
                         _LOGGER.critical(
                             f'######## ATTENTION! ######## Maximum number of failed authentication attempts (IBEAM_MAX_FAILED_AUTH={var.MAX_FAILED_AUTH}) reached. IBeam will shut down to prevent an account lock-out. It is recommended you attempt to authenticate manually in order to reset the counter. Read the execution logs and report issues at https://github.com/Voyz/ibeam/issues')
                         return False, True
 
                 time.sleep(1)
-                continue  # trigger retry
+                continue  # attempt a direct retry
 
-            elif trigger_id == var.TWO_FA_EL_ID:
+            elif trigger_identifier == elements['TWO_FA_EL_ID']:
                 time.sleep(1)
-                continue  # trigger retry
+                driver.refresh()
+                continue  # attempt a direct retry
                 pass  # this means no two_fa_code was returned and trigger remained the same - ie. don't authenticate
                 # todo: retry authentication or resend code
-            else:
-                _LOGGER.debug('Webpage displayed "Client login succeeds"')
+            elif trigger_identifier == elements['SUCCESS_EL_TEXT']:
+                _LOGGER.info('Webpage displayed "Client login succeeds"')
                 _FAILED_ATTEMPTS = 0
                 success = True
                 break
 
         time.sleep(2)
     except TimeoutException as e:
         exception_line = traceback.format_tb(sys.exc_info()[2])[0].replace('\n', '')
@@ -276,15 +412,15 @@
             raise RuntimeError('Error encountered during authentication') from e
         except Exception as full_e:
             _LOGGER.exception(full_e)
             save_screenshot(driver, '__generic-exception')
             success = False
     finally:
         # if sys.platform == 'linux' and display is not None:
-        _LOGGER.debug(f'Cleaning up the resources. Display: {display} | Driver: {driver}')
+        _LOGGER.info(f'Cleaning up the resources. Display: {display} | Driver: {driver}')
 
         if display is not None:
             display.stop()
 
         if driver is not None:
             release_chrome_driver(driver)
```

### Comparing `ibeam-0.4.3/ibeam/src/gateway_client.py` & `ibeam-0.4.4/ibeam/src/gateway_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -207,19 +207,19 @@
             t_end = time.time() + var.GATEWAY_STARTUP
             ping_success = False
             while time.time() < t_end:
                 status = self.http_handler.try_request(self.base_url, False)
                 if not status.running:
                     seconds_remaining = round(t_end - time.time())
                     if seconds_remaining > 0:
-                        _LOGGER.debug(
+                        _LOGGER.info(
                             f'Cannot ping Gateway. Retrying for another {seconds_remaining} seconds')
                         time.sleep(1)
                 else:
-                    _LOGGER.debug('Gateway connection established')
+                    _LOGGER.info('Gateway connection established')
                     ping_success = True
                     break
 
             if not ping_success:
                 _LOGGER.error('Gateway process found but cannot establish a connection with the Gateway')
 
         return processes[0].pid
@@ -348,18 +348,18 @@
         self._scheduler.start()
         try:
             while True:
                 time.sleep(1)
         except KeyboardInterrupt as e:
             _LOGGER.info('Keyboard interrupt, shutting down.')
             pass
-        self._scheduler.shutdown(True)
+        self._scheduler.shutdown(False)
 
     def _maintenance(self):
-        _LOGGER.debug('Maintenance')
+        _LOGGER.info('Maintenance')
 
         success, shutdown = self.start_and_authenticate(request_retries=var.REQUEST_RETRIES)
 
         if shutdown:
             _LOGGER.warning('Shutting IBeam down due to critical error.')
             self._scheduler.remove_all_jobs()
             self._scheduler.shutdown(False)
```

### Comparing `ibeam-0.4.3/ibeam/src/health_server.py` & `ibeam-0.4.4/ibeam/src/health_server.py`

 * *Files identical despite different names*

### Comparing `ibeam-0.4.3/ibeam/src/http_handler.py` & `ibeam-0.4.4/ibeam/src/http_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,14 +78,18 @@
             except HTTPError as e:
                 status.running = True
 
                 if e.code == 401:
                     # we expect this error, no need to log
                     pass
 
+                elif e.code == 500 and 'Internal Server Error' in str(e):
+                    _LOGGER.error(f'IBKR server error: "{e}". One of reasons for this error is IBKR server restart.')
+                    status.session = False  # ensure we reauthenticate
+
                 else:  # todo: possibly other codes could appear when not authenticated, fix when necessary
                     try:
                         raise RuntimeError('Unrecognised HTTPError') from e
                     except Exception as ee:
                         _LOGGER.exception(ee)
 
             except (URLError, socket.timeout) as e:
@@ -144,19 +148,19 @@
                 except Exception as ee:
                     _LOGGER.exception(ee)
 
             if max_attempts <= 1:
                 return status
             else:
                 if attempt >= max_attempts - 1:
-                    _LOGGER.debug(
+                    _LOGGER.info(
                         f'Max validate request retries reached after {max_attempts} attempts. Consider increasing the retries by setting IBEAM_REQUEST_RETRIES environment variable')
                     return status
                 else:
-                    _LOGGER.debug(f'Attempt number {attempt + 2}')
+                    _LOGGER.info(f'Attempt number {attempt + 2}')
                     return _request(attempt + 1)
 
         return _request(0)
 
     def __getstate__(self):
         state = self.__dict__.copy()
         # ssl_context can't be pickled
```

### Comparing `ibeam-0.4.3/ibeam/src/inputs_handler.py` & `ibeam-0.4.4/ibeam/src/inputs_handler.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         self.gateway_dir = gateway_dir
 
         self.cecert_jks_path = os.path.join(inputs_dir, 'cacert.jks')
         self.cecert_pem_path = os.path.join(inputs_dir, 'cacert.pem')
 
         self.valid_certificates = os.path.isfile(self.cecert_jks_path) and os.path.isfile(self.cecert_pem_path)
         if self.valid_certificates:
-            _LOGGER.debug('Certificates found and will be used for TLS verification')
+            _LOGGER.info('TLS certificates found and will be used for verification')
 
         gateway_root_dir = os.path.join(self.gateway_dir, 'root')
 
         config_source = os.path.join(self.inputs_dir, 'conf.yaml')
         if os.path.isfile(config_source):
             _LOGGER.info('Custom conf.yaml found and will be used by the Gateway')
             config_target = os.path.join(gateway_root_dir, 'conf.yaml')
```

### Comparing `ibeam-0.4.3/ibeam/src/logs.py` & `ibeam-0.4.4/ibeam/src/logs.py`

 * *Files identical despite different names*

### Comparing `ibeam-0.4.3/ibeam/src/process_utils.py` & `ibeam-0.4.4/ibeam/src/process_utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -30,24 +30,24 @@
 
 
 def start_gateway(gateway_dir):
     creationflags = 0  # when not on Windows, we send 0 to avoid errors.
 
     if sys.platform == 'win32':
         args = ["cmd", "/k", r"bin\run.bat", r"root\conf.yaml"]
-        _LOGGER.debug(f'Starting Windows process with params: {args}')
+        _LOGGER.info(f'Starting Gateway as Windows process with params: {args}')
         creationflags = subprocess.CREATE_NEW_CONSOLE
 
     elif sys.platform == 'darwin':
         args = ["open", "-F", "-a", "Terminal", r"bin/run.sh", r"root/conf.yaml"]
-        _LOGGER.debug(f'Starting Mac process with params: {args}')
+        _LOGGER.info(f'Starting Gateway as Mac process with params: {args}')
 
     elif sys.platform == 'linux':
         args = ["bash", r"bin/run.sh", r"root/conf.yaml"]
-        _LOGGER.debug(f'Starting Linux process with params: {args}')
+        _LOGGER.info(f'Starting Gateway as Linux process with params: {args}')
 
     else:
         raise EnvironmentError(f'Unknown platform: {sys.platform}')
 
     subprocess.Popen(
         args=args,
         cwd=gateway_dir,
```

### Comparing `ibeam-0.4.3/ibeam/src/two_fa_handlers/external_request_handler.py` & `ibeam-0.4.4/ibeam/src/two_fa_handlers/external_request_handler.py`

 * *Files identical despite different names*

### Comparing `ibeam-0.4.3/ibeam/src/two_fa_handlers/google_msg_handler.py` & `ibeam-0.4.4/ibeam/src/two_fa_handlers/google_msg_handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,17 +14,20 @@
 
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support import expected_conditions as EC
 from selenium.webdriver.support.wait import WebDriverWait
 
 _LOGGER = logging.getLogger('ibeam.' + Path(__file__).stem)
 
-_GOOG_QR_CODE_CLASS = os.environ.get('IBEAM_GOOG_QR_CODE_CLASS', 'qr-code')
+_GOOG_QR_CODE_CLASS = os.environ.get('IBEAM_GOOG_QR_CODE_CLASS', 'bigger-qr-code')
 """HTML element indicating web messages needs authorization."""
 
+_GOOG_QR_CODE_DATA = os.environ.get('IBEAM_GOOG_QR_CODE_DATA', 'qr-code')
+"""HTML data attribute with the qr code."""
+
 _GOOG_AUTH_REMEMBER_CLASS = os.environ.get('IBEAM_GOOG_AUTH_REMEMBER_CLASS', 'local-storage-checkbox')
 """HTML element to remember web messages device pairing."""
 
 _GOOG_MESSAGES_LIST_CLASS = os.environ.get('IBEAM_GOOG_MESSAGES_LIST_CLASS', '.text-content.unread .snippet-text')
 """HTML element indicating web messages has loaded."""
 
 _GOOG_2FA_HEADING = os.environ.get('IBEAM_GOOG_2FA_HEADING', 'Your requested authentication code')
@@ -38,74 +41,82 @@
 
     def __init__(self, driver_path):
         self.driver_path = driver_path
 
     def get_two_fa_code(self) -> Union[str, None]:
         code_two_fa = None
 
-        driver_2fa = new_chrome_driver(self.driver_path, name='google_msg')
+        driver_2fa = new_chrome_driver(self.driver_path, name='google_msg', incognito=False)
         if driver_2fa is None:
             return None
 
-        driver_2fa.get('https://messages.google.com/web')
+        try:
+            driver_2fa.get('https://messages.google.com/web')
+
+            sms_auth_present = EC.presence_of_element_located((By.CLASS_NAME, _GOOG_QR_CODE_CLASS))
+            sms_code_present = EC.text_to_be_present_in_element((By.CSS_SELECTOR, _GOOG_MESSAGES_LIST_CLASS),
+                                                                _GOOG_2FA_HEADING)
+
+            WebDriverWait(driver_2fa, 240).until(any_of(sms_auth_present, sms_code_present))
 
-        sms_auth_present = EC.presence_of_element_located((By.CLASS_NAME, _GOOG_QR_CODE_CLASS))
-        sms_code_present = EC.text_to_be_present_in_element((By.CSS_SELECTOR, _GOOG_MESSAGES_LIST_CLASS),
-                                                            _GOOG_2FA_HEADING)
+            sms_auth_el = driver_2fa.find_elements_by_class_name(_GOOG_QR_CODE_CLASS)
 
-        WebDriverWait(driver_2fa, 240).until(any_of(sms_auth_present, sms_code_present))
+            if sms_auth_el:
+                driver_2fa.find_element_by_class_name(_GOOG_AUTH_REMEMBER_CLASS).click()
 
-        sms_auth_el = driver_2fa.find_elements_by_class_name(_GOOG_QR_CODE_CLASS)
+                data = urllib.parse.quote(sms_auth_el[0].get_attribute('data-' + _GOOG_QR_CODE_DATA))
 
-        if sms_auth_el:
-            driver_2fa.find_element_by_class_name(_GOOG_AUTH_REMEMBER_CLASS).click()
+                _LOGGER.info(
+                    'Web messages is not authenticated. Open this URL to pair web messages with your android phone:')
+                _LOGGER.info(
+                    f'http://api.qrserver.com/v1/create-qr-code/?color=000000&bgcolor=FFFFFF&qzone=1&margin=0&size=400x400&ecc=L&data={data}')
 
-            data = urllib.parse.quote(sms_auth_el[0].get_attribute('data-' + _GOOG_QR_CODE_CLASS))
+                WebDriverWait(driver_2fa, 120).until(sms_code_present)
 
-            _LOGGER.info(
-                'Web messages is not authenticated. Open this URL to pair web messages with your android phone:')
-            _LOGGER.info(
-                f'http://api.qrserver.com/v1/create-qr-code/?color=000000&bgcolor=FFFFFF&qzone=1&margin=0&size=400x400&ecc=L&data={data}')
+            sms_list_el = driver_2fa.find_elements_by_css_selector(_GOOG_MESSAGES_LIST_CLASS)
 
-            WebDriverWait(driver_2fa, 120).until(sms_code_present)
+            if not sms_list_el:
+                _LOGGER.error('Timeout or authentication error while loading sms messages.')
+                save_screenshot(driver_2fa, postfix='__google_2fa')
+            else:
+                _LOGGER.info(f'First SMS found: "{sms_list_el[0].text}"')
 
-        sms_list_el = driver_2fa.find_elements_by_css_selector(_GOOG_MESSAGES_LIST_CLASS)
+                code_two_fa = re.search(r'(\d+)', sms_list_el[0].text).group(1)
 
-        if not sms_list_el:
-            _LOGGER.error('Timeout or authentication error while loading sms messages.')
-            save_screenshot(driver_2fa, postfix='__google_2fa')
-        else:
-            _LOGGER.info(sms_list_el[0].text)
-            code_two_fa = re.search(r'(\d+)', sms_list_el[0].text).group(1)
-            _LOGGER.debug('Waiting for SMS message to be visible')
-            WebDriverWait(driver_2fa, 30).until(EC.visibility_of(sms_list_el[0]))
+                _LOGGER.info('Waiting for SMS message to be visible')
+                WebDriverWait(driver_2fa, 30).until(EC.visibility_of(sms_list_el[0]))
 
-            clicked_ok = False
-            for i in range(_GOOG_MESSAGE_CLICK_RETRIES):
-                try:
-                    sms_list_el[0].click()  # mark message as read
-                    clicked_ok = True
-                    _LOGGER.debug('SMS message marked as read')
-                    break
-                except ElementClickInterceptedException as e:
-                    if isinstance(e, ElementClickInterceptedException) \
-                            and 'Other element would receive the click' in str(e):
-                        _LOGGER.warning(f'Failed marking SMS message as read due to obstructing elements')
-                    else:
-                        _LOGGER.exception(f'Exception while marking SMS message as read: {e}')
+                clicked_ok = False
+                for i in range(_GOOG_MESSAGE_CLICK_RETRIES):
+                    try:
+                        sms_list_el[0].click()  # mark message as read
+                        clicked_ok = True
+                        _LOGGER.info('SMS message marked as read')
+                        break
+                    except ElementClickInterceptedException as e:
+                        if isinstance(e, ElementClickInterceptedException) \
+                                and 'Other element would receive the click' in str(e):
+                            _LOGGER.warning(f'Failed marking SMS message as read due to obstructing elements')
+                        else:
+                            _LOGGER.exception(f'Exception while marking SMS message as read: {e}')
 
-                    save_screenshot(driver_2fa, postfix='__google_2fa')
+                        save_screenshot(driver_2fa, postfix='__google_2fa')
 
-                    _LOGGER.debug(f'Retrying clicking SMS message {_GOOG_MESSAGE_CLICK_RETRIES - i - 1} more times.')
-                    time.sleep(2)
+                        _LOGGER.info(f'Retrying clicking SMS message {_GOOG_MESSAGE_CLICK_RETRIES - i - 1} more times.')
+                        time.sleep(2)
 
-            if not clicked_ok:
-                _LOGGER.warning('Failed all attempts to mark SMS message as read')
+                if not clicked_ok:
+                    _LOGGER.warning('Failed all attempts to mark SMS message as read')
 
-            time.sleep(2)  # wait for click to mark message as read
+                time.sleep(2)  # wait for click to mark message as read
 
-        release_chrome_driver(driver_2fa)
+        except:
+            save_screenshot(driver_2fa, '__google-msg')
+            raise
+        finally:
+            _LOGGER.info(f'Cleaning up the resources. Google MSG Driver: {driver_2fa}')
+            release_chrome_driver(driver_2fa)
 
         return code_two_fa
 
     def __str__(self):
         return f"GoogleMessagesTwoFaHandler(driver_path={self.driver_path})"
```

### Comparing `ibeam-0.4.3/ibeam/src/two_fa_selector.py` & `ibeam-0.4.4/ibeam/src/two_fa_selector.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,27 +4,30 @@
 from pathlib import Path
 from typing import Union
 
 from ibeam.src import var
 from ibeam.src.inputs_handler import InputsHandler
 from ibeam.src.two_fa_handlers.external_request_handler import ExternalRequestTwoFaHandler
 from ibeam.src.two_fa_handlers.google_msg_handler import GoogleMessagesTwoFaHandler
+from ibeam.src.two_fa_handlers.notification_resend_handler import NotificationResendTwoFaHandler
 from ibeam.src.two_fa_handlers.two_fa_handler import TwoFaHandler
 
 _CUSTOM_TWO_FA_HANDLER = os.environ.get('IBEAM_CUSTOM_TWO_FA_HANDLER', 'custom_two_fa_handler.CustomTwoFaHandler')
 """Fully qualified path of the custom 2FA handler in the inputs directory."""
 
 
 def select(driver_path, inputs_handler: InputsHandler) -> Union[TwoFaHandler, None]:
     handler_name = var.TWO_FA_HANDLER
 
     if handler_name == 'GOOGLE_MSG':
         handler = GoogleMessagesTwoFaHandler(driver_path)
     elif handler_name == 'EXTERNAL_REQUEST':
         handler = ExternalRequestTwoFaHandler()
+    elif handler_name == 'NOTIFICATION_RESEND':
+        handler = NotificationResendTwoFaHandler()
     elif handler_name == 'CUSTOM_HANDLER':
         handler = load_custom_two_fa_handler(_CUSTOM_TWO_FA_HANDLER, inputs_handler)()
     else:
         handler = None
 
     return handler
```

### Comparing `ibeam-0.4.3/ibeam/src/var.py` & `ibeam-0.4.4/ibeam/src/var.py`

 * *Files 12% similar despite different names*

```diff
@@ -74,25 +74,25 @@
 """Gateway route with tickle call."""
 
 ROUTE_LOGOUT = os.environ.get('IBEAM_ROUTE_LOGOUT', '/v1/api/logout')
 """Gateway route with logout call."""
 
 ########### AUTHENTICATION ###########
 
-USER_NAME_EL_ID = os.environ.get('IBEAM_USER_NAME_EL_ID', 'user_name')
-"""HTML element id containing the username input field."""
+USER_NAME_EL = os.environ.get('IBEAM_USER_NAME_EL', None)
+"""HTML element name attribute containing the username input field."""
 
-PASSWORD_EL_ID = os.environ.get('IBEAM_PASSWORD_EL_ID', 'password')
-"""HTML element id containing the password input field."""
+PASSWORD_EL = os.environ.get('IBEAM_PASSWORD_EL', 'password')
+"""HTML element name attribute containing the password input field."""
 
-SUBMIT_EL_ID = os.environ.get('IBEAM_SUBMIT_EL_ID', 'submitForm')
-"""HTML element id containing the submit button."""
+SUBMIT_EL = os.environ.get('IBEAM_SUBMIT_EL', 'button.btn.btn-lg.btn-primary')
+"""HTML element name attribute containing the submit button."""
 
-ERROR_EL_ID = os.environ.get('IBEAM_ERROR_EL_ID', 'ERRORMSG')
-"""HTML element id containing the submit button."""
+ERROR_EL = os.environ.get('IBEAM_ERROR_EL', None)
+"""HTML element class name attribute containing the submit button."""
 
 SUCCESS_EL_TEXT = os.environ.get('IBEAM_SUCCESS_EL_TEXT', 'Client login succeeds')
 """HTML element text indicating successful authentication."""
 
 OAUTH_TIMEOUT = int(os.environ.get('IBEAM_OAUTH_TIMEOUT', 15))
 """How many seconds to wait for the OAuth login request to complete."""
 
@@ -110,19 +110,28 @@
 
 IBKEY_PROMO_EL_CLASS = os.environ.get('IBEAM_IBKEY_PROMO_EL_CLASS', 'ibkey-promo-skip')
 """HTML element class containing the ibkey promo skip button."""
 
 ########### TWO-FACTOR AUTHENTICATION ###########
 
 TWO_FA_EL_ID = os.environ.get('IBEAM_TWO_FA_EL_ID', 'twofactbase')
-"""HTML element check for if Gateway will require 2FA authentication."""
+"""HTML element check for if Gateway will require 2FA code authentication."""
+
+TWO_FA_NOTIFICATION_EL = os.environ.get('IBEAM_TWO_FA_NOTIFICATION_EL', 'login-step-notification')
+"""HTML element check for if Gateway will require 2FA notification authentication."""
 
 TWO_FA_INPUT_EL_ID = os.environ.get('IBEAM_TWO_FA_INPUT_EL_ID', 'chlginput')
 """HTML element to input 2FA code into"""
 
 TWO_FA_HANDLER = os.environ.get('IBEAM_TWO_FA_HANDLER', None)
 """Which 2FA handler should be used to acquire the code."""
 
 STRICT_TWO_FA_CODE = bool(os.environ.get('IBEAM_STRICT_TWO_FA_CODE', True))
 """Whether to ensure only 2FA code made of 6 digits can be used."""
 
+TWO_FA_SELECT_EL_ID = os.environ.get('IBEAM_TWO_FA_SELECT_EL_ID', 'sf_select')
+"""HTML element check for if Gateway requires to select the 2FA method."""
+
+TWO_FA_SELECT_TARGET = os.environ.get('IBEAM_TWO_FA_SELECT_TARGET', 'IB Key')
+"""Option that is to be chosen in the 2FA select dropdown"""
+
 all_variables = {item: value for item, value in vars().items() if (not item.startswith("__") and item.isupper())}
```

### Comparing `ibeam-0.4.3/ibeam.egg-info/SOURCES.txt` & `ibeam-0.4.4/ibeam.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -19,8 +19,9 @@
 ibeam/src/logs.py
 ibeam/src/process_utils.py
 ibeam/src/two_fa_selector.py
 ibeam/src/var.py
 ibeam/src/two_fa_handlers/__init__.py
 ibeam/src/two_fa_handlers/external_request_handler.py
 ibeam/src/two_fa_handlers/google_msg_handler.py
+ibeam/src/two_fa_handlers/notification_resend_handler.py
 ibeam/src/two_fa_handlers/two_fa_handler.py
```

### Comparing `ibeam-0.4.3/setup.py` & `ibeam-0.4.4/setup.py`

 * *Files identical despite different names*

