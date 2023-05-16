# Comparing `tmp/deepset_cloud_sdk-0.0.6.tar.gz` & `tmp/deepset_cloud_sdk-0.0.7.tar.gz`

## Comparing `deepset_cloud_sdk-0.0.6.tar` & `deepset_cloud_sdk-0.0.7.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.6/CONTRIBUTING.md
--rw-r--r--   0        0        0    48074 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.6/assets/logo.png
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.6/deepset_cloud_sdk/README.md
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.6/deepset_cloud_sdk/__about__.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.6/deepset_cloud_sdk/__init__.py
--rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.6/deepset_cloud_sdk/cli.py
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.6/deepset_cloud_sdk/models.py
--rw-r--r--   0        0        0     2354 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.6/deepset_cloud_sdk/api/config.py
--rw-r--r--   0        0        0     6699 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.6/deepset_cloud_sdk/api/deepset_cloud_api.py
--rw-r--r--   0        0        0     3878 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.6/deepset_cloud_sdk/api/files.py
--rw-r--r--   0        0        0     9332 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.6/deepset_cloud_sdk/api/upload_sessions.py
--rw-r--r--   0        0        0     8273 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.6/deepset_cloud_sdk/s3/upload.py
--rw-r--r--   0        0        0    10840 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.6/deepset_cloud_sdk/service/files_service.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.6/deepset_cloud_sdk/utils/__init__.py
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.6/deepset_cloud_sdk/utils/progress_bar.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.6/deepset_cloud_sdk/workflows/__init__.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.6/deepset_cloud_sdk/workflows/async_client/__init__.py
--rw-r--r--   0        0        0     4815 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.6/deepset_cloud_sdk/workflows/async_client/files.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.6/deepset_cloud_sdk/workflows/sync_client/__init__.py
--rw-r--r--   0        0        0     5154 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.6/deepset_cloud_sdk/workflows/sync_client/files.py
--rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.6/examples/cli/README.md
--rw-r--r--   0        0        0     3036 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.6/examples/data/example.pdf
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.6/examples/data/example.txt
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.6/examples/data/example.txt.meta.json
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.6/examples/sdk/README.md
--rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.6/examples/sdk/upload.py
--rw-r--r--   0        0        0     3165 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.6/.gitignore
--rw-r--r--   0        0        0     2690 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.6/README.md
--rw-r--r--   0        0        0     3907 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     3787 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.7/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.7/CONTRIBUTING.md
+-rw-r--r--   0        0        0    48074 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.7/assets/logo.png
+-rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.7/deepset_cloud_sdk/README.md
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.7/deepset_cloud_sdk/__about__.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.7/deepset_cloud_sdk/__init__.py
+-rw-r--r--   0        0        0     2824 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.7/deepset_cloud_sdk/cli.py
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.7/deepset_cloud_sdk/models.py
+-rw-r--r--   0        0        0     2388 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.7/deepset_cloud_sdk/api/config.py
+-rw-r--r--   0        0        0     6587 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.7/deepset_cloud_sdk/api/deepset_cloud_api.py
+-rw-r--r--   0        0        0     3876 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.7/deepset_cloud_sdk/api/files.py
+-rw-r--r--   0        0        0     9323 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.7/deepset_cloud_sdk/api/upload_sessions.py
+-rw-r--r--   0        0        0     8281 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.7/deepset_cloud_sdk/s3/upload.py
+-rw-r--r--   0        0        0    10891 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.7/deepset_cloud_sdk/service/files_service.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.7/deepset_cloud_sdk/utils/__init__.py
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.7/deepset_cloud_sdk/utils/progress_bar.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.7/deepset_cloud_sdk/workflows/__init__.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.7/deepset_cloud_sdk/workflows/async_client/__init__.py
+-rw-r--r--   0        0        0     5038 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.7/deepset_cloud_sdk/workflows/async_client/files.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.7/deepset_cloud_sdk/workflows/sync_client/__init__.py
+-rw-r--r--   0        0        0     5208 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.7/deepset_cloud_sdk/workflows/sync_client/files.py
+-rw-r--r--   0        0        0     2883 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.7/examples/cli/README.md
+-rw-r--r--   0        0        0     3036 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.7/examples/data/example.pdf
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.7/examples/data/example.txt
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.7/examples/data/example.txt.meta.json
+-rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.7/examples/sdk/README.md
+-rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.7/examples/sdk/upload.py
+-rw-r--r--   0        0        0     3165 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.7/.gitignore
+-rw-r--r--   0        0        0     2631 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.7/README.md
+-rw-r--r--   0        0        0     3955 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     3759 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.7/PKG-INFO
```

### Comparing `deepset_cloud_sdk-0.0.6/.pre-commit-config.yaml` & `deepset_cloud_sdk-0.0.7/.pre-commit-config.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -23,15 +23,16 @@
   - repo: https://github.com/pre-commit/mirrors-mypy
     # Please keep these aligned with the versions defined in the pyproject.toml [tool.hatch.envs.code-quality]
     rev: "v1.1.1"
     hooks:
       - id: mypy
         args:
           - "--ignore-missing-imports"
-        # additional_dependencies:
+        additional_dependencies:
+          - "types-tabulate~=0.9.0"
         #   - "types-Markdown~=3.4.2"
         #   - "types-requests~=2.28.11"
         #   - "types-PyYAML~=6.0.12"
         #   - "types-python-dateutil~=2.8.19"
         #   - "types-redis~=4.5.1"
 
   - repo: https://github.com/pycqa/isort
```

### Comparing `deepset_cloud_sdk-0.0.6/assets/logo.png` & `deepset_cloud_sdk-0.0.7/assets/logo.png`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-0.0.6/deepset_cloud_sdk/README.md` & `deepset_cloud_sdk-0.0.7/deepset_cloud_sdk/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-# Software development kit for the deepset.ai cloud API
+# Software development kit for the deepset Cloud API
 
 This package is split into multiple layers:
 - API layer
 - Client layer
 - Service layer
 - Workflow layer
 
 
 ### API layer
-This layer is the lowest level of abstraction and contains the API definition including all HTTP methods and takes care of the authentication.
+This layer is the lowest level of abstraction and contains the API definition, including all HTTP methods. It takes care of the authentication.
 You can find this layer in the `deepset_cloud_sdk/api/deepset_cloud_api.py` file. We should implement reties on this lowest layer.
 
 ### Client layer
-This layer adds a thin wrapper around the API layer and provides a more convenient interface to the API. It for example includes explicit methods
-for endpoints by specifying the HTTP methods and endpoints for e.g. uploading files.
+This layer adds a thin wrapper around the API layer and provides a more convenient interface to the API. It includes explicit methods
+for endpoints by specifying the HTTP methods and endpoints for example for uploading files.
 
 ### Service layer
-This layer takes care of combining client methods to provide more complex functionality. Within this layer we can add functionalities like
-first creating sessions, uploading files, and later closing them.
+This layer takes care of combining client methods to provide more complex functionality. Within this layer, we can add functionalities like
+creating sessions, uploading files, and closing sessions.
 
 ### Workflow layer
-Public methods to be used by users. These workflows are split into async and sync implementation.
+Public methods for users. These workflows are split into async and sync implementation.
 
 
 ## Software architecture principles
 
 ### Factories
 We are using factories implemented like this:
 ```python
