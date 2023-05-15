# Comparing `tmp/channels_yroom-0.0.4.tar.gz` & `tmp/channels_yroom-0.0.5.tar.gz`

## Comparing `channels_yroom-0.0.4.tar` & `channels_yroom-0.0.5.tar`

### file list

```diff
@@ -1,68 +1,70 @@
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/.dockerignore
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/.readthedocs.yaml
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/CHANGELOG.md
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/Dockerfile
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/docker-compose.yml
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/mkdocs.yml
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/.github/workflows/release.yml
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/.github/workflows/test.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/channels_yroom/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/channels_yroom/__init__.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/channels_yroom/admin.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/channels_yroom/apps.py
--rw-r--r--   0        0        0     8280 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/channels_yroom/channel.py
--rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/channels_yroom/conf.py
--rw-r--r--   0        0        0     3651 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/channels_yroom/consumer.py
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/channels_yroom/models.py
--rw-r--r--   0        0        0     4820 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/channels_yroom/proxy.py
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/channels_yroom/storage.py
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/channels_yroom/utils.py
--rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/channels_yroom/worker.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/channels_yroom/management/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/channels_yroom/management/commands/__init__.py
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/channels_yroom/management/commands/yroom.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/channels_yroom/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/channels_yroom/migrations/__init__.py
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/docs/api.md
--rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/docs/explanation.md
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/docs/index.md
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/docs/requirements.in
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/docs/requirements.txt
--rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/docs/settings.md
--rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/docs/tutorial.md
--rw-r--r--   0        0        0     2124 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/docs/howto/tiptap.md
--rwxr-xr-x   0        0        0      674 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/example/manage.py
--rw-r--r--   0        0        0    75131 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/example/package-lock.json
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/example/package.json
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/example/requirements.txt
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/example/vite.config.js
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/example/frontend/main.js
--rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/example/frontend/prosemirror.js
--rw-r--r--   0        0        0     6466 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/example/frontend/schema.js
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/example/frontend/style.css
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/example/textcollab/__init__.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/example/textcollab/admin.py
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/example/textcollab/apps.py
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/example/textcollab/consumers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/example/textcollab/models.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/example/textcollab/routing.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/example/textcollab/tests.py
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/example/textcollab/urls.py
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/example/textcollab/views.py
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/example/textcollab/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/example/textcollab/migrations/__init__.py
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/example/textcollab/templates/textcollab/index.html
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/example/textcollab/templates/textcollab/room.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/example/textcollab_project/__init__.py
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/example/textcollab_project/asgi.py
--rw-r--r--   0        0        0     5206 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/example/textcollab_project/settings.py
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/example/textcollab_project/urls.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/example/textcollab_project/wsgi.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/tests/__init__.py
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/tests/conftest.py
--rw-r--r--   0        0        0    13605 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/tests/test_consumer.py
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/.gitignore
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/LICENSE
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/README.md
--rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/.dockerignore
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/.readthedocs.yaml
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/CHANGELOG.md
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/Dockerfile
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/docker-compose.yml
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/mkdocs.yml
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/.github/workflows/release.yml
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/.github/workflows/test.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/channels_yroom/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/channels_yroom/__init__.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/channels_yroom/admin.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/channels_yroom/apps.py
+-rw-r--r--   0        0        0     8646 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/channels_yroom/channel.py
+-rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/channels_yroom/conf.py
+-rw-r--r--   0        0        0     3490 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/channels_yroom/consumer.py
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/channels_yroom/models.py
+-rw-r--r--   0        0        0     4820 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/channels_yroom/proxy.py
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/channels_yroom/storage.py
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/channels_yroom/utils.py
+-rw-r--r--   0        0        0     3268 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/channels_yroom/worker.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/channels_yroom/management/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/channels_yroom/management/commands/__init__.py
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/channels_yroom/management/commands/yroom.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/channels_yroom/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/channels_yroom/migrations/__init__.py
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/docs/api.md
+-rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/docs/explanation.md
+-rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/docs/index.md
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/docs/requirements.in
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/docs/requirements.txt
+-rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/docs/settings.md
+-rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/docs/tutorial.md
+-rw-r--r--   0        0        0     2384 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/docs/howto/tiptap.md
+-rwxr-xr-x   0        0        0      674 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/example/manage.py
+-rw-r--r--   0        0        0   174304 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/example/package-lock.json
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/example/package.json
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/example/requirements.txt
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/example/vite.config.js
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/example/frontend/main.js
+-rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/example/frontend/prosemirror.js
+-rw-r--r--   0        0        0     6466 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/example/frontend/schema.js
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/example/frontend/style.css
+-rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/example/frontend/tiptap.js
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/example/textcollab/__init__.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/example/textcollab/admin.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/example/textcollab/apps.py
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/example/textcollab/consumers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/example/textcollab/models.py
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/example/textcollab/routing.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/example/textcollab/tests.py
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/example/textcollab/urls.py
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/example/textcollab/views.py
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/example/textcollab/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/example/textcollab/migrations/__init__.py
+-rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/example/textcollab/templates/textcollab/index.html
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/example/textcollab/templates/textcollab/room.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/example/textcollab_project/__init__.py
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/example/textcollab_project/asgi.py
+-rw-r--r--   0        0        0     5400 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/example/textcollab_project/settings.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/example/textcollab_project/urls.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/example/textcollab_project/wsgi.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/tests/__init__.py
+-rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/tests/conftest.py
+-rw-r--r--   0        0        0    11246 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/tests/test_consumer.py
+-rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/tests/test_worker.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/LICENSE
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/README.md
+-rw-r--r--   0        0        0     2270 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/PKG-INFO
```

