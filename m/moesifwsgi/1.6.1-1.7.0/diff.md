# Comparing `tmp/moesifwsgi-1.6.1.tar.gz` & `tmp/moesifwsgi-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/moesifwsgi-1.6.1.tar", last modified: Thu Apr 20 01:34:17 2023, max compression
+gzip compressed data, was "moesifwsgi-1.7.0.tar", last modified: Tue May 16 00:37:58 2023, max compression
```

## Comparing `moesifwsgi-1.6.1.tar` & `moesifwsgi-1.7.0.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 keyur      (501) staff       (20)        0 2023-04-20 01:34:17.931962 moesifwsgi-1.6.1/
--rwxr-xr-x   0 keyur      (501) staff       (20)    11911 2020-06-25 11:08:31.000000 moesifwsgi-1.6.1/LICENSE
--rw-r--r--   0 keyur      (501) staff       (20)       61 2020-04-19 17:20:34.000000 moesifwsgi-1.6.1/MANIFEST.in
--rw-r--r--   0 keyur      (501) staff       (20)    20958 2023-04-20 01:34:17.932272 moesifwsgi-1.6.1/PKG-INFO
--rwxr-xr-x   0 keyur      (501) staff       (20)    16396 2023-04-19 16:52:37.000000 moesifwsgi-1.6.1/README.md
-drwxr-xr-x   0 keyur      (501) staff       (20)        0 2023-04-20 01:34:17.929460 moesifwsgi-1.6.1/moesifwsgi/
--rw-r--r--   0 keyur      (501) staff       (20)       26 2020-04-19 17:20:34.000000 moesifwsgi-1.6.1/moesifwsgi/__init__.py
--rw-r--r--   0 keyur      (501) staff       (20)     4634 2020-12-29 19:45:45.000000 moesifwsgi-1.6.1/moesifwsgi/client_ip.py
--rw-r--r--   0 keyur      (501) staff       (20)     3526 2023-04-20 01:32:27.000000 moesifwsgi-1.6.1/moesifwsgi/event_mapper.py
--rw-r--r--   0 keyur      (501) staff       (20)     1067 2023-04-20 01:32:27.000000 moesifwsgi-1.6.1/moesifwsgi/http_response_catcher.py
--rw-r--r--   0 keyur      (501) staff       (20)    10434 2023-04-20 01:32:27.000000 moesifwsgi-1.6.1/moesifwsgi/logger_helper.py
--rw-r--r--   0 keyur      (501) staff       (20)    13821 2023-04-20 01:32:27.000000 moesifwsgi-1.6.1/moesifwsgi/middleware.py
--rw-r--r--   0 keyur      (501) staff       (20)     3071 2023-04-20 01:32:27.000000 moesifwsgi-1.6.1/moesifwsgi/moesif_data_holder.py
--rw-r--r--   0 keyur      (501) staff       (20)     2344 2020-12-29 19:47:50.000000 moesifwsgi-1.6.1/moesifwsgi/parse_body.py
--rw-r--r--   0 keyur      (501) staff       (20)     4018 2022-01-13 23:06:22.000000 moesifwsgi-1.6.1/moesifwsgi/regex_config_helper.py
--rw-r--r--   0 keyur      (501) staff       (20)     2500 2023-04-20 01:32:27.000000 moesifwsgi-1.6.1/moesifwsgi/send_batch_events.py
--rw-r--r--   0 keyur      (501) staff       (20)     8531 2023-04-20 01:32:27.000000 moesifwsgi-1.6.1/moesifwsgi/update_companies.py
--rw-r--r--   0 keyur      (501) staff       (20)     8100 2023-04-20 01:32:27.000000 moesifwsgi-1.6.1/moesifwsgi/update_users.py
-drwxr-xr-x   0 keyur      (501) staff       (20)        0 2023-04-20 01:34:17.931704 moesifwsgi-1.6.1/moesifwsgi.egg-info/
--rw-r--r--   0 keyur      (501) staff       (20)    20958 2023-04-20 01:34:17.000000 moesifwsgi-1.6.1/moesifwsgi.egg-info/PKG-INFO
--rw-r--r--   0 keyur      (501) staff       (20)      562 2023-04-20 01:34:17.000000 moesifwsgi-1.6.1/moesifwsgi.egg-info/SOURCES.txt
--rw-r--r--   0 keyur      (501) staff       (20)        1 2023-04-20 01:34:17.000000 moesifwsgi-1.6.1/moesifwsgi.egg-info/dependency_links.txt
--rw-r--r--   0 keyur      (501) staff       (20)      104 2023-04-20 01:34:17.000000 moesifwsgi-1.6.1/moesifwsgi.egg-info/requires.txt
--rw-r--r--   0 keyur      (501) staff       (20)       11 2023-04-20 01:34:17.000000 moesifwsgi-1.6.1/moesifwsgi.egg-info/top_level.txt
--rw-r--r--   0 keyur      (501) staff       (20)       67 2023-04-20 01:34:17.933198 moesifwsgi-1.6.1/setup.cfg
--rw-r--r--   0 keyur      (501) staff       (20)     3370 2023-04-20 01:32:27.000000 moesifwsgi-1.6.1/setup.py
+drwxr-xr-x   0 praveen    (501) staff       (20)        0 2023-05-16 00:37:58.362638 moesifwsgi-1.7.0/
+-rwxr-xr-x   0 praveen    (501) staff       (20)    11911 2021-12-24 00:24:54.000000 moesifwsgi-1.7.0/LICENSE
+-rw-r--r--   0 praveen    (501) staff       (20)       61 2021-12-24 00:24:54.000000 moesifwsgi-1.7.0/MANIFEST.in
+-rw-r--r--   0 praveen    (501) staff       (20)    18592 2023-05-16 00:37:58.362741 moesifwsgi-1.7.0/PKG-INFO
+-rwxr-xr-x   0 praveen    (501) staff       (20)    17163 2023-05-16 00:12:53.000000 moesifwsgi-1.7.0/README.md
+drwxr-xr-x   0 praveen    (501) staff       (20)        0 2023-05-16 00:37:58.361639 moesifwsgi-1.7.0/moesifwsgi/
+-rw-r--r--   0 praveen    (501) staff       (20)       26 2021-12-24 00:24:54.000000 moesifwsgi-1.7.0/moesifwsgi/__init__.py
+-rw-r--r--   0 praveen    (501) staff       (20)     4634 2021-12-24 00:24:54.000000 moesifwsgi-1.7.0/moesifwsgi/client_ip.py
+-rw-r--r--   0 praveen    (501) staff       (20)     3784 2023-05-16 00:12:53.000000 moesifwsgi-1.7.0/moesifwsgi/config_manager.py
+-rw-r--r--   0 praveen    (501) staff       (20)     3526 2023-05-16 00:12:53.000000 moesifwsgi-1.7.0/moesifwsgi/event_mapper.py
+-rw-r--r--   0 praveen    (501) staff       (20)     1067 2023-05-16 00:12:53.000000 moesifwsgi-1.7.0/moesifwsgi/http_response_catcher.py
+-rw-r--r--   0 praveen    (501) staff       (20)    10434 2023-05-16 00:12:53.000000 moesifwsgi-1.7.0/moesifwsgi/logger_helper.py
+-rw-r--r--   0 praveen    (501) staff       (20)     9708 2023-05-16 00:12:53.000000 moesifwsgi-1.7.0/moesifwsgi/middleware.py
+-rw-r--r--   0 praveen    (501) staff       (20)     3071 2023-05-16 00:12:53.000000 moesifwsgi-1.7.0/moesifwsgi/moesif_data_holder.py
+-rw-r--r--   0 praveen    (501) staff       (20)     2344 2021-12-24 00:24:54.000000 moesifwsgi-1.7.0/moesifwsgi/parse_body.py
+-rw-r--r--   0 praveen    (501) staff       (20)     4018 2022-09-21 22:56:45.000000 moesifwsgi-1.7.0/moesifwsgi/regex_config_helper.py
+-rw-r--r--   0 praveen    (501) staff       (20)     8531 2023-05-16 00:12:53.000000 moesifwsgi-1.7.0/moesifwsgi/update_companies.py
+-rw-r--r--   0 praveen    (501) staff       (20)     8100 2023-05-16 00:12:53.000000 moesifwsgi-1.7.0/moesifwsgi/update_users.py
+-rw-r--r--   0 praveen    (501) staff       (20)     6887 2023-05-16 00:12:53.000000 moesifwsgi-1.7.0/moesifwsgi/workers.py
+drwxr-xr-x   0 praveen    (501) staff       (20)        0 2023-05-16 00:37:58.362510 moesifwsgi-1.7.0/moesifwsgi.egg-info/
+-rw-r--r--   0 praveen    (501) staff       (20)    18592 2023-05-16 00:37:58.000000 moesifwsgi-1.7.0/moesifwsgi.egg-info/PKG-INFO
+-rw-r--r--   0 praveen    (501) staff       (20)      581 2023-05-16 00:37:58.000000 moesifwsgi-1.7.0/moesifwsgi.egg-info/SOURCES.txt
+-rw-r--r--   0 praveen    (501) staff       (20)        1 2023-05-16 00:37:58.000000 moesifwsgi-1.7.0/moesifwsgi.egg-info/dependency_links.txt
+-rw-r--r--   0 praveen    (501) staff       (20)      130 2023-05-16 00:37:58.000000 moesifwsgi-1.7.0/moesifwsgi.egg-info/requires.txt
+-rw-r--r--   0 praveen    (501) staff       (20)       11 2023-05-16 00:37:58.000000 moesifwsgi-1.7.0/moesifwsgi.egg-info/top_level.txt
+-rw-r--r--   0 praveen    (501) staff       (20)       67 2023-05-16 00:37:58.363082 moesifwsgi-1.7.0/setup.cfg
+-rw-r--r--   0 praveen    (501) staff       (20)     3693 2023-05-16 00:12:53.000000 moesifwsgi-1.7.0/setup.py
```

### Comparing `moesifwsgi-1.6.1/LICENSE` & `moesifwsgi-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `moesifwsgi-1.6.1/PKG-INFO` & `moesifwsgi-1.7.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,450 +1,464 @@
 Metadata-Version: 2.1
 Name: moesifwsgi
-Version: 1.6.1
+Version: 1.7.0
 Summary: Moesif Middleware for Python WSGI based platforms (Flask, Bottle & Others)
 Home-page: https://www.moesif.com/docs/server-integration/python-wsgi/
 Author: Moesif, Inc
 Author-email: xing@moesif.com
 License: Apache Software License
-Description: # Moesif Middleware for Python WSGI based Frameworks
-        
-        [![Built For][ico-built-for]][link-built-for]
-        [![Latest Version][ico-version]][link-package]
-        [![Language Versions][ico-language]][link-language]
-        [![Software License][ico-license]][link-license]
-        [![Source Code][ico-source]][link-source]
-        
-        WSGI middleware that automatically logs _incoming_ or _outgoing_ API calls and sends to [Moesif](https://www.moesif.com) for API analytics and monitoring.
-        Supports Python Frameworks built on WSGI such as Flask, Bottle, and Pyramid.
-        
-        [Source Code on GitHub](https://github.com/moesif/moesifwsgi)
-        
-        [WSGI (Web Server Gateway Interface)](https://wsgi.readthedocs.io/en/latest/)
-        is a standard (PEP 3333) that describes
-        how a web server communicates with web applications. Many Python Frameworks
-        are build on top of WSGI, such as [Flask](http://flask.pocoo.org/),
-        [Bottle](https://bottlepy.org/docs/dev/), [Pyramid](https://trypyramid.com/) etc.
-        Moesif WSGI Middleware help APIs that are build on top of these Frameworks to
-        easily integrate with [Moesif](https://www.moesif.com).
-        
-        ## How to install
-        
-        ```shell
-        pip install moesifwsgi
-        ```
-        
-        ## How to use
-        
-        ### Flask
-        
-        Wrap your wsgi_app with the Moesif middleware.
-        
-        ```python
-        from moesifwsgi import MoesifMiddleware
-        
-        moesif_settings = {
-            'APPLICATION_ID': 'Your Moesif Application id',
-            'LOG_BODY': True,
-            # ... For other options see below.
-        }
-        
-        app.wsgi_app = MoesifMiddleware(app.wsgi_app, moesif_settings)
-        
-        ```
-        
-        Your Moesif Application Id can be found in the [_Moesif Portal_](https://www.moesif.com/).
-        After signing up for a Moesif account, your Moesif Application Id will be displayed during the onboarding steps. 
-        
-        You can always find your Moesif Application Id at any time by logging 
-        into the [_Moesif Portal_](https://www.moesif.com/), click on the top right menu,
-        and then clicking _API Keys_.
-        
-        For an example with Flask, see example in the `/examples/flask` folder of this repo.
-        
-        ### Bottle
-        Wrap your bottle app with the Moesif middleware.
-        
-        ```python
-        
-        from moesifwsgi import MoesifMiddleware
-        
-        app = bottle.Bottle()
-        
-        moesif_settings = {
-            'APPLICATION_ID': 'Your Moesif Application Id',
-            'LOG_BODY': True,
-            # ... For other options see below.
-        }
-        
-        bottle.run(app=MoesifMiddleware(app, moesif_settings))
-        
-        ```
-        
-        For an example with Bottle, see example in the `/examples/bottle` folder of this repo.
-        
-        ### Pyramid
-        
-        
-        ```python
-        from pyramid.config import Configurator
-        from moesifwsgi import MoesifMiddleware
-        
-        if __name__ == '__main__':
-            config = Configurator()
-            config.add_route('hello', '/')
-            config.scan()
-            app = config.make_wsgi_app()
-        
-            # configure your moesif settings
-            moesif_settings = {
-                'APPLICATION_ID': 'Your Moesif Application Id',
-                'LOG_BODY': True,
-                # ... For other options see below.
-            }
-            # Put middleware
-            app = MoesifMiddleware(app, moesif_settings)
-        
-            server = make_server('0.0.0.0', 8080, app)
-            server.serve_forever()
-        
-        ```
-        ### Other WSGI frameworks
-        
-        If you are using a framework that is built on top of WSGI, it should work just by adding the Moesif middleware.
-        Please read the documentation for your specific framework on how to add middleware.
-        
-        ## Configuration options
-        
-        #### __`APPLICATION_ID`__
-        (__required__), _string_, is obtained via your Moesif Account, this is required.
-        
-        #### __`SKIP`__
-        (optional) _(app, environ) => boolean_, a function that takes a WSGI app and an environ,
-        and returns true if you want to skip this particular event. The app is the original WSGI app instance, and the
-        environ is a [WSGI environ](http://wsgi.readthedocs.io/en/latest/definitions.html).
-        
-        #### __`IDENTIFY_USER`__
-        (optional, but highly recommended) _(app, environ, response_headers) => string_, a function that takes an app, an environ and an optional parameter response headers, and returns a string that is the user id used by your system. While Moesif tries to identify users automatically,
-        but different frameworks and your implementation might be very different, it would be helpful and much more accurate to provide this function.
-        
-        #### __`IDENTIFY_COMPANY`__
-        (optional) _(app, environ, response_headers) => string_, a function that takes an app, an environ and an optional parameter response headers, and returns a string that is the company id for this event.
-        
-        #### __`GET_METADATA`__
-        (optional) _(app, environ) => dictionary_, a function that takes an app and an environ, and
-        returns a dictionary (must be able to be encoded into JSON). This allows your
-        to associate this event with custom metadata. For example, you may want to save a VM instance_id, a trace_id, or a tenant_id with the request.
-        
-        #### __`GET_SESSION_TOKEN`__
-        (optional) _(app, environ) => string_, a function that takes an app and an environ, and returns a string that is the session token for this event. Again, Moesif tries to get the session token automatically, but if you setup is very different from standard, this function will be very help for tying events together, and help you replay the events.
-        
-        #### __`MASK_EVENT_MODEL`__
-        (optional) _(EventModel) => EventModel_, a function that takes an EventModel and returns an EventModel with desired data removed. The return value must be a valid EventModel required by Moesif data ingestion API. For details regarding EventModel please see the [Moesif Python API Documentation](https://www.moesif.com/docs/api?python).
-        
-        #### __`DEBUG`__
-        (optional) _boolean_, a flag to see debugging messages.
-        
-        #### __`LOG_BODY`__
-        (optional) _boolean_, default True, Set to False to remove logging request and response body.
-        
-        #### __`BATCH_SIZE`__
-        (optional) __int__, default 25, Maximum batch size when sending events to Moesif.
-        
-        #### __`AUTHORIZATION_HEADER_NAME`__
-        (optional) _string_, A request header field name used to identify the User in Moesif. Default value is `authorization`. Also, supports a comma separated string. We will check headers in order like `"X-Api-Key,Authorization"`.
-        
-        #### __`AUTHORIZATION_USER_ID_FIELD`__
-        (optional) _string_, A field name used to parse the User from authorization header in Moesif. Default value is `sub`.
-        
-        #### __`BASE_URI`__
-        (optional) _string_, A local proxy hostname when sending traffic via secure proxy. Please set this field when using secure proxy. For more details, refer [secure proxy documentation.](https://www.moesif.com/docs/platform/secure-proxy/#2-configure-moesif-sdk)
-        
-        ### Options specific to outgoing API calls 
-        
-        The options below are applicable to outgoing API calls (calls you initiate using the Python [Requests](http://docs.python-requests.org/en/master/) lib to third parties like Stripe or to your own services.
-        
-        For options that use the request and response as input arguments, these use the [Requests](http://docs.python-requests.org/en/master/api/) lib's request or response objects.
-        
-        If you are not using WSGI, you can import the [moesifpythonrequest](https://github.com/Moesif/moesifpythonrequest) directly.
-        
-        #### __`CAPTURE_OUTGOING_REQUESTS`__
-        _boolean_, Default False. Set to True to capture all outgoing API calls. False will disable this functionality. 
-        
-        ##### __`GET_METADATA_OUTGOING`__
-        (optional) _(req, res) => dictionary_, a function that enables you to return custom metadata associated with the logged API calls. 
-        Takes in the [Requests](http://docs.python-requests.org/en/master/api/) request and response object as arguments. You should implement a function that 
-        returns a dictionary containing your custom metadata. (must be able to be encoded into JSON). For example, you may want to save a VM instance_id, a trace_id, or a resource_id with the request.
-        
-        ##### __`SKIP_OUTGOING`__
-        (optional) _(req, res) => boolean_, a function that takes a [Requests](http://docs.python-requests.org/en/master/api/) request and response,
-        and returns true if you want to skip this particular event.
-        
-        ##### __`IDENTIFY_USER_OUTGOING`__
-        (optional, but highly recommended) _(req, res) => string_, a function that takes [Requests](http://docs.python-requests.org/en/master/api/) request and response, and returns a string that is the user id used by your system. While Moesif tries to identify users automatically,
-        but different frameworks and your implementation might be very different, it would be helpful and much more accurate to provide this function.
-        
-        ##### __`IDENTIFY_COMPANY_OUTGOING`__
-        (optional) _(req, res) => string_, a function that takes [Requests](http://docs.python-requests.org/en/master/api/) request and response, and returns a string that is the company id for this event.
-        
-        ##### __`GET_SESSION_TOKEN_OUTGOING`__
-        (optional) _(req, res) => string_, a function that takes [Requests](http://docs.python-requests.org/en/master/api/) request and response, and returns a string that is the session token for this event. Again, Moesif tries to get the session token automatically, but if you setup is very different from standard, this function will be very help for tying events together, and help you replay the events.
-        
-        ##### __`LOG_BODY_OUTGOING`__
-        (optional) _boolean_, default True, Set to False to remove logging request and response body.
-        
-        ### Example:
-        
-        ```python
-        def identify_user(app, environ, response_headers=dict()):
-            # Your custom code that returns a user id string
-            return "12345"
-        
-        def identify_company(app, environ, response_headers=dict()):
-            # Your custom code that returns a company id string
-            return "67890"
-        
-        def should_skip(app, environ):
-            # Your custom code that returns true to skip logging
-            return "health/probe" in environ.get('PATH_INFO', '')
-        
-        def get_token(app, environ):
-            # If you don't want to use the standard WSGI session token,
-            # add your custom code that returns a string for session/API token
-            return "XXXXXXXXXXXXXX"
-        
-        def mask_event(eventmodel):
-            # Your custom code to change or remove any sensitive fields
-            if 'password' in eventmodel.response.body:
-                eventmodel.response.body['password'] = None
-            return eventmodel
-        
-        def get_metadata(app, environ):
-            return {
-                'datacenter': 'westus',
-                'deployment_version': 'v1.2.3',
-            }
-        
-        moesif_settings = {
-            'APPLICATION_ID': 'Your Moesif Application Id',
-            'DEBUG': False,
-            'LOG_BODY': True,
-            'IDENTIFY_USER': identify_user,
-            'IDENTIFY_COMPANY': identify_company,
-            'GET_SESSION_TOKEN': get_token,
-            'SKIP': should_skip,
-            'MASK_EVENT_MODEL': mask_event,
-            'GET_METADATA': get_metadata,
-            'CAPTURE_OUTGOING_REQUESTS': False
-        }
-        
-        app.wsgi_app = MoesifMiddleware(app.wsgi_app, moesif_settings)
-        
-        ```
-        
-        ## Update User
-        
-        ### Update A Single User
-        Create or update a user profile in Moesif.
-        The metadata field can be any customer demographic or other info you want to store.
-        Only the `user_id` field is required.
-        For details, visit the [Python API Reference](https://www.moesif.com/docs/api?python#update-a-user).
-        
-        ```python
-        api_client = MoesifAPIClient("Your Moesif Application Id").api
-        
-        # Only user_id is required.
-        # Campaign object is optional, but useful if you want to track ROI of acquisition channels
-        # See https://www.moesif.com/docs/api#users for campaign schema
-        # metadata can be any custom object
-        user = {
-          'user_id': '12345',
-          'company_id': '67890', # If set, associate user with a company object
-          'campaign': {
-            'utm_source': 'google',
-            'utm_medium': 'cpc', 
-            'utm_campaign': 'adwords',
-            'utm_term': 'api+tooling',
-            'utm_content': 'landing'
-          },
-          'metadata': {
-            'email': 'john@acmeinc.com',
-            'first_name': 'John',
-            'last_name': 'Doe',
-            'title': 'Software Engineer',
-            'sales_info': {
-                'stage': 'Customer',
-                'lifetime_value': 24000,
-                'account_owner': 'mary@contoso.com'
-            },
-          }
-        }
-        
-        update_user = api_client.update_user(user)
-        ```
-        
-        ### Update Users in Batch
-        Similar to update_user, but used to update a list of users in one batch. 
-        Only the `user_id` field is required.
-        For details, visit the [Python API Reference](https://www.moesif.com/docs/api?python#update-users-in-batch).
-        
-        ```python
-        api_client = MoesifAPIClient("Your Moesif Application Id").api
-        
-        userA = {
-          'user_id': '12345',
-          'company_id': '67890', # If set, associate user with a company object
-          'metadata': {
-            'email': 'john@acmeinc.com',
-            'first_name': 'John',
-            'last_name': 'Doe',
-            'title': 'Software Engineer',
-            'sales_info': {
-                'stage': 'Customer',
-                'lifetime_value': 24000,
-                'account_owner': 'mary@contoso.com'
-            },
-          }
-        }
-        
-        userB = {
-          'user_id': '54321',
-          'company_id': '67890', # If set, associate user with a company object
-          'metadata': {
-            'email': 'mary@acmeinc.com',
-            'first_name': 'Mary',
-            'last_name': 'Jane',
-            'title': 'Software Engineer',
-            'sales_info': {
-                'stage': 'Customer',
-                'lifetime_value': 48000,
-                'account_owner': 'mary@contoso.com'
-            },
-          }
-        }
-        update_users = api_client.update_users_batch([userA, userB])
-        ```
-        
-        ## Update Company
-        
-        ### Update A Single Company
-        Create or update a company profile in Moesif.
-        The metadata field can be any company demographic or other info you want to store.
-        Only the `company_id` field is required.
-        For details, visit the [Python API Reference](https://www.moesif.com/docs/api?python#update-a-company).
-        
-        ```python
-        api_client = MoesifAPIClient("Your Moesif Application Id").api
-        
-        # Only company_id is required.
-        # Campaign object is optional, but useful if you want to track ROI of acquisition channels
-        # See https://www.moesif.com/docs/api#update-a-company for campaign schema
-        # metadata can be any custom object
-        company = {
-          'company_id': '67890',
-          'company_domain': 'acmeinc.com', # If domain is set, Moesif will enrich your profiles with publicly available info 
-          'campaign': {
-            'utm_source': 'google',
-            'utm_medium': 'cpc', 
-            'utm_campaign': 'adwords',
-            'utm_term': 'api+tooling',
-            'utm_content': 'landing'
-          },
-          'metadata': {
-            'org_name': 'Acme, Inc',
-            'plan_name': 'Free',
-            'deal_stage': 'Lead',
-            'mrr': 24000,
-            'demographics': {
-                'alexa_ranking': 500000,
-                'employee_count': 47
-            },
-          }
-        }
-        
-        update_company = api_client.update_company(company)
-        ```
-        
-        ### Update Companies in Batch
-        Similar to update_company, but used to update a list of companies in one batch. 
-        Only the `company_id` field is required.
-        For details, visit the [Python API Reference](https://www.moesif.com/docs/api?python#update-companies-in-batch).
-        
-        ```python
-        api_client = MoesifAPIClient("Your Moesif Application Id").api
-        
-        companyA = {
-          'company_id': '67890',
-          'company_domain': 'acmeinc.com', # If domain is set, Moesif will enrich your profiles with publicly available info 
-          'metadata': {
-            'org_name': 'Acme, Inc',
-            'plan_name': 'Free',
-            'deal_stage': 'Lead',
-            'mrr': 24000,
-            'demographics': {
-                'alexa_ranking': 500000,
-                'employee_count': 47
-            },
-          }
-        }
-        
-        companyB = {
-          'company_id': '09876',
-          'company_domain': 'contoso.com', # If domain is set, Moesif will enrich your profiles with publicly available info 
-          'metadata': {
-            'org_name': 'Contoso, Inc',
-            'plan_name': 'Free',
-            'deal_stage': 'Lead',
-            'mrr': 48000,
-            'demographics': {
-                'alexa_ranking': 500000,
-                'employee_count': 53
-            },
-          }
-        }
-        
-        update_companies = api_client.update_companies_batch([companyA, companyB])
-        ```
-        ## Troubleshooting
-        
-        When using Docker with Ubuntu based image, if events are not being captured, it could be possible as the image can't find any timezone configuration. 
-        In order to resolve that, add the following line to your Dockerfile
-        ```
-        ENV TZ=UTC
-        ```
-        or you could add `RUN apt-get install tzdata` in the Dockerfile.
-        
-        ## Other integrations
-        
-        To view more documentation on integration options, please visit __[the Integration Options Documentation](https://www.moesif.com/docs/getting-started/integration-options/).__
-        
-        [ico-built-for]: https://img.shields.io/badge/built%20for-python%20wsgi-blue.svg
-        [ico-version]: https://img.shields.io/pypi/v/moesifwsgi.svg
-        [ico-language]: https://img.shields.io/pypi/pyversions/moesifwsgi.svg
-        [ico-license]: https://img.shields.io/badge/License-Apache%202.0-green.svg
-        [ico-source]: https://img.shields.io/github/last-commit/moesif/moesifwsgi.svg?style=social
-        
-        [link-built-for]: https://en.wikipedia.org/wiki/Web_Server_Gateway_Interface
-        [link-package]: https://pypi.python.org/pypi/moesifwsgi
-        [link-language]: https://pypi.python.org/pypi/moesifwsgi
-        [link-license]: https://raw.githubusercontent.com/Moesif/moesifwsgi/master/LICENSE
-        [link-source]: https://github.com/Moesif/moesifwsgi
-        
 Keywords: log analysis restful api development debug wsgi flask bottle http middleware
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: Log Analysis
 Classifier: Topic :: Software Development :: Debuggers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
+License-File: LICENSE
+
+# Moesif Middleware for Python WSGI based Frameworks
+
+[![Built For][ico-built-for]][link-built-for]
+[![Latest Version][ico-version]][link-package]
+[![Language Versions][ico-language]][link-language]
+[![Software License][ico-license]][link-license]
+[![Source Code][ico-source]][link-source]
+
+WSGI middleware that automatically logs _incoming_ or _outgoing_ API calls and sends to [Moesif](https://www.moesif.com) for API analytics and monitoring.
+Supports Python Frameworks built on WSGI such as Flask, Bottle, and Pyramid.
+
+[Source Code on GitHub](https://github.com/moesif/moesifwsgi)
+
+[WSGI (Web Server Gateway Interface)](https://wsgi.readthedocs.io/en/latest/)
+is a standard (PEP 3333) that describes
+how a web server communicates with web applications. Many Python Frameworks
+are build on top of WSGI, such as [Flask](http://flask.pocoo.org/),
+[Bottle](https://bottlepy.org/docs/dev/), [Pyramid](https://trypyramid.com/) etc.
+Moesif WSGI Middleware help APIs that are build on top of these Frameworks to
+easily integrate with [Moesif](https://www.moesif.com).
+
+## How to install
+
+```shell
+pip install moesifwsgi
+```
+
+## How to use
+
+### Flask
+
+Wrap your wsgi_app with the Moesif middleware.
+
+```python
+from moesifwsgi import MoesifMiddleware
+
+moesif_settings = {
+    'APPLICATION_ID': 'Your Moesif Application id',
+    'LOG_BODY': True,
+    # ... For other options see below.
+}
+
+app.wsgi_app = MoesifMiddleware(app.wsgi_app, moesif_settings)
+
+```
+
+Your Moesif Application Id can be found in the [_Moesif Portal_](https://www.moesif.com/).
+After signing up for a Moesif account, your Moesif Application Id will be displayed during the onboarding steps. 
+
+You can always find your Moesif Application Id at any time by logging 
+into the [_Moesif Portal_](https://www.moesif.com/), click on the top right menu,
+and then clicking _API Keys_.
+
+For an example with Flask, see example in the `/examples/flask` folder of this repo.
+
+### Bottle
+Wrap your bottle app with the Moesif middleware.
+
+```python
+
+from moesifwsgi import MoesifMiddleware
+
+app = bottle.Bottle()
+
+moesif_settings = {
+    'APPLICATION_ID': 'Your Moesif Application Id',
+    'LOG_BODY': True,
+    # ... For other options see below.
+}
+
+bottle.run(app=MoesifMiddleware(app, moesif_settings))
+
+```
+
+For an example with Bottle, see example in the `/examples/bottle` folder of this repo.
+
+### Pyramid
+
+
+```python
+from pyramid.config import Configurator
+from moesifwsgi import MoesifMiddleware
+
+if __name__ == '__main__':
+    config = Configurator()
+    config.add_route('hello', '/')
+    config.scan()
+    app = config.make_wsgi_app()
+
+    # configure your moesif settings
+    moesif_settings = {
+        'APPLICATION_ID': 'Your Moesif Application Id',
+        'LOG_BODY': True,
+        # ... For other options see below.
+    }
+    # Put middleware
+    app = MoesifMiddleware(app, moesif_settings)
+
+    server = make_server('0.0.0.0', 8080, app)
+    server.serve_forever()
+
+```
+### Other WSGI frameworks
+
+If you are using a framework that is built on top of WSGI, it should work just by adding the Moesif middleware.
+Please read the documentation for your specific framework on how to add middleware.
+
+## Configuration options
+
+#### __`APPLICATION_ID`__
+(__required__), _string_, is obtained via your Moesif Account, this is required.
+
+#### __`SKIP`__
+(optional) _(app, environ) => boolean_, a function that takes a WSGI app and an environ,
+and returns true if you want to skip this particular event. The app is the original WSGI app instance, and the
+environ is a [WSGI environ](http://wsgi.readthedocs.io/en/latest/definitions.html).
+
+#### __`IDENTIFY_USER`__
+(optional, but highly recommended) _(app, environ, response_headers) => string_, a function that takes an app, an environ and an optional parameter response headers, and returns a string that is the user id used by your system. While Moesif tries to identify users automatically,
+but different frameworks and your implementation might be very different, it would be helpful and much more accurate to provide this function.
+
+#### __`IDENTIFY_COMPANY`__
+(optional) _(app, environ, response_headers) => string_, a function that takes an app, an environ and an optional parameter response headers, and returns a string that is the company id for this event.
+
+#### __`GET_METADATA`__
+(optional) _(app, environ) => dictionary_, a function that takes an app and an environ, and
+returns a dictionary (must be able to be encoded into JSON). This allows your
+to associate this event with custom metadata. For example, you may want to save a VM instance_id, a trace_id, or a tenant_id with the request.
+
+#### __`GET_SESSION_TOKEN`__
+(optional) _(app, environ) => string_, a function that takes an app and an environ, and returns a string that is the session token for this event. Again, Moesif tries to get the session token automatically, but if you setup is very different from standard, this function will be very help for tying events together, and help you replay the events.
+
+#### __`MASK_EVENT_MODEL`__
+(optional) _(EventModel) => EventModel_, a function that takes an EventModel and returns an EventModel with desired data removed. The return value must be a valid EventModel required by Moesif data ingestion API. For details regarding EventModel please see the [Moesif Python API Documentation](https://www.moesif.com/docs/api?python).
+
+#### __`DEBUG`__
+(optional) _boolean_, a flag to see debugging messages.
+
+#### __`LOG_BODY`__
+(optional) _boolean_, default True, Set to False to remove logging request and response body.
+
+#### __`EVENT_QUEUE_SIZE`__
+(optional) __int__, default 10000, the maximum number of event objects queued in memory pending upload to Moesif.  If the queue is full additional calls to `MoesifMiddleware` will return immediately without logging the event, so this number should be set based on the expected event size and memory capacity
+
+### __`EVENT_WORKER_COUNT`__
+(optional) __int__, default 2, the number of worker threads to use for uploading events to Moesif.  If you have a large number of events being logged, increasing this number can improve upload performance.
+
+#### __`BATCH_SIZE`__
+(optional) __int__, default 100, Maximum batch size when sending events to Moesif when reading from the queue
+
+#### __`EVENT_BATCH_TIMEOUT`__
+(optional) __int__, default 2, Maximum time in seconds to wait before sending a batch of events to Moesif when reading from the queue
+
+#### __`AUTHORIZATION_HEADER_NAME`__
+(optional) _string_, A request header field name used to identify the User in Moesif. Default value is `authorization`. Also, supports a comma separated string. We will check headers in order like `"X-Api-Key,Authorization"`.
+
+#### __`AUTHORIZATION_USER_ID_FIELD`__
+(optional) _string_, A field name used to parse the User from authorization header in Moesif. Default value is `sub`.
+
+#### __`BASE_URI`__
+(optional) _string_, A local proxy hostname when sending traffic via secure proxy. Please set this field when using secure proxy. For more details, refer [secure proxy documentation.](https://www.moesif.com/docs/platform/secure-proxy/#2-configure-moesif-sdk)
+
+### Options specific to outgoing API calls 
+
+The options below are applicable to outgoing API calls (calls you initiate using the Python [Requests](http://docs.python-requests.org/en/master/) lib to third parties like Stripe or to your own services.
+
+For options that use the request and response as input arguments, these use the [Requests](http://docs.python-requests.org/en/master/api/) lib's request or response objects.
+
+If you are not using WSGI, you can import the [moesifpythonrequest](https://github.com/Moesif/moesifpythonrequest) directly.
+
+#### __`CAPTURE_OUTGOING_REQUESTS`__
+_boolean_, Default False. Set to True to capture all outgoing API calls. False will disable this functionality. 
+
+##### __`GET_METADATA_OUTGOING`__
+(optional) _(req, res) => dictionary_, a function that enables you to return custom metadata associated with the logged API calls. 
+Takes in the [Requests](http://docs.python-requests.org/en/master/api/) request and response object as arguments. You should implement a function that 
+returns a dictionary containing your custom metadata. (must be able to be encoded into JSON). For example, you may want to save a VM instance_id, a trace_id, or a resource_id with the request.
+
+##### __`SKIP_OUTGOING`__
+(optional) _(req, res) => boolean_, a function that takes a [Requests](http://docs.python-requests.org/en/master/api/) request and response,
+and returns true if you want to skip this particular event.
+
+##### __`IDENTIFY_USER_OUTGOING`__
+(optional, but highly recommended) _(req, res) => string_, a function that takes [Requests](http://docs.python-requests.org/en/master/api/) request and response, and returns a string that is the user id used by your system. While Moesif tries to identify users automatically,
+but different frameworks and your implementation might be very different, it would be helpful and much more accurate to provide this function.
+
+##### __`IDENTIFY_COMPANY_OUTGOING`__
+(optional) _(req, res) => string_, a function that takes [Requests](http://docs.python-requests.org/en/master/api/) request and response, and returns a string that is the company id for this event.
+
+##### __`GET_SESSION_TOKEN_OUTGOING`__
+(optional) _(req, res) => string_, a function that takes [Requests](http://docs.python-requests.org/en/master/api/) request and response, and returns a string that is the session token for this event. Again, Moesif tries to get the session token automatically, but if you setup is very different from standard, this function will be very help for tying events together, and help you replay the events.
+
+##### __`LOG_BODY_OUTGOING`__
+(optional) _boolean_, default True, Set to False to remove logging request and response body.
+
+### Example:
+
+```python
+def identify_user(app, environ, response_headers=dict()):
+    # Your custom code that returns a user id string
+    return "12345"
+
+def identify_company(app, environ, response_headers=dict()):
+    # Your custom code that returns a company id string
+    return "67890"
+
+def should_skip(app, environ):
+    # Your custom code that returns true to skip logging
+    return "health/probe" in environ.get('PATH_INFO', '')
+
+def get_token(app, environ):
+    # If you don't want to use the standard WSGI session token,
+    # add your custom code that returns a string for session/API token
+    return "XXXXXXXXXXXXXX"
+
+def mask_event(eventmodel):
+    # Your custom code to change or remove any sensitive fields
+    if 'password' in eventmodel.response.body:
+        eventmodel.response.body['password'] = None
+    return eventmodel
+
+def get_metadata(app, environ):
+    return {
+        'datacenter': 'westus',
+        'deployment_version': 'v1.2.3',
+    }
+
+moesif_settings = {
+    'APPLICATION_ID': 'Your Moesif Application Id',
+    'DEBUG': False,
+    'LOG_BODY': True,
+    'IDENTIFY_USER': identify_user,
+    'IDENTIFY_COMPANY': identify_company,
+    'GET_SESSION_TOKEN': get_token,
+    'SKIP': should_skip,
+    'MASK_EVENT_MODEL': mask_event,
+    'GET_METADATA': get_metadata,
+    'CAPTURE_OUTGOING_REQUESTS': False
+}
+
+app.wsgi_app = MoesifMiddleware(app.wsgi_app, moesif_settings)
+
+```
+
+## Update User
+
+### Update A Single User
+Create or update a user profile in Moesif.
+The metadata field can be any customer demographic or other info you want to store.
+Only the `user_id` field is required.
+For details, visit the [Python API Reference](https://www.moesif.com/docs/api?python#update-a-user).
+
+```python
+api_client = MoesifAPIClient("Your Moesif Application Id").api
+
+# Only user_id is required.
+# Campaign object is optional, but useful if you want to track ROI of acquisition channels
+# See https://www.moesif.com/docs/api#users for campaign schema
+# metadata can be any custom object
+user = {
+  'user_id': '12345',
+  'company_id': '67890', # If set, associate user with a company object
+  'campaign': {
+    'utm_source': 'google',
+    'utm_medium': 'cpc', 
+    'utm_campaign': 'adwords',
+    'utm_term': 'api+tooling',
+    'utm_content': 'landing'
+  },
+  'metadata': {
+    'email': 'john@acmeinc.com',
+    'first_name': 'John',
+    'last_name': 'Doe',
+    'title': 'Software Engineer',
+    'sales_info': {
+        'stage': 'Customer',
+        'lifetime_value': 24000,
+        'account_owner': 'mary@contoso.com'
+    },
+  }
+}
+
+update_user = api_client.update_user(user)
+```
+
+### Update Users in Batch
+Similar to update_user, but used to update a list of users in one batch. 
+Only the `user_id` field is required.
+For details, visit the [Python API Reference](https://www.moesif.com/docs/api?python#update-users-in-batch).
+
+```python
+api_client = MoesifAPIClient("Your Moesif Application Id").api
+
+userA = {
+  'user_id': '12345',
+  'company_id': '67890', # If set, associate user with a company object
+  'metadata': {
+    'email': 'john@acmeinc.com',
+    'first_name': 'John',
+    'last_name': 'Doe',
+    'title': 'Software Engineer',
+    'sales_info': {
+        'stage': 'Customer',
+        'lifetime_value': 24000,
+        'account_owner': 'mary@contoso.com'
+    },
+  }
+}
+
+userB = {
+  'user_id': '54321',
+  'company_id': '67890', # If set, associate user with a company object
+  'metadata': {
+    'email': 'mary@acmeinc.com',
+    'first_name': 'Mary',
+    'last_name': 'Jane',
+    'title': 'Software Engineer',
+    'sales_info': {
+        'stage': 'Customer',
+        'lifetime_value': 48000,
+        'account_owner': 'mary@contoso.com'
+    },
+  }
+}
+update_users = api_client.update_users_batch([userA, userB])
+```
+
+## Update Company
+
+### Update A Single Company
+Create or update a company profile in Moesif.
+The metadata field can be any company demographic or other info you want to store.
+Only the `company_id` field is required.
+For details, visit the [Python API Reference](https://www.moesif.com/docs/api?python#update-a-company).
+
+```python
+api_client = MoesifAPIClient("Your Moesif Application Id").api
+
+# Only company_id is required.
+# Campaign object is optional, but useful if you want to track ROI of acquisition channels
+# See https://www.moesif.com/docs/api#update-a-company for campaign schema
+# metadata can be any custom object
+company = {
+  'company_id': '67890',
+  'company_domain': 'acmeinc.com', # If domain is set, Moesif will enrich your profiles with publicly available info 
+  'campaign': {
+    'utm_source': 'google',
+    'utm_medium': 'cpc', 
+    'utm_campaign': 'adwords',
+    'utm_term': 'api+tooling',
+    'utm_content': 'landing'
+  },
+  'metadata': {
+    'org_name': 'Acme, Inc',
+    'plan_name': 'Free',
+    'deal_stage': 'Lead',
+    'mrr': 24000,
+    'demographics': {
+        'alexa_ranking': 500000,
+        'employee_count': 47
+    },
+  }
+}
+
+update_company = api_client.update_company(company)
+```
+
+### Update Companies in Batch
+Similar to update_company, but used to update a list of companies in one batch. 
+Only the `company_id` field is required.
+For details, visit the [Python API Reference](https://www.moesif.com/docs/api?python#update-companies-in-batch).
+
+```python
+api_client = MoesifAPIClient("Your Moesif Application Id").api
+
+companyA = {
+  'company_id': '67890',
+  'company_domain': 'acmeinc.com', # If domain is set, Moesif will enrich your profiles with publicly available info 
+  'metadata': {
+    'org_name': 'Acme, Inc',
+    'plan_name': 'Free',
+    'deal_stage': 'Lead',
+    'mrr': 24000,
+    'demographics': {
+        'alexa_ranking': 500000,
+        'employee_count': 47
+    },
+  }
+}
+
+companyB = {
+  'company_id': '09876',
+  'company_domain': 'contoso.com', # If domain is set, Moesif will enrich your profiles with publicly available info 
+  'metadata': {
+    'org_name': 'Contoso, Inc',
+    'plan_name': 'Free',
+    'deal_stage': 'Lead',
+    'mrr': 48000,
+    'demographics': {
+        'alexa_ranking': 500000,
+        'employee_count': 53
+    },
+  }
+}
+
+update_companies = api_client.update_companies_batch([companyA, companyB])
+```
+## Troubleshooting
+
+When using Docker with Ubuntu based image, if events are not being captured, it could be possible as the image can't find any timezone configuration. 
+In order to resolve that, add the following line to your Dockerfile
+```
+ENV TZ=UTC
+```
+or you could add `RUN apt-get install tzdata` in the Dockerfile.
+
+## Other integrations
+
+To view more documentation on integration options, please visit __[the Integration Options Documentation](https://www.moesif.com/docs/getting-started/integration-options/).__
+
+[ico-built-for]: https://img.shields.io/badge/built%20for-python%20wsgi-blue.svg
+[ico-version]: https://img.shields.io/pypi/v/moesifwsgi.svg
+[ico-language]: https://img.shields.io/pypi/pyversions/moesifwsgi.svg
+[ico-license]: https://img.shields.io/badge/License-Apache%202.0-green.svg
+[ico-source]: https://img.shields.io/github/last-commit/moesif/moesifwsgi.svg?style=social
+
+[link-built-for]: https://en.wikipedia.org/wiki/Web_Server_Gateway_Interface
+[link-package]: https://pypi.python.org/pypi/moesifwsgi
+[link-language]: https://pypi.python.org/pypi/moesifwsgi
+[link-license]: https://raw.githubusercontent.com/Moesif/moesifwsgi/master/LICENSE
+[link-source]: https://github.com/Moesif/moesifwsgi
```

