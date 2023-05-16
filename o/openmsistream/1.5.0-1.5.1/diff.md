# Comparing `tmp/openmsistream-1.5.0.tar.gz` & `tmp/openmsistream-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openmsistream-1.5.0.tar", last modified: Mon May  8 20:19:57 2023, max compression
+gzip compressed data, was "openmsistream-1.5.1.tar", last modified: Tue May 16 17:13:34 2023, max compression
```

## Comparing `openmsistream-1.5.0.tar` & `openmsistream-1.5.1.tar`

### file list

```diff
@@ -1,116 +1,116 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:19:57.553995 openmsistream-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-05-08 20:19:51.000000 openmsistream-1.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-08 20:19:51.000000 openmsistream-1.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-08 20:19:57.553995 openmsistream-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-05-08 20:19:51.000000 openmsistream-1.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:19:57.537995 openmsistream-1.5.0/openmsistream/
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:19:57.537995 openmsistream-1.5.0/openmsistream/data_file_io/
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/data_file_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:19:57.537995 openmsistream-1.5.0/openmsistream/data_file_io/actor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/data_file_io/actor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7695 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/data_file_io/actor/data_file_chunk_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10790 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/data_file_io/actor/data_file_download_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)     7699 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/data_file_io/actor/data_file_stream_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12688 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/data_file_io/actor/data_file_stream_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)    18974 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/data_file_io/actor/data_file_stream_reproducer.py
--rw-r--r--   0 runner    (1001) docker     (123)    31418 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/data_file_io/actor/data_file_upload_directory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:19:57.541995 openmsistream-1.5.0/openmsistream/data_file_io/actor/file_registry/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/data_file_io/actor/file_registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13916 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/data_file_io/actor/file_registry/producer_file_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    16852 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/data_file_io/actor/file_registry/stream_handler_registries.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/data_file_io/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:19:57.541995 openmsistream-1.5.0/openmsistream/data_file_io/entity/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/data_file_io/entity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/data_file_io/entity/data_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     9997 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/data_file_io/entity/data_file_chunk.py
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/data_file_io/entity/data_file_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)    13001 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/data_file_io/entity/download_data_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/data_file_io/entity/reproducer_message.py
--rw-r--r--   0 runner    (1001) docker     (123)    17905 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/data_file_io/entity/upload_data_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     6721 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/data_file_io/entity/upload_directory_event_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/data_file_io/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:19:57.541995 openmsistream-1.5.0/openmsistream/kafka_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/kafka_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6354 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/kafka_wrapper/config_file_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:19:57.545995 openmsistream-1.5.0/openmsistream/kafka_wrapper/config_files/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/kafka_wrapper/config_files/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/kafka_wrapper/config_files/local_broker_test.config
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/kafka_wrapper/config_files/local_broker_test_encrypted.config
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/kafka_wrapper/config_files/local_broker_test_encrypted_2.config
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/kafka_wrapper/config_files/local_broker_test_metadata_rep_consumer.config
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/kafka_wrapper/config_files/local_broker_test_s3_transfer.config
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/kafka_wrapper/config_files/prod.config
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/kafka_wrapper/config_files/test.config
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/kafka_wrapper/config_files/test_encrypted.config
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/kafka_wrapper/config_files/test_encrypted_2.config
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/kafka_wrapper/config_files/test_metadata_rep_consumer.config
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/kafka_wrapper/config_files/test_s3_transfer.config
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:19:57.545995 openmsistream-1.5.0/openmsistream/kafka_wrapper/config_files/testing_node/
--rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/kafka_wrapper/config_files/testing_node/testing_node.config
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/kafka_wrapper/config_files/testing_node/testing_node.crypto
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/kafka_wrapper/config_files/testing_node/testing_node.seed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:19:57.545995 openmsistream-1.5.0/openmsistream/kafka_wrapper/config_files/testing_node_2/
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/kafka_wrapper/config_files/testing_node_2/testing_node_2.config
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/kafka_wrapper/config_files/testing_node_2/testing_node_2.crypto
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/kafka_wrapper/config_files/testing_node_2/testing_node_2.seed
--rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/kafka_wrapper/consumer_and_producer_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/kafka_wrapper/consumer_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/kafka_wrapper/controlled_message_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9651 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/kafka_wrapper/controlled_message_reproducer.py
--rw-r--r--   0 runner    (1001) docker     (123)    19752 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/kafka_wrapper/openmsistream_consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/kafka_wrapper/openmsistream_kafka_crypto.py
--rw-r--r--   0 runner    (1001) docker     (123)    16366 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/kafka_wrapper/openmsistream_producer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/kafka_wrapper/producer_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/kafka_wrapper/producible.py
--rw-r--r--   0 runner    (1001) docker     (123)     9474 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/kafka_wrapper/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/kafka_wrapper/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:19:57.545995 openmsistream-1.5.0/openmsistream/metadata_extraction/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/metadata_extraction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/metadata_extraction/metadata_json_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     7071 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/metadata_extraction/metadata_json_reproducer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:19:57.549995 openmsistream-1.5.0/openmsistream/s3_buckets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/s3_buckets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/s3_buckets/config_file_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/s3_buckets/s3_data_transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/s3_buckets/s3_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/s3_buckets/s3_transfer_stream_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:19:57.549995 openmsistream-1.5.0/openmsistream/services/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/services/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:19:57.549995 openmsistream-1.5.0/openmsistream/services/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/services/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/services/examples/runnable_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/services/examples/script_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/services/install_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     8932 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/services/linux_service_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/services/manage_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    22467 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/services/service_manager_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5508 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/services/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    12104 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/services/windows_service_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:19:57.553995 openmsistream-1.5.0/openmsistream/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22161 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/utilities/argument_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/utilities/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/utilities/config_file_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/utilities/controlled_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     6020 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/utilities/controlled_process_multi_threaded.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/utilities/controlled_process_single_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)    22492 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/utilities/dataclass_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/utilities/exception_tracking_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/utilities/has_argument_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/utilities/has_arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)     9644 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/utilities/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/utilities/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6654 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/utilities/provision_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/utilities/runnable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:19:57.537995 openmsistream-1.5.0/openmsistream.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-08 20:19:57.000000 openmsistream-1.5.0/openmsistream.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-05-08 20:19:57.000000 openmsistream-1.5.0/openmsistream.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 20:19:57.000000 openmsistream-1.5.0/openmsistream.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-08 20:19:57.000000 openmsistream-1.5.0/openmsistream.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-08 20:19:57.000000 openmsistream-1.5.0/openmsistream.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-08 20:19:57.000000 openmsistream-1.5.0/openmsistream.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-08 20:19:51.000000 openmsistream-1.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-08 20:19:57.553995 openmsistream-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-05-08 20:19:51.000000 openmsistream-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:13:34.463081 openmsistream-1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-05-16 17:13:25.000000 openmsistream-1.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-16 17:13:25.000000 openmsistream-1.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-16 17:13:34.463081 openmsistream-1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-05-16 17:13:25.000000 openmsistream-1.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:13:34.455081 openmsistream-1.5.1/openmsistream/
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:13:34.455081 openmsistream-1.5.1/openmsistream/data_file_io/
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/data_file_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:13:34.455081 openmsistream-1.5.1/openmsistream/data_file_io/actor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/data_file_io/actor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7695 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/data_file_io/actor/data_file_chunk_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10813 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/data_file_io/actor/data_file_download_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7699 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/data_file_io/actor/data_file_stream_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12711 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/data_file_io/actor/data_file_stream_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18974 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/data_file_io/actor/data_file_stream_reproducer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31405 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/data_file_io/actor/data_file_upload_directory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:13:34.455081 openmsistream-1.5.1/openmsistream/data_file_io/actor/file_registry/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/data_file_io/actor/file_registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13916 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/data_file_io/actor/file_registry/producer_file_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16852 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/data_file_io/actor/file_registry/stream_handler_registries.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/data_file_io/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:13:34.455081 openmsistream-1.5.1/openmsistream/data_file_io/entity/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/data_file_io/entity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/data_file_io/entity/data_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9997 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/data_file_io/entity/data_file_chunk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/data_file_io/entity/data_file_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13001 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/data_file_io/entity/download_data_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/data_file_io/entity/reproducer_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17892 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/data_file_io/entity/upload_data_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6721 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/data_file_io/entity/upload_directory_event_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/data_file_io/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:13:34.459081 openmsistream-1.5.1/openmsistream/kafka_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/kafka_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6354 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/kafka_wrapper/config_file_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:13:34.459081 openmsistream-1.5.1/openmsistream/kafka_wrapper/config_files/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/kafka_wrapper/config_files/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/kafka_wrapper/config_files/local_broker_test.config
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/kafka_wrapper/config_files/local_broker_test_encrypted.config
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/kafka_wrapper/config_files/local_broker_test_encrypted_2.config
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/kafka_wrapper/config_files/local_broker_test_metadata_rep_consumer.config
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/kafka_wrapper/config_files/local_broker_test_s3_transfer.config
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/kafka_wrapper/config_files/prod.config
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/kafka_wrapper/config_files/test.config
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/kafka_wrapper/config_files/test_encrypted.config
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/kafka_wrapper/config_files/test_encrypted_2.config
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/kafka_wrapper/config_files/test_metadata_rep_consumer.config
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/kafka_wrapper/config_files/test_s3_transfer.config
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:13:34.459081 openmsistream-1.5.1/openmsistream/kafka_wrapper/config_files/testing_node/
+-rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/kafka_wrapper/config_files/testing_node/testing_node.config
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/kafka_wrapper/config_files/testing_node/testing_node.crypto
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/kafka_wrapper/config_files/testing_node/testing_node.seed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:13:34.459081 openmsistream-1.5.1/openmsistream/kafka_wrapper/config_files/testing_node_2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/kafka_wrapper/config_files/testing_node_2/testing_node_2.config
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/kafka_wrapper/config_files/testing_node_2/testing_node_2.crypto
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/kafka_wrapper/config_files/testing_node_2/testing_node_2.seed
+-rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/kafka_wrapper/consumer_and_producer_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/kafka_wrapper/consumer_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/kafka_wrapper/controlled_message_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9651 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/kafka_wrapper/controlled_message_reproducer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19752 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/kafka_wrapper/openmsistream_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/kafka_wrapper/openmsistream_kafka_crypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16366 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/kafka_wrapper/openmsistream_producer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/kafka_wrapper/producer_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/kafka_wrapper/producible.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9474 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/kafka_wrapper/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/kafka_wrapper/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:13:34.459081 openmsistream-1.5.1/openmsistream/metadata_extraction/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/metadata_extraction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/metadata_extraction/metadata_json_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7071 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/metadata_extraction/metadata_json_reproducer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:13:34.459081 openmsistream-1.5.1/openmsistream/s3_buckets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/s3_buckets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/s3_buckets/config_file_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/s3_buckets/s3_data_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/s3_buckets/s3_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/s3_buckets/s3_transfer_stream_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:13:34.459081 openmsistream-1.5.1/openmsistream/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/services/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:13:34.463081 openmsistream-1.5.1/openmsistream/services/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/services/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/services/examples/runnable_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/services/examples/script_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/services/install_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8932 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/services/linux_service_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/services/manage_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22467 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/services/service_manager_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5508 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/services/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12104 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/services/windows_service_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:13:34.463081 openmsistream-1.5.1/openmsistream/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22077 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/utilities/argument_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/utilities/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/utilities/config_file_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/utilities/controlled_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6020 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/utilities/controlled_process_multi_threaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/utilities/controlled_process_single_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22492 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/utilities/dataclass_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/utilities/exception_tracking_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/utilities/has_argument_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/utilities/has_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9644 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/utilities/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/utilities/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6654 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/utilities/provision_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/utilities/runnable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:13:34.455081 openmsistream-1.5.1/openmsistream.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-16 17:13:34.000000 openmsistream-1.5.1/openmsistream.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-05-16 17:13:34.000000 openmsistream-1.5.1/openmsistream.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 17:13:34.000000 openmsistream-1.5.1/openmsistream.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-16 17:13:34.000000 openmsistream-1.5.1/openmsistream.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-16 17:13:34.000000 openmsistream-1.5.1/openmsistream.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-16 17:13:34.000000 openmsistream-1.5.1/openmsistream.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-16 17:13:25.000000 openmsistream-1.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-16 17:13:34.463081 openmsistream-1.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-05-16 17:13:25.000000 openmsistream-1.5.1/setup.py
```

### Comparing `openmsistream-1.5.0/LICENSE` & `openmsistream-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.0/PKG-INFO` & `openmsistream-1.5.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: openmsistream
-Version: 1.5.0
+Version: 1.5.1
 Summary: Python applications for materials data streaming using Apache Kafka. Developed for Open MSI (NSF DMREF award #1921959)
 Home-page: https://github.com/openmsi/openmsistream
 Author: OpenMSIStream
 Author-email: openmsistream@gmail.com
 License: GNU GPLv3
-Download-URL: https://github.com/openmsi/openmsistream/archive/refs/tags/v1.5.0.tar.gz
+Download-URL: https://github.com/openmsi/openmsistream/archive/refs/tags/v1.5.1.tar.gz
 Keywords: data_streaming,stream_processing,apache_kafka,materials,data_science
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7,<3.10
```

### Comparing `openmsistream-1.5.0/README.md` & `openmsistream-1.5.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # <div align="center"> OpenMSIStream </div>
-#### <div align="center">***v1.5.0***</div>
+#### <div align="center">***v1.5.1***</div>
 
 #### <div align="center">Maggie Eminizer<sup>1</sup>, Sam Tabrisky<sup>2,3,4</sup>, Amir Sharifzadeh<sup>1</sup>, Christopher DiMarco<sup>4</sup>, Jacob M. Diamond<sup>4,6</sup>, K.T. Ramesh<sup>4</sup>, Todd C. Hufnagel<sup>4,5,6</sup>, Tyrel M. McQueen<sup>4,5,7,8</sup>, David Elbert<sup>1,4</sup></div>
 
  <div align="center"><sup>1</sup> Institute for Data Intensive Engineering and Science (IDIES), The Johns Hopkins University, Baltimore, MD, USA </div>
  <div align="center"><sup>2</sup> Department of Biology, Dartmouth College, Hanover, NH, USA </div>
  <div align="center"><sup>3</sup> Department of Computer Science, Dartmouth College, Hanover, NH, USA </div>
  <div align="center"><sup>4</sup> Hopkins Extreme Materials Institute (HEMI), The Johns Hopkins University, Baltimore, MD, USA </div>
```

### Comparing `openmsistream-1.5.0/openmsistream/__init__.py` & `openmsistream-1.5.1/openmsistream/__init__.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.0/openmsistream/data_file_io/__init__.py` & `openmsistream-1.5.1/openmsistream/data_file_io/__init__.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.0/openmsistream/data_file_io/actor/data_file_chunk_handlers.py` & `openmsistream-1.5.1/openmsistream/data_file_io/actor/data_file_chunk_handlers.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.0/openmsistream/data_file_io/actor/data_file_download_directory.py` & `openmsistream-1.5.1/openmsistream/data_file_io/actor/data_file_download_directory.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,17 @@
 
 # imports
 import datetime, warnings
 
 with warnings.catch_warnings():
     warnings.simplefilter("ignore")
     from kafkacrypto.message import KafkaCryptoMessage
+from ...utilities.config import RUN_CONST
 from ...utilities import Runnable
-from ..config import DATA_FILE_HANDLING_CONST, RUN_OPT_CONST
+from ..config import DATA_FILE_HANDLING_CONST
 from ..utilities import get_encrypted_message_key_and_value_filenames
 from .. import DataFileDirectory, DownloadDataFileToDisk
 from .data_file_chunk_handlers import DataFileChunkProcessor
 
 
 class DataFileDownloadDirectory(DataFileDirectory, DataFileChunkProcessor, Runnable):
     """
@@ -192,15 +193,15 @@
             "output_dir",
             "config",
             "topic_name",
             "update_seconds",
             "consumer_group_id",
             "download_regex",
         ]
-        kwargs = {**superkwargs, "n_threads": RUN_OPT_CONST.N_DEFAULT_DOWNLOAD_THREADS}
+        kwargs = {**superkwargs, "n_threads": RUN_CONST.N_DEFAULT_DOWNLOAD_THREADS}
         return args, kwargs
 
     @classmethod
     def run_from_command_line(cls, args=None):
         """
         Run a :class:`~DataFileDownloadDirectory` directly from the command line
```

### Comparing `openmsistream-1.5.0/openmsistream/data_file_io/actor/data_file_stream_handler.py` & `openmsistream-1.5.1/openmsistream/data_file_io/actor/data_file_stream_handler.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.0/openmsistream/data_file_io/actor/data_file_stream_processor.py` & `openmsistream-1.5.1/openmsistream/data_file_io/actor/data_file_stream_processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """A DataFileStreamHandler that triggers some arbitrary local code when full files are available"""
 
 # imports
 from abc import ABC, abstractmethod
-from ..config import RUN_OPT_CONST, DATA_FILE_HANDLING_CONST
+from ...utilities.config import RUN_CONST
+from ..config import DATA_FILE_HANDLING_CONST
 from .data_file_chunk_handlers import DataFileChunkProcessor
 from .data_file_stream_handler import DataFileStreamHandler
 from .file_registry.stream_handler_registries import StreamProcessorRegistry
 
 
 class DataFileStreamProcessor(DataFileStreamHandler, DataFileChunkProcessor, ABC):
     """
@@ -252,9 +253,9 @@
         super()._on_shutdown()
         self.file_registry.consolidate_succeeded_files()
 
     @classmethod
     def get_command_line_arguments(cls):
         superargs, superkwargs = super().get_command_line_arguments()
         args = [*superargs, "topic_name", "download_regex"]
-        kwargs = {**superkwargs, "n_threads": RUN_OPT_CONST.N_DEFAULT_DOWNLOAD_THREADS}
+        kwargs = {**superkwargs, "n_threads": RUN_CONST.N_DEFAULT_DOWNLOAD_THREADS}
         return args, kwargs
```

### Comparing `openmsistream-1.5.0/openmsistream/data_file_io/actor/data_file_stream_reproducer.py` & `openmsistream-1.5.1/openmsistream/data_file_io/actor/data_file_stream_reproducer.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.0/openmsistream/data_file_io/actor/data_file_upload_directory.py` & `openmsistream-1.5.1/openmsistream/data_file_io/actor/data_file_upload_directory.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 
 # imports
 import datetime, time
 from threading import Lock
 from queue import Queue
 from watchdog.observers import Observer
 from ...kafka_wrapper import ProducerGroup
+from ...utilities.config import RUN_CONST
 from ...utilities import Runnable, ControlledProcessSingleThread
 from ...utilities.misc import populated_kwargs
 from ...utilities.exception_tracking_thread import ExceptionTrackingThread
-from ..config import RUN_OPT_CONST
 from .. import DataFileDirectory
 from .file_registry.producer_file_registry import ProducerFileRegistry
 from ..entity.upload_data_file import UploadDataFile
 from ..entity.upload_directory_event_handler import UploadDirectoryEventHandler
 
 
 class DataFileUploadDirectory(
@@ -55,15 +55,15 @@
 
     #################### PUBLIC FUNCTIONS ####################
 
     def __init__(
         self,
         dirpath,
         config_path,
-        upload_regex=RUN_OPT_CONST.DEFAULT_UPLOAD_REGEX,
+        upload_regex=RUN_CONST.DEFAULT_UPLOAD_REGEX,
         datafile_type=UploadDataFile,
         **kwargs,
     ):
         """
         Constructor method
         """
         # create a subdirectory for the logs
@@ -96,17 +96,17 @@
         self.__upload_queue = None
         self.__producers = []
         self.__upload_threads = []
 
     def upload_files_as_added(
         self,
         topic_name,
-        n_threads=RUN_OPT_CONST.N_DEFAULT_UPLOAD_THREADS,
-        chunk_size=RUN_OPT_CONST.DEFAULT_CHUNK_SIZE,
-        max_queue_size=RUN_OPT_CONST.DEFAULT_MAX_UPLOAD_QUEUE_MEGABYTES,
+        n_threads=RUN_CONST.N_DEFAULT_UPLOAD_THREADS,
+        chunk_size=RUN_CONST.DEFAULT_CHUNK_SIZE,
+        max_queue_size=RUN_CONST.DEFAULT_MAX_UPLOAD_QUEUE_MEGABYTES,
         upload_existing=False,
     ):
         """
         Watch for new files to be added to the directory.
         Chunk and produce newly added files as messages to a Kafka topic.
 
         :param topic_name: Name of the topic to produce messages to
@@ -558,15 +558,15 @@
             "topic_name",
             "upload_regex",
             "chunk_size",
             "queue_max_size",
             "update_seconds",
             "upload_existing",
         ]
