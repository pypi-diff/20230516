# Comparing `tmp/openimis-be-invoice-1.5.0.tar.gz` & `tmp/openimis-be-invoice-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openimis-be-invoice-1.5.0.tar", last modified: Fri Nov 11 08:12:11 2022, max compression
+gzip compressed data, was "openimis-be-invoice-1.5.1.tar", last modified: Tue May 16 21:38:47 2023, max compression
```

## Comparing `openimis-be-invoice-1.5.0.tar` & `openimis-be-invoice-1.5.1.tar`

### file list

```diff
@@ -1,130 +1,131 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 08:12:11.061965 openimis-be-invoice-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (121)    34523 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      717 2022-11-11 08:12:11.061965 openimis-be-invoice-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 08:12:11.045965 openimis-be-invoice-1.5.0/invoice/
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)     6841 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 08:12:11.049965 openimis-be-invoice-1.5.0/invoice/gql/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/gql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 08:12:11.049965 openimis-be-invoice-1.5.0/invoice/gql/bill/
--rw-r--r--   0 runner    (1001) docker     (121)      107 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/gql/bill/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      912 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/gql/bill/mutation.py
--rw-r--r--   0 runner    (1001) docker     (121)     1722 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/gql/bill/query.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 08:12:11.049965 openimis-be-invoice-1.5.0/invoice/gql/bill_event/
--rw-r--r--   0 runner    (1001) docker     (121)      128 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/gql/bill_event/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2565 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/gql/bill_event/mutation.py
--rw-r--r--   0 runner    (1001) docker     (121)     1463 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/gql/bill_event/query.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 08:12:11.049965 openimis-be-invoice-1.5.0/invoice/gql/bill_item/
--rw-r--r--   0 runner    (1001) docker     (121)       59 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/gql/bill_item/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/gql/bill_item/mutation.py
--rw-r--r--   0 runner    (1001) docker     (121)     1580 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/gql/bill_item/query.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 08:12:11.049965 openimis-be-invoice-1.5.0/invoice/gql/bill_payment/
--rw-r--r--   0 runner    (1001) docker     (121)       65 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/gql/bill_payment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2721 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/gql/bill_payment/mutation.py
--rw-r--r--   0 runner    (1001) docker     (121)     1482 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/gql/bill_payment/query.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 08:12:11.049965 openimis-be-invoice-1.5.0/invoice/gql/detail_payment_invoice/
--rw-r--r--   0 runner    (1001) docker     (121)       84 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/gql/detail_payment_invoice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3268 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/gql/detail_payment_invoice/mutation.py
--rw-r--r--   0 runner    (1001) docker     (121)     1562 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/gql/detail_payment_invoice/query.py
--rw-r--r--   0 runner    (1001) docker     (121)     5429 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/gql/filter_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 08:12:11.049965 openimis-be-invoice-1.5.0/invoice/gql/gql_types/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/gql/gql_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4948 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/gql/gql_types/bill_types.py
--rw-r--r--   0 runner    (1001) docker     (121)     5491 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/gql/gql_types/invoice_types.py
--rw-r--r--   0 runner    (1001) docker     (121)     2047 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/gql/gql_types/payment_types.py
--rw-r--r--   0 runner    (1001) docker     (121)     4679 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/gql/input_types.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 08:12:11.053965 openimis-be-invoice-1.5.0/invoice/gql/invoice/
--rw-r--r--   0 runner    (1001) docker     (121)      146 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/gql/invoice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2944 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/gql/invoice/mutation.py
--rw-r--r--   0 runner    (1001) docker     (121)     1754 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/gql/invoice/query.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 08:12:11.053965 openimis-be-invoice-1.5.0/invoice/gql/invoice_event/
--rw-r--r--   0 runner    (1001) docker     (121)       68 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/gql/invoice_event/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2614 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/gql/invoice_event/mutation.py
--rw-r--r--   0 runner    (1001) docker     (121)     1495 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/gql/invoice_event/query.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 08:12:11.053965 openimis-be-invoice-1.5.0/invoice/gql/invoice_line_item/
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/gql/invoice_line_item/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/gql/invoice_line_item/mutation.py
--rw-r--r--   0 runner    (1001) docker     (121)     1660 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/gql/invoice_line_item/query.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 08:12:11.053965 openimis-be-invoice-1.5.0/invoice/gql/invoice_payment/
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/gql/invoice_payment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2737 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/gql/invoice_payment/mutation.py
--rw-r--r--   0 runner    (1001) docker     (121)     1513 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/gql/invoice_payment/query.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 08:12:11.053965 openimis-be-invoice-1.5.0/invoice/gql/payment_invoice/
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/gql/payment_invoice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5360 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/gql/payment_invoice/mutation.py
--rw-r--r--   0 runner    (1001) docker     (121)     1790 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/gql/payment_invoice/query.py
--rw-r--r--   0 runner    (1001) docker     (121)      598 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/gql/query_mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 08:12:11.057965 openimis-be-invoice-1.5.0/invoice/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)    57283 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/migrations/0001_initial_migration.py
--rw-r--r--   0 runner    (1001) docker     (121)     1119 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/migrations/0002_auto_20211117_0904.py
--rw-r--r--   0 runner    (1001) docker     (121)     1072 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/migrations/0003_auto_20211203_1053.py
--rw-r--r--   0 runner    (1001) docker     (121)     2672 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/migrations/0004_invoice_bill_roles_for_admin.py
--rw-r--r--   0 runner    (1001) docker     (121)     2648 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/migrations/0005_invoice_bill_roles_for_accountant.py
--rw-r--r--   0 runner    (1001) docker     (121)    11594 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/migrations/0006_detailpaymentinvoice_historicaldetailpaymentinvoice_historicalpaymentinvoice_paymentinvoice.py
--rw-r--r--   0 runner    (1001) docker     (121)      710 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/migrations/0007_auto_20220411_1053.py
--rw-r--r--   0 runner    (1001) docker     (121)      556 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/migrations/0008_auto_20220411_1358.py
--rw-r--r--   0 runner    (1001) docker     (121)     2489 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/migrations/0009_auto_20220413_0824.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      897 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/mixins.py
--rw-r--r--   0 runner    (1001) docker     (121)    15240 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     5634 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 08:12:11.057965 openimis-be-invoice-1.5.0/invoice/services/
--rw-r--r--   0 runner    (1001) docker     (121)      362 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3542 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/services/bill.py
--rw-r--r--   0 runner    (1001) docker     (121)     2992 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/services/billLineItem.py
--rw-r--r--   0 runner    (1001) docker     (121)     4149 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/services/invoice.py
--rw-r--r--   0 runner    (1001) docker     (121)     3121 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/services/invoiceLineItem.py
--rw-r--r--   0 runner    (1001) docker     (121)     3649 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/services/invoicePayments.py
--rw-r--r--   0 runner    (1001) docker     (121)     5664 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/services/paymentInvoice.py
--rw-r--r--   0 runner    (1001) docker     (121)      996 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 08:12:11.057965 openimis-be-invoice-1.5.0/invoice/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 08:12:11.057965 openimis-be-invoice-1.5.0/invoice/tests/gql/
--rw-r--r--   0 runner    (1001) docker     (121)      227 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/tests/gql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2056 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/tests/gql/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     6138 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/tests/gql/detail_payment_invoice_schema.py
--rw-r--r--   0 runner    (1001) docker     (121)     2039 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/tests/gql/invoice_event_schema.py
--rw-r--r--   0 runner    (1001) docker     (121)     1353 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/tests/gql/invoice_line_item_schema.py
--rw-r--r--   0 runner    (1001) docker     (121)     5517 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/tests/gql/invoice_payment_schema.py
--rw-r--r--   0 runner    (1001) docker     (121)     3037 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/tests/gql/invoice_schema.py
--rw-r--r--   0 runner    (1001) docker     (121)     9241 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/tests/gql/payment_invoice_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 08:12:11.061965 openimis-be-invoice-1.5.0/invoice/tests/helpers/
--rw-r--r--   0 runner    (1001) docker     (121)      781 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/tests/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1722 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/tests/helpers/bill_helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1607 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/tests/helpers/bill_line_item_helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)      798 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/tests/helpers/bill_payment_helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     3867 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/tests/helpers/default_test_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     1745 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/tests/helpers/invoice_helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1802 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/tests/helpers/invoice_line_item_helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)      834 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/tests/helpers/invoice_payment_helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1878 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/tests/helpers/payment_invoice_helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     2129 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/tests/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 08:12:11.061965 openimis-be-invoice-1.5.0/invoice/tests/services/
--rw-r--r--   0 runner    (1001) docker     (121)      114 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/tests/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12998 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/tests/services/invoice.py
--rw-r--r--   0 runner    (1001) docker     (121)     6766 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/tests/services/invoiceLineItem.py
--rw-r--r--   0 runner    (1001) docker     (121)    12661 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/tests/services/invoicePayment.py
--rw-r--r--   0 runner    (1001) docker     (121)     7940 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/tests/services/paymentInvoice.py
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)     1369 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 08:12:11.061965 openimis-be-invoice-1.5.0/invoice/validation/
--rw-r--r--   0 runner    (1001) docker     (121)      471 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2122 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/validation/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     2193 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/validation/bill.py
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/validation/billLineItem.py
--rw-r--r--   0 runner    (1001) docker     (121)     2227 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/validation/invoice.py
--rw-r--r--   0 runner    (1001) docker     (121)      186 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/validation/invoiceLineItem.py
--rw-r--r--   0 runner    (1001) docker     (121)     2743 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/validation/invoicePayment.py
--rw-r--r--   0 runner    (1001) docker     (121)     3155 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/validation/paymentInvoice.py
--rw-r--r--   0 runner    (1001) docker     (121)     4761 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/validation/paymentStatusValidation.py
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-11-11 08:12:01.000000 openimis-be-invoice-1.5.0/invoice/views.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 08:12:11.061965 openimis-be-invoice-1.5.0/openimis_be_invoice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      717 2022-11-11 08:12:11.000000 openimis-be-invoice-1.5.0/openimis_be_invoice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3797 2022-11-11 08:12:11.000000 openimis-be-invoice-1.5.0/openimis_be_invoice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-11 08:12:11.000000 openimis-be-invoice-1.5.0/openimis_be_invoice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-11-11 08:12:11.000000 openimis-be-invoice-1.5.0/openimis_be_invoice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-11-11 08:12:11.000000 openimis-be-invoice-1.5.0/openimis_be_invoice.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-11 08:12:11.061965 openimis-be-invoice-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1219 2022-11-11 08:12:10.000000 openimis-be-invoice-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:47.798473 openimis-be-invoice-1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-16 21:38:47.798473 openimis-be-invoice-1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:47.790473 openimis-be-invoice-1.5.1/invoice/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6841 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:47.790473 openimis-be-invoice-1.5.1/invoice/gql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/gql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:47.790473 openimis-be-invoice-1.5.1/invoice/gql/bill/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/gql/bill/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/gql/bill/mutation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/gql/bill/query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:47.790473 openimis-be-invoice-1.5.1/invoice/gql/bill_event/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/gql/bill_event/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/gql/bill_event/mutation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/gql/bill_event/query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:47.790473 openimis-be-invoice-1.5.1/invoice/gql/bill_item/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/gql/bill_item/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/gql/bill_item/mutation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/gql/bill_item/query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:47.790473 openimis-be-invoice-1.5.1/invoice/gql/bill_payment/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/gql/bill_payment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/gql/bill_payment/mutation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/gql/bill_payment/query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:47.790473 openimis-be-invoice-1.5.1/invoice/gql/detail_payment_invoice/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/gql/detail_payment_invoice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/gql/detail_payment_invoice/mutation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/gql/detail_payment_invoice/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5429 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/gql/filter_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:47.790473 openimis-be-invoice-1.5.1/invoice/gql/gql_types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/gql/gql_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6304 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/gql/gql_types/bill_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/gql/gql_types/invoice_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/gql/gql_types/payment_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4679 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/gql/input_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:47.790473 openimis-be-invoice-1.5.1/invoice/gql/invoice/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/gql/invoice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/gql/invoice/mutation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/gql/invoice/query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:47.794473 openimis-be-invoice-1.5.1/invoice/gql/invoice_event/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/gql/invoice_event/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/gql/invoice_event/mutation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/gql/invoice_event/query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:47.794473 openimis-be-invoice-1.5.1/invoice/gql/invoice_line_item/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/gql/invoice_line_item/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/gql/invoice_line_item/mutation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/gql/invoice_line_item/query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:47.794473 openimis-be-invoice-1.5.1/invoice/gql/invoice_payment/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/gql/invoice_payment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/gql/invoice_payment/mutation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/gql/invoice_payment/query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:47.794473 openimis-be-invoice-1.5.1/invoice/gql/payment_invoice/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/gql/payment_invoice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5360 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/gql/payment_invoice/mutation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/gql/payment_invoice/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/gql/query_mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:47.794473 openimis-be-invoice-1.5.1/invoice/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)    57283 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/migrations/0001_initial_migration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/migrations/0002_auto_20211117_0904.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/migrations/0003_auto_20211203_1053.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/migrations/0004_invoice_bill_roles_for_admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/migrations/0005_invoice_bill_roles_for_accountant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11594 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/migrations/0006_detailpaymentinvoice_historicaldetailpaymentinvoice_historicalpaymentinvoice_paymentinvoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/migrations/0007_auto_20220411_1053.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/migrations/0008_auto_20220411_1358.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/migrations/0009_auto_20220413_0824.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/migrations/0010_auto_20230126_0903.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15277 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:47.794473 openimis-be-invoice-1.5.1/invoice/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/services/bill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/services/billLineItem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/services/invoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/services/invoiceLineItem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3649 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/services/invoicePayments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5664 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/services/paymentInvoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:47.794473 openimis-be-invoice-1.5.1/invoice/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:47.794473 openimis-be-invoice-1.5.1/invoice/tests/gql/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/tests/gql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/tests/gql/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/tests/gql/detail_payment_invoice_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/tests/gql/invoice_event_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/tests/gql/invoice_line_item_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5517 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/tests/gql/invoice_payment_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/tests/gql/invoice_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9241 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/tests/gql/payment_invoice_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:47.798473 openimis-be-invoice-1.5.1/invoice/tests/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/tests/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/tests/helpers/bill_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/tests/helpers/bill_line_item_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/tests/helpers/bill_payment_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/tests/helpers/default_test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/tests/helpers/invoice_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/tests/helpers/invoice_line_item_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/tests/helpers/invoice_payment_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/tests/helpers/payment_invoice_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/tests/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:47.798473 openimis-be-invoice-1.5.1/invoice/tests/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/tests/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12998 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/tests/services/invoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/tests/services/invoiceLineItem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12661 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/tests/services/invoicePayment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7940 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/tests/services/paymentInvoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:47.798473 openimis-be-invoice-1.5.1/invoice/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/validation/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/validation/bill.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/validation/billLineItem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/validation/invoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/validation/invoiceLineItem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/validation/invoicePayment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/validation/paymentInvoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/validation/paymentStatusValidation.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-16 21:38:37.000000 openimis-be-invoice-1.5.1/invoice/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:47.798473 openimis-be-invoice-1.5.1/openimis_be_invoice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-16 21:38:47.000000 openimis-be-invoice-1.5.1/openimis_be_invoice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-05-16 21:38:47.000000 openimis-be-invoice-1.5.1/openimis_be_invoice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 21:38:47.000000 openimis-be-invoice-1.5.1/openimis_be_invoice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-16 21:38:47.000000 openimis-be-invoice-1.5.1/openimis_be_invoice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-16 21:38:47.000000 openimis-be-invoice-1.5.1/openimis_be_invoice.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 21:38:47.798473 openimis-be-invoice-1.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-16 21:38:47.000000 openimis-be-invoice-1.5.1/setup.py
```

### Comparing `openimis-be-invoice-1.5.0/LICENSE` & `openimis-be-invoice-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.5.0/PKG-INFO` & `openimis-be-invoice-1.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-invoice
-Version: 1.5.0
+Version: 1.5.1
 Summary: The openIMIS Backend Invoice Payment reference module.
 Home-page: https://openimis.org/
 Author: Damian Borowiecki
 Author-email: dborowiecki@soldevelo.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-invoice-1.5.0/invoice/apps.py` & `openimis-be-invoice-1.5.1/invoice/apps.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.5.0/invoice/gql/bill/mutation.py` & `openimis-be-invoice-1.5.1/invoice/gql/bill/mutation.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.5.0/invoice/gql/bill/query.py` & `openimis-be-invoice-1.5.1/invoice/gql/invoice/query.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import graphene
 from django.contrib.auth.models import AnonymousUser
 from django.db.models import Q
 
 from core.schema import OrderedDjangoFilterConnectionField
 from core.utils import append_validity_filter
 from invoice.apps import InvoiceConfig
