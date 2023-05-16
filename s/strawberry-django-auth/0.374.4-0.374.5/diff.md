# Comparing `tmp/strawberry_django_auth-0.374.4.tar.gz` & `tmp/strawberry_django_auth-0.374.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strawberry_django_auth-0.374.4.tar", max compression
+gzip compressed data, was "strawberry_django_auth-0.374.5.tar", max compression
```

## Comparing `strawberry_django_auth-0.374.4.tar` & `strawberry_django_auth-0.374.5.tar`

### file list

```diff
@@ -1,53 +1,56 @@
--rw-r--r--   0        0        0     1075 2023-05-07 16:27:39.317448 strawberry_django_auth-0.374.4/LICENSE
--rw-r--r--   0        0        0     3820 2023-05-07 16:27:39.317448 strawberry_django_auth-0.374.4/README.md
--rw-r--r--   0        0        0       24 2023-05-07 16:27:39.369448 strawberry_django_auth-0.374.4/gqlauth/__init__.py
--rw-r--r--   0        0        0      168 2023-05-07 16:27:39.369448 strawberry_django_auth-0.374.4/gqlauth/admin.py
--rw-r--r--   0        0        0      215 2023-05-07 16:27:39.369448 strawberry_django_auth-0.374.4/gqlauth/apps.py
--rw-r--r--   0        0        0        0 2023-05-07 16:27:39.369448 strawberry_django_auth-0.374.4/gqlauth/captcha/__init__.py
--rw-r--r--   0        0        0     1267 2023-05-07 16:27:39.369448 strawberry_django_auth-0.374.4/gqlauth/captcha/captcha_factorty.py
--rw-r--r--   0        0        0     6602 2023-05-07 16:27:39.369448 strawberry_django_auth-0.374.4/gqlauth/captcha/create.py
--rw-r--r--   0        0        0    16724 2023-05-07 16:27:39.369448 strawberry_django_auth-0.374.4/gqlauth/captcha/fonts/Nehama.ttf
--rw-r--r--   0        0        0   221328 2023-05-07 16:27:39.373448 strawberry_django_auth-0.374.4/gqlauth/captcha/fonts/OpenSans-Semibold.ttf
--rw-r--r--   0        0        0    45448 2023-05-07 16:27:39.373448 strawberry_django_auth-0.374.4/gqlauth/captcha/fonts/pltwide.ttf
--rwxr-xr-x   0        0        0    22768 2023-05-07 16:27:39.373448 strawberry_django_auth-0.374.4/gqlauth/captcha/fonts/stam.ttf
--rw-r--r--   0        0        0     3248 2023-05-07 16:27:39.373448 strawberry_django_auth-0.374.4/gqlauth/captcha/models.py
--rw-r--r--   0        0        0      448 2023-05-07 16:27:39.373448 strawberry_django_auth-0.374.4/gqlauth/captcha/types_.py
--rw-r--r--   0        0        0        0 2023-05-07 16:27:39.373448 strawberry_django_auth-0.374.4/gqlauth/core/__init__.py
--rw-r--r--   0        0        0     1995 2023-05-07 16:27:39.373448 strawberry_django_auth-0.374.4/gqlauth/core/constants.py
--rw-r--r--   0        0        0      724 2023-05-07 16:27:39.373448 strawberry_django_auth-0.374.4/gqlauth/core/directives.py
--rw-r--r--   0        0        0     1093 2023-05-07 16:27:39.373448 strawberry_django_auth-0.374.4/gqlauth/core/exceptions.py
--rw-r--r--   0        0        0      231 2023-05-07 16:27:39.373448 strawberry_django_auth-0.374.4/gqlauth/core/interfaces.py
--rw-r--r--   0        0        0     4559 2023-05-07 16:27:39.373448 strawberry_django_auth-0.374.4/gqlauth/core/middlewares.py
--rw-r--r--   0        0        0     1453 2023-05-07 16:27:39.373448 strawberry_django_auth-0.374.4/gqlauth/core/mixins.py
--rw-r--r--   0        0        0     1516 2023-05-07 16:27:39.373448 strawberry_django_auth-0.374.4/gqlauth/core/scalars.py
--rw-r--r--   0        0        0      857 2023-05-07 16:27:39.373448 strawberry_django_auth-0.374.4/gqlauth/core/types_.py
--rw-r--r--   0        0        0     3979 2023-05-07 16:27:39.373448 strawberry_django_auth-0.374.4/gqlauth/core/utils.py
--rw-r--r--   0        0        0        0 2023-05-07 16:27:39.373448 strawberry_django_auth-0.374.4/gqlauth/jwt/__init__.py
--rw-r--r--   0        0        0        0 2023-05-07 16:27:39.373448 strawberry_django_auth-0.374.4/gqlauth/jwt/tools.py
--rw-r--r--   0        0        0     7498 2023-05-07 16:27:39.373448 strawberry_django_auth-0.374.4/gqlauth/jwt/types_.py
--rw-r--r--   0        0        0     2969 2023-05-07 16:27:39.373448 strawberry_django_auth-0.374.4/gqlauth/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-05-07 16:27:39.373448 strawberry_django_auth-0.374.4/gqlauth/migrations/__init__.py
--rw-r--r--   0        0        0     7322 2023-05-07 16:27:39.373448 strawberry_django_auth-0.374.4/gqlauth/models.py
--rw-r--r--   0        0        0        0 2023-05-07 16:27:39.373448 strawberry_django_auth-0.374.4/gqlauth/py.typed
--rw-r--r--   0        0        0      649 2023-05-07 16:27:39.373448 strawberry_django_auth-0.374.4/gqlauth/settings.py
--rw-r--r--   0        0        0     9830 2023-05-07 16:27:39.373448 strawberry_django_auth-0.374.4/gqlauth/settings_type.py
--rw-r--r--   0        0        0      171 2023-05-07 16:27:39.373448 strawberry_django_auth-0.374.4/gqlauth/templates/email/activation_email.html
--rw-r--r--   0        0        0       41 2023-05-07 16:27:39.373448 strawberry_django_auth-0.374.4/gqlauth/templates/email/activation_subject.txt
--rw-r--r--   0        0        0   176202 2023-05-07 16:27:39.373448 strawberry_django_auth-0.374.4/gqlauth/templates/email/images/gd4f267f778b22183ca1ded4dfae871eac04faaac23286dc27d9c228034ff735042cebd167fb684c47ea3bef8803094f5683f08a3728911b4b191f82a7c12de99_1280.jpg
--rw-r--r--   0        0        0   100933 2023-05-07 16:27:39.377448 strawberry_django_auth-0.374.4/gqlauth/templates/email/images/windrader-wind-power-fichtelberg-wind-park.jpg
--rw-r--r--   0        0        0      162 2023-05-07 16:27:39.377448 strawberry_django_auth-0.374.4/gqlauth/templates/email/password_reset_email.html
--rw-r--r--   0        0        0       39 2023-05-07 16:27:39.377448 strawberry_django_auth-0.374.4/gqlauth/templates/email/password_reset_subject.txt
--rw-r--r--   0        0        0      160 2023-05-07 16:27:39.377448 strawberry_django_auth-0.374.4/gqlauth/templates/email/password_set_email.html
--rw-r--r--   0        0        0       37 2023-05-07 16:27:39.377448 strawberry_django_auth-0.374.4/gqlauth/templates/email/password_set_subject.txt
--rw-r--r--   0        0        0        0 2023-05-07 16:27:39.377448 strawberry_django_auth-0.374.4/gqlauth/user/__init__.py
--rw-r--r--   0        0        0     2177 2023-05-07 16:27:39.377448 strawberry_django_auth-0.374.4/gqlauth/user/arg_mutations.py
--rw-r--r--   0        0        0     1628 2023-05-07 16:27:39.377448 strawberry_django_auth-0.374.4/gqlauth/user/forms.py
--rw-r--r--   0        0        0     1281 2023-05-07 16:27:39.377448 strawberry_django_auth-0.374.4/gqlauth/user/helpers.py
--rw-r--r--   0        0        0     1104 2023-05-07 16:27:39.377448 strawberry_django_auth-0.374.4/gqlauth/user/queries.py
--rw-r--r--   0        0        0     2277 2023-05-07 16:27:39.377448 strawberry_django_auth-0.374.4/gqlauth/user/relay.py
--rw-r--r--   0        0        0    19509 2023-05-07 16:27:39.377448 strawberry_django_auth-0.374.4/gqlauth/user/resolvers.py
--rw-r--r--   0        0        0      450 2023-05-07 16:27:39.377448 strawberry_django_auth-0.374.4/gqlauth/user/signals.py
--rw-r--r--   0        0        0     2005 2023-05-07 16:27:39.377448 strawberry_django_auth-0.374.4/gqlauth/user/types_.py
--rw-r--r--   0        0        0      119 2023-05-07 16:27:39.377448 strawberry_django_auth-0.374.4/gqlauth/user/views.py
--rw-r--r--   0        0        0     3243 2023-05-07 16:27:57.249386 strawberry_django_auth-0.374.4/pyproject.toml
--rw-r--r--   0        0        0     5340 1970-01-01 00:00:00.000000 strawberry_django_auth-0.374.4/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-05-16 17:54:40.574432 strawberry_django_auth-0.374.5/LICENSE
+-rw-r--r--   0        0        0     3820 2023-05-16 17:54:40.574432 strawberry_django_auth-0.374.5/README.md
+-rw-r--r--   0        0        0       24 2023-05-16 17:54:40.630432 strawberry_django_auth-0.374.5/gqlauth/__init__.py
+-rw-r--r--   0        0        0      168 2023-05-16 17:54:40.630432 strawberry_django_auth-0.374.5/gqlauth/admin.py
+-rw-r--r--   0        0        0      215 2023-05-16 17:54:40.630432 strawberry_django_auth-0.374.5/gqlauth/apps.py
+-rw-r--r--   0        0        0        0 2023-05-16 17:54:40.630432 strawberry_django_auth-0.374.5/gqlauth/captcha/__init__.py
+-rw-r--r--   0        0        0     1267 2023-05-16 17:54:40.630432 strawberry_django_auth-0.374.5/gqlauth/captcha/captcha_factorty.py
+-rw-r--r--   0        0        0     6602 2023-05-16 17:54:40.630432 strawberry_django_auth-0.374.5/gqlauth/captcha/create.py
+-rw-r--r--   0        0        0    16724 2023-05-16 17:54:40.630432 strawberry_django_auth-0.374.5/gqlauth/captcha/fonts/Nehama.ttf
+-rw-r--r--   0        0        0   221328 2023-05-16 17:54:40.630432 strawberry_django_auth-0.374.5/gqlauth/captcha/fonts/OpenSans-Semibold.ttf
+-rw-r--r--   0        0        0    45448 2023-05-16 17:54:40.630432 strawberry_django_auth-0.374.5/gqlauth/captcha/fonts/pltwide.ttf
+-rwxr-xr-x   0        0        0    22768 2023-05-16 17:54:40.630432 strawberry_django_auth-0.374.5/gqlauth/captcha/fonts/stam.ttf
+-rw-r--r--   0        0        0     3248 2023-05-16 17:54:40.630432 strawberry_django_auth-0.374.5/gqlauth/captcha/models.py
+-rw-r--r--   0        0        0      448 2023-05-16 17:54:40.630432 strawberry_django_auth-0.374.5/gqlauth/captcha/types_.py
+-rw-r--r--   0        0        0        0 2023-05-16 17:54:40.630432 strawberry_django_auth-0.374.5/gqlauth/core/__init__.py
+-rw-r--r--   0        0        0     1995 2023-05-16 17:54:40.630432 strawberry_django_auth-0.374.5/gqlauth/core/constants.py
+-rw-r--r--   0        0        0      724 2023-05-16 17:54:40.630432 strawberry_django_auth-0.374.5/gqlauth/core/directives.py
+-rw-r--r--   0        0        0     1093 2023-05-16 17:54:40.630432 strawberry_django_auth-0.374.5/gqlauth/core/exceptions.py
+-rw-r--r--   0        0        0      231 2023-05-16 17:54:40.630432 strawberry_django_auth-0.374.5/gqlauth/core/interfaces.py
+-rw-r--r--   0        0        0     4559 2023-05-16 17:54:40.630432 strawberry_django_auth-0.374.5/gqlauth/core/middlewares.py
+-rw-r--r--   0        0        0     1453 2023-05-16 17:54:40.630432 strawberry_django_auth-0.374.5/gqlauth/core/mixins.py
+-rw-r--r--   0        0        0     1516 2023-05-16 17:54:40.630432 strawberry_django_auth-0.374.5/gqlauth/core/scalars.py
+-rw-r--r--   0        0        0      857 2023-05-16 17:54:40.630432 strawberry_django_auth-0.374.5/gqlauth/core/types_.py
+-rw-r--r--   0        0        0     3979 2023-05-16 17:54:40.630432 strawberry_django_auth-0.374.5/gqlauth/core/utils.py
+-rw-r--r--   0        0        0        0 2023-05-16 17:54:40.630432 strawberry_django_auth-0.374.5/gqlauth/jwt/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-16 17:54:40.630432 strawberry_django_auth-0.374.5/gqlauth/jwt/tools.py
+-rw-r--r--   0        0        0     7498 2023-05-16 17:54:40.630432 strawberry_django_auth-0.374.5/gqlauth/jwt/types_.py
+-rw-r--r--   0        0        0     2969 2023-05-16 17:54:40.634433 strawberry_django_auth-0.374.5/gqlauth/migrations/0001_initial.py
+-rw-r--r--   0        0        0      355 2023-05-16 17:54:40.634433 strawberry_django_auth-0.374.5/gqlauth/migrations/0002_alter_userstatus_options.py
+-rw-r--r--   0        0        0      301 2023-05-16 17:54:40.634433 strawberry_django_auth-0.374.5/gqlauth/migrations/0003_delete_captcha.py
+-rw-r--r--   0        0        0     1062 2023-05-16 17:54:40.634433 strawberry_django_auth-0.374.5/gqlauth/migrations/0004_captcha.py
+-rw-r--r--   0        0        0        0 2023-05-16 17:54:40.634433 strawberry_django_auth-0.374.5/gqlauth/migrations/__init__.py
+-rw-r--r--   0        0        0     7322 2023-05-16 17:54:40.634433 strawberry_django_auth-0.374.5/gqlauth/models.py
+-rw-r--r--   0        0        0        0 2023-05-16 17:54:40.634433 strawberry_django_auth-0.374.5/gqlauth/py.typed
+-rw-r--r--   0        0        0      649 2023-05-16 17:54:40.634433 strawberry_django_auth-0.374.5/gqlauth/settings.py
+-rw-r--r--   0        0        0     9830 2023-05-16 17:54:40.634433 strawberry_django_auth-0.374.5/gqlauth/settings_type.py
+-rw-r--r--   0        0        0      171 2023-05-16 17:54:40.634433 strawberry_django_auth-0.374.5/gqlauth/templates/email/activation_email.html
+-rw-r--r--   0        0        0       41 2023-05-16 17:54:40.634433 strawberry_django_auth-0.374.5/gqlauth/templates/email/activation_subject.txt
+-rw-r--r--   0        0        0   176202 2023-05-16 17:54:40.634433 strawberry_django_auth-0.374.5/gqlauth/templates/email/images/gd4f267f778b22183ca1ded4dfae871eac04faaac23286dc27d9c228034ff735042cebd167fb684c47ea3bef8803094f5683f08a3728911b4b191f82a7c12de99_1280.jpg
+-rw-r--r--   0        0        0   100933 2023-05-16 17:54:40.634433 strawberry_django_auth-0.374.5/gqlauth/templates/email/images/windrader-wind-power-fichtelberg-wind-park.jpg
+-rw-r--r--   0        0        0      162 2023-05-16 17:54:40.634433 strawberry_django_auth-0.374.5/gqlauth/templates/email/password_reset_email.html
+-rw-r--r--   0        0        0       39 2023-05-16 17:54:40.634433 strawberry_django_auth-0.374.5/gqlauth/templates/email/password_reset_subject.txt
+-rw-r--r--   0        0        0      160 2023-05-16 17:54:40.634433 strawberry_django_auth-0.374.5/gqlauth/templates/email/password_set_email.html
+-rw-r--r--   0        0        0       37 2023-05-16 17:54:40.634433 strawberry_django_auth-0.374.5/gqlauth/templates/email/password_set_subject.txt
+-rw-r--r--   0        0        0        0 2023-05-16 17:54:40.634433 strawberry_django_auth-0.374.5/gqlauth/user/__init__.py
+-rw-r--r--   0        0        0     2177 2023-05-16 17:54:40.634433 strawberry_django_auth-0.374.5/gqlauth/user/arg_mutations.py
+-rw-r--r--   0        0        0     1628 2023-05-16 17:54:40.634433 strawberry_django_auth-0.374.5/gqlauth/user/forms.py
+-rw-r--r--   0        0        0     1281 2023-05-16 17:54:40.634433 strawberry_django_auth-0.374.5/gqlauth/user/helpers.py
+-rw-r--r--   0        0        0     1104 2023-05-16 17:54:40.634433 strawberry_django_auth-0.374.5/gqlauth/user/queries.py
+-rw-r--r--   0        0        0     2277 2023-05-16 17:54:40.634433 strawberry_django_auth-0.374.5/gqlauth/user/relay.py
+-rw-r--r--   0        0        0    19509 2023-05-16 17:54:40.634433 strawberry_django_auth-0.374.5/gqlauth/user/resolvers.py
+-rw-r--r--   0        0        0      450 2023-05-16 17:54:40.634433 strawberry_django_auth-0.374.5/gqlauth/user/signals.py
+-rw-r--r--   0        0        0     2005 2023-05-16 17:54:40.634433 strawberry_django_auth-0.374.5/gqlauth/user/types_.py
+-rw-r--r--   0        0        0      119 2023-05-16 17:54:40.634433 strawberry_django_auth-0.374.5/gqlauth/user/views.py
+-rw-r--r--   0        0        0     3209 2023-05-16 17:55:01.775578 strawberry_django_auth-0.374.5/pyproject.toml
+-rw-r--r--   0        0        0     5340 1970-01-01 00:00:00.000000 strawberry_django_auth-0.374.5/PKG-INFO
```

### Comparing `strawberry_django_auth-0.374.4/LICENSE` & `strawberry_django_auth-0.374.5/LICENSE`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.374.4/README.md` & `strawberry_django_auth-0.374.5/README.md`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.374.4/gqlauth/captcha/captcha_factorty.py` & `strawberry_django_auth-0.374.5/gqlauth/captcha/captcha_factorty.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.374.4/gqlauth/captcha/create.py` & `strawberry_django_auth-0.374.5/gqlauth/captcha/create.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.374.4/gqlauth/captcha/fonts/Nehama.ttf` & `strawberry_django_auth-0.374.5/gqlauth/captcha/fonts/Nehama.ttf`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.374.4/gqlauth/captcha/fonts/OpenSans-Semibold.ttf` & `strawberry_django_auth-0.374.5/gqlauth/captcha/fonts/OpenSans-Semibold.ttf`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.374.4/gqlauth/captcha/fonts/pltwide.ttf` & `strawberry_django_auth-0.374.5/gqlauth/captcha/fonts/pltwide.ttf`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.374.4/gqlauth/captcha/fonts/stam.ttf` & `strawberry_django_auth-0.374.5/gqlauth/captcha/fonts/stam.ttf`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.374.4/gqlauth/captcha/models.py` & `strawberry_django_auth-0.374.5/gqlauth/captcha/models.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.374.4/gqlauth/core/constants.py` & `strawberry_django_auth-0.374.5/gqlauth/core/constants.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.374.4/gqlauth/core/directives.py` & `strawberry_django_auth-0.374.5/gqlauth/core/directives.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.374.4/gqlauth/core/exceptions.py` & `strawberry_django_auth-0.374.5/gqlauth/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.374.4/gqlauth/core/middlewares.py` & `strawberry_django_auth-0.374.5/gqlauth/core/middlewares.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.374.4/gqlauth/core/mixins.py` & `strawberry_django_auth-0.374.5/gqlauth/core/mixins.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.374.4/gqlauth/core/scalars.py` & `strawberry_django_auth-0.374.5/gqlauth/core/scalars.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.374.4/gqlauth/core/types_.py` & `strawberry_django_auth-0.374.5/gqlauth/core/types_.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.374.4/gqlauth/core/utils.py` & `strawberry_django_auth-0.374.5/gqlauth/core/utils.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.374.4/gqlauth/jwt/types_.py` & `strawberry_django_auth-0.374.5/gqlauth/jwt/types_.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.374.4/gqlauth/migrations/0001_initial.py` & `strawberry_django_auth-0.374.5/gqlauth/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.374.4/gqlauth/models.py` & `strawberry_django_auth-0.374.5/gqlauth/models.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.374.4/gqlauth/settings.py` & `strawberry_django_auth-0.374.5/gqlauth/settings.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.374.4/gqlauth/settings_type.py` & `strawberry_django_auth-0.374.5/gqlauth/settings_type.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.374.4/gqlauth/templates/email/images/gd4f267f778b22183ca1ded4dfae871eac04faaac23286dc27d9c228034ff735042cebd167fb684c47ea3bef8803094f5683f08a3728911b4b191f82a7c12de99_1280.jpg` & `strawberry_django_auth-0.374.5/gqlauth/templates/email/images/gd4f267f778b22183ca1ded4dfae871eac04faaac23286dc27d9c228034ff735042cebd167fb684c47ea3bef8803094f5683f08a3728911b4b191f82a7c12de99_1280.jpg`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.374.4/gqlauth/templates/email/images/windrader-wind-power-fichtelberg-wind-park.jpg` & `strawberry_django_auth-0.374.5/gqlauth/templates/email/images/windrader-wind-power-fichtelberg-wind-park.jpg`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.374.4/gqlauth/user/arg_mutations.py` & `strawberry_django_auth-0.374.5/gqlauth/user/arg_mutations.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.374.4/gqlauth/user/forms.py` & `strawberry_django_auth-0.374.5/gqlauth/user/forms.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.374.4/gqlauth/user/helpers.py` & `strawberry_django_auth-0.374.5/gqlauth/user/helpers.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.374.4/gqlauth/user/queries.py` & `strawberry_django_auth-0.374.5/gqlauth/user/queries.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.374.4/gqlauth/user/relay.py` & `strawberry_django_auth-0.374.5/gqlauth/user/relay.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.374.4/gqlauth/user/resolvers.py` & `strawberry_django_auth-0.374.5/gqlauth/user/resolvers.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.374.4/gqlauth/user/types_.py` & `strawberry_django_auth-0.374.5/gqlauth/user/types_.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.374.4/pyproject.toml` & `strawberry_django_auth-0.374.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "strawberry-django-auth"
-version = "0.374.4"
+version = "0.374.5"
 description = "Graphql authentication system with Strawberry for Django."
 license = "MIT"
 authors = ["Nir.J Benlulu <nrbnlulu@gmail.com>"]
 maintainers = ["Nir.J Benlulu <nrbnlulu@gmail.com>"]
 readme = "README.md"
 classifiers = [
     'Environment :: Web Environment',
@@ -40,26 +40,25 @@
 pytest-cov = "^4.0"
 pytest-django = "^4.0.0"
 types-cryptography = "^3.3.23"
 django-mock-queries = "^2.1.7"
 types-mock = "^5.0.0"
 types-jwt = "^0.1.0"
 types-pkg-resources = "^0.1.0"
-mkdocs = "^1.3.0"
-mkdocs-markdownextradata-plugin = "^0.2.5"
-mkdocs-material = "^8.5.4"
-mkdocs-minify-plugin = "^0.5.0"
-pymdown-extensions = "^9.9"
-Markdown = "^3.4.1"
-Faker = "^18.2.0"
-pytest-asyncio = "^0.21.0"
-pydoc-markdown = {extras = ["novella"], version = "^4.6.4"}
-gql = {extras = ["all"], version = "^3.4.0"}
-setuptools = "^67.6.0"
-channels = {extras = ["daphne"], version = "^4.0.0"}
+mkdocs = ">=1.3.0"
+mkdocs-markdownextradata-plugin = ">=0.2.5"
+mkdocs-material = ">=8.5.4"
+mkdocs-minify-plugin = ">=0.5.0"
+pymdown-extensions = ">=9.9"
+Markdown = ">=3.4.1"
+Faker = ">=18.2.0"
+pytest-asyncio = ">=0.21.0"
+pydoc-markdown = {extras = ["novella"], version = ">=4.6.4"}
+setuptools = ">=67.6.0"
+channels = {extras = ["daphne"], version = ">=4.0.0"}
 
 
 [tool.pytest.ini_options]
 django_find_project = false
 minversion = "6.0"
 addopts = "-ra -q"
 testpaths = [
```

### Comparing `strawberry_django_auth-0.374.4/PKG-INFO` & `strawberry_django_auth-0.374.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strawberry-django-auth
-Version: 0.374.4
+Version: 0.374.5
 Summary: Graphql authentication system with Strawberry for Django.
 License: MIT
 Author: Nir.J Benlulu
 Author-email: nrbnlulu@gmail.com
 Maintainer: Nir.J Benlulu
 Maintainer-email: nrbnlulu@gmail.com
 Requires-Python: >=3.8,<3.12
```

