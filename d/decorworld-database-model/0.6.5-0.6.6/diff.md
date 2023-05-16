# Comparing `tmp/decorworld_database_model-0.6.5.tar.gz` & `tmp/decorworld_database_model-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decorworld_database_model-0.6.5.tar", max compression
+gzip compressed data, was "decorworld_database_model-0.6.6.tar", max compression
```

## Comparing `decorworld_database_model-0.6.5.tar` & `decorworld_database_model-0.6.6.tar`

### file list

```diff
@@ -1,54 +1,149 @@
--rw-r--r--   0        0        0        0 2022-11-14 11:28:19.771512 decorworld_database_model-0.6.5/decorworld_database_model/__init__.py
--rw-r--r--   0        0        0     2058 2022-11-14 11:36:26.543490 decorworld_database_model-0.6.5/decorworld_database_model/alembic/env.py
--rw-r--r--   0        0        0       38 2022-11-14 11:28:32.706440 decorworld_database_model-0.6.5/decorworld_database_model/alembic/README
--rw-r--r--   0        0        0      510 2022-11-14 11:28:32.707432 decorworld_database_model-0.6.5/decorworld_database_model/alembic/script.py.mako
--rw-r--r--   0        0        0     1091 2022-11-17 17:32:55.256233 decorworld_database_model-0.6.5/decorworld_database_model/alembic/versions/082d80622e74_create_order_item_table.py
--rw-r--r--   0        0        0     1176 2023-04-27 06:22:16.258902 decorworld_database_model-0.6.5/decorworld_database_model/alembic/versions/13a3b750c40e_add_pre_order_and_discount_columns_to_.py
--rw-r--r--   0        0        0     1056 2023-04-27 09:21:00.015484 decorworld_database_model-0.6.5/decorworld_database_model/alembic/versions/143be2620e05_rename_preorder_column_in_products_table.py
--rw-r--r--   0        0        0      833 2022-11-25 16:07:54.940915 decorworld_database_model-0.6.5/decorworld_database_model/alembic/versions/1f52b78d99b5_add_page_images_table.py
--rw-r--r--   0        0        0     1313 2023-04-27 06:20:08.624820 decorworld_database_model-0.6.5/decorworld_database_model/alembic/versions/21550951e198_drop_discounts_table.py
--rw-r--r--   0        0        0      949 2023-04-27 07:48:45.244503 decorworld_database_model-0.6.5/decorworld_database_model/alembic/versions/26cdf6a5af2b_change_discount_type_to_integer_from_.py
--rw-r--r--   0        0        0      923 2022-11-14 11:36:28.443321 decorworld_database_model-0.6.5/decorworld_database_model/alembic/versions/28e24bf5b755_create_user_table.py
--rw-r--r--   0        0        0      971 2022-11-17 17:39:09.649589 decorworld_database_model-0.6.5/decorworld_database_model/alembic/versions/3afcf5045272_create_favorite_table.py
--rw-r--r--   0        0        0     1093 2022-11-17 17:32:22.727240 decorworld_database_model-0.6.5/decorworld_database_model/alembic/versions/41640c6fbc41_create_product_table.py
--rw-r--r--   0        0        0      709 2022-11-27 07:47:32.279073 decorworld_database_model-0.6.5/decorworld_database_model/alembic/versions/432183be6e50_add_role_column_to_user_table.py
--rw-r--r--   0        0        0     1260 2023-04-27 07:36:26.657915 decorworld_database_model-0.6.5/decorworld_database_model/alembic/versions/437ce57390c5_remove_active_discount_column_and_.py
--rw-r--r--   0        0        0     1034 2022-11-25 13:12:14.766306 decorworld_database_model-0.6.5/decorworld_database_model/alembic/versions/46fe20e7d2c8_add_reviews_table.py
--rw-r--r--   0        0        0      741 2023-03-29 08:51:06.588874 decorworld_database_model-0.6.5/decorworld_database_model/alembic/versions/4cfd3fc062af_add_date_column_to_review.py
--rw-r--r--   0        0        0     2041 2022-11-17 17:20:22.941546 decorworld_database_model-0.6.5/decorworld_database_model/alembic/versions/556ff2c83f9f_create_order_table.py
--rw-r--r--   0        0        0      870 2022-11-17 17:19:16.180388 decorworld_database_model-0.6.5/decorworld_database_model/alembic/versions/57c6c9633e32_create_shipping_method_table.py
--rw-r--r--   0        0        0      943 2022-11-17 17:41:41.614167 decorworld_database_model-0.6.5/decorworld_database_model/alembic/versions/6787273bd08d_create_image_table.py
--rw-r--r--   0        0        0      852 2022-11-19 09:43:34.355183 decorworld_database_model-0.6.5/decorworld_database_model/alembic/versions/68b8e7a46dc0_add_contact_columns_to_order_table.py
--rw-r--r--   0        0        0     1039 2022-11-17 09:29:10.463996 decorworld_database_model-0.6.5/decorworld_database_model/alembic/versions/72c749f78b2c_add_registratrion_activation_and_update_.py
--rw-r--r--   0        0        0     1073 2022-11-17 17:37:07.585121 decorworld_database_model-0.6.5/decorworld_database_model/alembic/versions/7561a3637af6_create_discount_table.py
--rw-r--r--   0        0        0      746 2022-11-14 16:04:04.381269 decorworld_database_model-0.6.5/decorworld_database_model/alembic/versions/76e56ad9a0d6_add_active_column_to_users_table.py
--rw-r--r--   0        0        0     1241 2022-11-17 15:39:46.868782 decorworld_database_model-0.6.5/decorworld_database_model/alembic/versions/824f9117cea4_create_invoice_data_table.py
--rw-r--r--   0        0        0      790 2022-11-17 17:31:37.522016 decorworld_database_model-0.6.5/decorworld_database_model/alembic/versions/88d8f0924ac3_create_category_table.py
--rw-r--r--   0        0        0      948 2022-12-01 09:11:30.894051 decorworld_database_model-0.6.5/decorworld_database_model/alembic/versions/8f89b8df2fba_enable_longer_name_for_product.py
--rw-r--r--   0        0        0      706 2022-11-17 18:49:14.442466 decorworld_database_model-0.6.5/decorworld_database_model/alembic/versions/905e714689ea_add_description_column_to_product_table.py
--rw-r--r--   0        0        0      866 2022-11-17 17:19:57.038988 decorworld_database_model-0.6.5/decorworld_database_model/alembic/versions/94537a354aba_create_payment_method_table.py
--rw-r--r--   0        0        0     1103 2022-11-17 14:11:09.276179 decorworld_database_model-0.6.5/decorworld_database_model/alembic/versions/a2a05856eb15_create_address_table.py
--rw-r--r--   0        0        0      880 2022-11-19 09:34:42.463405 decorworld_database_model-0.6.5/decorworld_database_model/alembic/versions/ade770eba952_add_description_columns_to_order_table.py
--rw-r--r--   0        0        0      877 2022-11-25 14:27:47.383698 decorworld_database_model-0.6.5/decorworld_database_model/alembic/versions/b2424975cff5_modify_review_description_to_nullable.py
--rw-r--r--   0        0        0      698 2022-11-17 15:39:42.615558 decorworld_database_model-0.6.5/decorworld_database_model/alembic/versions/d190af5edcec_add_name_column_to_address_table.py
--rw-r--r--   0        0        0      835 2022-11-21 17:24:22.320177 decorworld_database_model-0.6.5/decorworld_database_model/alembic/versions/dc6a7a4506e7_add_order_number_column_to_order_table.py
--rw-r--r--   0        0        0      735 2023-04-27 06:35:08.361160 decorworld_database_model-0.6.5/decorworld_database_model/alembic/versions/fd54dd612c6e_add_uploaded_column_to_products_table.py
--rw-r--r--   0        0        0     3234 2022-11-14 11:34:58.943979 decorworld_database_model-0.6.5/decorworld_database_model/alembic.ini
--rw-r--r--   0        0        0      449 2023-04-27 06:18:17.177337 decorworld_database_model-0.6.5/decorworld_database_model/tables/__init__.py
--rw-r--r--   0        0        0     1143 2022-11-17 15:24:28.613902 decorworld_database_model-0.6.5/decorworld_database_model/tables/address.py
--rw-r--r--   0        0        0      160 2022-11-14 11:30:54.004559 decorworld_database_model-0.6.5/decorworld_database_model/tables/base.py
--rw-r--r--   0        0        0      628 2023-04-27 06:17:17.160232 decorworld_database_model-0.6.5/decorworld_database_model/tables/category.py
--rw-r--r--   0        0        0      790 2023-04-27 06:17:17.107376 decorworld_database_model-0.6.5/decorworld_database_model/tables/favorite.py
--rw-r--r--   0        0        0      784 2023-04-27 06:17:17.113356 decorworld_database_model-0.6.5/decorworld_database_model/tables/image.py
--rw-r--r--   0        0        0     1290 2023-04-27 06:17:17.082439 decorworld_database_model-0.6.5/decorworld_database_model/tables/invoice_data.py
--rw-r--r--   0        0        0     4192 2023-04-27 06:17:17.094407 decorworld_database_model-0.6.5/decorworld_database_model/tables/order.py
--rw-r--r--   0        0        0     1184 2022-11-27 10:47:07.768493 decorworld_database_model-0.6.5/decorworld_database_model/tables/order_item.py
--rw-r--r--   0        0        0      647 2022-11-25 16:07:28.582459 decorworld_database_model-0.6.5/decorworld_database_model/tables/page_image.py
--rw-r--r--   0        0        0      733 2023-04-27 06:17:17.101389 decorworld_database_model-0.6.5/decorworld_database_model/tables/payment_method.py
--rw-r--r--   0        0        0     1872 2023-04-27 09:19:32.565184 decorworld_database_model-0.6.5/decorworld_database_model/tables/product.py
--rw-r--r--   0        0        0     1328 2023-03-29 08:51:06.589872 decorworld_database_model-0.6.5/decorworld_database_model/tables/review.py
--rw-r--r--   0        0        0      740 2023-04-27 06:17:17.167212 decorworld_database_model-0.6.5/decorworld_database_model/tables/shipping_method.py
--rw-r--r--   0        0        0     1507 2022-11-27 07:46:49.104190 decorworld_database_model-0.6.5/decorworld_database_model/tables/user.py
--rw-r--r--   0        0        0      405 2023-04-27 09:21:00.120825 decorworld_database_model-0.6.5/pyproject.toml
--rw-r--r--   0        0        0      805 2023-04-27 09:21:44.793653 decorworld_database_model-0.6.5/setup.py
--rw-r--r--   0        0        0      479 2023-04-27 09:21:44.793653 decorworld_database_model-0.6.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2022-11-14 11:28:19.771512 decorworld_database_model-0.6.6/decorworld_database_model/__init__.py
+-rw-r--r--   0        0        0     1627 2022-11-14 11:36:28.291746 decorworld_database_model-0.6.6/decorworld_database_model/alembic/__pycache__/env.cpython-38.pyc
+-rw-r--r--   0        0        0     1687 2023-05-16 07:37:52.460283 decorworld_database_model-0.6.6/decorworld_database_model/alembic/__pycache__/env.cpython-39.pyc
+-rw-r--r--   0        0        0     2058 2022-11-14 11:36:26.543490 decorworld_database_model-0.6.6/decorworld_database_model/alembic/env.py
+-rw-r--r--   0        0        0       38 2022-11-14 11:28:32.706440 decorworld_database_model-0.6.6/decorworld_database_model/alembic/README
+-rw-r--r--   0        0        0      510 2022-11-14 11:28:32.707432 decorworld_database_model-0.6.6/decorworld_database_model/alembic/script.py.mako
+-rw-r--r--   0        0        0     1091 2022-11-17 17:32:55.256233 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/082d80622e74_create_order_item_table.py
+-rw-r--r--   0        0        0     1176 2023-04-27 06:22:16.258902 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/13a3b750c40e_add_pre_order_and_discount_columns_to_.py
+-rw-r--r--   0        0        0     1056 2023-04-27 09:21:00.015484 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/143be2620e05_rename_preorder_column_in_products_table.py
+-rw-r--r--   0        0        0      833 2022-11-25 16:07:54.940915 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/1f52b78d99b5_add_page_images_table.py
+-rw-r--r--   0        0        0     1313 2023-04-27 06:20:08.624820 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/21550951e198_drop_discounts_table.py
+-rw-r--r--   0        0        0      949 2023-04-27 07:48:45.244503 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/26cdf6a5af2b_change_discount_type_to_integer_from_.py
+-rw-r--r--   0        0        0      923 2022-11-14 11:36:28.443321 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/28e24bf5b755_create_user_table.py
+-rw-r--r--   0        0        0      971 2022-11-17 17:39:09.649589 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/3afcf5045272_create_favorite_table.py
+-rw-r--r--   0        0        0     1093 2022-11-17 17:32:22.727240 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/41640c6fbc41_create_product_table.py
+-rw-r--r--   0        0        0      709 2022-11-27 07:47:32.279073 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/432183be6e50_add_role_column_to_user_table.py
+-rw-r--r--   0        0        0     1260 2023-04-27 07:36:26.657915 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/437ce57390c5_remove_active_discount_column_and_.py
+-rw-r--r--   0        0        0     1034 2022-11-25 13:12:14.766306 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/46fe20e7d2c8_add_reviews_table.py
+-rw-r--r--   0        0        0      741 2023-03-29 08:51:06.588874 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/4cfd3fc062af_add_date_column_to_review.py
+-rw-r--r--   0        0        0     2041 2022-11-17 17:20:22.941546 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/556ff2c83f9f_create_order_table.py
+-rw-r--r--   0        0        0      870 2022-11-17 17:19:16.180388 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/57c6c9633e32_create_shipping_method_table.py
+-rw-r--r--   0        0        0      943 2022-11-17 17:41:41.614167 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/6787273bd08d_create_image_table.py
+-rw-r--r--   0        0        0      852 2022-11-19 09:43:34.355183 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/68b8e7a46dc0_add_contact_columns_to_order_table.py
+-rw-r--r--   0        0        0     1039 2022-11-17 09:29:10.463996 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/72c749f78b2c_add_registratrion_activation_and_update_.py
+-rw-r--r--   0        0        0     1073 2022-11-17 17:37:07.585121 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/7561a3637af6_create_discount_table.py
+-rw-r--r--   0        0        0      746 2022-11-14 16:04:04.381269 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/76e56ad9a0d6_add_active_column_to_users_table.py
+-rw-r--r--   0        0        0     1241 2022-11-17 15:39:46.868782 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/824f9117cea4_create_invoice_data_table.py
+-rw-r--r--   0        0        0      790 2022-11-17 17:31:37.522016 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/88d8f0924ac3_create_category_table.py
+-rw-r--r--   0        0        0      948 2022-12-01 09:11:30.894051 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/8f89b8df2fba_enable_longer_name_for_product.py
+-rw-r--r--   0        0        0      706 2022-11-17 18:49:14.442466 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/905e714689ea_add_description_column_to_product_table.py
+-rw-r--r--   0        0        0      866 2022-11-17 17:19:57.038988 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/94537a354aba_create_payment_method_table.py
+-rw-r--r--   0        0        0     1126 2022-11-17 17:32:55.256233 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/__pycache__/082d80622e74_create_order_item_table.cpython-38.pyc
+-rw-r--r--   0        0        0     1126 2023-05-16 07:38:44.369071 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/__pycache__/082d80622e74_create_order_item_table.cpython-39.pyc
+-rw-r--r--   0        0        0     1205 2023-04-27 06:22:16.259872 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/__pycache__/13a3b750c40e_add_pre_order_and_discount_columns_to_.cpython-38.pyc
+-rw-r--r--   0        0        0     1205 2023-05-16 07:38:44.370069 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/__pycache__/13a3b750c40e_add_pre_order_and_discount_columns_to_.cpython-39.pyc
+-rw-r--r--   0        0        0     1191 2023-04-27 09:21:16.792891 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/__pycache__/143be2620e05_rename_preorder_column_in_products_table.cpython-38.pyc
+-rw-r--r--   0        0        0     1191 2023-05-16 07:38:44.388020 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/__pycache__/143be2620e05_rename_preorder_column_in_products_table.cpython-39.pyc
+-rw-r--r--   0        0        0     1016 2022-11-25 16:07:54.940915 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/__pycache__/1f52b78d99b5_add_page_images_table.cpython-38.pyc
+-rw-r--r--   0        0        0     1016 2023-05-16 07:38:44.391013 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/__pycache__/1f52b78d99b5_add_page_images_table.cpython-39.pyc
+-rw-r--r--   0        0        0     1358 2023-04-27 06:21:38.131691 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/__pycache__/21550951e198_drop_discounts_table.cpython-38.pyc
+-rw-r--r--   0        0        0     1358 2023-05-16 07:38:44.393008 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/__pycache__/21550951e198_drop_discounts_table.cpython-39.pyc
+-rw-r--r--   0        0        0      992 2023-04-27 07:49:07.662286 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/__pycache__/26cdf6a5af2b_change_discount_type_to_integer_from_.cpython-38.pyc
+-rw-r--r--   0        0        0      992 2023-05-16 07:38:44.396000 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/__pycache__/26cdf6a5af2b_change_discount_type_to_integer_from_.cpython-39.pyc
+-rw-r--r--   0        0        0     1035 2022-11-14 11:36:28.445113 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/__pycache__/28e24bf5b755_create_user_table.cpython-38.pyc
+-rw-r--r--   0        0        0     1036 2023-05-16 07:38:44.397995 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/__pycache__/28e24bf5b755_create_user_table.cpython-39.pyc
+-rw-r--r--   0        0        0     1061 2022-11-17 17:39:09.649589 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/__pycache__/3afcf5045272_create_favorite_table.cpython-38.pyc
+-rw-r--r--   0        0        0     1061 2023-05-16 07:38:44.399989 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/__pycache__/3afcf5045272_create_favorite_table.cpython-39.pyc
+-rw-r--r--   0        0        0     1148 2022-11-17 17:32:22.727240 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/__pycache__/41640c6fbc41_create_product_table.cpython-38.pyc
+-rw-r--r--   0        0        0     1148 2023-05-16 07:38:44.402981 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/__pycache__/41640c6fbc41_create_product_table.cpython-39.pyc
+-rw-r--r--   0        0        0      924 2022-11-27 07:47:32.294695 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/__pycache__/432183be6e50_add_role_column_to_user_table.cpython-38.pyc
+-rw-r--r--   0        0        0      924 2023-05-16 07:38:44.404975 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/__pycache__/432183be6e50_add_role_column_to_user_table.cpython-39.pyc
+-rw-r--r--   0        0        0     1325 2023-04-27 07:36:48.516527 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/__pycache__/437ce57390c5_remove_active_discount_column_and_.cpython-38.pyc
+-rw-r--r--   0        0        0     1325 2023-05-16 07:38:44.406973 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/__pycache__/437ce57390c5_remove_active_discount_column_and_.cpython-39.pyc
+-rw-r--r--   0        0        0     1119 2022-11-25 13:12:14.766306 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/__pycache__/46fe20e7d2c8_add_reviews_table.cpython-38.pyc
+-rw-r--r--   0        0        0     1119 2023-05-16 07:38:44.408964 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/__pycache__/46fe20e7d2c8_add_reviews_table.cpython-39.pyc
+-rw-r--r--   0        0        0      914 2023-04-27 06:19:51.873397 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/__pycache__/4cfd3fc062af_add_date_column_to_review.cpython-38.pyc
+-rw-r--r--   0        0        0      914 2023-05-16 07:38:44.411957 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/__pycache__/4cfd3fc062af_add_date_column_to_review.cpython-39.pyc
+-rw-r--r--   0        0        0     1772 2022-11-17 17:20:22.941546 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/__pycache__/556ff2c83f9f_create_order_table.cpython-38.pyc
+-rw-r--r--   0        0        0     1772 2023-05-16 07:38:44.413951 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/__pycache__/556ff2c83f9f_create_order_table.cpython-39.pyc
+-rw-r--r--   0        0        0     1024 2022-11-17 17:19:16.196038 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/__pycache__/57c6c9633e32_create_shipping_method_table.cpython-38.pyc
+-rw-r--r--   0        0        0     1024 2023-05-16 07:38:44.415946 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/__pycache__/57c6c9633e32_create_shipping_method_table.cpython-39.pyc
+-rw-r--r--   0        0        0     1088 2022-11-17 17:41:41.614167 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/__pycache__/6787273bd08d_create_image_table.cpython-38.pyc
+-rw-r--r--   0        0        0     1088 2023-05-16 07:38:44.417940 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/__pycache__/6787273bd08d_create_image_table.cpython-39.pyc
+-rw-r--r--   0        0        0      993 2022-11-19 09:43:34.370910 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/__pycache__/68b8e7a46dc0_add_contact_columns_to_order_table.cpython-38.pyc
+-rw-r--r--   0        0        0      993 2023-05-16 07:38:44.419936 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/__pycache__/68b8e7a46dc0_add_contact_columns_to_order_table.cpython-39.pyc
+-rw-r--r--   0        0        0     1119 2022-11-17 09:29:10.463996 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/__pycache__/72c749f78b2c_add_registratrion_activation_and_update_.cpython-38.pyc
+-rw-r--r--   0        0        0     1119 2023-05-16 07:38:44.421930 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/__pycache__/72c749f78b2c_add_registratrion_activation_and_update_.cpython-39.pyc
+-rw-r--r--   0        0        0     1160 2022-11-17 17:37:07.585121 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/__pycache__/7561a3637af6_create_discount_table.cpython-38.pyc
+-rw-r--r--   0        0        0     1160 2023-05-16 07:38:44.424922 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/__pycache__/7561a3637af6_create_discount_table.cpython-39.pyc
+-rw-r--r--   0        0        0      965 2022-11-14 16:04:04.382267 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/__pycache__/76e56ad9a0d6_add_active_column_to_users_table.cpython-38.pyc
+-rw-r--r--   0        0        0      965 2023-05-16 07:38:44.426917 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/__pycache__/76e56ad9a0d6_add_active_column_to_users_table.cpython-39.pyc
+-rw-r--r--   0        0        0     1249 2022-11-17 15:39:46.868782 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/__pycache__/824f9117cea4_create_invoice_data_table.cpython-38.pyc
+-rw-r--r--   0        0        0     1249 2023-05-16 07:38:44.428912 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/__pycache__/824f9117cea4_create_invoice_data_table.cpython-39.pyc
+-rw-r--r--   0        0        0      965 2022-11-17 17:31:46.254540 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/__pycache__/88d8f0924ac3_create_category_table.cpython-38.pyc
+-rw-r--r--   0        0        0      965 2023-05-16 07:38:44.430906 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/__pycache__/88d8f0924ac3_create_category_table.cpython-39.pyc
+-rw-r--r--   0        0        0      994 2022-12-01 09:12:27.818550 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/__pycache__/8f89b8df2fba_enable_longer_name_for_product.cpython-38.pyc
+-rw-r--r--   0        0        0      994 2023-05-16 07:38:44.432901 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/__pycache__/8f89b8df2fba_enable_longer_name_for_product.cpython-39.pyc
+-rw-r--r--   0        0        0      909 2022-11-17 18:49:14.442466 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/__pycache__/905e714689ea_add_description_column_to_product_table.cpython-38.pyc
+-rw-r--r--   0        0        0      909 2023-05-16 07:38:44.434895 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/__pycache__/905e714689ea_add_description_column_to_product_table.cpython-39.pyc
+-rw-r--r--   0        0        0     1021 2022-11-17 17:19:57.038988 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/__pycache__/94537a354aba_create_payment_method_table.cpython-38.pyc
+-rw-r--r--   0        0        0     1021 2023-05-16 07:38:44.436890 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/__pycache__/94537a354aba_create_payment_method_table.cpython-39.pyc
+-rw-r--r--   0        0        0     1165 2022-11-17 14:11:09.291669 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/__pycache__/a2a05856eb15_create_address_table.cpython-38.pyc
+-rw-r--r--   0        0        0     1165 2023-05-16 07:38:44.448857 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/__pycache__/a2a05856eb15_create_address_table.cpython-39.pyc
+-rw-r--r--   0        0        0     1009 2022-11-19 09:34:42.463405 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/__pycache__/ade770eba952_add_description_columns_to_order_table.cpython-38.pyc
+-rw-r--r--   0        0        0     1009 2023-05-16 07:38:44.451851 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/__pycache__/ade770eba952_add_description_columns_to_order_table.cpython-39.pyc
+-rw-r--r--   0        0        0     1005 2022-11-25 14:27:47.383698 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/__pycache__/b2424975cff5_modify_review_description_to_nullable.cpython-38.pyc
+-rw-r--r--   0        0        0     1005 2023-05-16 07:38:44.453844 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/__pycache__/b2424975cff5_modify_review_description_to_nullable.cpython-39.pyc
+-rw-r--r--   0        0        0      927 2023-05-16 07:38:44.561557 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/__pycache__/b5f72dd98767_add_show_column_to_product_table.cpython-39.pyc
+-rw-r--r--   0        0        0      910 2022-11-17 15:39:46.837672 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/__pycache__/d190af5edcec_add_name_column_to_address_table.cpython-38.pyc
+-rw-r--r--   0        0        0      910 2023-05-16 07:38:44.455840 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/__pycache__/d190af5edcec_add_name_column_to_address_table.cpython-39.pyc
+-rw-r--r--   0        0        0     1023 2022-11-21 17:24:22.320177 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/__pycache__/dc6a7a4506e7_add_order_number_column_to_order_table.cpython-38.pyc
+-rw-r--r--   0        0        0     1023 2023-05-16 07:38:44.457834 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/__pycache__/dc6a7a4506e7_add_order_number_column_to_order_table.cpython-39.pyc
+-rw-r--r--   0        0        0      943 2023-04-27 06:35:08.362157 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/__pycache__/fd54dd612c6e_add_uploaded_column_to_products_table.cpython-38.pyc
+-rw-r--r--   0        0        0      943 2023-05-16 07:38:44.459829 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/__pycache__/fd54dd612c6e_add_uploaded_column_to_products_table.cpython-39.pyc
+-rw-r--r--   0        0        0     1103 2022-11-17 14:11:09.276179 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/a2a05856eb15_create_address_table.py
+-rw-r--r--   0        0        0      880 2022-11-19 09:34:42.463405 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/ade770eba952_add_description_columns_to_order_table.py
+-rw-r--r--   0        0        0      877 2022-11-25 14:27:47.383698 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/b2424975cff5_modify_review_description_to_nullable.py
+-rw-r--r--   0        0        0      720 2023-05-16 07:38:44.559562 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/b5f72dd98767_add_show_column_to_product_table.py
+-rw-r--r--   0        0        0      698 2022-11-17 15:39:42.615558 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/d190af5edcec_add_name_column_to_address_table.py
+-rw-r--r--   0        0        0      835 2022-11-21 17:24:22.320177 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/dc6a7a4506e7_add_order_number_column_to_order_table.py
+-rw-r--r--   0        0        0      735 2023-04-27 06:35:08.361160 decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/fd54dd612c6e_add_uploaded_column_to_products_table.py
+-rw-r--r--   0        0        0     3234 2022-11-14 11:34:58.943979 decorworld_database_model-0.6.6/decorworld_database_model/alembic.ini
+-rw-r--r--   0        0        0      449 2023-04-27 06:18:17.177337 decorworld_database_model-0.6.6/decorworld_database_model/tables/__init__.py
+-rw-r--r--   0        0        0      686 2023-04-27 06:18:58.311301 decorworld_database_model-0.6.6/decorworld_database_model/tables/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      759 2023-05-16 07:37:52.469259 decorworld_database_model-0.6.6/decorworld_database_model/tables/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1377 2022-11-17 15:38:13.840196 decorworld_database_model-0.6.6/decorworld_database_model/tables/__pycache__/address.cpython-38.pyc
+-rw-r--r--   0        0        0     1454 2023-05-16 07:38:08.350514 decorworld_database_model-0.6.6/decorworld_database_model/tables/__pycache__/address.cpython-39.pyc
+-rw-r--r--   0        0        0      244 2022-11-14 11:36:28.299749 decorworld_database_model-0.6.6/decorworld_database_model/tables/__pycache__/base.cpython-38.pyc
+-rw-r--r--   0        0        0      317 2023-05-16 07:37:52.471254 decorworld_database_model-0.6.6/decorworld_database_model/tables/__pycache__/base.cpython-39.pyc
+-rw-r--r--   0        0        0     1033 2023-04-27 06:19:51.542394 decorworld_database_model-0.6.6/decorworld_database_model/tables/__pycache__/category.cpython-38.pyc
+-rw-r--r--   0        0        0     1110 2023-05-16 07:38:44.299259 decorworld_database_model-0.6.6/decorworld_database_model/tables/__pycache__/category.cpython-39.pyc
+-rw-r--r--   0        0        0     1136 2023-04-27 06:19:51.546182 decorworld_database_model-0.6.6/decorworld_database_model/tables/__pycache__/favorite.cpython-38.pyc
+-rw-r--r--   0        0        0     1213 2023-05-16 07:38:44.303247 decorworld_database_model-0.6.6/decorworld_database_model/tables/__pycache__/favorite.cpython-39.pyc
+-rw-r--r--   0        0        0     1158 2023-04-27 06:18:59.499137 decorworld_database_model-0.6.6/decorworld_database_model/tables/__pycache__/image.cpython-38.pyc
+-rw-r--r--   0        0        0     1235 2023-05-16 07:38:08.376443 decorworld_database_model-0.6.6/decorworld_database_model/tables/__pycache__/image.cpython-39.pyc
+-rw-r--r--   0        0        0     1481 2023-04-27 06:18:59.328518 decorworld_database_model-0.6.6/decorworld_database_model/tables/__pycache__/invoice_data.cpython-38.pyc
+-rw-r--r--   0        0        0     1558 2023-05-16 07:38:08.355498 decorworld_database_model-0.6.6/decorworld_database_model/tables/__pycache__/invoice_data.cpython-39.pyc
+-rw-r--r--   0        0        0     3621 2023-04-27 06:18:59.439222 decorworld_database_model-0.6.6/decorworld_database_model/tables/__pycache__/order.cpython-38.pyc
+-rw-r--r--   0        0        0     3698 2023-05-16 07:38:08.369462 decorworld_database_model-0.6.6/decorworld_database_model/tables/__pycache__/order.cpython-39.pyc
+-rw-r--r--   0        0        0     1519 2022-11-27 10:50:10.032765 decorworld_database_model-0.6.6/decorworld_database_model/tables/__pycache__/order_item.cpython-38.pyc
+-rw-r--r--   0        0        0     1525 2023-05-16 07:38:08.371457 decorworld_database_model-0.6.6/decorworld_database_model/tables/__pycache__/order_item.cpython-39.pyc
+-rw-r--r--   0        0        0     1057 2022-11-25 16:07:54.847187 decorworld_database_model-0.6.6/decorworld_database_model/tables/__pycache__/page_image.cpython-38.pyc
+-rw-r--r--   0        0        0     1134 2023-05-16 07:38:44.310229 decorworld_database_model-0.6.6/decorworld_database_model/tables/__pycache__/page_image.cpython-39.pyc
+-rw-r--r--   0        0        0     1107 2023-04-27 06:18:59.377388 decorworld_database_model-0.6.6/decorworld_database_model/tables/__pycache__/payment_method.cpython-38.pyc
+-rw-r--r--   0        0        0     1184 2023-05-16 07:38:08.363478 decorworld_database_model-0.6.6/decorworld_database_model/tables/__pycache__/payment_method.cpython-39.pyc
+-rw-r--r--   0        0        0     1948 2023-04-27 09:20:23.883299 decorworld_database_model-0.6.6/decorworld_database_model/tables/__pycache__/product.cpython-38.pyc
+-rw-r--r--   0        0        0     2072 2023-05-16 07:38:33.498817 decorworld_database_model-0.6.6/decorworld_database_model/tables/__pycache__/product.cpython-39.pyc
+-rw-r--r--   0        0        0     1678 2023-03-29 09:32:45.408915 decorworld_database_model-0.6.6/decorworld_database_model/tables/__pycache__/review.cpython-38.pyc
+-rw-r--r--   0        0        0     1684 2023-05-16 07:38:44.306240 decorworld_database_model-0.6.6/decorworld_database_model/tables/__pycache__/review.cpython-39.pyc
+-rw-r--r--   0        0        0     1114 2023-04-27 06:18:59.371404 decorworld_database_model-0.6.6/decorworld_database_model/tables/__pycache__/shipping_method.cpython-38.pyc
+-rw-r--r--   0        0        0     1191 2023-05-16 07:38:08.359490 decorworld_database_model-0.6.6/decorworld_database_model/tables/__pycache__/shipping_method.cpython-39.pyc
+-rw-r--r--   0        0        0     1631 2022-11-27 07:47:32.044754 decorworld_database_model-0.6.6/decorworld_database_model/tables/__pycache__/user.cpython-38.pyc
+-rw-r--r--   0        0        0     1708 2023-05-16 07:37:52.642795 decorworld_database_model-0.6.6/decorworld_database_model/tables/__pycache__/user.cpython-39.pyc
+-rw-r--r--   0        0        0     1143 2022-11-17 15:24:28.613902 decorworld_database_model-0.6.6/decorworld_database_model/tables/address.py
+-rw-r--r--   0        0        0      160 2022-11-14 11:30:54.004559 decorworld_database_model-0.6.6/decorworld_database_model/tables/base.py
+-rw-r--r--   0        0        0      628 2023-04-27 06:17:17.160232 decorworld_database_model-0.6.6/decorworld_database_model/tables/category.py
+-rw-r--r--   0        0        0      790 2023-04-27 06:17:17.107376 decorworld_database_model-0.6.6/decorworld_database_model/tables/favorite.py
+-rw-r--r--   0        0        0      784 2023-04-27 06:17:17.113356 decorworld_database_model-0.6.6/decorworld_database_model/tables/image.py
+-rw-r--r--   0        0        0     1290 2023-04-27 06:17:17.082439 decorworld_database_model-0.6.6/decorworld_database_model/tables/invoice_data.py
+-rw-r--r--   0        0        0     4192 2023-04-27 06:17:17.094407 decorworld_database_model-0.6.6/decorworld_database_model/tables/order.py
+-rw-r--r--   0        0        0     1184 2022-11-27 10:47:07.768493 decorworld_database_model-0.6.6/decorworld_database_model/tables/order_item.py
+-rw-r--r--   0        0        0      647 2022-11-25 16:07:28.582459 decorworld_database_model-0.6.6/decorworld_database_model/tables/page_image.py
+-rw-r--r--   0        0        0      733 2023-04-27 06:17:17.101389 decorworld_database_model-0.6.6/decorworld_database_model/tables/payment_method.py
+-rw-r--r--   0        0        0     1974 2023-05-16 07:38:30.397182 decorworld_database_model-0.6.6/decorworld_database_model/tables/product.py
+-rw-r--r--   0        0        0     1328 2023-03-29 08:51:06.589872 decorworld_database_model-0.6.6/decorworld_database_model/tables/review.py
+-rw-r--r--   0        0        0      740 2023-04-27 06:17:17.167212 decorworld_database_model-0.6.6/decorworld_database_model/tables/shipping_method.py
+-rw-r--r--   0        0        0     1507 2022-11-27 07:46:49.104190 decorworld_database_model-0.6.6/decorworld_database_model/tables/user.py
+-rw-r--r--   0        0        0      405 2023-05-16 07:39:35.913695 decorworld_database_model-0.6.6/pyproject.toml
+-rw-r--r--   0        0        0      530 1970-01-01 00:00:00.000000 decorworld_database_model-0.6.6/PKG-INFO
```

### Comparing `decorworld_database_model-0.6.5/decorworld_database_model/alembic/env.py` & `decorworld_database_model-0.6.6/decorworld_database_model/alembic/env.py`

 * *Files identical despite different names*

### Comparing `decorworld_database_model-0.6.5/decorworld_database_model/alembic/versions/082d80622e74_create_order_item_table.py` & `decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/082d80622e74_create_order_item_table.py`

 * *Files identical despite different names*

### Comparing `decorworld_database_model-0.6.5/decorworld_database_model/alembic/versions/13a3b750c40e_add_pre_order_and_discount_columns_to_.py` & `decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/13a3b750c40e_add_pre_order_and_discount_columns_to_.py`

 * *Files identical despite different names*

### Comparing `decorworld_database_model-0.6.5/decorworld_database_model/alembic/versions/143be2620e05_rename_preorder_column_in_products_table.py` & `decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/143be2620e05_rename_preorder_column_in_products_table.py`

 * *Files identical despite different names*

### Comparing `decorworld_database_model-0.6.5/decorworld_database_model/alembic/versions/1f52b78d99b5_add_page_images_table.py` & `decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/1f52b78d99b5_add_page_images_table.py`

 * *Files identical despite different names*

### Comparing `decorworld_database_model-0.6.5/decorworld_database_model/alembic/versions/21550951e198_drop_discounts_table.py` & `decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/21550951e198_drop_discounts_table.py`

 * *Files identical despite different names*

### Comparing `decorworld_database_model-0.6.5/decorworld_database_model/alembic/versions/26cdf6a5af2b_change_discount_type_to_integer_from_.py` & `decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/26cdf6a5af2b_change_discount_type_to_integer_from_.py`

 * *Files identical despite different names*

### Comparing `decorworld_database_model-0.6.5/decorworld_database_model/alembic/versions/28e24bf5b755_create_user_table.py` & `decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/28e24bf5b755_create_user_table.py`

 * *Files identical despite different names*

### Comparing `decorworld_database_model-0.6.5/decorworld_database_model/alembic/versions/3afcf5045272_create_favorite_table.py` & `decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/3afcf5045272_create_favorite_table.py`

 * *Files identical despite different names*

### Comparing `decorworld_database_model-0.6.5/decorworld_database_model/alembic/versions/41640c6fbc41_create_product_table.py` & `decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/41640c6fbc41_create_product_table.py`

 * *Files identical despite different names*

### Comparing `decorworld_database_model-0.6.5/decorworld_database_model/alembic/versions/432183be6e50_add_role_column_to_user_table.py` & `decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/432183be6e50_add_role_column_to_user_table.py`

 * *Files identical despite different names*

### Comparing `decorworld_database_model-0.6.5/decorworld_database_model/alembic/versions/437ce57390c5_remove_active_discount_column_and_.py` & `decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/437ce57390c5_remove_active_discount_column_and_.py`

 * *Files identical despite different names*

### Comparing `decorworld_database_model-0.6.5/decorworld_database_model/alembic/versions/46fe20e7d2c8_add_reviews_table.py` & `decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/46fe20e7d2c8_add_reviews_table.py`

 * *Files identical despite different names*

### Comparing `decorworld_database_model-0.6.5/decorworld_database_model/alembic/versions/4cfd3fc062af_add_date_column_to_review.py` & `decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/4cfd3fc062af_add_date_column_to_review.py`

 * *Files identical despite different names*

### Comparing `decorworld_database_model-0.6.5/decorworld_database_model/alembic/versions/556ff2c83f9f_create_order_table.py` & `decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/556ff2c83f9f_create_order_table.py`

 * *Files identical despite different names*

### Comparing `decorworld_database_model-0.6.5/decorworld_database_model/alembic/versions/57c6c9633e32_create_shipping_method_table.py` & `decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/57c6c9633e32_create_shipping_method_table.py`

 * *Files identical despite different names*

### Comparing `decorworld_database_model-0.6.5/decorworld_database_model/alembic/versions/6787273bd08d_create_image_table.py` & `decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/6787273bd08d_create_image_table.py`

 * *Files identical despite different names*

### Comparing `decorworld_database_model-0.6.5/decorworld_database_model/alembic/versions/68b8e7a46dc0_add_contact_columns_to_order_table.py` & `decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/68b8e7a46dc0_add_contact_columns_to_order_table.py`

 * *Files identical despite different names*

### Comparing `decorworld_database_model-0.6.5/decorworld_database_model/alembic/versions/72c749f78b2c_add_registratrion_activation_and_update_.py` & `decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/72c749f78b2c_add_registratrion_activation_and_update_.py`

 * *Files identical despite different names*

### Comparing `decorworld_database_model-0.6.5/decorworld_database_model/alembic/versions/7561a3637af6_create_discount_table.py` & `decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/7561a3637af6_create_discount_table.py`

 * *Files identical despite different names*

### Comparing `decorworld_database_model-0.6.5/decorworld_database_model/alembic/versions/76e56ad9a0d6_add_active_column_to_users_table.py` & `decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/76e56ad9a0d6_add_active_column_to_users_table.py`

 * *Files identical despite different names*

### Comparing `decorworld_database_model-0.6.5/decorworld_database_model/alembic/versions/824f9117cea4_create_invoice_data_table.py` & `decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/824f9117cea4_create_invoice_data_table.py`

 * *Files identical despite different names*

### Comparing `decorworld_database_model-0.6.5/decorworld_database_model/alembic/versions/88d8f0924ac3_create_category_table.py` & `decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/88d8f0924ac3_create_category_table.py`

 * *Files identical despite different names*

### Comparing `decorworld_database_model-0.6.5/decorworld_database_model/alembic/versions/8f89b8df2fba_enable_longer_name_for_product.py` & `decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/8f89b8df2fba_enable_longer_name_for_product.py`

 * *Files identical despite different names*

### Comparing `decorworld_database_model-0.6.5/decorworld_database_model/alembic/versions/905e714689ea_add_description_column_to_product_table.py` & `decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/905e714689ea_add_description_column_to_product_table.py`

 * *Files identical despite different names*

### Comparing `decorworld_database_model-0.6.5/decorworld_database_model/alembic/versions/94537a354aba_create_payment_method_table.py` & `decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/94537a354aba_create_payment_method_table.py`

 * *Files identical despite different names*

### Comparing `decorworld_database_model-0.6.5/decorworld_database_model/alembic/versions/a2a05856eb15_create_address_table.py` & `decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/a2a05856eb15_create_address_table.py`

 * *Files identical despite different names*

### Comparing `decorworld_database_model-0.6.5/decorworld_database_model/alembic/versions/ade770eba952_add_description_columns_to_order_table.py` & `decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/ade770eba952_add_description_columns_to_order_table.py`

 * *Files identical despite different names*

### Comparing `decorworld_database_model-0.6.5/decorworld_database_model/alembic/versions/b2424975cff5_modify_review_description_to_nullable.py` & `decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/b2424975cff5_modify_review_description_to_nullable.py`

 * *Files identical despite different names*

### Comparing `decorworld_database_model-0.6.5/decorworld_database_model/alembic/versions/d190af5edcec_add_name_column_to_address_table.py` & `decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/d190af5edcec_add_name_column_to_address_table.py`

 * *Files identical despite different names*

### Comparing `decorworld_database_model-0.6.5/decorworld_database_model/alembic/versions/dc6a7a4506e7_add_order_number_column_to_order_table.py` & `decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/dc6a7a4506e7_add_order_number_column_to_order_table.py`

 * *Files identical despite different names*

### Comparing `decorworld_database_model-0.6.5/decorworld_database_model/alembic/versions/fd54dd612c6e_add_uploaded_column_to_products_table.py` & `decorworld_database_model-0.6.6/decorworld_database_model/alembic/versions/fd54dd612c6e_add_uploaded_column_to_products_table.py`

 * *Files identical despite different names*

### Comparing `decorworld_database_model-0.6.5/decorworld_database_model/alembic.ini` & `decorworld_database_model-0.6.6/decorworld_database_model/alembic.ini`

 * *Files identical despite different names*

### Comparing `decorworld_database_model-0.6.5/decorworld_database_model/tables/address.py` & `decorworld_database_model-0.6.6/decorworld_database_model/tables/address.py`

 * *Files identical despite different names*

### Comparing `decorworld_database_model-0.6.5/decorworld_database_model/tables/category.py` & `decorworld_database_model-0.6.6/decorworld_database_model/tables/category.py`

 * *Files identical despite different names*

### Comparing `decorworld_database_model-0.6.5/decorworld_database_model/tables/favorite.py` & `decorworld_database_model-0.6.6/decorworld_database_model/tables/favorite.py`

 * *Files identical despite different names*

### Comparing `decorworld_database_model-0.6.5/decorworld_database_model/tables/image.py` & `decorworld_database_model-0.6.6/decorworld_database_model/tables/image.py`

 * *Files identical despite different names*

### Comparing `decorworld_database_model-0.6.5/decorworld_database_model/tables/invoice_data.py` & `decorworld_database_model-0.6.6/decorworld_database_model/tables/invoice_data.py`

 * *Files identical despite different names*

### Comparing `decorworld_database_model-0.6.5/decorworld_database_model/tables/order.py` & `decorworld_database_model-0.6.6/decorworld_database_model/tables/order.py`

 * *Files identical despite different names*

### Comparing `decorworld_database_model-0.6.5/decorworld_database_model/tables/order_item.py` & `decorworld_database_model-0.6.6/decorworld_database_model/tables/order_item.py`

 * *Files identical despite different names*

### Comparing `decorworld_database_model-0.6.5/decorworld_database_model/tables/page_image.py` & `decorworld_database_model-0.6.6/decorworld_database_model/tables/page_image.py`

 * *Files identical despite different names*

### Comparing `decorworld_database_model-0.6.5/decorworld_database_model/tables/payment_method.py` & `decorworld_database_model-0.6.6/decorworld_database_model/tables/payment_method.py`

 * *Files identical despite different names*

### Comparing `decorworld_database_model-0.6.5/decorworld_database_model/tables/product.py` & `decorworld_database_model-0.6.6/decorworld_database_model/tables/product.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     number = Column(String(25), nullable=False)
     price = Column(Integer, nullable=False)
     quantity = Column(Integer, nullable=False)
     description = Column(Text, nullable=False)
     available_for_preorder = Column(Boolean, nullable=False, server_default=text('false'))
     discount = Column(Integer, nullable=False, server_default=text('0'))
     uploaded = Column(DateTime, nullable=False, server_default=func.now())