### Comparing `channels_yroom-0.0.4/Dockerfile` & `channels_yroom-0.0.5/Dockerfile`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.4/docker-compose.yml` & `channels_yroom-0.0.5/docker-compose.yml`

 * *Files 12% similar despite different names*

```diff
@@ -2,27 +2,29 @@
 
 x-app-defaults:
   &app_defaults
   build: .
   init: true
   links:
     - broker
+    - db
   environment:
     - REDIS_HOST=broker
+    - DJANGO_DEBUG=0
   depends_on:
     - broker
+    - db
 
 services:
   db:
     image: postgres:15
     volumes:
       - postgres_data:/var/lib/postgresql/data/
     environment:
       - "POSTGRES_HOST_AUTH_METHOD=trust"
-      - "DJANGO_DEBUG=0"
   broker:
     image: redis:5
     volumes:
       - "redis-data:/data"
   app:
     <<: *app_defaults
     command: "uvicorn --host 0.0.0.0 textcollab_project.asgi:application"
```

### Comparing `channels_yroom-0.0.4/mkdocs.yml` & `channels_yroom-0.0.5/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.4/.github/workflows/release.yml` & `channels_yroom-0.0.5/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.4/.github/workflows/test.yml` & `channels_yroom-0.0.5/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.4/channels_yroom/channel.py` & `channels_yroom-0.0.5/channels_yroom/channel.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,19 +4,15 @@
 from typing import Optional
 
 from channels.consumer import AsyncConsumer
 from yroom import YRoomManager, YRoomMessage
 
 from .conf import get_room_prefix, get_room_settings, get_settings
 from .storage import YDocStorage, get_ydoc_storage
-from .utils import (
-    YroomChannelMessage,
-    YroomChannelRPCMessage,
-    get_connection_group_name,
-)
+from .utils import YroomChannelMessage, YroomChannelRPCMessage
 
 logger = logging.getLogger(__name__)
 
 
 class YRoomChannelConsumer(AsyncConsumer):
     def __init__(self) -> None:
         self.room_manager: YRoomManager = YRoomManager(get_settings())
@@ -44,15 +40,17 @@
         if not self.room_manager.has_room(room_name):
             result = await self.create_room_from_snapshot(room_name, conn_id)
         if result is None:
             logger.debug(
                 "yroom connect, room present or no snapshot %s %s", room_name, conn_id
             )
             result = self.room_manager.connect(room_name, conn_id)
-        await self.respond(conn_id, room_name, result)
+        await self.respond(
+            result, room_name=room_name, channel_name=message["channel_name"]
+        )
 
     async def create_room_from_snapshot(
         self, room_name: str, conn_id: int = 0
     ) -> Optional[YRoomMessage]:
         logger.debug("yroom connect, no room yet %s %s", room_name, conn_id)
         storage = self.get_storage(room_name)
         logger.debug("Using yroom storage %s of %s", storage, self.storages)