-        kwargs = {**superkwargs, "n_threads": RUN_OPT_CONST.N_DEFAULT_UPLOAD_THREADS}
+        kwargs = {**superkwargs, "n_threads": RUN_CONST.N_DEFAULT_UPLOAD_THREADS}
         return args, kwargs
 
     @classmethod
     def run_from_command_line(cls, args=None):
         """
         Run a :class:`~DataFileUploadDirectory` directly from the command line
```

### Comparing `openmsistream-1.5.0/openmsistream/data_file_io/actor/file_registry/producer_file_registry.py` & `openmsistream-1.5.1/openmsistream/data_file_io/actor/file_registry/producer_file_registry.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.0/openmsistream/data_file_io/actor/file_registry/stream_handler_registries.py` & `openmsistream-1.5.1/openmsistream/data_file_io/actor/file_registry/stream_handler_registries.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.0/openmsistream/data_file_io/entity/data_file.py` & `openmsistream-1.5.1/openmsistream/data_file_io/entity/data_file.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.0/openmsistream/data_file_io/entity/data_file_chunk.py` & `openmsistream-1.5.1/openmsistream/data_file_io/entity/data_file_chunk.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.0/openmsistream/data_file_io/entity/data_file_directory.py` & `openmsistream-1.5.1/openmsistream/data_file_io/entity/data_file_directory.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.0/openmsistream/data_file_io/entity/download_data_file.py` & `openmsistream-1.5.1/openmsistream/data_file_io/entity/download_data_file.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.0/openmsistream/data_file_io/entity/reproducer_message.py` & `openmsistream-1.5.1/openmsistream/data_file_io/entity/reproducer_message.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.0/openmsistream/data_file_io/entity/upload_data_file.py` & `openmsistream-1.5.1/openmsistream/data_file_io/entity/upload_data_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """A DataFile that will be broken into chunks and uploaded to a topic"""
 
 # imports
 import time, datetime
 from threading import Thread
 from queue import Queue
 from hashlib import sha512
+from ...utilities.config import RUN_CONST
 from ...utilities import Runnable
 from ...kafka_wrapper import ProducerGroup
-from ..config import RUN_OPT_CONST
 from .. import DataFile
 from .data_file_chunk import DataFileChunk
 
 
 class UploadDataFile(DataFile, Runnable):
     """
     Class to represent a data file whose messages will be uploaded to a topic