-from invoice.gql.gql_types.bill_types import BillGQLType
-from invoice.models import Bill
+from invoice.gql.gql_types.invoice_types import InvoiceGQLType
+from invoice.models import Invoice
 import graphene_django_optimizer as gql_optimizer
 
 
-class BillQueryMixin:
-    bill = OrderedDjangoFilterConnectionField(
-        BillGQLType,
+class InvoiceQueryMixin:
+    invoice = OrderedDjangoFilterConnectionField(
+        InvoiceGQLType,
         orderBy=graphene.List(of_type=graphene.String),
         dateValidFrom__Gte=graphene.DateTime(),
         dateValidTo__Lte=graphene.DateTime(),
         applyDefaultValidityFilter=graphene.Boolean(),
-        client_mutation_id=graphene.String(),
+        client_mutation_id=graphene.String()
     )
 
-    def resolve_bill(self, info, **kwargs):
+    def resolve_invoice(self, info, **kwargs):
         filters = []
         filters += append_validity_filter(**kwargs)
 
         client_mutation_id = kwargs.get("client_mutation_id", None)
         if client_mutation_id:
             filters.append(Q(mutations__mutation__client_mutation_id=client_mutation_id))
 
@@ -32,15 +32,18 @@
         if subject_type:
             filters.append(Q(subject_type__model=subject_type))
 
         thirdparty_type = kwargs.get("thirdparty_type", None)
         if thirdparty_type:
             filters.append(Q(thirdparty_type__model=thirdparty_type))
 
-        BillQueryMixin._check_permissions(info.context.user)
-        return gql_optimizer.query(Bill.objects.filter(*filters).all(), info)
+        InvoiceQueryMixin._check_permissions(info.context.user)
+        return gql_optimizer.query(Invoice.objects.filter(*filters).all(), info)
 
     @staticmethod
     def _check_permissions(user):
         if type(user) is AnonymousUser or not user.id or not user.has_perms(
-                InvoiceConfig.gql_bill_search_perms):
+                InvoiceConfig.gql_invoice_search_perms):
             raise PermissionError("Unauthorized")
