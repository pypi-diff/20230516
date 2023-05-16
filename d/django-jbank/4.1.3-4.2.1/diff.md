# Comparing `tmp/django-jbank-4.1.3.tar.gz` & `tmp/django-jbank-4.2.1.tar.gz`

## Comparing `django-jbank-4.1.3.tar` & `django-jbank-4.2.1.tar`

### file list

```diff
@@ -1,366 +1,366 @@
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-05-03 19:07:13.000000 django-jbank-4.1.3/
--rw-rw-r--   0 jani      (1000) jani      (1000)      931 2023-03-27 06:59:59.000000 django-jbank-4.1.3/pyproject.toml
--rw-rw-r--   0 jani      (1000) jani      (1000)     1064 2023-04-05 11:04:17.000000 django-jbank-4.1.3/README.md
--rw-rw-r--   0 jani      (1000) jani      (1000)       38 2023-05-03 19:07:09.000000 django-jbank-4.1.3/setup.cfg
--rw-rw-r--   0 jani      (1000) jani      (1000)     1082 2020-05-26 21:27:46.000000 django-jbank-4.1.3/LICENSE.txt
--rw-rw-r--   0 jani      (1000) jani      (1000)     1310 2023-05-03 19:07:09.000000 django-jbank-4.1.3/PKG-INFO
--rw-rw-r--   0 jani      (1000) jani      (1000)      256 2022-07-02 11:10:09.000000 django-jbank-4.1.3/requirements-dev.txt
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-05-03 19:07:09.000000 django-jbank-4.1.3/django_jbank.egg-info/
--rw-rw-r--   0 jani      (1000) jani      (1000)     1310 2023-05-03 19:07:01.000000 django-jbank-4.1.3/django_jbank.egg-info/PKG-INFO
--rw-rw-r--   0 jani      (1000) jani      (1000)      139 2023-05-03 19:07:01.000000 django-jbank-4.1.3/django_jbank.egg-info/requires.txt
--rw-rw-r--   0 jani      (1000) jani      (1000)        1 2023-05-03 19:07:01.000000 django-jbank-4.1.3/django_jbank.egg-info/dependency_links.txt
--rw-rw-r--   0 jani      (1000) jani      (1000)        1 2020-05-26 21:28:24.000000 django-jbank-4.1.3/django_jbank.egg-info/not-zip-safe
--rw-rw-r--   0 jani      (1000) jani      (1000)        6 2023-05-03 19:07:01.000000 django-jbank-4.1.3/django_jbank.egg-info/top_level.txt
--rw-rw-r--   0 jani      (1000) jani      (1000)   609127 2023-05-03 19:07:09.000000 django-jbank-4.1.3/django_jbank.egg-info/SOURCES.txt
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-05-03 19:07:09.000000 django-jbank-4.1.3/htmlcov/
--rw-rw-r--   0 jani      (1000) jani      (1000)    20396 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_2442641f6b49fa31_pain002_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)     3065 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jquery.hotkeys.js
--rw-rw-r--   0 jani      (1000) jani      (1000)     4577 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_apps_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    12795 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jquery.tablesorter.min.js
--rw-rw-r--   0 jani      (1000) jani      (1000)    20010 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_wsedi_export_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    54955 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_wsedi_download_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    22199 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_management_commands_wsedi_import_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)   463697 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_2442641f6b49fa31_admin_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    13564 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_parse_saldo_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)     2756 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank___init___py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    22245 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_management_commands_wsedi_exec_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    26018 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_parse_xm_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    42120 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_svm_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)   152313 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_sepa_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)   106957 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_helpers_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    77825 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_2442641f6b49fa31_wsedi_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)     9556 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/manage_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)     4542 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3___init___py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    22558 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/index.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    12322 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_xmlsec1_examples_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    11994 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_management_commands_parse_aeb43_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)     6940 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_management_commands_test_to_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)     2533 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_management___init___py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)   155711 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_2442641f6b49fa31_sepa_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    14174 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_2442641f6b49fa31_x509_helpers_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)     4582 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_d1b4fb5372fdacae___init___py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    22201 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_wspki_exec_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)     2543 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_templates_jbank___init___py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    29198 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_parse_to_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    21506 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_test_pain001_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)     2543 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_templates_admin___init___py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    29235 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_parse_xp_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)     2575 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_templates_admin_jbank_statement___init___py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    22185 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_reparse_to_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    30153 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_make_x509_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    82193 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_wsedi_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)      731 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jquery.ba-throttle-debounce.min.js
--rw-rw-r--   0 jani      (1000) jani      (1000)    15825 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_test_payment_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    10869 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_test_xp_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)     9846 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_files_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    39776 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_management_commands_make_pain001_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    24060 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_management_commands_parse_ecb_rates_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)     4683 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_2442641f6b49fa31___init___py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    45984 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_csr_helpers_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    93373 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_tests_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    53341 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_management_commands_wsedi_download_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)   378796 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_2442641f6b49fa31_models_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    93109 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_2442641f6b49fa31_parsers_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)   348054 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_models_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    47349 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_2442641f6b49fa31_csr_helpers_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    10339 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_management_commands_xmlsec1_examples_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    60842 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_parsers_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)   102362 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_2442641f6b49fa31_svm_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)     1502 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jquery.isonscreen.js
--rw-rw-r--   0 jani      (1000) jani      (1000)     8921 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_test_to_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)     2551 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_management_commands___init___py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    17350 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_management_commands_wspki_exec_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    11825 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_2442641f6b49fa31_files_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    42348 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_management_commands_wsedi_upload_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    28422 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_management_commands_parse_svm_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)   111921 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_2442641f6b49fa31_tito_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    24166 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_wsedi_import_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    41408 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_make_pain001_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)   132280 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_wspki_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)     4538 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_9798a7910e9d8d38___init___py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)     9004 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/keybd_closed.png
--rw-rw-r--   0 jani      (1000) jani      (1000)     1732 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/favicon_32.png
--rw-rw-r--   0 jani      (1000) jani      (1000)    15523 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_test_app_req_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    61488 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_2442641f6b49fa31_aeb43_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)   190062 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_2442641f6b49fa31_camt_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)     7786 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_management_commands_parse_x509_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    13596 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_parse_ra_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    52753 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_management_commands_parse_xt_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    20188 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_management_commands_reparse_to_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)     9776 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_2442641f6b49fa31_services_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    54239 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_parse_xt_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)     9769 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_parse_x509_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)     2505 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_views_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)     2531 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_templates___init___py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    11551 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_ecb_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    11954 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_x509_helpers_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)   137549 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jquery.min.js
--rw-rw-r--   0 jani      (1000) jani      (1000)    17982 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_management_commands_wsedi_export_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)     4504 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_f6e593a656d19133___init___py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    44748 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_wsedi_upload_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    27154 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_management_commands_parse_to_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    13619 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_parse_euribor_rates_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)     4514 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_de1059d8df3ce8de___init___py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    35254 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_2442641f6b49fa31_helpers_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    58311 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_aeb43_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)     8924 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_test_svm_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)   140727 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_2442641f6b49fa31_wspki_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)     4474 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_2442641f6b49fa31_views_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)     4526 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_367ac34b948d641d___init___py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    29945 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_parse_svm_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    13834 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_management_commands_test_payment_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    23928 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_wsedi_exec_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)     6935 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_management_commands_test_svm_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    18044 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_2442641f6b49fa31_euribor_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)     2599 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_templates_admin_jbank_referencepaymentbatch___init___py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    27546 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_management_commands_parse_xp_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)     2555 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_templates_admin_jbank___init___py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)     6546 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_2442641f6b49fa31_apps_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)   112238 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_tito_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    20650 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/coverage_html.js
--rw-rw-r--   0 jani      (1000) jani      (1000)    12429 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/style.css
--rw-rw-r--   0 jani      (1000) jani      (1000)    13993 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_parse_aeb43_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    13624 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_management_commands_test_app_req_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)     9003 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/keybd_open.png
--rw-rw-r--   0 jani      (1000) jani      (1000)    19907 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_management_commands_test_pain001_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)     4520 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_c6b51be18eb0ec86___init___py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)     4558 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_d4f8c6455716e7bb___init___py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    24383 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_make_parse_format_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)   105315 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_2442641f6b49fa31_tests_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    13538 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_2442641f6b49fa31_ecb_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    20842 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_reparse_svm_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)   139457 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_camt_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    22274 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_management_commands_make_parse_format_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    25502 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_parse_ecb_rates_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)   386954 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_admin_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    28146 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_management_commands_make_x509_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)     8876 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_management_commands_test_xp_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    18793 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_management_commands_reparse_svm_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)      247 2020-05-27 18:47:15.000000 django-jbank-4.1.3/mypy.ini
--rw-rw-r--   0 jani      (1000) jani      (1000)      287 2020-09-02 13:51:57.000000 django-jbank-4.1.3/MANIFEST.in
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-05-03 19:07:09.000000 django-jbank-4.1.3/data/
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-05-03 19:07:09.000000 django-jbank-4.1.3/data/pain001/
--rw-rw-r--   0 jani      (1000) jani      (1000)     4044 2020-05-21 16:43:43.000000 django-jbank-4.1.3/data/pain001/pain.001.001.03.xml
--rw-rw-r--   0 jani      (1000) jani      (1000)    91224 2020-05-21 16:43:43.000000 django-jbank-4.1.3/data/ecb-rates-2019-08-15.xml
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-05-03 19:07:09.000000 django-jbank-4.1.3/data/pki/
--rw-rw-r--   0 jani      (1000) jani      (1000)    10099 2020-07-18 04:38:59.000000 django-jbank-4.1.3/data/pki/GetBankCertificate-res.xml
--rw-rw-r--   0 jani      (1000) jani      (1000)      638 2020-07-20 22:19:28.000000 django-jbank-4.1.3/data/pki/CreateCertificate-res.xml
--rw-rw-r--   0 jani      (1000) jani      (1000)     1547 2021-07-06 23:33:19.000000 django-jbank-4.1.3/data/x509-data.xml
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-05-03 19:07:09.000000 django-jbank-4.1.3/data/finvoice/
--rw-rw-r--   0 jani      (1000) jani      (1000)     5362 2020-05-21 16:43:43.000000 django-jbank-4.1.3/data/finvoice/xsd-test.xml
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-05-03 19:07:09.000000 django-jbank-4.1.3/data/xm/
--rw-rw-r--   0 jani      (1000) jani      (1000)     6994 2023-03-27 06:59:59.000000 django-jbank-4.1.3/data/xm/camt_054_credit_notoification_example_finland.xml
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-05-03 19:07:09.000000 django-jbank-4.1.3/data/x509/
--rw-rw-r--   0 jani      (1000) jani      (1000)     1561 2022-07-21 16:32:20.000000 django-jbank-4.1.3/data/x509/x509data.xml
--rw-rw-r--   0 jani      (1000) jani      (1000)     1486 2020-05-21 16:43:43.000000 django-jbank-4.1.3/data/x509/appreq.xml
--rw-rw-r--   0 jani      (1000) jani      (1000)      139 2023-02-14 22:34:42.000000 django-jbank-4.1.3/requirements.txt
--rw-rw-r--   0 jani      (1000) jani      (1000)      867 2023-05-03 19:06:59.000000 django-jbank-4.1.3/setup.py
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-05-03 19:07:09.000000 django-jbank-4.1.3/jbank/
--rw-rw-r--   0 jani      (1000) jani      (1000)     3440 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/helpers.py
--rw-rw-r--   0 jani      (1000) jani      (1000)    11013 2023-05-03 19:06:59.000000 django-jbank-4.1.3/jbank/wsedi.py
--rw-rw-r--   0 jani      (1000) jani      (1000)    44747 2023-05-03 19:06:59.000000 django-jbank-4.1.3/jbank/models.py
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-05-03 19:07:09.000000 django-jbank-4.1.3/jbank/management/
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-05-03 19:07:09.000000 django-jbank-4.1.3/jbank/management/commands/
--rw-rw-r--   0 jani      (1000) jani      (1000)     1014 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/management/commands/parse_ra.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      505 2021-07-06 21:13:32.000000 django-jbank-4.1.3/jbank/management/commands/test_to.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     3193 2021-07-06 21:13:32.000000 django-jbank-4.1.3/jbank/management/commands/make_x509.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      498 2021-07-06 21:13:32.000000 django-jbank-4.1.3/jbank/management/commands/parse_x509.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     1287 2021-09-14 00:17:15.000000 django-jbank-4.1.3/jbank/management/commands/test_app_req.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     3610 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/management/commands/parse_svm.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      859 2021-07-06 21:13:32.000000 django-jbank-4.1.3/jbank/management/commands/xmlsec1_examples.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     2338 2023-05-03 18:51:50.000000 django-jbank-4.1.3/jbank/management/commands/wsedi_exec.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     1195 2021-07-06 21:13:32.000000 django-jbank-4.1.3/jbank/management/commands/test_payment.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     2146 2021-09-09 00:31:49.000000 django-jbank-4.1.3/jbank/management/commands/wsedi_import.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     2557 2023-04-05 11:04:17.000000 django-jbank-4.1.3/jbank/management/commands/wspki_exec.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      498 2021-07-06 21:13:32.000000 django-jbank-4.1.3/jbank/management/commands/test_svm.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     3373 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/management/commands/parse_to.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     7308 2023-05-03 19:06:59.000000 django-jbank-4.1.3/jbank/management/commands/parse_xt.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     2085 2021-09-14 00:17:15.000000 django-jbank-4.1.3/jbank/management/commands/test_pain001.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     7591 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/management/commands/wsedi_download.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     2935 2023-05-03 19:06:59.000000 django-jbank-4.1.3/jbank/management/commands/parse_xm.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     2286 2021-09-09 00:31:49.000000 django-jbank-4.1.3/jbank/management/commands/reparse_svm.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     1002 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/management/commands/parse_saldo.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     2237 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/management/commands/make_parse_format.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     2690 2021-09-14 00:17:15.000000 django-jbank-4.1.3/jbank/management/commands/parse_ecb_rates.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     3091 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/management/commands/parse_xp.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      676 2021-07-06 21:13:32.000000 django-jbank-4.1.3/jbank/management/commands/test_xp.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     4589 2022-12-09 16:27:19.000000 django-jbank-4.1.3/jbank/management/commands/make_pain001.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     2450 2021-07-06 21:13:32.000000 django-jbank-4.1.3/jbank/management/commands/reparse_to.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     1190 2021-09-14 00:17:15.000000 django-jbank-4.1.3/jbank/management/commands/parse_euribor_rates.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     5375 2022-12-09 16:27:19.000000 django-jbank-4.1.3/jbank/management/commands/wsedi_upload.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     1541 2021-09-09 00:31:49.000000 django-jbank-4.1.3/jbank/management/commands/wsedi_export.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     1102 2021-07-06 21:13:32.000000 django-jbank-4.1.3/jbank/management/commands/parse_aeb43.py
--rw-rw-r--   0 jani      (1000) jani      (1000)        0 2020-05-21 16:43:43.000000 django-jbank-4.1.3/jbank/management/commands/__init__.py
--rw-rw-r--   0 jani      (1000) jani      (1000)        0 2020-05-21 16:43:43.000000 django-jbank-4.1.3/jbank/management/__init__.py
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-05-03 19:07:09.000000 django-jbank-4.1.3/jbank/migrations/
--rw-rw-r--   0 jani      (1000) jani      (1000)     1074 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0008_auto_20210512_2208.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      754 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0016_alter_payoutstatus_timestamp.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      760 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0004_statementfile.py
--rw-rw-r--   0 jani      (1000) jani      (1000)    57170 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0001_squashed_0071_wsediconnection_ca_cert_file.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      655 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0026_auto_20181205_0034.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     1735 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0034_auto_20190815_2059.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      886 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0007_auto_20171102_2351.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     1333 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0019_auto_20180209_0437.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      648 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0013_auto_20180126_0909.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      591 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0023_remove_accountbalance_connection_accountbalance_bic.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      428 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0004_refund_attachment.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     1192 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0015_auto_20180208_0643.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      422 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0068_auto_20200717_2327.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      580 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0055_auto_20191130_2011.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      461 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0070_wsediconnection_bank_signing_cert_file.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      443 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0020_payout_due_date.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      515 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0069_auto_20200717_2333.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      406 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0047_wsedisoapcall_error.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      347 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0050_remove_wsedisoapcall_payout.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      703 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0041_auto_20191127_0559.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      576 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0039_auto_20191127_0156.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      748 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0037_auto_20191127_0132.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     1672 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0008_auto_20171103_0007.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     1019 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0024_auto_20180425_1704.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      577 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0048_wsediconnection_soap_endpoint.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      464 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0028_auto_20190327_1830.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      480 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0066_wsediconnection_pin.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      667 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0018_auto_20180208_1130.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      482 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0053_wsediconnection_target_identifier.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      551 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0005_statementfile_created.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      643 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0025_auto_20181101_1430.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      703 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0027_auto_20190304_1913.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     1196 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0036_wsediconnection.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      439 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0015_ps_timestamp_fill.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      443 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0038_auto_20191127_0145.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     3784 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0028_referencepaymentrecord_creditor_bank_bic_and_more.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      523 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0010_statementrecorddetail_creditor_account_scheme.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     2493 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0011_auto_20180126_0851.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      487 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0045_wsediconnection_receiver_identifier.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      468 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0071_wsediconnection_ca_cert_file.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      623 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0051_payout_connection.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      967 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0018_alter_referencepaymentbatch_currency_identifier_and_more.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      638 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0003_statement_account.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     1096 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0007_auto_20210507_2122.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     1930 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0012_auto_20180126_0858.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      412 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0003_auto_20200902_1354.py
--rw-rw-r--   0 jani      (1000) jani      (1000)    15229 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0001_initial.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     1175 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0013_euriborrate.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      934 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0019_alter_payout_state.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      486 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0010_auto_20171226_1013.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      482 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0017_alter_statementrecord_name.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      418 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0059_auto_20200324_0234.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      514 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0030_alter_referencepaymentrecord_remittance_info.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      494 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0049_wsediconnection_sender_identifier.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      450 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0014_payoutstatus_timestamp.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      424 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0046_auto_20191128_2242.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      711 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0022_accountbalance_connection.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      462 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0065_wsediconnection_bank_root_cert_file.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     1520 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0020_accountbalance.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      405 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0023_auto_20180419_1316.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      748 2023-04-05 11:04:17.000000 django-jbank-4.1.3/jbank/migrations/0031_wsediconnection_old_encryption_key_file_and_more.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      687 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0021_auto_20180209_0935.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      500 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0009_referencepaymentbatchfile_cached_total_amount.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      441 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0057_wsediconnection_enabled.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     2335 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0043_wsedisoapcall.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      707 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0006_auto_20210318_2130.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      467 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0042_wsediconnection_bank_encryption_cert_file.py
--rw-rw-r--   0 jani      (1000) jani      (1000)    11060 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0029_auto_20190727_1352.py
--rw-rw-r--   0 jani      (1000) jani      (1000)    27144 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0064_auto_20200629_0344.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      692 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0062_auto_20200415_2300.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      498 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0005_auto_20201203_2308.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      670 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0061_auto_20200325_2204.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      698 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0060_auto_20200325_1906.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      462 2023-05-03 19:06:59.000000 django-jbank-4.1.3/jbank/migrations/0033_alter_statement_begin_date.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     1451 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0026_referencepaymentbatch_identifier_and_more.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      455 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0063_auto_20200608_1827.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      520 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0029_alter_referencepaymentrecord_remittance_info.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      488 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0033_auto_20190801_2121.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      665 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0052_auto_20191130_1927.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     1006 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0024_referencepaymentbatchfile_additional_info_and_more.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      525 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0009_auto_20171107_1847.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      491 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0058_auto_20200316_1949.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     3164 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0016_auto_20180208_0724.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      463 2023-04-05 11:04:17.000000 django-jbank-4.1.3/jbank/migrations/0032_wsediconnection_use_sha256.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      753 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0027_referencepaymentrecord_value_date_and_more.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      665 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0006_auto_20171102_2341.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      433 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0021_alter_accountbalance_balance.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      452 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0044_auto_20191128_2231.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      523 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0011_referencepaymentbatch_cached_total_amount.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      706 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0017_payoutparty_payouts_account.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      426 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0056_wsediconnection_debug_commands.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     3213 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0002_auto_20171031_0356.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      478 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0030_auto_20190727_1633.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      713 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0012_alter_referencepaymentrecord_delivery_method.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      434 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0067_wsediconnection_pki_endpoint.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     4229 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0014_payout_payoutstatus.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      534 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0025_auto_20230325_1014.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      488 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0035_auto_20190815_2137.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      449 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0040_wsediconnection_signing_key_file.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     2031 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0002_auto_20200817_2217.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      467 2023-05-03 19:06:59.000000 django-jbank-4.1.3/jbank/migrations/0034_wsediconnection_use_wsse_timestamp.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      460 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0054_wsediconnection_environment.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     1621 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0031_auto_20190727_1639.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      479 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0032_auto_20190727_1655.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      456 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0022_auto_20180411_1814.py
--rw-rw-r--   0 jani      (1000) jani      (1000)        0 2020-05-21 16:43:43.000000 django-jbank-4.1.3/jbank/migrations/__init__.py
--rw-rw-r--   0 jani      (1000) jani      (1000)    19043 2023-05-03 19:06:59.000000 django-jbank-4.1.3/jbank/wspki.py
--rw-rw-r--   0 jani      (1000) jani      (1000)       27 2020-05-26 21:27:46.000000 django-jbank-4.1.3/jbank/py.typed
--rw-rw-r--   0 jani      (1000) jani      (1000)    11505 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/svm.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      716 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/services.py
--rw-rw-r--   0 jani      (1000) jani      (1000)    23260 2023-05-03 19:06:59.000000 django-jbank-4.1.3/jbank/camt.py
--rw-rw-r--   0 jani      (1000) jani      (1000)    26191 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/tests.py
--rw-rw-r--   0 jani      (1000) jani      (1000)    52672 2023-05-03 19:06:59.000000 django-jbank-4.1.3/jbank/admin.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     6524 2021-07-06 23:33:19.000000 django-jbank-4.1.3/jbank/aeb43.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     1257 2021-07-06 21:13:32.000000 django-jbank-4.1.3/jbank/ecb.py
--rw-rw-r--   0 jani      (1000) jani      (1000)    22601 2021-09-09 00:31:49.000000 django-jbank-4.1.3/jbank/sepa.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     1189 2021-12-11 15:04:51.000000 django-jbank-4.1.3/jbank/x509_helpers.py
--rw-rw-r--   0 jani      (1000) jani      (1000)    10244 2023-05-03 19:06:59.000000 django-jbank-4.1.3/jbank/parsers.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     5273 2023-02-26 05:09:42.000000 django-jbank-4.1.3/jbank/csr_helpers.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      235 2021-07-06 21:13:32.000000 django-jbank-4.1.3/jbank/apps.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      819 2021-07-06 21:13:32.000000 django-jbank-4.1.3/jbank/files.py
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-05-03 19:07:09.000000 django-jbank-4.1.3/jbank/templates/
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-05-03 19:07:09.000000 django-jbank-4.1.3/jbank/templates/admin/
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-05-03 19:07:09.000000 django-jbank-4.1.3/jbank/templates/admin/jbank/
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-05-03 19:07:09.000000 django-jbank-4.1.3/jbank/templates/admin/jbank/referencepaymentbatch/
--rw-rw-r--   0 jani      (1000) jani      (1000)      793 2020-05-21 16:43:43.000000 django-jbank-4.1.3/jbank/templates/admin/jbank/referencepaymentbatch/change_form.html
--rw-rw-r--   0 jani      (1000) jani      (1000)        0 2020-05-21 16:43:43.000000 django-jbank-4.1.3/jbank/templates/admin/jbank/referencepaymentbatch/__init__.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      690 2020-05-21 16:43:43.000000 django-jbank-4.1.3/jbank/templates/admin/jbank/mark_as_manually_settled.html
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-05-03 19:07:09.000000 django-jbank-4.1.3/jbank/templates/admin/jbank/statement/
--rw-rw-r--   0 jani      (1000) jani      (1000)      782 2020-05-21 16:43:43.000000 django-jbank-4.1.3/jbank/templates/admin/jbank/statement/change_form.html
--rw-rw-r--   0 jani      (1000) jani      (1000)        0 2020-05-21 16:43:43.000000 django-jbank-4.1.3/jbank/templates/admin/jbank/statement/__init__.py
--rw-rw-r--   0 jani      (1000) jani      (1000)        0 2020-05-21 16:43:43.000000 django-jbank-4.1.3/jbank/templates/admin/jbank/__init__.py
--rw-rw-r--   0 jani      (1000) jani      (1000)        0 2020-05-21 16:43:43.000000 django-jbank-4.1.3/jbank/templates/admin/__init__.py
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-05-03 19:07:09.000000 django-jbank-4.1.3/jbank/templates/jbank/
--rw-rw-r--   0 jani      (1000) jani      (1000)     2041 2021-12-23 17:01:04.000000 django-jbank-4.1.3/jbank/templates/jbank/pki_certificate_status_request_template.xml
--rw-rw-r--   0 jani      (1000) jani      (1000)      962 2021-12-23 17:01:04.000000 django-jbank-4.1.3/jbank/templates/jbank/pki_create_certificate_request_template.xml
--rw-rw-r--   0 jani      (1000) jani      (1000)      876 2020-05-21 16:43:43.000000 django-jbank-4.1.3/jbank/templates/jbank/soap_template.xml
--rw-rw-r--   0 jani      (1000) jani      (1000)      562 2021-07-06 21:13:32.000000 django-jbank-4.1.3/jbank/templates/jbank/pki_get_certificate_soap_template.xml
--rw-rw-r--   0 jani      (1000) jani      (1000)     2079 2022-01-09 22:11:13.000000 django-jbank-4.1.3/jbank/templates/jbank/pki_renew_certificate_request_template.xml
--rw-rw-r--   0 jani      (1000) jani      (1000)      568 2021-12-23 17:01:04.000000 django-jbank-4.1.3/jbank/templates/jbank/pki_get_certificate_request_template.xml
--rw-rw-r--   0 jani      (1000) jani      (1000)     2223 2023-04-05 11:04:17.000000 django-jbank-4.1.3/jbank/templates/jbank/application_request_template-sha256.xml
--rw-rw-r--   0 jani      (1000) jani      (1000)     1686 2023-04-05 11:04:17.000000 django-jbank-4.1.3/jbank/templates/jbank/pki_get_certificate_renew_request_template-sha256.xml
--rw-rw-r--   0 jani      (1000) jani      (1000)     2087 2023-04-05 11:04:17.000000 django-jbank-4.1.3/jbank/templates/jbank/pki_renew_certificate_request_template-sha256.xml
--rw-rw-r--   0 jani      (1000) jani      (1000)     2215 2020-05-21 16:43:43.000000 django-jbank-4.1.3/jbank/templates/jbank/application_request_template.xml
--rw-rw-r--   0 jani      (1000) jani      (1000)      758 2020-05-21 16:43:43.000000 django-jbank-4.1.3/jbank/templates/jbank/encryption_template.xml
--rw-rw-r--   0 jani      (1000) jani      (1000)     5352 2023-04-05 11:04:17.000000 django-jbank-4.1.3/jbank/templates/jbank/enveloping-sha256-rsa-sha256.xml
--rw-rw-r--   0 jani      (1000) jani      (1000)     1678 2021-12-23 17:01:04.000000 django-jbank-4.1.3/jbank/templates/jbank/pki_get_certificate_renew_request_template.xml
--rw-rw-r--   0 jani      (1000) jani      (1000)      911 2021-12-23 17:01:04.000000 django-jbank-4.1.3/jbank/templates/jbank/pki_soap_template.xml
--rw-rw-r--   0 jani      (1000) jani      (1000)        0 2020-05-21 16:43:43.000000 django-jbank-4.1.3/jbank/templates/jbank/__init__.py
--rw-rw-r--   0 jani      (1000) jani      (1000)        0 2020-05-21 16:43:43.000000 django-jbank-4.1.3/jbank/templates/__init__.py
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-05-03 19:07:09.000000 django-jbank-4.1.3/jbank/locale/
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-05-03 19:07:09.000000 django-jbank-4.1.3/jbank/locale/fi/
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-05-03 19:07:09.000000 django-jbank-4.1.3/jbank/locale/fi/LC_MESSAGES/
--rw-rw-r--   0 jani      (1000) jani      (1000)    15825 2023-02-24 09:03:24.000000 django-jbank-4.1.3/jbank/locale/fi/LC_MESSAGES/django.mo
--rw-rw-r--   0 jani      (1000) jani      (1000)    26153 2023-02-24 09:03:24.000000 django-jbank-4.1.3/jbank/locale/fi/LC_MESSAGES/django.po
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-05-03 19:07:09.000000 django-jbank-4.1.3/jbank/locale/en/
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-05-03 19:07:09.000000 django-jbank-4.1.3/jbank/locale/en/LC_MESSAGES/
--rw-rw-r--   0 jani      (1000) jani      (1000)     1102 2023-02-24 08:59:20.000000 django-jbank-4.1.3/jbank/locale/en/LC_MESSAGES/django.mo
--rw-rw-r--   0 jani      (1000) jani      (1000)    21019 2023-02-24 09:03:24.000000 django-jbank-4.1.3/jbank/locale/en/LC_MESSAGES/django.po
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-05-03 19:07:09.000000 django-jbank-4.1.3/jbank/xmlsec1-examples/
--rw-rw-r--   0 jani      (1000) jani      (1000)     1058 2023-04-05 11:04:17.000000 django-jbank-4.1.3/jbank/xmlsec1-examples/Makefile
--rw-rw-r--   0 jani      (1000) jani      (1000)    10308 2020-05-21 16:43:43.000000 django-jbank-4.1.3/jbank/xmlsec1-examples/encrypt3.c
--rw-rw-r--   0 jani      (1000) jani      (1000)     9710 2020-05-21 16:43:43.000000 django-jbank-4.1.3/jbank/xmlsec1-examples/sign3.c
--rw-rw-r--   0 jani      (1000) jani      (1000)     7127 2020-05-21 16:43:43.000000 django-jbank-4.1.3/jbank/xmlsec1-examples/decrypt3.c
--rw-rw-r--   0 jani      (1000) jani      (1000)     7088 2020-05-21 16:43:43.000000 django-jbank-4.1.3/jbank/xmlsec1-examples/verify3.c
--rw-rw-r--   0 jani      (1000) jani      (1000)     9718 2023-04-05 11:04:17.000000 django-jbank-4.1.3/jbank/xmlsec1-examples/sign3-sha256.c
--rw-rw-r--   0 jani      (1000) jani      (1000)     1582 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/pain002.py
--rw-rw-r--   0 jani      (1000) jani      (1000)        0 2020-05-21 16:43:43.000000 django-jbank-4.1.3/jbank/views.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     1562 2023-05-03 19:06:59.000000 django-jbank-4.1.3/jbank/euribor.py
--rw-rw-r--   0 jani      (1000) jani      (1000)    12672 2021-08-11 21:48:35.000000 django-jbank-4.1.3/jbank/tito.py
--rw-rw-r--   0 jani      (1000) jani      (1000)       46 2021-07-06 21:13:32.000000 django-jbank-4.1.3/jbank/__init__.py
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-05-16 17:40:43.000000 django-jbank-4.2.1/
+-rw-rw-r--   0 jani      (1000) jani      (1000)      931 2023-03-27 06:59:59.000000 django-jbank-4.2.1/pyproject.toml
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1064 2023-05-16 17:40:29.000000 django-jbank-4.2.1/README.md
+-rw-rw-r--   0 jani      (1000) jani      (1000)       38 2023-05-16 17:40:39.000000 django-jbank-4.2.1/setup.cfg
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1082 2020-05-26 21:27:46.000000 django-jbank-4.2.1/LICENSE.txt
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1310 2023-05-16 17:40:39.000000 django-jbank-4.2.1/PKG-INFO
+-rw-rw-r--   0 jani      (1000) jani      (1000)      256 2022-07-02 11:10:09.000000 django-jbank-4.2.1/requirements-dev.txt
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-05-16 17:40:39.000000 django-jbank-4.2.1/django_jbank.egg-info/
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1310 2023-05-16 17:40:31.000000 django-jbank-4.2.1/django_jbank.egg-info/PKG-INFO
+-rw-rw-r--   0 jani      (1000) jani      (1000)      139 2023-05-16 17:40:31.000000 django-jbank-4.2.1/django_jbank.egg-info/requires.txt
+-rw-rw-r--   0 jani      (1000) jani      (1000)        1 2023-05-16 17:40:31.000000 django-jbank-4.2.1/django_jbank.egg-info/dependency_links.txt
+-rw-rw-r--   0 jani      (1000) jani      (1000)        1 2020-05-26 21:28:24.000000 django-jbank-4.2.1/django_jbank.egg-info/not-zip-safe
+-rw-rw-r--   0 jani      (1000) jani      (1000)        6 2023-05-16 17:40:31.000000 django-jbank-4.2.1/django_jbank.egg-info/top_level.txt
+-rw-rw-r--   0 jani      (1000) jani      (1000)   609735 2023-05-16 17:40:38.000000 django-jbank-4.2.1/django_jbank.egg-info/SOURCES.txt
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-05-16 17:40:39.000000 django-jbank-4.2.1/htmlcov/
+-rw-rw-r--   0 jani      (1000) jani      (1000)    20396 2023-03-27 06:36:02.000000 django-jbank-4.2.1/htmlcov/d_2442641f6b49fa31_pain002_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)     3065 2021-06-23 23:14:44.000000 django-jbank-4.2.1/htmlcov/jquery.hotkeys.js
+-rw-rw-r--   0 jani      (1000) jani      (1000)     4577 2021-06-23 23:14:44.000000 django-jbank-4.2.1/htmlcov/jbank_apps_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    12795 2021-06-23 23:14:44.000000 django-jbank-4.2.1/htmlcov/jquery.tablesorter.min.js
+-rw-rw-r--   0 jani      (1000) jani      (1000)    20010 2023-03-27 06:36:02.000000 django-jbank-4.2.1/htmlcov/d_d9f236fb879a91e3_wsedi_export_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    54955 2023-03-27 06:36:02.000000 django-jbank-4.2.1/htmlcov/d_d9f236fb879a91e3_wsedi_download_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    22199 2021-06-23 23:14:44.000000 django-jbank-4.2.1/htmlcov/jbank_management_commands_wsedi_import_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)   463697 2023-03-27 06:36:02.000000 django-jbank-4.2.1/htmlcov/d_2442641f6b49fa31_admin_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    13564 2023-03-27 06:36:02.000000 django-jbank-4.2.1/htmlcov/d_d9f236fb879a91e3_parse_saldo_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2756 2021-06-23 23:14:44.000000 django-jbank-4.2.1/htmlcov/jbank___init___py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    22245 2021-06-23 23:14:44.000000 django-jbank-4.2.1/htmlcov/jbank_management_commands_wsedi_exec_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    26018 2023-03-27 06:36:02.000000 django-jbank-4.2.1/htmlcov/d_d9f236fb879a91e3_parse_xm_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    42120 2021-06-23 23:14:44.000000 django-jbank-4.2.1/htmlcov/jbank_svm_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)   152313 2021-06-23 23:14:44.000000 django-jbank-4.2.1/htmlcov/jbank_sepa_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)   106957 2021-06-23 23:14:44.000000 django-jbank-4.2.1/htmlcov/jbank_helpers_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    77825 2023-03-27 06:36:02.000000 django-jbank-4.2.1/htmlcov/d_2442641f6b49fa31_wsedi_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)     9556 2023-03-27 06:36:02.000000 django-jbank-4.2.1/htmlcov/manage_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)     4542 2023-03-27 06:36:02.000000 django-jbank-4.2.1/htmlcov/d_d9f236fb879a91e3___init___py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    22558 2023-03-27 06:36:02.000000 django-jbank-4.2.1/htmlcov/index.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    12322 2023-03-27 06:36:02.000000 django-jbank-4.2.1/htmlcov/d_d9f236fb879a91e3_xmlsec1_examples_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    11994 2021-06-23 23:14:44.000000 django-jbank-4.2.1/htmlcov/jbank_management_commands_parse_aeb43_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)     6940 2021-06-23 23:14:44.000000 django-jbank-4.2.1/htmlcov/jbank_management_commands_test_to_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2533 2021-06-23 23:14:44.000000 django-jbank-4.2.1/htmlcov/jbank_management___init___py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)   155711 2023-03-27 06:36:02.000000 django-jbank-4.2.1/htmlcov/d_2442641f6b49fa31_sepa_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    14174 2023-03-27 06:36:02.000000 django-jbank-4.2.1/htmlcov/d_2442641f6b49fa31_x509_helpers_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)     4582 2023-03-27 06:36:02.000000 django-jbank-4.2.1/htmlcov/d_d1b4fb5372fdacae___init___py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    22201 2023-03-27 06:36:02.000000 django-jbank-4.2.1/htmlcov/d_d9f236fb879a91e3_wspki_exec_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2543 2021-06-23 23:14:44.000000 django-jbank-4.2.1/htmlcov/jbank_templates_jbank___init___py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    29198 2023-03-27 06:36:02.000000 django-jbank-4.2.1/htmlcov/d_d9f236fb879a91e3_parse_to_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    21506 2023-03-27 06:36:02.000000 django-jbank-4.2.1/htmlcov/d_d9f236fb879a91e3_test_pain001_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2543 2021-06-23 23:14:44.000000 django-jbank-4.2.1/htmlcov/jbank_templates_admin___init___py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    29235 2023-03-27 06:36:02.000000 django-jbank-4.2.1/htmlcov/d_d9f236fb879a91e3_parse_xp_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2575 2021-06-23 23:14:44.000000 django-jbank-4.2.1/htmlcov/jbank_templates_admin_jbank_statement___init___py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    22185 2023-03-27 06:36:02.000000 django-jbank-4.2.1/htmlcov/d_d9f236fb879a91e3_reparse_to_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    30153 2023-03-27 06:36:02.000000 django-jbank-4.2.1/htmlcov/d_d9f236fb879a91e3_make_x509_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    82193 2021-06-23 23:14:44.000000 django-jbank-4.2.1/htmlcov/jbank_wsedi_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)      731 2021-06-23 23:14:44.000000 django-jbank-4.2.1/htmlcov/jquery.ba-throttle-debounce.min.js
+-rw-rw-r--   0 jani      (1000) jani      (1000)    15825 2023-03-27 06:36:02.000000 django-jbank-4.2.1/htmlcov/d_d9f236fb879a91e3_test_payment_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    10869 2023-03-27 06:36:02.000000 django-jbank-4.2.1/htmlcov/d_d9f236fb879a91e3_test_xp_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)     9846 2021-06-23 23:14:44.000000 django-jbank-4.2.1/htmlcov/jbank_files_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    39776 2021-06-23 23:14:44.000000 django-jbank-4.2.1/htmlcov/jbank_management_commands_make_pain001_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    24060 2021-06-23 23:14:44.000000 django-jbank-4.2.1/htmlcov/jbank_management_commands_parse_ecb_rates_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)     4683 2023-03-27 06:36:02.000000 django-jbank-4.2.1/htmlcov/d_2442641f6b49fa31___init___py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    45984 2021-06-23 23:14:44.000000 django-jbank-4.2.1/htmlcov/jbank_csr_helpers_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    93373 2021-06-23 23:14:44.000000 django-jbank-4.2.1/htmlcov/jbank_tests_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    53341 2021-06-23 23:14:44.000000 django-jbank-4.2.1/htmlcov/jbank_management_commands_wsedi_download_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)   378796 2023-03-27 06:36:02.000000 django-jbank-4.2.1/htmlcov/d_2442641f6b49fa31_models_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    93109 2023-03-27 06:36:02.000000 django-jbank-4.2.1/htmlcov/d_2442641f6b49fa31_parsers_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)   348054 2021-06-23 23:14:44.000000 django-jbank-4.2.1/htmlcov/jbank_models_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    47349 2023-03-27 06:36:02.000000 django-jbank-4.2.1/htmlcov/d_2442641f6b49fa31_csr_helpers_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    10339 2021-06-23 23:14:44.000000 django-jbank-4.2.1/htmlcov/jbank_management_commands_xmlsec1_examples_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    60842 2021-06-23 23:14:44.000000 django-jbank-4.2.1/htmlcov/jbank_parsers_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)   102362 2023-03-27 06:36:02.000000 django-jbank-4.2.1/htmlcov/d_2442641f6b49fa31_svm_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1502 2021-06-23 23:14:44.000000 django-jbank-4.2.1/htmlcov/jquery.isonscreen.js
+-rw-rw-r--   0 jani      (1000) jani      (1000)     8921 2023-03-27 06:36:02.000000 django-jbank-4.2.1/htmlcov/d_d9f236fb879a91e3_test_to_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2551 2021-06-23 23:14:44.000000 django-jbank-4.2.1/htmlcov/jbank_management_commands___init___py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    17350 2021-06-23 23:14:44.000000 django-jbank-4.2.1/htmlcov/jbank_management_commands_wspki_exec_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    11825 2023-03-27 06:36:02.000000 django-jbank-4.2.1/htmlcov/d_2442641f6b49fa31_files_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    42348 2021-06-23 23:14:44.000000 django-jbank-4.2.1/htmlcov/jbank_management_commands_wsedi_upload_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    28422 2021-06-23 23:14:44.000000 django-jbank-4.2.1/htmlcov/jbank_management_commands_parse_svm_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)   111921 2023-03-27 06:36:02.000000 django-jbank-4.2.1/htmlcov/d_2442641f6b49fa31_tito_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    24166 2023-03-27 06:36:02.000000 django-jbank-4.2.1/htmlcov/d_d9f236fb879a91e3_wsedi_import_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    41408 2023-03-27 06:36:02.000000 django-jbank-4.2.1/htmlcov/d_d9f236fb879a91e3_make_pain001_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)   132280 2021-06-23 23:14:44.000000 django-jbank-4.2.1/htmlcov/jbank_wspki_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)     4538 2023-03-27 06:36:02.000000 django-jbank-4.2.1/htmlcov/d_9798a7910e9d8d38___init___py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)     9004 2023-03-27 06:36:02.000000 django-jbank-4.2.1/htmlcov/keybd_closed.png
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1732 2023-03-27 06:36:02.000000 django-jbank-4.2.1/htmlcov/favicon_32.png
+-rw-rw-r--   0 jani      (1000) jani      (1000)    15523 2023-03-27 06:36:02.000000 django-jbank-4.2.1/htmlcov/d_d9f236fb879a91e3_test_app_req_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    61488 2023-03-27 06:36:02.000000 django-jbank-4.2.1/htmlcov/d_2442641f6b49fa31_aeb43_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)   190062 2023-03-27 06:36:02.000000 django-jbank-4.2.1/htmlcov/d_2442641f6b49fa31_camt_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)     7786 2021-06-23 23:14:44.000000 django-jbank-4.2.1/htmlcov/jbank_management_commands_parse_x509_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    13596 2023-03-27 06:36:02.000000 django-jbank-4.2.1/htmlcov/d_d9f236fb879a91e3_parse_ra_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    52753 2021-06-23 23:14:44.000000 django-jbank-4.2.1/htmlcov/jbank_management_commands_parse_xt_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    20188 2021-06-23 23:14:44.000000 django-jbank-4.2.1/htmlcov/jbank_management_commands_reparse_to_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)     9776 2023-03-27 06:36:02.000000 django-jbank-4.2.1/htmlcov/d_2442641f6b49fa31_services_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    54239 2023-03-27 06:36:02.000000 django-jbank-4.2.1/htmlcov/d_d9f236fb879a91e3_parse_xt_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)     9769 2023-03-27 06:36:02.000000 django-jbank-4.2.1/htmlcov/d_d9f236fb879a91e3_parse_x509_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2505 2021-06-23 23:14:44.000000 django-jbank-4.2.1/htmlcov/jbank_views_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2531 2021-06-23 23:14:44.000000 django-jbank-4.2.1/htmlcov/jbank_templates___init___py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    11551 2021-06-23 23:14:44.000000 django-jbank-4.2.1/htmlcov/jbank_ecb_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    11954 2021-06-23 23:14:44.000000 django-jbank-4.2.1/htmlcov/jbank_x509_helpers_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)   137549 2021-06-23 23:14:44.000000 django-jbank-4.2.1/htmlcov/jquery.min.js
+-rw-rw-r--   0 jani      (1000) jani      (1000)    17982 2021-06-23 23:14:44.000000 django-jbank-4.2.1/htmlcov/jbank_management_commands_wsedi_export_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)     4504 2023-03-27 06:36:02.000000 django-jbank-4.2.1/htmlcov/d_f6e593a656d19133___init___py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    44748 2023-03-27 06:36:02.000000 django-jbank-4.2.1/htmlcov/d_d9f236fb879a91e3_wsedi_upload_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    27154 2021-06-23 23:14:44.000000 django-jbank-4.2.1/htmlcov/jbank_management_commands_parse_to_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    13619 2023-03-27 06:36:02.000000 django-jbank-4.2.1/htmlcov/d_d9f236fb879a91e3_parse_euribor_rates_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)     4514 2023-03-27 06:36:02.000000 django-jbank-4.2.1/htmlcov/d_de1059d8df3ce8de___init___py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    35254 2023-03-27 06:36:02.000000 django-jbank-4.2.1/htmlcov/d_2442641f6b49fa31_helpers_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    58311 2021-06-23 23:14:44.000000 django-jbank-4.2.1/htmlcov/jbank_aeb43_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)     8924 2023-03-27 06:36:02.000000 django-jbank-4.2.1/htmlcov/d_d9f236fb879a91e3_test_svm_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)   140727 2023-03-27 06:36:02.000000 django-jbank-4.2.1/htmlcov/d_2442641f6b49fa31_wspki_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)     4474 2023-03-27 06:36:02.000000 django-jbank-4.2.1/htmlcov/d_2442641f6b49fa31_views_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)     4526 2023-03-27 06:36:02.000000 django-jbank-4.2.1/htmlcov/d_367ac34b948d641d___init___py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    29945 2023-03-27 06:36:02.000000 django-jbank-4.2.1/htmlcov/d_d9f236fb879a91e3_parse_svm_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    13834 2021-06-23 23:14:44.000000 django-jbank-4.2.1/htmlcov/jbank_management_commands_test_payment_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    23928 2023-03-27 06:36:02.000000 django-jbank-4.2.1/htmlcov/d_d9f236fb879a91e3_wsedi_exec_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)     6935 2021-06-23 23:14:44.000000 django-jbank-4.2.1/htmlcov/jbank_management_commands_test_svm_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    18044 2023-03-27 06:36:02.000000 django-jbank-4.2.1/htmlcov/d_2442641f6b49fa31_euribor_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2599 2021-06-23 23:14:44.000000 django-jbank-4.2.1/htmlcov/jbank_templates_admin_jbank_referencepaymentbatch___init___py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    27546 2021-06-23 23:14:44.000000 django-jbank-4.2.1/htmlcov/jbank_management_commands_parse_xp_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2555 2021-06-23 23:14:44.000000 django-jbank-4.2.1/htmlcov/jbank_templates_admin_jbank___init___py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)     6546 2023-03-27 06:36:02.000000 django-jbank-4.2.1/htmlcov/d_2442641f6b49fa31_apps_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)   112238 2021-06-23 23:14:44.000000 django-jbank-4.2.1/htmlcov/jbank_tito_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    20650 2023-03-27 06:36:02.000000 django-jbank-4.2.1/htmlcov/coverage_html.js
+-rw-rw-r--   0 jani      (1000) jani      (1000)    12429 2023-03-27 06:36:02.000000 django-jbank-4.2.1/htmlcov/style.css
+-rw-rw-r--   0 jani      (1000) jani      (1000)    13993 2023-03-27 06:36:02.000000 django-jbank-4.2.1/htmlcov/d_d9f236fb879a91e3_parse_aeb43_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    13624 2021-06-23 23:14:44.000000 django-jbank-4.2.1/htmlcov/jbank_management_commands_test_app_req_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)     9003 2023-03-27 06:36:02.000000 django-jbank-4.2.1/htmlcov/keybd_open.png
+-rw-rw-r--   0 jani      (1000) jani      (1000)    19907 2021-06-23 23:14:44.000000 django-jbank-4.2.1/htmlcov/jbank_management_commands_test_pain001_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)     4520 2023-03-27 06:36:02.000000 django-jbank-4.2.1/htmlcov/d_c6b51be18eb0ec86___init___py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)     4558 2023-03-27 06:36:02.000000 django-jbank-4.2.1/htmlcov/d_d4f8c6455716e7bb___init___py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    24383 2023-03-27 06:36:02.000000 django-jbank-4.2.1/htmlcov/d_d9f236fb879a91e3_make_parse_format_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)   105315 2023-03-27 06:36:02.000000 django-jbank-4.2.1/htmlcov/d_2442641f6b49fa31_tests_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    13538 2023-03-27 06:36:02.000000 django-jbank-4.2.1/htmlcov/d_2442641f6b49fa31_ecb_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    20842 2023-03-27 06:36:02.000000 django-jbank-4.2.1/htmlcov/d_d9f236fb879a91e3_reparse_svm_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)   139457 2021-06-23 23:14:44.000000 django-jbank-4.2.1/htmlcov/jbank_camt_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    22274 2021-06-23 23:14:44.000000 django-jbank-4.2.1/htmlcov/jbank_management_commands_make_parse_format_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    25502 2023-03-27 06:36:02.000000 django-jbank-4.2.1/htmlcov/d_d9f236fb879a91e3_parse_ecb_rates_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)   386954 2021-06-23 23:14:44.000000 django-jbank-4.2.1/htmlcov/jbank_admin_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    28146 2021-06-23 23:14:44.000000 django-jbank-4.2.1/htmlcov/jbank_management_commands_make_x509_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)     8876 2021-06-23 23:14:44.000000 django-jbank-4.2.1/htmlcov/jbank_management_commands_test_xp_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    18793 2021-06-23 23:14:44.000000 django-jbank-4.2.1/htmlcov/jbank_management_commands_reparse_svm_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)      247 2020-05-27 18:47:15.000000 django-jbank-4.2.1/mypy.ini
+-rw-rw-r--   0 jani      (1000) jani      (1000)      287 2020-09-02 13:51:57.000000 django-jbank-4.2.1/MANIFEST.in
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-05-16 17:40:39.000000 django-jbank-4.2.1/data/
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-05-16 17:40:39.000000 django-jbank-4.2.1/data/pain001/
+-rw-rw-r--   0 jani      (1000) jani      (1000)     4044 2020-05-21 16:43:43.000000 django-jbank-4.2.1/data/pain001/pain.001.001.03.xml
+-rw-rw-r--   0 jani      (1000) jani      (1000)    91224 2020-05-21 16:43:43.000000 django-jbank-4.2.1/data/ecb-rates-2019-08-15.xml
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-05-16 17:40:39.000000 django-jbank-4.2.1/data/pki/
+-rw-rw-r--   0 jani      (1000) jani      (1000)    10099 2020-07-18 04:38:59.000000 django-jbank-4.2.1/data/pki/GetBankCertificate-res.xml
+-rw-rw-r--   0 jani      (1000) jani      (1000)      638 2020-07-20 22:19:28.000000 django-jbank-4.2.1/data/pki/CreateCertificate-res.xml
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1547 2021-07-06 23:33:19.000000 django-jbank-4.2.1/data/x509-data.xml
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-05-16 17:40:39.000000 django-jbank-4.2.1/data/finvoice/
+-rw-rw-r--   0 jani      (1000) jani      (1000)     5362 2020-05-21 16:43:43.000000 django-jbank-4.2.1/data/finvoice/xsd-test.xml
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-05-16 17:40:39.000000 django-jbank-4.2.1/data/xm/
+-rw-rw-r--   0 jani      (1000) jani      (1000)     6994 2023-03-27 06:59:59.000000 django-jbank-4.2.1/data/xm/camt_054_credit_notoification_example_finland.xml
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-05-16 17:40:39.000000 django-jbank-4.2.1/data/x509/
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1561 2022-07-21 16:32:20.000000 django-jbank-4.2.1/data/x509/x509data.xml
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1486 2020-05-21 16:43:43.000000 django-jbank-4.2.1/data/x509/appreq.xml
+-rw-rw-r--   0 jani      (1000) jani      (1000)      139 2023-02-14 22:34:42.000000 django-jbank-4.2.1/requirements.txt
+-rw-rw-r--   0 jani      (1000) jani      (1000)      867 2023-05-16 17:40:29.000000 django-jbank-4.2.1/setup.py
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-05-16 17:40:39.000000 django-jbank-4.2.1/jbank/
+-rw-rw-r--   0 jani      (1000) jani      (1000)     3425 2023-05-16 17:40:29.000000 django-jbank-4.2.1/jbank/helpers.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     7737 2023-05-16 17:40:29.000000 django-jbank-4.2.1/jbank/wsedi.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)    44691 2023-05-16 17:40:29.000000 django-jbank-4.2.1/jbank/models.py
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-05-16 17:40:39.000000 django-jbank-4.2.1/jbank/management/
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-05-16 17:40:39.000000 django-jbank-4.2.1/jbank/management/commands/
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1014 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/management/commands/parse_ra.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      505 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/management/commands/test_to.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     3193 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/management/commands/make_x509.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      498 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/management/commands/parse_x509.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1287 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/management/commands/test_app_req.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     3610 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/management/commands/parse_svm.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      859 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/management/commands/xmlsec1_examples.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2338 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/management/commands/wsedi_exec.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1195 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/management/commands/test_payment.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2146 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/management/commands/wsedi_import.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2557 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/management/commands/wspki_exec.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      498 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/management/commands/test_svm.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     3373 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/management/commands/parse_to.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     7308 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/management/commands/parse_xt.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2085 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/management/commands/test_pain001.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     5963 2023-05-16 17:40:29.000000 django-jbank-4.2.1/jbank/management/commands/wsedi_download.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2935 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/management/commands/parse_xm.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2286 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/management/commands/reparse_svm.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1002 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/management/commands/parse_saldo.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2237 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/management/commands/make_parse_format.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2690 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/management/commands/parse_ecb_rates.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     3091 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/management/commands/parse_xp.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      676 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/management/commands/test_xp.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     4589 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/management/commands/make_pain001.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2450 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/management/commands/reparse_to.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1190 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/management/commands/parse_euribor_rates.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     4983 2023-05-16 17:40:29.000000 django-jbank-4.2.1/jbank/management/commands/wsedi_upload.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1541 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/management/commands/wsedi_export.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1102 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/management/commands/parse_aeb43.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)        0 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/management/commands/__init__.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)        0 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/management/__init__.py
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-05-16 17:40:39.000000 django-jbank-4.2.1/jbank/migrations/
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1074 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0008_auto_20210512_2208.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      754 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0016_alter_payoutstatus_timestamp.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      760 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0004_statementfile.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)    57170 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0001_squashed_0071_wsediconnection_ca_cert_file.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      655 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0026_auto_20181205_0034.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1735 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0034_auto_20190815_2059.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      886 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0007_auto_20171102_2351.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1333 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0019_auto_20180209_0437.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      648 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0013_auto_20180126_0909.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      591 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0023_remove_accountbalance_connection_accountbalance_bic.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      428 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0004_refund_attachment.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1192 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0015_auto_20180208_0643.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      422 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0068_auto_20200717_2327.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      580 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0055_auto_20191130_2011.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      461 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0070_wsediconnection_bank_signing_cert_file.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      443 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0020_payout_due_date.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      515 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0069_auto_20200717_2333.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      406 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0047_wsedisoapcall_error.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      347 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0050_remove_wsedisoapcall_payout.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      703 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0041_auto_20191127_0559.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      576 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0039_auto_20191127_0156.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      748 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0037_auto_20191127_0132.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1672 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0008_auto_20171103_0007.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1019 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0024_auto_20180425_1704.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      577 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0048_wsediconnection_soap_endpoint.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      464 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0028_auto_20190327_1830.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      480 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0066_wsediconnection_pin.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      667 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0018_auto_20180208_1130.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      482 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0053_wsediconnection_target_identifier.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      551 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0005_statementfile_created.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      643 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0025_auto_20181101_1430.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      703 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0027_auto_20190304_1913.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1196 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0036_wsediconnection.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      439 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0015_ps_timestamp_fill.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      443 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0038_auto_20191127_0145.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     3784 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0028_referencepaymentrecord_creditor_bank_bic_and_more.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      523 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0010_statementrecorddetail_creditor_account_scheme.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2493 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0011_auto_20180126_0851.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      487 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0045_wsediconnection_receiver_identifier.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      468 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0071_wsediconnection_ca_cert_file.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      623 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0051_payout_connection.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      967 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0018_alter_referencepaymentbatch_currency_identifier_and_more.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      638 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0003_statement_account.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1096 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0007_auto_20210507_2122.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1930 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0012_auto_20180126_0858.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      412 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0003_auto_20200902_1354.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)    15229 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0001_initial.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1175 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0013_euriborrate.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      934 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0019_alter_payout_state.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      486 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0010_auto_20171226_1013.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      482 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0017_alter_statementrecord_name.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      418 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0059_auto_20200324_0234.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      514 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0030_alter_referencepaymentrecord_remittance_info.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      494 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0049_wsediconnection_sender_identifier.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      450 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0014_payoutstatus_timestamp.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      424 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0046_auto_20191128_2242.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      711 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0022_accountbalance_connection.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      462 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0065_wsediconnection_bank_root_cert_file.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1520 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0020_accountbalance.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      405 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0023_auto_20180419_1316.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      748 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0031_wsediconnection_old_encryption_key_file_and_more.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      687 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0021_auto_20180209_0935.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      500 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0009_referencepaymentbatchfile_cached_total_amount.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      441 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0057_wsediconnection_enabled.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2335 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0043_wsedisoapcall.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      707 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0006_auto_20210318_2130.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      467 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0042_wsediconnection_bank_encryption_cert_file.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)    11060 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0029_auto_20190727_1352.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)    27144 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0064_auto_20200629_0344.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      692 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0062_auto_20200415_2300.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      498 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0005_auto_20201203_2308.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      670 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0061_auto_20200325_2204.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      698 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0060_auto_20200325_1906.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      462 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0033_alter_statement_begin_date.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1451 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0026_referencepaymentbatch_identifier_and_more.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      455 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0063_auto_20200608_1827.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      520 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0029_alter_referencepaymentrecord_remittance_info.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      488 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0033_auto_20190801_2121.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      665 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0052_auto_20191130_1927.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1006 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0024_referencepaymentbatchfile_additional_info_and_more.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      525 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0009_auto_20171107_1847.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      491 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0058_auto_20200316_1949.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     3164 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0016_auto_20180208_0724.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      463 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0032_wsediconnection_use_sha256.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      753 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0027_referencepaymentrecord_value_date_and_more.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      665 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0006_auto_20171102_2341.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      433 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0021_alter_accountbalance_balance.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      452 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0044_auto_20191128_2231.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      523 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0011_referencepaymentbatch_cached_total_amount.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      706 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0017_payoutparty_payouts_account.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      426 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0056_wsediconnection_debug_commands.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     3213 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0002_auto_20171031_0356.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      478 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0030_auto_20190727_1633.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      713 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0012_alter_referencepaymentrecord_delivery_method.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      434 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0067_wsediconnection_pki_endpoint.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     4229 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0014_payout_payoutstatus.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      534 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0025_auto_20230325_1014.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      488 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0035_auto_20190815_2137.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      449 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0040_wsediconnection_signing_key_file.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2031 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0002_auto_20200817_2217.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      467 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0034_wsediconnection_use_wsse_timestamp.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      460 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0054_wsediconnection_environment.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1621 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0031_auto_20190727_1639.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      479 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0032_auto_20190727_1655.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      456 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/0022_auto_20180411_1814.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)        0 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/migrations/__init__.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)    19040 2023-05-16 17:40:29.000000 django-jbank-4.2.1/jbank/wspki.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)       27 2020-05-26 21:27:46.000000 django-jbank-4.2.1/jbank/py.typed
+-rw-rw-r--   0 jani      (1000) jani      (1000)    11520 2023-05-16 17:40:29.000000 django-jbank-4.2.1/jbank/svm.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      716 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/services.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)    23256 2023-05-16 17:40:29.000000 django-jbank-4.2.1/jbank/camt.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)    26191 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/tests.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)    52642 2023-05-16 17:40:29.000000 django-jbank-4.2.1/jbank/admin.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     6524 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/aeb43.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1247 2023-05-16 17:40:29.000000 django-jbank-4.2.1/jbank/ecb.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)    22581 2023-05-16 17:40:29.000000 django-jbank-4.2.1/jbank/sepa.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1189 2023-05-16 17:40:29.000000 django-jbank-4.2.1/jbank/x509_helpers.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)    10244 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/parsers.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     5301 2023-05-16 17:40:29.000000 django-jbank-4.2.1/jbank/csr_helpers.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      235 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/apps.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      828 2023-05-16 17:40:29.000000 django-jbank-4.2.1/jbank/files.py
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-05-16 17:40:39.000000 django-jbank-4.2.1/jbank/templates/
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-05-16 17:40:39.000000 django-jbank-4.2.1/jbank/templates/admin/
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-05-16 17:40:39.000000 django-jbank-4.2.1/jbank/templates/admin/jbank/
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-05-16 17:40:39.000000 django-jbank-4.2.1/jbank/templates/admin/jbank/referencepaymentbatch/
+-rw-rw-r--   0 jani      (1000) jani      (1000)      793 2020-05-21 16:43:43.000000 django-jbank-4.2.1/jbank/templates/admin/jbank/referencepaymentbatch/change_form.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)        0 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/templates/admin/jbank/referencepaymentbatch/__init__.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      690 2020-05-21 16:43:43.000000 django-jbank-4.2.1/jbank/templates/admin/jbank/mark_as_manually_settled.html
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-05-16 17:40:39.000000 django-jbank-4.2.1/jbank/templates/admin/jbank/statement/
+-rw-rw-r--   0 jani      (1000) jani      (1000)      782 2020-05-21 16:43:43.000000 django-jbank-4.2.1/jbank/templates/admin/jbank/statement/change_form.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)        0 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/templates/admin/jbank/statement/__init__.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)        0 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/templates/admin/jbank/__init__.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)        0 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/templates/admin/__init__.py
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-05-16 17:40:39.000000 django-jbank-4.2.1/jbank/templates/jbank/
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2041 2021-12-23 17:01:04.000000 django-jbank-4.2.1/jbank/templates/jbank/pki_certificate_status_request_template.xml
+-rw-rw-r--   0 jani      (1000) jani      (1000)      962 2021-12-23 17:01:04.000000 django-jbank-4.2.1/jbank/templates/jbank/pki_create_certificate_request_template.xml
+-rw-rw-r--   0 jani      (1000) jani      (1000)      876 2020-05-21 16:43:43.000000 django-jbank-4.2.1/jbank/templates/jbank/soap_template.xml
+-rw-rw-r--   0 jani      (1000) jani      (1000)      562 2021-07-06 21:13:32.000000 django-jbank-4.2.1/jbank/templates/jbank/pki_get_certificate_soap_template.xml
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2079 2022-01-09 22:11:13.000000 django-jbank-4.2.1/jbank/templates/jbank/pki_renew_certificate_request_template.xml
+-rw-rw-r--   0 jani      (1000) jani      (1000)      568 2021-12-23 17:01:04.000000 django-jbank-4.2.1/jbank/templates/jbank/pki_get_certificate_request_template.xml
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2223 2023-04-05 11:04:17.000000 django-jbank-4.2.1/jbank/templates/jbank/application_request_template-sha256.xml
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1686 2023-04-05 11:04:17.000000 django-jbank-4.2.1/jbank/templates/jbank/pki_get_certificate_renew_request_template-sha256.xml
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2087 2023-04-05 11:04:17.000000 django-jbank-4.2.1/jbank/templates/jbank/pki_renew_certificate_request_template-sha256.xml
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2215 2020-05-21 16:43:43.000000 django-jbank-4.2.1/jbank/templates/jbank/application_request_template.xml
+-rw-rw-r--   0 jani      (1000) jani      (1000)      758 2020-05-21 16:43:43.000000 django-jbank-4.2.1/jbank/templates/jbank/encryption_template.xml
+-rw-rw-r--   0 jani      (1000) jani      (1000)     5352 2023-04-05 11:04:17.000000 django-jbank-4.2.1/jbank/templates/jbank/enveloping-sha256-rsa-sha256.xml
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1678 2021-12-23 17:01:04.000000 django-jbank-4.2.1/jbank/templates/jbank/pki_get_certificate_renew_request_template.xml
+-rw-rw-r--   0 jani      (1000) jani      (1000)      911 2021-12-23 17:01:04.000000 django-jbank-4.2.1/jbank/templates/jbank/pki_soap_template.xml
+-rw-rw-r--   0 jani      (1000) jani      (1000)        0 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/templates/jbank/__init__.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)        0 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/templates/__init__.py
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-05-16 17:40:38.000000 django-jbank-4.2.1/jbank/locale/
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-05-16 17:40:38.000000 django-jbank-4.2.1/jbank/locale/fi/
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-05-16 17:40:39.000000 django-jbank-4.2.1/jbank/locale/fi/LC_MESSAGES/
+-rw-rw-r--   0 jani      (1000) jani      (1000)    15825 2023-02-24 09:03:24.000000 django-jbank-4.2.1/jbank/locale/fi/LC_MESSAGES/django.mo
+-rw-rw-r--   0 jani      (1000) jani      (1000)    26153 2023-02-24 09:03:24.000000 django-jbank-4.2.1/jbank/locale/fi/LC_MESSAGES/django.po
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-05-16 17:40:38.000000 django-jbank-4.2.1/jbank/locale/en/
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-05-16 17:40:39.000000 django-jbank-4.2.1/jbank/locale/en/LC_MESSAGES/
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1102 2023-02-24 08:59:20.000000 django-jbank-4.2.1/jbank/locale/en/LC_MESSAGES/django.mo
+-rw-rw-r--   0 jani      (1000) jani      (1000)    21019 2023-02-24 09:03:24.000000 django-jbank-4.2.1/jbank/locale/en/LC_MESSAGES/django.po
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-05-16 17:40:39.000000 django-jbank-4.2.1/jbank/xmlsec1-examples/
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1058 2023-04-05 11:04:17.000000 django-jbank-4.2.1/jbank/xmlsec1-examples/Makefile
+-rw-rw-r--   0 jani      (1000) jani      (1000)    10308 2020-05-21 16:43:43.000000 django-jbank-4.2.1/jbank/xmlsec1-examples/encrypt3.c
+-rw-rw-r--   0 jani      (1000) jani      (1000)     9710 2020-05-21 16:43:43.000000 django-jbank-4.2.1/jbank/xmlsec1-examples/sign3.c
+-rw-rw-r--   0 jani      (1000) jani      (1000)     7127 2020-05-21 16:43:43.000000 django-jbank-4.2.1/jbank/xmlsec1-examples/decrypt3.c
+-rw-rw-r--   0 jani      (1000) jani      (1000)     7088 2020-05-21 16:43:43.000000 django-jbank-4.2.1/jbank/xmlsec1-examples/verify3.c
+-rw-rw-r--   0 jani      (1000) jani      (1000)     9718 2023-04-05 11:04:17.000000 django-jbank-4.2.1/jbank/xmlsec1-examples/sign3-sha256.c
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1582 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/pain002.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)        0 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/views.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1562 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/euribor.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)    12672 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/tito.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)       46 2023-05-15 21:54:48.000000 django-jbank-4.2.1/jbank/__init__.py
```