@@ -53,16 +53,16 @@
         self.__file_hash = None
         self.__chunked_at_timestamp = None
 
     def upload_whole_file(
         self,
         config_path,
         topic_name,
-        n_threads=RUN_OPT_CONST.N_DEFAULT_UPLOAD_THREADS,
-        chunk_size=RUN_OPT_CONST.DEFAULT_CHUNK_SIZE,
+        n_threads=RUN_CONST.N_DEFAULT_UPLOAD_THREADS,
+        chunk_size=RUN_CONST.DEFAULT_CHUNK_SIZE,
     ):
         """
         Chunk and upload an entire file on disk to a broker's topic.
 
         :param config_path: Path to the config file to use in defining the Broker connection
             and Producers
         :type config_path: :class:`pathlib.Path`
@@ -107,15 +107,15 @@
                 timeout=-1
             )  # don't leave the function until all messages have been sent/received
             producer.close()
         producer_group.close()
         self.logger.info(f"Done uploading {self.filepath}")
 
     def add_chunks_to_upload(
-        self, chunks_to_add=None, chunk_size=RUN_OPT_CONST.DEFAULT_CHUNK_SIZE
+        self, chunks_to_add=None, chunk_size=RUN_CONST.DEFAULT_CHUNK_SIZE
     ):
         """
         Add chunks from this file to the internal list of chunks to upload,
         possibly with some selection defined by :attr:`~select_bytes`
 
         :param chunks_to_add: a list of chunk indices to add to the list to be uploaded
             (Default=None adds all chunks)
