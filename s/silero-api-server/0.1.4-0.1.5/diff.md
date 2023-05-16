# Comparing `tmp/silero_api_server-0.1.4.tar.gz` & `tmp/silero_api_server-0.1.5.tar.gz`

## Comparing `silero_api_server-0.1.4.tar` & `silero_api_server-0.1.5.tar`

### file list

```diff
@@ -1,14 +1,11 @@
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 silero_api_server-0.1.4/.env
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 silero_api_server-0.1.4/requirements.txt
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 silero_api_server-0.1.4/run.ps1
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 silero_api_server-0.1.4/run.sh
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 silero_api_server-0.1.4/.github/workflows/publish-to-test-pypi.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 silero_api_server-0.1.4/silero_api_server/__init__.py
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 silero_api_server-0.1.4/silero_api_server/__main__.py
--rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 silero_api_server-0.1.4/silero_api_server/server.py
--rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 silero_api_server-0.1.4/silero_api_server/tts.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 silero_api_server-0.1.4/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 silero_api_server-0.1.4/LICENSE
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 silero_api_server-0.1.4/README.md
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 silero_api_server-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 silero_api_server-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 silero_api_server-0.1.5/requirements.txt
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 silero_api_server-0.1.5/.github/workflows/publish-to-test-pypi.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 silero_api_server-0.1.5/silero_api_server/__init__.py
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 silero_api_server-0.1.5/silero_api_server/__main__.py
+-rw-r--r--   0        0        0     2210 2020-02-02 00:00:00.000000 silero_api_server-0.1.5/silero_api_server/server.py
+-rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 silero_api_server-0.1.5/silero_api_server/tts.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 silero_api_server-0.1.5/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 silero_api_server-0.1.5/LICENSE
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 silero_api_server-0.1.5/README.md
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 silero_api_server-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 silero_api_server-0.1.5/PKG-INFO
```

### Comparing `silero_api_server-0.1.4/.github/workflows/publish-to-test-pypi.yml` & `silero_api_server-0.1.5/.github/workflows/publish-to-test-pypi.yml`

 * *Files identical despite different names*

### Comparing `silero_api_server-0.1.4/silero_api_server/server.py` & `silero_api_server-0.1.5/silero_api_server/server.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 
 import pathlib
-import dotenv, os
+import os
 from fastapi import FastAPI, Response, HTTPException, Request
 from fastapi.middleware.cors import CORSMiddleware
 from fastapi.responses import FileResponse
 from fastapi.staticfiles import StaticFiles
 from pydantic import BaseModel
 import uvicorn
 from silero_api_server.tts import SileroTtsService
 from loguru import logger
 from typing import Optional
 
 
-dotenv.load_dotenv()
-HOSTNAME = os.getenv('TTS_SERVER_HOSTNAME')
-PORT = os.getenv('TTS_SERVER_PORT')
-LOCAL_URL = f"http://{HOSTNAME}:{PORT}"
 
 module_path = pathlib.Path(__file__).resolve().parent
 os.chdir(module_path)
 SAMPLE_PATH = "samples"
 
 tts_service = SileroTtsService(f"{module_path}//{SAMPLE_PATH}")
 app = FastAPI()
```

### Comparing `silero_api_server-0.1.4/silero_api_server/tts.py` & `silero_api_server-0.1.5/silero_api_server/tts.py`

 * *Files identical despite different names*

### Comparing `silero_api_server-0.1.4/LICENSE` & `silero_api_server-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `silero_api_server-0.1.4/pyproject.toml` & `silero_api_server-0.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `silero_api_server-0.1.4/PKG-INFO` & `silero_api_server-0.1.5/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: silero-api-server
-Version: 0.1.4
+Version: 0.1.5
 Summary: A simple FastAPI server to host Silero TTS
 Project-URL: Homepage, https://github.com/ouoertheo/silero-api-server
 Project-URL: Bug Tracker, https://github.com/ouoertheo/silero-api-server/issues
 Author-email: Ouoertheo <ouoertheo@tomeofjamin.net>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -22,28 +22,32 @@
 Description-Content-Type: text/markdown
 
 # A simple FastAPI Server to run Silero TTS
 [Silero PyTorch Page](https://pytorch.org/hub/snakers4_silero-models_tts/)
 [Silero GitHub Page](https://github.com/snakers4/silero-models)
 
 ## Installation
-Recommended to use venv. You can install using the following commands. Change the script name if you are installing from cmd or bash
-```
-py -m venv .\venv
-.\venv\scripts\Activate.ps1
-pip install -r requirements.txt
+`pip install silero-api-server`
+
+## Starting Server
+`py -m silero_api_server` will run on default ip and port (0.0.0.0:8001)
+
 ```
+usage: silero_api_server [-h] [-o HOST] [-p PORT]
 
-## Configuration
-The server runs on `localhost:8001` by default. You can leave IP at 0.0.0.0 to listen on all IPs.
-Ports will be updated in the `run` script. Port and hostname will be updated in `.env` file. 
+Run Silero within a FastAPI application
 
-On first run of server, the model will need to be downloaded, this will happen automatically and may take a few minutes depending on your connection speed.
+options:
+  -h, --help            show this help message and exit
+  -o HOST, --host HOST
+  -p PORT, --port PORT
+```
 
-## Starting Server
-Enter the venv `.\venv\scripts\Activate.ps1`
-Execute the included `run.ps1` or `run.sh`
-You can access the API spec at `http://localhost:8001/docs`
+On first run of server, two operations occur automatically. These may take a minute or two.
+1. The model will be downloaded 
+2. Voice samples will be generated generated. 
+
+# API Docs
+API Docs can be accessed from [http://localhost:8001/docs](http://localhost:8001/docs)
 
-## Voice Samples
-Samples must be generated by a POST command to `/generate-samples`  (easy way to run is from http://localhost:8001/docs)
+# Voice Samples
 Samples are served statically by the web server at `/samples/{speaker}.wav` or callable from the API from `/tts/sample?speaker={speaker}` endpoint.
```