### Comparing `django-jbank-4.1.3/pyproject.toml` & `django-jbank-4.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/README.md` & `django-jbank-4.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 django-jbank
 ============
 
-Basic Finnish bank file format support for Django projects. Django 3.0 support and unit test coverage 51%.
+Basic (Finnish) bank file format support for Django projects. Django 4 support and unit test coverage 51%.
 
 Features
 ========
 
 * Finnish banks:
   * Parsing TO/TITO files
   * Parsing SVM/KTL files
```

### Comparing `django-jbank-4.1.3/LICENSE.txt` & `django-jbank-4.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/PKG-INFO` & `django-jbank-4.2.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: django-jbank
-Version: 4.1.3
+Version: 4.2.1
 Summary: Finnish bank file format support for Django projects
 Home-page: 
 Author: Jani Kajala
 Author-email: kajala@gmail.com
 License: MIT licence, see LICENCE.txt
 License-File: LICENSE.txt
 
 django-jbank
 ============
 
-Basic Finnish bank file format support for Django projects. Django 3.0 support and unit test coverage 51%.
+Basic (Finnish) bank file format support for Django projects. Django 4 support and unit test coverage 51%.
 
 Features
 ========
 
 * Finnish banks:
   * Parsing TO/TITO files
   * Parsing SVM/KTL files
