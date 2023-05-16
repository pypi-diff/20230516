# Comparing `tmp/eventsourcing_eventstoredb-0.3.4.tar.gz` & `tmp/eventsourcing_eventstoredb-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eventsourcing_eventstoredb-0.3.4.tar", max compression
+gzip compressed data, was "eventsourcing_eventstoredb-0.4.tar", max compression
```

## Comparing `eventsourcing_eventstoredb-0.3.4.tar` & `eventsourcing_eventstoredb-0.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1520 2023-01-10 14:57:04.745967 eventsourcing_eventstoredb-0.3.4/LICENSE
--rw-r--r--   0        0        0     7379 2023-01-10 14:57:04.746414 eventsourcing_eventstoredb-0.3.4/README.md
--rw-r--r--   0        0        0       76 2023-01-10 14:57:04.746761 eventsourcing_eventstoredb-0.3.4/eventsourcing_eventstoredb/__init__.py
--rw-r--r--   0        0        0     1504 2023-02-14 14:08:11.951274 eventsourcing_eventstoredb-0.3.4/eventsourcing_eventstoredb/factory.py
--rw-r--r--   0        0        0        0 2023-01-10 14:57:04.747064 eventsourcing_eventstoredb-0.3.4/eventsourcing_eventstoredb/py.typed
--rw-r--r--   0        0        0     9437 2023-02-14 14:08:11.951581 eventsourcing_eventstoredb-0.3.4/eventsourcing_eventstoredb/recorders.py
--rw-r--r--   0        0        0     2576 2023-02-14 14:08:11.670336 eventsourcing_eventstoredb-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     8438 1970-01-01 00:00:00.000000 eventsourcing_eventstoredb-0.3.4/setup.py
--rw-r--r--   0        0        0     8651 1970-01-01 00:00:00.000000 eventsourcing_eventstoredb-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1520 2023-01-10 14:57:04.745967 eventsourcing_eventstoredb-0.4/LICENSE
+-rw-r--r--   0        0        0     7215 2023-05-16 19:32:35.713962 eventsourcing_eventstoredb-0.4/README.md
+-rw-r--r--   0        0        0       76 2023-01-10 14:57:04.746761 eventsourcing_eventstoredb-0.4/eventsourcing_eventstoredb/__init__.py
+-rw-r--r--   0        0        0     2082 2023-05-16 19:32:35.714638 eventsourcing_eventstoredb-0.4/eventsourcing_eventstoredb/factory.py
+-rw-r--r--   0        0        0        0 2023-01-10 14:57:04.747064 eventsourcing_eventstoredb-0.4/eventsourcing_eventstoredb/py.typed
+-rw-r--r--   0        0        0     9566 2023-05-16 19:32:35.715203 eventsourcing_eventstoredb-0.4/eventsourcing_eventstoredb/recorders.py
+-rw-r--r--   0        0        0     2574 2023-05-16 19:32:35.716646 eventsourcing_eventstoredb-0.4/pyproject.toml
+-rw-r--r--   0        0        0     8257 1970-01-01 00:00:00.000000 eventsourcing_eventstoredb-0.4/setup.py
+-rw-r--r--   0        0        0     8485 1970-01-01 00:00:00.000000 eventsourcing_eventstoredb-0.4/PKG-INFO
```

### Comparing `eventsourcing_eventstoredb-0.3.4/LICENSE` & `eventsourcing_eventstoredb-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `eventsourcing_eventstoredb-0.3.4/README.md` & `eventsourcing_eventstoredb-0.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -52,30 +52,27 @@
 
     @event('TrickAdded')
     def add_trick(self, trick):
         self.tricks.append(trick)
 ```
 
 Configure the application to use EventStoreDB. Set environment variable