### Comparing `moesifwsgi-1.6.1/README.md` & `moesifwsgi-1.7.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -135,16 +135,25 @@
 
 #### __`DEBUG`__
 (optional) _boolean_, a flag to see debugging messages.
 
 #### __`LOG_BODY`__
 (optional) _boolean_, default True, Set to False to remove logging request and response body.
 
+#### __`EVENT_QUEUE_SIZE`__
+(optional) __int__, default 10000, the maximum number of event objects queued in memory pending upload to Moesif.  If the queue is full additional calls to `MoesifMiddleware` will return immediately without logging the event, so this number should be set based on the expected event size and memory capacity
+
+### __`EVENT_WORKER_COUNT`__
+(optional) __int__, default 2, the number of worker threads to use for uploading events to Moesif.  If you have a large number of events being logged, increasing this number can improve upload performance.
+
 #### __`BATCH_SIZE`__
-(optional) __int__, default 25, Maximum batch size when sending events to Moesif.
+(optional) __int__, default 100, Maximum batch size when sending events to Moesif when reading from the queue
+
+#### __`EVENT_BATCH_TIMEOUT`__
+(optional) __int__, default 2, Maximum time in seconds to wait before sending a batch of events to Moesif when reading from the queue
 
 #### __`AUTHORIZATION_HEADER_NAME`__
 (optional) _string_, A request header field name used to identify the User in Moesif. Default value is `authorization`. Also, supports a comma separated string. We will check headers in order like `"X-Api-Key,Authorization"`.
 
 #### __`AUTHORIZATION_USER_ID_FIELD`__
 (optional) _string_, A field name used to parse the User from authorization header in Moesif. Default value is `sub`.
