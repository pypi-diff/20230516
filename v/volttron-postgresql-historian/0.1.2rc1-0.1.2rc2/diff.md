# Comparing `tmp/volttron_postgresql_historian-0.1.2rc1.tar.gz` & `tmp/volttron_postgresql_historian-0.1.2rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volttron_postgresql_historian-0.1.2rc1.tar", max compression
+gzip compressed data, was "volttron_postgresql_historian-0.1.2rc2.tar", max compression
```

## Comparing `volttron_postgresql_historian-0.1.2rc1.tar` & `volttron_postgresql_historian-0.1.2rc2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11928 2023-05-12 20:47:21.648528 volttron_postgresql_historian-0.1.2rc1/LICENSE
--rwxr-xr-x   0        0        0     9154 2023-05-12 20:47:21.648528 volttron_postgresql_historian-0.1.2rc1/README.md
--rw-r--r--   0        0        0     1374 2023-05-12 20:48:49.686171 volttron_postgresql_historian-0.1.2rc1/pyproject.toml
--rw-r--r--   0        0        0     1082 2023-05-12 20:47:21.648528 volttron_postgresql_historian-0.1.2rc1/src/historian/postgresql/__init__.py
--rw-r--r--   0        0        0    18297 2023-05-12 20:47:21.648528 volttron_postgresql_historian-0.1.2rc1/src/historian/postgresql/postgresqlfuncts.py
--rw-r--r--   0        0        0    10470 1970-01-01 00:00:00.000000 volttron_postgresql_historian-0.1.2rc1/setup.py
--rw-r--r--   0        0        0     9977 1970-01-01 00:00:00.000000 volttron_postgresql_historian-0.1.2rc1/PKG-INFO
+-rw-r--r--   0        0        0    11928 2023-05-16 16:11:20.319883 volttron_postgresql_historian-0.1.2rc2/LICENSE
+-rwxr-xr-x   0        0        0     9043 2023-05-16 16:11:20.319883 volttron_postgresql_historian-0.1.2rc2/README.md
+-rw-r--r--   0        0        0     1374 2023-05-16 16:12:47.290533 volttron_postgresql_historian-0.1.2rc2/pyproject.toml
+-rw-r--r--   0        0        0     1082 2023-05-16 16:11:20.319883 volttron_postgresql_historian-0.1.2rc2/src/historian/postgresql/__init__.py
+-rw-r--r--   0        0        0    18297 2023-05-16 16:11:20.319883 volttron_postgresql_historian-0.1.2rc2/src/historian/postgresql/postgresqlfuncts.py
+-rw-r--r--   0        0        0    10358 1970-01-01 00:00:00.000000 volttron_postgresql_historian-0.1.2rc2/setup.py
+-rw-r--r--   0        0        0     9866 1970-01-01 00:00:00.000000 volttron_postgresql_historian-0.1.2rc2/PKG-INFO
```

### Comparing `volttron_postgresql_historian-0.1.2rc1/LICENSE` & `volttron_postgresql_historian-0.1.2rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `volttron_postgresql_historian-0.1.2rc1/README.md` & `volttron_postgresql_historian-0.1.2rc2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 [![Eclipse VOLTTRON™](https://img.shields.io/badge/Eclips%20VOLTTRON--red.svg)](https://volttron.readthedocs.io/en/latest/)
 ![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)
 ![Python 3.11](https://img.shields.io/badge/python-3.11-blue.svg)
-[![Run Pytests](https://github.com/eclipse-volttron/volttron-postgresql-historian/actions/workflows/run-test.yml/badge.svg)](https://github.com/eclipse-volttron/volttron-postgresql-historian/actions/workflows/run-test.yml)
+[![Run Pytests](https://github.com/eclipse-volttron/volttron-postgresql-historian/actions/workflows/run-tests.yml/badge.svg)](https://github.com/eclipse-volttron/volttron-postgresql-historian/actions/workflows/run-tests.yml)
 [![pypi version](https://img.shields.io/pypi/v/volttron-postgresql-historian.svg)](https://pypi.org/project/volttron-postgresql-historian/)
-![Passing?](https://github.com/VOLTTRON/volttron-postgresql-historian/actions/workflows/run-tests.yml/badge.svg)
 
 VOLTTRON historian agent that stores data into a PostgreSQL database
 
 ### Installation notes
 
 1.  The PostgreSQL database driver supports recent PostgreSQL versions.
     It was tested on 10.x, but should work with 9.x and 11.x.
```