+
+
+
```

### Comparing `openimis-be-invoice-1.5.0/invoice/gql/bill_event/mutation.py` & `openimis-be-invoice-1.5.1/invoice/gql/bill_event/mutation.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.5.0/invoice/gql/bill_event/query.py` & `openimis-be-invoice-1.5.1/invoice/gql/bill_event/query.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.5.0/invoice/gql/bill_item/query.py` & `openimis-be-invoice-1.5.1/invoice/gql/bill_item/query.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.5.0/invoice/gql/bill_payment/mutation.py` & `openimis-be-invoice-1.5.1/invoice/gql/bill_payment/mutation.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.5.0/invoice/gql/bill_payment/query.py` & `openimis-be-invoice-1.5.1/invoice/gql/bill_payment/query.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.5.0/invoice/gql/detail_payment_invoice/mutation.py` & `openimis-be-invoice-1.5.1/invoice/gql/detail_payment_invoice/mutation.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.5.0/invoice/gql/detail_payment_invoice/query.py` & `openimis-be-invoice-1.5.1/invoice/gql/detail_payment_invoice/query.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.5.0/invoice/gql/filter_mixin.py` & `openimis-be-invoice-1.5.1/invoice/gql/filter_mixin.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.5.0/invoice/gql/gql_types/bill_types.py` & `openimis-be-invoice-1.5.1/invoice/gql/gql_types/bill_types.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,42 +1,55 @@
 import graphene
 import json
 from django.contrib.contenttypes.models import ContentType
 from django.core.serializers.json import DjangoJSONEncoder
 from graphene_django import DjangoObjectType
 
 from core import prefix_filterset, ExtendedConnection