```

### Comparing `moesifwsgi-1.6.1/moesifwsgi/client_ip.py` & `moesifwsgi-1.7.0/moesifwsgi/client_ip.py`

 * *Files identical despite different names*

### Comparing `moesifwsgi-1.6.1/moesifwsgi/event_mapper.py` & `moesifwsgi-1.7.0/moesifwsgi/event_mapper.py`

 * *Files identical despite different names*

### Comparing `moesifwsgi-1.6.1/moesifwsgi/http_response_catcher.py` & `moesifwsgi-1.7.0/moesifwsgi/http_response_catcher.py`

 * *Files identical despite different names*

### Comparing `moesifwsgi-1.6.1/moesifwsgi/logger_helper.py` & `moesifwsgi-1.7.0/moesifwsgi/logger_helper.py`

 * *Files identical despite different names*

### Comparing `moesifwsgi-1.6.1/moesifwsgi/middleware.py` & `moesifwsgi-1.7.0/moesifwsgi/middleware.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,263 +1,212 @@
 # -*- coding: utf-8 -*-
-import gzip
-from datetime import datetime, timedelta
-import queue
-import random
 import itertools
 import math
-import base64
+import random
+from datetime import datetime
+import sys
+
+from moesifwsgi.config_manager import ConfigUpdateManager
+from moesifwsgi.workers import BatchedWorkerPool
 
 try:
     from cStringIO import StringIO
 except ImportError:
     from io import StringIO