```

### Comparing `django-jbank-4.1.3/django_jbank.egg-info/PKG-INFO` & `django-jbank-4.2.1/django_jbank.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: django-jbank
-Version: 4.1.3
+Version: 4.2.1
 Summary: Finnish bank file format support for Django projects
 Home-page: 
 Author: Jani Kajala
 Author-email: kajala@gmail.com
 License: MIT licence, see LICENCE.txt
 License-File: LICENSE.txt
 
 django-jbank
 ============
 
-Basic Finnish bank file format support for Django projects. Django 3.0 support and unit test coverage 51%.
+Basic (Finnish) bank file format support for Django projects. Django 4 support and unit test coverage 51%.
 
 Features
 ========
 
 * Finnish banks:
   * Parsing TO/TITO files
   * Parsing SVM/KTL files
```

### Comparing `django-jbank-4.1.3/django_jbank.egg-info/SOURCES.txt` & `django-jbank-4.2.1/django_jbank.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -3008,14 +3008,17 @@
 ./venv/lib/python3.10/site-packages/django_stubs_ext/py.typed
 ./venv/lib/python3.10/site-packages/django_stubs_ext-0.8.0.dist-info/LICENSE.txt
 ./venv/lib/python3.10/site-packages/django_stubs_ext-0.8.0.dist-info/top_level.txt
 ./venv/lib/python3.10/site-packages/djangorestframework-3.13.1.dist-info/LICENSE.md
 ./venv/lib/python3.10/site-packages/djangorestframework-3.13.1.dist-info/top_level.txt
 ./venv/lib/python3.10/site-packages/djangorestframework_stubs-1.10.0.dist-info/LICENSE.txt
 ./venv/lib/python3.10/site-packages/djangorestframework_stubs-1.10.0.dist-info/top_level.txt