+from invoice.apps import InvoiceConfig
 from invoice.gql.filter_mixin import GenericFilterGQLTypeMixin
 from invoice.models import Bill, \
     BillItem, BillEvent, BillPayment
 from invoice.utils import underscore_to_camel
 from location.models import Location
 from product.models import Product
+from django.core.exceptions import PermissionDenied
+from django.utils.translation import gettext as _
 
 
 class BillGQLType(DjangoObjectType, GenericFilterGQLTypeMixin):
 
     subject_type = graphene.Int()
     def resolve_subject_type(root, info):
+        if not info.context.user.has_perms(InvoiceConfig.gql_bill_search_perms):
+            raise PermissionDenied(_("unauthorized"))
         return root.subject_type.id
 
     subject_type_name = graphene.String()
     def resolve_subject_type_name(root, info):
+        if not info.context.user.has_perms(InvoiceConfig.gql_bill_search_perms):
+            raise PermissionDenied(_("unauthorized"))
         return root.subject_type.name
 
     thirdparty_type = graphene.Int()
     def resolve_thirdparty_type(root, info):
+        if not info.context.user.has_perms(InvoiceConfig.gql_bill_search_perms):
+            raise PermissionDenied(_("unauthorized"))
         return root.thirdparty_type.id
 
     thirdparty_type_name = graphene.String()
     def resolve_thirdparty_type_name(root, info):
+        if not info.context.user.has_perms(InvoiceConfig.gql_bill_search_perms):
+            raise PermissionDenied(_("unauthorized"))
         return root.thirdparty_type.name
 
     subject = graphene.JSONString()
     def resolve_subject(root, info):
+        if not info.context.user.has_perms(InvoiceConfig.gql_bill_search_perms):
+            raise PermissionDenied(_("unauthorized"))
         subject_object_dict = root.subject.__dict__
         subject_object_dict.pop('_state')
         subject_object_dict = {
             underscore_to_camel(k): v for k, v in list(subject_object_dict.items())
         }
         if root.subject_type.name == "batch run":
             location = Location.objects.filter(id=subject_object_dict['locationId'], validity_to__isnull=True)
@@ -45,14 +58,16 @@
                 underscore_to_camel(k): v for k, v in location.first().items()
             }
         subject_object_dict = json.dumps(subject_object_dict, cls=DjangoJSONEncoder)
         return subject_object_dict
 
     thirdparty = graphene.JSONString()
     def resolve_thirdparty(root, info):
+        if not info.context.user.has_perms(InvoiceConfig.gql_bill_search_perms):
+            raise PermissionDenied(_("unauthorized"))
         thirdparty_object_dict = root.thirdparty.__dict__
         thirdparty_object_dict.pop('_state')
         thirdparty_object_dict = {
             underscore_to_camel(k): v for k, v in list(thirdparty_object_dict.items())
         }
         thirdparty_object_dict = json.dumps(thirdparty_object_dict, cls=DjangoJSONEncoder)
         return thirdparty_object_dict
@@ -72,22 +87,28 @@
             return Bill.get_queryset(queryset, info)
 
 
 class BillItemGQLType(DjangoObjectType, GenericFilterGQLTypeMixin):
 
     line_type = graphene.Int()
     def resolve_line_type(root, info):
+        if not info.context.user.has_perms(InvoiceConfig.gql_bill_search_perms):
+            raise PermissionDenied(_("unauthorized"))
         return root.line_type.id
 
     line_type_name = graphene.String()
     def resolve_line_type_name(root, info):
+        if not info.context.user.has_perms(InvoiceConfig.gql_bill_search_perms):
+            raise PermissionDenied(_("unauthorized"))
         return root.line_type.name
 
     line = graphene.JSONString()
     def resolve_line(root, info):
+        if not info.context.user.has_perms(InvoiceConfig.gql_bill_search_perms):
+            raise PermissionDenied(_("unauthorized"))
         line_object_dict = root.line.__dict__
         line_object_dict.pop('_state')
         key_values = list(line_object_dict.items())
         line_object_dict.clear()
         for k, v in key_values:
             new_key = underscore_to_camel(k)
             line_object_dict[new_key] = v