+
+import atexit
+import logging
+
 from moesifapi.moesif_api_client import *
-from .update_companies import Company
-from .update_users import User
 from moesifpythonrequest.app_config.app_config import AppConfig
-from .parse_body import ParseBody
-from .logger_helper import LoggerHelper
-from .moesif_data_holder import DataHolder
-from .event_mapper import EventMapper
-from .send_batch_events import SendEventAsync
+from moesifpythonrequest.start_capture.start_capture import StartCapture
+
 from .client_ip import ClientIp
+from .event_mapper import EventMapper
 from .http_response_catcher import HttpResponseCatcher
-from moesifpythonrequest.start_capture.start_capture import StartCapture
-from apscheduler.schedulers.background import BackgroundScheduler
-from apscheduler.triggers.interval import IntervalTrigger
-from apscheduler.events import EVENT_JOB_ERROR, EVENT_JOB_EXECUTED
-import atexit
-import logging
+from .logger_helper import LoggerHelper
+from .moesif_data_holder import DataHolder
+from .parse_body import ParseBody
+from .update_companies import Company
+from .update_users import User
+
+logger = logging.getLogger(__name__)
 
 
 class MoesifMiddleware(object):
     """WSGI Middleware for recording of request-response"""
+
     def __init__(self, app, settings):
         self.app = app
+        self.settings = settings
+        self.DEBUG = self.settings.get("DEBUG", False)
+        self.initialize_logger()
+        self.validate_settings()
+
+        self.initialize_counter()
+        self.initialize_client()
+        self.initialize_config()
+        self.initialize_worker_pool()
+
+        # graceful shutodown handlers
+        atexit.register(self.worker_pool.stop)
+
+    def initialize_logger(self):
+        """Initialize logger mirroring the debug and stdout behavior of previous print statements for compatibility"""
+        logging.basicConfig(
+            level=logging.DEBUG if self.DEBUG else logging.INFO,
+            format='%(asctime)s\t%(levelname)s\tPID: %(process)d\tThread: %(thread)d\t%(funcName)s\t%(message)s',
+            handlers=[logging.StreamHandler()]
+        )
+
+    def validate_settings(self):
+        if self.settings is None or not self.settings.get("APPLICATION_ID", None):
+            raise Exception("Moesif Application ID is required in settings")
+
+    def initialize_counter(self):
         try:
             self.request_counter = itertools.count().next  # Threadsafe counter for Python 2
         except AttributeError:
             self.request_counter = itertools.count().__next__  # Threadsafe counter for Python 3
-
-        if settings is None:
-            raise Exception('Moesif Application ID is required in settings')
-        self.settings = settings
-
-        if settings.get('APPLICATION_ID', None):
-            self.client = MoesifAPIClient(settings.get('APPLICATION_ID'))
-        else:
-            raise Exception('Moesif Application ID is required in settings')
-
-        if settings.get('DEBUG', False):
-            Configuration.BASE_URI = self.get_configuration_uri(settings, 'BASE_URI', 'LOCAL_MOESIF_BASEURL')
-        Configuration.version = 'moesifwsgi-python/1.6.1'
-        self.DEBUG = settings.get('DEBUG', False)
+        self.dropped_events = 0
+        self.parse_body = ParseBody()
+        self.event_mapper = EventMapper()
         self.logger_helper = LoggerHelper()
-        if settings.get('CAPTURE_OUTGOING_REQUESTS', False):
-            try:
-                if self.DEBUG:
-                    print('Start capturing outgoing requests for pid - ' + self.logger_helper.get_worker_pid())
-                # Start capturing outgoing requests
-                StartCapture().start_capture_outgoing(settings)
-            except:
-                print('Error while starting to capture the outgoing events for pid - ' + self.logger_helper.get_worker_pid())
-        self.api_version = settings.get('API_VERSION')
+
+    def initialize_client(self):
+        self.api_version = self.settings.get("API_VERSION")
+        self.client = MoesifAPIClient(self.settings.get("APPLICATION_ID"))
         self.api_client = self.client.api
-        self.LOG_BODY = self.settings.get('LOG_BODY', True)
+
+    def initialize_config(self):
         if self.DEBUG:
+            logger.debug("Debug is enabled. Starting Moesif middleware for pid - " + self.logger_helper.get_worker_pid())
             response_catcher = HttpResponseCatcher()
             self.api_client.http_call_back = response_catcher