@@ -160,15 +160,15 @@
         if len(self.chunks_to_upload) > 0 and self.__fully_enqueued:
             self.__fully_enqueued = False
 
     def enqueue_chunks_for_upload(
         self,
         queue,
         n_threads=None,
-        chunk_size=RUN_OPT_CONST.DEFAULT_CHUNK_SIZE,
+        chunk_size=RUN_CONST.DEFAULT_CHUNK_SIZE,
         queue_full_timeout=0.001,
     ):
         """
         Add some chunks of this file from the internal list to a given upload queue
         (the internal list will be created if :func:`~add_chunks_to_upload`
         hasn't already been called).
 
@@ -291,15 +291,15 @@
 
     #################### CLASS METHODS ####################
 
     @classmethod
     def get_command_line_arguments(cls):
         superargs, superkwargs = super().get_command_line_arguments()
         args = [*superargs, "filepath", "config", "topic_name", "chunk_size"]
-        kwargs = {**superkwargs, "n_threads": RUN_OPT_CONST.N_DEFAULT_UPLOAD_THREADS}
+        kwargs = {**superkwargs, "n_threads": RUN_CONST.N_DEFAULT_UPLOAD_THREADS}
         return args, kwargs
 
     @classmethod
     def run_from_command_line(cls, args=None):
         """
         Run an :class:`~UploadDataFile` directly from the command line