-`PERSISTENCE_MODULE` to `'eventsourcing_eventstoredb'`, and set
-`EVENTSTOREDB_URI` to the host and port of your EventStoreDB.
+`PERSISTENCE_MODULE` to `'eventsourcing_eventstoredb'`. Also set
+`EVENTSTOREDB_URI` to an EventStoreDB connection string URI, and
+`EVENTSTOREDB_ROOT_CERTIFICATES` to the SSL/TLS certificate used
+by the EventStoreDB server(s). Please refer to the
+[esdbclient](https://github.com/pyeventsourcing/esdbclient)
+documentation for more information about these settings.
 
 ```python
 school = TrainingSchool(env={
     'PERSISTENCE_MODULE': 'eventsourcing_eventstoredb',
-    'EVENTSTOREDB_URI': 'localhost:2113',
 })
 ```
 
-*NB: SSL/TLS not yet supported:* In case you are running against a cluster, or want to use SSL/TLS certificates,
-you can specify these things in the URI.
-
-```
-    'EVENTSTOREDB_URI': 'esdb://localhost:2111,localhost:2112,localhost:2113?tls&rootCertificate=./certs/ca/ca.crt'
-```
 
 Call application methods from tests and user interfaces.
 
 ```python
 dog_id = school.register('Fido')
 school.add_trick(dog_id, 'roll over')
 school.add_trick(dog_id, 'play dead')
@@ -86,28 +83,27 @@
 
 To see the events have been saved, we can reconstruct the application
 and get Fido's details again.
 
 ```python
 school = TrainingSchool(env={
     'PERSISTENCE_MODULE': 'eventsourcing_eventstoredb',
-    'EVENTSTOREDB_URI': 'localhost:2113',
 })
 
 dog_details = school.get_dog(dog_id)
 
 assert dog_details['name'] == 'Fido'
 assert dog_details['tricks'] == ['roll over', 'play dead']
 ```
 
 For more information, please refer to the Python
-[eventsourcing](https://github.com/johnbywater/eventsourcing) library
+[eventsourcing](https://github.com/pyeventsourcing/eventsourcing) library
 and the [EventStoreDB](https://www.eventstore.com/) project.
 
-## Developers
+## Contributors
 
 ### Install Poetry
 
 The first thing is to check you have Poetry installed.
 
     $ poetry --version
 
@@ -166,18 +162,17 @@
 
 Use the Makefile to create a new Poetry virtual environment for the
 project and install the project's package dependencies into it,
 using the following command.
 
     $ make install-packages
 
-If you want to skip the installation of your project's package, use the
-`--no-root` option.
+It's also possible to also install the project in 'editable mode'.
 
-    $ make install-packages --no-root
+    $ make install
 
 Please note, if you create the virtual environment in this way, and then try to
 open the project in PyCharm and configure the project to use this virtual
 environment as an "Existing Poetry Environment", PyCharm sometimes has some
 issues (don't know why) which might be problematic. If you encounter such
 issues, you can resolve these issues by deleting the virtual environment
 and creating the Poetry virtual environment using PyCharm (see above).
```

### Comparing `eventsourcing_eventstoredb-0.3.4/eventsourcing_eventstoredb/recorders.py` & `eventsourcing_eventstoredb-0.4/eventsourcing_eventstoredb/recorders.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import json
 import re
 import sys
 from typing import Any, List, Optional, Sequence
 from uuid import UUID
 
 from esdbclient import DEFAULT_EXCLUDE_FILTER, ESDBClient, NewEvent
-from esdbclient.exceptions import ExpectedPositionError, StreamNotFound
+from esdbclient.exceptions import NotFound, WrongExpectedPosition
 from eventsourcing.persistence import (
     AggregateRecorder,
     ApplicationRecorder,
     IntegrityError,
     Notification,
     PersistenceError,
     ProgrammingError,
@@ -83,26 +83,27 @@
                 ).encode("utf8")
             else:
                 metadata = b""
             new_event = NewEvent(
                 type=stored_event.topic,
                 data=stored_event.state,
                 metadata=metadata,
+                content_type="application/octet-stream",
             )
             new_events.append(new_event)
         try:
             if self.for_snapshotting:
                 stream_name = self.create_snapshot_stream_name(stream_name)
                 expected_position = -1  # Disable OCC.
             commit_position = self.client.append_events(
                 stream_name=stream_name,
                 expected_position=expected_position,
                 events=new_events,
             )
-        except ExpectedPositionError as e:
+        except WrongExpectedPosition as e:
             raise IntegrityError(e) from e
         except Exception as e:
             raise PersistenceError(e) from e
         return [commit_position] * len(new_events)  # The best we can do?
 
     def create_snapshot_stream_name(self, stream_name: str) -> str:
         # return str(uuid5(NAMESPACE_OID, f"/snapshots/{stream_name}"))
@@ -157,20 +158,23 @@
                         return []
                     _limit = max(0, current_position - gt)
                     if limit is None:
                         limit = _limit
                     else:
                         limit = min(limit, _limit)
 
-        recorded_events = self.client.read_stream_events(
-            stream_name=stream_name,
-            stream_position=position,
-            backwards=desc,
-            limit=limit if limit is not None else sys.maxsize,
-        )
+        try:
+            recorded_events = self.client.iter_stream_events(
+                stream_name=stream_name,
+                stream_position=position,
+                backwards=desc,
+                limit=limit if limit is not None else sys.maxsize,
+            )
+        except NotFound:
+            return []
 
         stored_events = []
         try:
             for ev in recorded_events:
                 if self.for_snapshotting:
                     originator_version = json.loads(ev.metadata.decode("utf8"))[
                         "originator_version"
@@ -181,15 +185,15 @@
                 se = StoredEvent(
                     originator_id=originator_id,
                     originator_version=originator_version,
                     topic=ev.type,
                     state=ev.data,
                 )
                 stored_events.append(se)
-        except StreamNotFound:
+        except NotFound:
             return []
 
         return stored_events
 
 
 class EventStoreDBApplicationRecorder(
     EventStoreDBAggregateRecorder, ApplicationRecorder
```

### Comparing `eventsourcing_eventstoredb-0.3.4/pyproject.toml` & `eventsourcing_eventstoredb-0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eventsourcing-eventstoredb"
-version = "0.3.4"
+version = "0.4"
 description = "Python package for eventsourcing with EventStoreDB"
 authors = [
     "John Bywater <john.bywater@appropriatesoftware.net>",
 ]
 license = "BSD 3-Clause"
 classifiers = [
     "Development Status :: 3 - Alpha",
@@ -22,15 +22,15 @@
 include = ["eventsourcing_eventstoredb/py.typed"]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 eventsourcing = { version = "~9.2.14" }
 #eventsourcing = { path = "../eventsourcing/", develop = true }
 #esdbclient = { path = "../esdbclient/", develop = true }
-esdbclient = "0.10"
+esdbclient = "0.14"
 
 
 [tool.poetry.dev-dependencies]
 black = { version = "*", allow-prereleases = true }
 flake8 = "*"
 flake8-broken-line = "*"
 flake8-bugbear = "*"
```

### Comparing `eventsourcing_eventstoredb-0.3.4/setup.py` & `eventsourcing_eventstoredb-0.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 packages = \
 ['eventsourcing_eventstoredb']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['esdbclient==0.10', 'eventsourcing>=9.2.14,<9.3.0']
+['esdbclient==0.14', 'eventsourcing>=9.2.14,<9.3.0']
 
 setup_kwargs = {
     'name': 'eventsourcing-eventstoredb',
-    'version': '0.3.4',
+    'version': '0.4',
     'description': 'Python package for eventsourcing with EventStoreDB',
-    'long_description': '# Event Sourcing in Python with EventStoreDB\n\nThis is an extension package for the Python\n[eventsourcing](https://github.com/pyeventsourcing/eventsourcing) library\nthat provides a persistence module for [EventStoreDB](https://www.eventstore.com/).\nIt uses the [esdbclient](https://github.com/pyeventsourcing/esdbclient)\npackage to communicate with EventStoreDB via its gRPC interface.\n\n## Installation\n\nUse pip to install the [stable distribution](https://pypi.org/project/eventsourcing-eventstoredb/)\nfrom the Python Package Index.\n\n    $ pip install eventsourcing-eventstoredb\n\nPlease note, it is recommended to install Python packages into a Python virtual environment.\n\n## Getting started\n\nDefine aggregates and applications in the usual way. Please note, aggregate\nsequences  in EventStoreDB start from position `0`, so set INITIAL_VERSION\non your aggregate classes accordingly.\n\n```python\nfrom eventsourcing.application import Application\nfrom eventsourcing.domain import Aggregate, event\n\n\nclass TrainingSchool(Application):\n    def register(self, name):\n        dog = Dog(name)\n        self.save(dog)\n        return dog.id\n\n    def add_trick(self, dog_id, trick):\n        dog = self.repository.get(dog_id)\n        dog.add_trick(trick)\n        self.save(dog)\n\n    def get_dog(self, dog_id):\n        dog = self.repository.get(dog_id)\n        return {\'name\': dog.name, \'tricks\': list(dog.tricks)}\n\n\nclass Dog(Aggregate):\n    INITIAL_VERSION = 0\n\n    @event(\'Registered\')\n    def __init__(self, name):\n        self.name = name\n        self.tricks = []\n\n    @event(\'TrickAdded\')\n    def add_trick(self, trick):\n        self.tricks.append(trick)\n```\n\nConfigure the application to use EventStoreDB. Set environment variable\n`PERSISTENCE_MODULE` to `\'eventsourcing_eventstoredb\'`, and set\n`EVENTSTOREDB_URI` to the host and port of your EventStoreDB.\n\n```python\nschool = TrainingSchool(env={\n    \'PERSISTENCE_MODULE\': \'eventsourcing_eventstoredb\',\n    \'EVENTSTOREDB_URI\': \'localhost:2113\',\n})\n```\n\n*NB: SSL/TLS not yet supported:* In case you are running against a cluster, or want to use SSL/TLS certificates,\nyou can specify these things in the URI.\n\n```\n    \'EVENTSTOREDB_URI\': \'esdb://localhost:2111,localhost:2112,localhost:2113?tls&rootCertificate=./certs/ca/ca.crt\'\n```\n\nCall application methods from tests and user interfaces.\n\n```python\ndog_id = school.register(\'Fido\')\nschool.add_trick(dog_id, \'roll over\')\nschool.add_trick(dog_id, \'play dead\')\ndog_details = school.get_dog(dog_id)\nassert dog_details[\'name\'] == \'Fido\'\nassert dog_details[\'tricks\'] == [\'roll over\', \'play dead\']\n```\n\nTo see the events have been saved, we can reconstruct the application\nand get Fido\'s details again.\n\n```python\nschool = TrainingSchool(env={\n    \'PERSISTENCE_MODULE\': \'eventsourcing_eventstoredb\',\n    \'EVENTSTOREDB_URI\': \'localhost:2113\',\n})\n\ndog_details = school.get_dog(dog_id)\n\nassert dog_details[\'name\'] == \'Fido\'\nassert dog_details[\'tricks\'] == [\'roll over\', \'play dead\']\n```\n\nFor more information, please refer to the Python\n[eventsourcing](https://github.com/johnbywater/eventsourcing) library\nand the [EventStoreDB](https://www.eventstore.com/) project.\n\n## Developers\n\n### Install Poetry\n\nThe first thing is to check you have Poetry installed.\n\n    $ poetry --version\n\nIf you don\'t, then please [install Poetry](https://python-poetry.org/docs/#installing-with-the-official-installer).\n\nIt will help to make sure Poetry\'s bin directory is in your `PATH` environment variable.\n\nBut in any case, make sure you know the path to the `poetry` executable. The Poetry\ninstaller tells you where it has been installed, and how to configure your shell.\n\nPlease refer to the [Poetry docs](https://python-poetry.org/docs/) for guidance on\nusing Poetry.\n\n### Setup for PyCharm users\n\nYou can easily obtain the project files using PyCharm (menu "Git > Clone...").\nPyCharm will then usually prompt you to open the project.\n\nOpen the project in a new window. PyCharm will then usually prompt you to create\na new virtual environment.\n\nCreate a new Poetry virtual environment for the project. If PyCharm doesn\'t already\nknow where your `poetry` executable is, then set the path to your `poetry` executable\nin the "New Poetry Environment" form input field labelled "Poetry executable". In the\n"New Poetry Environment" form, you will also have the opportunity to select which\nPython executable will be used by the virtual environment.\n\nPyCharm will then create a new Poetry virtual environment for your project, using\na particular version of Python, and also install into this virtual environment the\nproject\'s package dependencies according to the `pyproject.toml` file, or the\n`poetry.lock` file if that exists in the project files.\n\nYou can add different Poetry environments for different Python versions, and switch\nbetween them using the "Python Interpreter" settings of PyCharm. If you want to use\na version of Python that isn\'t installed, either use your favourite package manager,\nor install Python by downloading an installer for recent versions of Python directly\nfrom the [Python website](https://www.python.org/downloads/).\n\nOnce project dependencies have been installed, you should be able to run tests\nfrom within PyCharm (right-click on the `tests` folder and select the \'Run\' option).\n\nBecause of a conflict between pytest and PyCharm\'s debugger and the coverage tool,\nyou may need to add ``--no-cov`` as an option to the test runner template. Alternatively,\njust use the Python Standard Library\'s ``unittest`` module.\n\nYou should also be able to open a terminal window in PyCharm, and run the project\'s\nMakefile commands from the command line (see below).\n\n### Setup from command line\n\nObtain the project files, using Git or suitable alternative.\n\nIn a terminal application, change your current working directory\nto the root folder of the project files. There should be a Makefile\nin this folder.\n\nUse the Makefile to create a new Poetry virtual environment for the\nproject and install the project\'s package dependencies into it,\nusing the following command.\n\n    $ make install-packages\n\nIf you want to skip the installation of your project\'s package, use the\n`--no-root` option.\n\n    $ make install-packages --no-root\n\nPlease note, if you create the virtual environment in this way, and then try to\nopen the project in PyCharm and configure the project to use this virtual\nenvironment as an "Existing Poetry Environment", PyCharm sometimes has some\nissues (don\'t know why) which might be problematic. If you encounter such\nissues, you can resolve these issues by deleting the virtual environment\nand creating the Poetry virtual environment using PyCharm (see above).\n\n### Project Makefile commands\n\nYou can start EventStoreDB using the following command.\n\n    $ make start-eventstoredb\n\nYou can run tests using the following command (needs EventStoreDB to be running).\n\n    $ make test\n\nYou can stop EventStoreDB using the following command.\n\n    $ make stop-eventstoredb\n\nYou can check the formatting of the code using the following command.\n\n    $ make lint\n\nYou can reformat the code using the following command.\n\n    $ make fmt\n\nTests belong in `./tests`. Code-under-test belongs in `./eventsourcing_eventstoredb`.\n\nEdit package dependencies in `pyproject.toml`. Update installed packages (and the\n`poetry.lock` file) using the following command.\n\n    $ make update-packages\n',
+    'long_description': '# Event Sourcing in Python with EventStoreDB\n\nThis is an extension package for the Python\n[eventsourcing](https://github.com/pyeventsourcing/eventsourcing) library\nthat provides a persistence module for [EventStoreDB](https://www.eventstore.com/).\nIt uses the [esdbclient](https://github.com/pyeventsourcing/esdbclient)\npackage to communicate with EventStoreDB via its gRPC interface.\n\n## Installation\n\nUse pip to install the [stable distribution](https://pypi.org/project/eventsourcing-eventstoredb/)\nfrom the Python Package Index.\n\n    $ pip install eventsourcing-eventstoredb\n\nPlease note, it is recommended to install Python packages into a Python virtual environment.\n\n## Getting started\n\nDefine aggregates and applications in the usual way. Please note, aggregate\nsequences  in EventStoreDB start from position `0`, so set INITIAL_VERSION\non your aggregate classes accordingly.\n\n```python\nfrom eventsourcing.application import Application\nfrom eventsourcing.domain import Aggregate, event\n\n\nclass TrainingSchool(Application):\n    def register(self, name):\n        dog = Dog(name)\n        self.save(dog)\n        return dog.id\n\n    def add_trick(self, dog_id, trick):\n        dog = self.repository.get(dog_id)\n        dog.add_trick(trick)\n        self.save(dog)\n\n    def get_dog(self, dog_id):\n        dog = self.repository.get(dog_id)\n        return {\'name\': dog.name, \'tricks\': list(dog.tricks)}\n\n\nclass Dog(Aggregate):\n    INITIAL_VERSION = 0\n\n    @event(\'Registered\')\n    def __init__(self, name):\n        self.name = name\n        self.tricks = []\n\n    @event(\'TrickAdded\')\n    def add_trick(self, trick):\n        self.tricks.append(trick)\n```\n\nConfigure the application to use EventStoreDB. Set environment variable\n`PERSISTENCE_MODULE` to `\'eventsourcing_eventstoredb\'`. Also set\n`EVENTSTOREDB_URI` to an EventStoreDB connection string URI, and\n`EVENTSTOREDB_ROOT_CERTIFICATES` to the SSL/TLS certificate used\nby the EventStoreDB server(s). Please refer to the\n[esdbclient](https://github.com/pyeventsourcing/esdbclient)\ndocumentation for more information about these settings.\n\n```python\nschool = TrainingSchool(env={\n    \'PERSISTENCE_MODULE\': \'eventsourcing_eventstoredb\',\n})\n```\n\n\nCall application methods from tests and user interfaces.\n\n```python\ndog_id = school.register(\'Fido\')\nschool.add_trick(dog_id, \'roll over\')\nschool.add_trick(dog_id, \'play dead\')\ndog_details = school.get_dog(dog_id)\nassert dog_details[\'name\'] == \'Fido\'\nassert dog_details[\'tricks\'] == [\'roll over\', \'play dead\']\n```\n\nTo see the events have been saved, we can reconstruct the application\nand get Fido\'s details again.\n\n```python\nschool = TrainingSchool(env={\n    \'PERSISTENCE_MODULE\': \'eventsourcing_eventstoredb\',\n})\n\ndog_details = school.get_dog(dog_id)\n\nassert dog_details[\'name\'] == \'Fido\'\nassert dog_details[\'tricks\'] == [\'roll over\', \'play dead\']\n```\n\nFor more information, please refer to the Python\n[eventsourcing](https://github.com/pyeventsourcing/eventsourcing) library\nand the [EventStoreDB](https://www.eventstore.com/) project.\n\n## Contributors\n\n### Install Poetry\n\nThe first thing is to check you have Poetry installed.\n\n    $ poetry --version\n\nIf you don\'t, then please [install Poetry](https://python-poetry.org/docs/#installing-with-the-official-installer).\n\nIt will help to make sure Poetry\'s bin directory is in your `PATH` environment variable.\n\nBut in any case, make sure you know the path to the `poetry` executable. The Poetry\ninstaller tells you where it has been installed, and how to configure your shell.\n\nPlease refer to the [Poetry docs](https://python-poetry.org/docs/) for guidance on\nusing Poetry.\n\n### Setup for PyCharm users\n\nYou can easily obtain the project files using PyCharm (menu "Git > Clone...").\nPyCharm will then usually prompt you to open the project.\n\nOpen the project in a new window. PyCharm will then usually prompt you to create\na new virtual environment.\n\nCreate a new Poetry virtual environment for the project. If PyCharm doesn\'t already\nknow where your `poetry` executable is, then set the path to your `poetry` executable\nin the "New Poetry Environment" form input field labelled "Poetry executable". In the\n"New Poetry Environment" form, you will also have the opportunity to select which\nPython executable will be used by the virtual environment.\n\nPyCharm will then create a new Poetry virtual environment for your project, using\na particular version of Python, and also install into this virtual environment the\nproject\'s package dependencies according to the `pyproject.toml` file, or the\n`poetry.lock` file if that exists in the project files.\n\nYou can add different Poetry environments for different Python versions, and switch\nbetween them using the "Python Interpreter" settings of PyCharm. If you want to use\na version of Python that isn\'t installed, either use your favourite package manager,\nor install Python by downloading an installer for recent versions of Python directly\nfrom the [Python website](https://www.python.org/downloads/).\n\nOnce project dependencies have been installed, you should be able to run tests\nfrom within PyCharm (right-click on the `tests` folder and select the \'Run\' option).\n\nBecause of a conflict between pytest and PyCharm\'s debugger and the coverage tool,\nyou may need to add ``--no-cov`` as an option to the test runner template. Alternatively,\njust use the Python Standard Library\'s ``unittest`` module.\n\nYou should also be able to open a terminal window in PyCharm, and run the project\'s\nMakefile commands from the command line (see below).\n\n### Setup from command line\n\nObtain the project files, using Git or suitable alternative.\n\nIn a terminal application, change your current working directory\nto the root folder of the project files. There should be a Makefile\nin this folder.\n\nUse the Makefile to create a new Poetry virtual environment for the\nproject and install the project\'s package dependencies into it,\nusing the following command.\n\n    $ make install-packages\n\nIt\'s also possible to also install the project in \'editable mode\'.\n\n    $ make install\n\nPlease note, if you create the virtual environment in this way, and then try to\nopen the project in PyCharm and configure the project to use this virtual\nenvironment as an "Existing Poetry Environment", PyCharm sometimes has some\nissues (don\'t know why) which might be problematic. If you encounter such\nissues, you can resolve these issues by deleting the virtual environment\nand creating the Poetry virtual environment using PyCharm (see above).\n\n### Project Makefile commands\n\nYou can start EventStoreDB using the following command.\n\n    $ make start-eventstoredb\n\nYou can run tests using the following command (needs EventStoreDB to be running).\n\n    $ make test\n\nYou can stop EventStoreDB using the following command.\n\n    $ make stop-eventstoredb\n\nYou can check the formatting of the code using the following command.\n\n    $ make lint\n\nYou can reformat the code using the following command.\n\n    $ make fmt\n\nTests belong in `./tests`. Code-under-test belongs in `./eventsourcing_eventstoredb`.\n\nEdit package dependencies in `pyproject.toml`. Update installed packages (and the\n`poetry.lock` file) using the following command.\n\n    $ make update-packages\n',
     'author': 'John Bywater',
     'author_email': 'john.bywater@appropriatesoftware.net',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/pyeventsourcing/eventsourcing-eventstoredb',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `eventsourcing_eventstoredb-0.3.4/PKG-INFO` & `eventsourcing_eventstoredb-0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eventsourcing-eventstoredb
-Version: 0.3.4
+Version: 0.4
 Summary: Python package for eventsourcing with EventStoreDB
 Home-page: https://github.com/pyeventsourcing/eventsourcing-eventstoredb
 License: BSD 3-Clause
 Author: John Bywater
 Author-email: john.bywater@appropriatesoftware.net
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: esdbclient (==0.10)
+Requires-Dist: esdbclient (==0.14)
 Requires-Dist: eventsourcing (>=9.2.14,<9.3.0)
 Project-URL: Repository, https://github.com/pyeventsourcing/eventsourcing-eventstoredb
 Description-Content-Type: text/markdown
 
 # Event Sourcing in Python with EventStoreDB
 
 This is an extension package for the Python
@@ -81,30 +81,27 @@
 
     @event('TrickAdded')
     def add_trick(self, trick):
         self.tricks.append(trick)
 ```
 
 Configure the application to use EventStoreDB. Set environment variable
-`PERSISTENCE_MODULE` to `'eventsourcing_eventstoredb'`, and set
-`EVENTSTOREDB_URI` to the host and port of your EventStoreDB.
+`PERSISTENCE_MODULE` to `'eventsourcing_eventstoredb'`. Also set
+`EVENTSTOREDB_URI` to an EventStoreDB connection string URI, and
+`EVENTSTOREDB_ROOT_CERTIFICATES` to the SSL/TLS certificate used
+by the EventStoreDB server(s). Please refer to the
+[esdbclient](https://github.com/pyeventsourcing/esdbclient)
+documentation for more information about these settings.
 
 ```python
 school = TrainingSchool(env={
     'PERSISTENCE_MODULE': 'eventsourcing_eventstoredb',
-    'EVENTSTOREDB_URI': 'localhost:2113',
 })
 ```
 
-*NB: SSL/TLS not yet supported:* In case you are running against a cluster, or want to use SSL/TLS certificates,
-you can specify these things in the URI.
-
-```
-    'EVENTSTOREDB_URI': 'esdb://localhost:2111,localhost:2112,localhost:2113?tls&rootCertificate=./certs/ca/ca.crt'
-```
 
 Call application methods from tests and user interfaces.
 
 ```python
 dog_id = school.register('Fido')
 school.add_trick(dog_id, 'roll over')
 school.add_trick(dog_id, 'play dead')
@@ -115,28 +112,27 @@
 
 To see the events have been saved, we can reconstruct the application
 and get Fido's details again.
 
 ```python
 school = TrainingSchool(env={
     'PERSISTENCE_MODULE': 'eventsourcing_eventstoredb',
-    'EVENTSTOREDB_URI': 'localhost:2113',
 })
 
 dog_details = school.get_dog(dog_id)
 
 assert dog_details['name'] == 'Fido'
 assert dog_details['tricks'] == ['roll over', 'play dead']
 ```
 
 For more information, please refer to the Python
-[eventsourcing](https://github.com/johnbywater/eventsourcing) library
+[eventsourcing](https://github.com/pyeventsourcing/eventsourcing) library
 and the [EventStoreDB](https://www.eventstore.com/) project.
 
-## Developers
+## Contributors
 
 ### Install Poetry
 
 The first thing is to check you have Poetry installed.
 
     $ poetry --version
 
@@ -195,18 +191,17 @@
 
 Use the Makefile to create a new Poetry virtual environment for the
 project and install the project's package dependencies into it,
 using the following command.
 
     $ make install-packages
 
-If you want to skip the installation of your project's package, use the
-`--no-root` option.
+It's also possible to also install the project in 'editable mode'.
 
-    $ make install-packages --no-root
+    $ make install
 
 Please note, if you create the virtual environment in this way, and then try to
 open the project in PyCharm and configure the project to use this virtual
 environment as an "Existing Poetry Environment", PyCharm sometimes has some
 issues (don't know why) which might be problematic. If you encounter such
 issues, you can resolve these issues by deleting the virtual environment
 and creating the Poetry virtual environment using PyCharm (see above).
```