```

### Comparing `openimis-be-invoice-1.5.0/invoice/gql/gql_types/invoice_types.py` & `openimis-be-invoice-1.5.1/invoice/gql/gql_types/invoice_types.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,40 +1,53 @@
 import graphene
 import json
 from django.core.serializers.json import DjangoJSONEncoder
 from graphene_django import DjangoObjectType
 
 from core import prefix_filterset, ExtendedConnection
 from insuree.models import Insuree
+from invoice.apps import InvoiceConfig
 from invoice.gql.filter_mixin import GenericFilterGQLTypeMixin
 from invoice.models import Invoice, InvoiceLineItem, InvoicePayment, InvoiceEvent, InvoiceMutation, \
     InvoicePaymentMutation, InvoiceLineItemMutation, InvoiceEventMutation
 from invoice.utils import underscore_to_camel
+from django.core.exceptions import PermissionDenied
+from django.utils.translation import gettext as _
 
 
 class InvoiceGQLType(DjangoObjectType, GenericFilterGQLTypeMixin):
 
     subject_type = graphene.Int()
     def resolve_subject_type(root, info):
+        if not info.context.user.has_perms(InvoiceConfig.gql_invoice_search_perms):
+            raise PermissionDenied(_("unauthorized"))
         return root.subject_type.id
 
     subject_type_name = graphene.String()
     def resolve_subject_type_name(root, info):
+        if not info.context.user.has_perms(InvoiceConfig.gql_invoice_search_perms):
+            raise PermissionDenied(_("unauthorized"))
         return root.subject_type.name
 
     thirdparty_type = graphene.Int()
     def resolve_thirdparty_type(root, info):
+        if not info.context.user.has_perms(InvoiceConfig.gql_invoice_search_perms):
+            raise PermissionDenied(_("unauthorized"))
         return root.thirdparty_type.id
 
     thirdparty_type_name = graphene.String()
     def resolve_thirdparty_type_name(root, info):
+        if not info.context.user.has_perms(InvoiceConfig.gql_invoice_search_perms):
+            raise PermissionDenied(_("unauthorized"))
         return root.thirdparty_type.name
 
     subject = graphene.JSONString()
     def resolve_subject(root, info):
+        if not info.context.user.has_perms(InvoiceConfig.gql_invoice_search_perms):
+            raise PermissionDenied(_("unauthorized"))
         subject_object_dict = root.subject.__dict__
         subject_object_dict.pop('_state')
         subject_object_dict = {
             underscore_to_camel(k): v for k, v in list(subject_object_dict.items())
         }
         if root.subject_type.name == "family":
             insuree = Insuree.objects.filter(id=subject_object_dict['headInsureeId'], validity_to__isnull=True)
@@ -43,14 +56,16 @@
                 underscore_to_camel(k): v for k, v in insuree.first().items()
             }
         subject_object_dict = json.dumps(subject_object_dict, cls=DjangoJSONEncoder)
         return subject_object_dict
 
     thirdparty = graphene.JSONString()
     def resolve_thirdparty(root, info):
+        if not info.context.user.has_perms(InvoiceConfig.gql_invoice_search_perms):
+            raise PermissionDenied(_("unauthorized"))
         thirdparty_object_dict = root.thirdparty.__dict__
         thirdparty_object_dict.pop('_state')
         thirdparty_object_dict = {
             underscore_to_camel(k): v for k, v in list(thirdparty_object_dict.items())
         }
         thirdparty_object_dict = json.dumps(thirdparty_object_dict, cls=DjangoJSONEncoder)
         return thirdparty_object_dict
@@ -70,22 +85,28 @@
             return Invoice.get_queryset(queryset, info)
 
 
 class InvoiceLineItemGQLType(DjangoObjectType, GenericFilterGQLTypeMixin):
 
     line_type = graphene.Int()
     def resolve_line_type(root, info):
+        if not info.context.user.has_perms(InvoiceConfig.gql_invoice_search_perms):
+            raise PermissionDenied(_("unauthorized"))
         return root.line_type.id
 
     line_type_name = graphene.String()
     def resolve_line_type_name(root, info):
+        if not info.context.user.has_perms(InvoiceConfig.gql_invoice_search_perms):
+            raise PermissionDenied(_("unauthorized"))
         return root.line_type.name
 
     line = graphene.JSONString()
     def resolve_line(root, info):
+        if not info.context.user.has_perms(InvoiceConfig.gql_invoice_search_perms):
+            raise PermissionDenied(_("unauthorized"))
         line_object_dict = root.line.__dict__
         line_object_dict.pop('_state')
         key_values = list(line_object_dict.items())
         line_object_dict.clear()
         for k, v in key_values:
             new_key = underscore_to_camel(k)
             line_object_dict[new_key] = v
```

### Comparing `openimis-be-invoice-1.5.0/invoice/gql/gql_types/payment_types.py` & `openimis-be-invoice-1.5.1/invoice/gql/gql_types/payment_types.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 import json
 import graphene
 
 from django.core.serializers.json import DjangoJSONEncoder
 from graphene_django import DjangoObjectType
 
 from core import prefix_filterset, ExtendedConnection
+from invoice.apps import InvoiceConfig
 from invoice.gql.filter_mixin import GenericFilterGQLTypeMixin
 from invoice.models import PaymentInvoice, DetailPaymentInvoice
 from invoice.utils import underscore_to_camel
+from django.utils.translation import gettext as _
+from django.core.exceptions import PermissionDenied
 
 
 class PaymentInvoiceGQLType(DjangoObjectType, GenericFilterGQLTypeMixin):
 
     class Meta:
         model = PaymentInvoice
         interfaces = (graphene.relay.Node,)
@@ -26,22 +29,28 @@
             return PaymentInvoice.get_queryset(queryset, info)
 
 
 class DetailPaymentInvoiceGQLType(DjangoObjectType, GenericFilterGQLTypeMixin):
 
     subject_type = graphene.Int()
     def resolve_subject_type(root, info):
+        if not info.context.user.has_perms(InvoiceConfig.gql_invoice_payment_search_perms):
+            raise PermissionDenied(_("unauthorized"))
         return root.subject_type.id
 
     subject_type_name = graphene.String()
     def resolve_subject_type_name(root, info):
+        if not info.context.user.has_perms(InvoiceConfig.gql_invoice_payment_search_perms):
+            raise PermissionDenied(_("unauthorized"))
         return root.subject_type.name
 
     subject = graphene.JSONString()
     def resolve_subject(root, info):