```

### Comparing `deepset_cloud_sdk-0.0.6/deepset_cloud_sdk/api/config.py` & `deepset_cloud_sdk-0.0.7/deepset_cloud_sdk/api/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,19 +10,19 @@
 
 ENV_FILE_PATH = os.path.expanduser("~/.deepset-cloud-cli/.env")
 
 
 def load_environment() -> bool:
     """Load environment variables from .env file.
 
-    If a .env file is present in the current directory, load the environment variables from there.
+    If an .env file is present in the current directory, load the environment variables from there.
     Otherwise, load the environment variables from the .env file in the home directory that can be created using the CLI.
     To create the .env file in the home directory, run `deepset-cloud-cli login` in the terminal.
 
-    :return: True if the environment variables were loaded successfully, False otherwise
+    :return: True if the environment variables were loaded successfully, False otherwise.
     """
     successfully_loded_env: bool = False
     current_path_env = os.path.join(os.getcwd(), ".env")
     if os.path.isfile(current_path_env):
         # Load the environment variables from the .env file in the current directory
         successfully_loded_env = load_dotenv(current_path_env)
         return successfully_loded_env
@@ -33,31 +33,31 @@
 
 
 loaded_env_vars = load_environment()
 if loaded_env_vars:
     logger.info("Environment variables loaded successfully")
 else:
     logger.info(
-        "No environment variables loaded from .env file. API_KEY and API_URL need to be set manually. If you dont wan't to set them manually, run `deepset-cloud-cli login` in the terminal."
+        "No environment variables were loaded from the .env file. Set API_KEY and API_URL manually. If you dont wan't to set them manually, run `deepset-cloud-cli login` in the terminal."
     )
 
 # connection to deepset Cloud
 API_URL: str = os.getenv("API_URL", "https://api.cloud.deepset.ai/")
 API_KEY: str = os.getenv("API_KEY", "")
 
 # configuration to use a selectd workspace
 DEFAULT_WORKSPACE_NAME: str = os.getenv("DEFAULT_WORKSPACE_NAME", "")
 
 
 @dataclass
 class CommonConfig:
-    """Common config for connecting to Deepset Cloud API."""
+    """Common config for connecting to the deepset Cloud API."""
 
     api_key: str = API_KEY
     api_url: str = API_URL
 
     def __post_init__(self) -> None:
         """Validate config."""
         assert (
             self.api_key != ""
-        ), "API_KEY environment variable must be set. Please visit https://cloud.deepset.ai/settings/connections to get an API key."
+        ), "You must set the API_KEY environment variable. Go to [Connections](https://cloud.deepset.ai/settings/connections) in deepset Cloud to get an API key."
         assert self.api_url != "", "API_URL environment variable must be set"
```

### Comparing `deepset_cloud_sdk-0.0.6/deepset_cloud_sdk/api/deepset_cloud_api.py` & `deepset_cloud_sdk-0.0.7/deepset_cloud_sdk/api/deepset_cloud_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,30 +10,27 @@
 
 from deepset_cloud_sdk.api.config import CommonConfig
 
 logger = structlog.get_logger(__name__)
 
 
 class WorkspaceNotDefinedError(Exception):
-    """Workspace not defined error. This exception is raised if a workspace_name is not defined.
-
-    This can happen if neither an environment variable was set, nor a workspace_name was passed as an argument.
-    """
+    """The workspace_name is not defined. Set an environment variable or pass the `workspace_name` argument."""
 
 
 class DeepsetCloudAPI:
-    """Deepset cloud API client.
+    """deepset Cloud API client.
 
-    This class takes care of all API calls to deepset Cloud and handles authentication and error handling.
+    This class takes care of all API calls to deepset Cloud and handles authentication and errors.
     """
 
     def __init__(self, config: CommonConfig, client: httpx.AsyncClient) -> None:
-        """Create a deepset cloud api client.
+        """Create a deepset Cloud API client.
 
-        Add a config for authencation and a httpx client for
+        Add a config for authencation and a HTTPX client for
         sending requests.
 
         :param config: Config for authentication.
         :param client: HTTPX client for sending requests.
         """
         self.headers = {
             "Accept": "application/json",
@@ -41,21 +38,21 @@
         }
         self.base_url = lambda workspace_name: self._get_base_url(config.api_url)(workspace_name)
         self.client = client
 
     @staticmethod
     def _get_base_url(api_url: str) -> Callable:
         def func(workspace_name: str) -> str:
-            """Get the base url for the API.
+            """Get the base URL for the API.
 
             :param workspace_name: Name of the workspace to use.
-            :return: Base url.
+            :return: Base URL.
             """
             if not workspace_name or workspace_name == "":
-                raise WorkspaceNotDefinedError(f"Workspace name not defined. Got '{workspace_name}'")
+                raise WorkspaceNotDefinedError(f"Workspace name is not defined. Got '{workspace_name}'")
 
             return f"{api_url}/workspaces/{workspace_name}"
 
         return func
 
     @classmethod
     @asynccontextmanager
@@ -192,14 +189,14 @@
             data=data or {},
             status=response.status_code,
         )
         return response
 
 
 def get_deepset_cloud_api(config: CommonConfig, client: httpx.AsyncClient) -> DeepsetCloudAPI:
-    """Deepset Cloud API factory. Returns an instance of DeepsetCloudAPI.
+    """Deepset Cloud API factory. Return an instance of DeepsetCloudAPI.
 
     :param config: CommonConfig object.
     :param client: httpx.AsyncClient object.
     :return: DeepsetCloudAPI object.
     """
     return DeepsetCloudAPI(config=config, client=client)
```

### Comparing `deepset_cloud_sdk-0.0.6/deepset_cloud_sdk/api/files.py` & `deepset_cloud_sdk-0.0.7/deepset_cloud_sdk/api/files.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 File API for deepset Cloud.
 
-This module takes care of all file related API calls to deepset Cloud, including uploading, downloading, listing and
+This module takes care of all file-related API calls to deepset Cloud, including uploading, downloading, listing and
 deleting files.
 """
 
 import datetime
 import inspect
 import time
 from dataclasses import dataclass
@@ -18,51 +18,51 @@
 from deepset_cloud_sdk.api.deepset_cloud_api import DeepsetCloudAPI
 
 logger = structlog.get_logger(__name__)
 
 
 @dataclass
 class File:
-    """File primitive from deepset Cloud. This dataclass is used for all file related operations that dont include thea actual file content."""
+    """File primitive from deepset Cloud. This dataclass is used for all file-related operations that don't include thea actual file content."""
 
     file_id: UUID
     url: str
     name: str
     size: int
     created_at: datetime.datetime
     meta: Dict[str, Any]
 
     @classmethod
     def from_dict(cls, env: Dict[str, Any]) -> Any:
         """Parse a dictionary into a File object.
 
-        Not existing keys will be ignored.
+        Ignores keys that don't exist.
 
         :param env: Dictionary to parse.
         """
         to_parse = {k: v for k, v in env.items() if k in inspect.signature(cls).parameters}
         to_parse["created_at"] = datetime.datetime.fromisoformat(to_parse["created_at"])
         to_parse["file_id"] = UUID(to_parse["file_id"])
         return cls(**to_parse)
 
 
 @dataclass
 class FileList:
-    """List of files from deepset Cloud. This dataclass is used for all file related operations that return a list of files."""
+    """List of files from deepset Cloud. This dataclass is used for all file-related operations that return a list of files."""
 
     total: int
     data: List[File]
     has_more: bool
 
 
 class FilesAPI:
     """File API for deepset Cloud.
 
-    This module takes care of all file related API calls to deepset Cloud, including
-    uploading, downloading, listing and deleting files.
+    This module takes care of all file-related API calls to deepset Cloud, including
+    uploading, downloading, listing, and deleting files.
 
     :param deepset_cloud_api: Instance of the DeepsetCloudAPI.
     """
 
     def __init__(self, deepset_cloud_api: DeepsetCloudAPI) -> None:
         """
         Create FileAPI object.
@@ -78,15 +78,15 @@
         name: Optional[str] = None,
         content: Optional[str] = None,
         odata_filter: Optional[str] = None,
         after_value: Optional[Any] = None,
         after_file_id: Optional[UUID] = None,
     ) -> FileList:
         """