@@ -61,19 +59,24 @@
         if snapshot:
             logger.debug("yroom connect, snapshot found %s %s", room_name, snapshot)
             return self.room_manager.connect_with_data(room_name, conn_id, snapshot)
 
     async def message(self, message: YroomChannelMessage) -> None:
         room_name = message["room"]
         conn_id = message["conn_id"]
+        channel_name = message["channel_name"]
         logger.debug("yroom consumer message %s %s: %s", room_name, conn_id, message)
+        # If room not present (and connect is lost/expired?), try restore first
+        if not self.room_manager.has_room(room_name):
+            # Ignore result, connect is kind of optional
+            await self.create_room_from_snapshot(room_name, conn_id)
         result = self.room_manager.handle_message(
             room_name, conn_id, message["payload"]
         )
-        await self.respond(conn_id, room_name, result)
+        await self.respond(result, room_name=room_name, channel_name=channel_name)
 
     @asynccontextmanager
     async def try_room(self, room_name: str) -> None:
         try:
             has_room = True
             if not self.room_manager.has_room(room_name):
                 has_room = False
@@ -113,33 +116,37 @@
             message["channel"],
             {
                 "type": "rpc_response",
                 "result": result,
             },
         )
 
-    async def respond(self, conn_id: int, room_name: str, result: YRoomMessage) -> None:
+    async def respond(
+        self,
+        result: YRoomMessage,
+        room_name: str,
+        channel_name: Optional[str] = None,
+    ) -> None:
         logger.debug(
-            "yroom response in room %s at conection %s (client: %s, broadcast: %s)",
+            "yroom response in room %s at channel %s (client: %s, broadcast: %s)",
             room_name,
-            conn_id,
-            result.payload,
-            result.broadcast_payload,
-        )
-        if result.payload:
-            conn_group_name = get_connection_group_name(conn_id)
-            await self.send_response(conn_group_name, result.payload)
-        if result.broadcast_payload:
-            await self.send_response(room_name, result.broadcast_payload)
-
-    async def send_response(self, group_name: str, payload: bytes) -> None:
-        await self.channel_layer.group_send(
-            group_name,
-            {"type": "forward_payload", "payload": payload},
+            channel_name,
+            result.payloads,
+            result.broadcast_payloads,
         )
+        if result.payloads and channel_name:
+            await self.channel_layer.send(
+                channel_name,
+                {"type": "forward_payload", "payloads": result.payloads},
+            )
+        if result.broadcast_payloads:
+            await self.channel_layer.group_send(
+                room_name,
+                {"type": "forward_payload", "payloads": result.broadcast_payloads},
+            )
 
     async def disconnect(self, message: YroomChannelMessage) -> None:
         await self.disconnect_client(message["room"], conn_id=message["conn_id"])
 
     async def disconnect_client(
         self, room_name: str, conn_id: int = 0, send_response: bool = True
     ) -> None:
@@ -148,15 +155,15 @@
             return
         logger.debug("yroom consumer disconnect %s %s", room_name, conn_id)
         result = self.room_manager.disconnect(room_name, conn_id)
         if not self.room_manager.is_room_alive(room_name):
             logger.debug("Room %s is empty", room_name)
             await self.schedule_room_removal(room_name)
         if send_response:
-            await self.respond(conn_id, room_name, result)
+            await self.respond(result, room_name=room_name, channel_name=None)
 
     async def schedule_room_removal(self, room_name: str):
         if room_name in self.cleanup_tasks:
             self.cleanup_tasks[room_name].cancel()
 
         task = asyncio.create_task(self.remove_room_soon(room_name))
         self.cleanup_tasks[room_name] = task