+        if not info.context.user.has_perms(InvoiceConfig.gql_invoice_payment_search_perms):
+            raise PermissionDenied(_("unauthorized"))
         subject_object_dict = root.subject.__dict__
         subject_object_dict.pop('_state')
         subject_object_dict = {
             underscore_to_camel(k): v for k, v in list(subject_object_dict.items())
         }
         subject_object_dict = json.dumps(subject_object_dict, cls=DjangoJSONEncoder)
         return subject_object_dict
```

### Comparing `openimis-be-invoice-1.5.0/invoice/gql/input_types.py` & `openimis-be-invoice-1.5.1/invoice/gql/input_types.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.5.0/invoice/gql/invoice/mutation.py` & `openimis-be-invoice-1.5.1/invoice/gql/invoice/mutation.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.5.0/invoice/gql/invoice/query.py` & `openimis-be-invoice-1.5.1/invoice/gql/invoice_event/query.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,49 +1,40 @@
 import graphene
 from django.contrib.auth.models import AnonymousUser
 from django.db.models import Q
 
 from core.schema import OrderedDjangoFilterConnectionField
 from core.utils import append_validity_filter
 from invoice.apps import InvoiceConfig
-from invoice.gql.gql_types.invoice_types import InvoiceGQLType
-from invoice.models import Invoice
+from invoice.gql.gql_types.invoice_types import InvoiceEventGQLType
+from invoice.models import InvoiceEvent
 import graphene_django_optimizer as gql_optimizer
 
 
-class InvoiceQueryMixin:
-    invoice = OrderedDjangoFilterConnectionField(
-        InvoiceGQLType,
+class InvoiceEventQueryMixin:
+    invoice_event = OrderedDjangoFilterConnectionField(
+        InvoiceEventGQLType,
         orderBy=graphene.List(of_type=graphene.String),
         dateValidFrom__Gte=graphene.DateTime(),
         dateValidTo__Lte=graphene.DateTime(),
         applyDefaultValidityFilter=graphene.Boolean(),
-        client_mutation_id=graphene.String()
+        client_mutation_id=graphene.String(),
     )
 
-    def resolve_invoice(self, info, **kwargs):
+    def resolve_invoice_event(self, info, **kwargs):
         filters = []
         filters += append_validity_filter(**kwargs)
 
         client_mutation_id = kwargs.get("client_mutation_id", None)
         if client_mutation_id:
             filters.append(Q(mutations__mutation__client_mutation_id=client_mutation_id))
 
-        subject_type = kwargs.get("subject_type", None)
-        if subject_type:
-            filters.append(Q(subject_type__model=subject_type))
-
-        thirdparty_type = kwargs.get("thirdparty_type", None)
-        if thirdparty_type:
-            filters.append(Q(thirdparty_type__model=thirdparty_type))
-
-        InvoiceQueryMixin._check_permissions(info.context.user)
-        return gql_optimizer.query(Invoice.objects.filter(*filters).all(), info)
+        InvoiceEventQueryMixin._check_permissions(info.context.user)
+        return gql_optimizer.query(InvoiceEvent.objects.filter(*filters).all(), info)
 
     @staticmethod
     def _check_permissions(user):
         if type(user) is AnonymousUser or not user.id or not user.has_perms(
-                InvoiceConfig.gql_invoice_search_perms):
+                InvoiceConfig.gql_invoice_event_search_perms):
             raise PermissionError("Unauthorized")
 
 
-
```

### Comparing `openimis-be-invoice-1.5.0/invoice/gql/invoice_event/mutation.py` & `openimis-be-invoice-1.5.1/invoice/gql/invoice_event/mutation.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.5.0/invoice/gql/invoice_event/query.py` & `openimis-be-invoice-1.5.1/invoice/gql/invoice_payment/query.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 import graphene
 from django.contrib.auth.models import AnonymousUser
 from django.db.models import Q
 
 from core.schema import OrderedDjangoFilterConnectionField
 from core.utils import append_validity_filter
 from invoice.apps import InvoiceConfig
-from invoice.gql.gql_types.invoice_types import InvoiceEventGQLType
-from invoice.models import InvoiceEvent
+from invoice.gql.gql_types.invoice_types import InvoicePaymentGQLType
+from invoice.models import InvoicePayment
 import graphene_django_optimizer as gql_optimizer
 
 
-class InvoiceEventQueryMixin:
-    invoice_event = OrderedDjangoFilterConnectionField(
-        InvoiceEventGQLType,
+class InvoicePaymentQueryMixin:
+    invoice_payment = OrderedDjangoFilterConnectionField(
+        InvoicePaymentGQLType,
         orderBy=graphene.List(of_type=graphene.String),
         dateValidFrom__Gte=graphene.DateTime(),
         dateValidTo__Lte=graphene.DateTime(),
         applyDefaultValidityFilter=graphene.Boolean(),
         client_mutation_id=graphene.String(),
     )
 
-    def resolve_invoice_event(self, info, **kwargs):
+    def resolve_invoice_payment(self, info, **kwargs):
         filters = []
         filters += append_validity_filter(**kwargs)
 
         client_mutation_id = kwargs.get("client_mutation_id", None)
         if client_mutation_id:
             filters.append(Q(mutations__mutation__client_mutation_id=client_mutation_id))
 
-        InvoiceEventQueryMixin._check_permissions(info.context.user)
-        return gql_optimizer.query(InvoiceEvent.objects.filter(*filters).all(), info)
+        InvoicePaymentQueryMixin._check_permissions(info.context.user)
+        return gql_optimizer.query(InvoicePayment.objects.filter(*filters).all(), info)
 
     @staticmethod
     def _check_permissions(user):
         if type(user) is AnonymousUser or not user.id or not user.has_perms(
-                InvoiceConfig.gql_invoice_event_search_perms):
+                InvoiceConfig.gql_invoice_payment_search_perms):
             raise PermissionError("Unauthorized")
```

### Comparing `openimis-be-invoice-1.5.0/invoice/gql/invoice_line_item/query.py` & `openimis-be-invoice-1.5.1/invoice/gql/invoice_line_item/query.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.5.0/invoice/gql/invoice_payment/mutation.py` & `openimis-be-invoice-1.5.1/invoice/gql/invoice_payment/mutation.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.5.0/invoice/gql/invoice_payment/query.py` & `openimis-be-invoice-1.5.1/invoice/gql/payment_invoice/query.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,48 @@
 import graphene