+    show = Column(Boolean, nullable=False, server_default=text("true"))
 
     image = relationship('Image', foreign_keys='Image.product_id')
 
 
 class ProductSchema(Schema):
 
     model_class = Product
@@ -44,13 +45,14 @@
     number = fields.String()
     price = fields.Integer()
     quantity = fields.Integer()
     description = fields.String()
     available_for_preorder = fields.Boolean(data_key='availableForPreorder')
     discount = fields.Integer()
     uploaded = fields.DateTime()
+    show = fields.Boolean()
 
     image = fields.Nested(ImageSchema)
 
     @post_load
     def make_product(self, data, **kwargs):
         return Product(**data)
```

### Comparing `decorworld_database_model-0.6.5/decorworld_database_model/tables/review.py` & `decorworld_database_model-0.6.6/decorworld_database_model/tables/review.py`

 * *Files identical despite different names*

### Comparing `decorworld_database_model-0.6.5/decorworld_database_model/tables/shipping_method.py` & `decorworld_database_model-0.6.6/decorworld_database_model/tables/shipping_method.py`

 * *Files identical despite different names*

### Comparing `decorworld_database_model-0.6.5/decorworld_database_model/tables/user.py` & `decorworld_database_model-0.6.6/decorworld_database_model/tables/user.py`

 * *Files identical despite different names*