-        List files in a workspace, paginated with cursor based pagination.
+        List files in a workspace, paginated with cursor-based pagination.
 
         :param workspace_name: Name of the workspace to use.
         :param limit: Number of files to return per page.
         :param name: Name of the file to odata_filter by.
         :param content: Content of the file to odata_filter by.
         :param odata_filter: Odata odata_filter to apply.
         :param after_value: Value to start after.
```

### Comparing `deepset_cloud_sdk-0.0.6/deepset_cloud_sdk/api/upload_sessions.py` & `deepset_cloud_sdk-0.0.7/deepset_cloud_sdk/api/upload_sessions.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 
 
 @dataclass
 class UploadSessionIngestionStatus:
     """Upload session ingestion status.
 
     This status only contains the number of processed and therefore failed and finished files.
-    The total number of uploaded files need to be tracked by the client.
+    The total number of uploaded files needs to be tracked by the client.
     """
 
     failed_files: int
     finished_files: int
 
 
 @dataclass
@@ -117,17 +117,17 @@
         """
         self._deepset_cloud_api = deepset_cloud_api
 
     async def create(self, workspace_name: str, write_mode: WriteMode = WriteMode.KEEP) -> UploadSession:
         """Create upload session.
 
         This method creates an upload session for a given workspace. The upload session
-        is valid for 24 hours. After that, a new upload session needs to be created.
+        is valid for 24 hours. After that, you need to create a new upload session.
 
-        Each session needs to be closed to start the ingestion.
+        You must close a session to start the ingestion.
 
         :param workspace_name: Name of the workspace.
         :raises FailedToSendUploadSessionRequest: If the session could not be created.
         :return: UploadSession object.
         """
         response = await self._deepset_cloud_api.post(
             workspace_name=workspace_name, endpoint="upload_sessions", data={"write_mode": write_mode.value}
@@ -151,16 +151,16 @@
                 url=response_body["aws_prefixed_request_config"]["url"],
             ),
         )
 
     async def close(self, workspace_name: str, session_id: UUID) -> None:
         """Close upload session.
 
-        This method closes an upload session for a given workspace. Once the session is closed, no more files can be
-        uploaded to this session and the ingestion is automatically started.
+        This method closes an upload session for a given workspace. Once the session is closed, you can't upload
+        more files to this session and the ingestion is automatically started.
         This means that your files will appear in the workspace after a short while.
 
         :param workspace_name: Name of the workspace.
         :param session_id: ID of the session.
         :raises FailedToSendUploadSessionRequest: If the session could not be closed.
         :raises FailedToSendUploadSessionRequest: If the status could not be fetched.
         """
```

### Comparing `deepset_cloud_sdk-0.0.6/deepset_cloud_sdk/s3/upload.py` & `deepset_cloud_sdk-0.0.7/deepset_cloud_sdk/s3/upload.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Module for Upload related S3 Operations."""
+"""Module for upload-related S3 operations."""
 import asyncio
 import json
 import os
 import re
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Any, Coroutine, List
@@ -36,20 +36,19 @@
 
     file_name: str
     success: bool
 
 
 def make_safe_file_name(file_name: str) -> str:
     """
-    Transform a given string to a representation that can be accepted by S3.
+    Transform a given string to a representation that S3 accepts.
 
-    :param str: The file name
-    :return str: The transformed string
-    See for details of character exclusions:
-    https://docs.aws.amazon.com/AmazonS3/latest/userguide/object-keys.html
+    :param str: The file name.
+    :return str: The transformed string.
+    For character exclusions, see [Creating object key names](https://docs.aws.amazon.com/AmazonS3/latest/userguide/object-keys.html).
     """
     transformed = re.sub(r"[\\\\#%\"'\|<>\{\}`\^\[\]~\x00-\x1F]", "_", file_name)
     return quote(transformed)
 
 
 class S3:
     """Client for S3 operations related to deepset Cloud uploads."""
@@ -69,15 +68,15 @@
         file_name: str,
         upload_session: UploadSession,
         content: Any,
         client_session: aiohttp.ClientSession,
     ) -> aiohttp.ClientResponse:
         """Upload a file to the prefixed S3 namespace.
 
-        :param file_path: The Path to upload from.
+        :param file_path: The path to upload from.
         :param upload_session: UploadSession to associate the upload with.
         :param client_session: The aiohttp ClientSession to use for this request.
         :return: ClientResponse object.
         """
         aws_safe_name = make_safe_file_name(file_name)
         aws_config = upload_session.aws_prefixed_request_config
 
@@ -98,18 +97,18 @@
         file_path: Path,
         upload_session: UploadSession,
         client_session: aiohttp.ClientSession,
         progress: ProgressBar,
     ) -> S3UploadResult:
         """Upload a file to the prefixed S3 namespace given a path.
 
-        :param file_path: The Path to upload from.
+        :param file_path: The path to upload from.
         :param upload_session: UploadSession to associate the upload with.
         :param client_session: The aiohttp ClientSession to use for this request.
-        :param progress: A progress bar
+        :param progress: A progress bar.
         :return: S3UploadResult object.
         """
         async with self.semaphore:
             with open(file_path, "rb") as file:
                 file_name = os.path.basename(file_path)
                 try:
                     await self._upload_file_with_retries(file_name, upload_session, file, client_session)
@@ -131,28 +130,28 @@
         progress: ProgressBar,
     ) -> S3UploadResult:
         """Upload text to the prefixed S3 namespace.
 
         :param file_name: Name of the file.
         :param upload_session: UploadSession to associate the upload with.
         :param client_session: The aiohttp ClientSession to use for this request.
-        :param progress: A progress bar
+        :param progress: A progress bar.
         :return: S3UploadResult object.
         """
         try:
             await self._upload_file_with_retries(file_name, upload_session, content, client_session)
             progress.next()
             return S3UploadResult(file_name=file_name, success=True)
         except HTTPError:
             logger.warn("Could not upload a file to S3", file_name=file_name, session_id=upload_session.session_id)
             progress.next()
             return S3UploadResult(file_name=file_name, success=False)
 
     async def _process_results(self, tasks: List[Coroutine[Any, Any, S3UploadResult]]) -> S3UploadSummary:
-        """Summarise the results of the Uploads to S3.
+        """Summarize the results of the uploads to S3.
 
         :param tasks: List of upload tasks.
         :return: S3UploadResult object.
         """
         results: List[S3UploadResult] = await asyncio.gather(*tasks)
         logger.info("Finished uploading files", results=results)
 
@@ -173,15 +172,15 @@
 
         return result_summary
 
     async def upload_files_from_paths(self, upload_session: UploadSession, file_paths: List[Path]) -> S3UploadSummary:
         """Upload a set of files to the prefixed S3 namespace given a list of paths.
 
         :param upload_session: UploadSession to associate the upload with.
-        :param file_paths: A list of Paths to upload.
+        :param file_paths: A list of paths to upload.
         :return: S3UploadSummary object.
         """
         with ProgressBar(
             f"Uploading to S3",
             max=len(file_paths),
         ) as bar:
             async with aiohttp.ClientSession(connector=self.connector) as client_session:
```

### Comparing `deepset_cloud_sdk-0.0.6/deepset_cloud_sdk/service/files_service.py` & `deepset_cloud_sdk-0.0.7/deepset_cloud_sdk/service/files_service.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Module for all file related operations."""
+"""Module for all file-related operations."""
 from __future__ import annotations
 
 import asyncio
 import enum
 import os
 import time
 from contextlib import asynccontextmanager