### Comparing `volttron_postgresql_historian-0.1.2rc1/pyproject.toml` & `volttron_postgresql_historian-0.1.2rc2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "volttron-postgresql-historian"
-version = "0.1.2rc1"
+version = "0.1.2rc2"
 description = "VOLTTRON historian agent that stores data in a PostgreSQL database. It extends the SQLHistorian class."
 authors = ["VOLTTRON Team <volttron@pnnl.gov>"]
 license = "Apache License 2.0"
 readme = "README.md"
 repository = "https://github.com/eclipse-volttron/volttron-postgresql-historian"
 homepage = "https://github.com/eclipse-volttron/volttron-postgresql-historian"
 keywords = []
```

### Comparing `volttron_postgresql_historian-0.1.2rc1/src/historian/postgresql/__init__.py` & `volttron_postgresql_historian-0.1.2rc2/src/historian/postgresql/__init__.py`

 * *Files identical despite different names*

### Comparing `volttron_postgresql_historian-0.1.2rc1/src/historian/postgresql/postgresqlfuncts.py` & `volttron_postgresql_historian-0.1.2rc2/src/historian/postgresql/postgresqlfuncts.py`

 * *Files identical despite different names*

### Comparing `volttron_postgresql_historian-0.1.2rc1/setup.py` & `volttron_postgresql_historian-0.1.2rc2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 
 entry_points = \
 {'console_scripts': ['volttron-postgresql-historian = '
                      'historian.sql.historian:main']}
 
 setup_kwargs = {
     'name': 'volttron-postgresql-historian',
-    'version': '0.1.2rc1',
+    'version': '0.1.2rc2',
     'description': 'VOLTTRON historian agent that stores data in a PostgreSQL database. It extends the SQLHistorian class.',
-    'long_description': '[![Eclipse VOLTTRON™](https://img.shields.io/badge/Eclips%20VOLTTRON--red.svg)](https://volttron.readthedocs.io/en/latest/)\n![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)\n![Python 3.11](https://img.shields.io/badge/python-3.11-blue.svg)\n[![Run Pytests](https://github.com/eclipse-volttron/volttron-postgresql-historian/actions/workflows/run-test.yml/badge.svg)](https://github.com/eclipse-volttron/volttron-postgresql-historian/actions/workflows/run-test.yml)\n[![pypi version](https://img.shields.io/pypi/v/volttron-postgresql-historian.svg)](https://pypi.org/project/volttron-postgresql-historian/)\n![Passing?](https://github.com/VOLTTRON/volttron-postgresql-historian/actions/workflows/run-tests.yml/badge.svg)\n\nVOLTTRON historian agent that stores data into a PostgreSQL database\n\n### Installation notes\n\n1.  The PostgreSQL database driver supports recent PostgreSQL versions.\n    It was tested on 10.x, but should work with 9.x and 11.x.\n2.  The user must have SELECT, INSERT, and UPDATE privileges on\n    historian tables.\n3.  The tables in the database are created as part of the execution of\n    the SQLHistorianAgent, but this will fail if the database user does\n    not have CREATE privileges.\n4.  Care must be exercised when using multiple historians with the same\n    database. This configuration may be used only if there is no overlap\n    in the topics handled by each instance. Otherwise, duplicate topic\n    IDs may be created, producing strange results.\n\n\n### Configuration\n\nPostgreSQL historian supports two configuration parameters\n    \n   - connection -  This is a mandatory parameter with type indicating the type of sql historian (i.e. postgresql) and params containing the database access details\n   - tables_def - Optional parameter to provide custom table names for topics, data, and metadata.\n    \nThe configuration can be in a json or yaml formatted file. The following examples show minimal connection \nconfigurations for a psycopg2-based historian. Other options are available and are [documented here](https://www.psycopg.org/docs/module.html#psycopg2.connect) \n**Not all parameters have been tested,  use at your own risk**.\n\n#### Local PostgreSQL Database\n\nThe following snippet demonstrates how to configure the historian to use a PostgreSQL database on the local system that\nis configured to use Unix domain sockets. The user executing volttron must have appropriate privileges.\n\n\n##### Yaml Format:\n```yaml\n    connection:\n          # type should be postgresql\n          type: postgresql\n          params:\n            # Relative to the agents data directory\n            dbname: "volttron"\n        \n    tables_def:\n        # prefix for data, topics, and (in version < 4.0.0 metadata tables)\n        # default is ""\n        table_prefix: ""\n        # table name for time series data. default "data"\n        data_table: data\n        # table name for list of topics. default "topics"\n        topics_table: topics\n ```\n\n##### JSON format:\n```json\n    {\n        "connection": {\n            "type": "postgresql", \n            "params": { "dbname": "volttron" }\n        }\n    }\n```\n\n#### Remote PostgreSQL Database\n\nThe following snippet demonstrates how to configure the historian to use a remote PostgreSQL database.\n```json\n    {\n        "connection": {\n            "type": "postgresql", \n            "params": { \n                "dbname": "volttron", \n                "host": "historian.example.com", \n                "port": 5432, \n                "user": "volttron", \n                "password": "secret" }\n        }\n    }\n```\n\n#### TimescaleDB Support\n\nBoth of the above PostgreSQL connection types can make use of TimescaleDB\\\'s high performance Hypertable backend for \nthe primary timeseries table. The agent assumes you have completed the TimescaleDB installation and setup the \ndatabase by following the instructions here: <https://docs.timescale.com/latest/getting-started/setup> To use, simply\nadd \\\'timescale_dialect: true\\\' to the connection params in the agent config as below\n\n```json\n    {\n        "connection": {\n            "type": "postgresql", \n            "params": { \n                "dbname": "volttron", \n                "host": "historian.example.com", \n                "port": 5432, \n                "user": "volttron", \n                "password": "secret" ,\n                "timescale_dialect": true }\n        }\n\n    }\n```\n\n## Requirements\n\n - Python >= 3.10\n - psycopg2 library\n\n## Installation\n\n1. Create and activate a virtual environment.\n\n   ```shell\n    python -m venv env\n    source env/bin/activate\n    ```\n\n2. Installing volttron-postgresql-historian requires a running volttron instance and the psycopg2 library \n\n    ```shell\n    pip install volttron\n    pip install psycopg2-binary\n    \n    # Start platform with output going to volttron.log\n    volttron -vv -l volttron.log &\n    ```\n3. Setup database\n   \n   If this is not a development environment we highly recommend that you create the database and database tables using\n   a user with appropriate permissions. This way the database user used by the historian need not have CREATE privileges\n   Postgres historian expects two tables \n   a. A topics tables that stores the list of unique topics and its metadata. The default name is "topics". If you use \n      a different name please specify it as part of "tables_def" configuration parameter in agent config. See [example configuration](#yaml-format)\n   b. A data table that stores the timeseries data and refers to the topic table using a topic id. The default name is \n      "data". If you use a different name please specify it as part of "tables_def" configuration parameter in \n      agent config. See [example configuration](#yaml-format)\n\n   Below are the sql statements to create database and tables\n   <u>Create Database</u>\n    ```\n       CREATE DATABASE volttron\n    ```\n   <u>TOPICS tables:</u>\n    ```\n        CREATE TABLE IF NOT EXISTS topics (\n            topic_id SERIAL PRIMARY KEY NOT NULL, \n            topic_name VARCHAR(512) NOT NULL, \n            metadata TEXT, \n            UNIQUE (topic_name)\n       )\n    ```\n    <u>DATA table:</u>\n    ```\n       CREATE TABLE IF NOT EXISTS data (\n           ts TIMESTAMP NOT NULL, \n           topic_id INTEGER NOT NULL, \n           value_string TEXT NOT NULL, \n           UNIQUE (topic_id, ts)\n       )\n    ```\n     <u>Optional timescale hypertable</u>\n    ```\n       SELECT create_hypertable(data, \'ts\', if_not_exists => true)\n    ```\n     <u>Create index to speed up data access</u>\n       If using hypertables:\n    ```\n        CREATE INDEX IF NOT EXISTS idx_data ON data (topic_id, ts)\n    ```\n      If not using hypertables:\n    ```\n        CREATE INDEX IF NOT EXISTS idx_data ON data (ts ASC)\n    ```\n    <u>Provide correct user permissions for database user to be used by historian agent</u>\n    ```\n        CREATE USER <some username> with encrypted password <some password>\n        GRANT SELECT, INSERT, UPDATE on database <historian db name> to <username used above>\n    ``` \n    **NOTE**\n    For development environments, you can create a test database and test user, grant all privileges on that test \n    database to the test user and let the historian create tables and indexes at startup. We do not recommend this for \n    production environments\n\n4. Create an agent configuration file \n\n    Create an agent configuration with appropriate connection parameters as described in the [Configurations section](#Configuration)\n\n5. Install and start the volttron-postgresql-historian.\n\n    ```shell\n    vctl install volttron-postgresql-historian --agent-config <path to configuration> --start\n    ```\n\n6. View the status of the installed agent\n\n    ```shell\n    vctl status\n    ```\n\n## Development\n\nPlease see the following for contributing guidelines [contributing](https://github.com/eclipse-volttron/volttron-core/blob/develop/CONTRIBUTING.md).\n\nPlease see the following helpful guide about [developing modular VOLTTRON agents](https://github.com/eclipse-volttron/volttron-core/blob/develop/DEVELOPING_ON_MODULAR.md)\n\n# Disclaimer Notice\n\nThis material was prepared as an account of work sponsored by an agency of the\nUnited States Government.  Neither the United States Government nor the United\nStates Department of Energy, nor Battelle, nor any of their employees, nor any\njurisdiction or organization that has cooperated in the development of these\nmaterials, makes any warranty, express or implied, or assumes any legal\nliability or responsibility for the accuracy, completeness, or usefulness or any\ninformation, apparatus, product, software, or process disclosed, or represents\nthat its use would not infringe privately owned rights.\n\nReference herein to any specific commercial product, process, or service by\ntrade name, trademark, manufacturer, or otherwise does not necessarily\nconstitute or imply its endorsement, recommendation, or favoring by the United\nStates Government or any agency thereof, or Battelle Memorial Institute. The\nviews and opinions of authors expressed herein do not necessarily state or\nreflect those of the United States Government or any agency thereof.\n',
+    'long_description': '[![Eclipse VOLTTRON™](https://img.shields.io/badge/Eclips%20VOLTTRON--red.svg)](https://volttron.readthedocs.io/en/latest/)\n![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)\n![Python 3.11](https://img.shields.io/badge/python-3.11-blue.svg)\n[![Run Pytests](https://github.com/eclipse-volttron/volttron-postgresql-historian/actions/workflows/run-tests.yml/badge.svg)](https://github.com/eclipse-volttron/volttron-postgresql-historian/actions/workflows/run-tests.yml)\n[![pypi version](https://img.shields.io/pypi/v/volttron-postgresql-historian.svg)](https://pypi.org/project/volttron-postgresql-historian/)\n\nVOLTTRON historian agent that stores data into a PostgreSQL database\n\n### Installation notes\n\n1.  The PostgreSQL database driver supports recent PostgreSQL versions.\n    It was tested on 10.x, but should work with 9.x and 11.x.\n2.  The user must have SELECT, INSERT, and UPDATE privileges on\n    historian tables.\n3.  The tables in the database are created as part of the execution of\n    the SQLHistorianAgent, but this will fail if the database user does\n    not have CREATE privileges.\n4.  Care must be exercised when using multiple historians with the same\n    database. This configuration may be used only if there is no overlap\n    in the topics handled by each instance. Otherwise, duplicate topic\n    IDs may be created, producing strange results.\n\n\n### Configuration\n\nPostgreSQL historian supports two configuration parameters\n    \n   - connection -  This is a mandatory parameter with type indicating the type of sql historian (i.e. postgresql) and params containing the database access details\n   - tables_def - Optional parameter to provide custom table names for topics, data, and metadata.\n    \nThe configuration can be in a json or yaml formatted file. The following examples show minimal connection \nconfigurations for a psycopg2-based historian. Other options are available and are [documented here](https://www.psycopg.org/docs/module.html#psycopg2.connect) \n**Not all parameters have been tested,  use at your own risk**.\n\n#### Local PostgreSQL Database\n\nThe following snippet demonstrates how to configure the historian to use a PostgreSQL database on the local system that\nis configured to use Unix domain sockets. The user executing volttron must have appropriate privileges.\n\n\n##### Yaml Format:\n```yaml\n    connection:\n          # type should be postgresql\n          type: postgresql\n          params:\n            # Relative to the agents data directory\n            dbname: "volttron"\n        \n    tables_def:\n        # prefix for data, topics, and (in version < 4.0.0 metadata tables)\n        # default is ""\n        table_prefix: ""\n        # table name for time series data. default "data"\n        data_table: data\n        # table name for list of topics. default "topics"\n        topics_table: topics\n ```\n\n##### JSON format:\n```json\n    {\n        "connection": {\n            "type": "postgresql", \n            "params": { "dbname": "volttron" }\n        }\n    }\n```\n\n#### Remote PostgreSQL Database\n\nThe following snippet demonstrates how to configure the historian to use a remote PostgreSQL database.\n```json\n    {\n        "connection": {\n            "type": "postgresql", \n            "params": { \n                "dbname": "volttron", \n                "host": "historian.example.com", \n                "port": 5432, \n                "user": "volttron", \n                "password": "secret" }\n        }\n    }\n```\n\n#### TimescaleDB Support\n\nBoth of the above PostgreSQL connection types can make use of TimescaleDB\\\'s high performance Hypertable backend for \nthe primary timeseries table. The agent assumes you have completed the TimescaleDB installation and setup the \ndatabase by following the instructions here: <https://docs.timescale.com/latest/getting-started/setup> To use, simply\nadd \\\'timescale_dialect: true\\\' to the connection params in the agent config as below\n\n```json\n    {\n        "connection": {\n            "type": "postgresql", \n            "params": { \n                "dbname": "volttron", \n                "host": "historian.example.com", \n                "port": 5432, \n                "user": "volttron", \n                "password": "secret" ,\n                "timescale_dialect": true }\n        }\n\n    }\n```\n\n## Requirements\n\n - Python >= 3.10\n - psycopg2 library\n\n## Installation\n\n1. Create and activate a virtual environment.\n\n   ```shell\n    python -m venv env\n    source env/bin/activate\n    ```\n\n2. Installing volttron-postgresql-historian requires a running volttron instance and the psycopg2 library \n\n    ```shell\n    pip install volttron\n    pip install psycopg2-binary\n    \n    # Start platform with output going to volttron.log\n    volttron -vv -l volttron.log &\n    ```\n3. Setup database\n   \n   If this is not a development environment we highly recommend that you create the database and database tables using\n   a user with appropriate permissions. This way the database user used by the historian need not have CREATE privileges\n   Postgres historian expects two tables \n   a. A topics tables that stores the list of unique topics and its metadata. The default name is "topics". If you use \n      a different name please specify it as part of "tables_def" configuration parameter in agent config. See [example configuration](#yaml-format)\n   b. A data table that stores the timeseries data and refers to the topic table using a topic id. The default name is \n      "data". If you use a different name please specify it as part of "tables_def" configuration parameter in \n      agent config. See [example configuration](#yaml-format)\n\n   Below are the sql statements to create database and tables\n   <u>Create Database</u>\n    ```\n       CREATE DATABASE volttron\n    ```\n   <u>TOPICS tables:</u>\n    ```\n        CREATE TABLE IF NOT EXISTS topics (\n            topic_id SERIAL PRIMARY KEY NOT NULL, \n            topic_name VARCHAR(512) NOT NULL, \n            metadata TEXT, \n            UNIQUE (topic_name)\n       )\n    ```\n    <u>DATA table:</u>\n    ```\n       CREATE TABLE IF NOT EXISTS data (\n           ts TIMESTAMP NOT NULL, \n           topic_id INTEGER NOT NULL, \n           value_string TEXT NOT NULL, \n           UNIQUE (topic_id, ts)\n       )\n    ```\n     <u>Optional timescale hypertable</u>\n    ```\n       SELECT create_hypertable(data, \'ts\', if_not_exists => true)\n    ```\n     <u>Create index to speed up data access</u>\n       If using hypertables:\n    ```\n        CREATE INDEX IF NOT EXISTS idx_data ON data (topic_id, ts)\n    ```\n      If not using hypertables:\n    ```\n        CREATE INDEX IF NOT EXISTS idx_data ON data (ts ASC)\n    ```\n    <u>Provide correct user permissions for database user to be used by historian agent</u>\n    ```\n        CREATE USER <some username> with encrypted password <some password>\n        GRANT SELECT, INSERT, UPDATE on database <historian db name> to <username used above>\n    ``` \n    **NOTE**\n    For development environments, you can create a test database and test user, grant all privileges on that test \n    database to the test user and let the historian create tables and indexes at startup. We do not recommend this for \n    production environments\n\n4. Create an agent configuration file \n\n    Create an agent configuration with appropriate connection parameters as described in the [Configurations section](#Configuration)\n\n5. Install and start the volttron-postgresql-historian.\n\n    ```shell\n    vctl install volttron-postgresql-historian --agent-config <path to configuration> --start\n    ```\n\n6. View the status of the installed agent\n\n    ```shell\n    vctl status\n    ```\n\n## Development\n\nPlease see the following for contributing guidelines [contributing](https://github.com/eclipse-volttron/volttron-core/blob/develop/CONTRIBUTING.md).\n\nPlease see the following helpful guide about [developing modular VOLTTRON agents](https://github.com/eclipse-volttron/volttron-core/blob/develop/DEVELOPING_ON_MODULAR.md)\n\n# Disclaimer Notice\n\nThis material was prepared as an account of work sponsored by an agency of the\nUnited States Government.  Neither the United States Government nor the United\nStates Department of Energy, nor Battelle, nor any of their employees, nor any\njurisdiction or organization that has cooperated in the development of these\nmaterials, makes any warranty, express or implied, or assumes any legal\nliability or responsibility for the accuracy, completeness, or usefulness or any\ninformation, apparatus, product, software, or process disclosed, or represents\nthat its use would not infringe privately owned rights.\n\nReference herein to any specific commercial product, process, or service by\ntrade name, trademark, manufacturer, or otherwise does not necessarily\nconstitute or imply its endorsement, recommendation, or favoring by the United\nStates Government or any agency thereof, or Battelle Memorial Institute. The\nviews and opinions of authors expressed herein do not necessarily state or\nreflect those of the United States Government or any agency thereof.\n',
     'author': 'VOLTTRON Team',
     'author_email': 'volttron@pnnl.gov',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/eclipse-volttron/volttron-postgresql-historian',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `volttron_postgresql_historian-0.1.2rc1/PKG-INFO` & `volttron_postgresql_historian-0.1.2rc2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volttron-postgresql-historian
-Version: 0.1.2rc1
+Version: 0.1.2rc2
 Summary: VOLTTRON historian agent that stores data in a PostgreSQL database. It extends the SQLHistorian class.
 Home-page: https://github.com/eclipse-volttron/volttron-postgresql-historian
 License: Apache-2.0
 Author: VOLTTRON Team
 Author-email: volttron@pnnl.gov
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -15,17 +15,16 @@
 Requires-Dist: volttron-lib-sql-historian (>=0.1.1a8,<0.2.0)
 Project-URL: Repository, https://github.com/eclipse-volttron/volttron-postgresql-historian
 Description-Content-Type: text/markdown
 
 [![Eclipse VOLTTRON™](https://img.shields.io/badge/Eclips%20VOLTTRON--red.svg)](https://volttron.readthedocs.io/en/latest/)
 ![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)
 ![Python 3.11](https://img.shields.io/badge/python-3.11-blue.svg)
-[![Run Pytests](https://github.com/eclipse-volttron/volttron-postgresql-historian/actions/workflows/run-test.yml/badge.svg)](https://github.com/eclipse-volttron/volttron-postgresql-historian/actions/workflows/run-test.yml)
+[![Run Pytests](https://github.com/eclipse-volttron/volttron-postgresql-historian/actions/workflows/run-tests.yml/badge.svg)](https://github.com/eclipse-volttron/volttron-postgresql-historian/actions/workflows/run-tests.yml)
 [![pypi version](https://img.shields.io/pypi/v/volttron-postgresql-historian.svg)](https://pypi.org/project/volttron-postgresql-historian/)
-![Passing?](https://github.com/VOLTTRON/volttron-postgresql-historian/actions/workflows/run-tests.yml/badge.svg)
 
 VOLTTRON historian agent that stores data into a PostgreSQL database
 
 ### Installation notes
 
 1.  The PostgreSQL database driver supports recent PostgreSQL versions.
     It was tested on 10.x, but should work with 9.x and 11.x.
```