+./venv/lib/python3.10/site-packages/docconvert-2.1.0.dist-info/LICENSE.md
+./venv/lib/python3.10/site-packages/docconvert-2.1.0.dist-info/entry_points.txt
+./venv/lib/python3.10/site-packages/docconvert-2.1.0.dist-info/top_level.txt
 ./venv/lib/python3.10/site-packages/docutils-0.18.1.dist-info/COPYING.txt
 ./venv/lib/python3.10/site-packages/docutils-0.18.1.dist-info/SOURCES.html
 ./venv/lib/python3.10/site-packages/docutils-0.18.1.dist-info/dependency_links.html
 ./venv/lib/python3.10/site-packages/docutils-0.18.1.dist-info/top_level.html
 ./venv/lib/python3.10/site-packages/docutils-0.18.1.dist-info/top_level.txt
 ./venv/lib/python3.10/site-packages/docutils/parsers/rst/include/README.txt
 ./venv/lib/python3.10/site-packages/docutils/parsers/rst/include/isoamsa.txt
@@ -3183,17 +3186,18 @@
 ./venv/lib/python3.10/site-packages/pbr/tests/testpackage/data_files/b.txt
 ./venv/lib/python3.10/site-packages/pbr/tests/testpackage/pbr_testpackage/package_data/1.txt
 ./venv/lib/python3.10/site-packages/pbr/tests/testpackage/pbr_testpackage/package_data/2.txt
 ./venv/lib/python3.10/site-packages/pbr/tests/testpackage/src/testext.c
 ./venv/lib/python3.10/site-packages/pep8_naming-0.10.0.dist-info/entry_points.txt
 ./venv/lib/python3.10/site-packages/pep8_naming-0.10.0.dist-info/top_level.txt
 ./venv/lib/python3.10/site-packages/pip/py.typed