+            Configuration.BASE_URI = self.settings.get("BASE_URI") or self.settings.get("LOCAL_MOESIF_BASEURL", "https://api.moesif.net")
+        Configuration.version = "moesifwsgi-python/1.6.1"
+        if self.settings.get("CAPTURE_OUTGOING_REQUESTS", False):
+            self.start_capture_outgoing()
+
+        self.LOG_BODY = self.settings.get("LOG_BODY", True)
         self.client_ip = ClientIp()
         self.app_config = AppConfig()
-        self.parse_body = ParseBody()
-        self.event_mapper = EventMapper()
-        self.send_async_events = SendEventAsync()
-        self.config_etag = None
-        self.config = self.app_config.get_config(self.api_client, self.DEBUG)
-        self.sampling_percentage = 100
-        self.last_updated_time = datetime.utcnow()
-        self.moesif_events_queue = queue.Queue()
-        self.BATCH_SIZE = self.settings.get('BATCH_SIZE', 25)
-        self.last_event_job_run_time = datetime(1970, 1, 1, 0, 0)  # Assuming job never ran, set it to epoch start time
-        self.scheduler = None
-        self.is_event_job_scheduled = False
-        try:
-            if self.config:
-                self.config_etag, self.sampling_percentage, self.last_updated_time = self.app_config.parse_configuration(
-                    self.config, self.DEBUG)
-        except Exception as ex:
-            if self.DEBUG:
-                print('Error while parsing application configuration on initialization for pid - ' + self.logger_helper.get_worker_pid())
-                print(str(ex))
-
-    # Function to get configuration uri
-    def get_configuration_uri(self, settings, field, deprecated_field):
-        uri = settings.get(field)
-        if uri:
-            return uri
-        else:
-            return settings.get(deprecated_field, 'https://api.moesif.net')
+        self.config = ConfigUpdateManager(self.api_client, self.app_config, self.DEBUG)
+
+    def initialize_worker_pool(self):
+        # Create queues and threads which will batch and send events in the background
+        self.worker_pool = BatchedWorkerPool(
+            worker_count=self.settings.get("EVENT_WORKER_COUNT", 2),
+            api_client=self.api_client,
+            config=self.config,
+            debug=self.DEBUG,
+            max_queue_size=self.settings.get("EVENT_QUEUE_SIZE", 10000),
+            batch_size=self.settings.get("BATCH_SIZE", 100),
+            timeout=self.settings.get("EVENT_BATCH_TIMEOUT", 2),
+        )
 
     def __call__(self, environ, start_response):
         request_time = datetime.utcnow().strftime("%Y-%m-%dT%H:%M:%S.%f")[:-3]
-        if self.DEBUG:
-            print("event request time: ", request_time)
+        logger.debug(f"event request time: {request_time}")
 
-        data_holder = DataHolder(
-                        self.settings.get('DISABLED_TRANSACTION_ID', False),
-                        self.request_counter(),
-                        environ['REQUEST_METHOD'],
-                        self.logger_helper.request_url(environ),
-                        self.client_ip.get_client_address(environ),
-                        [(k, v) for k,v in self.logger_helper.parse_request_headers(environ)],
-                        *self.logger_helper.request_body(environ),
-                        request_time
-                    )
+        event_info = self.prepare_event_info(environ, start_response, request_time)
 
         response_headers_mapping = {}
         def _start_response(status, response_headers, *args):
             # Capture status and response_headers for later processing
-            data_holder.capture_response_status(status, response_headers, self.DEBUG)
-
+            event_info.capture_response_status(status, response_headers, self.DEBUG)
             if response_headers:
                 try:
                     for pair in response_headers:
                         response_headers_mapping[pair[0]] = pair[1]
                 except Exception as e:
-                    print('Error while parsing response headers for pid - ' + self.logger_helper.get_worker_pid(), e)
-
+                    logger.exception("Error while parsing response headers", e)
             return start_response(status, response_headers, *args)
+        response_chunks = event_info.finish_response(self.app(environ, _start_response))
 
-        response_chunks = data_holder.finish_response(self.app(environ, _start_response))
-        if self.DEBUG:
-            try:
-                print("event response time for pid - " + self.logger_helper.get_worker_pid(), data_holder.response_time)
-            except Exception as e:
-                print("Error while fetching response time for pid - " + self.logger_helper.get_worker_pid(), e)
-
-        data_holder.set_user_id(self.logger_helper.get_user_id(environ, self.settings, self.app, self.DEBUG, response_headers_mapping))
-        data_holder.set_company_id(self.logger_helper.get_company_id(environ, self.settings, self.app, self.DEBUG, response_headers_mapping))
-        data_holder.set_metadata(self.logger_helper.get_metadata(environ, self.settings, self.app, self.DEBUG))
-        data_holder.set_session_token(self.logger_helper.get_session_token(environ, self.settings, self.app, self.DEBUG))
+        try:
+            logger.debug(f"event response time: {event_info.response_time}")
+        except Exception as e:
+            logger.exception(f"Error while fetching response time", e)
+
+        self.add_user_and_metadata(event_info, environ, response_headers_mapping)
 
-        # return data to WSGI server
         try:
             return response_chunks
         finally:
-            if not self.logger_helper.should_skip(environ, self.settings, self.app, self.DEBUG):
-                random_percentage = random.random() * 100
+            self.process_and_add_event_if_required(event_info, environ, response_headers_mapping)
 
-                # Prepare event to be sent to Moesif
-                event_data = self.process_data(data_holder)
+    def prepare_event_info(self, environ, start_response, request_time):
+        event_info = DataHolder(
+            self.settings.get("DISABLED_TRANSACTION_ID", False),
+            self.request_counter(),
+            environ["REQUEST_METHOD"],
+            self.logger_helper.request_url(environ),
+            self.client_ip.get_client_address(environ),
+            [(k, v) for k, v in self.logger_helper.parse_request_headers(environ)],
+            *self.logger_helper.request_body(environ),
+            request_time,
+        )
+        return event_info
+
+    def add_user_and_metadata(self, event_info, environ, response_headers_mapping):
+        event_info.set_user_id(self.logger_helper.get_user_id(environ, self.settings, self.app, self.DEBUG, response_headers_mapping))
+        event_info.set_company_id(self.logger_helper.get_company_id(environ, self.settings, self.app, self.DEBUG, response_headers_mapping))
+        event_info.set_metadata(self.logger_helper.get_metadata(environ, self.settings, self.app, self.DEBUG))
+        event_info.set_session_token(self.logger_helper.get_session_token(environ, self.settings, self.app, self.DEBUG))
+
+    def process_and_add_event_if_required(self, event_info, environ, response_headers_mapping):
+        if event_info is None:
+            logger.debug("Skipped Event as the moesif event model is None")
+            return
+        if self.logger_helper.should_skip(environ, self.settings, self.app, self.DEBUG):
+            logger.debug("Skipped Event using should_skip configuration option")
+            return
+                
+        # Prepare event to be sent to Moesif and check the config for applicable sampling rules
+        event_data = self.process_data(event_info)
+        event_sampling_percentage = self.config.get_sampling_percentage(
+            event_data,
+            self.logger_helper.get_user_id(environ, self.settings, self.app, self.DEBUG, response_headers_mapping),
+            self.logger_helper.get_company_id(environ, self.settings, self.app, self.DEBUG, response_headers_mapping)
+        )
+
+        # if the event has a sample rate of less than 100, then we need to check if this event should be skipped and not sent to Moesif
+        random_percentage = random.random() * 100
+        if random_percentage >= event_sampling_percentage:
+            logger.debug("Skipped Event due to sampling percentage: " + str(event_sampling_percentage) + " and random percentage: " + str(random_percentage))
+            return
 
-                self.sampling_percentage = self.app_config.get_sampling_percentage(event_data, self.config,
-                                                                                   self.logger_helper.get_user_id(
-                                                                                       environ, self.settings, self.app,
-                                                                                       self.DEBUG, response_headers_mapping),
-                                                                                   self.logger_helper.get_company_id(
-                                                                                       environ, self.settings, self.app,
-                                                                                       self.DEBUG, response_headers_mapping))
-
-                if self.sampling_percentage >= random_percentage:
-                    if event_data:
-                        # Add Weight to the event
-                        event_data.weight = 1 if self.sampling_percentage == 0 else math.floor(100 / self.sampling_percentage)
-                        try:
-                            if not self.is_event_job_scheduled and datetime.utcnow() > self.last_event_job_run_time + timedelta(
-                                    minutes=5):
-                                try:
-                                    self.schedule_background_job()
-                                    self.is_event_job_scheduled = True
-                                    self.last_event_job_run_time = datetime.utcnow()
-                                except Exception as ex:
-                                    self.is_event_job_scheduled = False
-                                    if self.DEBUG:
-                                        print('Error while starting the event scheduler job in background for pid - '
-                                              + self.logger_helper.get_worker_pid())
-                                        print(str(ex))
-                            # Add Event to the queue
-                            if self.DEBUG:
-                                print('Add Event to the queue for pid - ' + self.logger_helper.get_worker_pid())
-                            self.moesif_events_queue.put(event_data)
-                        except Exception as ex:
-                            if self.DEBUG:
-                                print("Error while adding event to the queue for pid - " + self.logger_helper.get_worker_pid())
-                                print(str(ex))
-                    else:
-                        if self.DEBUG:
-                            print('Skipped Event as the moesif event model is None for pid - ' + self.logger_helper.get_worker_pid())
-                else:
-                    if self.DEBUG:
-                        print("Skipped Event due to sampling percentage: " + str(self.sampling_percentage)
-                              + " and random percentage: " + str(random_percentage) + " for pid - " + self.logger_helper.get_worker_pid())
+        # Add proportionate weight to the event for sampling percentage lower than 100
+        event_data.weight = 1 if event_sampling_percentage == 0 else math.floor(100 / event_sampling_percentage)
+        try:
+            # Add Event to the queue if able and count the dropped event if at capacity
+            if self.worker_pool.add_event(event_data):
+                logger.debug("Add Event to the queue")
             else:
-                if self.DEBUG:
-                    print('Skipped Event using should_skip configuration option for pid - ' + self.logger_helper.get_worker_pid())
+                self.dropped_events += 1
+                logger.info("Dropped Event due to queue capacity drop_count=" + str(self.dropped_events))
+        # add_event does not throw exceptions so this is unexepected
+        except Exception as ex:
+            logger.exception("Error while adding event to the queue for", ex)
 
-    def process_data(self, data):
 
+    def process_data(self, data):
         # Prepare Event Request Model
         event_req = self.event_mapper.to_request(data, self.LOG_BODY, self.api_version)
 
         # Prepare Event Response Model
         event_rsp = self.event_mapper.to_response(data, self.LOG_BODY, self.DEBUG)
 
         # Prepare Event Model
         event_model = self.event_mapper.to_event(data, event_req, event_rsp)
 
         # Mask Event Model
         return self.logger_helper.mask_event(event_model, self.settings, self.DEBUG)
 
-    # Function to listen to the send event job response
-    def moesif_event_listener(self, event):
-        if event.exception:
-            if self.DEBUG:
-                print('Error reading response from the scheduled job for pid - ' + self.logger_helper.get_worker_pid())
-        else:
-            if event.retval:
-                response_etag, self.last_event_job_run_time = event.retval
-                if response_etag is not None \
-                    and self.config_etag is not None \
-                    and self.config_etag != response_etag \
-                        and datetime.utcnow() > self.last_updated_time + timedelta(minutes=5):
-                    try:
-                        self.config = self.app_config.get_config(self.api_client, self.DEBUG)
-                        self.config_etag, self.sampling_percentage, self.last_updated_time = self.app_config.parse_configuration(
-                            self.config, self.DEBUG)
-                    except Exception as ex:
-                        if self.DEBUG:
-                            print('Error while updating the application configuration for pid - ' + self.logger_helper.get_worker_pid())
-                            print(str(ex))
-
-    def schedule_background_job(self):
-        try:
-            if not self.scheduler:
-                self.scheduler = BackgroundScheduler(daemon=True)
-            if not self.scheduler.get_jobs():
-                self.scheduler.add_listener(self.moesif_event_listener, EVENT_JOB_EXECUTED | EVENT_JOB_ERROR)
-                self.scheduler.start()
-                self.scheduler.add_job(
-                    func=lambda: self.send_async_events.batch_events(self.api_client, self.moesif_events_queue,
-                                                                     self.DEBUG, self.BATCH_SIZE),
-                    trigger=IntervalTrigger(seconds=2),
-                    id='moesif_events_batch_job',
-                    name='Schedule events batch job every 2 second',
-                    replace_existing=True)
-
-                # Avoid passing logging message to the ancestor loggers
-                logging.getLogger('apscheduler.executors.default').setLevel(logging.WARNING)
-                logging.getLogger('apscheduler.executors.default').propagate = False
-
-                # Exit handler when exiting the app
-                atexit.register(lambda: self.send_async_events.exit_handler(self.scheduler, self.DEBUG))
-        except Exception as ex:
-            print("Error when scheduling the job for pid - " + self.logger_helper.get_worker_pid())
-            print(str(ex))
-
     def update_user(self, user_profile):
         User().update_user(user_profile, self.api_client, self.DEBUG)
 
     def update_users_batch(self, user_profiles):
         User().update_users_batch(user_profiles, self.api_client, self.DEBUG)
 
     def update_company(self, company_profile):