```

### Comparing `openmsistream-1.5.0/openmsistream/data_file_io/entity/upload_directory_event_handler.py` & `openmsistream-1.5.1/openmsistream/data_file_io/entity/upload_directory_event_handler.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.0/openmsistream/data_file_io/utilities.py` & `openmsistream-1.5.1/openmsistream/data_file_io/utilities.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.0/openmsistream/kafka_wrapper/__init__.py` & `openmsistream-1.5.1/openmsistream/kafka_wrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.0/openmsistream/kafka_wrapper/config_file_parser.py` & `openmsistream-1.5.1/openmsistream/kafka_wrapper/config_file_parser.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.0/openmsistream/kafka_wrapper/config_files/local_broker_test_s3_transfer.config` & `openmsistream-1.5.1/openmsistream/kafka_wrapper/config_files/local_broker_test_s3_transfer.config`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.0/openmsistream/kafka_wrapper/config_files/prod.config` & `openmsistream-1.5.1/openmsistream/kafka_wrapper/config_files/prod.config`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.0/openmsistream/kafka_wrapper/config_files/test.config` & `openmsistream-1.5.1/openmsistream/kafka_wrapper/config_files/test.config`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.0/openmsistream/kafka_wrapper/config_files/test_encrypted.config` & `openmsistream-1.5.1/openmsistream/kafka_wrapper/config_files/test_encrypted.config`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.0/openmsistream/kafka_wrapper/config_files/test_encrypted_2.config` & `openmsistream-1.5.1/openmsistream/kafka_wrapper/config_files/test_encrypted_2.config`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.0/openmsistream/kafka_wrapper/config_files/test_s3_transfer.config` & `openmsistream-1.5.1/openmsistream/kafka_wrapper/config_files/test_s3_transfer.config`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.0/openmsistream/kafka_wrapper/config_files/testing_node/testing_node.config` & `openmsistream-1.5.1/openmsistream/kafka_wrapper/config_files/testing_node/testing_node.config`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.0/openmsistream/kafka_wrapper/config_files/testing_node_2/testing_node_2.config` & `openmsistream-1.5.1/openmsistream/kafka_wrapper/config_files/testing_node_2/testing_node_2.config`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.0/openmsistream/kafka_wrapper/consumer_and_producer_group.py` & `openmsistream-1.5.1/openmsistream/kafka_wrapper/consumer_and_producer_group.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.0/openmsistream/kafka_wrapper/consumer_group.py` & `openmsistream-1.5.1/openmsistream/kafka_wrapper/consumer_group.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.0/openmsistream/kafka_wrapper/controlled_message_processor.py` & `openmsistream-1.5.1/openmsistream/kafka_wrapper/controlled_message_processor.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.0/openmsistream/kafka_wrapper/controlled_message_reproducer.py` & `openmsistream-1.5.1/openmsistream/kafka_wrapper/controlled_message_reproducer.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.0/openmsistream/kafka_wrapper/openmsistream_consumer.py` & `openmsistream-1.5.1/openmsistream/kafka_wrapper/openmsistream_consumer.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.0/openmsistream/kafka_wrapper/openmsistream_kafka_crypto.py` & `openmsistream-1.5.1/openmsistream/kafka_wrapper/openmsistream_kafka_crypto.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.0/openmsistream/kafka_wrapper/openmsistream_producer.py` & `openmsistream-1.5.1/openmsistream/kafka_wrapper/openmsistream_producer.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.0/openmsistream/kafka_wrapper/producer_group.py` & `openmsistream-1.5.1/openmsistream/kafka_wrapper/producer_group.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.0/openmsistream/kafka_wrapper/producible.py` & `openmsistream-1.5.1/openmsistream/kafka_wrapper/producible.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.0/openmsistream/kafka_wrapper/serialization.py` & `openmsistream-1.5.1/openmsistream/kafka_wrapper/serialization.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.0/openmsistream/kafka_wrapper/utilities.py` & `openmsistream-1.5.1/openmsistream/kafka_wrapper/utilities.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.0/openmsistream/metadata_extraction/metadata_json_message.py` & `openmsistream-1.5.1/openmsistream/metadata_extraction/metadata_json_message.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.0/openmsistream/metadata_extraction/metadata_json_reproducer.py` & `openmsistream-1.5.1/openmsistream/metadata_extraction/metadata_json_reproducer.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.0/openmsistream/s3_buckets/config_file_parser.py` & `openmsistream-1.5.1/openmsistream/s3_buckets/config_file_parser.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.0/openmsistream/s3_buckets/s3_data_transfer.py` & `openmsistream-1.5.1/openmsistream/s3_buckets/s3_data_transfer.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.0/openmsistream/s3_buckets/s3_service.py` & `openmsistream-1.5.1/openmsistream/s3_buckets/s3_service.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.0/openmsistream/s3_buckets/s3_transfer_stream_processor.py` & `openmsistream-1.5.1/openmsistream/s3_buckets/s3_transfer_stream_processor.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.0/openmsistream/services/config.py` & `openmsistream-1.5.1/openmsistream/services/config.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.0/openmsistream/services/examples/runnable_example.py` & `openmsistream-1.5.1/openmsistream/services/examples/runnable_example.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.0/openmsistream/services/examples/script_example.py` & `openmsistream-1.5.1/openmsistream/services/examples/script_example.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.0/openmsistream/services/install_service.py` & `openmsistream-1.5.1/openmsistream/services/install_service.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.0/openmsistream/services/linux_service_manager.py` & `openmsistream-1.5.1/openmsistream/services/linux_service_manager.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.0/openmsistream/services/manage_service.py` & `openmsistream-1.5.1/openmsistream/services/manage_service.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.0/openmsistream/services/service_manager_base.py` & `openmsistream-1.5.1/openmsistream/services/service_manager_base.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.0/openmsistream/services/utilities.py` & `openmsistream-1.5.1/openmsistream/services/utilities.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.0/openmsistream/services/windows_service_manager.py` & `openmsistream-1.5.1/openmsistream/services/windows_service_manager.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.0/openmsistream/utilities/__init__.py` & `openmsistream-1.5.1/openmsistream/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.0/openmsistream/utilities/argument_parsing.py` & `openmsistream-1.5.1/openmsistream/utilities/argument_parsing.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """Custom argument parser and associated functions"""
 
 # imports
 import pathlib, math, re, logging
 from argparse import ArgumentParser