-./venv/lib/python3.10/site-packages/pip-23.0.1.dist-info/LICENSE.txt
-./venv/lib/python3.10/site-packages/pip-23.0.1.dist-info/entry_points.txt
-./venv/lib/python3.10/site-packages/pip-23.0.1.dist-info/top_level.txt
+./venv/lib/python3.10/site-packages/pip-23.1.2.dist-info/AUTHORS.txt
+./venv/lib/python3.10/site-packages/pip-23.1.2.dist-info/LICENSE.txt
+./venv/lib/python3.10/site-packages/pip-23.1.2.dist-info/entry_points.txt
+./venv/lib/python3.10/site-packages/pip-23.1.2.dist-info/top_level.txt
 ./venv/lib/python3.10/site-packages/pip/_vendor/vendor.txt
 ./venv/lib/python3.10/site-packages/pkginfo-1.8.2.dist-info/LICENSE.txt
 ./venv/lib/python3.10/site-packages/pkginfo-1.8.2.dist-info/entry_points.txt
 ./venv/lib/python3.10/site-packages/pkginfo-1.8.2.dist-info/top_level.txt
 ./venv/lib/python3.10/site-packages/platformdirs/py.typed
 ./venv/lib/python3.10/site-packages/platformdirs-2.5.2.dist-info/entry_points.txt
 ./venv/lib/python3.10/site-packages/platformdirs-2.5.2.dist-info/license_files/LICENSE.txt
@@ -6257,14 +6261,17 @@
 ./venv/lib64/python3.10/site-packages/django_stubs_ext/py.typed
 ./venv/lib64/python3.10/site-packages/django_stubs_ext-0.8.0.dist-info/LICENSE.txt
 ./venv/lib64/python3.10/site-packages/django_stubs_ext-0.8.0.dist-info/top_level.txt
 ./venv/lib64/python3.10/site-packages/djangorestframework-3.13.1.dist-info/LICENSE.md
 ./venv/lib64/python3.10/site-packages/djangorestframework-3.13.1.dist-info/top_level.txt
 ./venv/lib64/python3.10/site-packages/djangorestframework_stubs-1.10.0.dist-info/LICENSE.txt
 ./venv/lib64/python3.10/site-packages/djangorestframework_stubs-1.10.0.dist-info/top_level.txt
+./venv/lib64/python3.10/site-packages/docconvert-2.1.0.dist-info/LICENSE.md
+./venv/lib64/python3.10/site-packages/docconvert-2.1.0.dist-info/entry_points.txt
+./venv/lib64/python3.10/site-packages/docconvert-2.1.0.dist-info/top_level.txt
 ./venv/lib64/python3.10/site-packages/docutils-0.18.1.dist-info/COPYING.txt
 ./venv/lib64/python3.10/site-packages/docutils-0.18.1.dist-info/SOURCES.html
 ./venv/lib64/python3.10/site-packages/docutils-0.18.1.dist-info/dependency_links.html
 ./venv/lib64/python3.10/site-packages/docutils-0.18.1.dist-info/top_level.html
 ./venv/lib64/python3.10/site-packages/docutils-0.18.1.dist-info/top_level.txt
 ./venv/lib64/python3.10/site-packages/docutils/parsers/rst/include/README.txt
 ./venv/lib64/python3.10/site-packages/docutils/parsers/rst/include/isoamsa.txt
@@ -6432,17 +6439,18 @@
 ./venv/lib64/python3.10/site-packages/pbr/tests/testpackage/data_files/b.txt
 ./venv/lib64/python3.10/site-packages/pbr/tests/testpackage/pbr_testpackage/package_data/1.txt
 ./venv/lib64/python3.10/site-packages/pbr/tests/testpackage/pbr_testpackage/package_data/2.txt
 ./venv/lib64/python3.10/site-packages/pbr/tests/testpackage/src/testext.c
 ./venv/lib64/python3.10/site-packages/pep8_naming-0.10.0.dist-info/entry_points.txt
 ./venv/lib64/python3.10/site-packages/pep8_naming-0.10.0.dist-info/top_level.txt
 ./venv/lib64/python3.10/site-packages/pip/py.typed
-./venv/lib64/python3.10/site-packages/pip-23.0.1.dist-info/LICENSE.txt
-./venv/lib64/python3.10/site-packages/pip-23.0.1.dist-info/entry_points.txt
-./venv/lib64/python3.10/site-packages/pip-23.0.1.dist-info/top_level.txt
+./venv/lib64/python3.10/site-packages/pip-23.1.2.dist-info/AUTHORS.txt
+./venv/lib64/python3.10/site-packages/pip-23.1.2.dist-info/LICENSE.txt
+./venv/lib64/python3.10/site-packages/pip-23.1.2.dist-info/entry_points.txt
+./venv/lib64/python3.10/site-packages/pip-23.1.2.dist-info/top_level.txt
 ./venv/lib64/python3.10/site-packages/pip/_vendor/vendor.txt
 ./venv/lib64/python3.10/site-packages/pkginfo-1.8.2.dist-info/LICENSE.txt
 ./venv/lib64/python3.10/site-packages/pkginfo-1.8.2.dist-info/entry_points.txt
 ./venv/lib64/python3.10/site-packages/pkginfo-1.8.2.dist-info/top_level.txt
 ./venv/lib64/python3.10/site-packages/platformdirs/py.typed
 ./venv/lib64/python3.10/site-packages/platformdirs-2.5.2.dist-info/entry_points.txt
 ./venv/lib64/python3.10/site-packages/platformdirs-2.5.2.dist-info/license_files/LICENSE.txt