```

### Comparing `moesifwsgi-1.6.1/moesifwsgi/moesif_data_holder.py` & `moesifwsgi-1.7.0/moesifwsgi/moesif_data_holder.py`

 * *Files identical despite different names*

### Comparing `moesifwsgi-1.6.1/moesifwsgi/parse_body.py` & `moesifwsgi-1.7.0/moesifwsgi/parse_body.py`

 * *Files identical despite different names*

### Comparing `moesifwsgi-1.6.1/moesifwsgi/regex_config_helper.py` & `moesifwsgi-1.7.0/moesifwsgi/regex_config_helper.py`

 * *Files identical despite different names*

### Comparing `moesifwsgi-1.6.1/moesifwsgi/update_companies.py` & `moesifwsgi-1.7.0/moesifwsgi/update_companies.py`

 * *Files identical despite different names*

### Comparing `moesifwsgi-1.6.1/moesifwsgi/update_users.py` & `moesifwsgi-1.7.0/moesifwsgi/update_users.py`

 * *Files identical despite different names*

### Comparing `moesifwsgi-1.6.1/moesifwsgi.egg-info/PKG-INFO` & `moesifwsgi-1.7.0/moesifwsgi.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,450 +1,464 @@
 Metadata-Version: 2.1
 Name: moesifwsgi
-Version: 1.6.1
+Version: 1.7.0
 Summary: Moesif Middleware for Python WSGI based platforms (Flask, Bottle & Others)
 Home-page: https://www.moesif.com/docs/server-integration/python-wsgi/
 Author: Moesif, Inc
 Author-email: xing@moesif.com
 License: Apache Software License