-from ..data_file_io.config import RUN_OPT_CONST
 from .config import RUN_CONST
 
 #################### MISC. FUNCTIONS ####################
 
 
 def existing_file(argstring):
     """
@@ -188,97 +187,97 @@
                     "Name should only contain valid characters"
                 ),
             },
         ],
         "config": [
             "optional",
             {
-                "default": RUN_OPT_CONST.DEFAULT_CONFIG_FILE,
+                "default": RUN_CONST.DEFAULT_CONFIG_FILE,
                 "type": config_path,
                 "help": (
                     f"Name of config file to use in {RUN_CONST.CONFIG_FILE_DIR.resolve()}, "
                     "or path to a file in a different location"
                 ),
             },
         ],
         "topic_name": [
             "optional",
             {
-                "default": RUN_OPT_CONST.DEFAULT_TOPIC_NAME,
+                "default": RUN_CONST.DEFAULT_TOPIC_NAME,
                 "help": "Name of the topic to produce to or consume from",
             },
         ],
         "consumer_topic_name": [
             "optional",
             {
-                "default": RUN_OPT_CONST.DEFAULT_TOPIC_NAME,
+                "default": RUN_CONST.DEFAULT_TOPIC_NAME,
                 "help": "Name of the topic to consume from",
             },
         ],
         "producer_topic_name": [
             "optional",
             {
-                "default": RUN_OPT_CONST.DEFAULT_TOPIC_NAME,
+                "default": RUN_CONST.DEFAULT_TOPIC_NAME,
                 "help": "Name of the topic to produce to",
             },
         ],
         "n_threads": [
             "optional",
             {
                 "default": RUN_CONST.DEFAULT_N_THREADS,
                 "type": positive_int,
                 "help": "Maximum number of threads to use",
             },
         ],
         "n_consumer_threads": [
             "optional",
             {
-                "default": RUN_OPT_CONST.N_DEFAULT_DOWNLOAD_THREADS,
+                "default": RUN_CONST.N_DEFAULT_DOWNLOAD_THREADS,
                 "type": positive_int,
                 "help": "Number of consumer threads to use",
             },
         ],
         "n_producer_threads": [
             "optional",
             {
-                "default": RUN_OPT_CONST.N_DEFAULT_UPLOAD_THREADS,
+                "default": RUN_CONST.N_DEFAULT_UPLOAD_THREADS,
                 "type": positive_int,
                 "help": "Number of producer threads to use",
             },
         ],
         "upload_regex": [
             "optional",
             {
-                "default": RUN_OPT_CONST.DEFAULT_UPLOAD_REGEX,
+                "default": RUN_CONST.DEFAULT_UPLOAD_REGEX,
                 "type": re.compile,
                 "help": "Only files with paths matching this regular expression will be uploaded",
             },
         ],
         "download_regex": [
             "optional",
             {
                 "type": re.compile,
                 "help": "Only files with paths matching this regular expression will be uploaded",
             },
         ],
         "chunk_size": [
             "optional",
             {
-                "default": RUN_OPT_CONST.DEFAULT_CHUNK_SIZE,
+                "default": RUN_CONST.DEFAULT_CHUNK_SIZE,
                 "type": int_power_of_two,
                 "help": (
                     "Max size (in bytes) of chunks into which files should be broken "
                     "as they are uploaded"
                 ),
             },
         ],
         "queue_max_size": [
             "optional",
             {
-                "default": RUN_OPT_CONST.DEFAULT_MAX_UPLOAD_QUEUE_MEGABYTES,
+                "default": RUN_CONST.DEFAULT_MAX_UPLOAD_QUEUE_MEGABYTES,
                 "type": int,
                 "help": (
                     "Maximum allowed size in MB of the internal upload queue. "
                     "Use to adjust RAM usage if necessary."
                 ),
             },
         ],
```

### Comparing `openmsistream-1.5.0/openmsistream/utilities/config_file_parser.py` & `openmsistream-1.5.1/openmsistream/utilities/config_file_parser.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.0/openmsistream/utilities/controlled_process.py` & `openmsistream-1.5.1/openmsistream/utilities/controlled_process.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.0/openmsistream/utilities/controlled_process_multi_threaded.py` & `openmsistream-1.5.1/openmsistream/utilities/controlled_process_multi_threaded.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.0/openmsistream/utilities/controlled_process_single_thread.py` & `openmsistream-1.5.1/openmsistream/utilities/controlled_process_single_thread.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.0/openmsistream/utilities/dataclass_table.py` & `openmsistream-1.5.1/openmsistream/utilities/dataclass_table.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.0/openmsistream/utilities/exception_tracking_thread.py` & `openmsistream-1.5.1/openmsistream/utilities/exception_tracking_thread.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.0/openmsistream/utilities/has_arguments.py` & `openmsistream-1.5.1/openmsistream/utilities/has_arguments.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.0/openmsistream/utilities/logging.py` & `openmsistream-1.5.1/openmsistream/utilities/logging.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.0/openmsistream/utilities/misc.py` & `openmsistream-1.5.1/openmsistream/utilities/misc.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.0/openmsistream/utilities/provision_wrapper.py` & `openmsistream-1.5.1/openmsistream/utilities/provision_wrapper.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.0/openmsistream/utilities/runnable.py` & `openmsistream-1.5.1/openmsistream/utilities/runnable.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.0/openmsistream.egg-info/PKG-INFO` & `openmsistream-1.5.1/openmsistream.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: openmsistream
-Version: 1.5.0
+Version: 1.5.1
 Summary: Python applications for materials data streaming using Apache Kafka. Developed for Open MSI (NSF DMREF award #1921959)
 Home-page: https://github.com/openmsi/openmsistream
 Author: OpenMSIStream
 Author-email: openmsistream@gmail.com
 License: GNU GPLv3
-Download-URL: https://github.com/openmsi/openmsistream/archive/refs/tags/v1.5.0.tar.gz
+Download-URL: https://github.com/openmsi/openmsistream/archive/refs/tags/v1.5.1.tar.gz
 Keywords: data_streaming,stream_processing,apache_kafka,materials,data_science
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7,<3.10
```

### Comparing `openmsistream-1.5.0/openmsistream.egg-info/SOURCES.txt` & `openmsistream-1.5.1/openmsistream.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.0/openmsistream.egg-info/entry_points.txt` & `openmsistream-1.5.1/openmsistream.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.0/setup.py` & `openmsistream-1.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # imports
 import setuptools
 
 # version tag
-version = "1.5.0"
+version = "1.5.1"
 
 long_description = ""
 with open("README.md", "r") as readme:
     for il, line in enumerate(readme.readlines(), start=1):
         if il >= 18:
             long_description += line
```