@@ -29,15 +29,15 @@
 from deepset_cloud_sdk.models import DeepsetCloudFile
 from deepset_cloud_sdk.s3.upload import S3
 
 logger = structlog.get_logger(__name__)
 
 
 class FilesService:
-    """Service for all file related operations."""
+    """Service for all file-related operations."""
 
     def __init__(self, upload_sessions: UploadSessionsAPI, files: FilesAPI, s3: S3):
         """Initialize the service.
 
         :param upload_sessions: API for upload sessions.
         :param files: API for files.
         :param aws: AWS client.
@@ -106,17 +106,17 @@
         file_paths: List[Path],
         write_mode: WriteMode = WriteMode.KEEP,
         blocking: bool = True,
         timeout_s: int = 300,
     ) -> None:
         """Upload a list of files to a workspace.
 
-        Upload a list of files via upload sessions to a selected workspace. If blocking is True, the function waits until
-        all files are uploaded and listed by deepsetCloud. If blocking is False, the function returns immediately after
-        the upload of the files is done. Note: It can take a while until the files are listed in deepsetCloud.
+        Upload a list of files  to a selected workspace using upload sessions. If blocking is True, the function waits until
+        all files are uploaded and listed by deepset Cloud. If blocking is False, the function returns immediately after
+        the upload of the files is done. Note: It can take a while until the files are listed in deepset Cloud.
 
         :param workspace_name: Name of the workspace to upload the files to.
         :file_paths: List of file paths to upload.
         :blocking: If True, blocks until the ingestion is finished.
         :timeout_s: Timeout in seconds for the blocking ingestion.
         :raises TimeoutError: If blocking is True and the ingestion takes longer than timeout_s.
         """
@@ -150,17 +150,17 @@
         folder_path: Path,
         write_mode: WriteMode = WriteMode.KEEP,
         blocking: bool = True,
         timeout_s: int = 300,
     ) -> None:
         """Upload a folder to a workspace.
 
-        Upload a folder via upload sessions to a selected workspace. If blocking is True, the function waits until
-        all files are uploaded and listed by deepsetCloud. If blocking is False, the function returns immediately after
-        the upload of the files is done. Note: It can take a while until the files are listed in deepsetCloud.
+        Upload a folder to a selected workspace using upload sessions. If blocking is True, the function waits until
+        all files are uploaded and listed by deepset Cloud. If blocking is False, the function returns immediately after
+        the upload of the files is done. Note: It can take a while until the files are listed in deepset Cloud.
 
         :param workspace_name: Name of the workspace to upload the files to.
         :folder_path: Path to the folder to upload.
         :blocking: If True, blocks until the ingestion is finished.
         :timeout_s: Timeout in seconds for the blocking ingestion.
         :raises TimeoutError: If blocking is True and the ingestion takes longer than timeout_s.
         """
@@ -193,25 +193,25 @@
         write_mode: WriteMode = WriteMode.KEEP,
         blocking: bool = True,
         timeout_s: int = 300,
     ) -> None:
         """
         Upload a list of raw texts to a workspace.
 
-        Upload a list of raw texts via upload sessions to a selected workspace. This method accepts a list of DeepsetCloudFiles
-        which contain the raw text, file name and optional meta data.
+        Upload a list of raw texts to a selected workspace using upload sessions. This method accepts a list of DeepsetCloudFiles
+        which contain raw text, file name, and optional meta data.
 
-        If blocking is True, the function waits until all files are uploaded and listed by deepsetCloud.
+        If blocking is True, the function waits until all files are uploaded and listed by deepset Cloud.
         If blocking is False, the function returns immediately after the upload of the files is done.
-        Note: It can take a while until the files are listed in deepsetCloud.
+        Note: It can take a while until the files are listed in deepset Cloud.
 
         :param workspace_name: Name of the workspace to upload the files to.
         :dc_files: List of DeepsetCloudFiles to upload.
         :blocking: If True, blocks until the ingestion is finished.
-        :timeout_s: Timeout in seconds for the blocking ingestion.
+        :timeout_s: Timeout in seconds for blocking.
         :raises TimeoutError: If blocking is True and the ingestion takes longer than timeout_s.
         """
         # create session to upload files to
         async with self._create_upload_session(workspace_name=workspace_name, write_mode=write_mode) as upload_session:
             await self._s3.upload_texts(upload_session=upload_session, dc_files=dc_files)
 
         if blocking:
@@ -230,15 +230,15 @@
         odata_filter: Optional[str] = None,
         batch_size: int = 100,
         timeout_s: int = 20,
     ) -> AsyncGenerator[List[File], None]:
         """List all files in a workspace.
 
         Returns an async generator that yields lists of files. The generator is finished when all files are listed.
-        The batch size per number of returned files can be specified with batch_size.
+        You can specfy the batch size per number of returned files with batch_size.
 
         :param workspace_name: Name of the workspace to use.
         :param name: odata_filter by file name.
         :param content: odata_filter by file content.
         :param odata_filter: odata_filter by file meta data.
         :param batch_size: Number of files to return per request.
         :param timeout_s: Timeout in seconds for the listing.
@@ -258,10 +258,12 @@
                 content=content,
                 odata_filter=odata_filter,
                 limit=batch_size,
                 after_file_id=after_file_id,
                 after_value=after_value,
             )
             has_more = response.has_more
+            if not response.data:
+                return
             after_value = response.data[-1].created_at
             after_file_id = response.data[-1].file_id
             yield response.data
```

### Comparing `deepset_cloud_sdk-0.0.6/deepset_cloud_sdk/workflows/async_client/files.py` & `deepset_cloud_sdk-0.0.7/deepset_cloud_sdk/workflows/async_client/files.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # pylint:disable=too-many-arguments
-"""This module contains async functions for uploading files and folders to the Deepset Cloud."""
+"""This module contains async functions for uploading files and folders to deepset Cloud."""
 from pathlib import Path
 from typing import AsyncGenerator, List, Optional
 
+from sniffio import AsyncLibraryNotFoundError
+
 from deepset_cloud_sdk.api.config import (
     API_KEY,
     API_URL,
     DEFAULT_WORKSPACE_NAME,
     CommonConfig,
 )
 from deepset_cloud_sdk.api.files import File