-Description: # Moesif Middleware for Python WSGI based Frameworks
-        
-        [![Built For][ico-built-for]][link-built-for]
-        [![Latest Version][ico-version]][link-package]
-        [![Language Versions][ico-language]][link-language]
-        [![Software License][ico-license]][link-license]
-        [![Source Code][ico-source]][link-source]
-        
-        WSGI middleware that automatically logs _incoming_ or _outgoing_ API calls and sends to [Moesif](https://www.moesif.com) for API analytics and monitoring.
-        Supports Python Frameworks built on WSGI such as Flask, Bottle, and Pyramid.
-        
-        [Source Code on GitHub](https://github.com/moesif/moesifwsgi)
-        
-        [WSGI (Web Server Gateway Interface)](https://wsgi.readthedocs.io/en/latest/)
-        is a standard (PEP 3333) that describes
-        how a web server communicates with web applications. Many Python Frameworks
-        are build on top of WSGI, such as [Flask](http://flask.pocoo.org/),
-        [Bottle](https://bottlepy.org/docs/dev/), [Pyramid](https://trypyramid.com/) etc.
-        Moesif WSGI Middleware help APIs that are build on top of these Frameworks to
-        easily integrate with [Moesif](https://www.moesif.com).
-        
-        ## How to install
-        
-        ```shell
-        pip install moesifwsgi
-        ```
-        
-        ## How to use
-        
-        ### Flask
-        
-        Wrap your wsgi_app with the Moesif middleware.
-        
-        ```python
-        from moesifwsgi import MoesifMiddleware
-        
-        moesif_settings = {
-            'APPLICATION_ID': 'Your Moesif Application id',
-            'LOG_BODY': True,
-            # ... For other options see below.
-        }
-        
-        app.wsgi_app = MoesifMiddleware(app.wsgi_app, moesif_settings)
-        
-        ```
-        
-        Your Moesif Application Id can be found in the [_Moesif Portal_](https://www.moesif.com/).
-        After signing up for a Moesif account, your Moesif Application Id will be displayed during the onboarding steps. 
-        
-        You can always find your Moesif Application Id at any time by logging 
-        into the [_Moesif Portal_](https://www.moesif.com/), click on the top right menu,
-        and then clicking _API Keys_.
-        
-        For an example with Flask, see example in the `/examples/flask` folder of this repo.
-        
-        ### Bottle
-        Wrap your bottle app with the Moesif middleware.
-        
-        ```python
-        
-        from moesifwsgi import MoesifMiddleware
-        
-        app = bottle.Bottle()
-        
-        moesif_settings = {
-            'APPLICATION_ID': 'Your Moesif Application Id',
-            'LOG_BODY': True,
-            # ... For other options see below.
-        }
-        
-        bottle.run(app=MoesifMiddleware(app, moesif_settings))
-        
-        ```
-        
-        For an example with Bottle, see example in the `/examples/bottle` folder of this repo.
-        
-        ### Pyramid
-        
-        
-        ```python
-        from pyramid.config import Configurator
-        from moesifwsgi import MoesifMiddleware
-        
-        if __name__ == '__main__':
-            config = Configurator()
-            config.add_route('hello', '/')
-            config.scan()
-            app = config.make_wsgi_app()
-        
-            # configure your moesif settings
-            moesif_settings = {
-                'APPLICATION_ID': 'Your Moesif Application Id',
-                'LOG_BODY': True,
-                # ... For other options see below.
-            }
-            # Put middleware
-            app = MoesifMiddleware(app, moesif_settings)
-        
-            server = make_server('0.0.0.0', 8080, app)
-            server.serve_forever()
-        
-        ```
-        ### Other WSGI frameworks
-        
-        If you are using a framework that is built on top of WSGI, it should work just by adding the Moesif middleware.
-        Please read the documentation for your specific framework on how to add middleware.
-        
-        ## Configuration options
-        
-        #### __`APPLICATION_ID`__
-        (__required__), _string_, is obtained via your Moesif Account, this is required.
-        
-        #### __`SKIP`__
-        (optional) _(app, environ) => boolean_, a function that takes a WSGI app and an environ,
-        and returns true if you want to skip this particular event. The app is the original WSGI app instance, and the
-        environ is a [WSGI environ](http://wsgi.readthedocs.io/en/latest/definitions.html).
-        
-        #### __`IDENTIFY_USER`__
-        (optional, but highly recommended) _(app, environ, response_headers) => string_, a function that takes an app, an environ and an optional parameter response headers, and returns a string that is the user id used by your system. While Moesif tries to identify users automatically,
-        but different frameworks and your implementation might be very different, it would be helpful and much more accurate to provide this function.
-        
-        #### __`IDENTIFY_COMPANY`__
-        (optional) _(app, environ, response_headers) => string_, a function that takes an app, an environ and an optional parameter response headers, and returns a string that is the company id for this event.
-        
-        #### __`GET_METADATA`__
-        (optional) _(app, environ) => dictionary_, a function that takes an app and an environ, and
-        returns a dictionary (must be able to be encoded into JSON). This allows your
-        to associate this event with custom metadata. For example, you may want to save a VM instance_id, a trace_id, or a tenant_id with the request.
-        
-        #### __`GET_SESSION_TOKEN`__
-        (optional) _(app, environ) => string_, a function that takes an app and an environ, and returns a string that is the session token for this event. Again, Moesif tries to get the session token automatically, but if you setup is very different from standard, this function will be very help for tying events together, and help you replay the events.
-        
-        #### __`MASK_EVENT_MODEL`__
-        (optional) _(EventModel) => EventModel_, a function that takes an EventModel and returns an EventModel with desired data removed. The return value must be a valid EventModel required by Moesif data ingestion API. For details regarding EventModel please see the [Moesif Python API Documentation](https://www.moesif.com/docs/api?python).
-        
-        #### __`DEBUG`__
-        (optional) _boolean_, a flag to see debugging messages.
-        
-        #### __`LOG_BODY`__
-        (optional) _boolean_, default True, Set to False to remove logging request and response body.
-        
-        #### __`BATCH_SIZE`__
-        (optional) __int__, default 25, Maximum batch size when sending events to Moesif.
-        
-        #### __`AUTHORIZATION_HEADER_NAME`__
-        (optional) _string_, A request header field name used to identify the User in Moesif. Default value is `authorization`. Also, supports a comma separated string. We will check headers in order like `"X-Api-Key,Authorization"`.
-        
-        #### __`AUTHORIZATION_USER_ID_FIELD`__
-        (optional) _string_, A field name used to parse the User from authorization header in Moesif. Default value is `sub`.
-        
-        #### __`BASE_URI`__
-        (optional) _string_, A local proxy hostname when sending traffic via secure proxy. Please set this field when using secure proxy. For more details, refer [secure proxy documentation.](https://www.moesif.com/docs/platform/secure-proxy/#2-configure-moesif-sdk)
-        
-        ### Options specific to outgoing API calls 
-        
-        The options below are applicable to outgoing API calls (calls you initiate using the Python [Requests](http://docs.python-requests.org/en/master/) lib to third parties like Stripe or to your own services.
-        
-        For options that use the request and response as input arguments, these use the [Requests](http://docs.python-requests.org/en/master/api/) lib's request or response objects.
-        
-        If you are not using WSGI, you can import the [moesifpythonrequest](https://github.com/Moesif/moesifpythonrequest) directly.
-        
-        #### __`CAPTURE_OUTGOING_REQUESTS`__
-        _boolean_, Default False. Set to True to capture all outgoing API calls. False will disable this functionality. 
-        
-        ##### __`GET_METADATA_OUTGOING`__
-        (optional) _(req, res) => dictionary_, a function that enables you to return custom metadata associated with the logged API calls. 
-        Takes in the [Requests](http://docs.python-requests.org/en/master/api/) request and response object as arguments. You should implement a function that 
-        returns a dictionary containing your custom metadata. (must be able to be encoded into JSON). For example, you may want to save a VM instance_id, a trace_id, or a resource_id with the request.
-        
-        ##### __`SKIP_OUTGOING`__
-        (optional) _(req, res) => boolean_, a function that takes a [Requests](http://docs.python-requests.org/en/master/api/) request and response,
-        and returns true if you want to skip this particular event.
-        
-        ##### __`IDENTIFY_USER_OUTGOING`__
-        (optional, but highly recommended) _(req, res) => string_, a function that takes [Requests](http://docs.python-requests.org/en/master/api/) request and response, and returns a string that is the user id used by your system. While Moesif tries to identify users automatically,
-        but different frameworks and your implementation might be very different, it would be helpful and much more accurate to provide this function.
-        
-        ##### __`IDENTIFY_COMPANY_OUTGOING`__
-        (optional) _(req, res) => string_, a function that takes [Requests](http://docs.python-requests.org/en/master/api/) request and response, and returns a string that is the company id for this event.
-        
-        ##### __`GET_SESSION_TOKEN_OUTGOING`__
-        (optional) _(req, res) => string_, a function that takes [Requests](http://docs.python-requests.org/en/master/api/) request and response, and returns a string that is the session token for this event. Again, Moesif tries to get the session token automatically, but if you setup is very different from standard, this function will be very help for tying events together, and help you replay the events.
-        
-        ##### __`LOG_BODY_OUTGOING`__
-        (optional) _boolean_, default True, Set to False to remove logging request and response body.
-        
-        ### Example:
-        
-        ```python
-        def identify_user(app, environ, response_headers=dict()):
-            # Your custom code that returns a user id string
-            return "12345"
-        
-        def identify_company(app, environ, response_headers=dict()):
-            # Your custom code that returns a company id string
-            return "67890"
-        
-        def should_skip(app, environ):
-            # Your custom code that returns true to skip logging
-            return "health/probe" in environ.get('PATH_INFO', '')
-        
-        def get_token(app, environ):
-            # If you don't want to use the standard WSGI session token,
-            # add your custom code that returns a string for session/API token
-            return "XXXXXXXXXXXXXX"
-        
-        def mask_event(eventmodel):
-            # Your custom code to change or remove any sensitive fields
-            if 'password' in eventmodel.response.body:
-                eventmodel.response.body['password'] = None
-            return eventmodel
-        
-        def get_metadata(app, environ):
-            return {
-                'datacenter': 'westus',
-                'deployment_version': 'v1.2.3',
-            }
-        
-        moesif_settings = {
-            'APPLICATION_ID': 'Your Moesif Application Id',
-            'DEBUG': False,
-            'LOG_BODY': True,
-            'IDENTIFY_USER': identify_user,
-            'IDENTIFY_COMPANY': identify_company,
-            'GET_SESSION_TOKEN': get_token,
-            'SKIP': should_skip,
-            'MASK_EVENT_MODEL': mask_event,
-            'GET_METADATA': get_metadata,
-            'CAPTURE_OUTGOING_REQUESTS': False
-        }
-        
-        app.wsgi_app = MoesifMiddleware(app.wsgi_app, moesif_settings)
-        
-        ```
-        
-        ## Update User
-        
-        ### Update A Single User
-        Create or update a user profile in Moesif.
-        The metadata field can be any customer demographic or other info you want to store.
-        Only the `user_id` field is required.
-        For details, visit the [Python API Reference](https://www.moesif.com/docs/api?python#update-a-user).
-        
-        ```python
-        api_client = MoesifAPIClient("Your Moesif Application Id").api
-        
-        # Only user_id is required.
-        # Campaign object is optional, but useful if you want to track ROI of acquisition channels
-        # See https://www.moesif.com/docs/api#users for campaign schema
-        # metadata can be any custom object
-        user = {
-          'user_id': '12345',
-          'company_id': '67890', # If set, associate user with a company object
-          'campaign': {
-            'utm_source': 'google',
-            'utm_medium': 'cpc', 
-            'utm_campaign': 'adwords',
-            'utm_term': 'api+tooling',
-            'utm_content': 'landing'
-          },
-          'metadata': {
-            'email': 'john@acmeinc.com',
-            'first_name': 'John',
-            'last_name': 'Doe',
-            'title': 'Software Engineer',
-            'sales_info': {
-                'stage': 'Customer',
-                'lifetime_value': 24000,
-                'account_owner': 'mary@contoso.com'
-            },
-          }
-        }
-        
-        update_user = api_client.update_user(user)
-        ```
-        
-        ### Update Users in Batch
-        Similar to update_user, but used to update a list of users in one batch. 
-        Only the `user_id` field is required.
-        For details, visit the [Python API Reference](https://www.moesif.com/docs/api?python#update-users-in-batch).
-        
-        ```python
-        api_client = MoesifAPIClient("Your Moesif Application Id").api
-        
-        userA = {
-          'user_id': '12345',
-          'company_id': '67890', # If set, associate user with a company object
-          'metadata': {
-            'email': 'john@acmeinc.com',
-            'first_name': 'John',
-            'last_name': 'Doe',
-            'title': 'Software Engineer',
-            'sales_info': {
-                'stage': 'Customer',
-                'lifetime_value': 24000,
-                'account_owner': 'mary@contoso.com'
-            },
-          }
-        }
-        
-        userB = {
-          'user_id': '54321',
-          'company_id': '67890', # If set, associate user with a company object
-          'metadata': {
-            'email': 'mary@acmeinc.com',
-            'first_name': 'Mary',
-            'last_name': 'Jane',
-            'title': 'Software Engineer',
-            'sales_info': {
-                'stage': 'Customer',
-                'lifetime_value': 48000,
-                'account_owner': 'mary@contoso.com'
-            },
-          }
-        }
-        update_users = api_client.update_users_batch([userA, userB])
-        ```
-        
-        ## Update Company
-        
-        ### Update A Single Company
-        Create or update a company profile in Moesif.
-        The metadata field can be any company demographic or other info you want to store.
-        Only the `company_id` field is required.
-        For details, visit the [Python API Reference](https://www.moesif.com/docs/api?python#update-a-company).
-        
-        ```python
-        api_client = MoesifAPIClient("Your Moesif Application Id").api
-        
-        # Only company_id is required.
-        # Campaign object is optional, but useful if you want to track ROI of acquisition channels
-        # See https://www.moesif.com/docs/api#update-a-company for campaign schema
-        # metadata can be any custom object
-        company = {
-          'company_id': '67890',
-          'company_domain': 'acmeinc.com', # If domain is set, Moesif will enrich your profiles with publicly available info 
-          'campaign': {
-            'utm_source': 'google',
-            'utm_medium': 'cpc', 
-            'utm_campaign': 'adwords',
-            'utm_term': 'api+tooling',
-            'utm_content': 'landing'
-          },
-          'metadata': {
-            'org_name': 'Acme, Inc',
-            'plan_name': 'Free',
-            'deal_stage': 'Lead',
-            'mrr': 24000,
-            'demographics': {
-                'alexa_ranking': 500000,
-                'employee_count': 47
-            },
-          }
-        }
-        
-        update_company = api_client.update_company(company)
-        ```
-        
-        ### Update Companies in Batch
-        Similar to update_company, but used to update a list of companies in one batch. 
-        Only the `company_id` field is required.
-        For details, visit the [Python API Reference](https://www.moesif.com/docs/api?python#update-companies-in-batch).
-        
-        ```python
-        api_client = MoesifAPIClient("Your Moesif Application Id").api
-        
-        companyA = {
-          'company_id': '67890',
-          'company_domain': 'acmeinc.com', # If domain is set, Moesif will enrich your profiles with publicly available info 
-          'metadata': {
-            'org_name': 'Acme, Inc',
-            'plan_name': 'Free',
-            'deal_stage': 'Lead',
-            'mrr': 24000,
-            'demographics': {
-                'alexa_ranking': 500000,
-                'employee_count': 47
-            },
-          }
-        }
-        
-        companyB = {
-          'company_id': '09876',
-          'company_domain': 'contoso.com', # If domain is set, Moesif will enrich your profiles with publicly available info 
-          'metadata': {
-            'org_name': 'Contoso, Inc',
-            'plan_name': 'Free',
-            'deal_stage': 'Lead',
-            'mrr': 48000,
-            'demographics': {
-                'alexa_ranking': 500000,
-                'employee_count': 53
-            },
-          }
-        }
-        
-        update_companies = api_client.update_companies_batch([companyA, companyB])
-        ```
-        ## Troubleshooting
-        
-        When using Docker with Ubuntu based image, if events are not being captured, it could be possible as the image can't find any timezone configuration. 
-        In order to resolve that, add the following line to your Dockerfile
-        ```
-        ENV TZ=UTC
-        ```
-        or you could add `RUN apt-get install tzdata` in the Dockerfile.
-        
-        ## Other integrations
-        
-        To view more documentation on integration options, please visit __[the Integration Options Documentation](https://www.moesif.com/docs/getting-started/integration-options/).__
-        
-        [ico-built-for]: https://img.shields.io/badge/built%20for-python%20wsgi-blue.svg
-        [ico-version]: https://img.shields.io/pypi/v/moesifwsgi.svg
-        [ico-language]: https://img.shields.io/pypi/pyversions/moesifwsgi.svg
-        [ico-license]: https://img.shields.io/badge/License-Apache%202.0-green.svg
-        [ico-source]: https://img.shields.io/github/last-commit/moesif/moesifwsgi.svg?style=social
-        
-        [link-built-for]: https://en.wikipedia.org/wiki/Web_Server_Gateway_Interface
-        [link-package]: https://pypi.python.org/pypi/moesifwsgi
-        [link-language]: https://pypi.python.org/pypi/moesifwsgi
-        [link-license]: https://raw.githubusercontent.com/Moesif/moesifwsgi/master/LICENSE
-        [link-source]: https://github.com/Moesif/moesifwsgi
-        
 Keywords: log analysis restful api development debug wsgi flask bottle http middleware
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: Log Analysis
 Classifier: Topic :: Software Development :: Debuggers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
+License-File: LICENSE
+
+# Moesif Middleware for Python WSGI based Frameworks
+
+[![Built For][ico-built-for]][link-built-for]
+[![Latest Version][ico-version]][link-package]
+[![Language Versions][ico-language]][link-language]
+[![Software License][ico-license]][link-license]
+[![Source Code][ico-source]][link-source]
+
+WSGI middleware that automatically logs _incoming_ or _outgoing_ API calls and sends to [Moesif](https://www.moesif.com) for API analytics and monitoring.
+Supports Python Frameworks built on WSGI such as Flask, Bottle, and Pyramid.
+
+[Source Code on GitHub](https://github.com/moesif/moesifwsgi)
+
+[WSGI (Web Server Gateway Interface)](https://wsgi.readthedocs.io/en/latest/)
+is a standard (PEP 3333) that describes
+how a web server communicates with web applications. Many Python Frameworks
+are build on top of WSGI, such as [Flask](http://flask.pocoo.org/),
+[Bottle](https://bottlepy.org/docs/dev/), [Pyramid](https://trypyramid.com/) etc.
+Moesif WSGI Middleware help APIs that are build on top of these Frameworks to
+easily integrate with [Moesif](https://www.moesif.com).
+
+## How to install
+
+```shell
+pip install moesifwsgi
+```
+
+## How to use
+
+### Flask
+
+Wrap your wsgi_app with the Moesif middleware.
+
+```python
+from moesifwsgi import MoesifMiddleware
+
+moesif_settings = {
+    'APPLICATION_ID': 'Your Moesif Application id',
+    'LOG_BODY': True,
+    # ... For other options see below.
+}
+
+app.wsgi_app = MoesifMiddleware(app.wsgi_app, moesif_settings)
+
+```
+
+Your Moesif Application Id can be found in the [_Moesif Portal_](https://www.moesif.com/).
+After signing up for a Moesif account, your Moesif Application Id will be displayed during the onboarding steps. 
+
+You can always find your Moesif Application Id at any time by logging 
+into the [_Moesif Portal_](https://www.moesif.com/), click on the top right menu,
+and then clicking _API Keys_.
+
+For an example with Flask, see example in the `/examples/flask` folder of this repo.
+
+### Bottle
+Wrap your bottle app with the Moesif middleware.
+
+```python
+
+from moesifwsgi import MoesifMiddleware
+
+app = bottle.Bottle()
+
+moesif_settings = {
+    'APPLICATION_ID': 'Your Moesif Application Id',
+    'LOG_BODY': True,
+    # ... For other options see below.
+}
+
+bottle.run(app=MoesifMiddleware(app, moesif_settings))
+
+```
+
+For an example with Bottle, see example in the `/examples/bottle` folder of this repo.
+
+### Pyramid
+
+
+```python
+from pyramid.config import Configurator
+from moesifwsgi import MoesifMiddleware
+
+if __name__ == '__main__':
+    config = Configurator()
+    config.add_route('hello', '/')
+    config.scan()
+    app = config.make_wsgi_app()
+
+    # configure your moesif settings
+    moesif_settings = {
+        'APPLICATION_ID': 'Your Moesif Application Id',
+        'LOG_BODY': True,
+        # ... For other options see below.
+    }
+    # Put middleware
+    app = MoesifMiddleware(app, moesif_settings)
+
+    server = make_server('0.0.0.0', 8080, app)
+    server.serve_forever()
+
+```
+### Other WSGI frameworks
+
+If you are using a framework that is built on top of WSGI, it should work just by adding the Moesif middleware.
+Please read the documentation for your specific framework on how to add middleware.
+
+## Configuration options
+
+#### __`APPLICATION_ID`__
+(__required__), _string_, is obtained via your Moesif Account, this is required.
+
+#### __`SKIP`__
+(optional) _(app, environ) => boolean_, a function that takes a WSGI app and an environ,
+and returns true if you want to skip this particular event. The app is the original WSGI app instance, and the
+environ is a [WSGI environ](http://wsgi.readthedocs.io/en/latest/definitions.html).
+
+#### __`IDENTIFY_USER`__
+(optional, but highly recommended) _(app, environ, response_headers) => string_, a function that takes an app, an environ and an optional parameter response headers, and returns a string that is the user id used by your system. While Moesif tries to identify users automatically,
+but different frameworks and your implementation might be very different, it would be helpful and much more accurate to provide this function.
+
+#### __`IDENTIFY_COMPANY`__
+(optional) _(app, environ, response_headers) => string_, a function that takes an app, an environ and an optional parameter response headers, and returns a string that is the company id for this event.
+
+#### __`GET_METADATA`__
+(optional) _(app, environ) => dictionary_, a function that takes an app and an environ, and
+returns a dictionary (must be able to be encoded into JSON). This allows your
+to associate this event with custom metadata. For example, you may want to save a VM instance_id, a trace_id, or a tenant_id with the request.
+
+#### __`GET_SESSION_TOKEN`__
+(optional) _(app, environ) => string_, a function that takes an app and an environ, and returns a string that is the session token for this event. Again, Moesif tries to get the session token automatically, but if you setup is very different from standard, this function will be very help for tying events together, and help you replay the events.
+
+#### __`MASK_EVENT_MODEL`__
+(optional) _(EventModel) => EventModel_, a function that takes an EventModel and returns an EventModel with desired data removed. The return value must be a valid EventModel required by Moesif data ingestion API. For details regarding EventModel please see the [Moesif Python API Documentation](https://www.moesif.com/docs/api?python).
+
+#### __`DEBUG`__
+(optional) _boolean_, a flag to see debugging messages.
+
+#### __`LOG_BODY`__
+(optional) _boolean_, default True, Set to False to remove logging request and response body.
+
+#### __`EVENT_QUEUE_SIZE`__
+(optional) __int__, default 10000, the maximum number of event objects queued in memory pending upload to Moesif.  If the queue is full additional calls to `MoesifMiddleware` will return immediately without logging the event, so this number should be set based on the expected event size and memory capacity
+
+### __`EVENT_WORKER_COUNT`__
+(optional) __int__, default 2, the number of worker threads to use for uploading events to Moesif.  If you have a large number of events being logged, increasing this number can improve upload performance.
+
+#### __`BATCH_SIZE`__
+(optional) __int__, default 100, Maximum batch size when sending events to Moesif when reading from the queue
+
+#### __`EVENT_BATCH_TIMEOUT`__
+(optional) __int__, default 2, Maximum time in seconds to wait before sending a batch of events to Moesif when reading from the queue
+
+#### __`AUTHORIZATION_HEADER_NAME`__
+(optional) _string_, A request header field name used to identify the User in Moesif. Default value is `authorization`. Also, supports a comma separated string. We will check headers in order like `"X-Api-Key,Authorization"`.
+
+#### __`AUTHORIZATION_USER_ID_FIELD`__
+(optional) _string_, A field name used to parse the User from authorization header in Moesif. Default value is `sub`.
+
+#### __`BASE_URI`__
+(optional) _string_, A local proxy hostname when sending traffic via secure proxy. Please set this field when using secure proxy. For more details, refer [secure proxy documentation.](https://www.moesif.com/docs/platform/secure-proxy/#2-configure-moesif-sdk)
+
+### Options specific to outgoing API calls 
+
+The options below are applicable to outgoing API calls (calls you initiate using the Python [Requests](http://docs.python-requests.org/en/master/) lib to third parties like Stripe or to your own services.
+
+For options that use the request and response as input arguments, these use the [Requests](http://docs.python-requests.org/en/master/api/) lib's request or response objects.
+
+If you are not using WSGI, you can import the [moesifpythonrequest](https://github.com/Moesif/moesifpythonrequest) directly.
+
+#### __`CAPTURE_OUTGOING_REQUESTS`__
+_boolean_, Default False. Set to True to capture all outgoing API calls. False will disable this functionality. 
+
+##### __`GET_METADATA_OUTGOING`__
+(optional) _(req, res) => dictionary_, a function that enables you to return custom metadata associated with the logged API calls. 
+Takes in the [Requests](http://docs.python-requests.org/en/master/api/) request and response object as arguments. You should implement a function that 
+returns a dictionary containing your custom metadata. (must be able to be encoded into JSON). For example, you may want to save a VM instance_id, a trace_id, or a resource_id with the request.
+
+##### __`SKIP_OUTGOING`__
+(optional) _(req, res) => boolean_, a function that takes a [Requests](http://docs.python-requests.org/en/master/api/) request and response,
+and returns true if you want to skip this particular event.
+
+##### __`IDENTIFY_USER_OUTGOING`__
+(optional, but highly recommended) _(req, res) => string_, a function that takes [Requests](http://docs.python-requests.org/en/master/api/) request and response, and returns a string that is the user id used by your system. While Moesif tries to identify users automatically,
+but different frameworks and your implementation might be very different, it would be helpful and much more accurate to provide this function.
+
+##### __`IDENTIFY_COMPANY_OUTGOING`__
+(optional) _(req, res) => string_, a function that takes [Requests](http://docs.python-requests.org/en/master/api/) request and response, and returns a string that is the company id for this event.
+
+##### __`GET_SESSION_TOKEN_OUTGOING`__
+(optional) _(req, res) => string_, a function that takes [Requests](http://docs.python-requests.org/en/master/api/) request and response, and returns a string that is the session token for this event. Again, Moesif tries to get the session token automatically, but if you setup is very different from standard, this function will be very help for tying events together, and help you replay the events.
+
+##### __`LOG_BODY_OUTGOING`__
+(optional) _boolean_, default True, Set to False to remove logging request and response body.
+
+### Example:
+
+```python
+def identify_user(app, environ, response_headers=dict()):
+    # Your custom code that returns a user id string
+    return "12345"
+
+def identify_company(app, environ, response_headers=dict()):
+    # Your custom code that returns a company id string
+    return "67890"
+
+def should_skip(app, environ):
+    # Your custom code that returns true to skip logging
+    return "health/probe" in environ.get('PATH_INFO', '')
+
+def get_token(app, environ):
+    # If you don't want to use the standard WSGI session token,
+    # add your custom code that returns a string for session/API token
+    return "XXXXXXXXXXXXXX"
+
+def mask_event(eventmodel):
+    # Your custom code to change or remove any sensitive fields
+    if 'password' in eventmodel.response.body:
+        eventmodel.response.body['password'] = None
+    return eventmodel
+
+def get_metadata(app, environ):
+    return {
+        'datacenter': 'westus',
+        'deployment_version': 'v1.2.3',
+    }
+
+moesif_settings = {
+    'APPLICATION_ID': 'Your Moesif Application Id',
+    'DEBUG': False,
+    'LOG_BODY': True,
+    'IDENTIFY_USER': identify_user,
+    'IDENTIFY_COMPANY': identify_company,
+    'GET_SESSION_TOKEN': get_token,
+    'SKIP': should_skip,
+    'MASK_EVENT_MODEL': mask_event,
+    'GET_METADATA': get_metadata,
+    'CAPTURE_OUTGOING_REQUESTS': False
+}
+
+app.wsgi_app = MoesifMiddleware(app.wsgi_app, moesif_settings)
+
+```
+
+## Update User
+
+### Update A Single User
+Create or update a user profile in Moesif.
+The metadata field can be any customer demographic or other info you want to store.
+Only the `user_id` field is required.
+For details, visit the [Python API Reference](https://www.moesif.com/docs/api?python#update-a-user).
+
+```python
+api_client = MoesifAPIClient("Your Moesif Application Id").api
+
+# Only user_id is required.
+# Campaign object is optional, but useful if you want to track ROI of acquisition channels
+# See https://www.moesif.com/docs/api#users for campaign schema
+# metadata can be any custom object
+user = {
+  'user_id': '12345',
+  'company_id': '67890', # If set, associate user with a company object
+  'campaign': {
+    'utm_source': 'google',
+    'utm_medium': 'cpc', 
+    'utm_campaign': 'adwords',
+    'utm_term': 'api+tooling',
+    'utm_content': 'landing'
+  },
+  'metadata': {
+    'email': 'john@acmeinc.com',
+    'first_name': 'John',
+    'last_name': 'Doe',
+    'title': 'Software Engineer',
+    'sales_info': {
+        'stage': 'Customer',
+        'lifetime_value': 24000,
+        'account_owner': 'mary@contoso.com'
+    },
+  }
+}
+
+update_user = api_client.update_user(user)
+```
+
+### Update Users in Batch
+Similar to update_user, but used to update a list of users in one batch. 
+Only the `user_id` field is required.
+For details, visit the [Python API Reference](https://www.moesif.com/docs/api?python#update-users-in-batch).
+
+```python
+api_client = MoesifAPIClient("Your Moesif Application Id").api
+
+userA = {
+  'user_id': '12345',
+  'company_id': '67890', # If set, associate user with a company object
+  'metadata': {
+    'email': 'john@acmeinc.com',
+    'first_name': 'John',
+    'last_name': 'Doe',
+    'title': 'Software Engineer',
+    'sales_info': {
+        'stage': 'Customer',
+        'lifetime_value': 24000,
+        'account_owner': 'mary@contoso.com'
+    },
+  }
+}
+
+userB = {
+  'user_id': '54321',
+  'company_id': '67890', # If set, associate user with a company object
+  'metadata': {
+    'email': 'mary@acmeinc.com',
+    'first_name': 'Mary',
+    'last_name': 'Jane',
+    'title': 'Software Engineer',
+    'sales_info': {
+        'stage': 'Customer',
+        'lifetime_value': 48000,
+        'account_owner': 'mary@contoso.com'
+    },
+  }
+}
+update_users = api_client.update_users_batch([userA, userB])
+```
+
+## Update Company
+
+### Update A Single Company
+Create or update a company profile in Moesif.
+The metadata field can be any company demographic or other info you want to store.
+Only the `company_id` field is required.
+For details, visit the [Python API Reference](https://www.moesif.com/docs/api?python#update-a-company).
+
+```python
+api_client = MoesifAPIClient("Your Moesif Application Id").api
+
+# Only company_id is required.
+# Campaign object is optional, but useful if you want to track ROI of acquisition channels
+# See https://www.moesif.com/docs/api#update-a-company for campaign schema
+# metadata can be any custom object
+company = {
+  'company_id': '67890',
+  'company_domain': 'acmeinc.com', # If domain is set, Moesif will enrich your profiles with publicly available info 
+  'campaign': {
+    'utm_source': 'google',
+    'utm_medium': 'cpc', 
+    'utm_campaign': 'adwords',
+    'utm_term': 'api+tooling',
+    'utm_content': 'landing'
+  },
+  'metadata': {
+    'org_name': 'Acme, Inc',
+    'plan_name': 'Free',
+    'deal_stage': 'Lead',
+    'mrr': 24000,
+    'demographics': {
+        'alexa_ranking': 500000,
+        'employee_count': 47
+    },
+  }
+}
+
+update_company = api_client.update_company(company)
+```
+
+### Update Companies in Batch
+Similar to update_company, but used to update a list of companies in one batch. 
+Only the `company_id` field is required.
+For details, visit the [Python API Reference](https://www.moesif.com/docs/api?python#update-companies-in-batch).
+
+```python
+api_client = MoesifAPIClient("Your Moesif Application Id").api
+
+companyA = {
+  'company_id': '67890',
+  'company_domain': 'acmeinc.com', # If domain is set, Moesif will enrich your profiles with publicly available info 
+  'metadata': {
+    'org_name': 'Acme, Inc',
+    'plan_name': 'Free',
+    'deal_stage': 'Lead',
+    'mrr': 24000,
+    'demographics': {
+        'alexa_ranking': 500000,
+        'employee_count': 47
+    },
+  }
+}
+
+companyB = {
+  'company_id': '09876',
+  'company_domain': 'contoso.com', # If domain is set, Moesif will enrich your profiles with publicly available info 
+  'metadata': {
+    'org_name': 'Contoso, Inc',
+    'plan_name': 'Free',
+    'deal_stage': 'Lead',
+    'mrr': 48000,
+    'demographics': {
+        'alexa_ranking': 500000,
+        'employee_count': 53
+    },
+  }
+}
+
+update_companies = api_client.update_companies_batch([companyA, companyB])
+```
+## Troubleshooting
+
+When using Docker with Ubuntu based image, if events are not being captured, it could be possible as the image can't find any timezone configuration. 
+In order to resolve that, add the following line to your Dockerfile
+```
+ENV TZ=UTC
+```
+or you could add `RUN apt-get install tzdata` in the Dockerfile.
+
+## Other integrations
+
+To view more documentation on integration options, please visit __[the Integration Options Documentation](https://www.moesif.com/docs/getting-started/integration-options/).__
+
+[ico-built-for]: https://img.shields.io/badge/built%20for-python%20wsgi-blue.svg
+[ico-version]: https://img.shields.io/pypi/v/moesifwsgi.svg
+[ico-language]: https://img.shields.io/pypi/pyversions/moesifwsgi.svg
+[ico-license]: https://img.shields.io/badge/License-Apache%202.0-green.svg
+[ico-source]: https://img.shields.io/github/last-commit/moesif/moesifwsgi.svg?style=social
+
+[link-built-for]: https://en.wikipedia.org/wiki/Web_Server_Gateway_Interface
+[link-package]: https://pypi.python.org/pypi/moesifwsgi
+[link-language]: https://pypi.python.org/pypi/moesifwsgi
+[link-license]: https://raw.githubusercontent.com/Moesif/moesifwsgi/master/LICENSE
+[link-source]: https://github.com/Moesif/moesifwsgi
```

### Comparing `moesifwsgi-1.6.1/moesifwsgi.egg-info/SOURCES.txt` & `moesifwsgi-1.7.0/moesifwsgi.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 moesifwsgi/__init__.py
 moesifwsgi/client_ip.py
+moesifwsgi/config_manager.py
 moesifwsgi/event_mapper.py
 moesifwsgi/http_response_catcher.py
 moesifwsgi/logger_helper.py
 moesifwsgi/middleware.py
 moesifwsgi/moesif_data_holder.py
 moesifwsgi/parse_body.py
 moesifwsgi/regex_config_helper.py
-moesifwsgi/send_batch_events.py
 moesifwsgi/update_companies.py
 moesifwsgi/update_users.py
+moesifwsgi/workers.py
 moesifwsgi.egg-info/PKG-INFO
 moesifwsgi.egg-info/SOURCES.txt
 moesifwsgi.egg-info/dependency_links.txt
 moesifwsgi.egg-info/requires.txt
 moesifwsgi.egg-info/top_level.txt
```

### Comparing `moesifwsgi-1.6.1/setup.py` & `moesifwsgi-1.7.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 setup(
     name='moesifwsgi',
 
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='1.6.1',
+    version='1.7.0',
 
     description='Moesif Middleware for Python WSGI based platforms (Flask, Bottle & Others)',
     long_description=long_description,
     long_description_content_type="text/markdown",
 
     # The project's main homepage.
     url='https://www.moesif.com/docs/server-integration/python-wsgi/',
@@ -60,33 +60,44 @@
 
         # Pick your license as you wish (should match "license" above)
         'License :: OSI Approved :: Apache Software License',
 
         # Specify the Python versions you support here. In particular, ensure
         # that you indicate whether you support Python 2, Python 3 or both.
         'Programming Language :: Python :: 2',
-        'Programming Language :: Python :: 2.6',
         'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.3',
         'Programming Language :: Python :: 3.4',
         'Programming Language :: Python :: 3.5',
+        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ],
 
     keywords='log analysis restful api development debug wsgi flask bottle http middleware',
 
     # You can just specify the packages manually here if your project is
     # simple. Or you can use find_packages().
     packages=find_packages(exclude=['contrib', 'docs', 'tests']),
 
     # List run-time dependencies here.  These will be installed by pip when
     # your project is installed. For an analysis of "install_requires" vs pip's
     # requirements files see:
     # https://packaging.python.org/en/latest/requirements.html
-    install_requires=['requests', 'isodatetimehandler', 'moesifapi>=1.4.0', 'moesifpythonrequest>=0.3.0', 'apscheduler'],
+    install_requires=[
+        'requests>=2.0.0', 
+        'isodatetimehandler>=1.0.0', 
+        'moesifapi>=1.4.0', 
+        'moesifpythonrequest>=0.3.0', 
+        'readerwriterlock>=1.0.9'
+    ],
 
     # List additional groups of dependencies here (e.g. development
     # dependencies). You can install these using the following syntax,
     # for example:
     # $ pip install -e .[dev,test]
     extras_require={
         'dev': [],
```