```

### Comparing `channels_yroom-0.0.4/channels_yroom/conf.py` & `channels_yroom-0.0.5/channels_yroom/conf.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from django.conf import settings
-from django.core.exceptions import ImproperlyConfigured
 
 DEFAULT_ROOM = "default"
 PREFIX_SEPARATOR = "."
 DEFAULTS = {
     "CHANNEL_NAME": "yroom",
     "REMOVE_ROOM_DELAY": 30,  # in seconds
     "STORAGE_BACKEND": "channels_yroom.storage.YDocDatabaseStorage",
@@ -35,8 +34,8 @@
     prefix = get_room_prefix(room_name)
     yroom_settings = get_settings()
     if prefix in yroom_settings:
         return yroom_settings[prefix]
     try:
         return yroom_settings[DEFAULT_ROOM]
     except KeyError:
-        raise ImproperlyConfigured("YROOM_SETTINGS must contain a 'default' key.")
+        return DEFAULTS.copy()
```

### Comparing `channels_yroom-0.0.4/channels_yroom/consumer.py` & `channels_yroom-0.0.5/channels_yroom/consumer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,15 @@
 import logging
 import random
 from typing import Optional
 
 from channels.generic.websocket import AsyncWebsocketConsumer
 
 from .conf import get_room_settings
-from .utils import (
-    YroomChannelMessage,
-    YroomChannelMessageType,
-    YroomChannelResponse,
-    get_connection_group_name,
-)
+from .utils import YroomChannelMessage, YroomChannelMessageType, YroomChannelResponse
 
 logger = logging.getLogger(__name__)
 
 
 class YroomConsumer(AsyncWebsocketConsumer):
     room_name = "yroom_default"
 
@@ -45,43 +40,41 @@
     async def join_room(self) -> None:
         # Join room group
         self.room_name = self.get_room_name()
         self.conn_id = self.get_connection_id()
 
         logger.debug("joining room %s as %s", self.room_name, self.conn_id)
         await self.channel_layer.group_add(self.room_name, self.channel_name)
-        conn_group_name = get_connection_group_name(self.conn_id)
-        await self.channel_layer.group_add(conn_group_name, self.channel_name)
         await self.accept()
         self.room_settings = get_room_settings(self.room_name)
         await self.channel_layer.send(
             self.room_settings["CHANNEL_NAME"],
             YroomChannelMessage(
                 type=YroomChannelMessageType.connect.value,
                 room=self.room_name,
                 conn_id=self.conn_id,
+                channel_name=self.channel_name,
             ),
         )
 
     async def disconnect(self, close_code) -> None:
         await self.leave_room()
 
     async def leave_room(self) -> None:
         # Leave room group
         logger.debug("leaving room %s as %s", self.room_name, self.conn_id)
         await self.channel_layer.group_discard(self.room_name, self.channel_name)
-        conn_group_name = get_connection_group_name(self.conn_id)
-        await self.channel_layer.group_discard(conn_group_name, self.channel_name)
         # Tell yroom worker that client disconnected
         await self.channel_layer.send(
             self.room_settings["CHANNEL_NAME"],
             YroomChannelMessage(
                 type=YroomChannelMessageType.disconnect.value,
                 room=self.room_name,
                 conn_id=self.conn_id,
+                channel_name=self.channel_name,
             ),
         )
 
     async def receive(
         self, text_data: Optional[str] = None, bytes_data: Optional[bytes] = None
     ) -> None:
         # Receive message from WebSocket
@@ -91,13 +84,15 @@
     async def handle_room_message(self, bytes_data: bytes) -> None:
         await self.channel_layer.send(
             self.room_settings["CHANNEL_NAME"],
             YroomChannelMessage(
                 type=YroomChannelMessageType.message.value,
                 room=self.room_name,
                 conn_id=self.conn_id,
+                channel_name=self.channel_name,
                 payload=bytes_data,
             ),
         )
 
     async def forward_payload(self, message: YroomChannelResponse) -> None:
-        await self.send(bytes_data=message["payload"])
+        for payload in message["payloads"]:
+            await self.send(bytes_data=payload)
```

### Comparing `channels_yroom-0.0.4/channels_yroom/models.py` & `channels_yroom-0.0.5/channels_yroom/models.py`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.4/channels_yroom/proxy.py` & `channels_yroom-0.0.5/channels_yroom/proxy.py`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.4/channels_yroom/storage.py` & `channels_yroom-0.0.5/channels_yroom/storage.py`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.4/channels_yroom/utils.py` & `channels_yroom-0.0.5/channels_yroom/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from enum import Enum
 from typing import Any, List, Optional, TypedDict
 
 
 class YroomChannelResponse(TypedDict):
     type: str
-    payload: bytes
+    payloads: List[bytes]
 
 
 class YroomChannelMessageType(str, Enum):
     connect = "connect"
     disconnect = "disconnect"
     message = "message"
     rpc = "rpc"
 
 
 class _YroomChannelMessage(TypedDict):  # implicitly total=True
     type: YroomChannelMessageType
     room: str
     conn_id: int
+    channel_name: str
 
 
 class YroomChannelMessage(_YroomChannelMessage, total=False):
     payload: bytes
 
 
 class YroomChannelRPCMessage(TypedDict):
@@ -31,11 +32,7 @@
     method: str
     params: List[Any]
 
 
 class YroomChannelRPCResponse(TypedDict):
     type: str
     result: Optional[str]
-
-
-def get_connection_group_name(conn_id) -> str:
-    return "yroom-connection_%s" % conn_id
```

### Comparing `channels_yroom-0.0.4/channels_yroom/worker.py` & `channels_yroom-0.0.5/channels_yroom/worker.py`

 * *Files 18% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     def __init__(self, channel, channel_layer, application=None):
         self.channel = channel
         self.channel_layer = channel_layer
         if application is None:
             self.application = get_default_application()
         else:
             self.application = application
+        self.shutting_down = False
 
     def run(self):
         """
         Runs the asyncio event loop with our handler loop.
         """
         loop = asyncio.get_event_loop()
         self._setup_signal_handlers(loop)
@@ -56,24 +57,30 @@
                 send=self.receive_from_worker,
             ),
         )
         # The consumer is also listening on a channel layer
         # but only on a new random channel
         # so we listen on the given channel and forward messages
         while True:
+            if self.shutting_down:
+                # Stop relaying messages when shutting down
+                break
             message = await self.channel_layer.receive(self.channel)
             if not message.get("type", None):
                 raise ValueError("Worker received message with no type.")
             # Run the message into the app
             await self.input_queue.put(message)
 
     async def shutdown_worker(self, signal, loop):
         """
         Shuts down worker gracefully.
         """
+        if self.shutting_down:
+            return
+        self.shutting_down = True
         self._clear_signal_handlers(loop)
         logger.info(f"Received signal {signal.name}...")
         shutdown_message = {"type": "shutdown", "signal": signal.name}
         self.shutdown_event = asyncio.Event()
         logger.info("Sending shutdown message to worker...")
         await self.input_queue.put(shutdown_message)
         logger.info("Waiting on cleanup...")
```

### Comparing `channels_yroom-0.0.4/channels_yroom/management/commands/yroom.py` & `channels_yroom-0.0.5/channels_yroom/management/commands/yroom.py`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.4/channels_yroom/migrations/0001_initial.py` & `channels_yroom-0.0.5/channels_yroom/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.4/docs/explanation.md` & `channels_yroom-0.0.5/docs/explanation.md`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.4/docs/index.md` & `channels_yroom-0.0.5/docs/index.md`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.4/docs/requirements.txt` & `channels_yroom-0.0.5/docs/requirements.txt`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.4/docs/settings.md` & `channels_yroom-0.0.5/docs/settings.md`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.4/docs/tutorial.md` & `channels_yroom-0.0.5/docs/tutorial.md`

 * *Files 14% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 Set up your WebSocket consumer in your app `consumers.py`.
 
 ```python
 from channels_yroom.consumer import YroomConsumer
 
 class TextCollaborationConsumer(YroomConsumer):
-    def get_room_group_name(self) -> str:
+    def get_room_name(self) -> str:
         """
         Determine a unique name for this room, e.g. based on URL
         """
         room_name = self.scope["url_route"]["kwargs"]["room_name"]
         return "textcollab.%s" % room_name
 
     async def connect(self) -> None:
@@ -58,14 +58,35 @@
                 "yroom": YRoomChannelConsumer.as_asgi(),
             }
         ),
     }
 )
 ```
 