```

### Comparing `django-jbank-4.1.3/htmlcov/d_2442641f6b49fa31_pain002_py.html` & `django-jbank-4.2.1/htmlcov/d_2442641f6b49fa31_pain002_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/jquery.hotkeys.js` & `django-jbank-4.2.1/htmlcov/jquery.hotkeys.js`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/jbank_apps_py.html` & `django-jbank-4.2.1/htmlcov/jbank_apps_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/jquery.tablesorter.min.js` & `django-jbank-4.2.1/htmlcov/jquery.tablesorter.min.js`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_wsedi_export_py.html` & `django-jbank-4.2.1/htmlcov/d_d9f236fb879a91e3_wsedi_export_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_wsedi_download_py.html` & `django-jbank-4.2.1/htmlcov/d_d9f236fb879a91e3_wsedi_download_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/jbank_management_commands_wsedi_import_py.html` & `django-jbank-4.2.1/htmlcov/jbank_management_commands_wsedi_import_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/d_2442641f6b49fa31_admin_py.html` & `django-jbank-4.2.1/htmlcov/d_2442641f6b49fa31_admin_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_parse_saldo_py.html` & `django-jbank-4.2.1/htmlcov/d_d9f236fb879a91e3_parse_saldo_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/jbank___init___py.html` & `django-jbank-4.2.1/htmlcov/jbank___init___py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/jbank_management_commands_wsedi_exec_py.html` & `django-jbank-4.2.1/htmlcov/jbank_management_commands_wsedi_exec_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_parse_xm_py.html` & `django-jbank-4.2.1/htmlcov/d_d9f236fb879a91e3_parse_xm_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/jbank_svm_py.html` & `django-jbank-4.2.1/htmlcov/jbank_svm_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/jbank_sepa_py.html` & `django-jbank-4.2.1/htmlcov/jbank_sepa_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/jbank_helpers_py.html` & `django-jbank-4.2.1/htmlcov/jbank_helpers_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/d_2442641f6b49fa31_wsedi_py.html` & `django-jbank-4.2.1/htmlcov/d_2442641f6b49fa31_wsedi_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/manage_py.html` & `django-jbank-4.2.1/htmlcov/manage_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3___init___py.html` & `django-jbank-4.2.1/htmlcov/d_d9f236fb879a91e3___init___py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/index.html` & `django-jbank-4.2.1/htmlcov/index.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_xmlsec1_examples_py.html` & `django-jbank-4.2.1/htmlcov/d_d9f236fb879a91e3_xmlsec1_examples_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/jbank_management_commands_parse_aeb43_py.html` & `django-jbank-4.2.1/htmlcov/jbank_management_commands_parse_aeb43_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/jbank_management_commands_test_to_py.html` & `django-jbank-4.2.1/htmlcov/jbank_management_commands_test_to_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/jbank_management___init___py.html` & `django-jbank-4.2.1/htmlcov/jbank_management___init___py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/d_2442641f6b49fa31_sepa_py.html` & `django-jbank-4.2.1/htmlcov/d_2442641f6b49fa31_sepa_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/d_2442641f6b49fa31_x509_helpers_py.html` & `django-jbank-4.2.1/htmlcov/d_2442641f6b49fa31_x509_helpers_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/d_d1b4fb5372fdacae___init___py.html` & `django-jbank-4.2.1/htmlcov/d_d1b4fb5372fdacae___init___py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_wspki_exec_py.html` & `django-jbank-4.2.1/htmlcov/d_d9f236fb879a91e3_wspki_exec_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/jbank_templates_jbank___init___py.html` & `django-jbank-4.2.1/htmlcov/jbank_templates_jbank___init___py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_parse_to_py.html` & `django-jbank-4.2.1/htmlcov/d_d9f236fb879a91e3_parse_to_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_test_pain001_py.html` & `django-jbank-4.2.1/htmlcov/d_d9f236fb879a91e3_test_pain001_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/jbank_templates_admin___init___py.html` & `django-jbank-4.2.1/htmlcov/jbank_templates_admin___init___py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_parse_xp_py.html` & `django-jbank-4.2.1/htmlcov/d_d9f236fb879a91e3_parse_xp_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/jbank_templates_admin_jbank_statement___init___py.html` & `django-jbank-4.2.1/htmlcov/jbank_templates_admin_jbank_statement___init___py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_reparse_to_py.html` & `django-jbank-4.2.1/htmlcov/d_d9f236fb879a91e3_reparse_to_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_make_x509_py.html` & `django-jbank-4.2.1/htmlcov/d_d9f236fb879a91e3_make_x509_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/jbank_wsedi_py.html` & `django-jbank-4.2.1/htmlcov/jbank_wsedi_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/jquery.ba-throttle-debounce.min.js` & `django-jbank-4.2.1/htmlcov/jquery.ba-throttle-debounce.min.js`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_test_payment_py.html` & `django-jbank-4.2.1/htmlcov/d_d9f236fb879a91e3_test_payment_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_test_xp_py.html` & `django-jbank-4.2.1/htmlcov/d_d9f236fb879a91e3_test_xp_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/jbank_files_py.html` & `django-jbank-4.2.1/htmlcov/jbank_files_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/jbank_management_commands_make_pain001_py.html` & `django-jbank-4.2.1/htmlcov/jbank_management_commands_make_pain001_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/jbank_management_commands_parse_ecb_rates_py.html` & `django-jbank-4.2.1/htmlcov/jbank_management_commands_parse_ecb_rates_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/d_2442641f6b49fa31___init___py.html` & `django-jbank-4.2.1/htmlcov/d_2442641f6b49fa31___init___py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/jbank_csr_helpers_py.html` & `django-jbank-4.2.1/htmlcov/jbank_csr_helpers_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/jbank_tests_py.html` & `django-jbank-4.2.1/htmlcov/jbank_tests_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/jbank_management_commands_wsedi_download_py.html` & `django-jbank-4.2.1/htmlcov/jbank_management_commands_wsedi_download_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/d_2442641f6b49fa31_models_py.html` & `django-jbank-4.2.1/htmlcov/d_2442641f6b49fa31_models_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/d_2442641f6b49fa31_parsers_py.html` & `django-jbank-4.2.1/htmlcov/d_2442641f6b49fa31_parsers_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/jbank_models_py.html` & `django-jbank-4.2.1/htmlcov/jbank_models_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/d_2442641f6b49fa31_csr_helpers_py.html` & `django-jbank-4.2.1/htmlcov/d_2442641f6b49fa31_csr_helpers_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/jbank_management_commands_xmlsec1_examples_py.html` & `django-jbank-4.2.1/htmlcov/jbank_management_commands_xmlsec1_examples_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/jbank_parsers_py.html` & `django-jbank-4.2.1/htmlcov/jbank_parsers_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/d_2442641f6b49fa31_svm_py.html` & `django-jbank-4.2.1/htmlcov/d_2442641f6b49fa31_svm_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/jquery.isonscreen.js` & `django-jbank-4.2.1/htmlcov/jquery.isonscreen.js`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_test_to_py.html` & `django-jbank-4.2.1/htmlcov/d_d9f236fb879a91e3_test_to_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/jbank_management_commands___init___py.html` & `django-jbank-4.2.1/htmlcov/jbank_management_commands___init___py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/jbank_management_commands_wspki_exec_py.html` & `django-jbank-4.2.1/htmlcov/jbank_management_commands_wspki_exec_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/d_2442641f6b49fa31_files_py.html` & `django-jbank-4.2.1/htmlcov/d_2442641f6b49fa31_files_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/jbank_management_commands_wsedi_upload_py.html` & `django-jbank-4.2.1/htmlcov/jbank_management_commands_wsedi_upload_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/jbank_management_commands_parse_svm_py.html` & `django-jbank-4.2.1/htmlcov/jbank_management_commands_parse_svm_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/d_2442641f6b49fa31_tito_py.html` & `django-jbank-4.2.1/htmlcov/d_2442641f6b49fa31_tito_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_wsedi_import_py.html` & `django-jbank-4.2.1/htmlcov/d_d9f236fb879a91e3_wsedi_import_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_make_pain001_py.html` & `django-jbank-4.2.1/htmlcov/d_d9f236fb879a91e3_make_pain001_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/jbank_wspki_py.html` & `django-jbank-4.2.1/htmlcov/jbank_wspki_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/d_9798a7910e9d8d38___init___py.html` & `django-jbank-4.2.1/htmlcov/d_9798a7910e9d8d38___init___py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/keybd_closed.png` & `django-jbank-4.2.1/htmlcov/keybd_closed.png`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/favicon_32.png` & `django-jbank-4.2.1/htmlcov/favicon_32.png`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_test_app_req_py.html` & `django-jbank-4.2.1/htmlcov/d_d9f236fb879a91e3_test_app_req_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/d_2442641f6b49fa31_aeb43_py.html` & `django-jbank-4.2.1/htmlcov/d_2442641f6b49fa31_aeb43_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/d_2442641f6b49fa31_camt_py.html` & `django-jbank-4.2.1/htmlcov/d_2442641f6b49fa31_camt_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/jbank_management_commands_parse_x509_py.html` & `django-jbank-4.2.1/htmlcov/jbank_management_commands_parse_x509_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_parse_ra_py.html` & `django-jbank-4.2.1/htmlcov/d_d9f236fb879a91e3_parse_ra_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/jbank_management_commands_parse_xt_py.html` & `django-jbank-4.2.1/htmlcov/jbank_management_commands_parse_xt_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/jbank_management_commands_reparse_to_py.html` & `django-jbank-4.2.1/htmlcov/jbank_management_commands_reparse_to_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/d_2442641f6b49fa31_services_py.html` & `django-jbank-4.2.1/htmlcov/d_2442641f6b49fa31_services_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_parse_xt_py.html` & `django-jbank-4.2.1/htmlcov/d_d9f236fb879a91e3_parse_xt_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_parse_x509_py.html` & `django-jbank-4.2.1/htmlcov/d_d9f236fb879a91e3_parse_x509_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/jbank_views_py.html` & `django-jbank-4.2.1/htmlcov/jbank_views_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/jbank_templates___init___py.html` & `django-jbank-4.2.1/htmlcov/jbank_templates___init___py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/jbank_ecb_py.html` & `django-jbank-4.2.1/htmlcov/jbank_ecb_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/jbank_x509_helpers_py.html` & `django-jbank-4.2.1/htmlcov/jbank_x509_helpers_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/jquery.min.js` & `django-jbank-4.2.1/htmlcov/jquery.min.js`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/jbank_management_commands_wsedi_export_py.html` & `django-jbank-4.2.1/htmlcov/jbank_management_commands_wsedi_export_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/d_f6e593a656d19133___init___py.html` & `django-jbank-4.2.1/htmlcov/d_f6e593a656d19133___init___py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_wsedi_upload_py.html` & `django-jbank-4.2.1/htmlcov/d_d9f236fb879a91e3_wsedi_upload_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/jbank_management_commands_parse_to_py.html` & `django-jbank-4.2.1/htmlcov/jbank_management_commands_parse_to_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_parse_euribor_rates_py.html` & `django-jbank-4.2.1/htmlcov/d_d9f236fb879a91e3_parse_euribor_rates_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/d_de1059d8df3ce8de___init___py.html` & `django-jbank-4.2.1/htmlcov/d_de1059d8df3ce8de___init___py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/d_2442641f6b49fa31_helpers_py.html` & `django-jbank-4.2.1/htmlcov/d_2442641f6b49fa31_helpers_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/jbank_aeb43_py.html` & `django-jbank-4.2.1/htmlcov/jbank_aeb43_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_test_svm_py.html` & `django-jbank-4.2.1/htmlcov/d_d9f236fb879a91e3_test_svm_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/d_2442641f6b49fa31_wspki_py.html` & `django-jbank-4.2.1/htmlcov/d_2442641f6b49fa31_wspki_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/d_2442641f6b49fa31_views_py.html` & `django-jbank-4.2.1/htmlcov/d_2442641f6b49fa31_views_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/d_367ac34b948d641d___init___py.html` & `django-jbank-4.2.1/htmlcov/d_367ac34b948d641d___init___py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_parse_svm_py.html` & `django-jbank-4.2.1/htmlcov/d_d9f236fb879a91e3_parse_svm_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/jbank_management_commands_test_payment_py.html` & `django-jbank-4.2.1/htmlcov/jbank_management_commands_test_payment_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_wsedi_exec_py.html` & `django-jbank-4.2.1/htmlcov/d_d9f236fb879a91e3_wsedi_exec_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/jbank_management_commands_test_svm_py.html` & `django-jbank-4.2.1/htmlcov/jbank_management_commands_test_svm_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/d_2442641f6b49fa31_euribor_py.html` & `django-jbank-4.2.1/htmlcov/d_2442641f6b49fa31_euribor_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/jbank_templates_admin_jbank_referencepaymentbatch___init___py.html` & `django-jbank-4.2.1/htmlcov/jbank_templates_admin_jbank_referencepaymentbatch___init___py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/jbank_management_commands_parse_xp_py.html` & `django-jbank-4.2.1/htmlcov/jbank_management_commands_parse_xp_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/jbank_templates_admin_jbank___init___py.html` & `django-jbank-4.2.1/htmlcov/jbank_templates_admin_jbank___init___py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/d_2442641f6b49fa31_apps_py.html` & `django-jbank-4.2.1/htmlcov/d_2442641f6b49fa31_apps_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/jbank_tito_py.html` & `django-jbank-4.2.1/htmlcov/jbank_tito_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/coverage_html.js` & `django-jbank-4.2.1/htmlcov/coverage_html.js`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/style.css` & `django-jbank-4.2.1/htmlcov/style.css`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_parse_aeb43_py.html` & `django-jbank-4.2.1/htmlcov/d_d9f236fb879a91e3_parse_aeb43_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/jbank_management_commands_test_app_req_py.html` & `django-jbank-4.2.1/htmlcov/jbank_management_commands_test_app_req_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/keybd_open.png` & `django-jbank-4.2.1/htmlcov/keybd_open.png`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/jbank_management_commands_test_pain001_py.html` & `django-jbank-4.2.1/htmlcov/jbank_management_commands_test_pain001_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/d_c6b51be18eb0ec86___init___py.html` & `django-jbank-4.2.1/htmlcov/d_c6b51be18eb0ec86___init___py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/d_d4f8c6455716e7bb___init___py.html` & `django-jbank-4.2.1/htmlcov/d_d4f8c6455716e7bb___init___py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_make_parse_format_py.html` & `django-jbank-4.2.1/htmlcov/d_d9f236fb879a91e3_make_parse_format_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/d_2442641f6b49fa31_tests_py.html` & `django-jbank-4.2.1/htmlcov/d_2442641f6b49fa31_tests_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/d_2442641f6b49fa31_ecb_py.html` & `django-jbank-4.2.1/htmlcov/d_2442641f6b49fa31_ecb_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_reparse_svm_py.html` & `django-jbank-4.2.1/htmlcov/d_d9f236fb879a91e3_reparse_svm_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/jbank_camt_py.html` & `django-jbank-4.2.1/htmlcov/jbank_camt_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/jbank_management_commands_make_parse_format_py.html` & `django-jbank-4.2.1/htmlcov/jbank_management_commands_make_parse_format_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_parse_ecb_rates_py.html` & `django-jbank-4.2.1/htmlcov/d_d9f236fb879a91e3_parse_ecb_rates_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/jbank_admin_py.html` & `django-jbank-4.2.1/htmlcov/jbank_admin_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/jbank_management_commands_make_x509_py.html` & `django-jbank-4.2.1/htmlcov/jbank_management_commands_make_x509_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/jbank_management_commands_test_xp_py.html` & `django-jbank-4.2.1/htmlcov/jbank_management_commands_test_xp_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/htmlcov/jbank_management_commands_reparse_svm_py.html` & `django-jbank-4.2.1/htmlcov/jbank_management_commands_reparse_svm_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/data/pain001/pain.001.001.03.xml` & `django-jbank-4.2.1/data/pain001/pain.001.001.03.xml`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/data/ecb-rates-2019-08-15.xml` & `django-jbank-4.2.1/data/ecb-rates-2019-08-15.xml`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/data/pki/GetBankCertificate-res.xml` & `django-jbank-4.2.1/data/pki/GetBankCertificate-res.xml`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/data/pki/CreateCertificate-res.xml` & `django-jbank-4.2.1/data/pki/CreateCertificate-res.xml`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/data/x509-data.xml` & `django-jbank-4.2.1/data/x509-data.xml`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/data/finvoice/xsd-test.xml` & `django-jbank-4.2.1/data/finvoice/xsd-test.xml`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/data/xm/camt_054_credit_notoification_example_finland.xml` & `django-jbank-4.2.1/data/xm/camt_054_credit_notoification_example_finland.xml`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/data/x509/x509data.xml` & `django-jbank-4.2.1/data/x509/x509data.xml`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/data/x509/appreq.xml` & `django-jbank-4.2.1/data/x509/appreq.xml`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/setup.py` & `django-jbank-4.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     return [line for line in lineiter if line and not line.startswith("#")]
 
 
 install_requires = parse_requirements("requirements.txt", session=False)
 
 setup(
     name="django-jbank",
-    version="4.1.3",
+    version="4.2.1",
     author="Jani Kajala",
     author_email="kajala@gmail.com",
     packages=find_packages(exclude=["project", "venv"]),
     include_package_data=True,
     url="",
     license="MIT licence, see LICENCE.txt",
     description="Finnish bank file format support for Django projects",
```

### Comparing `django-jbank-4.1.3/jbank/helpers.py` & `django-jbank-4.2.1/jbank/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,17 +53,15 @@
 
 
 def make_msg_id() -> str:
     return re.sub(r"[^\d]", "", now().isoformat())[:-4]
 
 
 def validate_xml(content: bytes, xsd_file_name: str):
-    """
-    Validates XML using XSD
-    """
+    """Validates XML using XSD"""
     schema = etree.XMLSchema(file=xsd_file_name)
     parser = objectify.makeparser(schema=schema)
     objectify.fromstring(content, parser)
 
 
 def parse_date_or_relative_date(value: str, tz: Any = None) -> Optional[date]:
     try:
@@ -81,16 +79,15 @@
         end_date = time_now.astimezone(tz).date() + timedelta(days=1)
     if options["end_date"]:
         end_date = parse_date_or_relative_date(options["end_date"], tz=tz)
     return start_date, end_date
 
 
 def save_or_store_media(file: models.FileField, filename: str):
-    """
-    Saves FileField filename as relative path if it's under MEDIA_ROOT.
+    """Saves FileField filename as relative path if it's under MEDIA_ROOT.
     Otherwise writes file under media root.
     """
     if is_media_full_path(filename):
         file.name = strip_media_root(filename)  # type: ignore
     else:
         with open(filename, "rb") as fp:
             plain_filename = os.path.basename(filename)
```

### Comparing `django-jbank-4.1.3/jbank/models.py` & `django-jbank-4.2.1/jbank/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -189,17 +189,15 @@
 
     class Meta:
         verbose_name = _("statement record")
         verbose_name_plural = _("statement records")
 
     @property
     def is_settled(self) -> bool:
-        """
-        True if entry is either manually settled or has SUM(children)==amount.
-        """
+        """True if entry is either manually settled or has SUM(children)==amount."""
         return self.manually_settled or sum_queryset(self.child_set) == self.amount  # type: ignore
 
     def clean(self):
         self.source_file = self.statement
         self.timestamp = pytz.utc.localize(datetime.combine(self.record_date, time(0, 0)))
         if self.name:
             self.description = "{name}: {record_description}".format(record_description=self.record_description, name=self.name)
@@ -312,15 +310,16 @@
     def __str__(self):
         return "[{}]".format(self.id)
 
 
 class ReferencePaymentBatchManager(models.Manager):
     def latest_record_date(self) -> Optional[datetime]:
         """