@@ -32,36 +34,40 @@
 
     :param api_key: API key to use for authentication.
     :param api_url: API URL to use for authentication.
     :param workspace_name: Name of the workspace to list the files from.
     :param batch_size: Batch size for the listing.
     :return: List of files.
     """
-    async with FilesService.factory(_get_config(api_key=api_key, api_url=api_url)) as file_service:
-        async for file_batch in file_service.list_all(
-            workspace_name=workspace_name,
-            name=name,
-            content=content,
-            odata_filter=odata_filter,
-            batch_size=batch_size,
-            timeout_s=timeout_s,
-        ):
-            yield file_batch
+    try:
+        async with FilesService.factory(_get_config(api_key=api_key, api_url=api_url)) as file_service:
+            async for file_batch in file_service.list_all(
+                workspace_name=workspace_name,
+                name=name,
+                content=content,
+                odata_filter=odata_filter,
+                batch_size=batch_size,
+                timeout_s=timeout_s,
+            ):
+                yield file_batch
+    except AsyncLibraryNotFoundError:
+        # since we are using asyncio.run() in the sync wrapper, we need to catch this error
+        pass
 
 
 async def upload_file_paths(
     file_paths: List[Path],
     api_key: Optional[str] = None,
     api_url: Optional[str] = None,
     workspace_name: str = DEFAULT_WORKSPACE_NAME,
     write_mode: WriteMode = WriteMode.KEEP,
     blocking: bool = True,
     timeout_s: int = 300,
 ) -> None:
-    """Upload files to the Deepset Cloud.
+    """Upload files to deepset Cloud.
 
     :param file_paths: List of file paths to upload.
     :param api_key: API key to use for authentication.
     :param api_url: API URL to use for authentication.
     :param workspace_name: Name of the workspace to upload the files to.
     :param blocking: Whether to wait for the upload to finish.
     :param timeout_s: Timeout in seconds for the upload.
@@ -81,15 +87,15 @@
     api_key: Optional[str] = None,
     api_url: Optional[str] = None,
     workspace_name: str = DEFAULT_WORKSPACE_NAME,
     write_mode: WriteMode = WriteMode.KEEP,
     blocking: bool = True,
     timeout_s: int = 300,
 ) -> None:
-    """Upload a folder to the Deepset Cloud.
+    """Upload a folder to deepset Cloud.
 
     :param folder_path: Path to the folder to upload.
     :param api_key: API key to use for authentication.
     :param api_url: API URL to use for authentication.
     :param workspace_name: Name of the workspace to upload the files to.
     :param blocking: Whether to wait for the upload to finish.
     :param timeout_s: Timeout in seconds for the upload.
@@ -109,15 +115,15 @@
     api_key: Optional[str] = None,
     api_url: Optional[str] = None,
     workspace_name: str = DEFAULT_WORKSPACE_NAME,
     write_mode: WriteMode = WriteMode.KEEP,
     blocking: bool = True,
     timeout_s: int = 300,
 ) -> None:
-    """Upload texts to the Deepset Cloud.
+    """Upload texts to deepset Cloud.
 
     :param dc_files: List of DeepsetCloudFiles to upload.
     :param api_key: API key to use for authentication.
     :param api_url: API URL to use for authentication.
     :param workspace_name: Name of the workspace to upload the files to.
     :param blocking: Whether to wait for the upload to finish.
     :param timeout_s: Timeout in seconds for the upload.
```

### Comparing `deepset_cloud_sdk-0.0.6/deepset_cloud_sdk/workflows/sync_client/files.py` & `deepset_cloud_sdk-0.0.7/deepset_cloud_sdk/workflows/sync_client/files.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-# pylint: disable=too-many-arguments
 """Sync client for files workflow."""
 import asyncio
 from pathlib import Path
-from typing import List, Optional
+from typing import Generator, List, Optional
+
+import structlog
 
 from deepset_cloud_sdk.api.config import DEFAULT_WORKSPACE_NAME
 from deepset_cloud_sdk.api.files import File
 from deepset_cloud_sdk.api.upload_sessions import WriteMode
 from deepset_cloud_sdk.service.files_service import DeepsetCloudFile
 from deepset_cloud_sdk.workflows.async_client.files import (
     list_files as async_list_files,
@@ -17,25 +18,27 @@
 from deepset_cloud_sdk.workflows.async_client.files import (
     upload_folder as async_upload_folder,
 )
 from deepset_cloud_sdk.workflows.async_client.files import (
     upload_texts as async_upload_texts,
 )
 
+logger = structlog.get_logger(__name__)
+
 
 def upload_file_paths(
     file_paths: List[Path],
     api_key: Optional[str] = None,
     api_url: Optional[str] = None,
     workspace_name: str = DEFAULT_WORKSPACE_NAME,
     write_mode: WriteMode = WriteMode.KEEP,
     blocking: bool = True,
     timeout_s: int = 300,
 ) -> None:
-    """Upload files to the Deepset Cloud.
+    """Upload files to deepset Cloud.
 
     :param file_paths: List of file paths to upload.
     :param api_key: API key to use for authentication.
     :param api_url: API URL to use for authentication.
     :param workspace_name: Name of the workspace to upload the files to.
     :param blocking: Whether to wait for the upload to finish.
     :param timeout_s: Timeout in seconds for the upload.
@@ -58,15 +61,15 @@
     api_key: Optional[str] = None,
     api_url: Optional[str] = None,
     workspace_name: str = DEFAULT_WORKSPACE_NAME,
     write_mode: WriteMode = WriteMode.KEEP,
     blocking: bool = True,
     timeout_s: int = 300,
 ) -> None:
-    """Upload a folder to the Deepset Cloud.
+    """Upload a folder to deepset Cloud.
 
     :param folder_path: Path to the folder to upload.
     :param api_key: API key to use for authentication.
     :param api_url: API URL to use for authentication.
     :param workspace_name: Name of the workspace to upload the files to.
     :param blocking: Whether to wait for the upload to finish.
     :param timeout_s: Timeout in seconds for the upload.
@@ -89,15 +92,15 @@
     api_key: Optional[str] = None,
     api_url: Optional[str] = None,
     workspace_name: str = DEFAULT_WORKSPACE_NAME,
     write_mode: WriteMode = WriteMode.KEEP,
     blocking: bool = True,
     timeout_s: int = 300,
 ) -> None:
-    """Upload texts to the Deepset Cloud.
+    """Upload texts to deepset Cloud.
 
     :param dc_files: List of DeepsetCloudFiles to upload.
     :param api_key: API key to use for authentication.
     :param api_url: API URL to use for authentication.
     :param workspace_name: Name of the workspace to upload the files to.
     :param blocking: Whether to wait for the upload to finish.
     :param timeout_s: Timeout in seconds for the upload.
@@ -120,38 +123,40 @@
     api_url: Optional[str] = None,
     workspace_name: str = DEFAULT_WORKSPACE_NAME,
     name: Optional[str] = None,
     content: Optional[str] = None,
     odata_filter: Optional[str] = None,
     batch_size: int = 100,
     timeout_s: int = 300,
-) -> List[File]:
-    """List files in the Deepset Cloud.
+) -> Generator[List[File], None, None]:
+    """List files in deepset Cloud.
 
-    WARNING: this will only work for workspaces up to 1000 files.
+    WARNING: This only works for workspaces with up to 1000 files.
     TODO: make this a generator
 
     :param api_key: API key to use for authentication.
     :param api_url: API URL to use for authentication.
     :param workspace_name: Name of the workspace to list the files from.
     :param name: Name of the file to odata_filter for.
     :param content: Content of the file to odata_filter for.
     :param odata_filter: odata_filter to apply to the file list.
     :param batch_size: Batch size to use for the file list.
     """
+    loop = asyncio.new_event_loop()
 
-    async def list_files_async() -> List[File]:
-        files: List[File] = []
-        async for file_batch in async_list_files(
-            api_key=api_key,
-            api_url=api_url,
-            workspace_name=workspace_name,
-            name=name,
-            content=content,
-            odata_filter=odata_filter,
-            batch_size=batch_size,
-            timeout_s=timeout_s,
-        ):
-            files += file_batch
-        return files
-
-    return asyncio.run(list_files_async())
+    async_list_files_generator = async_list_files(
+        api_key=api_key,
+        api_url=api_url,
+        workspace_name=workspace_name,
+        name=name,
+        content=content,
+        odata_filter=odata_filter,
+        batch_size=batch_size,
+        timeout_s=timeout_s,
+    )
+    try:
+        while True:
+            yield loop.run_until_complete(async_list_files_generator.__anext__())
+    except StopAsyncIteration:
+        pass
+    finally:
+        loop.close()
```

### Comparing `deepset_cloud_sdk-0.0.6/examples/cli/README.md` & `deepset_cloud_sdk-0.0.7/examples/cli/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,53 +1,68 @@
 # deepset Cloud CLI