+### Use a channel layer for inter-process communication
+
+**Warning: The In-Memory Channel Layer will not work with `channels-yroom`!**
+
+Because the `yroom` communication runs through a worker process, we need inter-process communication.
+Configure the official Redis Channel Layer in your settings:
+
+```python
+CHANNEL_LAYERS = {
+    "default": {
+        "BACKEND": "channels_redis.core.RedisChannelLayer",
+        "CONFIG": {
+            "hosts": [("127.0.0.1", 6379)],
+        },
+    },
+}
+```
+
+Make sure to have a Redis server running.
+
+
 ### Run yroom worker process
 
 In addition to your webserver with WebSockets support (e.g. daphne or uvicorn), you need to run a [channels worker](https://channels.readthedocs.io/en/stable/topics/worker.html). You can run the `yroom` worker implementation that supports graceful shutdown:
 
 ```sh
 python manage.py yroom
-```
+```
```

### Comparing `channels_yroom-0.0.4/docs/howto/tiptap.md` & `channels_yroom-0.0.5/docs/howto/tiptap.md`

 * *Files 24% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import { HocuspocusProvider } from '@hocuspocus/provider';
 import Collaboration from '@tiptap/extension-collaboration';
 import StarterKit from '@tiptap/starter-kit';
 import { Editor } from '@tiptap/vue-3';
 
 import * as Y from 'yjs';
 
-const wsUrl = `ws${window.location.protocol === 'https:' ? 's' : ''}://${window.location.host}/ws/text-editor-collab/1`
+const wsUrl = `ws${window.location.protocol === 'https:' ? 's' : ''}://${window.location.host}/ws/tiptap/test`
 const ydoc = new Y.Doc()
 const documentName = 'text'
 
 const provider = new HocuspocusProvider({
     url: wsUrl,
     name: documentName,
     document: ydoc,
@@ -38,47 +38,51 @@
 
 Your `consumers.py` could look like this:
 
 ```python
 from channels_yroom.consumer import YroomConsumer
 
 
-def get_room_name(room_name: str) -> str:
-    # The room prefix is 'tiptap-editor'
-    return "tiptap-editor.%s" % room_name
+def get_tiptap_room_name(room_name: str) -> str:
+    # The room prefix is 'textcollab_tiptap.'
+    return "textcollab_tiptap.%s" % room_name
 
 
-class TextEditorCollabConsumer(YroomConsumer):
+class TipTapConsumer(YroomConsumer):
     def get_room_name(self) -> str:
-        room_name = str(self.scope["url_route"]["kwargs"]["pk"])
-        return get_room_name(room_name)
+        room_name = self.scope["url_route"]["kwargs"]["room_name"]
+        return get_tiptap_room_name(room_name)
+
 ```
 
 Your `settings.py` should contain the following:
 
 ```python
 YROOM_ROOM_SETTINGS = {
     "tiptap-editor": {
         # HocuspocusProvider adds and expects a name prefix
-        "name_prefixed": True,
+        "PROTOCOL_NAME_PREFIX": True,
         # Since the server doesn't know the name on connect,
         # it has to wait for communication from client
-        "server_sync_first": False,
+        "SERVER_START_SYNC": False,
+        # HocuspocusProvider can only read one message per WS frame
+        "PROTOCOL_DISABLE_PIPELINING": True,
     }
 }
 ```
 
 To complete this example, here is the `routing.py`
 
 ```python
 from django.urls import re_path
 
 from . import consumers
 
 ws_urlpatterns = [
     re_path(
-        r"ws/text-editor-collab/(?P<pk>\d+)$",
-        consumers.TextEditorCollabConsumer.as_asgi(),
+        r"ws/tiptap/(?P<room_name>\w+)$",
+        consumers.TipTapConsumer.as_asgi()
     ),
 ]
 ```
 
+A full [Django Tiptap example can be found in the example directory of the repository](https://github.com/stefanw/channels-yroom/tree/main/example).
```

### Comparing `channels_yroom-0.0.4/example/manage.py` & `channels_yroom-0.0.5/example/manage.py`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.4/example/frontend/prosemirror.js` & `channels_yroom-0.0.5/example/frontend/prosemirror.js`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.4/example/frontend/schema.js` & `channels_yroom-0.0.5/example/frontend/schema.js`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.4/example/textcollab/views.py` & `channels_yroom-0.0.5/example/textcollab/views.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,42 @@
 from typing import Optional
 
 from django.http import HttpResponse
 from django.shortcuts import render
 
-from channels_yroom.proxy import YroomDocument
+from channels_yroom.proxy import DataUnavailable, YroomDocument
 
-from .consumers import get_room_name
+from .consumers import get_prosemirror_room_name, get_tiptap_room_name
 
 
 def index(request):
     return render(request, "textcollab/index.html")
 
 
-def room(request, room_name):
-    return render(request, "textcollab/room.html", {"room_name": room_name})
+def room(request, room_name, editor="prosemirror"):
+    return render(
+        request,
+        "textcollab/room.html",
+        {
+            "room_settings": {
+                "roomName": room_name,
+                "editor": editor,
+                "wsPath": f"/ws/{editor}/",
+            }
+        },
+    )
 
 
-YDOC_XML_FRAGMENT_KEY = "prosemirror"
-
-
-async def save_room(request, room_name):
+async def save_room(request, room_name, editor="prosemirror"):
     # Get the XML fragment from the server ydoc
-    room_group_name = get_room_name(room_name)
+    if editor == "prosemirror":
+        room_group_name = get_prosemirror_room_name(room_name)
+        YDOC_XML_FRAGMENT_KEY = "prosemirror"
+    elif editor == "tiptap":
+        room_group_name = get_tiptap_room_name(room_name)
+        YDOC_XML_FRAGMENT_KEY = "default"
     doc = YroomDocument(room_group_name)
-    result: Optional[str] = await doc.export_xml_fragment(YDOC_XML_FRAGMENT_KEY)
-    if result is None:
+    try:
+        result: Optional[str] = await doc.export_xml_fragment(YDOC_XML_FRAGMENT_KEY)
+    except DataUnavailable:
         return HttpResponse(status=404)
     return HttpResponse(result)
```

### Comparing `channels_yroom-0.0.4/example/textcollab/migrations/0001_initial.py` & `channels_yroom-0.0.5/example/textcollab/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.4/example/textcollab/templates/textcollab/index.html` & `channels_yroom-0.0.5/example/textcollab/templates/textcollab/index.html`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,43 @@
 <!DOCTYPE html>
 <html>
 <head>
     <meta charset="utf-8"/>
     <title>Text Collaboration Rooms</title>
 </head>
 <body>
-    What text collaboration room would you like to enter?<br>
+    <p>What Prosemirror text collaboration room would you like to enter?</p>
     <input id="room-name-input" type="text" size="100"><br>
     <input id="room-name-submit" type="button" value="Enter">
 
+    <hr/>
+    What TipTap text collaboration room would you like to enter?<br>
+    <input id="room-name-input-tiptap" type="text" size="100"><br>
+    <input id="room-name-submit-tiptap" type="button" value="Enter">
+
+
     <script>
         document.querySelector('#room-name-input').focus();
         document.querySelector('#room-name-input').onkeyup = function(e) {
             if (e.keyCode === 13) {  // enter, return
                 document.querySelector('#room-name-submit').click();
             }
         };
 
         document.querySelector('#room-name-submit').onclick = function(e) {
             var roomName = document.querySelector('#room-name-input').value;
-            window.location.pathname = '/' + roomName + '/';
+            window.location.pathname = '/prosemirror/' + roomName + '/';
+        };
+
+        document.querySelector('#room-name-input-tiptap').onkeyup = function(e) {
+            if (e.keyCode === 13) {  // enter, return
+                document.querySelector('#room-name-submit-tiptap').click();
+            }
+        };
+
+        document.querySelector('#room-name-submit-tiptap').onclick = function(e) {
+            var roomName = document.querySelector('#room-name-input-tiptap').value;
+            window.location.pathname = '/tiptap/' + roomName + '/';
         };
     </script>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,4 +1,9 @@
-What text collaboration room would you like to enter?
+What Prosemirror text collaboration room would you like to enter?
+[
+]
+[Unknown INPUT type]
+===============================================================================
+What TipTap text collaboration room would you like to enter?
 [
 ]
 [Unknown INPUT type]
```

### Comparing `channels_yroom-0.0.4/example/textcollab_project/asgi.py` & `channels_yroom-0.0.5/example/textcollab_project/asgi.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -10,22 +10,22 @@
 import os
 
 from django.core.asgi import get_asgi_application
 
 os.environ.setdefault("DJANGO_SETTINGS_MODULE", "textcollab_project.settings")
 django_asgi_app = get_asgi_application()
 
+
+import textcollab.routing
 from channels.auth import AuthMiddlewareStack
 from channels.routing import ChannelNameRouter, ProtocolTypeRouter, URLRouter
 from channels.security.websocket import AllowedHostsOriginValidator
 
-import textcollab.routing
 from channels_yroom.channel import YRoomChannelConsumer
 
-
 application = ProtocolTypeRouter(
     {
         "http": django_asgi_app,
         "websocket": AllowedHostsOriginValidator(
             AuthMiddlewareStack(URLRouter(textcollab.routing.websocket_urlpatterns))
         ),
         "channel": ChannelNameRouter(
```

### Comparing `channels_yroom-0.0.4/example/textcollab_project/settings.py` & `channels_yroom-0.0.5/example/textcollab_project/settings.py`

 * *Files 5% similar despite different names*

```diff
@@ -189,7 +189,16 @@
         "django.db.backends": {
             "level": "ERROR",
             "handlers": ["console"],
             "propagate": False,
         },
     },
 }
+
+YROOM_SETTINGS = {
+    "default": {},
+    "textcollab_tiptap": {
+        "SERVER_START_SYNC": False,
+        "PROTOCOL_NAME_PREFIX": True,
+        "PROTOCOL_DISABLE_PIPELINING": True,
+    },
+}
```

### Comparing `channels_yroom-0.0.4/example/textcollab_project/urls.py` & `channels_yroom-0.0.5/example/textcollab_project/urls.py`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.4/LICENSE` & `channels_yroom-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.4/pyproject.toml` & `channels_yroom-0.0.5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,15 @@
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
   "Django >= 3.2",
   "channels >= 4.0",
-  "yroom >= 0.0.6",
+  "yroom >= 0.0.8",
 ]
 dynamic = ["version"]
 
 [project.urls]
 Documentation = "https://github.com/stefanw/channels-yroom#readme"
 Issues = "https://github.com/stefanw/channels-yroom/issues"
 Source = "https://github.com/stefanw/channels-yroom"
@@ -50,14 +50,15 @@
   "pytest",
   "y-py",
 ]
 
 [tool.hatch.envs.test.scripts]
 test = "pytest --cov-report=term-missing --cov-config=pyproject.toml --cov=channels_yroom --cov=tests {args}"
 no-cov = "test --no-cov {args}"
+covhtml = "coverage html"
 
 [[tool.hatch.envs.test.matrix]]
 python = ["3.8", "3.9", "3.10", "3.11"]
 
 [tool.hatch.envs.docs]
 skip-install = true
 detached = true
```

### Comparing `channels_yroom-0.0.4/PKG-INFO` & `channels_yroom-0.0.5/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: channels-yroom
-Version: 0.0.4
+Version: 0.0.5
 Summary: Yjs sync protocol server for Django channels
 Project-URL: Documentation, https://github.com/stefanw/channels-yroom#readme
 Project-URL: Issues, https://github.com/stefanw/channels-yroom/issues
 Project-URL: Source, https://github.com/stefanw/channels-yroom
 Author-email: Stefan Wehrmeyer <mail@stefanwehrmeyer.com>
 License-Expression: MIT
 License-File: LICENSE
@@ -15,23 +15,44 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
 Requires-Dist: channels>=4.0
 Requires-Dist: django>=3.2
-Requires-Dist: yroom>=0.0.6
+Requires-Dist: yroom>=0.0.8
 Description-Content-Type: text/markdown
 
 # Channels-Yroom
 
 ![PyPI](https://img.shields.io/pypi/v/channels-yroom)
 
 `channels-yroom` is a Django Channels WebSocket consumer and worker for synchronizing Yjs clients. It implements the network protocol for Yjs doc synchronization and awareness updates and makes them available as Django Channels WebSocket consumer and worker.
 
 ## Documentation
 
 [Read the documentation](https://channels-yroom.readthedocs.io/en/latest/)
 
+## Showcase: text collaboration example
+
+The `example` folder contains a simple project that uses `y-prosemirror` to allow for realtime collaboration on rich text.
+
+Run the included Docker compose file to check it out:
+
+```sh
+docker compose up
+# Then visit localhost:8000
+```
+
+## Development
+
+Project uses `hatch` for the development workflow:
+
+```
+pip install hatch
+
+hatch run +py=3.10 test:test
+```
+
 ## License
 
 MIT
```