+import graphene_django_optimizer as gql_optimizer
+
 from django.contrib.auth.models import AnonymousUser
 from django.db.models import Q
 
 from core.schema import OrderedDjangoFilterConnectionField
 from core.utils import append_validity_filter
 from invoice.apps import InvoiceConfig
-from invoice.gql.gql_types.invoice_types import InvoicePaymentGQLType
-from invoice.models import InvoicePayment
-import graphene_django_optimizer as gql_optimizer
+from invoice.gql.gql_types.payment_types import PaymentInvoiceGQLType
+from invoice.models import PaymentInvoice
 
 
-class InvoicePaymentQueryMixin:
-    invoice_payment = OrderedDjangoFilterConnectionField(
-        InvoicePaymentGQLType,
+class PaymentInvoiceQueryMixin:
+    payment_invoice = OrderedDjangoFilterConnectionField(
+        PaymentInvoiceGQLType,
         orderBy=graphene.List(of_type=graphene.String),
+        subjectIds=graphene.List(of_type=graphene.UUID),
         dateValidFrom__Gte=graphene.DateTime(),
         dateValidTo__Lte=graphene.DateTime(),
         applyDefaultValidityFilter=graphene.Boolean(),
         client_mutation_id=graphene.String(),
     )
 
-    def resolve_invoice_payment(self, info, **kwargs):
+    def resolve_payment_invoice(self, info, **kwargs):
         filters = []
         filters += append_validity_filter(**kwargs)
 
+        query = PaymentInvoice.objects
+
+        subject_ids = kwargs.get('subjectIds', None)
+        if subject_ids:
+            query = query.filter(
+                invoice_payments__subject_id__in=subject_ids
+            ).distinct()
+
         client_mutation_id = kwargs.get("client_mutation_id", None)
         if client_mutation_id:
             filters.append(Q(mutations__mutation__client_mutation_id=client_mutation_id))
 
-        InvoicePaymentQueryMixin._check_permissions(info.context.user)
-        return gql_optimizer.query(InvoicePayment.objects.filter(*filters).all(), info)
+        PaymentInvoiceQueryMixin._check_permissions(info.context.user)
+        return gql_optimizer.query(query.filter(*filters).all(), info)
 
     @staticmethod
     def _check_permissions(user):
         if type(user) is AnonymousUser or not user.id or not user.has_perms(
                 InvoiceConfig.gql_invoice_payment_search_perms):
             raise PermissionError("Unauthorized")
-
-
```

### Comparing `openimis-be-invoice-1.5.0/invoice/gql/payment_invoice/mutation.py` & `openimis-be-invoice-1.5.1/invoice/gql/payment_invoice/mutation.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.5.0/invoice/gql/query_mixins.py` & `openimis-be-invoice-1.5.1/invoice/gql/query_mixins.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.5.0/invoice/migrations/0001_initial_migration.py` & `openimis-be-invoice-1.5.1/invoice/migrations/0001_initial_migration.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.5.0/invoice/migrations/0002_auto_20211117_0904.py` & `openimis-be-invoice-1.5.1/invoice/migrations/0002_auto_20211117_0904.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.5.0/invoice/migrations/0003_auto_20211203_1053.py` & `openimis-be-invoice-1.5.1/invoice/migrations/0003_auto_20211203_1053.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.5.0/invoice/migrations/0004_invoice_bill_roles_for_admin.py` & `openimis-be-invoice-1.5.1/invoice/migrations/0004_invoice_bill_roles_for_admin.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.5.0/invoice/migrations/0005_invoice_bill_roles_for_accountant.py` & `openimis-be-invoice-1.5.1/invoice/migrations/0005_invoice_bill_roles_for_accountant.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.5.0/invoice/migrations/0006_detailpaymentinvoice_historicaldetailpaymentinvoice_historicalpaymentinvoice_paymentinvoice.py` & `openimis-be-invoice-1.5.1/invoice/migrations/0006_detailpaymentinvoice_historicaldetailpaymentinvoice_historicalpaymentinvoice_paymentinvoice.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.5.0/invoice/migrations/0007_auto_20220411_1053.py` & `openimis-be-invoice-1.5.1/invoice/migrations/0007_auto_20220411_1053.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.5.0/invoice/migrations/0008_auto_20220411_1358.py` & `openimis-be-invoice-1.5.1/invoice/migrations/0008_auto_20220411_1358.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.5.0/invoice/migrations/0009_auto_20220413_0824.py` & `openimis-be-invoice-1.5.1/invoice/migrations/0009_auto_20220413_0824.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.5.0/invoice/mixins.py` & `openimis-be-invoice-1.5.1/invoice/mixins.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.5.0/invoice/models.py` & `openimis-be-invoice-1.5.1/invoice/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -179,15 +179,16 @@
     class Meta:
         managed = True
         db_table = 'tblInvoiceEvent'
 
 
 class Bill(GenericInvoice):
     subject_type = models.ForeignKey(ContentType, models.DO_NOTHING,
-                                        db_column='SubjectType', null=True, related_name='subject_type_bill', unique=False)
+                                        db_column='SubjectType', null=True, related_name='subject_type_bill',
+                                     unique=False)
     subject_id = models.CharField(db_column='SubjectId', max_length=255, null=True)  # object is referenced by uuid
     subject = GenericForeignKey('subject_type', 'subject_id')
 
     date_bill = DateField(db_column='DateBill', default=date.today, null=True)
 
     class Meta:
         managed = True