-The deepset Cloud CLI is a command-line interface tool that allows you to interact with the deepset Cloud SDK and perform various operations, such as uploading files and folders to your deepset Cloud workspace.
+The deepset Cloud CLI is a command-line interface tool that you can use to interact with the deepset Cloud SDK and perform various operations, such as uploading files and folders to your deepset Cloud workspace.
 
 ## Installation
-To install the deepset Cloud CLI, you can use `pip`:
+To install the deepset Cloud CLI, use `pip`:
 
 ```shell
 pip3 install deepset-cloud-sdk
 ```
 ## Configuration
-Before using the deepset Cloud CLI, you need to log in and provide your credentials. You can do this by running the following command:
+Before using the deepset Cloud CLI, log in and provide your credentials. You can do this by running the command:
 
 ```shell
 deepset-cloud-cli login
 ```
 
-This command will prompt you to enter your API key and default workspace name. Once you provide these details, the CLI will store your credentials securely in the ~/.deepset-cloud-cli/.env file. This file will be used as the default configuration for subsequent CLI commands.
-
-Alternatively, if you want to use a different environment file for your configuration, you can create an `.env` file in the local directory.
-Additionally, you have the flexibility to provide the credentials directly as command-line arguments or set them programmatically in your code, instead of using the environment file. This can be useful in certain scenarios or for automation purposes.
+This command prompts you to enter your API key and default workspace name. Once you provide these details, the CLI stores your credentials in the `~/.deepset-cloud-cli/.env` file. This file is used as the default configuration for subsequent CLI commands.
 
+Alternatively, to use a different environment file for your configuration, you can create an `.env` file in the local directory. Additionally, you have the flexibility to provide the credentials directly as command-line arguments or set them programmatically in your code.
 
 ## Usage
-Once you have installed the deepset Cloud CLI and configured the necessary environment variables, you can run it from the console using the following command:
-
+You can use the deepset Cloud CLI by running the following command:
 ```shell
 deepset-cloud-cli <command>
 ```
-Replace <command> with one of the supported commands. Currently, the supported commands are:
+Replace <command> with one of the supported commands. To list all available commands, run: `deepset-cloud-cli --help`.
 
-upload-folder: Uploads a file or a folder to your deepset Cloud workspace.
-Example Commands
-Here are a couple of example commands that demonstrate how to use the deepset Cloud CLI:
+## Example Commands
 
+### Upload Files and Folders
+Here are a couple of example commands that demonstrate how to use the deepset Cloud CLI:
 ```shell
-deepset-cloud-cli upload-folder ./examples/data/example.txt
+deepset-cloud-cli upload-file-paths ./examples/data/example.txt
 ```
 This command uploads the file example.txt to your deepset Cloud workspace.
 
 ```shell
 deepset-cloud-cli upload-folder "./examples/data"
 ```
 This command uploads the entire data folder, located in the examples directory, to your deepset Cloud workspace.
+Note that the paths provided in the above examples are relative to the current working directory.
+
+If you want to overwrite existing files in your project, you can use the `--write-mode` flag. For example:
+```shell
+deepset-cloud-cli upload-file-paths ./examples/data/example.txt --write-mode OVERWRITE
+```
+This syncs your local files with the files in your deepset Cloud workspace without having to manually delete the files in your workspace.
+
 
-Please note that the paths provided in the above examples are relative to the current working directory.
+### List files
+You can run the `list-files` operation to search files in your deepset Cloud workspace. For example:
+```shell
+deepset-cloud-cli list-files
+```
+with optional arguments:
+```shell
+--name "<your-file-name>"  # search by file name
+--content "content" # search by file content
+--odata-filter "key eq 'value'" # search by odata filter
+```
 
 ### Documentation
-For more information and detailed usage instructions, please refer to the deepset Cloud SDK documentation.
+For more information and detailed usage instructions, see the deepset Cloud SDK documentation.
 