-        :return: datetime of latest record available or None
+        Returns:
+            datetime of latest record available or None
         """
         obj = self.order_by("-record_date").first()
         if not obj:
             return None
         return obj.record_date  # type: ignore
 
 
@@ -348,17 +347,15 @@
     def total_amount(self) -> Decimal:
         return self.get_total_amount()
 
     total_amount.fget.short_description = _("total amount")  # type: ignore
 
 
 class ReferencePaymentRecord(AccountEntry):
-    """
-    Reference payment record. See jacc.Invoice for date/time variable naming conventions.
-    """
+    """Reference payment record. See jacc.Invoice for date/time variable naming conventions."""
 
     objects = PaymentRecordManager()  # type: ignore
     batch = models.ForeignKey(ReferencePaymentBatch, verbose_name=_("batch"), related_name="record_set", on_delete=models.CASCADE)
     line_number = models.SmallIntegerField(_("line number"), default=0, blank=True)
     record_type = SafeCharField(_("record type"), max_length=4, blank=True, default="")
     account_number = SafeCharField(_("account number"), max_length=32, db_index=True)
     record_date = models.DateField(_("record date"), db_index=True)
@@ -380,24 +377,23 @@
 
     class Meta:
         verbose_name = _("reference payment records")
         verbose_name_plural = _("reference payment records")
 
     @property
     def is_settled(self) -> bool:
-        """
-        True if entry is either manually settled or has SUM(children)==amount.
-        """
+        """True if entry is either manually settled or has SUM(children)==amount."""
         return self.manually_settled or sum_queryset(self.child_set) == self.amount  # type: ignore
 
     @property
     def remittance_info_short(self) -> str:
-        """
-        Remittance info without preceding zeroes.
-        :return: str
+        """Remittance info without preceding zeroes.
+
+        Returns:
+            str
         """
         return re.sub(r"^0+", "", self.remittance_info)
 
     def clean(self):
         self.source_file = self.batch
         self.timestamp = pytz.utc.localize(datetime.combine(self.paid_date or self.record_date, time(0, 0)))
         self.description = "{amount} {remittance_info} {payer_name}".format(
@@ -477,26 +473,22 @@
         verbose_name_plural = _("payout parties")
 
     def __str__(self):
         return "{} ({})".format(self.name, self.account_number)
 
     @property
     def is_payout_party_used(self) -> bool:
-        """
-        True if payout party has been used in any payment.
-        """
+        """True if payout party has been used in any payment."""
         if not hasattr(self, "id") or self.id is None:
             return False
         return Payout.objects.all().filter(Q(recipient=self) | Q(payer=self)).exists()
 
     @property
     def is_account_number_changed(self) -> bool:
-        """
-        True if account number has been changed compared to the one stored in DB.
-        """
+        """True if account number has been changed compared to the one stored in DB."""
         if not hasattr(self, "id") or self.id is None:
             return False
         return PayoutParty.objects.all().filter(id=self.id).exclude(account_number=self.account_number).exists()
 
     def clean(self):
         if not self.bic:
             self.bic = iban_bic(self.account_number)
@@ -866,21 +858,24 @@
     def sign_pki_request(self, content: bytes, signing_key_full_path: str, signing_cert_full_path: str) -> bytes:
         return self._sign_request(content, signing_key_full_path, signing_cert_full_path)
 
     def sign_application_request(self, content: bytes) -> bytes:
         return self._sign_request(content, self.signing_key_full_path, self.signing_cert_full_path)
 
     def _sign_request(self, content: bytes, signing_key_full_path: str, signing_cert_full_path: str) -> bytes:
-        """
-        Sign a request.
+        """Sign a request.
         See https://users.dcc.uchile.cl/~pcamacho/tutorial/web/xmlsec/xmlsec.html
-        :param content: XML application request
-        :param signing_key_full_path: Override signing key full path (if not use self.signing_key_full_path)
-        :param signing_cert_full_path: Override signing key full path (if not use self.signing_cert_full_path)
-        :return: str
+
+        Args:
+            content: XML application request
+            signing_key_full_path: Override signing key full path (if not use self.signing_key_full_path)
+            signing_cert_full_path: Override signing key full path (if not use self.signing_cert_full_path)
+
+        Returns:
+            str
         """
         with tempfile.NamedTemporaryFile() as fp:
             fp.write(content)
             fp.flush()
             if self.use_sha256:
                 cmd = [self._xmlsec1_example_bin("sign3-sha256"), fp.name, signing_key_full_path, signing_cert_full_path]
             else:
```

### Comparing `django-jbank-4.1.3/jbank/management/commands/parse_ra.py` & `django-jbank-4.2.1/jbank/management/commands/parse_ra.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/management/commands/make_x509.py` & `django-jbank-4.2.1/jbank/management/commands/make_x509.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/management/commands/test_app_req.py` & `django-jbank-4.2.1/jbank/management/commands/test_app_req.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/management/commands/parse_svm.py` & `django-jbank-4.2.1/jbank/management/commands/parse_svm.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/management/commands/xmlsec1_examples.py` & `django-jbank-4.2.1/jbank/management/commands/xmlsec1_examples.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/management/commands/wsedi_exec.py` & `django-jbank-4.2.1/jbank/management/commands/wsedi_exec.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/management/commands/test_payment.py` & `django-jbank-4.2.1/jbank/management/commands/test_payment.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/management/commands/wsedi_import.py` & `django-jbank-4.2.1/jbank/management/commands/wsedi_import.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/management/commands/wspki_exec.py` & `django-jbank-4.2.1/jbank/management/commands/wspki_exec.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/management/commands/parse_to.py` & `django-jbank-4.2.1/jbank/management/commands/parse_to.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/management/commands/parse_xt.py` & `django-jbank-4.2.1/jbank/management/commands/parse_xt.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/management/commands/test_pain001.py` & `django-jbank-4.2.1/jbank/management/commands/test_pain001.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/management/commands/parse_xm.py` & `django-jbank-4.2.1/jbank/management/commands/parse_xm.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/management/commands/reparse_svm.py` & `django-jbank-4.2.1/jbank/management/commands/reparse_svm.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/management/commands/parse_saldo.py` & `django-jbank-4.2.1/jbank/management/commands/parse_saldo.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/management/commands/make_parse_format.py` & `django-jbank-4.2.1/jbank/management/commands/make_parse_format.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/management/commands/parse_ecb_rates.py` & `django-jbank-4.2.1/jbank/management/commands/parse_ecb_rates.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/management/commands/parse_xp.py` & `django-jbank-4.2.1/jbank/management/commands/parse_xp.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/management/commands/test_xp.py` & `django-jbank-4.2.1/jbank/management/commands/test_xp.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/management/commands/make_pain001.py` & `django-jbank-4.2.1/jbank/management/commands/make_pain001.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/management/commands/reparse_to.py` & `django-jbank-4.2.1/jbank/management/commands/reparse_to.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/management/commands/parse_euribor_rates.py` & `django-jbank-4.2.1/jbank/management/commands/parse_euribor_rates.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/management/commands/wsedi_upload.py` & `django-jbank-4.2.1/jbank/management/commands/wsedi_upload.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # pylint: disable=logging-format-interpolation,too-many-locals
 import logging
 import traceback
 from django.core.management.base import CommandParser
 from jutil.xml import xml_to_dict
 from jbank.models import Payout, PayoutStatus, PAYOUT_ERROR, PAYOUT_WAITING_UPLOAD, PAYOUT_UPLOADED, WsEdiConnection
-from jbank.wsedi import wsedi_upload_file, wsedi_execute
+from jbank.wsedi import wsedi_execute
 from jutil.command import SafeCommand
 
 
 logger = logging.getLogger(__name__)
 
 
 class Command(SafeCommand):
@@ -39,51 +39,44 @@
             payouts = payouts.filter(state=PAYOUT_WAITING_UPLOAD)
             if options["ws"]:
                 payouts = payouts.filter(connection_id=options["ws"])
 
         for p in list(payouts.order_by("id").distinct()):
             assert isinstance(p, Payout)
             p.refresh_from_db()
-            ws_connection = p.connection or default_ws
 
-            if p.state != PAYOUT_WAITING_UPLOAD:
-                logger.info("Skipping {} since not in state PAYOUT_WAITING_UPLOAD".format(p))
-                continue
-            if ws_connection and not ws_connection.enabled:
-                logger.info("WS connection %s not enabled, skipping payment %s", ws_connection, p)
-                continue
+            ws_connection = p.connection or default_ws
+            if ws_connection is None:
+                raise Exception(f"WS-connection not set for {p} and --default-ws is missing")
 
             response_code = ""
             response_text = ""
             try:
+                if p.state != PAYOUT_WAITING_UPLOAD:
+                    logger.info("Skipping %s since not in state PAYOUT_WAITING_UPLOAD", p)
+                    continue
+                if not ws_connection.enabled:
+                    logger.info("WS connection %s not enabled, skipping payment %s", ws_connection, p)
+                    continue
+
                 # upload file
                 logger.info("Uploading payment id={} {} file {}".format(p.id, file_type, p.full_path))
                 with open(p.full_path, "rt", encoding="utf-8") as fp:
                     file_content = fp.read()
                 p.state = PAYOUT_UPLOADED
                 p.save(update_fields=["state"])
-                if ws_connection:
-                    content = wsedi_execute(
-                        ws_connection,
-                        "UploadFile",
-                        file_content=file_content,
-                        file_type=file_type,
-                        verbose=options["verbose"],
-                    )
-                    data = xml_to_dict(content, array_tags=["FileDescriptor"])
-                else:
-                    res = wsedi_upload_file(
-                        file_content=file_content,
-                        file_type=file_type,
-                        file_name=p.file_name,
-                        verbose=options["verbose"],
-                    )
-                    logger.info("HTTP response {}".format(res.status_code))
-                    logger.info(res.text)
-                    data = res.json()
+
+                content = wsedi_execute(
+                    ws_connection,
+                    "UploadFile",
+                    file_content=file_content,
+                    file_type=file_type,
+                    verbose=options["verbose"],
+                )
+                data = xml_to_dict(content, array_tags=["FileDescriptor"])
 
                 # parse response
                 response_code = data.get("ResponseCode", "")[:4]
                 response_text = data.get("ResponseText", "")[:255]
                 if response_code != "00":
                     msg = "WS-EDI file {} upload failed: {} ({})".format(p.file_name, response_text, response_code)
                     logger.error(msg)
```

### Comparing `django-jbank-4.1.3/jbank/management/commands/wsedi_export.py` & `django-jbank-4.2.1/jbank/management/commands/wsedi_export.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/management/commands/parse_aeb43.py` & `django-jbank-4.2.1/jbank/management/commands/parse_aeb43.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/migrations/0008_auto_20210512_2208.py` & `django-jbank-4.2.1/jbank/migrations/0008_auto_20210512_2208.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/migrations/0016_alter_payoutstatus_timestamp.py` & `django-jbank-4.2.1/jbank/migrations/0016_alter_payoutstatus_timestamp.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/migrations/0004_statementfile.py` & `django-jbank-4.2.1/jbank/migrations/0004_statementfile.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/migrations/0001_squashed_0071_wsediconnection_ca_cert_file.py` & `django-jbank-4.2.1/jbank/migrations/0001_squashed_0071_wsediconnection_ca_cert_file.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/migrations/0026_auto_20181205_0034.py` & `django-jbank-4.2.1/jbank/migrations/0026_auto_20181205_0034.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/migrations/0034_auto_20190815_2059.py` & `django-jbank-4.2.1/jbank/migrations/0034_auto_20190815_2059.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/migrations/0007_auto_20171102_2351.py` & `django-jbank-4.2.1/jbank/migrations/0007_auto_20171102_2351.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/migrations/0019_auto_20180209_0437.py` & `django-jbank-4.2.1/jbank/migrations/0019_auto_20180209_0437.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/migrations/0013_auto_20180126_0909.py` & `django-jbank-4.2.1/jbank/migrations/0013_auto_20180126_0909.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/migrations/0023_remove_accountbalance_connection_accountbalance_bic.py` & `django-jbank-4.2.1/jbank/migrations/0023_remove_accountbalance_connection_accountbalance_bic.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/migrations/0015_auto_20180208_0643.py` & `django-jbank-4.2.1/jbank/migrations/0015_auto_20180208_0643.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/migrations/0055_auto_20191130_2011.py` & `django-jbank-4.2.1/jbank/migrations/0055_auto_20191130_2011.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/migrations/0069_auto_20200717_2333.py` & `django-jbank-4.2.1/jbank/migrations/0069_auto_20200717_2333.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/migrations/0041_auto_20191127_0559.py` & `django-jbank-4.2.1/jbank/migrations/0041_auto_20191127_0559.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/migrations/0039_auto_20191127_0156.py` & `django-jbank-4.2.1/jbank/migrations/0039_auto_20191127_0156.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/migrations/0037_auto_20191127_0132.py` & `django-jbank-4.2.1/jbank/migrations/0037_auto_20191127_0132.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/migrations/0008_auto_20171103_0007.py` & `django-jbank-4.2.1/jbank/migrations/0008_auto_20171103_0007.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/migrations/0024_auto_20180425_1704.py` & `django-jbank-4.2.1/jbank/migrations/0024_auto_20180425_1704.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/migrations/0048_wsediconnection_soap_endpoint.py` & `django-jbank-4.2.1/jbank/migrations/0048_wsediconnection_soap_endpoint.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/migrations/0018_auto_20180208_1130.py` & `django-jbank-4.2.1/jbank/migrations/0018_auto_20180208_1130.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/migrations/0005_statementfile_created.py` & `django-jbank-4.2.1/jbank/migrations/0005_statementfile_created.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/migrations/0025_auto_20181101_1430.py` & `django-jbank-4.2.1/jbank/migrations/0025_auto_20181101_1430.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/migrations/0027_auto_20190304_1913.py` & `django-jbank-4.2.1/jbank/migrations/0027_auto_20190304_1913.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/migrations/0036_wsediconnection.py` & `django-jbank-4.2.1/jbank/migrations/0036_wsediconnection.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/migrations/0028_referencepaymentrecord_creditor_bank_bic_and_more.py` & `django-jbank-4.2.1/jbank/migrations/0028_referencepaymentrecord_creditor_bank_bic_and_more.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/migrations/0010_statementrecorddetail_creditor_account_scheme.py` & `django-jbank-4.2.1/jbank/migrations/0010_statementrecorddetail_creditor_account_scheme.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/migrations/0011_auto_20180126_0851.py` & `django-jbank-4.2.1/jbank/migrations/0011_auto_20180126_0851.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/migrations/0051_payout_connection.py` & `django-jbank-4.2.1/jbank/migrations/0051_payout_connection.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/migrations/0018_alter_referencepaymentbatch_currency_identifier_and_more.py` & `django-jbank-4.2.1/jbank/migrations/0018_alter_referencepaymentbatch_currency_identifier_and_more.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/migrations/0003_statement_account.py` & `django-jbank-4.2.1/jbank/migrations/0003_statement_account.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/migrations/0007_auto_20210507_2122.py` & `django-jbank-4.2.1/jbank/migrations/0007_auto_20210507_2122.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/migrations/0012_auto_20180126_0858.py` & `django-jbank-4.2.1/jbank/migrations/0012_auto_20180126_0858.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/migrations/0001_initial.py` & `django-jbank-4.2.1/jbank/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/migrations/0013_euriborrate.py` & `django-jbank-4.2.1/jbank/migrations/0013_euriborrate.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/migrations/0019_alter_payout_state.py` & `django-jbank-4.2.1/jbank/migrations/0019_alter_payout_state.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/migrations/0030_alter_referencepaymentrecord_remittance_info.py` & `django-jbank-4.2.1/jbank/migrations/0030_alter_referencepaymentrecord_remittance_info.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/migrations/0022_accountbalance_connection.py` & `django-jbank-4.2.1/jbank/migrations/0022_accountbalance_connection.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/migrations/0020_accountbalance.py` & `django-jbank-4.2.1/jbank/migrations/0020_accountbalance.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/migrations/0031_wsediconnection_old_encryption_key_file_and_more.py` & `django-jbank-4.2.1/jbank/migrations/0031_wsediconnection_old_encryption_key_file_and_more.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/migrations/0021_auto_20180209_0935.py` & `django-jbank-4.2.1/jbank/migrations/0021_auto_20180209_0935.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/migrations/0043_wsedisoapcall.py` & `django-jbank-4.2.1/jbank/migrations/0043_wsedisoapcall.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/migrations/0006_auto_20210318_2130.py` & `django-jbank-4.2.1/jbank/migrations/0006_auto_20210318_2130.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/migrations/0029_auto_20190727_1352.py` & `django-jbank-4.2.1/jbank/migrations/0029_auto_20190727_1352.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/migrations/0064_auto_20200629_0344.py` & `django-jbank-4.2.1/jbank/migrations/0064_auto_20200629_0344.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/migrations/0062_auto_20200415_2300.py` & `django-jbank-4.2.1/jbank/migrations/0062_auto_20200415_2300.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/migrations/0061_auto_20200325_2204.py` & `django-jbank-4.2.1/jbank/migrations/0061_auto_20200325_2204.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/migrations/0060_auto_20200325_1906.py` & `django-jbank-4.2.1/jbank/migrations/0060_auto_20200325_1906.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/migrations/0026_referencepaymentbatch_identifier_and_more.py` & `django-jbank-4.2.1/jbank/migrations/0026_referencepaymentbatch_identifier_and_more.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/migrations/0029_alter_referencepaymentrecord_remittance_info.py` & `django-jbank-4.2.1/jbank/migrations/0029_alter_referencepaymentrecord_remittance_info.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/migrations/0052_auto_20191130_1927.py` & `django-jbank-4.2.1/jbank/migrations/0052_auto_20191130_1927.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/migrations/0024_referencepaymentbatchfile_additional_info_and_more.py` & `django-jbank-4.2.1/jbank/migrations/0024_referencepaymentbatchfile_additional_info_and_more.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/migrations/0009_auto_20171107_1847.py` & `django-jbank-4.2.1/jbank/migrations/0009_auto_20171107_1847.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/migrations/0016_auto_20180208_0724.py` & `django-jbank-4.2.1/jbank/migrations/0016_auto_20180208_0724.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/migrations/0027_referencepaymentrecord_value_date_and_more.py` & `django-jbank-4.2.1/jbank/migrations/0027_referencepaymentrecord_value_date_and_more.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/migrations/0006_auto_20171102_2341.py` & `django-jbank-4.2.1/jbank/migrations/0006_auto_20171102_2341.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/migrations/0011_referencepaymentbatch_cached_total_amount.py` & `django-jbank-4.2.1/jbank/migrations/0011_referencepaymentbatch_cached_total_amount.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/migrations/0017_payoutparty_payouts_account.py` & `django-jbank-4.2.1/jbank/migrations/0017_payoutparty_payouts_account.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/migrations/0002_auto_20171031_0356.py` & `django-jbank-4.2.1/jbank/migrations/0002_auto_20171031_0356.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/migrations/0012_alter_referencepaymentrecord_delivery_method.py` & `django-jbank-4.2.1/jbank/migrations/0012_alter_referencepaymentrecord_delivery_method.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/migrations/0014_payout_payoutstatus.py` & `django-jbank-4.2.1/jbank/migrations/0014_payout_payoutstatus.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/migrations/0025_auto_20230325_1014.py` & `django-jbank-4.2.1/jbank/migrations/0025_auto_20230325_1014.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/migrations/0002_auto_20200817_2217.py` & `django-jbank-4.2.1/jbank/migrations/0002_auto_20200817_2217.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/migrations/0031_auto_20190727_1639.py` & `django-jbank-4.2.1/jbank/migrations/0031_auto_20190727_1639.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/wspki.py` & `django-jbank-4.2.1/jbank/wspki.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,18 +38,21 @@
     if len(els) > 1:
         return None
     return els[0]
 
 
 def etree_get_element(el: etree.Element, ns: str, tag: str) -> etree.Element:
     """
-    :param el: Root Element
-    :param ns: Target namespace
-    :param tag: Target tag
-    :return: Found Element
+    Args:
+        el: Root Element
+        ns: Target namespace
+        tag: Target tag
+
+    Returns:
+        Found Element
     """
     if not ns.startswith("{"):
         ns = "{" + ns + "}"
     els = list(el.iter("{}{}".format(ns, tag)))
     if not els:
         raise Exception("{} not found from {}".format(tag, el))
     if len(els) > 1:
@@ -326,23 +329,26 @@
     command: str,
     soap_action_header: bool = False,
     xml_sig: bool = False,
     lowercase_environment: bool = False,
     verbose: bool = False,
 ) -> bytes:
     """
-    :param ws:
-    :param payout_party:
-    :param command:
-    :param soap_action_header:
-    :param xml_sig:
-    :param lowercase_environment:
-    :param use_sha256:
-    :param verbose:
-    :return: str
+    Args:
+        ws
+        payout_party
+        command
+        soap_action_header
+        xml_sig
+        lowercase_environment
+        use_sha256
+        verbose
+
+    Returns:
+        str
     """
     if ws and not ws.enabled:
         raise Exception(_("ws.edi.connection.not.enabled").format(ws=ws))
 
     soap_call = WsEdiSoapCall(connection=ws, command=command)
     soap_call.full_clean()
     soap_call.save()
```

### Comparing `django-jbank-4.1.3/jbank/svm.py` & `django-jbank-4.2.1/jbank/svm.py`

 * *Files 3% similar despite different names*

```diff
@@ -135,20 +135,23 @@
     if summary is not None:
         data["summary"] = summary
     return data
 
 
 @transaction.atomic  # noqa
 def create_statement(statement_data: dict, name: str, file: StatementFile, **kw) -> Statement:  # noqa
-    """
-    Creates Statement from statement data parsed by parse_tiliote_statements()
-    :param statement_data: See parse_tiliote_statements
-    :param name: File name of the account statement
-    :param file: Source statement file
-    :return: Statement
+    """Creates Statement from statement data parsed by parse_tiliote_statements()
+
+    Args:
+        statement_data: See parse_tiliote_statements
+        name: File name of the account statement
+        file: Source statement file
+
+    Returns:
+        Statement
     """
     if "header" not in statement_data or not statement_data["header"]:
         raise ValidationError("Invalid header field in statement data {}: {}".format(name, statement_data.get("header")))
     header = statement_data["header"]
 
     account_number = header["account_number"]
     if not account_number:
@@ -204,19 +207,22 @@
             sepa_info.save()
 
     return stm
 
 
 @transaction.atomic
 def create_reference_payment_batch(batch_data: dict, name: str, file: ReferencePaymentBatchFile, **kw) -> ReferencePaymentBatch:
-    """
-    Creates ReferencePaymentBatch from data parsed by parse_svm_batches()
-    :param batch_data: See parse_svm_batches
-    :param name: File name of the batch file
-    :return: ReferencePaymentBatch
+    """Creates ReferencePaymentBatch from data parsed by parse_svm_batches()
+
+    Args:
+        batch_data: See parse_svm_batches
+        name: File name of the batch file
+
+    Returns:
+        ReferencePaymentBatch
     """
     if ReferencePaymentBatch.objects.exclude(file=file).filter(name=name).first():
         raise ValidationError("Reference payment batch file {} already exists".format(name))
 
     if "header" not in batch_data or not batch_data["header"]:
         raise ValidationError("Invalid header field in reference payment batch data {}: {}".format(name, batch_data.get("header")))
     header = batch_data["header"]
```

### Comparing `django-jbank-4.1.3/jbank/services.py` & `django-jbank-4.2.1/jbank/services.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/camt.py` & `django-jbank-4.2.1/jbank/camt.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,20 +176,23 @@
 
 def camt053_get_unified_str(qs, k: str) -> str:
     return camt053_get_unified_val(qs, k, "")
 
 
 @transaction.atomic  # noqa
 def camt053_create_statement(statement_data: dict, name: str, file: StatementFile, **kw) -> Statement:  # noqa
-    """
-    Creates camt.053 Statement from statement data parsed by camt053_parse_statement_from_file()
-    :param statement_data: XML data in form of dict
-    :param name: File name of the account statement
-    :param file: Source statement file
-    :return: Statement
+    """Creates camt.053 Statement from statement data parsed by camt053_parse_statement_from_file()
+
+    Args:
+        statement_data: XML data in form of dict
+        name: File name of the account statement
+        file: Source statement file
+
+    Returns:
+        Statement
     """
     account_number = camt053_get_account_iban(statement_data)
     account_currency = camt053_get_account_currency(statement_data)
     if not account_number:
         raise ValidationError("{name}: ".format(name=name) + _("account.not.found").format(account_number=""))
     accounts = list(Account.objects.filter(name=account_number, currency=account_currency))
     if len(accounts) != 1:
@@ -414,17 +417,15 @@
         )
     with open(filename, "rb") as fp:
         data = xml_to_dict(fp.read(), array_tags=CAMT054_ARRAY_TAGS, int_tags=CAMT054_INT_TAGS)
         return data
 
 
 def camt054_parse_ntfctn_acct(ntfctn: dict, default_currency: str = "EUR") -> Tuple[str, str]:
-    """
-    Returns account_number, currency from Ntfctn
-    """
+    """Returns account_number, currency from Ntfctn"""
     acc_data = ntfctn["Acct"]
     currency = acc_data.get("Ccy") or default_currency
     account_number = acc_data["Id"].get("IBAN") or acc_data["Id"].get("BBAN")
     return account_number, currency
 
 
 def camt054_parse_date(data: dict, key: str) -> date:
```

### Comparing `django-jbank-4.1.3/jbank/tests.py` & `django-jbank-4.2.1/jbank/tests.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/admin.py` & `django-jbank-4.2.1/jbank/admin.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,17 +101,15 @@
             out = "&nbsp;" + value_str[-3:] + out
             value_str = value_str[:-3]
         out = value_str + out
         return mark_safe(out)
 
 
 class SettlementEntryTypesFilter(SimpleListFilter):
-    """
-    Filters incoming settlement type entries.
-    """
+    """Filters incoming settlement type entries."""
 
     title = _("account entry types")
     parameter_name = "type"
 
     def lookups(self, request, model_admin):
         choices = []
         for e in EntryType.objects.all().filter(is_settlement=True).order_by("name"):
@@ -123,17 +121,15 @@
         val = self.value()
         if val:
             return queryset.filter(type__id=val)
         return queryset
 
 
 class AccountEntryMatchedFilter(SimpleListFilter):
-    """
-    Filters incoming payments which do not have any child/derived account entries.
-    """
+    """Filters incoming payments which do not have any child/derived account entries."""
 
     title = _("account.entry.matched.filter")
     parameter_name = "matched"
 
     def lookups(self, request, model_admin):
         return [
             ("1", capfirst(_("account.entry.not.matched"))),
@@ -162,17 +158,15 @@
             if val == "4":
                 # return everything but manually marked as settled
                 return queryset.filter(manually_settled=False)
         return queryset
 
 
 class AccountNameFilter(SimpleListFilter):
-    """
-    Filters account entries based on account name.
-    """
+    """Filters account entries based on account name."""
 
     title = _("account.name.filter")
     parameter_name = "account-name"
 
     def lookups(self, request, model_admin):
         ops = []
         qs = model_admin.get_queryset(request)
```

### Comparing `django-jbank-4.1.3/jbank/aeb43.py` & `django-jbank-4.2.1/jbank/aeb43.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/ecb.py` & `django-jbank-4.2.1/jbank/ecb.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from datetime import datetime
 from decimal import Decimal
 import xml.etree.ElementTree as ET  # noqa
 from urllib import request
 
 
 def parse_euro_exchange_rates_xml(content: str):
-    """
-    Parses Euro currency exchange rates from string.
+    """Parses Euro currency exchange rates from string.
     Format is XML from European Central Bank (http://www.ecb.europa.eu/stats/eurofxref/eurofxref-hist-90d.xml).
     Returns list of (record_date: date, currency: str, rate: str) tuples of Euro exchange rates.
     """
     out = []
     root = ET.fromstring(content)
     cube_tag = "{http://www.ecb.int/vocabulary/2002-08-01/eurofxref}Cube"
     cube = root.findall(cube_tag)[0]
@@ -19,13 +18,12 @@
         for currency_cube in date_cube.findall(cube_tag):
             currency = currency_cube.attrib["currency"]
             out.append((record_date.date(), currency, Decimal(currency_cube.attrib["rate"])))
     return out
 
 
 def download_euro_exchange_rates_xml() -> str:
-    """
-    Downloads Euro currency exchange rates XML file from European Central Bank.
+    """Downloads Euro currency exchange rates XML file from European Central Bank.
     Returns XML as str
     """
     with request.urlopen("http://www.ecb.europa.eu/stats/eurofxref/eurofxref-hist-90d.xml") as conn:
         return conn.read()
```

### Comparing `django-jbank-4.1.3/jbank/sepa.py` & `django-jbank-4.2.1/jbank/sepa.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,17 +87,15 @@
         elif self.remittance_info_type == PAIN001_REMITTANCE_INFO_OCR:
             fi_payment_reference_validator(self.remittance_info)
         elif self.remittance_info_type == PAIN001_REMITTANCE_INFO_OCR_ISO:
             iso_payment_reference_validator(self.remittance_info)
 
 
 class Pain001:
-    """
-    Class for generating pain.001.001.03 SEPA payment XML files.
-    """
+    """Class for generating pain.001.001.03 SEPA payment XML files."""
 
     pain_element_name = "CstmrCdtTrfInitn"
     tz_str = "Europe/Helsinki"
     tz: Any = None
     xml_declaration: Any = None
 
     def __init__(
@@ -480,17 +478,15 @@
     def render_to_file(self, filename: str, xml_bytes: Optional[bytes] = None):
         xml_bytes = xml_bytes or self.render_to_bytes()
         with open(filename, "wb") as fp:
             fp.write(xml_bytes)
 
 
 class Pain002:
-    """
-    Class for parsing pain.002.001.03 SEPA payment status XML files.
-    """
+    """Class for parsing pain.002.001.03 SEPA payment status XML files."""
 
     credit_datetime: datetime
     msg_id: str = ""
     original_msg_id: str = ""
     group_status: str = ""
     status_reason: str = ""
```

### Comparing `django-jbank-4.1.3/jbank/x509_helpers.py` & `django-jbank-4.2.1/jbank/x509_helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,18 +12,19 @@
     """
     with open(filename, "rb") as fp:
         pem_data = fp.read()
     return x509.load_pem_x509_certificate(pem_data, cryptography.hazmat.backends.default_backend())  # noqa
 
 
 def write_cert_pem_file(filename: str, cert_base64: bytes):
-    """
-    Writes PEM data to file.
-    :param filename: PEM filename
-    :param cert_base64: Base64 encoded certificate data without BEGIN CERTIFICATE / END CERTIFICATE
+    """Writes PEM data to file.
+
+    Args:
+        filename: PEM filename
+        cert_base64: Base64 encoded certificate data without BEGIN CERTIFICATE / END CERTIFICATE
     """
     if b"BEGIN" in cert_base64 or b"END" in cert_base64:
         raise ValidationError("write_cert_pem_file() assumes PEM data does not contain header/footer")
     with open(filename, "wb") as fp:
         fp.write(b"-----BEGIN CERTIFICATE-----\n")
         blocks = cert_base64
         while blocks:
```

### Comparing `django-jbank-4.1.3/jbank/parsers.py` & `django-jbank-4.2.1/jbank/parsers.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/csr_helpers.py` & `django-jbank-4.2.1/jbank/csr_helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,18 +23,21 @@
 
 def get_public_key_pem(public_key: RSAPublicKey) -> bytes:
     pem = public_key.public_bytes(encoding=serialization.Encoding.PEM, format=serialization.PublicFormat.SubjectPublicKeyInfo)
     return pem
 
 
 def get_private_key_pem(private_key: RSAPrivateKey) -> bytes:
-    """
-    Returns private key PEM file bytes.
-    :param private_key: RSPrivateKey
-    :return: bytes
+    """Returns private key PEM file bytes.
+
+    Args:
+        private_key: RSPrivateKey
+
+    Returns:
+        bytes
     """
     return private_key.private_bytes(  # type: ignore
         encoding=serialization.Encoding.PEM,
         format=serialization.PrivateFormat.PKCS8,
         encryption_algorithm=serialization.NoEncryption(),
     )
 
@@ -47,31 +50,35 @@
 
 def load_private_key_from_pem_file(filename: str, password: Optional[bytes] = None) -> RSAPrivateKey:
     with open(filename, "rb") as fp:
         return load_private_key_from_pem_data(fp.read(), password)
 
 
 def write_private_key_pem_file(filename: str, key_base64: bytes):
-    """
-    Writes PEM data to file.
-    :param filename: PEM filename
-    :param key_base64: Base64 encoded certificate data without BEGIN CERTIFICATE / END CERTIFICATE
+    """Writes PEM data to file.
+
+    Args:
+        filename: PEM filename
+        key_base64: Base64 encoded certificate data without BEGIN CERTIFICATE / END CERTIFICATE
     """
     if b"BEGIN" not in key_base64 or b"END" not in key_base64:
         raise ValidationError("write_private_key_pem_file() assumes PEM data does contains BEGIN / END header and footer")
     with open(filename, "wb") as fp:
         fp.write(key_base64)
         logger.info("%s written", filename)
 
 
 def strip_pem_header_and_footer(pem: bytes) -> bytes:
-    """
-    Strips -----BEGIN and -----END parts of the CSR PEM.
-    :param pem: bytes
-    :return: bytes
+    """Strips -----BEGIN and -----END parts of the CSR PEM.
+
+    Args:
+        pem: bytes
+
+    Returns:
+        bytes
     """
     if not pem.startswith(b"-----BEGIN "):
         raise Exception("PEM does not appear to have header: {}...".format(pem[:32].decode() + "..."))
     return b"\n".join(pem.split(b"\n")[1:-2])
 
 
 def create_csr_pem(  # pylint: disable=too-many-arguments,too-many-locals
@@ -97,17 +104,18 @@
     state_or_province_name: str = "",
     street_address: str = "",
     surname: str = "",
     title: str = "",
     user_id: str = "",
     x500_unique_identifier: str = "",
 ) -> bytes:
-    """
-    See http://fileformats.archiveteam.org/wiki/PKCS10
-    :return: CSR PEM as bytes
+    """See http://fileformats.archiveteam.org/wiki/PKCS10
+
+    Returns:
+        CSR PEM as bytes
     """
     pairs = [
         (common_name, "COMMON_NAME"),
         (country_name, "COUNTRY_NAME"),
         (dn_qualifier, "DN_QUALIFIER"),
         (business_category, "BUSINESS_CATEGORY"),
         (domain_component, "DOMAIN_COMPONENT"),
```

### Comparing `django-jbank-4.1.3/jbank/files.py` & `django-jbank-4.2.1/jbank/files.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 import os
 from pathlib import Path
 from typing import List
 
 
 def list_dir_files(path: str, suffix: str = "") -> List[str]:
-    """
-    Lists all files (and only files) in a directory, or return [path] if path is a file itself.
-    :param path: Directory or a file
-    :param suffix: Optional suffix to match (case insensitive). Default is none.
-    :return: list of absolute paths to files
+    """Lists all files (and only files) in a directory, or return [path] if path is a file itself.
+
+    Args:
+        path: Directory or a file
+        suffix: Optional suffix to match (case insensitive). Default is none.
+
+    Returns:
+        list of absolute paths to files
     """
     if suffix:
         suffix = suffix.lower()
     if Path(path).is_file():
         files = [os.path.abspath(path)]
     else:
         files = []
```

### Comparing `django-jbank-4.1.3/jbank/templates/admin/jbank/referencepaymentbatch/change_form.html` & `django-jbank-4.2.1/jbank/templates/admin/jbank/referencepaymentbatch/change_form.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/templates/admin/jbank/mark_as_manually_settled.html` & `django-jbank-4.2.1/jbank/templates/admin/jbank/mark_as_manually_settled.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/templates/admin/jbank/statement/change_form.html` & `django-jbank-4.2.1/jbank/templates/admin/jbank/statement/change_form.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/templates/jbank/pki_certificate_status_request_template.xml` & `django-jbank-4.2.1/jbank/templates/jbank/pki_certificate_status_request_template.xml`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/templates/jbank/pki_create_certificate_request_template.xml` & `django-jbank-4.2.1/jbank/templates/jbank/pki_create_certificate_request_template.xml`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/templates/jbank/soap_template.xml` & `django-jbank-4.2.1/jbank/templates/jbank/soap_template.xml`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/templates/jbank/pki_get_certificate_soap_template.xml` & `django-jbank-4.2.1/jbank/templates/jbank/pki_get_certificate_soap_template.xml`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/templates/jbank/pki_renew_certificate_request_template.xml` & `django-jbank-4.2.1/jbank/templates/jbank/pki_renew_certificate_request_template.xml`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/templates/jbank/pki_get_certificate_request_template.xml` & `django-jbank-4.2.1/jbank/templates/jbank/pki_get_certificate_request_template.xml`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/templates/jbank/application_request_template-sha256.xml` & `django-jbank-4.2.1/jbank/templates/jbank/application_request_template-sha256.xml`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/templates/jbank/pki_get_certificate_renew_request_template-sha256.xml` & `django-jbank-4.2.1/jbank/templates/jbank/pki_get_certificate_renew_request_template-sha256.xml`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/templates/jbank/pki_renew_certificate_request_template-sha256.xml` & `django-jbank-4.2.1/jbank/templates/jbank/pki_renew_certificate_request_template-sha256.xml`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/templates/jbank/application_request_template.xml` & `django-jbank-4.2.1/jbank/templates/jbank/application_request_template.xml`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/templates/jbank/encryption_template.xml` & `django-jbank-4.2.1/jbank/templates/jbank/encryption_template.xml`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/templates/jbank/enveloping-sha256-rsa-sha256.xml` & `django-jbank-4.2.1/jbank/templates/jbank/enveloping-sha256-rsa-sha256.xml`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/templates/jbank/pki_get_certificate_renew_request_template.xml` & `django-jbank-4.2.1/jbank/templates/jbank/pki_get_certificate_renew_request_template.xml`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/templates/jbank/pki_soap_template.xml` & `django-jbank-4.2.1/jbank/templates/jbank/pki_soap_template.xml`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/locale/fi/LC_MESSAGES/django.mo` & `django-jbank-4.2.1/jbank/locale/fi/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/locale/fi/LC_MESSAGES/django.po` & `django-jbank-4.2.1/jbank/locale/fi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/locale/en/LC_MESSAGES/django.mo` & `django-jbank-4.2.1/jbank/locale/en/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/locale/en/LC_MESSAGES/django.po` & `django-jbank-4.2.1/jbank/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/xmlsec1-examples/Makefile` & `django-jbank-4.2.1/jbank/xmlsec1-examples/Makefile`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/xmlsec1-examples/encrypt3.c` & `django-jbank-4.2.1/jbank/xmlsec1-examples/encrypt3.c`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/xmlsec1-examples/sign3.c` & `django-jbank-4.2.1/jbank/xmlsec1-examples/sign3.c`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/xmlsec1-examples/decrypt3.c` & `django-jbank-4.2.1/jbank/xmlsec1-examples/decrypt3.c`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/xmlsec1-examples/verify3.c` & `django-jbank-4.2.1/jbank/xmlsec1-examples/verify3.c`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/xmlsec1-examples/sign3-sha256.c` & `django-jbank-4.2.1/jbank/xmlsec1-examples/sign3-sha256.c`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/pain002.py` & `django-jbank-4.2.1/jbank/pain002.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/euribor.py` & `django-jbank-4.2.1/jbank/euribor.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.3/jbank/tito.py` & `django-jbank-4.2.1/jbank/tito.py`

 * *Files identical despite different names*