```

### Comparing `openimis-be-invoice-1.5.0/invoice/schema.py` & `openimis-be-invoice-1.5.1/invoice/schema.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.5.0/invoice/services/bill.py` & `openimis-be-invoice-1.5.1/invoice/services/bill.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.5.0/invoice/services/billLineItem.py` & `openimis-be-invoice-1.5.1/invoice/services/billLineItem.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.5.0/invoice/services/invoice.py` & `openimis-be-invoice-1.5.1/invoice/services/invoice.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.5.0/invoice/services/invoiceLineItem.py` & `openimis-be-invoice-1.5.1/invoice/services/invoiceLineItem.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.5.0/invoice/services/invoicePayments.py` & `openimis-be-invoice-1.5.1/invoice/services/invoicePayments.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.5.0/invoice/services/paymentInvoice.py` & `openimis-be-invoice-1.5.1/invoice/services/paymentInvoice.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.5.0/invoice/signals.py` & `openimis-be-invoice-1.5.1/invoice/signals.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.5.0/invoice/tests/gql/base.py` & `openimis-be-invoice-1.5.1/invoice/tests/gql/base.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.5.0/invoice/tests/gql/detail_payment_invoice_schema.py` & `openimis-be-invoice-1.5.1/invoice/tests/gql/detail_payment_invoice_schema.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.5.0/invoice/tests/gql/invoice_event_schema.py` & `openimis-be-invoice-1.5.1/invoice/tests/gql/invoice_event_schema.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.5.0/invoice/tests/gql/invoice_line_item_schema.py` & `openimis-be-invoice-1.5.1/invoice/tests/gql/invoice_line_item_schema.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.5.0/invoice/tests/gql/invoice_payment_schema.py` & `openimis-be-invoice-1.5.1/invoice/tests/gql/invoice_payment_schema.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.5.0/invoice/tests/gql/invoice_schema.py` & `openimis-be-invoice-1.5.1/invoice/tests/gql/invoice_schema.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.5.0/invoice/tests/gql/payment_invoice_schema.py` & `openimis-be-invoice-1.5.1/invoice/tests/gql/payment_invoice_schema.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.5.0/invoice/tests/helpers/__init__.py` & `openimis-be-invoice-1.5.1/invoice/tests/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.5.0/invoice/tests/helpers/bill_helpers.py` & `openimis-be-invoice-1.5.1/invoice/tests/helpers/bill_helpers.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.5.0/invoice/tests/helpers/bill_line_item_helpers.py` & `openimis-be-invoice-1.5.1/invoice/tests/helpers/bill_line_item_helpers.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.5.0/invoice/tests/helpers/bill_payment_helpers.py` & `openimis-be-invoice-1.5.1/invoice/tests/helpers/bill_payment_helpers.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.5.0/invoice/tests/helpers/default_test_data.py` & `openimis-be-invoice-1.5.1/invoice/tests/helpers/default_test_data.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.5.0/invoice/tests/helpers/invoice_helpers.py` & `openimis-be-invoice-1.5.1/invoice/tests/helpers/invoice_helpers.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.5.0/invoice/tests/helpers/invoice_line_item_helpers.py` & `openimis-be-invoice-1.5.1/invoice/tests/helpers/invoice_line_item_helpers.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.5.0/invoice/tests/helpers/invoice_payment_helpers.py` & `openimis-be-invoice-1.5.1/invoice/tests/helpers/invoice_payment_helpers.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.5.0/invoice/tests/helpers/payment_invoice_helpers.py` & `openimis-be-invoice-1.5.1/invoice/tests/helpers/payment_invoice_helpers.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.5.0/invoice/tests/helpers.py` & `openimis-be-invoice-1.5.1/invoice/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.5.0/invoice/tests/services/invoice.py` & `openimis-be-invoice-1.5.1/invoice/tests/services/invoice.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.5.0/invoice/tests/services/invoiceLineItem.py` & `openimis-be-invoice-1.5.1/invoice/tests/services/invoiceLineItem.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.5.0/invoice/tests/services/invoicePayment.py` & `openimis-be-invoice-1.5.1/invoice/tests/services/invoicePayment.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.5.0/invoice/tests/services/paymentInvoice.py` & `openimis-be-invoice-1.5.1/invoice/tests/services/paymentInvoice.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.5.0/invoice/utils.py` & `openimis-be-invoice-1.5.1/invoice/utils.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.5.0/invoice/validation/base.py` & `openimis-be-invoice-1.5.1/invoice/validation/base.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.5.0/invoice/validation/bill.py` & `openimis-be-invoice-1.5.1/invoice/validation/bill.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.5.0/invoice/validation/invoice.py` & `openimis-be-invoice-1.5.1/invoice/validation/invoice.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.5.0/invoice/validation/invoicePayment.py` & `openimis-be-invoice-1.5.1/invoice/validation/invoicePayment.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.5.0/invoice/validation/paymentInvoice.py` & `openimis-be-invoice-1.5.1/invoice/validation/paymentInvoice.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.5.0/invoice/validation/paymentStatusValidation.py` & `openimis-be-invoice-1.5.1/invoice/validation/paymentStatusValidation.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.5.0/openimis_be_invoice.egg-info/PKG-INFO` & `openimis-be-invoice-1.5.1/openimis_be_invoice.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-invoice
-Version: 1.5.0
+Version: 1.5.1
 Summary: The openIMIS Backend Invoice Payment reference module.
 Home-page: https://openimis.org/
 Author: Damian Borowiecki
 Author-email: dborowiecki@soldevelo.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-invoice-1.5.0/openimis_be_invoice.egg-info/SOURCES.txt` & `openimis-be-invoice-1.5.1/openimis_be_invoice.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -54,14 +54,15 @@
 invoice/migrations/0003_auto_20211203_1053.py
 invoice/migrations/0004_invoice_bill_roles_for_admin.py
 invoice/migrations/0005_invoice_bill_roles_for_accountant.py
 invoice/migrations/0006_detailpaymentinvoice_historicaldetailpaymentinvoice_historicalpaymentinvoice_paymentinvoice.py
 invoice/migrations/0007_auto_20220411_1053.py
 invoice/migrations/0008_auto_20220411_1358.py
 invoice/migrations/0009_auto_20220413_0824.py
+invoice/migrations/0010_auto_20230126_0903.py
 invoice/migrations/__init__.py
 invoice/services/__init__.py
 invoice/services/bill.py
 invoice/services/billLineItem.py
 invoice/services/invoice.py
 invoice/services/invoiceLineItem.py
 invoice/services/invoicePayments.py
```

### Comparing `openimis-be-invoice-1.5.0/setup.py` & `openimis-be-invoice-1.5.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='openimis-be-invoice',
-    version='1.5.0',
+    version='v1.5.1',
     packages=find_packages(),
     include_package_data=True,
     license='GNU AGPL v3',
     description='The openIMIS Backend Invoice Payment reference module.',
     long_description=README,
     long_description_content_type='text/markdown',
     url='https://openimis.org/',
```