-###Support
-If you encounter any issues or have any questions, please feel free to reach out to our team on [discord](https://discord.com/invite/qZxjM4bAHU).
+### Support
+If you encounter any issues or have any questions, feel free to reach out to our team on [discord](https://discord.com/invite/qZxjM4bAHU).
 
 We hope you find the deepset Cloud CLI useful in your projects. Happy coding!
```

### Comparing `deepset_cloud_sdk-0.0.6/examples/data/example.pdf` & `deepset_cloud_sdk-0.0.7/examples/data/example.pdf`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-0.0.6/examples/sdk/upload.py` & `deepset_cloud_sdk-0.0.7/examples/sdk/upload.py`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-0.0.6/.gitignore` & `deepset_cloud_sdk-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-0.0.6/README.md` & `deepset_cloud_sdk-0.0.7/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -6,34 +6,34 @@
 [![Deploy PyPi](https://github.com/deepset-ai/deepset-cloud-sdk/actions/workflows/deploy-prod.yml/badge.svg)](https://github.com/deepset-ai/deepset-cloud-sdk/actions/workflows/deploy-prod.yml)
 [![Compliance Checks](https://github.com/deepset-ai/deepset-cloud-sdk/actions/workflows/compliance.yml/badge.svg)](https://github.com/deepset-ai/deepset-cloud-sdk/actions/workflows/compliance.yml)
 
 The deepset Cloud SDK is an open source software development kit that provides convenient access and integration with deepset Cloud, a powerful cloud offering for various natural language processing (NLP) tasks.
 This README provides an overview of the SDK and its features, and information on contributing to the project and exploring related resources.
 
 # Supported Features
-The current version of the SDK focuses on providing an easy way to upload files to deepset Cloud for further processing and analysis. For detailed instructions and examples, see file_uploads/README.md.
-
-## Examples
-The following examples demonstrate how to use the deepset Cloud SDK to interact with deepset Cloud.
-- [Upload datasets to deepset Cloud via SDK](/examples/sdk/upload.py)
-- [Upload datasets to deepset Cloud via CLI](/examples/cli/README.md)
-
-## CLI
+The following examples demonstrate how to use the deepset Cloud SDK to interact with deepset Cloud using Python.
 You can use the deepset Cloud SDK in the command line as well. For more information, see the [CLI documentation](/examples/cli/README.md).
+- [SDK - Upload datasets](/examples/sdk/upload.py)
+- [CLI - Upload datasets](/examples/cli/README.md)
 
 ## Installation
-The deepset Cloud SDK is available on PyPI and can be installed using pip:
+The deepset Cloud SDK is available on PyPI and you can install it using pip:
 ```bash
 pip install deepset-cloud-sdk
 ```
 
+### Development Installation
+To install the deepset Cloud SDK for development, clone the repository and install the package in editable mode:
+```bash
+pip install hatch==1.7.0
+hatch build
+```
 
 ## Contributing
-We welcome contributions from the open source community to enhance the deepset Cloud SDK. I
-f you would like to contribute, refer to the [CONTRIBUTING.md](CONTRIBUTING.md) file for guidelines and instructions on how to get started.
+We welcome contributions from the open source community to enhance the deepset Cloud SDK. If you would like to contribute, have a look at [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines and instructions on how to get started.
 We appreciate your contributions, whether they're bug fixes, new features, or documentation improvements.
 
 
 ---
 
 ## Interested in deepset Cloud?
 If you are interested in exploring deepset Cloud, visit cloud.deepset.ai.
```

#### html2text {}

```diff
@@ -7,29 +7,28 @@
 deploy-prod.yml) [![Compliance Checks](https://github.com/deepset-ai/deepset-
 cloud-sdk/actions/workflows/compliance.yml/badge.svg)](https://github.com/
 deepset-ai/deepset-cloud-sdk/actions/workflows/compliance.yml) The deepset
 Cloud SDK is an open source software development kit that provides convenient
 access and integration with deepset Cloud, a powerful cloud offering for
 various natural language processing (NLP) tasks. This README provides an
 overview of the SDK and its features, and information on contributing to the
-project and exploring related resources. # Supported Features The current
-version of the SDK focuses on providing an easy way to upload files to deepset
-Cloud for further processing and analysis. For detailed instructions and
-examples, see file_uploads/README.md. ## Examples The following examples
-demonstrate how to use the deepset Cloud SDK to interact with deepset Cloud. -
-[Upload datasets to deepset Cloud via SDK](/examples/sdk/upload.py) - [Upload
-datasets to deepset Cloud via CLI](/examples/cli/README.md) ## CLI You can use
-the deepset Cloud SDK in the command line as well. For more information, see
-the [CLI documentation](/examples/cli/README.md). ## Installation The deepset
-Cloud SDK is available on PyPI and can be installed using pip: ```bash pip
-install deepset-cloud-sdk ``` ## Contributing We welcome contributions from the
-open source community to enhance the deepset Cloud SDK. I f you would like to
-contribute, refer to the [CONTRIBUTING.md](CONTRIBUTING.md) file for guidelines
-and instructions on how to get started. We appreciate your contributions,
-whether they're bug fixes, new features, or documentation improvements. --- ##
-Interested in deepset Cloud? If you are interested in exploring deepset Cloud,
-visit cloud.deepset.ai. deepset Cloud provides a range of NLP capabilities and
-services to help you build and deploy powerful natural language processing
-applications. ## Interested in Haystack? deepset Cloud is powered by Haystack,
-an open source framework for building end-to-end NLP pipelines. - [Project
-website](https://haystack.deepset.ai/) - [GitHub repository](https://
-github.com/deepset-ai/haystack)
+project and exploring related resources. # Supported Features The following
+examples demonstrate how to use the deepset Cloud SDK to interact with deepset
+Cloud using Python. You can use the deepset Cloud SDK in the command line as
+well. For more information, see the [CLI documentation](/examples/cli/
+README.md). - [SDK - Upload datasets](/examples/sdk/upload.py) - [CLI - Upload
+datasets](/examples/cli/README.md) ## Installation The deepset Cloud SDK is
+available on PyPI and you can install it using pip: ```bash pip install
+deepset-cloud-sdk ``` ### Development Installation To install the deepset Cloud
+SDK for development, clone the repository and install the package in editable
+mode: ```bash pip install hatch==1.7.0 hatch build ``` ## Contributing We
+welcome contributions from the open source community to enhance the deepset
+Cloud SDK. If you would like to contribute, have a look at [CONTRIBUTING.md]
+(CONTRIBUTING.md) for guidelines and instructions on how to get started. We
+appreciate your contributions, whether they're bug fixes, new features, or
+documentation improvements. --- ## Interested in deepset Cloud? If you are
+interested in exploring deepset Cloud, visit cloud.deepset.ai. deepset Cloud
+provides a range of NLP capabilities and services to help you build and deploy
+powerful natural language processing applications. ## Interested in Haystack?
+deepset Cloud is powered by Haystack, an open source framework for building
+end-to-end NLP pipelines. - [Project website](https://haystack.deepset.ai/) -
+[GitHub repository](https://github.com/deepset-ai/haystack)
```

### Comparing `deepset_cloud_sdk-0.0.6/pyproject.toml` & `deepset_cloud_sdk-0.0.7/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 dependencies = [
   "structlog==23.1.0",
   "httpx==0.24.0",
   "python-dotenv==1.0.0",
   "typer==0.9.0",
   "tenacity==8.2.2",
   "aiohttp==3.8.4",
+  "tabulate==0.9.0",
   "progress==1.6"
 ]
 
 [project.urls]
 Documentation = "https://github.com/deepset-ai/deepset-cloud-sdk#readme"
 Issues = "https://github.com/deepset-ai/deepset-cloud-sdk/issues"
 Source = "https://github.com/deepset-ai/deepset-cloud-sdk"
@@ -54,15 +55,15 @@
 
 [tool.hatch.envs.default]
 dependencies = [
   "structlog==23.1.0",
   "httpx==0.24.0",
   "python-dotenv==1.0.0",
   "tenacity==8.2.2",
-  "aiohttp==3.8.4",
+  "aiohttp==3.8.4"
 ]
 
 [tool.hatch.envs.test.scripts]
 unit-with-cov = "pytest --cov-report=term-missing --cov-config=pyproject.toml --cov=deepset_cloud_sdk tests/unit"
 integration = "pytest --cov-report=term-missing --cov-config=pyproject.toml --cov=deepset_cloud_sdk tests/integration"
 
 [tool.hatch.envs.test]
@@ -81,14 +82,15 @@
 dependencies = [
   "pylint==2.15.2",
   "pydocstyle==6.3.0",
   "black==23.3.0",
   "isort==5.12.0",
   "mypy==1.1.1",
   "pre-commit==2.20.0",
+  "types-tabulate==0.9.0.2"
 ]
 
 [tool.hatch.envs.code-quality.scripts]
 types = "mypy deepset_cloud_sdk tests"
 format = "black deepset_cloud_sdk tests --check"
 format-fix = "black deepset_cloud_sdk tests"
 lint = "pylint deepset_cloud_sdk"
@@ -137,15 +139,15 @@
   "fixme",
   "c-extension-no-member",
   "wrong-spelling-in-comment",
   "wrong-spelling-in-docstring",
   "missing-module-docstring"
   ]
 [tool.pylint.'DESIGN']
-max-args=7
+max-args=9
 
 [tool.pylint.'SIMILARITIES']
 min-similarity-lines=6
 
 [tool.pylint.'BASIC']
 good-names=[
   "i",
```

### Comparing `deepset_cloud_sdk-0.0.6/PKG-INFO` & `deepset_cloud_sdk-0.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepset-cloud-sdk
-Version: 0.0.6
+Version: 0.0.7
 Summary: deepset cloud SDK
 Project-URL: Documentation, https://github.com/deepset-ai/deepset-cloud-sdk#readme
 Project-URL: Issues, https://github.com/deepset-ai/deepset-cloud-sdk/issues
 Project-URL: Source, https://github.com/deepset-ai/deepset-cloud-sdk
 Author-email: deepset <rohan.janjua@deepset.ai>
 License-Expression: MIT
 Classifier: Development Status :: 4 - Beta
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
 Requires-Dist: aiohttp==3.8.4
 Requires-Dist: httpx==0.24.0
 Requires-Dist: progress==1.6
 Requires-Dist: python-dotenv==1.0.0
 Requires-Dist: structlog==23.1.0
+Requires-Dist: tabulate==0.9.0
 Requires-Dist: tenacity==8.2.2
 Requires-Dist: typer==0.9.0
 Description-Content-Type: text/markdown
 
 <p align="center">
   <a href="https://cloud.deepset.ai/"><img src="/assets/logo.png"  alt="deepset Cloud SDK"></a>
 </p>
@@ -33,34 +34,34 @@
 [![Deploy PyPi](https://github.com/deepset-ai/deepset-cloud-sdk/actions/workflows/deploy-prod.yml/badge.svg)](https://github.com/deepset-ai/deepset-cloud-sdk/actions/workflows/deploy-prod.yml)
 [![Compliance Checks](https://github.com/deepset-ai/deepset-cloud-sdk/actions/workflows/compliance.yml/badge.svg)](https://github.com/deepset-ai/deepset-cloud-sdk/actions/workflows/compliance.yml)
 
 The deepset Cloud SDK is an open source software development kit that provides convenient access and integration with deepset Cloud, a powerful cloud offering for various natural language processing (NLP) tasks.
 This README provides an overview of the SDK and its features, and information on contributing to the project and exploring related resources.
 
 # Supported Features
-The current version of the SDK focuses on providing an easy way to upload files to deepset Cloud for further processing and analysis. For detailed instructions and examples, see file_uploads/README.md.
-
-## Examples
-The following examples demonstrate how to use the deepset Cloud SDK to interact with deepset Cloud.
-- [Upload datasets to deepset Cloud via SDK](/examples/sdk/upload.py)
-- [Upload datasets to deepset Cloud via CLI](/examples/cli/README.md)
-
-## CLI
+The following examples demonstrate how to use the deepset Cloud SDK to interact with deepset Cloud using Python.
 You can use the deepset Cloud SDK in the command line as well. For more information, see the [CLI documentation](/examples/cli/README.md).
+- [SDK - Upload datasets](/examples/sdk/upload.py)
+- [CLI - Upload datasets](/examples/cli/README.md)
 
 ## Installation
-The deepset Cloud SDK is available on PyPI and can be installed using pip:
+The deepset Cloud SDK is available on PyPI and you can install it using pip:
 ```bash
 pip install deepset-cloud-sdk
 ```
 
+### Development Installation
+To install the deepset Cloud SDK for development, clone the repository and install the package in editable mode:
+```bash
+pip install hatch==1.7.0
+hatch build
+```
 
 ## Contributing
-We welcome contributions from the open source community to enhance the deepset Cloud SDK. I
-f you would like to contribute, refer to the [CONTRIBUTING.md](CONTRIBUTING.md) file for guidelines and instructions on how to get started.
+We welcome contributions from the open source community to enhance the deepset Cloud SDK. If you would like to contribute, have a look at [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines and instructions on how to get started.
 We appreciate your contributions, whether they're bug fixes, new features, or documentation improvements.
 
 
 ---
 
 ## Interested in deepset Cloud?
 If you are interested in exploring deepset Cloud, visit cloud.deepset.ai.
```

#### html2text {}

```diff
@@ -1,51 +1,50 @@
-Metadata-Version: 2.1 Name: deepset-cloud-sdk Version: 0.0.6 Summary: deepset
+Metadata-Version: 2.1 Name: deepset-cloud-sdk Version: 0.0.7 Summary: deepset
 cloud SDK Project-URL: Documentation, https://github.com/deepset-ai/deepset-
 cloud-sdk#readme Project-URL: Issues, https://github.com/deepset-ai/deepset-
 cloud-sdk/issues Project-URL: Source, https://github.com/deepset-ai/deepset-
 cloud-sdk Author-email: deepset
 janjua@deepset.ai> License-Expression: MIT Classifier: Development Status :: 4
 - Beta Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python ::
 Implementation :: CPython Classifier: Programming Language :: Python ::
 Implementation :: PyPy Requires-Python: >=3.8 Requires-Dist: aiohttp==3.8.4
 Requires-Dist: httpx==0.24.0 Requires-Dist: progress==1.6 Requires-Dist:
 python-dotenv==1.0.0 Requires-Dist: structlog==23.1.0 Requires-Dist:
-tenacity==8.2.2 Requires-Dist: typer==0.9.0 Description-Content-Type: text/
-markdown
+tabulate==0.9.0 Requires-Dist: tenacity==8.2.2 Requires-Dist: typer==0.9.0
+Description-Content-Type: text/markdown
                               [deepset_Cloud_SDK]
 [![Tests](https://github.com/deepset-ai/deepset-cloud-sdk/actions/workflows/
 continuous-integration.yml/badge.svg)](https://github.com/deepset-ai/deepset-
 cloud-sdk/actions/workflows/continuous-integration.yml) [![Deploy PyPi](https:/
 /github.com/deepset-ai/deepset-cloud-sdk/actions/workflows/deploy-prod.yml/
 badge.svg)](https://github.com/deepset-ai/deepset-cloud-sdk/actions/workflows/
 deploy-prod.yml) [![Compliance Checks](https://github.com/deepset-ai/deepset-
 cloud-sdk/actions/workflows/compliance.yml/badge.svg)](https://github.com/
 deepset-ai/deepset-cloud-sdk/actions/workflows/compliance.yml) The deepset
 Cloud SDK is an open source software development kit that provides convenient
 access and integration with deepset Cloud, a powerful cloud offering for
 various natural language processing (NLP) tasks. This README provides an
 overview of the SDK and its features, and information on contributing to the
-project and exploring related resources. # Supported Features The current
-version of the SDK focuses on providing an easy way to upload files to deepset
-Cloud for further processing and analysis. For detailed instructions and
-examples, see file_uploads/README.md. ## Examples The following examples
-demonstrate how to use the deepset Cloud SDK to interact with deepset Cloud. -
-[Upload datasets to deepset Cloud via SDK](/examples/sdk/upload.py) - [Upload
-datasets to deepset Cloud via CLI](/examples/cli/README.md) ## CLI You can use
-the deepset Cloud SDK in the command line as well. For more information, see
-the [CLI documentation](/examples/cli/README.md). ## Installation The deepset
-Cloud SDK is available on PyPI and can be installed using pip: ```bash pip
-install deepset-cloud-sdk ``` ## Contributing We welcome contributions from the
-open source community to enhance the deepset Cloud SDK. I f you would like to
-contribute, refer to the [CONTRIBUTING.md](CONTRIBUTING.md) file for guidelines
-and instructions on how to get started. We appreciate your contributions,
-whether they're bug fixes, new features, or documentation improvements. --- ##
-Interested in deepset Cloud? If you are interested in exploring deepset Cloud,
-visit cloud.deepset.ai. deepset Cloud provides a range of NLP capabilities and
-services to help you build and deploy powerful natural language processing
-applications. ## Interested in Haystack? deepset Cloud is powered by Haystack,
-an open source framework for building end-to-end NLP pipelines. - [Project
-website](https://haystack.deepset.ai/) - [GitHub repository](https://
-github.com/deepset-ai/haystack)
+project and exploring related resources. # Supported Features The following
+examples demonstrate how to use the deepset Cloud SDK to interact with deepset
+Cloud using Python. You can use the deepset Cloud SDK in the command line as
+well. For more information, see the [CLI documentation](/examples/cli/
+README.md). - [SDK - Upload datasets](/examples/sdk/upload.py) - [CLI - Upload
+datasets](/examples/cli/README.md) ## Installation The deepset Cloud SDK is
+available on PyPI and you can install it using pip: ```bash pip install
+deepset-cloud-sdk ``` ### Development Installation To install the deepset Cloud
+SDK for development, clone the repository and install the package in editable
+mode: ```bash pip install hatch==1.7.0 hatch build ``` ## Contributing We
+welcome contributions from the open source community to enhance the deepset
+Cloud SDK. If you would like to contribute, have a look at [CONTRIBUTING.md]
+(CONTRIBUTING.md) for guidelines and instructions on how to get started. We
+appreciate your contributions, whether they're bug fixes, new features, or
+documentation improvements. --- ## Interested in deepset Cloud? If you are
+interested in exploring deepset Cloud, visit cloud.deepset.ai. deepset Cloud
+provides a range of NLP capabilities and services to help you build and deploy
+powerful natural language processing applications. ## Interested in Haystack?
+deepset Cloud is powered by Haystack, an open source framework for building
+end-to-end NLP pipelines. - [Project website](https://haystack.deepset.ai/) -
+[GitHub repository](https://github.com/deepset-ai/haystack)
```

