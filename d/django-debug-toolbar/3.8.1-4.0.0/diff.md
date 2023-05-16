# Comparing `tmp/django_debug_toolbar-3.8.1.tar.gz` & `tmp/django_debug_toolbar-4.0.0.tar.gz`

## Comparing `django_debug_toolbar-3.8.1.tar` & `django_debug_toolbar-4.0.0.tar`

### file list

```diff
@@ -1,117 +1,116 @@
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/CONTRIBUTING.md
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/__init__.py
--rw-r--r--   0        0        0     5639 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/apps.py
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/decorators.py
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/forms.py
--rw-r--r--   0        0        0     3918 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/middleware.py
--rw-r--r--   0        0        0     2918 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/settings.py
--rw-r--r--   0        0        0     6238 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/toolbar.py
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/urls.py
--rw-r--r--   0        0        0    12281 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/utils.py
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/views.py
--rw-r--r--   0        0        0     2875 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/locale/ca/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    14620 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/locale/ca/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     9526 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/locale/cs/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    17589 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/locale/cs/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    10180 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    18512 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    14978 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     9967 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    18810 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     6597 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/locale/fa/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    17417 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/locale/fa/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     4659 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/locale/fi/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    15320 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/locale/fi/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    10291 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    19006 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/locale/he/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    14358 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/locale/he/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2948 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/locale/id/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    14488 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/locale/id/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     8532 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    17907 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/locale/it/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/locale/ja/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    15916 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/locale/ja/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     4274 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/locale/nl/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    15143 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/locale/nl/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     4810 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/locale/pl/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    15793 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/locale/pl/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/locale/pt/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    14821 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/locale/pt/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     9018 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    17059 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/locale/pt_BR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    11888 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    21517 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     9984 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/locale/sk/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    18180 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/locale/sk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/locale/sv_SE/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    14567 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/locale/sv_SE/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    14831 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/locale/uk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     8538 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/locale/zh_CN/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    16282 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/locale/zh_CN/LC_MESSAGES/django.po
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/management/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/management/commands/__init__.py
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/management/commands/debugsqlshell.py
--rw-r--r--   0        0        0     8127 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/panels/__init__.py
--rw-r--r--   0        0        0     8024 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/panels/cache.py
--rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/panels/headers.py
--rw-r--r--   0        0        0     3489 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/panels/logging.py
--rw-r--r--   0        0        0     5680 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/panels/profiling.py
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/panels/redirects.py
--rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/panels/request.py
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/panels/settings.py
--rw-r--r--   0        0        0     3393 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/panels/signals.py
--rw-r--r--   0        0        0     6395 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/panels/staticfiles.py
--rw-r--r--   0        0        0     4140 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/panels/timer.py
--rw-r--r--   0        0        0     1959 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/panels/versions.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/panels/history/__init__.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/panels/history/forms.py
--rw-r--r--   0        0        0     3771 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/panels/history/panel.py
--rw-r--r--   0        0        0     2614 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/panels/history/views.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/panels/sql/__init__.py
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/panels/sql/forms.py
--rw-r--r--   0        0        0    10518 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/panels/sql/panel.py
--rw-r--r--   0        0        0     9444 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/panels/sql/tracking.py
--rw-r--r--   0        0        0     2817 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/panels/sql/utils.py
--rw-r--r--   0        0        0     5206 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/panels/sql/views.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/panels/templates/__init__.py
--rw-r--r--   0        0        0     8450 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/panels/templates/panel.py
--rw-r--r--   0        0        0     2246 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/panels/templates/views.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/static/debug_toolbar/css/print.css
--rw-r--r--   0        0        0    12378 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/static/debug_toolbar/css/toolbar.css
--rw-r--r--   0        0        0     3330 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/static/debug_toolbar/js/history.js
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/static/debug_toolbar/js/redirect.js
--rw-r--r--   0        0        0     3686 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/static/debug_toolbar/js/timer.js
--rw-r--r--   0        0        0    13404 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/static/debug_toolbar/js/toolbar.js
--rw-r--r--   0        0        0     4527 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/static/debug_toolbar/js/utils.js
--rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/templates/debug_toolbar/base.html
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/templates/debug_toolbar/redirect.html
--rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/templates/debug_toolbar/includes/panel_button.html
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/templates/debug_toolbar/includes/panel_content.html
--rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/templates/debug_toolbar/panels/cache.html
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/templates/debug_toolbar/panels/headers.html
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/templates/debug_toolbar/panels/history.html
--rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/templates/debug_toolbar/panels/history_tr.html
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/templates/debug_toolbar/panels/logging.html
--rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/templates/debug_toolbar/panels/profiling.html
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/templates/debug_toolbar/panels/request.html
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/templates/debug_toolbar/panels/request_variables.html
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/templates/debug_toolbar/panels/settings.html
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/templates/debug_toolbar/panels/signals.html
--rw-r--r--   0        0        0     5763 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/templates/debug_toolbar/panels/sql.html
--rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/templates/debug_toolbar/panels/sql_explain.html
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/templates/debug_toolbar/panels/sql_profile.html
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/templates/debug_toolbar/panels/sql_select.html
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/templates/debug_toolbar/panels/staticfiles.html
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/templates/debug_toolbar/panels/template_source.html
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/templates/debug_toolbar/panels/templates.html
--rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/templates/debug_toolbar/panels/timer.html
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/templates/debug_toolbar/panels/versions.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/debug_toolbar/templatetags/__init__.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/.gitignore
--rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/LICENSE
--rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/README.rst
--rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/pyproject.toml
--rw-r--r--   0        0        0     3870 2020-02-02 00:00:00.000000 django_debug_toolbar-3.8.1/PKG-INFO
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/__init__.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/_stubs.py
+-rw-r--r--   0        0        0     5639 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/apps.py
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/decorators.py
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/forms.py
+-rw-r--r--   0        0        0     3930 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/middleware.py
+-rw-r--r--   0        0        0     3228 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/settings.py
+-rw-r--r--   0        0        0     6239 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/toolbar.py
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/urls.py
+-rw-r--r--   0        0        0    13101 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/utils.py
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/views.py
+-rw-r--r--   0        0        0     2875 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/locale/ca/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    15096 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/locale/ca/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     9526 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    18361 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/locale/cs/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    10180 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    17796 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    14330 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     9967 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    18086 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     6597 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/locale/fa/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    16706 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/locale/fa/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     4659 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/locale/fi/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    16045 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/locale/fi/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    10291 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    18288 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/locale/he/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    14785 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/locale/he/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2948 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/locale/id/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    15032 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/locale/id/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     8532 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    17175 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/locale/it/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    15143 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/locale/ja/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     4274 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    15689 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/locale/nl/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     4810 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/locale/pl/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    16540 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/locale/pl/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/locale/pt/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    15300 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/locale/pt/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     9018 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    17812 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/locale/pt_BR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    11888 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    20656 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     9984 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/locale/sk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    19081 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/locale/sk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/locale/sv_SE/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    15128 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/locale/sv_SE/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    15296 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     8538 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/locale/zh_CN/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    16981 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/locale/zh_CN/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/management/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/management/commands/__init__.py
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/management/commands/debugsqlshell.py
+-rw-r--r--   0        0        0     8127 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/panels/__init__.py
+-rw-r--r--   0        0        0     8024 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/panels/cache.py
+-rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/panels/headers.py
+-rw-r--r--   0        0        0     5680 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/panels/profiling.py
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/panels/redirects.py
+-rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/panels/request.py
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/panels/settings.py
+-rw-r--r--   0        0        0     3393 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/panels/signals.py
+-rw-r--r--   0        0        0     6394 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/panels/staticfiles.py
+-rw-r--r--   0        0        0     4140 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/panels/timer.py
+-rw-r--r--   0        0        0     1959 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/panels/versions.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/panels/history/__init__.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/panels/history/forms.py
+-rw-r--r--   0        0        0     3771 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/panels/history/panel.py
+-rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/panels/history/views.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/panels/sql/__init__.py
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/panels/sql/forms.py
+-rw-r--r--   0        0        0    11583 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/panels/sql/panel.py
+-rw-r--r--   0        0        0    10064 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/panels/sql/tracking.py
+-rw-r--r--   0        0        0     2817 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/panels/sql/utils.py
+-rw-r--r--   0        0        0     5326 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/panels/sql/views.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/panels/templates/__init__.py
+-rw-r--r--   0        0        0     8450 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/panels/templates/panel.py
+-rw-r--r--   0        0        0     2306 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/panels/templates/views.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/static/debug_toolbar/css/print.css
+-rw-r--r--   0        0        0    12378 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/static/debug_toolbar/css/toolbar.css
+-rw-r--r--   0        0        0     3330 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/static/debug_toolbar/js/history.js
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/static/debug_toolbar/js/redirect.js
+-rw-r--r--   0        0        0     3686 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/static/debug_toolbar/js/timer.js
+-rw-r--r--   0        0        0    13404 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/static/debug_toolbar/js/toolbar.js
+-rw-r--r--   0        0        0     4527 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/static/debug_toolbar/js/utils.js
+-rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/templates/debug_toolbar/base.html
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/templates/debug_toolbar/redirect.html
+-rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/templates/debug_toolbar/includes/panel_button.html
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/templates/debug_toolbar/includes/panel_content.html
+-rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/templates/debug_toolbar/panels/cache.html
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/templates/debug_toolbar/panels/headers.html
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/templates/debug_toolbar/panels/history.html
+-rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/templates/debug_toolbar/panels/history_tr.html
+-rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/templates/debug_toolbar/panels/profiling.html
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/templates/debug_toolbar/panels/request.html
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/templates/debug_toolbar/panels/request_variables.html
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/templates/debug_toolbar/panels/settings.html
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/templates/debug_toolbar/panels/signals.html
+-rw-r--r--   0        0        0     5763 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/templates/debug_toolbar/panels/sql.html
+-rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/templates/debug_toolbar/panels/sql_explain.html
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/templates/debug_toolbar/panels/sql_profile.html
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/templates/debug_toolbar/panels/sql_select.html
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/templates/debug_toolbar/panels/staticfiles.html
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/templates/debug_toolbar/panels/template_source.html
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/templates/debug_toolbar/panels/templates.html
+-rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/templates/debug_toolbar/panels/timer.html
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/templates/debug_toolbar/panels/versions.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/debug_toolbar/templatetags/__init__.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/.gitignore
+-rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/LICENSE
+-rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/README.rst
+-rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3859 2020-02-02 00:00:00.000000 django_debug_toolbar-4.0.0/PKG-INFO
```

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/apps.py` & `django_debug_toolbar-4.0.0/debug_toolbar/apps.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/forms.py` & `django_debug_toolbar-4.0.0/debug_toolbar/forms.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/middleware.py` & `django_debug_toolbar-4.0.0/debug_toolbar/middleware.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 def show_toolbar(request):
     """
     Default function to determine whether to show the toolbar on a given page.
     """
     return settings.DEBUG and request.META.get("REMOTE_ADDR") in settings.INTERNAL_IPS
 
 
-@lru_cache()
+@lru_cache(maxsize=None)
 def get_show_toolbar():
     # If SHOW_TOOLBAR_CALLBACK is a string, which is the recommended
     # setup, resolve it to the corresponding callable.
     func_or_path = dt_settings.get_config()["SHOW_TOOLBAR_CALLBACK"]
     if isinstance(func_or_path, str):
         return import_string(func_or_path)
     else:
```

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/settings.py` & `django_debug_toolbar-4.0.0/debug_toolbar/settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import warnings
 from functools import lru_cache
 
 from django.conf import settings
 from django.dispatch import receiver
 from django.test.signals import setting_changed
 
 CONFIG_DEFAULTS = {
@@ -40,15 +41,15 @@
     "SKIP_TEMPLATE_PREFIXES": ("django/forms/widgets/", "admin/widgets/"),
     "SQL_WARNING_THRESHOLD": 500,  # milliseconds
     "OBSERVE_REQUEST_CALLBACK": "debug_toolbar.toolbar.observe_request",
     "TOOLBAR_LANGUAGE": None,
 }
 
 
-@lru_cache()
+@lru_cache(maxsize=None)
 def get_config():
     USER_CONFIG = getattr(settings, "DEBUG_TOOLBAR_CONFIG", {})
     CONFIG = CONFIG_DEFAULTS.copy()
     CONFIG.update(USER_CONFIG)
     return CONFIG
 
 
@@ -60,26 +61,33 @@
     "debug_toolbar.panels.headers.HeadersPanel",
     "debug_toolbar.panels.request.RequestPanel",
     "debug_toolbar.panels.sql.SQLPanel",
     "debug_toolbar.panels.staticfiles.StaticFilesPanel",
     "debug_toolbar.panels.templates.TemplatesPanel",
     "debug_toolbar.panels.cache.CachePanel",
     "debug_toolbar.panels.signals.SignalsPanel",
-    "debug_toolbar.panels.logging.LoggingPanel",
     "debug_toolbar.panels.redirects.RedirectsPanel",
     "debug_toolbar.panels.profiling.ProfilingPanel",
 ]
 
 
-@lru_cache()
+@lru_cache(maxsize=None)
 def get_panels():
     try:
         PANELS = list(settings.DEBUG_TOOLBAR_PANELS)
     except AttributeError:
         PANELS = PANELS_DEFAULTS
+
+    logging_panel = "debug_toolbar.panels.logging.LoggingPanel"
+    if logging_panel in PANELS:
+        PANELS = [panel for panel in PANELS if panel != logging_panel]
+        warnings.warn(
+            f"Please remove {logging_panel} from your DEBUG_TOOLBAR_PANELS setting.",
+            DeprecationWarning,
+        )
     return PANELS
 
 
 @receiver(setting_changed)
 def update_toolbar_config(*, setting, **kwargs):
     """
     Refresh configuration when overriding settings.
```

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/toolbar.py` & `django_debug_toolbar-4.0.0/debug_toolbar/toolbar.py`

 * *Files 0% similar despite different names*

```diff
@@ -162,15 +162,15 @@
                 request.path, getattr(request, "urlconf", None)
             )
         except Resolver404:
             return False
         return resolver_match.namespaces and resolver_match.namespaces[-1] == APP_NAME
 
     @staticmethod
-    @lru_cache(maxsize=128)
+    @lru_cache(maxsize=None)
     def get_observe_request():
         # If OBSERVE_REQUEST_CALLBACK is a string, which is the recommended
         # setup, resolve it to the corresponding callable.
         func_or_path = dt_settings.get_config()["OBSERVE_REQUEST_CALLBACK"]
         if isinstance(func_or_path, str):
             return import_string(func_or_path)
         else:
```

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/utils.py` & `django_debug_toolbar-4.0.0/debug_toolbar/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,53 +1,55 @@
 import inspect
 import linecache
 import os.path
 import sys
 import warnings
-from pprint import pformat
+from pprint import PrettyPrinter, pformat
+from typing import Any, Dict, List, Optional, Sequence, Tuple, Union
 
 from asgiref.local import Local
+from django.http import QueryDict
 from django.template import Node
 from django.utils.html import format_html
-from django.utils.safestring import mark_safe
+from django.utils.safestring import SafeString, mark_safe
 
-from debug_toolbar import settings as dt_settings
+from debug_toolbar import _stubs as stubs, settings as dt_settings
 
 try:
     import threading
 except ImportError:
     threading = None
 
 
 _local_data = Local()
 
 
-def _is_excluded_frame(frame, excluded_modules):
+def _is_excluded_frame(frame: Any, excluded_modules: Optional[Sequence[str]]) -> bool:
     if not excluded_modules:
         return False
     frame_module = frame.f_globals.get("__name__")
     if not isinstance(frame_module, str):
         return False
     return any(
         frame_module == excluded_module
         or frame_module.startswith(excluded_module + ".")
         for excluded_module in excluded_modules
     )
 
 
-def _stack_trace_deprecation_warning():
+def _stack_trace_deprecation_warning() -> None:
     warnings.warn(
         "get_stack() and tidy_stacktrace() are deprecated in favor of"
         " get_stack_trace()",
         DeprecationWarning,
         stacklevel=2,
     )
 
 
-def tidy_stacktrace(stack):
+def tidy_stacktrace(stack: List[stubs.InspectStack]) -> stubs.TidyStackTrace:
     """
     Clean up stacktrace and remove all entries that are excluded by the
     HIDE_IN_STACKTRACES setting.
 
     ``stack`` should be a list of frame tuples from ``inspect.stack()`` or
     ``debug_toolbar.utils.get_stack()``.
     """
@@ -56,23 +58,23 @@
     trace = []
     excluded_modules = dt_settings.get_config()["HIDE_IN_STACKTRACES"]
     for frame, path, line_no, func_name, text in (f[:5] for f in stack):
         if _is_excluded_frame(frame, excluded_modules):
             continue
         text = "".join(text).strip() if text else ""
         frame_locals = (
-            frame.f_locals
+            pformat(frame.f_locals)
             if dt_settings.get_config()["ENABLE_STACKTRACES_LOCALS"]
             else None
         )
         trace.append((path, line_no, func_name, text, frame_locals))
     return trace
 
 
-def render_stacktrace(trace):
+def render_stacktrace(trace: stubs.TidyStackTrace) -> SafeString:
     show_locals = dt_settings.get_config()["ENABLE_STACKTRACES_LOCALS"]
     html = ""
     for abspath, lineno, func, code, locals_ in trace:
         if os.path.sep in abspath:
             directory, filename = abspath.rsplit(os.path.sep, 1)
             # We want the separator to appear in the UI so add it back.
             directory += os.path.sep
@@ -93,21 +95,21 @@
             func,
             lineno,
             code,
         )
         if show_locals:
             html += format_html(
                 '  <pre class="djdt-locals">{}</pre>\n',
-                pformat(locals_),
+                locals_,
             )
         html += "\n"
     return mark_safe(html)
 
 
-def get_template_info():
+def get_template_info() -> Optional[Dict[str, Any]]:
     template_info = None
     cur_frame = sys._getframe().f_back
     try:
         while cur_frame is not None:
             in_utils_module = cur_frame.f_code.co_filename.endswith(
                 "/debug_toolbar/utils.py"
             )
@@ -127,58 +129,62 @@
             cur_frame = cur_frame.f_back
     except Exception:
         pass
     del cur_frame
     return template_info
 
 
-def get_template_context(node, context, context_lines=3):
+def get_template_context(
+    node: Node, context: stubs.RequestContext, context_lines: int = 3
+) -> Dict[str, Any]:
     line, source_lines, name = get_template_source_from_exception_info(node, context)
     debug_context = []
     start = max(1, line - context_lines)
     end = line + 1 + context_lines
 
     for line_num, content in source_lines:
         if start <= line_num <= end:
             debug_context.append(
                 {"num": line_num, "content": content, "highlight": (line_num == line)}
             )
 
     return {"name": name, "context": debug_context}
 
 
-def get_template_source_from_exception_info(node, context):
+def get_template_source_from_exception_info(
+    node: Node, context: stubs.RequestContext
+) -> Tuple[int, List[Tuple[int, str]], str]:
     if context.template.origin == node.origin:
         exception_info = context.template.get_exception_info(
             Exception("DDT"), node.token
         )
     else:
         exception_info = context.render_context.template.get_exception_info(
             Exception("DDT"), node.token
         )
     line = exception_info["line"]
     source_lines = exception_info["source_lines"]
     name = exception_info["name"]
     return line, source_lines, name
 
 
-def get_name_from_obj(obj):
+def get_name_from_obj(obj: Any) -> str:
     if hasattr(obj, "__name__"):
         name = obj.__name__
     else:
         name = obj.__class__.__name__
 
     if hasattr(obj, "__module__"):
         module = obj.__module__
         name = f"{module}.{name}"
 
     return name
 
 
-def getframeinfo(frame, context=1):
+def getframeinfo(frame: Any, context: int = 1) -> inspect.Traceback:
     """
     Get information about a frame or traceback object.
 
     A tuple of five things is returned: the filename, the line number of
     the current line, the function name, a list of lines of context from
     the source code, and the index of the current line within that list.
     The optional second argument specifies the number of lines of context
@@ -209,29 +215,31 @@
             index = lineno - 1 - start
     else:
         lines = index = None
 
     return inspect.Traceback(filename, lineno, frame.f_code.co_name, lines, index)
 
 
-def get_sorted_request_variable(variable):
+def get_sorted_request_variable(
+    variable: Union[Dict[str, Any], QueryDict]
+) -> Dict[str, Union[List[Tuple[str, Any]], Any]]:
     """
     Get a data structure for showing a sorted list of variables from the
     request data.
     """
     try:
         if isinstance(variable, dict):
             return {"list": [(k, variable.get(k)) for k in sorted(variable)]}
         else:
             return {"list": [(k, variable.getlist(k)) for k in sorted(variable)]}
     except TypeError:
         return {"raw": variable}
 
 
-def get_stack(context=1):
+def get_stack(context=1) -> List[stubs.InspectStack]:
     """
     Get a list of records for a frame and all higher (calling) frames.
 
     Each record contains a frame object, filename, line number, function
     name, a list of lines of context, and index within the context.
 
     Modified version of ``inspect.stack()`` which calls our own ``getframeinfo()``
@@ -254,14 +262,16 @@
             skip -= 1
         else:
             yield frame
         frame = frame.f_back
 
 
 class _StackTraceRecorder:
+    pretty_printer = PrettyPrinter()
+
     def __init__(self):
         self.filename_cache = {}
 
     def get_source_file(self, frame):
         frame_filename = frame.f_code.co_filename
 
         value = self.filename_cache.get(frame_filename)
@@ -276,15 +286,21 @@
                 # encounters the filename in this frame.
                 linecache.checkcache(filename)
             value = (filename, is_source)
             self.filename_cache[frame_filename] = value
 
         return value
 
-    def get_stack_trace(self, *, excluded_modules=None, include_locals=False, skip=0):
+    def get_stack_trace(
+        self,
+        *,
+        excluded_modules: Optional[Sequence[str]] = None,
+        include_locals: bool = False,
+        skip: int = 0,
+    ):
         trace = []
         skip += 1  # Skip the frame for this method.
         for frame in _stack_frames(skip=skip):
             if _is_excluded_frame(frame, excluded_modules):
                 continue
 
             filename, is_source = self.get_source_file(frame)
@@ -297,15 +313,18 @@
                 module_globals = module.__dict__ if module is not None else None
                 source_line = linecache.getline(
                     filename, line_no, module_globals
                 ).strip()
             else:
                 source_line = ""
 
-            frame_locals = frame.f_locals if include_locals else None
+            if include_locals:
+                frame_locals = self.pretty_printer.pformat(frame.f_locals)
+            else:
+                frame_locals = None
 
             trace.append((filename, line_no, func_name, source_line, frame_locals))
         trace.reverse()
         return trace
 
 
 def get_stack_trace(*, skip=0):
```

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/views.py` & `django_debug_toolbar-4.0.0/debug_toolbar/views.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from django.http import JsonResponse
 from django.utils.html import escape
 from django.utils.translation import gettext as _
 
-from debug_toolbar.decorators import require_show_toolbar
+from debug_toolbar.decorators import render_with_toolbar_language, require_show_toolbar
 from debug_toolbar.toolbar import DebugToolbar
 
 
 @require_show_toolbar
+@render_with_toolbar_language
 def render_panel(request):
     """Render the contents of a panel"""
     toolbar = DebugToolbar.fetch(request.GET["store_id"])
     if toolbar is None:
         content = _(
             "Data for this panel isn't available anymore. "
             "Please reload the page and retry."
```

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/locale/ca/LC_MESSAGES/django.mo` & `django_debug_toolbar-4.0.0/debug_toolbar/locale/ca/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/locale/ca/LC_MESSAGES/django.po` & `django_debug_toolbar-4.0.0/debug_toolbar/locale/en/LC_MESSAGES/django.po`

 * *Files 11% similar despite different names*

```diff
@@ -1,363 +1,345 @@
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 #
 #
-# Translators:
-# Libre El Chaval <el.libre@gmail.com>, 2013
 msgid ""
 msgstr ""
 "Project-Id-Version: Django Debug Toolbar\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2014-04-25 21:52+0200\n"
-"PO-Revision-Date: 2014-04-25 19:53+0000\n"
-"Last-Translator: Aymeric Augustin <aymeric.augustin@m4x.org>\n"
-"Language-Team: Catalan (http://www.transifex.com/projects/p/django-debug-toolbar/language/ca/)\n"
+"POT-Creation-Date: 2023-01-20 17:23+0100\n"
+"PO-Revision-Date: 2012-03-31 20:10+0000\n"
+"Last-Translator: \n"
+"Language-Team: \n"
+"Language: en\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: ca\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Plural-Forms: nplurals=2; plural=(n != 1)\n"
 
-#: apps.py:11
+#: apps.py:15
 msgid "Debug Toolbar"
 msgstr ""
 
-#: views.py:14
-msgid ""
-"Data for this panel isn't available anymore. Please reload the page and "
-"retry."
-msgstr ""
-
-#: panels/cache.py:191
+#: panels/cache.py:180
 msgid "Cache"
-msgstr "Caxè"
+msgstr ""
 
-#: panels/cache.py:196
+#: panels/cache.py:186
 #, python-format
 msgid "%(cache_calls)d call in %(time).2fms"
 msgid_plural "%(cache_calls)d calls in %(time).2fms"
 msgstr[0] ""
 msgstr[1] ""
 
-#: panels/cache.py:204
+#: panels/cache.py:195
 #, python-format
 msgid "Cache calls from %(count)d backend"
 msgid_plural "Cache calls from %(count)d backends"
 msgstr[0] ""
 msgstr[1] ""
 
-#: panels/headers.py:35
+#: panels/headers.py:31
 msgid "Headers"
-msgstr "Encapçalaments"
-
-#: panels/logging.py:64
-msgid "Logging"
-msgstr "Entrant"
-
-#: panels/logging.py:70
-#, python-format
-msgid "%(count)s message"
-msgid_plural "%(count)s messages"
-msgstr[0] ""
-msgstr[1] ""
+msgstr ""
 
-#: panels/logging.py:73
-msgid "Log messages"
-msgstr "Registre de missatges"
+#: panels/history/panel.py:18 panels/history/panel.py:19
+msgid "History"
+msgstr ""
 
-#: panels/profiling.py:127
+#: panels/profiling.py:140
 msgid "Profiling"
 msgstr ""
 
-#: panels/redirects.py:17
+#: panels/redirects.py:14
 msgid "Intercept redirects"
 msgstr ""
 
-#: panels/request.py:18
+#: panels/request.py:16
 msgid "Request"
-msgstr "Demanar"
+msgstr ""
 
-#: panels/request.py:35
+#: panels/request.py:36
 msgid "<no view>"
 msgstr ""
 
-#: panels/request.py:47
+#: panels/request.py:53
 msgid "<unavailable>"
 msgstr ""
 
-#: panels/settings.py:20
+#: panels/settings.py:17
 msgid "Settings"
-msgstr "Configuració"
+msgstr ""
 
-#: panels/settings.py:23
+#: panels/settings.py:20
 #, python-format
-msgid "Settings from <code>%s</code>"
+msgid "Settings from %s"
 msgstr ""
 
-#: panels/signals.py:45
+#: panels/signals.py:57
 #, python-format
 msgid "%(num_receivers)d receiver of 1 signal"
 msgid_plural "%(num_receivers)d receivers of 1 signal"
 msgstr[0] ""
 msgstr[1] ""
 
-#: panels/signals.py:48
+#: panels/signals.py:62
 #, python-format
 msgid "%(num_receivers)d receiver of %(num_signals)d signals"
 msgid_plural "%(num_receivers)d receivers of %(num_signals)d signals"
 msgstr[0] ""
 msgstr[1] ""
 
-#: panels/signals.py:53
+#: panels/signals.py:67
 msgid "Signals"
-msgstr "Senyals"
+msgstr ""
+
+#: panels/sql/panel.py:23
+msgid "Autocommit"
+msgstr ""
 
-#: panels/staticfiles.py:89
+#: panels/sql/panel.py:24
+msgid "Read uncommitted"
+msgstr ""
+
+#: panels/sql/panel.py:25
+msgid "Read committed"
+msgstr ""
+
+#: panels/sql/panel.py:26
+msgid "Repeatable read"
+msgstr ""
+
+#: panels/sql/panel.py:27
+msgid "Serializable"
+msgstr ""
+
+#: panels/sql/panel.py:39
+msgid "Idle"
+msgstr ""
+
+#: panels/sql/panel.py:40
+msgid "Active"
+msgstr ""
+
+#: panels/sql/panel.py:41
+msgid "In transaction"
+msgstr ""
+
+#: panels/sql/panel.py:42
+msgid "In error"
+msgstr ""
+
+#: panels/sql/panel.py:43
+msgid "Unknown"
+msgstr ""
+
+#: panels/sql/panel.py:130
+msgid "SQL"
+msgstr ""
+
+#: panels/sql/panel.py:135
+#, python-format
+msgid "%(query_count)d query in %(sql_time).2fms"
+msgid_plural "%(query_count)d queries in %(sql_time).2fms"
+msgstr[0] ""
+msgstr[1] ""
+
+#: panels/sql/panel.py:147
+#, python-format
+msgid "SQL queries from %(count)d connection"
+msgid_plural "SQL queries from %(count)d connections"
+msgstr[0] ""
+msgstr[1] ""
+
+#: panels/staticfiles.py:84
 #, python-format
 msgid "Static files (%(num_found)s found, %(num_used)s used)"
 msgstr ""
 
-#: panels/staticfiles.py:107
+#: panels/staticfiles.py:105
 msgid "Static files"
 msgstr ""
 
-#: panels/staticfiles.py:112
+#: panels/staticfiles.py:111
 #, python-format
 msgid "%(num_used)s file used"
 msgid_plural "%(num_used)s files used"
 msgstr[0] ""
 msgstr[1] ""
 
-#: panels/timer.py:23
+#: panels/templates/panel.py:143
+msgid "Templates"
+msgstr ""
+
+#: panels/templates/panel.py:148
+#, python-format
+msgid "Templates (%(num_templates)s rendered)"
+msgstr ""
+
+#: panels/templates/panel.py:180
+msgid "No origin"
+msgstr ""
+
+#: panels/timer.py:25
 #, python-format
 msgid "CPU: %(cum)0.2fms (%(total)0.2fms)"
 msgstr ""
 
-#: panels/timer.py:28
+#: panels/timer.py:30
 #, python-format
 msgid "Total: %0.2fms"
-msgstr "Total: %0.2fms"
+msgstr ""
 
-#: panels/timer.py:34 templates/debug_toolbar/panels/logging.html:7
+#: panels/timer.py:36 templates/debug_toolbar/panels/history.html:9
 #: templates/debug_toolbar/panels/sql_explain.html:11
 #: templates/debug_toolbar/panels/sql_profile.html:12
 #: templates/debug_toolbar/panels/sql_select.html:11
 msgid "Time"
-msgstr "Hora"
+msgstr ""
 
-#: panels/timer.py:42
+#: panels/timer.py:44
 msgid "User CPU time"
 msgstr ""
 
-#: panels/timer.py:42
+#: panels/timer.py:44
 #, python-format
 msgid "%(utime)0.3f msec"
 msgstr ""
 
-#: panels/timer.py:43
+#: panels/timer.py:45
 msgid "System CPU time"
 msgstr ""
 
-#: panels/timer.py:43
+#: panels/timer.py:45
 #, python-format
 msgid "%(stime)0.3f msec"
 msgstr ""
 
-#: panels/timer.py:44
+#: panels/timer.py:46
 msgid "Total CPU time"
 msgstr ""
 
-#: panels/timer.py:44
+#: panels/timer.py:46
 #, python-format
 msgid "%(total)0.3f msec"
 msgstr ""
 
-#: panels/timer.py:45
+#: panels/timer.py:47
 msgid "Elapsed time"
-msgstr "Temps emprat"
+msgstr ""
 
-#: panels/timer.py:45
+#: panels/timer.py:47
 #, python-format
 msgid "%(total_time)0.3f msec"
 msgstr ""
 
-#: panels/timer.py:46
+#: panels/timer.py:49
 msgid "Context switches"
 msgstr ""
 
-#: panels/timer.py:46
+#: panels/timer.py:50
 #, python-format
 msgid "%(vcsw)d voluntary, %(ivcsw)d involuntary"
 msgstr ""
 
-#: panels/versions.py:25
+#: panels/versions.py:19
 msgid "Versions"
-msgstr "Versions"
-
-#: panels/sql/panel.py:22
-msgid "Autocommit"
-msgstr ""
-
-#: panels/sql/panel.py:23
-msgid "Read uncommitted"
-msgstr ""
-
-#: panels/sql/panel.py:24
-msgid "Read committed"
 msgstr ""
 
-#: panels/sql/panel.py:25
-msgid "Repeatable read"
-msgstr ""
-
-#: panels/sql/panel.py:26
-msgid "Serializable"
-msgstr "Seriable"
-
-#: panels/sql/panel.py:37
-msgid "Idle"
+#: templates/debug_toolbar/base.html:22
+msgid "Hide toolbar"
 msgstr ""
 
-#: panels/sql/panel.py:38
-msgid "Active"
-msgstr "Actiu"
-
-#: panels/sql/panel.py:39
-msgid "In transaction"
-msgstr "En transacció"
-
-#: panels/sql/panel.py:40
-msgid "In error"
+#: templates/debug_toolbar/base.html:22
+msgid "Hide"
 msgstr ""
 
-#: panels/sql/panel.py:41
-msgid "Unknown"
-msgstr "Desconegut"
-
-#: panels/sql/panel.py:105
-msgid "SQL"
-msgstr "SQL"
-
-#: panels/templates/panel.py:141
-msgid "Templates"
-msgstr "Plantilles"
-
-#: panels/templates/panel.py:146
-#, python-format
-msgid "Templates (%(num_templates)s rendered)"
+#: templates/debug_toolbar/base.html:29
+msgid "Show toolbar"
 msgstr ""
 
-#: templates/debug_toolbar/base.html:19
-msgid "Hide toolbar"
-msgstr "Amagar barra d'eina"
-
-#: templates/debug_toolbar/base.html:19
-msgid "Hide"
-msgstr "Amagar"
-
-#: templates/debug_toolbar/base.html:25
+#: templates/debug_toolbar/includes/panel_button.html:4
 msgid "Disable for next and successive requests"
 msgstr ""
 
-#: templates/debug_toolbar/base.html:25
+#: templates/debug_toolbar/includes/panel_button.html:4
 msgid "Enable for next and successive requests"
 msgstr ""
 
-#: templates/debug_toolbar/base.html:47
-msgid "Show toolbar"
-msgstr "Mostrar barra d'eines"
-
-#: templates/debug_toolbar/base.html:53
-msgid "Close"
-msgstr "Tancar"
-
-#: templates/debug_toolbar/redirect.html:8
-msgid "Location:"
-msgstr "Ubicació:"
-
-#: templates/debug_toolbar/redirect.html:10
-msgid ""
-"The Django Debug Toolbar has intercepted a redirect to the above URL for "
-"debug viewing purposes. You can click the above link to continue with the "
-"redirect as normal."
-msgstr ""
-
 #: templates/debug_toolbar/panels/cache.html:2
 msgid "Summary"
-msgstr "Resum"
+msgstr ""
 
 #: templates/debug_toolbar/panels/cache.html:6
 msgid "Total calls"
-msgstr "Total crides"
+msgstr ""
 
 #: templates/debug_toolbar/panels/cache.html:7
 msgid "Total time"
-msgstr "Total temps"
+msgstr ""
 
 #: templates/debug_toolbar/panels/cache.html:8
 msgid "Cache hits"
 msgstr ""
 
 #: templates/debug_toolbar/panels/cache.html:9
 msgid "Cache misses"
 msgstr ""
 
 #: templates/debug_toolbar/panels/cache.html:21
 msgid "Commands"
-msgstr "Comandes"
+msgstr ""
 
 #: templates/debug_toolbar/panels/cache.html:39
 msgid "Calls"
-msgstr "Crides"
+msgstr ""
 
 #: templates/debug_toolbar/panels/cache.html:43
-#: templates/debug_toolbar/panels/sql.html:20
+#: templates/debug_toolbar/panels/sql.html:36
 msgid "Time (ms)"
-msgstr "Temps (ms)"
+msgstr ""
 
 #: templates/debug_toolbar/panels/cache.html:44
 msgid "Type"
-msgstr "Tipus"
+msgstr ""
 
 #: templates/debug_toolbar/panels/cache.html:45
 #: templates/debug_toolbar/panels/request.html:8
 msgid "Arguments"
 msgstr ""
 
 #: templates/debug_toolbar/panels/cache.html:46
 #: templates/debug_toolbar/panels/request.html:9
 msgid "Keyword arguments"
 msgstr ""
 
 #: templates/debug_toolbar/panels/cache.html:47
 msgid "Backend"
-msgstr "Administració"
+msgstr ""
 
 #: templates/debug_toolbar/panels/headers.html:3
 msgid "Request headers"
 msgstr ""
 
 #: templates/debug_toolbar/panels/headers.html:8
 #: templates/debug_toolbar/panels/headers.html:27
 #: templates/debug_toolbar/panels/headers.html:48
 msgid "Key"
-msgstr "Clau"
+msgstr ""
 
 #: templates/debug_toolbar/panels/headers.html:9
 #: templates/debug_toolbar/panels/headers.html:28
 #: templates/debug_toolbar/panels/headers.html:49
-#: templates/debug_toolbar/panels/request.html:33
-#: templates/debug_toolbar/panels/request.html:59
-#: templates/debug_toolbar/panels/request.html:85
-#: templates/debug_toolbar/panels/request.html:110
+#: templates/debug_toolbar/panels/history_tr.html:23
+#: templates/debug_toolbar/panels/request_variables.html:12
 #: templates/debug_toolbar/panels/settings.html:6
 #: templates/debug_toolbar/panels/timer.html:11
 msgid "Value"
-msgstr "Valor"
+msgstr ""
 
 #: templates/debug_toolbar/panels/headers.html:22
 msgid "Response headers"
 msgstr ""
 
 #: templates/debug_toolbar/panels/headers.html:41
 msgid "WSGI environ"
@@ -365,243 +347,251 @@
 
 #: templates/debug_toolbar/panels/headers.html:43
 msgid ""
 "Since the WSGI environ inherits the environment of the server, only a "
 "significant subset is shown below."
 msgstr ""
 
-#: templates/debug_toolbar/panels/logging.html:6
-msgid "Level"
-msgstr "Nivell"
-
-#: templates/debug_toolbar/panels/logging.html:8
-msgid "Channel"
-msgstr "Canal"
-
-#: templates/debug_toolbar/panels/logging.html:9
-msgid "Message"
-msgstr "Missatge"
+#: templates/debug_toolbar/panels/history.html:10
+msgid "Method"
+msgstr ""
 
-#: templates/debug_toolbar/panels/logging.html:10
-#: templates/debug_toolbar/panels/staticfiles.html:45
-msgid "Location"
-msgstr "Ubicació"
+#: templates/debug_toolbar/panels/history.html:11
+#: templates/debug_toolbar/panels/staticfiles.html:43
+msgid "Path"
+msgstr ""
+
+#: templates/debug_toolbar/panels/history.html:12
+msgid "Request Variables"
+msgstr ""
+
+#: templates/debug_toolbar/panels/history.html:13
+msgid "Status"
+msgstr ""
+
+#: templates/debug_toolbar/panels/history.html:14
+#: templates/debug_toolbar/panels/sql.html:37
+msgid "Action"
+msgstr ""
 
-#: templates/debug_toolbar/panels/logging.html:26
-msgid "No messages logged"
+#: templates/debug_toolbar/panels/history_tr.html:22
+#: templates/debug_toolbar/panels/request_variables.html:11
+msgid "Variable"
 msgstr ""
 
 #: templates/debug_toolbar/panels/profiling.html:5
 msgid "Call"
-msgstr "Cridar"
+msgstr ""
 
 #: templates/debug_toolbar/panels/profiling.html:6
 msgid "CumTime"
 msgstr ""
 
 #: templates/debug_toolbar/panels/profiling.html:7
 #: templates/debug_toolbar/panels/profiling.html:9
 msgid "Per"
-msgstr "Per"
+msgstr ""
 
 #: templates/debug_toolbar/panels/profiling.html:8
 msgid "TotTime"
-msgstr "TempsTotal"
+msgstr ""
 
 #: templates/debug_toolbar/panels/profiling.html:10
 msgid "Count"
-msgstr "Recomptar"
+msgstr ""
 
 #: templates/debug_toolbar/panels/request.html:3
 msgid "View information"
-msgstr "Veure informació"
+msgstr ""
 
 #: templates/debug_toolbar/panels/request.html:7
 msgid "View function"
 msgstr ""
 
 #: templates/debug_toolbar/panels/request.html:10
 msgid "URL name"
 msgstr ""
 
 #: templates/debug_toolbar/panels/request.html:24
 msgid "Cookies"
 msgstr ""
 
-#: templates/debug_toolbar/panels/request.html:32
-#: templates/debug_toolbar/panels/request.html:58
-#: templates/debug_toolbar/panels/request.html:84
-#: templates/debug_toolbar/panels/request.html:109
-msgid "Variable"
-msgstr "Variable"
-
-#: templates/debug_toolbar/panels/request.html:46
+#: templates/debug_toolbar/panels/request.html:27
 msgid "No cookies"
 msgstr ""
 
-#: templates/debug_toolbar/panels/request.html:50
+#: templates/debug_toolbar/panels/request.html:31
 msgid "Session data"
 msgstr ""
 
-#: templates/debug_toolbar/panels/request.html:72
+#: templates/debug_toolbar/panels/request.html:34
 msgid "No session data"
 msgstr ""
 
-#: templates/debug_toolbar/panels/request.html:76
+#: templates/debug_toolbar/panels/request.html:38
 msgid "GET data"
 msgstr ""
 
-#: templates/debug_toolbar/panels/request.html:98
+#: templates/debug_toolbar/panels/request.html:41
 msgid "No GET data"
-msgstr "Sense dades GET"
+msgstr ""
 
-#: templates/debug_toolbar/panels/request.html:102
+#: templates/debug_toolbar/panels/request.html:45
 msgid "POST data"
 msgstr ""
 
-#: templates/debug_toolbar/panels/request.html:123
+#: templates/debug_toolbar/panels/request.html:48
 msgid "No POST data"
-msgstr "Sense dades POST"
+msgstr ""
 
 #: templates/debug_toolbar/panels/settings.html:5
 msgid "Setting"
-msgstr "Configuració"
+msgstr ""
 
 #: templates/debug_toolbar/panels/signals.html:5
 msgid "Signal"
-msgstr "Senyal"
-
-#: templates/debug_toolbar/panels/signals.html:6
-msgid "Providing"
 msgstr ""
 
-#: templates/debug_toolbar/panels/signals.html:7
+#: templates/debug_toolbar/panels/signals.html:6
 msgid "Receivers"
-msgstr "Destinataris"
+msgstr ""
 
-#: templates/debug_toolbar/panels/sql.html:7
+#: templates/debug_toolbar/panels/sql.html:6
 #, python-format
 msgid "%(num)s query"
 msgid_plural "%(num)s queries"
 msgstr[0] ""
 msgstr[1] ""
 
-#: templates/debug_toolbar/panels/sql.html:18
+#: templates/debug_toolbar/panels/sql.html:8
+#, python-format
+msgid ""
+"including <abbr title=\"Similar queries are queries with the same SQL, but "
+"potentially different parameters.\">%(count)s similar</abbr>"
+msgstr ""
+
+#: templates/debug_toolbar/panels/sql.html:12
+#, python-format
+msgid ""
+"and <abbr title=\"Duplicate queries are identical to each other: they "
+"execute exactly the same SQL and parameters.\">%(dupes)s duplicates</abbr>"
+msgstr ""
+
+#: templates/debug_toolbar/panels/sql.html:34
 msgid "Query"
-msgstr "Petició"
+msgstr ""
 
-#: templates/debug_toolbar/panels/sql.html:19
+#: templates/debug_toolbar/panels/sql.html:35
 #: templates/debug_toolbar/panels/timer.html:36
 msgid "Timeline"
-msgstr "Línia temporal"
+msgstr ""
 
-#: templates/debug_toolbar/panels/sql.html:21
-msgid "Action"
-msgstr "Acció"
+#: templates/debug_toolbar/panels/sql.html:52
+#, python-format
+msgid "%(count)s similar queries."
+msgstr ""
 
-#: templates/debug_toolbar/panels/sql.html:64
+#: templates/debug_toolbar/panels/sql.html:58
+#, python-format
+msgid "Duplicated %(dupes)s times."
+msgstr ""
+
+#: templates/debug_toolbar/panels/sql.html:95
 msgid "Connection:"
-msgstr "Connexió:"
+msgstr ""
 
-#: templates/debug_toolbar/panels/sql.html:66
+#: templates/debug_toolbar/panels/sql.html:97
 msgid "Isolation level:"
 msgstr ""
 
-#: templates/debug_toolbar/panels/sql.html:69
+#: templates/debug_toolbar/panels/sql.html:100
 msgid "Transaction status:"
 msgstr ""
 
-#: templates/debug_toolbar/panels/sql.html:83
+#: templates/debug_toolbar/panels/sql.html:114
 msgid "(unknown)"
-msgstr "(desconegut)"
+msgstr ""
 
-#: templates/debug_toolbar/panels/sql.html:92
+#: templates/debug_toolbar/panels/sql.html:123
 msgid "No SQL queries were recorded during this request."
 msgstr ""
 
-#: templates/debug_toolbar/panels/sql_explain.html:3
-#: templates/debug_toolbar/panels/sql_profile.html:3
-#: templates/debug_toolbar/panels/sql_select.html:3
-#: templates/debug_toolbar/panels/template_source.html:3
-msgid "Back"
-msgstr "Tornar"
-
 #: templates/debug_toolbar/panels/sql_explain.html:4
 msgid "SQL explained"
 msgstr ""
 
 #: templates/debug_toolbar/panels/sql_explain.html:9
 #: templates/debug_toolbar/panels/sql_profile.html:10
 #: templates/debug_toolbar/panels/sql_select.html:9
 msgid "Executed SQL"
-msgstr "SQL Executat"
+msgstr ""
 
 #: templates/debug_toolbar/panels/sql_explain.html:13
 #: templates/debug_toolbar/panels/sql_profile.html:14
 #: templates/debug_toolbar/panels/sql_select.html:13
 msgid "Database"
-msgstr "Base de dades"
+msgstr ""
 
 #: templates/debug_toolbar/panels/sql_profile.html:4
 msgid "SQL profiled"
 msgstr ""
 
 #: templates/debug_toolbar/panels/sql_profile.html:37
 msgid "Error"
-msgstr "Error"
+msgstr ""
 
 #: templates/debug_toolbar/panels/sql_select.html:4
 msgid "SQL selected"
 msgstr ""
 
 #: templates/debug_toolbar/panels/sql_select.html:36
 msgid "Empty set"
 msgstr ""
 
-#: templates/debug_toolbar/panels/staticfiles.html:4
+#: templates/debug_toolbar/panels/staticfiles.html:3
 msgid "Static file path"
 msgid_plural "Static file paths"
 msgstr[0] ""
 msgstr[1] ""
 
-#: templates/debug_toolbar/panels/staticfiles.html:8
+#: templates/debug_toolbar/panels/staticfiles.html:7
 #, python-format
 msgid "(prefix %(prefix)s)"
 msgstr ""
 
-#: templates/debug_toolbar/panels/staticfiles.html:12
-#: templates/debug_toolbar/panels/staticfiles.html:23
-#: templates/debug_toolbar/panels/staticfiles.html:35
+#: templates/debug_toolbar/panels/staticfiles.html:11
+#: templates/debug_toolbar/panels/staticfiles.html:22
+#: templates/debug_toolbar/panels/staticfiles.html:34
 #: templates/debug_toolbar/panels/templates.html:10
-#: templates/debug_toolbar/panels/templates.html:28
-#: templates/debug_toolbar/panels/templates.html:43
+#: templates/debug_toolbar/panels/templates.html:30
+#: templates/debug_toolbar/panels/templates.html:47
 msgid "None"
-msgstr "Cap"
+msgstr ""
 
-#: templates/debug_toolbar/panels/staticfiles.html:15
+#: templates/debug_toolbar/panels/staticfiles.html:14
 msgid "Static file app"
 msgid_plural "Static file apps"
 msgstr[0] ""
 msgstr[1] ""
 
-#: templates/debug_toolbar/panels/staticfiles.html:26
+#: templates/debug_toolbar/panels/staticfiles.html:25
 msgid "Static file"
 msgid_plural "Static files"
 msgstr[0] ""
 msgstr[1] ""
 
-#: templates/debug_toolbar/panels/staticfiles.html:40
+#: templates/debug_toolbar/panels/staticfiles.html:39
 #, python-format
 msgid "%(payload_count)s file"
 msgid_plural "%(payload_count)s files"
 msgstr[0] ""
 msgstr[1] ""
 
 #: templates/debug_toolbar/panels/staticfiles.html:44
-msgid "Path"
+msgid "Location"
 msgstr ""
 
 #: templates/debug_toolbar/panels/template_source.html:4
 msgid "Template source:"
 msgstr ""
 
 #: templates/debug_toolbar/panels/templates.html:2
@@ -610,47 +600,68 @@
 msgstr[0] ""
 msgstr[1] ""
 
 #: templates/debug_toolbar/panels/templates.html:13
 msgid "Template"
 msgid_plural "Templates"
 msgstr[0] ""
-msgstr[1] "Plantilles"
+msgstr[1] ""
 
-#: templates/debug_toolbar/panels/templates.html:21
-#: templates/debug_toolbar/panels/templates.html:37
+#: templates/debug_toolbar/panels/templates.html:22
+#: templates/debug_toolbar/panels/templates.html:40
 msgid "Toggle context"
 msgstr ""
 
-#: templates/debug_toolbar/panels/templates.html:31
+#: templates/debug_toolbar/panels/templates.html:33
 msgid "Context processor"
 msgid_plural "Context processors"
 msgstr[0] ""
 msgstr[1] ""
 
 #: templates/debug_toolbar/panels/timer.html:2
 msgid "Resource usage"
 msgstr ""
 
 #: templates/debug_toolbar/panels/timer.html:10
 msgid "Resource"
-msgstr "Font"
+msgstr ""
 
 #: templates/debug_toolbar/panels/timer.html:26
 msgid "Browser timing"
 msgstr ""
 
 #: templates/debug_toolbar/panels/timer.html:35
 msgid "Timing attribute"
 msgstr ""
 
 #: templates/debug_toolbar/panels/timer.html:37
 msgid "Milliseconds since navigation start (+length)"
 msgstr ""
 
-#: templates/debug_toolbar/panels/versions.html:5
+#: templates/debug_toolbar/panels/versions.html:10
+msgid "Package"
+msgstr ""
+
+#: templates/debug_toolbar/panels/versions.html:11
 msgid "Name"
-msgstr "Nom"
+msgstr ""
 
-#: templates/debug_toolbar/panels/versions.html:6
+#: templates/debug_toolbar/panels/versions.html:12
 msgid "Version"
-msgstr "Versió"
+msgstr ""
+
+#: templates/debug_toolbar/redirect.html:10
+msgid "Location:"
+msgstr ""
+
+#: templates/debug_toolbar/redirect.html:12
+msgid ""
+"The Django Debug Toolbar has intercepted a redirect to the above URL for "
+"debug viewing purposes. You can click the above link to continue with the "
+"redirect as normal."
+msgstr ""
+
+#: views.py:16
+msgid ""
+"Data for this panel isn't available anymore. Please reload the page and "
+"retry."
+msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/locale/cs/LC_MESSAGES/django.mo` & `django_debug_toolbar-4.0.0/debug_toolbar/locale/cs/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/locale/cs/LC_MESSAGES/django.po` & `django_debug_toolbar-4.0.0/debug_toolbar/locale/cs/LC_MESSAGES/django.po`

 * *Files 4% similar despite different names*

```diff
@@ -4,294 +4,285 @@
 #
 # Translators:
 # Vlada Macek <macek@sandbox.cz>, 2013
 msgid ""
 msgstr ""
 "Project-Id-Version: Django Debug Toolbar\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2014-04-25 21:52+0200\n"
+"POT-Creation-Date: 2023-01-20 17:23+0100\n"
 "PO-Revision-Date: 2014-04-25 19:53+0000\n"
 "Last-Translator: Aymeric Augustin <aymeric.augustin@m4x.org>\n"
-"Language-Team: Czech (http://www.transifex.com/projects/p/django-debug-toolbar/language/cs/)\n"
+"Language-Team: Czech (http://www.transifex.com/projects/p/django-debug-"
+"toolbar/language/cs/)\n"
+"Language: cs\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: cs\n"
 "Plural-Forms: nplurals=3; plural=(n==1) ? 0 : (n>=2 && n<=4) ? 1 : 2;\n"
 
-#: apps.py:11
+#: apps.py:15
 msgid "Debug Toolbar"
 msgstr ""
 
-#: views.py:14
-msgid ""
-"Data for this panel isn't available anymore. Please reload the page and "
-"retry."
-msgstr "Data pro tento panel již nejsou k dispozici. Obnovte stránku a zkuste to znova."
-
-#: panels/cache.py:191
+#: panels/cache.py:180
 msgid "Cache"
 msgstr "Mezipaměť"
 
-#: panels/cache.py:196
+#: panels/cache.py:186
 #, python-format
 msgid "%(cache_calls)d call in %(time).2fms"
 msgid_plural "%(cache_calls)d calls in %(time).2fms"
 msgstr[0] "%(cache_calls)d volání během %(time).2fms"
 msgstr[1] "%(cache_calls)d volání během %(time).2fms"
 msgstr[2] "%(cache_calls)d volání během %(time).2fms"
 
-#: panels/cache.py:204
+#: panels/cache.py:195
 #, python-format
 msgid "Cache calls from %(count)d backend"
 msgid_plural "Cache calls from %(count)d backends"
 msgstr[0] "Volání mezipaměti z %(count)d backendu"
 msgstr[1] "Volání mezipaměti z %(count)d backendů"
 msgstr[2] "Volání mezipaměti z %(count)d backendů"
 
-#: panels/headers.py:35
+#: panels/headers.py:31
 msgid "Headers"
 msgstr "Záhlaví"
 
-#: panels/logging.py:64
-msgid "Logging"
-msgstr "Protokol"
-
-#: panels/logging.py:70
-#, python-format
-msgid "%(count)s message"
-msgid_plural "%(count)s messages"
-msgstr[0] "%(count)s zpráva"
-msgstr[1] "%(count)s zprávy"
-msgstr[2] "%(count)s zpráv"
-
-#: panels/logging.py:73
-msgid "Log messages"
-msgstr "Zprávy protokolu"
+#: panels/history/panel.py:18 panels/history/panel.py:19
+msgid "History"
+msgstr ""
 
-#: panels/profiling.py:127
+#: panels/profiling.py:140
 msgid "Profiling"
 msgstr "Profilování"
 
-#: panels/redirects.py:17
+#: panels/redirects.py:14
 msgid "Intercept redirects"
 msgstr "Zachycení přesměrování"
 
-#: panels/request.py:18
+#: panels/request.py:16
 msgid "Request"
 msgstr "Požadavek"
 
-#: panels/request.py:35
+#: panels/request.py:36
 msgid "<no view>"
 msgstr "<žádný pohled>"
 
-#: panels/request.py:47
+#: panels/request.py:53
 msgid "<unavailable>"
 msgstr "<není k dispozici>"
 
-#: panels/settings.py:20
+#: panels/settings.py:17
 msgid "Settings"
 msgstr "Settings"
 
-#: panels/settings.py:23
-#, python-format
-msgid "Settings from <code>%s</code>"
+#: panels/settings.py:20
+#, fuzzy, python-format
+#| msgid "Settings from <code>%s</code>"
+msgid "Settings from %s"
 msgstr "Nastavení z modulu <code>%s</code>"
 
-#: panels/signals.py:45
+#: panels/signals.py:57
 #, python-format
 msgid "%(num_receivers)d receiver of 1 signal"
 msgid_plural "%(num_receivers)d receivers of 1 signal"
 msgstr[0] "%(num_receivers)d příjemce 1 signálu"
 msgstr[1] "%(num_receivers)d příjemci 1 signálu"
 msgstr[2] "%(num_receivers)d příjemců 1 signálu"
 
-#: panels/signals.py:48
+#: panels/signals.py:62
 #, python-format
 msgid "%(num_receivers)d receiver of %(num_signals)d signals"
 msgid_plural "%(num_receivers)d receivers of %(num_signals)d signals"
 msgstr[0] "%(num_receivers)d příjemce %(num_signals)d signálů"
 msgstr[1] "%(num_receivers)d příjemci %(num_signals)d signálů"
 msgstr[2] "%(num_receivers)d příjemců %(num_signals)d signálů"
 
-#: panels/signals.py:53
+#: panels/signals.py:67
 msgid "Signals"
 msgstr "Signály"
 
-#: panels/staticfiles.py:89
+#: panels/sql/panel.py:23
+msgid "Autocommit"
+msgstr "Autocommit"
+
+#: panels/sql/panel.py:24
+msgid "Read uncommitted"
+msgstr "Read uncommitted"
+
+#: panels/sql/panel.py:25
+msgid "Read committed"
+msgstr "Read committed"
+
+#: panels/sql/panel.py:26
+msgid "Repeatable read"
+msgstr "Repeatable read"
+
+#: panels/sql/panel.py:27
+msgid "Serializable"
+msgstr "Serializable"
+
+#: panels/sql/panel.py:39
+msgid "Idle"
+msgstr "V klidu (idle)"
+
+#: panels/sql/panel.py:40
+msgid "Active"
+msgstr "Aktivní"
+
+#: panels/sql/panel.py:41
+msgid "In transaction"
+msgstr "Uvnitř transakce"
+
+#: panels/sql/panel.py:42
+msgid "In error"
+msgstr "V chybovém stavu"
+
+#: panels/sql/panel.py:43
+msgid "Unknown"
+msgstr "Neznámé"
+
+#: panels/sql/panel.py:130
+msgid "SQL"
+msgstr "SQL"
+
+#: panels/sql/panel.py:135
+#, fuzzy, python-format
+#| msgid "%(cache_calls)d call in %(time).2fms"
+#| msgid_plural "%(cache_calls)d calls in %(time).2fms"
+msgid "%(query_count)d query in %(sql_time).2fms"
+msgid_plural "%(query_count)d queries in %(sql_time).2fms"
+msgstr[0] "%(cache_calls)d volání během %(time).2fms"
+msgstr[1] "%(cache_calls)d volání během %(time).2fms"
+msgstr[2] "%(cache_calls)d volání během %(time).2fms"
+
+#: panels/sql/panel.py:147
+#, python-format
+msgid "SQL queries from %(count)d connection"
+msgid_plural "SQL queries from %(count)d connections"
+msgstr[0] ""
+msgstr[1] ""
+msgstr[2] ""
+
+#: panels/staticfiles.py:84
 #, python-format
 msgid "Static files (%(num_found)s found, %(num_used)s used)"
 msgstr "Statické soubory (nalezeno: %(num_found)s, použito: %(num_used)s)"
 
-#: panels/staticfiles.py:107
+#: panels/staticfiles.py:105
 msgid "Static files"
 msgstr "Statické soubory"
 
-#: panels/staticfiles.py:112
+#: panels/staticfiles.py:111
 #, python-format
 msgid "%(num_used)s file used"
 msgid_plural "%(num_used)s files used"
 msgstr[0] "%(num_used)s soubor použit"
 msgstr[1] "%(num_used)s soubory použity"
 msgstr[2] "%(num_used)s souborů použito"
 
-#: panels/timer.py:23
+#: panels/templates/panel.py:143
+msgid "Templates"
+msgstr "Šablony"
+
+#: panels/templates/panel.py:148
+#, python-format
+msgid "Templates (%(num_templates)s rendered)"
+msgstr "Šablony (renderovaných: %(num_templates)s)"
+
+#: panels/templates/panel.py:180
+msgid "No origin"
+msgstr ""
+
+#: panels/timer.py:25
 #, python-format
 msgid "CPU: %(cum)0.2fms (%(total)0.2fms)"
 msgstr "CPU: %(cum)0.2fms (%(total)0.2fms)"
 
-#: panels/timer.py:28
+#: panels/timer.py:30
 #, python-format
 msgid "Total: %0.2fms"
 msgstr "Celkem: %0.2fms"
 
-#: panels/timer.py:34 templates/debug_toolbar/panels/logging.html:7
+#: panels/timer.py:36 templates/debug_toolbar/panels/history.html:9
 #: templates/debug_toolbar/panels/sql_explain.html:11
 #: templates/debug_toolbar/panels/sql_profile.html:12
 #: templates/debug_toolbar/panels/sql_select.html:11
 msgid "Time"
 msgstr "Čas"
 
-#: panels/timer.py:42
+#: panels/timer.py:44
 msgid "User CPU time"
 msgstr "Uživatelský čas CPU"
 
-#: panels/timer.py:42
+#: panels/timer.py:44
 #, python-format
 msgid "%(utime)0.3f msec"
 msgstr "%(utime)0.3f msec"
 
-#: panels/timer.py:43
+#: panels/timer.py:45
 msgid "System CPU time"
 msgstr "Systémový čas CPU"
 
-#: panels/timer.py:43
+#: panels/timer.py:45
 #, python-format
 msgid "%(stime)0.3f msec"
 msgstr "%(stime)0.3f msec"
 
-#: panels/timer.py:44
+#: panels/timer.py:46
 msgid "Total CPU time"
 msgstr "Celkový čas CPU"
 
-#: panels/timer.py:44
+#: panels/timer.py:46
 #, python-format
 msgid "%(total)0.3f msec"
 msgstr "%(total)0.3f msec"
 
-#: panels/timer.py:45
+#: panels/timer.py:47
 msgid "Elapsed time"
 msgstr "Uplynulý čas"
 
-#: panels/timer.py:45
+#: panels/timer.py:47
 #, python-format
 msgid "%(total_time)0.3f msec"
 msgstr "%(total_time)0.3f msec"
 
-#: panels/timer.py:46
+#: panels/timer.py:49
 msgid "Context switches"
 msgstr "Přepnutí kontextu"
 
-#: panels/timer.py:46
+#: panels/timer.py:50
 #, python-format
 msgid "%(vcsw)d voluntary, %(ivcsw)d involuntary"
 msgstr "%(vcsw)d dobrovolně, %(ivcsw)d nedobrovolně"
 
-#: panels/versions.py:25
+#: panels/versions.py:19
 msgid "Versions"
 msgstr "Verze"
 
-#: panels/sql/panel.py:22
-msgid "Autocommit"
-msgstr "Autocommit"
-
-#: panels/sql/panel.py:23
-msgid "Read uncommitted"
-msgstr "Read uncommitted"
-
-#: panels/sql/panel.py:24
-msgid "Read committed"
-msgstr "Read committed"
-
-#: panels/sql/panel.py:25
-msgid "Repeatable read"
-msgstr "Repeatable read"
-
-#: panels/sql/panel.py:26
-msgid "Serializable"
-msgstr "Serializable"
-
-#: panels/sql/panel.py:37
-msgid "Idle"
-msgstr "V klidu (idle)"
-
-#: panels/sql/panel.py:38
-msgid "Active"
-msgstr "Aktivní"
-
-#: panels/sql/panel.py:39
-msgid "In transaction"
-msgstr "Uvnitř transakce"
-
-#: panels/sql/panel.py:40
-msgid "In error"
-msgstr "V chybovém stavu"
-
-#: panels/sql/panel.py:41
-msgid "Unknown"
-msgstr "Neznámé"
-
-#: panels/sql/panel.py:105
-msgid "SQL"
-msgstr "SQL"
-
-#: panels/templates/panel.py:141
-msgid "Templates"
-msgstr "Šablony"
-
-#: panels/templates/panel.py:146
-#, python-format
-msgid "Templates (%(num_templates)s rendered)"
-msgstr "Šablony (renderovaných: %(num_templates)s)"
-
-#: templates/debug_toolbar/base.html:19
+#: templates/debug_toolbar/base.html:22
 msgid "Hide toolbar"
 msgstr "Skrýt lištu"
 
-#: templates/debug_toolbar/base.html:19
+#: templates/debug_toolbar/base.html:22
 msgid "Hide"
 msgstr "Skrýt"
 
-#: templates/debug_toolbar/base.html:25
+#: templates/debug_toolbar/base.html:29
+msgid "Show toolbar"
+msgstr "Zobrazit lištu"
+
+#: templates/debug_toolbar/includes/panel_button.html:4
 msgid "Disable for next and successive requests"
 msgstr "Vypnout pro následné požadavky"
 
-#: templates/debug_toolbar/base.html:25
+#: templates/debug_toolbar/includes/panel_button.html:4
 msgid "Enable for next and successive requests"
 msgstr "Zapnout pro následné požadavky"
 
-#: templates/debug_toolbar/base.html:47
-msgid "Show toolbar"
-msgstr "Zobrazit lištu"
-
-#: templates/debug_toolbar/base.html:53
-msgid "Close"
-msgstr "Zavřít"
-
-#: templates/debug_toolbar/redirect.html:8
-msgid "Location:"
-msgstr "Adresa:"
-
-#: templates/debug_toolbar/redirect.html:10
-msgid ""
-"The Django Debug Toolbar has intercepted a redirect to the above URL for "
-"debug viewing purposes. You can click the above link to continue with the "
-"redirect as normal."
-msgstr "Aplikace Django Debug Toolbar zachytila přesměrování na výše uvedenou adresu URL za účelem ladicího zobrazení. Chcete-li přesměrování dokončit, klepněte na odkaz výše."
-
 #: templates/debug_toolbar/panels/cache.html:2
 msgid "Summary"
 msgstr "Souhrn"
 
 #: templates/debug_toolbar/panels/cache.html:6
 msgid "Total calls"
 msgstr "Celkem volání"
@@ -313,15 +304,15 @@
 msgstr "Příkazy"
 
 #: templates/debug_toolbar/panels/cache.html:39
 msgid "Calls"
 msgstr "Volání"
 
 #: templates/debug_toolbar/panels/cache.html:43
-#: templates/debug_toolbar/panels/sql.html:20
+#: templates/debug_toolbar/panels/sql.html:36
 msgid "Time (ms)"
 msgstr "Čas (ms)"
 
 #: templates/debug_toolbar/panels/cache.html:44
 msgid "Type"
 msgstr "Typ"
 
@@ -348,18 +339,16 @@
 #: templates/debug_toolbar/panels/headers.html:48
 msgid "Key"
 msgstr "Klíč"
 
 #: templates/debug_toolbar/panels/headers.html:9
 #: templates/debug_toolbar/panels/headers.html:28
 #: templates/debug_toolbar/panels/headers.html:49
-#: templates/debug_toolbar/panels/request.html:33
-#: templates/debug_toolbar/panels/request.html:59
-#: templates/debug_toolbar/panels/request.html:85
-#: templates/debug_toolbar/panels/request.html:110
+#: templates/debug_toolbar/panels/history_tr.html:23
+#: templates/debug_toolbar/panels/request_variables.html:12
 #: templates/debug_toolbar/panels/settings.html:6
 #: templates/debug_toolbar/panels/timer.html:11
 msgid "Value"
 msgstr "Hodnota"
 
 #: templates/debug_toolbar/panels/headers.html:22
 msgid "Response headers"
@@ -369,36 +358,46 @@
 msgid "WSGI environ"
 msgstr "Prostředí WSGI"
 
 #: templates/debug_toolbar/panels/headers.html:43
 msgid ""
 "Since the WSGI environ inherits the environment of the server, only a "
 "significant subset is shown below."
-msgstr "Níže je zobrazena pouze podstatná část proměnných prostředí, protože WSGI je dědí od serveru."
+msgstr ""
+"Níže je zobrazena pouze podstatná část proměnných prostředí, protože WSGI je "
+"dědí od serveru."
 
-#: templates/debug_toolbar/panels/logging.html:6
-msgid "Level"
-msgstr "Úroveň"
-
-#: templates/debug_toolbar/panels/logging.html:8
-msgid "Channel"
-msgstr "Kanál"
-
-#: templates/debug_toolbar/panels/logging.html:9
-msgid "Message"
-msgstr "Zpráva"
+#: templates/debug_toolbar/panels/history.html:10
+msgid "Method"
+msgstr ""
 
-#: templates/debug_toolbar/panels/logging.html:10
-#: templates/debug_toolbar/panels/staticfiles.html:45
-msgid "Location"
-msgstr "Adresa"
+#: templates/debug_toolbar/panels/history.html:11
+#: templates/debug_toolbar/panels/staticfiles.html:43
+msgid "Path"
+msgstr "Cesta"
 
-#: templates/debug_toolbar/panels/logging.html:26
-msgid "No messages logged"
-msgstr "Nebyly protokolovány žádné zprávy."
+#: templates/debug_toolbar/panels/history.html:12
+#, fuzzy
+#| msgid "Request headers"
+msgid "Request Variables"
+msgstr "Záhlaví požadavku"
+
+#: templates/debug_toolbar/panels/history.html:13
+msgid "Status"
+msgstr ""
+
+#: templates/debug_toolbar/panels/history.html:14
+#: templates/debug_toolbar/panels/sql.html:37
+msgid "Action"
+msgstr "Akce"
+
+#: templates/debug_toolbar/panels/history_tr.html:22
+#: templates/debug_toolbar/panels/request_variables.html:11
+msgid "Variable"
+msgstr "Proměnná"
 
 #: templates/debug_toolbar/panels/profiling.html:5
 msgid "Call"
 msgstr "Volání"
 
 #: templates/debug_toolbar/panels/profiling.html:6
 msgid "CumTime"
@@ -429,113 +428,117 @@
 msgid "URL name"
 msgstr "Název URL"
 
 #: templates/debug_toolbar/panels/request.html:24
 msgid "Cookies"
 msgstr "Soubory cookie"
 
-#: templates/debug_toolbar/panels/request.html:32
-#: templates/debug_toolbar/panels/request.html:58
-#: templates/debug_toolbar/panels/request.html:84
-#: templates/debug_toolbar/panels/request.html:109
-msgid "Variable"
-msgstr "Proměnná"
-
-#: templates/debug_toolbar/panels/request.html:46
+#: templates/debug_toolbar/panels/request.html:27
 msgid "No cookies"
 msgstr "Žádné soubory cookie"
 
-#: templates/debug_toolbar/panels/request.html:50
+#: templates/debug_toolbar/panels/request.html:31
 msgid "Session data"
 msgstr "Data sezení"
 
-#: templates/debug_toolbar/panels/request.html:72
+#: templates/debug_toolbar/panels/request.html:34
 msgid "No session data"
 msgstr "Žádná data sezení"
 
-#: templates/debug_toolbar/panels/request.html:76
+#: templates/debug_toolbar/panels/request.html:38
 msgid "GET data"
 msgstr "Data typu GET"
 
-#: templates/debug_toolbar/panels/request.html:98
+#: templates/debug_toolbar/panels/request.html:41
 msgid "No GET data"
 msgstr "Žádná data typu GET"
 
-#: templates/debug_toolbar/panels/request.html:102
+#: templates/debug_toolbar/panels/request.html:45
 msgid "POST data"
 msgstr "Data typu POST"
 
-#: templates/debug_toolbar/panels/request.html:123
+#: templates/debug_toolbar/panels/request.html:48
 msgid "No POST data"
 msgstr "Žádná data typu POST"
 
 #: templates/debug_toolbar/panels/settings.html:5
 msgid "Setting"
 msgstr "Nastavení"
 
 #: templates/debug_toolbar/panels/signals.html:5
 msgid "Signal"
 msgstr "Signál"
 
 #: templates/debug_toolbar/panels/signals.html:6
-msgid "Providing"
-msgstr "Poskytuje"
-
-#: templates/debug_toolbar/panels/signals.html:7
 msgid "Receivers"
 msgstr "Příjemci"
 
-#: templates/debug_toolbar/panels/sql.html:7
+#: templates/debug_toolbar/panels/sql.html:6
 #, python-format
 msgid "%(num)s query"
 msgid_plural "%(num)s queries"
 msgstr[0] "%(num)s dotaz"
 msgstr[1] "%(num)s dotazy"
 msgstr[2] "%(num)s dotazů"
 
-#: templates/debug_toolbar/panels/sql.html:18
+#: templates/debug_toolbar/panels/sql.html:8
+#, python-format
+msgid ""
+"including <abbr title=\"Similar queries are queries with the same SQL, but "
+"potentially different parameters.\">%(count)s similar</abbr>"
+msgstr ""
+
+#: templates/debug_toolbar/panels/sql.html:12
+#, python-format
+msgid ""
+"and <abbr title=\"Duplicate queries are identical to each other: they "
+"execute exactly the same SQL and parameters.\">%(dupes)s duplicates</abbr>"
+msgstr ""
+
+#: templates/debug_toolbar/panels/sql.html:34
 msgid "Query"
 msgstr "Dotaz"
 
-#: templates/debug_toolbar/panels/sql.html:19
+#: templates/debug_toolbar/panels/sql.html:35
 #: templates/debug_toolbar/panels/timer.html:36
 msgid "Timeline"
 msgstr "Časová osa"
 
-#: templates/debug_toolbar/panels/sql.html:21
-msgid "Action"
-msgstr "Akce"
+#: templates/debug_toolbar/panels/sql.html:52
+#, fuzzy, python-format
+#| msgid "%(count)s message"
+#| msgid_plural "%(count)s messages"
+msgid "%(count)s similar queries."
+msgstr "%(count)s zpráva"
+
+#: templates/debug_toolbar/panels/sql.html:58
+#, python-format
+msgid "Duplicated %(dupes)s times."
+msgstr ""
 
-#: templates/debug_toolbar/panels/sql.html:64
+#: templates/debug_toolbar/panels/sql.html:95
 msgid "Connection:"
 msgstr "Spojení:"
 
-#: templates/debug_toolbar/panels/sql.html:66
+#: templates/debug_toolbar/panels/sql.html:97
 msgid "Isolation level:"
 msgstr "Úroveň izolace:"
 
-#: templates/debug_toolbar/panels/sql.html:69
+#: templates/debug_toolbar/panels/sql.html:100
 msgid "Transaction status:"
 msgstr "Stav transakce:"
 
-#: templates/debug_toolbar/panels/sql.html:83
+#: templates/debug_toolbar/panels/sql.html:114
 msgid "(unknown)"
 msgstr "(neznámé)"
 
-#: templates/debug_toolbar/panels/sql.html:92
+#: templates/debug_toolbar/panels/sql.html:123
 msgid "No SQL queries were recorded during this request."
 msgstr "Pro tento požadavek nebyl zaznamenán žádný dotaz SQL."
 
-#: templates/debug_toolbar/panels/sql_explain.html:3
-#: templates/debug_toolbar/panels/sql_profile.html:3
-#: templates/debug_toolbar/panels/sql_select.html:3
-#: templates/debug_toolbar/panels/template_source.html:3
-msgid "Back"
-msgstr "Zpět"
-
 #: templates/debug_toolbar/panels/sql_explain.html:4
 msgid "SQL explained"
 msgstr "Vysvětlené SQL"
 
 #: templates/debug_toolbar/panels/sql_explain.html:9
 #: templates/debug_toolbar/panels/sql_profile.html:10
 #: templates/debug_toolbar/panels/sql_select.html:9
@@ -560,60 +563,60 @@
 msgid "SQL selected"
 msgstr "Vybrané SQL"
 
 #: templates/debug_toolbar/panels/sql_select.html:36
 msgid "Empty set"
 msgstr "Prázdná sada"
 
-#: templates/debug_toolbar/panels/staticfiles.html:4
+#: templates/debug_toolbar/panels/staticfiles.html:3
 msgid "Static file path"
 msgid_plural "Static file paths"
 msgstr[0] "Cesta ke statickým souborům"
 msgstr[1] "Cesty ke statickým souborům"
 msgstr[2] "Cesty ke statickým souborům"
 
-#: templates/debug_toolbar/panels/staticfiles.html:8
+#: templates/debug_toolbar/panels/staticfiles.html:7
 #, python-format
 msgid "(prefix %(prefix)s)"
 msgstr "(prefix %(prefix)s)"
 
-#: templates/debug_toolbar/panels/staticfiles.html:12
-#: templates/debug_toolbar/panels/staticfiles.html:23
-#: templates/debug_toolbar/panels/staticfiles.html:35
+#: templates/debug_toolbar/panels/staticfiles.html:11
+#: templates/debug_toolbar/panels/staticfiles.html:22
+#: templates/debug_toolbar/panels/staticfiles.html:34
 #: templates/debug_toolbar/panels/templates.html:10
-#: templates/debug_toolbar/panels/templates.html:28
-#: templates/debug_toolbar/panels/templates.html:43
+#: templates/debug_toolbar/panels/templates.html:30
+#: templates/debug_toolbar/panels/templates.html:47
 msgid "None"
 msgstr "Žádné"
 
-#: templates/debug_toolbar/panels/staticfiles.html:15
+#: templates/debug_toolbar/panels/staticfiles.html:14
 msgid "Static file app"
 msgid_plural "Static file apps"
 msgstr[0] "Aplikace se statickými soubory"
 msgstr[1] "Aplikace se statickými soubory"
 msgstr[2] "Aplikace se statickými soubory"
 
-#: templates/debug_toolbar/panels/staticfiles.html:26
+#: templates/debug_toolbar/panels/staticfiles.html:25
 msgid "Static file"
 msgid_plural "Static files"
 msgstr[0] "Statický soubor"
 msgstr[1] "Statické soubory"
 msgstr[2] "Statické soubory"
 
-#: templates/debug_toolbar/panels/staticfiles.html:40
+#: templates/debug_toolbar/panels/staticfiles.html:39
 #, python-format
 msgid "%(payload_count)s file"
 msgid_plural "%(payload_count)s files"
 msgstr[0] "%(payload_count)s soubor"
 msgstr[1] "%(payload_count)s soubory"
 msgstr[2] "%(payload_count)s souborů"
 
 #: templates/debug_toolbar/panels/staticfiles.html:44
-msgid "Path"
-msgstr "Cesta"
+msgid "Location"
+msgstr "Adresa"
 
 #: templates/debug_toolbar/panels/template_source.html:4
 msgid "Template source:"
 msgstr "Zdroj šablony:"
 
 #: templates/debug_toolbar/panels/templates.html:2
 msgid "Template path"
@@ -625,20 +628,20 @@
 #: templates/debug_toolbar/panels/templates.html:13
 msgid "Template"
 msgid_plural "Templates"
 msgstr[0] "Šablona"
 msgstr[1] "Šablony"
 msgstr[2] "Šablony"
 
-#: templates/debug_toolbar/panels/templates.html:21
-#: templates/debug_toolbar/panels/templates.html:37
+#: templates/debug_toolbar/panels/templates.html:22
+#: templates/debug_toolbar/panels/templates.html:40
 msgid "Toggle context"
 msgstr "Zap./vyp. kontext"
 
-#: templates/debug_toolbar/panels/templates.html:31
+#: templates/debug_toolbar/panels/templates.html:33
 msgid "Context processor"
 msgid_plural "Context processors"
 msgstr[0] "Procesor kontextu"
 msgstr[1] "Procesory kontextu"
 msgstr[2] "Procesory kontextu"
 
 #: templates/debug_toolbar/panels/timer.html:2
@@ -657,14 +660,40 @@
 msgid "Timing attribute"
 msgstr "Atribut"
 
 #: templates/debug_toolbar/panels/timer.html:37
 msgid "Milliseconds since navigation start (+length)"
 msgstr "Milisekund od začátku navigace (+délka)"
 
-#: templates/debug_toolbar/panels/versions.html:5
+#: templates/debug_toolbar/panels/versions.html:10
+msgid "Package"
+msgstr ""
+
+#: templates/debug_toolbar/panels/versions.html:11
 msgid "Name"
 msgstr "Název"
 
-#: templates/debug_toolbar/panels/versions.html:6
+#: templates/debug_toolbar/panels/versions.html:12
 msgid "Version"
 msgstr "Verze"
+
+#: templates/debug_toolbar/redirect.html:10
+msgid "Location:"
+msgstr "Adresa:"
+
+#: templates/debug_toolbar/redirect.html:12
+msgid ""
+"The Django Debug Toolbar has intercepted a redirect to the above URL for "
+"debug viewing purposes. You can click the above link to continue with the "
+"redirect as normal."
+msgstr ""
+"Aplikace Django Debug Toolbar zachytila přesměrování na výše uvedenou adresu "
+"URL za účelem ladicího zobrazení. Chcete-li přesměrování dokončit, klepněte "
+"na odkaz výše."
+
+#: views.py:16
+msgid ""
+"Data for this panel isn't available anymore. Please reload the page and "
+"retry."
+msgstr ""
+"Data pro tento panel již nejsou k dispozici. Obnovte stránku a zkuste to "
+"znova."
```

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/locale/de/LC_MESSAGES/django.mo` & `django_debug_toolbar-4.0.0/debug_toolbar/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/locale/de/LC_MESSAGES/django.po` & `django_debug_toolbar-4.0.0/debug_toolbar/locale/fr/LC_MESSAGES/django.po`

 * *Files 4% similar despite different names*

```diff
@@ -1,703 +1,688 @@
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 #
 #
 # Translators:
-# Jannis Leidel <jannis@leidel.info>, 2012-2014,2021
-# Matthias Kestenholz <mk@feinheit.ch>, 2021
+# Anthony Jorion <pingax@gmail.com>, 2013
+# Aymeric Augustin <aymeric.augustin@m4x.org>, 2014
+# Claude Paroz <claude@2xlibre.net>, 2013
+# Colin O'Brien <colin@things.be>, 2021
+# David Paccoud, 2009
+# Dominick Rivard <dominick.rivard@gmail.com>, 2013
+# Maxime Abry <maxime.abry@critizr.com>, 2016
 msgid ""
 msgstr ""
 "Project-Id-Version: Django Debug Toolbar\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-08-14 10:25-0500\n"
-"PO-Revision-Date: 2021-12-04 17:38+0000\n"
-"Last-Translator: Tim Schilling\n"
-"Language-Team: German (http://www.transifex.com/django-debug-toolbar/django-debug-toolbar/language/de/)\n"
+"POT-Creation-Date: 2023-01-20 17:23+0100\n"
+"PO-Revision-Date: 2021-09-30 09:21+0000\n"
+"Last-Translator: Colin O'Brien <colin@things.be>\n"
+"Language-Team: French (http://www.transifex.com/django-debug-toolbar/django-"
+"debug-toolbar/language/fr/)\n"
+"Language: fr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: de\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
 #: apps.py:15
 msgid "Debug Toolbar"
-msgstr "Debug Toolbar"
+msgstr "Barre d'outils de débogage"
 
-#: panels/cache.py:227
+#: panels/cache.py:180
 msgid "Cache"
 msgstr "Cache"
 
-#: panels/cache.py:234
+#: panels/cache.py:186
 #, python-format
 msgid "%(cache_calls)d call in %(time).2fms"
 msgid_plural "%(cache_calls)d calls in %(time).2fms"
-msgstr[0] "%(cache_calls)d Abfrage in %(time).2fms"
-msgstr[1] "%(cache_calls)d Abfragen in %(time).2fms"
+msgstr[0] "%(cache_calls)d appel en %(time).2fms"
+msgstr[1] "%(cache_calls)d appels en %(time).2fms"
 
-#: panels/cache.py:246
+#: panels/cache.py:195
 #, python-format
 msgid "Cache calls from %(count)d backend"
 msgid_plural "Cache calls from %(count)d backends"
-msgstr[0] "Cache-Aufrufe von %(count)d Backend"
-msgstr[1] "Cache-Aufrufe von %(count)d Backends"
+msgstr[0] "Appels au cache depuis %(count)d moteur"
+msgstr[1] "Appels au cache depuis %(count)d moteurs"
 
-#: panels/headers.py:33
+#: panels/headers.py:31
 msgid "Headers"
-msgstr "Header"
+msgstr "En-têtes"
 
-#: panels/history/panel.py:20 panels/history/panel.py:21
+#: panels/history/panel.py:18 panels/history/panel.py:19
 msgid "History"
-msgstr "Geschichte"
+msgstr "Historique"
 
-#: panels/logging.py:63
-msgid "Logging"
-msgstr "Logging"
-
-#: panels/logging.py:69
-#, python-format
-msgid "%(count)s message"
-msgid_plural "%(count)s messages"
-msgstr[0] "%(count)s Eintrag"
-msgstr[1] "%(count)s Einträge"
-
-#: panels/logging.py:73
-msgid "Log messages"
-msgstr "Logeinträge"
-
-#: panels/profiling.py:150
+#: panels/profiling.py:140
 msgid "Profiling"
-msgstr "Profiling"
+msgstr "Profilage"
 
 #: panels/redirects.py:14
 msgid "Intercept redirects"
-msgstr "Umleitungen abfangen"
+msgstr "Interception des redirections"
 
 #: panels/request.py:16
 msgid "Request"
-msgstr "Anfrage"
+msgstr "Requête"
 
 #: panels/request.py:36
 msgid "<no view>"
-msgstr "<kein View>"
+msgstr "<pas de vue>"
 
 #: panels/request.py:53
 msgid "<unavailable>"
-msgstr "<nicht verfügbar>"
+msgstr "<indisponible>"
 
-#: panels/settings.py:24
+#: panels/settings.py:17
 msgid "Settings"
-msgstr "Einstellungen"
+msgstr "Paramètres"
 
-#: panels/settings.py:27
+#: panels/settings.py:20
 #, python-format
 msgid "Settings from %s"
-msgstr "Einstellungen von %s"
+msgstr "Paramètres de %s"
 
-#: panels/signals.py:58
+#: panels/signals.py:57
 #, python-format
 msgid "%(num_receivers)d receiver of 1 signal"
 msgid_plural "%(num_receivers)d receivers of 1 signal"
-msgstr[0] "%(num_receivers)d Empfänger von einem Signal"
-msgstr[1] "%(num_receivers)d Empfänger von einem Signal"
+msgstr[0] "%(num_receivers)d receveur d'un signal"
+msgstr[1] "%(num_receivers)d receveurs d'un signal"
 
-#: panels/signals.py:66
+#: panels/signals.py:62
 #, python-format
 msgid "%(num_receivers)d receiver of %(num_signals)d signals"
 msgid_plural "%(num_receivers)d receivers of %(num_signals)d signals"
-msgstr[0] "%(num_receivers)d Empfänger von %(num_signals)d Signalen"
-msgstr[1] "%(num_receivers)d Empfänger von %(num_signals)d Signalen"
+msgstr[0] "%(num_receivers)d receveur de %(num_signals)d signaux"
+msgstr[1] "%(num_receivers)d receveurs de %(num_signals)d signaux"
 
-#: panels/signals.py:73
+#: panels/signals.py:67
 msgid "Signals"
-msgstr "Signale"
+msgstr "Signaux"
 
-#: panels/sql/panel.py:24
+#: panels/sql/panel.py:23
 msgid "Autocommit"
-msgstr "Autocommit"
+msgstr "Auto validation"
 
-#: panels/sql/panel.py:25
+#: panels/sql/panel.py:24
 msgid "Read uncommitted"
-msgstr "Read uncommitted"
+msgstr "Lecture non validée"
 
-#: panels/sql/panel.py:26
+#: panels/sql/panel.py:25
 msgid "Read committed"
-msgstr "Read committed"
+msgstr "Lecture validée"
 
-#: panels/sql/panel.py:27
+#: panels/sql/panel.py:26
 msgid "Repeatable read"
-msgstr "Repeatable read"
+msgstr "Lecture répétable"
 
-#: panels/sql/panel.py:28
+#: panels/sql/panel.py:27
 msgid "Serializable"
-msgstr "Serializable"
+msgstr "Sérialisable"
 
-#: panels/sql/panel.py:40
+#: panels/sql/panel.py:39
 msgid "Idle"
-msgstr "Wartet"
+msgstr "Inactif"
 
-#: panels/sql/panel.py:41
+#: panels/sql/panel.py:40
 msgid "Active"
-msgstr "Aktiv"
+msgstr "Actif"
 
-#: panels/sql/panel.py:42
+#: panels/sql/panel.py:41
 msgid "In transaction"
-msgstr "In einer Transaktion"
+msgstr "Transaction en cours"
 
-#: panels/sql/panel.py:43
+#: panels/sql/panel.py:42
 msgid "In error"
-msgstr "Fehler"
+msgstr "Erreur"
 
-#: panels/sql/panel.py:44
+#: panels/sql/panel.py:43
 msgid "Unknown"
-msgstr "Unbekannt"
+msgstr "Indéterminé"
 
-#: panels/sql/panel.py:109
+#: panels/sql/panel.py:130
 msgid "SQL"
 msgstr "SQL"
 
-#: panels/sql/panel.py:114
+#: panels/sql/panel.py:135
 #, python-format
 msgid "%(query_count)d query in %(sql_time).2fms"
 msgid_plural "%(query_count)d queries in %(sql_time).2fms"
-msgstr[0] "%(query_count)d Abfrage in %(sql_time).2f ms"
-msgstr[1] "%(query_count)d Abfragen in %(sql_time).2f ms"
+msgstr[0] "%(query_count)d requête en %(sql_time).2f ms"
+msgstr[1] "%(query_count)d requêtes en %(sql_time).2f ms"
 
-#: panels/sql/panel.py:127
+#: panels/sql/panel.py:147
 #, python-format
 msgid "SQL queries from %(count)d connection"
 msgid_plural "SQL queries from %(count)d connections"
-msgstr[0] "SQL-Abfragen von %(count)d Verbindung"
-msgstr[1] "SQL-Abfragen von %(count)d Verbindungen"
+msgstr[0] "requêtes SQL venant de %(count)d connexion"
+msgstr[1] "Requêtes SQL venant de %(count)d connexions"
 
-#: panels/staticfiles.py:85
+#: panels/staticfiles.py:84
 #, python-format
 msgid "Static files (%(num_found)s found, %(num_used)s used)"
-msgstr "Statische Dateien (%(num_found)s gefunden, %(num_used)s benutzt)"
+msgstr "Fichiers statiques (%(num_found)s trouvé(s), %(num_used)s utilisé(s))"
 
-#: panels/staticfiles.py:106
+#: panels/staticfiles.py:105
 msgid "Static files"
-msgstr "Statische Dateien"
+msgstr "Fichiers statiques"
 
-#: panels/staticfiles.py:112
+#: panels/staticfiles.py:111
 #, python-format
 msgid "%(num_used)s file used"
 msgid_plural "%(num_used)s files used"
-msgstr[0] "%(num_used)s Datei benutzt"
-msgstr[1] "%(num_used)s Dateien benutzt"
+msgstr[0] "%(num_used)s fichier utilisé"
+msgstr[1] "%(num_used)s fichiers utilisés"
 
-#: panels/templates/panel.py:144
+#: panels/templates/panel.py:143
 msgid "Templates"
-msgstr "Templates"
+msgstr "Gabarits"
 
-#: panels/templates/panel.py:149
+#: panels/templates/panel.py:148
 #, python-format
 msgid "Templates (%(num_templates)s rendered)"
-msgstr "Templates (%(num_templates)s gerendert)"
+msgstr "Gabarits (%(num_templates)s affichés)"
 
-#: panels/templates/panel.py:181
+#: panels/templates/panel.py:180
 msgid "No origin"
-msgstr "Kein Ursprung"
+msgstr "Sans Origine"
 
 #: panels/timer.py:25
 #, python-format
 msgid "CPU: %(cum)0.2fms (%(total)0.2fms)"
 msgstr "CPU: %(cum)0.2fms (%(total)0.2fms)"
 
 #: panels/timer.py:30
 #, python-format
 msgid "Total: %0.2fms"
-msgstr "Gesamt: %0.2fms"
+msgstr "Total : %0.2fms"
 
 #: panels/timer.py:36 templates/debug_toolbar/panels/history.html:9
-#: templates/debug_toolbar/panels/logging.html:7
 #: templates/debug_toolbar/panels/sql_explain.html:11
 #: templates/debug_toolbar/panels/sql_profile.html:12
 #: templates/debug_toolbar/panels/sql_select.html:11
 msgid "Time"
-msgstr "Zeit"
+msgstr "Temps"
 
 #: panels/timer.py:44
 msgid "User CPU time"
-msgstr "CPU-Zeit Benutzer"
+msgstr "Temps CPU de l'utilisateur"
 
 #: panels/timer.py:44
 #, python-format
 msgid "%(utime)0.3f msec"
 msgstr "%(utime)0.3f ms"
 
 #: panels/timer.py:45
 msgid "System CPU time"
-msgstr "CPU-Zeit System"
+msgstr "Temps CPU du système"
 
 #: panels/timer.py:45
 #, python-format
 msgid "%(stime)0.3f msec"
 msgstr "%(stime)0.3f ms"
 
 #: panels/timer.py:46
 msgid "Total CPU time"
-msgstr "CPU-Zeit gesamt"
+msgstr "Temps total du CPU"
 
 #: panels/timer.py:46
 #, python-format
 msgid "%(total)0.3f msec"
 msgstr "%(total)0.3f ms"
 
 #: panels/timer.py:47
 msgid "Elapsed time"
-msgstr "Verstrichene Zeit"
+msgstr "Temps écoulé"
 
 #: panels/timer.py:47
 #, python-format
 msgid "%(total_time)0.3f msec"
 msgstr "%(total_time)0.3f ms"
 
 #: panels/timer.py:49
 msgid "Context switches"
-msgstr "Kontextwechsel"
+msgstr "Basculements de contexte"
 
 #: panels/timer.py:50
 #, python-format
 msgid "%(vcsw)d voluntary, %(ivcsw)d involuntary"
-msgstr "%(vcsw)d freiwillig, %(ivcsw)d unfreiwillig"
+msgstr "%(vcsw)d volontaire, %(ivcsw)d involontaire"
 
 #: panels/versions.py:19
 msgid "Versions"
-msgstr "Versionen"
+msgstr "Versions"
 
-#: templates/debug_toolbar/base.html:18
+#: templates/debug_toolbar/base.html:22
 msgid "Hide toolbar"
-msgstr "Toolbar ausblenden"
+msgstr "Masquer la barre d'outils"
 
-#: templates/debug_toolbar/base.html:18
+#: templates/debug_toolbar/base.html:22
 msgid "Hide"
-msgstr "Ausblenden"
+msgstr "Masquer"
 
-#: templates/debug_toolbar/base.html:25
+#: templates/debug_toolbar/base.html:29
 msgid "Show toolbar"
-msgstr "Toolbar einblenden"
+msgstr "Afficher la barre d'outils"
 
 #: templates/debug_toolbar/includes/panel_button.html:4
 msgid "Disable for next and successive requests"
-msgstr "Für nächste und die darauffolgenden Anfragen deaktivieren"
+msgstr "Désactiver pour les requêtes suivantes"
 
 #: templates/debug_toolbar/includes/panel_button.html:4
 msgid "Enable for next and successive requests"
-msgstr "Für nächste und die darauffolgenden Anfragen aktivieren"
+msgstr "Activer pour les requêtes suivantes"
 
 #: templates/debug_toolbar/panels/cache.html:2
 msgid "Summary"
-msgstr "Zusammenfassung"
+msgstr "Résumé"
 
 #: templates/debug_toolbar/panels/cache.html:6
 msgid "Total calls"
-msgstr "Aufrufe gesamt"
+msgstr "Nombre total d'appels"
 
 #: templates/debug_toolbar/panels/cache.html:7
 msgid "Total time"
-msgstr "Zeit gesamt"
+msgstr "Temps total"
 
 #: templates/debug_toolbar/panels/cache.html:8
 msgid "Cache hits"
-msgstr "Cache erfolgreich"
+msgstr "Succès de cache"
 
 #: templates/debug_toolbar/panels/cache.html:9
 msgid "Cache misses"
-msgstr "Cache verfehlt"
+msgstr "Défauts de cache"
 
 #: templates/debug_toolbar/panels/cache.html:21
 msgid "Commands"
-msgstr "Befehle"
+msgstr "Commandes"
 
 #: templates/debug_toolbar/panels/cache.html:39
 msgid "Calls"
-msgstr "Aufrufe"
+msgstr "Appels"
 
 #: templates/debug_toolbar/panels/cache.html:43
 #: templates/debug_toolbar/panels/sql.html:36
 msgid "Time (ms)"
-msgstr "Zeit (ms)"
+msgstr "Temps (ms)"
 
 #: templates/debug_toolbar/panels/cache.html:44
 msgid "Type"
-msgstr "Typ"
+msgstr "Type"
 
 #: templates/debug_toolbar/panels/cache.html:45
 #: templates/debug_toolbar/panels/request.html:8
 msgid "Arguments"
-msgstr "Argumente"
+msgstr "Paramètres"
 
 #: templates/debug_toolbar/panels/cache.html:46
 #: templates/debug_toolbar/panels/request.html:9
 msgid "Keyword arguments"
-msgstr "Schlüsselwort-Argumente"
+msgstr "Paramètres nommés"
 
 #: templates/debug_toolbar/panels/cache.html:47
 msgid "Backend"
-msgstr "Backend"
+msgstr "Moteur"
 
 #: templates/debug_toolbar/panels/headers.html:3
 msgid "Request headers"
-msgstr "Anfrage-Header"
+msgstr "En-têtes de requête"
 
 #: templates/debug_toolbar/panels/headers.html:8
 #: templates/debug_toolbar/panels/headers.html:27
 #: templates/debug_toolbar/panels/headers.html:48
 msgid "Key"
-msgstr "Schlüssel"
+msgstr "Clé"
 
 #: templates/debug_toolbar/panels/headers.html:9
 #: templates/debug_toolbar/panels/headers.html:28
 #: templates/debug_toolbar/panels/headers.html:49
 #: templates/debug_toolbar/panels/history_tr.html:23
-#: templates/debug_toolbar/panels/request_variables.html:11
+#: templates/debug_toolbar/panels/request_variables.html:12
 #: templates/debug_toolbar/panels/settings.html:6
 #: templates/debug_toolbar/panels/timer.html:11
 msgid "Value"
-msgstr "Wert"
+msgstr "Valeur"
 
 #: templates/debug_toolbar/panels/headers.html:22
 msgid "Response headers"
-msgstr "Antwort-Header"
+msgstr "En-têtes de réponse"
 
 #: templates/debug_toolbar/panels/headers.html:41
 msgid "WSGI environ"
-msgstr "WSGI-Umgebung"
+msgstr "Environnement WSGI"
 
 #: templates/debug_toolbar/panels/headers.html:43
 msgid ""
 "Since the WSGI environ inherits the environment of the server, only a "
 "significant subset is shown below."
-msgstr "Da sich die WSGI-Umgebung von der Umgebung des Servers ableitet, wird nur eine notwendige Teilmenge dargestellt."
+msgstr ""
+"Comme l'environnement WSGI hérite de celui du serveur, seul un sous-ensemble "
+"pertinent est affiché ci-dessous."
 
 #: templates/debug_toolbar/panels/history.html:10
 msgid "Method"
-msgstr "Methode"
+msgstr "Méthode"
 
 #: templates/debug_toolbar/panels/history.html:11
 #: templates/debug_toolbar/panels/staticfiles.html:43
 msgid "Path"
-msgstr "Pfad"
+msgstr "Chemin"
 
 #: templates/debug_toolbar/panels/history.html:12
 msgid "Request Variables"
-msgstr "Anfrage-Variablen"
+msgstr "Variables de Requête"
 
 #: templates/debug_toolbar/panels/history.html:13
 msgid "Status"
-msgstr "Status"
+msgstr "État"
 
 #: templates/debug_toolbar/panels/history.html:14
 #: templates/debug_toolbar/panels/sql.html:37
 msgid "Action"
-msgstr "Aktion"
+msgstr "Action"
 
 #: templates/debug_toolbar/panels/history_tr.html:22
-#: templates/debug_toolbar/panels/request_variables.html:10
+#: templates/debug_toolbar/panels/request_variables.html:11
 msgid "Variable"
 msgstr "Variable"
 
-#: templates/debug_toolbar/panels/logging.html:6
-msgid "Level"
-msgstr "Level"
-
-#: templates/debug_toolbar/panels/logging.html:8
-msgid "Channel"
-msgstr "Kanal"
-
-#: templates/debug_toolbar/panels/logging.html:9
-msgid "Message"
-msgstr "Eintrag"
-
-#: templates/debug_toolbar/panels/logging.html:10
-#: templates/debug_toolbar/panels/staticfiles.html:44
-msgid "Location"
-msgstr "Ort"
-
-#: templates/debug_toolbar/panels/logging.html:26
-msgid "No messages logged"
-msgstr "Keine Logbucheinträge vorhanden"
-
 #: templates/debug_toolbar/panels/profiling.html:5
 msgid "Call"
-msgstr "Aufruf"
+msgstr "Appel"
 
 #: templates/debug_toolbar/panels/profiling.html:6
 msgid "CumTime"
-msgstr "Gesamt"
+msgstr "Temps cumulé"
 
 #: templates/debug_toolbar/panels/profiling.html:7
 #: templates/debug_toolbar/panels/profiling.html:9
 msgid "Per"
-msgstr "Per"
+msgstr "Par"
 
 #: templates/debug_toolbar/panels/profiling.html:8
 msgid "TotTime"
-msgstr "Total"
+msgstr "Temps total"
 
 #: templates/debug_toolbar/panels/profiling.html:10
 msgid "Count"
-msgstr "Anzahl"
+msgstr "Compte"
 
 #: templates/debug_toolbar/panels/request.html:3
 msgid "View information"
-msgstr "View-Informationen"
+msgstr "Afficher l'information"
 
 #: templates/debug_toolbar/panels/request.html:7
 msgid "View function"
-msgstr "View-Funktion"
+msgstr "Fonction de vue"
 
 #: templates/debug_toolbar/panels/request.html:10
 msgid "URL name"
-msgstr "URL-Name"
+msgstr "Nom d'URL"
 
 #: templates/debug_toolbar/panels/request.html:24
 msgid "Cookies"
 msgstr "Cookies"
 
 #: templates/debug_toolbar/panels/request.html:27
 msgid "No cookies"
-msgstr "Keine Cookies"
+msgstr "Pas de cookies"
 
 #: templates/debug_toolbar/panels/request.html:31
 msgid "Session data"
-msgstr "Sitzungsdaten"
+msgstr "Données de session"
 
 #: templates/debug_toolbar/panels/request.html:34
 msgid "No session data"
-msgstr "Keine Sitzungsdaten"
+msgstr "Pas de données de session"
 
 #: templates/debug_toolbar/panels/request.html:38
 msgid "GET data"
-msgstr "GET-Daten"
+msgstr "Données GET"
 
 #: templates/debug_toolbar/panels/request.html:41
 msgid "No GET data"
-msgstr "Keine GET-Daten"
+msgstr "Aucune donnée GET"
 
 #: templates/debug_toolbar/panels/request.html:45
 msgid "POST data"
-msgstr "POST-Daten"
+msgstr "Données POST"
 
 #: templates/debug_toolbar/panels/request.html:48
 msgid "No POST data"
-msgstr "Keine POST-Daten"
+msgstr "Aucune donnée POST"
 
 #: templates/debug_toolbar/panels/settings.html:5
 msgid "Setting"
-msgstr "Einstellung"
+msgstr "Paramètre"
 
 #: templates/debug_toolbar/panels/signals.html:5
 msgid "Signal"
 msgstr "Signal"
 
 #: templates/debug_toolbar/panels/signals.html:6
 msgid "Receivers"
-msgstr "Empfänger"
+msgstr "Receveurs"
 
 #: templates/debug_toolbar/panels/sql.html:6
 #, python-format
 msgid "%(num)s query"
 msgid_plural "%(num)s queries"
-msgstr[0] "%(num)s Abfrage"
-msgstr[1] "%(num)s Abfragen"
+msgstr[0] "%(num)s requête"
+msgstr[1] "%(num)s requêtes"
 
 #: templates/debug_toolbar/panels/sql.html:8
 #, python-format
 msgid ""
 "including <abbr title=\"Similar queries are queries with the same SQL, but "
 "potentially different parameters.\">%(count)s similar</abbr>"
-msgstr "inklusive <abbr title=\"Similar queries are queries with the same SQL, but potentially different parameters.\">%(count)s ähnlich</abbr>"
+msgstr ""
+"comprenant <abbr title=\"Similar queries are queries with the same SQL, but "
+"potentially different parameters.\">%(count)s similaires</abbr>"
 
 #: templates/debug_toolbar/panels/sql.html:12
 #, python-format
 msgid ""
 "and <abbr title=\"Duplicate queries are identical to each other: they "
 "execute exactly the same SQL and parameters.\">%(dupes)s duplicates</abbr>"
-msgstr "und <abbr title=\"Duplicate queries are identical to each other: they execute exactly the same SQL and parameters.\">%(dupes)s dupliziert</abbr>"
+msgstr ""
+"et <abbr title=\"Duplicate queries are identical to each other: they execute "
+"exactly the same SQL and parameters.\">%(dupes)s en double</abbr>"
 
 #: templates/debug_toolbar/panels/sql.html:34
 msgid "Query"
-msgstr "Abfrage"
+msgstr "Requête"
 
 #: templates/debug_toolbar/panels/sql.html:35
 #: templates/debug_toolbar/panels/timer.html:36
 msgid "Timeline"
-msgstr "Verlauf"
+msgstr "Chronologie"
 
 #: templates/debug_toolbar/panels/sql.html:52
 #, python-format
 msgid "%(count)s similar queries."
-msgstr "%(count)s ähnliche Abfragen."
+msgstr "%(count)s requêtes similaires."
 
 #: templates/debug_toolbar/panels/sql.html:58
 #, python-format
 msgid "Duplicated %(dupes)s times."
-msgstr "%(dupes)s-mal dupliziert."
+msgstr "Dupliqué %(dupes)s fois."
 
 #: templates/debug_toolbar/panels/sql.html:95
 msgid "Connection:"
-msgstr "Verbindung:"
+msgstr "Connexion :"
 
 #: templates/debug_toolbar/panels/sql.html:97
 msgid "Isolation level:"
-msgstr "Isolationsebene:"
+msgstr "Niveau d'isolation :"
 
 #: templates/debug_toolbar/panels/sql.html:100
 msgid "Transaction status:"
-msgstr "Transaktionsstatus:"
+msgstr "État de la transaction :"
 
 #: templates/debug_toolbar/panels/sql.html:114
 msgid "(unknown)"
-msgstr "(unbekannt)"
+msgstr "(indéterminé)"
 
 #: templates/debug_toolbar/panels/sql.html:123
 msgid "No SQL queries were recorded during this request."
-msgstr "Es wurde keine SQL-Abfrage während dieses Vorgangs aufgezeichnet."
+msgstr "Aucune requête SQL n'a été enregistrée durant cette requête."
 
 #: templates/debug_toolbar/panels/sql_explain.html:4
 msgid "SQL explained"
-msgstr "SQL erklärt"
+msgstr "SQL expliqué"
 
 #: templates/debug_toolbar/panels/sql_explain.html:9
 #: templates/debug_toolbar/panels/sql_profile.html:10
 #: templates/debug_toolbar/panels/sql_select.html:9
 msgid "Executed SQL"
-msgstr "Ausgeführtes SQL"
+msgstr "SQL Exécuté"
 
 #: templates/debug_toolbar/panels/sql_explain.html:13
 #: templates/debug_toolbar/panels/sql_profile.html:14
 #: templates/debug_toolbar/panels/sql_select.html:13
 msgid "Database"
-msgstr "Datenbank"
+msgstr "Base de données"
 
 #: templates/debug_toolbar/panels/sql_profile.html:4
 msgid "SQL profiled"
-msgstr "SQL durchleuchtet"
+msgstr "SQL profilé"
 
 #: templates/debug_toolbar/panels/sql_profile.html:37
 msgid "Error"
-msgstr "Fehler"
+msgstr "Erreur"
 
 #: templates/debug_toolbar/panels/sql_select.html:4
 msgid "SQL selected"
-msgstr "SQL ausgewählt"
+msgstr "SQL sélectionné"
 
 #: templates/debug_toolbar/panels/sql_select.html:36
 msgid "Empty set"
-msgstr "Leeres Set"
+msgstr "Ensemble vide"
 
 #: templates/debug_toolbar/panels/staticfiles.html:3
 msgid "Static file path"
 msgid_plural "Static file paths"
-msgstr[0] "Pfad mit statischen Dateien"
-msgstr[1] "Pfade mit statischen Dateien"
+msgstr[0] "Chemin de fichier statique"
+msgstr[1] "Chemins de fichiers statiques"
 
 #: templates/debug_toolbar/panels/staticfiles.html:7
 #, python-format
 msgid "(prefix %(prefix)s)"
-msgstr "(Präfix %(prefix)s)"
+msgstr "(préfixe %(prefix)s)"
 
 #: templates/debug_toolbar/panels/staticfiles.html:11
 #: templates/debug_toolbar/panels/staticfiles.html:22
 #: templates/debug_toolbar/panels/staticfiles.html:34
 #: templates/debug_toolbar/panels/templates.html:10
 #: templates/debug_toolbar/panels/templates.html:30
 #: templates/debug_toolbar/panels/templates.html:47
 msgid "None"
-msgstr "-"
+msgstr "Aucun"
 
 #: templates/debug_toolbar/panels/staticfiles.html:14
 msgid "Static file app"
 msgid_plural "Static file apps"
-msgstr[0] "App mit statischen Dateien"
-msgstr[1] "Apps mit statischen Dateien"
+msgstr[0] "Application de fichiers statiques"
+msgstr[1] "Applications de fichiers statiques"
 
 #: templates/debug_toolbar/panels/staticfiles.html:25
 msgid "Static file"
 msgid_plural "Static files"
-msgstr[0] "Statische Datei"
-msgstr[1] "Statische Dateien"
+msgstr[0] ""
+msgstr[1] "Fichiers statiques"
 
 #: templates/debug_toolbar/panels/staticfiles.html:39
 #, python-format
 msgid "%(payload_count)s file"
 msgid_plural "%(payload_count)s files"
-msgstr[0] "%(payload_count)s Datei"
-msgstr[1] "%(payload_count)s Dateien"
+msgstr[0] "%(payload_count)s fichier"
+msgstr[1] "%(payload_count)s fichiers"
+
+#: templates/debug_toolbar/panels/staticfiles.html:44
+msgid "Location"
+msgstr "Emplacement"
 
 #: templates/debug_toolbar/panels/template_source.html:4
 msgid "Template source:"
-msgstr "Template-Quelle:"
+msgstr "Source du gabarit :"
 
 #: templates/debug_toolbar/panels/templates.html:2
 msgid "Template path"
 msgid_plural "Template paths"
-msgstr[0] "Template-Pfad"
-msgstr[1] "Template-Pfade"
+msgstr[0] ""
+msgstr[1] "Chemin du gabarit"
 
 #: templates/debug_toolbar/panels/templates.html:13
 msgid "Template"
 msgid_plural "Templates"
-msgstr[0] "Template"
-msgstr[1] "Templates"
+msgstr[0] ""
+msgstr[1] "Gabarit"
 
 #: templates/debug_toolbar/panels/templates.html:22
 #: templates/debug_toolbar/panels/templates.html:40
 msgid "Toggle context"
-msgstr "Context zeigen"
+msgstr "Afficher/masquer le contexte"
 
 #: templates/debug_toolbar/panels/templates.html:33
 msgid "Context processor"
 msgid_plural "Context processors"
-msgstr[0] "Context-Prozessor"
-msgstr[1] "Context-Prozessoren"
+msgstr[0] "Processeur de contexte"
+msgstr[1] "Processeurs de contexte"
 
 #: templates/debug_toolbar/panels/timer.html:2
 msgid "Resource usage"
-msgstr "Ressourcenverwendung"
+msgstr "Utilisation des ressources"
 
 #: templates/debug_toolbar/panels/timer.html:10
 msgid "Resource"
 msgstr "Ressource"
 
 #: templates/debug_toolbar/panels/timer.html:26
 msgid "Browser timing"
-msgstr "Browserzeit"
+msgstr "Chronologie du navigateur"
 
 #: templates/debug_toolbar/panels/timer.html:35
 msgid "Timing attribute"
-msgstr "Timing-Attribut"
+msgstr "Attribut mesuré"
 
 #: templates/debug_toolbar/panels/timer.html:37
 msgid "Milliseconds since navigation start (+length)"
-msgstr "Millisekunden seit Seitenaufruf (plus Dauer)"
+msgstr "Millisecondes depuis le début de la navigation (+longueur)"
 
 #: templates/debug_toolbar/panels/versions.html:10
 msgid "Package"
-msgstr "Paket"
+msgstr "Paquet"
 
 #: templates/debug_toolbar/panels/versions.html:11
 msgid "Name"
-msgstr "Name"
+msgstr "Nom"
 
 #: templates/debug_toolbar/panels/versions.html:12
 msgid "Version"
 msgstr "Version"
 
 #: templates/debug_toolbar/redirect.html:10
 msgid "Location:"
-msgstr "Ziel:"
+msgstr "Emplacement :"
 
 #: templates/debug_toolbar/redirect.html:12
 msgid ""
 "The Django Debug Toolbar has intercepted a redirect to the above URL for "
 "debug viewing purposes. You can click the above link to continue with the "
 "redirect as normal."
-msgstr "Die Django Debug Toolbar hat eine Weiterleitung an die obenstehende URL zur weiteren Überprüfung abgefangen. Klicken Sie den Link, um wie gewohnt weitergeleitet zu werden."
+msgstr ""
+"La barre de débogage Django a intercepté une redirection vers l'URL ci-"
+"dessus afin de permettre la consultation des messages de débogage.  Vous "
+"pouvez cliquer sur le lien ci-dessus pour continuer normalement avec la "
+"redirection."
 
-#: views.py:15
+#: views.py:16
 msgid ""
 "Data for this panel isn't available anymore. Please reload the page and "
 "retry."
-msgstr "Die Daten für dieses Panel sind nicht mehr verfügbar. Bitte laden Sie die Seite neu."
+msgstr ""
+"Les données de ce panneau ne sont plus disponibles. Rechargez la page et "
+"essayez à nouveau."
```

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/locale/en/LC_MESSAGES/django.po` & `django_debug_toolbar-4.0.0/debug_toolbar/locale/pt/LC_MESSAGES/django.po`

 * *Files 6% similar despite different names*

```diff
@@ -1,221 +1,209 @@
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 #
 #
+# Translators:
+# joseduraes <jdmduraes@gmail.com>, 2014
 msgid ""
 msgstr ""
 "Project-Id-Version: Django Debug Toolbar\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-08-23 19:54-0500\n"
-"PO-Revision-Date: 2012-03-31 20:10+0000\n"
-"Last-Translator: \n"
-"Language-Team: \n"
-"Language: en\n"
+"POT-Creation-Date: 2023-01-20 17:23+0100\n"
+"PO-Revision-Date: 2014-04-25 19:53+0000\n"
+"Last-Translator: Aymeric Augustin <aymeric.augustin@m4x.org>\n"
+"Language-Team: Portuguese (http://www.transifex.com/projects/p/django-debug-"
+"toolbar/language/pt/)\n"
+"Language: pt\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1)\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: apps.py:15
 msgid "Debug Toolbar"
 msgstr ""
 
-#: panels/cache.py:227
+#: panels/cache.py:180
 msgid "Cache"
 msgstr ""
 
-#: panels/cache.py:234
+#: panels/cache.py:186
 #, python-format
 msgid "%(cache_calls)d call in %(time).2fms"
 msgid_plural "%(cache_calls)d calls in %(time).2fms"
 msgstr[0] ""
 msgstr[1] ""
 
-#: panels/cache.py:246
+#: panels/cache.py:195
 #, python-format
 msgid "Cache calls from %(count)d backend"
 msgid_plural "Cache calls from %(count)d backends"
 msgstr[0] ""
 msgstr[1] ""
 
-#: panels/headers.py:33
+#: panels/headers.py:31
 msgid "Headers"
 msgstr ""
 
-#: panels/history/panel.py:20 panels/history/panel.py:21
+#: panels/history/panel.py:18 panels/history/panel.py:19
 msgid "History"
 msgstr ""
 
-#: panels/logging.py:63
-msgid "Logging"
-msgstr ""
-
-#: panels/logging.py:69
-#, python-format
-msgid "%(count)s message"
-msgid_plural "%(count)s messages"
-msgstr[0] ""
-msgstr[1] ""
-
-#: panels/logging.py:73
-msgid "Log messages"
-msgstr ""
-
-#: panels/profiling.py:150
+#: panels/profiling.py:140
 msgid "Profiling"
 msgstr ""
 
 #: panels/redirects.py:14
 msgid "Intercept redirects"
-msgstr ""
+msgstr "Intercetar redirecionamentos"
 
 #: panels/request.py:16
 msgid "Request"
-msgstr ""
+msgstr "Pedido"
 
 #: panels/request.py:36
 msgid "<no view>"
 msgstr ""
 
 #: panels/request.py:53
 msgid "<unavailable>"
-msgstr ""
+msgstr "<indisponível>"
 
-#: panels/settings.py:24
+#: panels/settings.py:17
 msgid "Settings"
-msgstr ""
+msgstr "Configurações"
 
-#: panels/settings.py:27
-#, python-format
+#: panels/settings.py:20
+#, fuzzy, python-format
+#| msgid "Settings"
 msgid "Settings from %s"
-msgstr ""
+msgstr "Configurações"
 
-#: panels/signals.py:58
+#: panels/signals.py:57
 #, python-format
 msgid "%(num_receivers)d receiver of 1 signal"
 msgid_plural "%(num_receivers)d receivers of 1 signal"
 msgstr[0] ""
 msgstr[1] ""
 
-#: panels/signals.py:66
+#: panels/signals.py:62
 #, python-format
 msgid "%(num_receivers)d receiver of %(num_signals)d signals"
 msgid_plural "%(num_receivers)d receivers of %(num_signals)d signals"
 msgstr[0] ""
 msgstr[1] ""
 
-#: panels/signals.py:73
+#: panels/signals.py:67
 msgid "Signals"
-msgstr ""
+msgstr "Sinais"
 
-#: panels/sql/panel.py:24
+#: panels/sql/panel.py:23
 msgid "Autocommit"
 msgstr ""
 
-#: panels/sql/panel.py:25
+#: panels/sql/panel.py:24
 msgid "Read uncommitted"
 msgstr ""
 
-#: panels/sql/panel.py:26
+#: panels/sql/panel.py:25
 msgid "Read committed"
 msgstr ""
 
-#: panels/sql/panel.py:27
+#: panels/sql/panel.py:26
 msgid "Repeatable read"
 msgstr ""
 
-#: panels/sql/panel.py:28
+#: panels/sql/panel.py:27
 msgid "Serializable"
-msgstr ""
+msgstr "Variável"
 
-#: panels/sql/panel.py:40
+#: panels/sql/panel.py:39
 msgid "Idle"
 msgstr ""
 
-#: panels/sql/panel.py:41
+#: panels/sql/panel.py:40
 msgid "Active"
-msgstr ""
+msgstr "Acção"
 
-#: panels/sql/panel.py:42
+#: panels/sql/panel.py:41
 msgid "In transaction"
 msgstr ""
 
-#: panels/sql/panel.py:43
+#: panels/sql/panel.py:42
 msgid "In error"
-msgstr ""
+msgstr "Erro"
 
-#: panels/sql/panel.py:44
+#: panels/sql/panel.py:43
 msgid "Unknown"
-msgstr ""
+msgstr "Desconhecido"
 
-#: panels/sql/panel.py:109
+#: panels/sql/panel.py:130
 msgid "SQL"
 msgstr ""
 
-#: panels/sql/panel.py:114
+#: panels/sql/panel.py:135
 #, python-format
 msgid "%(query_count)d query in %(sql_time).2fms"
 msgid_plural "%(query_count)d queries in %(sql_time).2fms"
 msgstr[0] ""
 msgstr[1] ""
 
-#: panels/sql/panel.py:127
+#: panels/sql/panel.py:147
 #, python-format
 msgid "SQL queries from %(count)d connection"
 msgid_plural "SQL queries from %(count)d connections"
 msgstr[0] ""
 msgstr[1] ""
 
-#: panels/staticfiles.py:85
+#: panels/staticfiles.py:84
 #, python-format
 msgid "Static files (%(num_found)s found, %(num_used)s used)"
 msgstr ""
 
-#: panels/staticfiles.py:106
+#: panels/staticfiles.py:105
 msgid "Static files"
-msgstr ""
+msgstr "Ficheiros estáticos"
 
-#: panels/staticfiles.py:112
+#: panels/staticfiles.py:111
 #, python-format
 msgid "%(num_used)s file used"
 msgid_plural "%(num_used)s files used"
 msgstr[0] ""
 msgstr[1] ""
 
-#: panels/templates/panel.py:144
+#: panels/templates/panel.py:143
 msgid "Templates"
-msgstr ""
+msgstr "Templates"
 
-#: panels/templates/panel.py:149
+#: panels/templates/panel.py:148
 #, python-format
 msgid "Templates (%(num_templates)s rendered)"
-msgstr ""
+msgstr "Templates (%(num_templates)s renderizados)"
 
-#: panels/templates/panel.py:181
+#: panels/templates/panel.py:180
 msgid "No origin"
 msgstr ""
 
 #: panels/timer.py:25
 #, python-format
 msgid "CPU: %(cum)0.2fms (%(total)0.2fms)"
 msgstr ""
 
 #: panels/timer.py:30
 #, python-format
 msgid "Total: %0.2fms"
-msgstr ""
+msgstr "Total: %0.2fms"
 
 #: panels/timer.py:36 templates/debug_toolbar/panels/history.html:9
-#: templates/debug_toolbar/panels/logging.html:7
 #: templates/debug_toolbar/panels/sql_explain.html:11
 #: templates/debug_toolbar/panels/sql_profile.html:12
 #: templates/debug_toolbar/panels/sql_select.html:11
 msgid "Time"
-msgstr ""
+msgstr "Tempo"
 
 #: panels/timer.py:44
 msgid "User CPU time"
 msgstr ""
 
 #: panels/timer.py:44
 #, python-format
@@ -256,39 +244,39 @@
 #: panels/timer.py:50
 #, python-format
 msgid "%(vcsw)d voluntary, %(ivcsw)d involuntary"
 msgstr ""
 
 #: panels/versions.py:19
 msgid "Versions"
-msgstr ""
+msgstr "Versões"
 
-#: templates/debug_toolbar/base.html:18
+#: templates/debug_toolbar/base.html:22
 msgid "Hide toolbar"
-msgstr ""
+msgstr "Ocultar barra"
 
-#: templates/debug_toolbar/base.html:18
+#: templates/debug_toolbar/base.html:22
 msgid "Hide"
-msgstr ""
+msgstr "Ocultar"
 
-#: templates/debug_toolbar/base.html:25
+#: templates/debug_toolbar/base.html:29
 msgid "Show toolbar"
-msgstr ""
+msgstr "Mostrar barra"
 
 #: templates/debug_toolbar/includes/panel_button.html:4
 msgid "Disable for next and successive requests"
-msgstr ""
+msgstr "Desactivar para o seguinte e sucessivos pedidos"
 
 #: templates/debug_toolbar/includes/panel_button.html:4
 msgid "Enable for next and successive requests"
-msgstr ""
+msgstr "Activar para o próximo e sucessivos pedidos"
 
 #: templates/debug_toolbar/panels/cache.html:2
 msgid "Summary"
-msgstr ""
+msgstr "Resumo"
 
 #: templates/debug_toolbar/panels/cache.html:6
 msgid "Total calls"
 msgstr ""
 
 #: templates/debug_toolbar/panels/cache.html:7
 msgid "Total time"
@@ -300,28 +288,28 @@
 
 #: templates/debug_toolbar/panels/cache.html:9
 msgid "Cache misses"
 msgstr ""
 
 #: templates/debug_toolbar/panels/cache.html:21
 msgid "Commands"
-msgstr ""
+msgstr "Comandos"
 
 #: templates/debug_toolbar/panels/cache.html:39
 msgid "Calls"
 msgstr ""
 
 #: templates/debug_toolbar/panels/cache.html:43
 #: templates/debug_toolbar/panels/sql.html:36
 msgid "Time (ms)"
 msgstr ""
 
 #: templates/debug_toolbar/panels/cache.html:44
 msgid "Type"
-msgstr ""
+msgstr "Tipo"
 
 #: templates/debug_toolbar/panels/cache.html:45
 #: templates/debug_toolbar/panels/request.html:8
 msgid "Arguments"
 msgstr ""
 
 #: templates/debug_toolbar/panels/cache.html:46
@@ -337,25 +325,25 @@
 msgid "Request headers"
 msgstr ""
 
 #: templates/debug_toolbar/panels/headers.html:8
 #: templates/debug_toolbar/panels/headers.html:27
 #: templates/debug_toolbar/panels/headers.html:48
 msgid "Key"
-msgstr ""
+msgstr "Chave"
 
 #: templates/debug_toolbar/panels/headers.html:9
 #: templates/debug_toolbar/panels/headers.html:28
 #: templates/debug_toolbar/panels/headers.html:49
 #: templates/debug_toolbar/panels/history_tr.html:23
-#: templates/debug_toolbar/panels/request_variables.html:11
+#: templates/debug_toolbar/panels/request_variables.html:12
 #: templates/debug_toolbar/panels/settings.html:6
 #: templates/debug_toolbar/panels/timer.html:11
 msgid "Value"
-msgstr ""
+msgstr "Valor"
 
 #: templates/debug_toolbar/panels/headers.html:22
 msgid "Response headers"
 msgstr ""
 
 #: templates/debug_toolbar/panels/headers.html:41
 msgid "WSGI environ"
@@ -373,51 +361,32 @@
 
 #: templates/debug_toolbar/panels/history.html:11
 #: templates/debug_toolbar/panels/staticfiles.html:43
 msgid "Path"
 msgstr ""
 
 #: templates/debug_toolbar/panels/history.html:12
+#, fuzzy
+#| msgid "Variable"
 msgid "Request Variables"
-msgstr ""
+msgstr "Variável"
 
 #: templates/debug_toolbar/panels/history.html:13
 msgid "Status"
 msgstr ""
 
 #: templates/debug_toolbar/panels/history.html:14
 #: templates/debug_toolbar/panels/sql.html:37
 msgid "Action"
-msgstr ""
+msgstr "Acção"
 
 #: templates/debug_toolbar/panels/history_tr.html:22
-#: templates/debug_toolbar/panels/request_variables.html:10
+#: templates/debug_toolbar/panels/request_variables.html:11
 msgid "Variable"
-msgstr ""
-
-#: templates/debug_toolbar/panels/logging.html:6
-msgid "Level"
-msgstr ""
-
-#: templates/debug_toolbar/panels/logging.html:8
-msgid "Channel"
-msgstr ""
-
-#: templates/debug_toolbar/panels/logging.html:9
-msgid "Message"
-msgstr ""
-
-#: templates/debug_toolbar/panels/logging.html:10
-#: templates/debug_toolbar/panels/staticfiles.html:44
-msgid "Location"
-msgstr ""
-
-#: templates/debug_toolbar/panels/logging.html:26
-msgid "No messages logged"
-msgstr ""
+msgstr "Variável"
 
 #: templates/debug_toolbar/panels/profiling.html:5
 msgid "Call"
 msgstr ""
 
 #: templates/debug_toolbar/panels/profiling.html:6
 msgid "CumTime"
@@ -466,35 +435,35 @@
 
 #: templates/debug_toolbar/panels/request.html:38
 msgid "GET data"
 msgstr ""
 
 #: templates/debug_toolbar/panels/request.html:41
 msgid "No GET data"
-msgstr ""
+msgstr "Sem dados GET"
 
 #: templates/debug_toolbar/panels/request.html:45
 msgid "POST data"
-msgstr ""
+msgstr "dados POST"
 
 #: templates/debug_toolbar/panels/request.html:48
 msgid "No POST data"
-msgstr ""
+msgstr "Sem variáveis POST"
 
 #: templates/debug_toolbar/panels/settings.html:5
 msgid "Setting"
-msgstr ""
+msgstr "Configurações"
 
 #: templates/debug_toolbar/panels/signals.html:5
 msgid "Signal"
-msgstr ""
+msgstr "Sinal"
 
 #: templates/debug_toolbar/panels/signals.html:6
 msgid "Receivers"
-msgstr ""
+msgstr "Receptores"
 
 #: templates/debug_toolbar/panels/sql.html:6
 #, python-format
 msgid "%(num)s query"
 msgid_plural "%(num)s queries"
 msgstr[0] ""
 msgstr[1] ""
@@ -538,104 +507,108 @@
 
 #: templates/debug_toolbar/panels/sql.html:97
 msgid "Isolation level:"
 msgstr ""
 
 #: templates/debug_toolbar/panels/sql.html:100
 msgid "Transaction status:"
-msgstr ""
+msgstr "Estado da transacção:"
 
 #: templates/debug_toolbar/panels/sql.html:114
 msgid "(unknown)"
-msgstr ""
+msgstr "(desconhecido)"
 
 #: templates/debug_toolbar/panels/sql.html:123
 msgid "No SQL queries were recorded during this request."
-msgstr ""
+msgstr "Nenhuma query SQL foi registada durante este pedido."
 
 #: templates/debug_toolbar/panels/sql_explain.html:4
 msgid "SQL explained"
 msgstr ""
 
 #: templates/debug_toolbar/panels/sql_explain.html:9
 #: templates/debug_toolbar/panels/sql_profile.html:10
 #: templates/debug_toolbar/panels/sql_select.html:9
 msgid "Executed SQL"
-msgstr ""
+msgstr "SQL Executado"
 
 #: templates/debug_toolbar/panels/sql_explain.html:13
 #: templates/debug_toolbar/panels/sql_profile.html:14
 #: templates/debug_toolbar/panels/sql_select.html:13
 msgid "Database"
 msgstr ""
 
 #: templates/debug_toolbar/panels/sql_profile.html:4
 msgid "SQL profiled"
 msgstr ""
 
 #: templates/debug_toolbar/panels/sql_profile.html:37
 msgid "Error"
-msgstr ""
+msgstr "Erro"
 
 #: templates/debug_toolbar/panels/sql_select.html:4
 msgid "SQL selected"
 msgstr ""
 
 #: templates/debug_toolbar/panels/sql_select.html:36
 msgid "Empty set"
-msgstr ""
+msgstr "Set vazio"
 
 #: templates/debug_toolbar/panels/staticfiles.html:3
 msgid "Static file path"
 msgid_plural "Static file paths"
 msgstr[0] ""
 msgstr[1] ""
 
 #: templates/debug_toolbar/panels/staticfiles.html:7
 #, python-format
 msgid "(prefix %(prefix)s)"
-msgstr ""
+msgstr "(prefixo %(prefix)s)"
 
 #: templates/debug_toolbar/panels/staticfiles.html:11
 #: templates/debug_toolbar/panels/staticfiles.html:22
 #: templates/debug_toolbar/panels/staticfiles.html:34
 #: templates/debug_toolbar/panels/templates.html:10
 #: templates/debug_toolbar/panels/templates.html:30
 #: templates/debug_toolbar/panels/templates.html:47
 msgid "None"
-msgstr ""
+msgstr "Nenhum"
 
 #: templates/debug_toolbar/panels/staticfiles.html:14
 msgid "Static file app"
 msgid_plural "Static file apps"
 msgstr[0] ""
 msgstr[1] ""
 
 #: templates/debug_toolbar/panels/staticfiles.html:25
 msgid "Static file"
 msgid_plural "Static files"
-msgstr[0] ""
-msgstr[1] ""
+msgstr[0] "Ficheiro estático"
+msgstr[1] "Ficheiros estáticos"
 
 #: templates/debug_toolbar/panels/staticfiles.html:39
 #, python-format
 msgid "%(payload_count)s file"
 msgid_plural "%(payload_count)s files"
 msgstr[0] ""
 msgstr[1] ""
 
+#: templates/debug_toolbar/panels/staticfiles.html:44
+msgid "Location"
+msgstr "Localização"
+
 #: templates/debug_toolbar/panels/template_source.html:4
 msgid "Template source:"
 msgstr ""
 
 #: templates/debug_toolbar/panels/templates.html:2
 msgid "Template path"
 msgid_plural "Template paths"
 msgstr[0] ""
-msgstr[1] ""
+msgstr[1] "Caminho da Template"
 
 #: templates/debug_toolbar/panels/templates.html:13
 msgid "Template"
 msgid_plural "Templates"
 msgstr[0] ""
 msgstr[1] ""
 
@@ -644,23 +617,23 @@
 msgid "Toggle context"
 msgstr ""
 
 #: templates/debug_toolbar/panels/templates.html:33
 msgid "Context processor"
 msgid_plural "Context processors"
 msgstr[0] ""
-msgstr[1] ""
+msgstr[1] "Processador de Contexto"
 
 #: templates/debug_toolbar/panels/timer.html:2
 msgid "Resource usage"
 msgstr ""
 
 #: templates/debug_toolbar/panels/timer.html:10
 msgid "Resource"
-msgstr ""
+msgstr "Recurso"
 
 #: templates/debug_toolbar/panels/timer.html:26
 msgid "Browser timing"
 msgstr ""
 
 #: templates/debug_toolbar/panels/timer.html:35
 msgid "Timing attribute"
@@ -672,29 +645,29 @@
 
 #: templates/debug_toolbar/panels/versions.html:10
 msgid "Package"
 msgstr ""
 
 #: templates/debug_toolbar/panels/versions.html:11
 msgid "Name"
-msgstr ""
+msgstr "Nome"
 
 #: templates/debug_toolbar/panels/versions.html:12
 msgid "Version"
-msgstr ""
+msgstr "Versão"
 
 #: templates/debug_toolbar/redirect.html:10
 msgid "Location:"
-msgstr ""
+msgstr "Localização"
 
 #: templates/debug_toolbar/redirect.html:12
 msgid ""
 "The Django Debug Toolbar has intercepted a redirect to the above URL for "
 "debug viewing purposes. You can click the above link to continue with the "
 "redirect as normal."
 msgstr ""
 
-#: views.py:15
+#: views.py:16
 msgid ""
 "Data for this panel isn't available anymore. Please reload the page and "
 "retry."
 msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/locale/es/LC_MESSAGES/django.mo` & `django_debug_toolbar-4.0.0/debug_toolbar/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/locale/es/LC_MESSAGES/django.po` & `django_debug_toolbar-4.0.0/debug_toolbar/locale/es/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -8,70 +8,56 @@
 # Leonardo J. Caballero G. <leonardocaballero@gmail.com>, 2013-2014,2020
 # marcelor <marcelor@gmail.com>, 2013
 # Sergio Infante <rsinfante@gmail.com>, 2015
 msgid ""
 msgstr ""
 "Project-Id-Version: Django Debug Toolbar\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-08-14 10:25-0500\n"
+"POT-Creation-Date: 2023-01-20 17:23+0100\n"
 "PO-Revision-Date: 2021-10-01 11:10+0000\n"
 "Last-Translator: Daniel Iglesias <igledaniel@gmail.com>\n"
-"Language-Team: Spanish (http://www.transifex.com/django-debug-toolbar/django-debug-toolbar/language/es/)\n"
+"Language-Team: Spanish (http://www.transifex.com/django-debug-toolbar/django-"
+"debug-toolbar/language/es/)\n"
+"Language: es\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: es\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: apps.py:15
 msgid "Debug Toolbar"
 msgstr "Barra de herramientas de Depuración"
 
-#: panels/cache.py:227
+#: panels/cache.py:180
 msgid "Cache"
 msgstr "Cache"
 
-#: panels/cache.py:234
+#: panels/cache.py:186
 #, python-format
 msgid "%(cache_calls)d call in %(time).2fms"
 msgid_plural "%(cache_calls)d calls in %(time).2fms"
 msgstr[0] "%(cache_calls)d llamada en %(time).2fms"
 msgstr[1] "%(cache_calls)d llamadas en %(time).2fms"
 
-#: panels/cache.py:246
+#: panels/cache.py:195
 #, python-format
 msgid "Cache calls from %(count)d backend"
 msgid_plural "Cache calls from %(count)d backends"
 msgstr[0] "%(count)d llamadas al Cache desde el backend"
 msgstr[1] "%(count)d llamadas al Caché desde backends"
 
-#: panels/headers.py:33
+#: panels/headers.py:31
 msgid "Headers"
 msgstr "Encabezados"
 
-#: panels/history/panel.py:20 panels/history/panel.py:21
+#: panels/history/panel.py:18 panels/history/panel.py:19
 msgid "History"
 msgstr "Historial"
 
-#: panels/logging.py:63
-msgid "Logging"
-msgstr "Registros"
-
-#: panels/logging.py:69
-#, python-format
-msgid "%(count)s message"
-msgid_plural "%(count)s messages"
-msgstr[0] "%(count)s mensaje"
-msgstr[1] "%(count)s mensajes"
-
-#: panels/logging.py:73
-msgid "Log messages"
-msgstr "Mensajes del registro"
-
-#: panels/profiling.py:150
+#: panels/profiling.py:140
 msgid "Profiling"
 msgstr "Análisis de rendimiento"
 
 #: panels/redirects.py:14
 msgid "Intercept redirects"
 msgstr "Interceptar re-direcionamiento"
 
@@ -83,140 +69,139 @@
 msgid "<no view>"
 msgstr "<sin vista>"
 
 #: panels/request.py:53
 msgid "<unavailable>"
 msgstr "<no disponible>"
 
-#: panels/settings.py:24
+#: panels/settings.py:17
 msgid "Settings"
 msgstr "Configuraciones"
 
-#: panels/settings.py:27
+#: panels/settings.py:20
 #, python-format
 msgid "Settings from %s"
 msgstr "Valores procedentes de %s"
 
-#: panels/signals.py:58
+#: panels/signals.py:57
 #, python-format
 msgid "%(num_receivers)d receiver of 1 signal"
 msgid_plural "%(num_receivers)d receivers of 1 signal"
 msgstr[0] "%(num_receivers)d receptor de 1 señal"
 msgstr[1] "%(num_receivers)d receptores de 1 señal"
 
-#: panels/signals.py:66
+#: panels/signals.py:62
 #, python-format
 msgid "%(num_receivers)d receiver of %(num_signals)d signals"
 msgid_plural "%(num_receivers)d receivers of %(num_signals)d signals"
 msgstr[0] "%(num_receivers)d receptor de %(num_signals)d señales"
 msgstr[1] "%(num_receivers)d receptores de %(num_signals)d señales"
 
-#: panels/signals.py:73
+#: panels/signals.py:67
 msgid "Signals"
 msgstr "Señales"
 
-#: panels/sql/panel.py:24
+#: panels/sql/panel.py:23
 msgid "Autocommit"
 msgstr "Autocommit"
 
-#: panels/sql/panel.py:25
+#: panels/sql/panel.py:24
 msgid "Read uncommitted"
 msgstr "Leer cambios tentativos"
 
-#: panels/sql/panel.py:26
+#: panels/sql/panel.py:25
 msgid "Read committed"
 msgstr "Leer cambios permanentes"
 
-#: panels/sql/panel.py:27
+#: panels/sql/panel.py:26
 msgid "Repeatable read"
 msgstr "Lectura repetible"
 
-#: panels/sql/panel.py:28
+#: panels/sql/panel.py:27
 msgid "Serializable"
 msgstr "Serializable"
 
-#: panels/sql/panel.py:40
+#: panels/sql/panel.py:39
 msgid "Idle"
 msgstr "Inactivo"
 
-#: panels/sql/panel.py:41
+#: panels/sql/panel.py:40
 msgid "Active"
 msgstr "Activo"
 
-#: panels/sql/panel.py:42
+#: panels/sql/panel.py:41
 msgid "In transaction"
 msgstr "En transacción"
 
-#: panels/sql/panel.py:43
+#: panels/sql/panel.py:42
 msgid "In error"
 msgstr "En error"
 
-#: panels/sql/panel.py:44
+#: panels/sql/panel.py:43
 msgid "Unknown"
 msgstr "Desconocido"
 
-#: panels/sql/panel.py:109
+#: panels/sql/panel.py:130
 msgid "SQL"
 msgstr "SQL"
 
-#: panels/sql/panel.py:114
+#: panels/sql/panel.py:135
 #, python-format
 msgid "%(query_count)d query in %(sql_time).2fms"
 msgid_plural "%(query_count)d queries in %(sql_time).2fms"
 msgstr[0] ""
 msgstr[1] ""
 
-#: panels/sql/panel.py:127
+#: panels/sql/panel.py:147
 #, python-format
 msgid "SQL queries from %(count)d connection"
 msgid_plural "SQL queries from %(count)d connections"
 msgstr[0] ""
 msgstr[1] ""
 
-#: panels/staticfiles.py:85
+#: panels/staticfiles.py:84
 #, python-format
 msgid "Static files (%(num_found)s found, %(num_used)s used)"
 msgstr "Archivos estáticos (%(num_found)s encontrados, %(num_used)s en uso)"
 
-#: panels/staticfiles.py:106
+#: panels/staticfiles.py:105
 msgid "Static files"
 msgstr "Archivos estáticos"
 
-#: panels/staticfiles.py:112
+#: panels/staticfiles.py:111
 #, python-format
 msgid "%(num_used)s file used"
 msgid_plural "%(num_used)s files used"
 msgstr[0] "%(num_used)s archivo usado"
 msgstr[1] "%(num_used)s archivos usados"
 
-#: panels/templates/panel.py:144
+#: panels/templates/panel.py:143
 msgid "Templates"
 msgstr "Plantillas"
 
-#: panels/templates/panel.py:149
+#: panels/templates/panel.py:148
 #, python-format
 msgid "Templates (%(num_templates)s rendered)"
 msgstr "Plantillas (%(num_templates)s renderizadas)"
 
-#: panels/templates/panel.py:181
+#: panels/templates/panel.py:180
 msgid "No origin"
 msgstr "Sin origen"
 
 #: panels/timer.py:25
 #, python-format
 msgid "CPU: %(cum)0.2fms (%(total)0.2fms)"
 msgstr "CPU: %(cum)0.2fms (%(total)0.2fms)"
 
 #: panels/timer.py:30
 #, python-format
 msgid "Total: %0.2fms"
 msgstr "Total: %0.2fms"
 
 #: panels/timer.py:36 templates/debug_toolbar/panels/history.html:9
-#: templates/debug_toolbar/panels/logging.html:7
 #: templates/debug_toolbar/panels/sql_explain.html:11
 #: templates/debug_toolbar/panels/sql_profile.html:12
 #: templates/debug_toolbar/panels/sql_select.html:11
 msgid "Time"
 msgstr "Tiempo"
 
 #: panels/timer.py:44
@@ -264,23 +249,23 @@
 msgid "%(vcsw)d voluntary, %(ivcsw)d involuntary"
 msgstr "%(vcsw)d voluntario, %(ivcsw)d involuntario"
 
 #: panels/versions.py:19
 msgid "Versions"
 msgstr "Versiones"
 
-#: templates/debug_toolbar/base.html:18
+#: templates/debug_toolbar/base.html:22
 msgid "Hide toolbar"
 msgstr "Ocutar barra de herramientas"
 
-#: templates/debug_toolbar/base.html:18
+#: templates/debug_toolbar/base.html:22
 msgid "Hide"
 msgstr "Ocultar"
 
-#: templates/debug_toolbar/base.html:25
+#: templates/debug_toolbar/base.html:29
 msgid "Show toolbar"
 msgstr "Mostrar barra de herramientas"
 
 #: templates/debug_toolbar/includes/panel_button.html:4
 msgid "Disable for next and successive requests"
 msgstr "Deshabilitar para el próximo y sucesivos peticiones"
 
@@ -349,15 +334,15 @@
 msgid "Key"
 msgstr "Clave"
 
 #: templates/debug_toolbar/panels/headers.html:9
 #: templates/debug_toolbar/panels/headers.html:28
 #: templates/debug_toolbar/panels/headers.html:49
 #: templates/debug_toolbar/panels/history_tr.html:23
-#: templates/debug_toolbar/panels/request_variables.html:11
+#: templates/debug_toolbar/panels/request_variables.html:12
 #: templates/debug_toolbar/panels/settings.html:6
 #: templates/debug_toolbar/panels/timer.html:11
 msgid "Value"
 msgstr "Valor"
 
 #: templates/debug_toolbar/panels/headers.html:22
 msgid "Response headers"
@@ -367,15 +352,17 @@
 msgid "WSGI environ"
 msgstr "Entorno WSGI"
 
 #: templates/debug_toolbar/panels/headers.html:43
 msgid ""
 "Since the WSGI environ inherits the environment of the server, only a "
 "significant subset is shown below."
-msgstr "Ya que el entorno WSGI hereda el entorno del servidor, solo un subconjunto significativo es mostrado más abajo."
+msgstr ""
+"Ya que el entorno WSGI hereda el entorno del servidor, solo un subconjunto "
+"significativo es mostrado más abajo."
 
 #: templates/debug_toolbar/panels/history.html:10
 msgid "Method"
 msgstr "Método"
 
 #: templates/debug_toolbar/panels/history.html:11
 #: templates/debug_toolbar/panels/staticfiles.html:43
@@ -392,39 +379,18 @@
 
 #: templates/debug_toolbar/panels/history.html:14
 #: templates/debug_toolbar/panels/sql.html:37
 msgid "Action"
 msgstr "Acción"
 
 #: templates/debug_toolbar/panels/history_tr.html:22
-#: templates/debug_toolbar/panels/request_variables.html:10
+#: templates/debug_toolbar/panels/request_variables.html:11
 msgid "Variable"
 msgstr "Variable"
 
-#: templates/debug_toolbar/panels/logging.html:6
-msgid "Level"
-msgstr "Nivel"
-
-#: templates/debug_toolbar/panels/logging.html:8
-msgid "Channel"
-msgstr "Canal"
-
-#: templates/debug_toolbar/panels/logging.html:9
-msgid "Message"
-msgstr "Mensaje"
-
-#: templates/debug_toolbar/panels/logging.html:10
-#: templates/debug_toolbar/panels/staticfiles.html:44
-msgid "Location"
-msgstr "Ubicación"
-
-#: templates/debug_toolbar/panels/logging.html:26
-msgid "No messages logged"
-msgstr "No hay mensajes registrados"
-
 #: templates/debug_toolbar/panels/profiling.html:5
 msgid "Call"
 msgstr "Llamar"
 
 #: templates/debug_toolbar/panels/profiling.html:6
 msgid "CumTime"
 msgstr "TiempoAcum"
@@ -513,15 +479,17 @@
 msgstr ""
 
 #: templates/debug_toolbar/panels/sql.html:12
 #, python-format
 msgid ""
 "and <abbr title=\"Duplicate queries are identical to each other: they "
 "execute exactly the same SQL and parameters.\">%(dupes)s duplicates</abbr>"
-msgstr "y <abbr title=\"Las consultas repetidas son idénticas: ejecutan el mismo SQL con los mismos parámetros. \">%(dupes)s repetidos</abbr>"
+msgstr ""
+"y <abbr title=\"Las consultas repetidas son idénticas: ejecutan el mismo SQL "
+"con los mismos parámetros. \">%(dupes)s repetidos</abbr>"
 
 #: templates/debug_toolbar/panels/sql.html:34
 msgid "Query"
 msgstr "Query"
 
 #: templates/debug_toolbar/panels/sql.html:35
 #: templates/debug_toolbar/panels/timer.html:36
@@ -625,14 +593,18 @@
 #: templates/debug_toolbar/panels/staticfiles.html:39
 #, python-format
 msgid "%(payload_count)s file"
 msgid_plural "%(payload_count)s files"
 msgstr[0] "%(payload_count)s archivo"
 msgstr[1] "%(payload_count)s archivos"
 
+#: templates/debug_toolbar/panels/staticfiles.html:44
+msgid "Location"
+msgstr "Ubicación"
+
 #: templates/debug_toolbar/panels/template_source.html:4
 msgid "Template source:"
 msgstr "Fuente de plantilla:"
 
 #: templates/debug_toolbar/panels/templates.html:2
 msgid "Template path"
 msgid_plural "Template paths"
@@ -693,14 +665,20 @@
 msgstr "Ubicación:"
 
 #: templates/debug_toolbar/redirect.html:12
 msgid ""
 "The Django Debug Toolbar has intercepted a redirect to the above URL for "
 "debug viewing purposes. You can click the above link to continue with the "
 "redirect as normal."
-msgstr "El Django Debug Toolbar ha interceptado un re-direccionamiento a la dirección de Internet mostrada arriba, con el propósito de inspeccionarla. Usted puede hacer clic en el vínculo de arriba para continuar con el re-direccionamiento normalmente."
+msgstr ""
+"El Django Debug Toolbar ha interceptado un re-direccionamiento a la "
+"dirección de Internet mostrada arriba, con el propósito de inspeccionarla. "
+"Usted puede hacer clic en el vínculo de arriba para continuar con el re-"
+"direccionamiento normalmente."
 
-#: views.py:15
+#: views.py:16
 msgid ""
 "Data for this panel isn't available anymore. Please reload the page and "
 "retry."
-msgstr "La información de este panel ya no se encuentra disponible. Por favor recargue la página y pruebe nuevamente."
+msgstr ""
+"La información de este panel ya no se encuentra disponible. Por favor "
+"recargue la página y pruebe nuevamente."
```

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/locale/fa/LC_MESSAGES/django.mo` & `django_debug_toolbar-4.0.0/debug_toolbar/locale/fa/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/locale/fa/LC_MESSAGES/django.po` & `django_debug_toolbar-4.0.0/debug_toolbar/locale/fa/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,70 +4,56 @@
 #
 # Translators:
 # Ali Soltani <alisoltanics@gmail.com>, 2021
 msgid ""
 msgstr ""
 "Project-Id-Version: Django Debug Toolbar\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-08-14 10:25-0500\n"
+"POT-Creation-Date: 2023-01-20 17:23+0100\n"
 "PO-Revision-Date: 2021-09-30 18:42+0000\n"
 "Last-Translator: Ali Soltani <alisoltanics@gmail.com>\n"
-"Language-Team: Persian (http://www.transifex.com/django-debug-toolbar/django-debug-toolbar/language/fa/)\n"
+"Language-Team: Persian (http://www.transifex.com/django-debug-toolbar/django-"
+"debug-toolbar/language/fa/)\n"
+"Language: fa\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: fa\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
 #: apps.py:15
 msgid "Debug Toolbar"
 msgstr "نوار ابزار دیباگ"
 
-#: panels/cache.py:227
+#: panels/cache.py:180
 msgid "Cache"
 msgstr "Cache"
 
-#: panels/cache.py:234
+#: panels/cache.py:186
 #, python-format
 msgid "%(cache_calls)d call in %(time).2fms"
 msgid_plural "%(cache_calls)d calls in %(time).2fms"
 msgstr[0] ""
 msgstr[1] ""
 
-#: panels/cache.py:246
+#: panels/cache.py:195
 #, python-format
 msgid "Cache calls from %(count)d backend"
 msgid_plural "Cache calls from %(count)d backends"
 msgstr[0] ""
 msgstr[1] ""
 
-#: panels/headers.py:33
+#: panels/headers.py:31
 msgid "Headers"
 msgstr "هدر ها"
 
-#: panels/history/panel.py:20 panels/history/panel.py:21
+#: panels/history/panel.py:18 panels/history/panel.py:19
 msgid "History"
 msgstr "تاریخچه"
 
-#: panels/logging.py:63
-msgid "Logging"
-msgstr "لاگ"
-
-#: panels/logging.py:69
-#, python-format
-msgid "%(count)s message"
-msgid_plural "%(count)s messages"
-msgstr[0] ""
-msgstr[1] ""
-
-#: panels/logging.py:73
-msgid "Log messages"
-msgstr "پیام های لاگ"
-
-#: panels/profiling.py:150
+#: panels/profiling.py:140
 msgid "Profiling"
 msgstr "نمایه سازی"
 
 #: panels/redirects.py:14
 msgid "Intercept redirects"
 msgstr ""
 
@@ -79,140 +65,139 @@
 msgid "<no view>"
 msgstr ""
 
 #: panels/request.py:53
 msgid "<unavailable>"
 msgstr ""
 
-#: panels/settings.py:24
+#: panels/settings.py:17
 msgid "Settings"
 msgstr "تنظیمات"
 
-#: panels/settings.py:27
+#: panels/settings.py:20
 #, python-format
 msgid "Settings from %s"
 msgstr "تنظیمات از %s"
 
-#: panels/signals.py:58
+#: panels/signals.py:57
 #, python-format
 msgid "%(num_receivers)d receiver of 1 signal"
 msgid_plural "%(num_receivers)d receivers of 1 signal"
 msgstr[0] ""
 msgstr[1] ""
 
-#: panels/signals.py:66
+#: panels/signals.py:62
 #, python-format
 msgid "%(num_receivers)d receiver of %(num_signals)d signals"
 msgid_plural "%(num_receivers)d receivers of %(num_signals)d signals"
 msgstr[0] ""
 msgstr[1] ""
 
-#: panels/signals.py:73
+#: panels/signals.py:67
 msgid "Signals"
 msgstr "signal ها"
 
-#: panels/sql/panel.py:24
+#: panels/sql/panel.py:23
 msgid "Autocommit"
 msgstr "کامیت خودکار"
 
-#: panels/sql/panel.py:25
+#: panels/sql/panel.py:24
 msgid "Read uncommitted"
 msgstr ""
 
-#: panels/sql/panel.py:26
+#: panels/sql/panel.py:25
 msgid "Read committed"
 msgstr ""
 
-#: panels/sql/panel.py:27
+#: panels/sql/panel.py:26
 msgid "Repeatable read"
 msgstr ""
 
-#: panels/sql/panel.py:28
+#: panels/sql/panel.py:27
 msgid "Serializable"
 msgstr "قابل سریالایز شدن"
 
-#: panels/sql/panel.py:40
+#: panels/sql/panel.py:39
 msgid "Idle"
 msgstr "IDLE"
 
-#: panels/sql/panel.py:41
+#: panels/sql/panel.py:40
 msgid "Active"
 msgstr "فعال"
 
-#: panels/sql/panel.py:42
+#: panels/sql/panel.py:41
 msgid "In transaction"
 msgstr "در تراکنش"
 
-#: panels/sql/panel.py:43
+#: panels/sql/panel.py:42
 msgid "In error"
 msgstr "در خطا"
 
-#: panels/sql/panel.py:44
+#: panels/sql/panel.py:43
 msgid "Unknown"
 msgstr "ناشناخته"
 
-#: panels/sql/panel.py:109
+#: panels/sql/panel.py:130
 msgid "SQL"
 msgstr "اس کیو ال"
 
-#: panels/sql/panel.py:114
+#: panels/sql/panel.py:135
 #, python-format
 msgid "%(query_count)d query in %(sql_time).2fms"
 msgid_plural "%(query_count)d queries in %(sql_time).2fms"
 msgstr[0] ""
 msgstr[1] ""
 
-#: panels/sql/panel.py:127
+#: panels/sql/panel.py:147
 #, python-format
 msgid "SQL queries from %(count)d connection"
 msgid_plural "SQL queries from %(count)d connections"
 msgstr[0] ""
 msgstr[1] ""
 
-#: panels/staticfiles.py:85
+#: panels/staticfiles.py:84
 #, python-format
 msgid "Static files (%(num_found)s found, %(num_used)s used)"
 msgstr ""
 
-#: panels/staticfiles.py:106
+#: panels/staticfiles.py:105
 msgid "Static files"
 msgstr "فایل های استاتیک"
 
-#: panels/staticfiles.py:112
+#: panels/staticfiles.py:111
 #, python-format
 msgid "%(num_used)s file used"
 msgid_plural "%(num_used)s files used"
 msgstr[0] ""
 msgstr[1] ""
 
-#: panels/templates/panel.py:144
+#: panels/templates/panel.py:143
 msgid "Templates"
 msgstr "تمپلیت ها"
 
-#: panels/templates/panel.py:149
+#: panels/templates/panel.py:148
 #, python-format
 msgid "Templates (%(num_templates)s rendered)"
 msgstr "تمپلیت ها (%(num_templates)s rendered)"
 
-#: panels/templates/panel.py:181
+#: panels/templates/panel.py:180
 msgid "No origin"
 msgstr "بدون origin"
 
 #: panels/timer.py:25
 #, python-format
 msgid "CPU: %(cum)0.2fms (%(total)0.2fms)"
 msgstr ""
 
 #: panels/timer.py:30
 #, python-format
 msgid "Total: %0.2fms"
 msgstr ""
 
 #: panels/timer.py:36 templates/debug_toolbar/panels/history.html:9
-#: templates/debug_toolbar/panels/logging.html:7
 #: templates/debug_toolbar/panels/sql_explain.html:11
 #: templates/debug_toolbar/panels/sql_profile.html:12
 #: templates/debug_toolbar/panels/sql_select.html:11
 msgid "Time"
 msgstr "زمان"
 
 #: panels/timer.py:44
@@ -260,23 +245,23 @@
 msgid "%(vcsw)d voluntary, %(ivcsw)d involuntary"
 msgstr ""
 
 #: panels/versions.py:19
 msgid "Versions"
 msgstr "ورژن ها"
 
-#: templates/debug_toolbar/base.html:18
+#: templates/debug_toolbar/base.html:22
 msgid "Hide toolbar"
 msgstr "پنهان کردن toolbar"
 
-#: templates/debug_toolbar/base.html:18
+#: templates/debug_toolbar/base.html:22
 msgid "Hide"
 msgstr "پنهان کردن"
 
-#: templates/debug_toolbar/base.html:25
+#: templates/debug_toolbar/base.html:29
 msgid "Show toolbar"
 msgstr "نمایش toolbar"
 
 #: templates/debug_toolbar/includes/panel_button.html:4
 msgid "Disable for next and successive requests"
 msgstr "غیر فعال کردن برای ریکوئست های پی در پی"
 
@@ -298,15 +283,17 @@
 
 #: templates/debug_toolbar/panels/cache.html:8
 msgid "Cache hits"
 msgstr "Cache hits"
 
 #: templates/debug_toolbar/panels/cache.html:9
 msgid "Cache misses"
-msgstr "Cache misses\n "
+msgstr ""
+"Cache misses\n"
+" "
 
 #: templates/debug_toolbar/panels/cache.html:21
 msgid "Commands"
 msgstr "دستورات"
 
 #: templates/debug_toolbar/panels/cache.html:39
 msgid "Calls"
@@ -345,15 +332,15 @@
 msgid "Key"
 msgstr "کلید"
 
 #: templates/debug_toolbar/panels/headers.html:9
 #: templates/debug_toolbar/panels/headers.html:28
 #: templates/debug_toolbar/panels/headers.html:49
 #: templates/debug_toolbar/panels/history_tr.html:23
-#: templates/debug_toolbar/panels/request_variables.html:11
+#: templates/debug_toolbar/panels/request_variables.html:12
 #: templates/debug_toolbar/panels/settings.html:6
 #: templates/debug_toolbar/panels/timer.html:11
 msgid "Value"
 msgstr "مقدار"
 
 #: templates/debug_toolbar/panels/headers.html:22
 msgid "Response headers"
@@ -363,15 +350,17 @@
 msgid "WSGI environ"
 msgstr "محیط WSGI"
 
 #: templates/debug_toolbar/panels/headers.html:43
 msgid ""
 "Since the WSGI environ inherits the environment of the server, only a "
 "significant subset is shown below."
-msgstr "از آنجا که محیط WSGI محیط سرور را به ارث می برد ، فقط یک زیر مجموعه مهم در زیر نشان داده شده است."
+msgstr ""
+"از آنجا که محیط WSGI محیط سرور را به ارث می برد ، فقط یک زیر مجموعه مهم در "
+"زیر نشان داده شده است."
 
 #: templates/debug_toolbar/panels/history.html:10
 msgid "Method"
 msgstr "متد"
 
 #: templates/debug_toolbar/panels/history.html:11
 #: templates/debug_toolbar/panels/staticfiles.html:43
@@ -388,39 +377,18 @@
 
 #: templates/debug_toolbar/panels/history.html:14
 #: templates/debug_toolbar/panels/sql.html:37
 msgid "Action"
 msgstr "اکشن"
 
 #: templates/debug_toolbar/panels/history_tr.html:22
-#: templates/debug_toolbar/panels/request_variables.html:10
+#: templates/debug_toolbar/panels/request_variables.html:11
 msgid "Variable"
 msgstr "متغیر"
 
-#: templates/debug_toolbar/panels/logging.html:6
-msgid "Level"
-msgstr "سطح"
-
-#: templates/debug_toolbar/panels/logging.html:8
-msgid "Channel"
-msgstr "کانال"
-
-#: templates/debug_toolbar/panels/logging.html:9
-msgid "Message"
-msgstr "پیام"
-
-#: templates/debug_toolbar/panels/logging.html:10
-#: templates/debug_toolbar/panels/staticfiles.html:44
-msgid "Location"
-msgstr "مکان"
-
-#: templates/debug_toolbar/panels/logging.html:26
-msgid "No messages logged"
-msgstr "پیامی لاگ نشده"
-
 #: templates/debug_toolbar/panels/profiling.html:5
 msgid "Call"
 msgstr "Call"
 
 #: templates/debug_toolbar/panels/profiling.html:6
 msgid "CumTime"
 msgstr ""
@@ -621,14 +589,18 @@
 #: templates/debug_toolbar/panels/staticfiles.html:39
 #, python-format
 msgid "%(payload_count)s file"
 msgid_plural "%(payload_count)s files"
 msgstr[0] ""
 msgstr[1] ""
 
+#: templates/debug_toolbar/panels/staticfiles.html:44
+msgid "Location"
+msgstr "مکان"
+
 #: templates/debug_toolbar/panels/template_source.html:4
 msgid "Template source:"
 msgstr "منبع تمپلیت:"
 
 #: templates/debug_toolbar/panels/templates.html:2
 msgid "Template path"
 msgid_plural "Template paths"
@@ -691,12 +663,12 @@
 #: templates/debug_toolbar/redirect.html:12
 msgid ""
 "The Django Debug Toolbar has intercepted a redirect to the above URL for "
 "debug viewing purposes. You can click the above link to continue with the "
 "redirect as normal."
 msgstr ""
 
-#: views.py:15
+#: views.py:16
 msgid ""
 "Data for this panel isn't available anymore. Please reload the page and "
 "retry."
 msgstr "دیتا برای نمایش در دسترس نیست. لطفا صفحه را ریفرش کنید."
```

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/locale/fi/LC_MESSAGES/django.mo` & `django_debug_toolbar-4.0.0/debug_toolbar/locale/fi/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/locale/fi/LC_MESSAGES/django.po` & `django_debug_toolbar-4.0.0/debug_toolbar/locale/id/LC_MESSAGES/django.po`

 * *Files 11% similar despite different names*

```diff
@@ -1,289 +1,270 @@
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 #
 #
 # Translators:
-# nanook <klaus.dahlen@gmail.com>, 2012
+# Muhammad Panji <sumodirjo@gmail.com>, 2012
 msgid ""
 msgstr ""
 "Project-Id-Version: Django Debug Toolbar\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2014-04-25 21:52+0200\n"
+"POT-Creation-Date: 2023-01-20 17:23+0100\n"
 "PO-Revision-Date: 2014-04-25 19:53+0000\n"
 "Last-Translator: Aymeric Augustin <aymeric.augustin@m4x.org>\n"
-"Language-Team: Finnish (http://www.transifex.com/projects/p/django-debug-toolbar/language/fi/)\n"
+"Language-Team: Indonesian (http://www.transifex.com/projects/p/django-debug-"
+"toolbar/language/id/)\n"
+"Language: id\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: fi\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 
-#: apps.py:11
+#: apps.py:15
 msgid "Debug Toolbar"
 msgstr ""
 
-#: views.py:14
-msgid ""
-"Data for this panel isn't available anymore. Please reload the page and "
-"retry."
-msgstr ""
-
-#: panels/cache.py:191
+#: panels/cache.py:180
 msgid "Cache"
-msgstr "Välimuisti"
+msgstr ""
 
-#: panels/cache.py:196
+#: panels/cache.py:186
 #, python-format
 msgid "%(cache_calls)d call in %(time).2fms"
 msgid_plural "%(cache_calls)d calls in %(time).2fms"
-msgstr[0] "%(cache_calls)d kutsu %(time).2fms"
-msgstr[1] "%(cache_calls)d kutsua %(time).2fms"
+msgstr[0] ""
 
-#: panels/cache.py:204
+#: panels/cache.py:195
 #, python-format
 msgid "Cache calls from %(count)d backend"
 msgid_plural "Cache calls from %(count)d backends"
 msgstr[0] ""
-msgstr[1] ""
 
-#: panels/headers.py:35
+#: panels/headers.py:31
 msgid "Headers"
 msgstr ""
 
-#: panels/logging.py:64
-msgid "Logging"
-msgstr "Loki"
-
-#: panels/logging.py:70
-#, python-format
-msgid "%(count)s message"
-msgid_plural "%(count)s messages"
-msgstr[0] "%(count)s viesti"
-msgstr[1] "%(count)s viestiä"
-
-#: panels/logging.py:73
-msgid "Log messages"
+#: panels/history/panel.py:18 panels/history/panel.py:19
+msgid "History"
 msgstr ""
 
-#: panels/profiling.py:127
+#: panels/profiling.py:140
 msgid "Profiling"
-msgstr "Profilointi"
+msgstr ""
 
-#: panels/redirects.py:17
+#: panels/redirects.py:14
 msgid "Intercept redirects"
 msgstr ""
 
-#: panels/request.py:18
+#: panels/request.py:16
 msgid "Request"
 msgstr ""
 
-#: panels/request.py:35
+#: panels/request.py:36
 msgid "<no view>"
 msgstr ""
 
-#: panels/request.py:47
+#: panels/request.py:53
 msgid "<unavailable>"
 msgstr ""
 
-#: panels/settings.py:20
+#: panels/settings.py:17
 msgid "Settings"
-msgstr "Asetukset"
+msgstr "Pengaturan"
 
-#: panels/settings.py:23
-#, python-format
-msgid "Settings from <code>%s</code>"
-msgstr "Asetukset tiedostosta <code>%s</code>"
+#: panels/settings.py:20
+#, fuzzy, python-format
+#| msgid "Settings from <code>%s</code>"
+msgid "Settings from %s"
+msgstr "Pengaturan dari <code>%s</code>"
 
-#: panels/signals.py:45
+#: panels/signals.py:57
 #, python-format
 msgid "%(num_receivers)d receiver of 1 signal"
 msgid_plural "%(num_receivers)d receivers of 1 signal"
-msgstr[0] "%(num_receivers)d vastaanotin 1 signaalille"
-msgstr[1] "%(num_receivers)d vastaanotinta 1 signaalille"
+msgstr[0] ""
 
-#: panels/signals.py:48
+#: panels/signals.py:62
 #, python-format
 msgid "%(num_receivers)d receiver of %(num_signals)d signals"
 msgid_plural "%(num_receivers)d receivers of %(num_signals)d signals"
-msgstr[0] "%(num_receivers)d vastaanotin %(num_signals)d signaalille"
-msgstr[1] "%(num_receivers)d vastaanotinta %(num_signals)d signaalille"
+msgstr[0] ""
 
-#: panels/signals.py:53
+#: panels/signals.py:67
 msgid "Signals"
-msgstr "Signaalit"
+msgstr "Sinyal"
+
+#: panels/sql/panel.py:23
+msgid "Autocommit"
+msgstr ""
+
+#: panels/sql/panel.py:24
+msgid "Read uncommitted"
+msgstr ""
+
+#: panels/sql/panel.py:25
+msgid "Read committed"
+msgstr ""
+
+#: panels/sql/panel.py:26
+msgid "Repeatable read"
+msgstr ""
+
+#: panels/sql/panel.py:27
+msgid "Serializable"
+msgstr "Variabel"
+
+#: panels/sql/panel.py:39
+msgid "Idle"
+msgstr ""
+
+#: panels/sql/panel.py:40
+msgid "Active"
+msgstr "Aksi"
+
+#: panels/sql/panel.py:41
+msgid "In transaction"
+msgstr "Status transaksi:"
+
+#: panels/sql/panel.py:42
+msgid "In error"
+msgstr ""
+
+#: panels/sql/panel.py:43
+msgid "Unknown"
+msgstr "(tidak diketahui)"
+
+#: panels/sql/panel.py:130
+msgid "SQL"
+msgstr "SQL"
+
+#: panels/sql/panel.py:135
+#, python-format
+msgid "%(query_count)d query in %(sql_time).2fms"
+msgid_plural "%(query_count)d queries in %(sql_time).2fms"
+msgstr[0] ""
+
+#: panels/sql/panel.py:147
+#, python-format
+msgid "SQL queries from %(count)d connection"
+msgid_plural "SQL queries from %(count)d connections"
+msgstr[0] ""
 
-#: panels/staticfiles.py:89
+#: panels/staticfiles.py:84
 #, python-format
 msgid "Static files (%(num_found)s found, %(num_used)s used)"
 msgstr ""
 
-#: panels/staticfiles.py:107
+#: panels/staticfiles.py:105
 msgid "Static files"
-msgstr "Staattiset tiedostot"
+msgstr "Berkas statik"
 
-#: panels/staticfiles.py:112
+#: panels/staticfiles.py:111
 #, python-format
 msgid "%(num_used)s file used"
 msgid_plural "%(num_used)s files used"
 msgstr[0] ""
-msgstr[1] ""
 
-#: panels/timer.py:23
+#: panels/templates/panel.py:143
+msgid "Templates"
+msgstr "Template"
+
+#: panels/templates/panel.py:148
+#, python-format
+msgid "Templates (%(num_templates)s rendered)"
+msgstr ""
+
+#: panels/templates/panel.py:180
+msgid "No origin"
+msgstr ""
+
+#: panels/timer.py:25
 #, python-format
 msgid "CPU: %(cum)0.2fms (%(total)0.2fms)"
 msgstr "CPU: %(cum)0.2fms (%(total)0.2fms)"
 
-#: panels/timer.py:28
+#: panels/timer.py:30
 #, python-format
 msgid "Total: %0.2fms"
 msgstr ""
 
-#: panels/timer.py:34 templates/debug_toolbar/panels/logging.html:7
+#: panels/timer.py:36 templates/debug_toolbar/panels/history.html:9
 #: templates/debug_toolbar/panels/sql_explain.html:11
 #: templates/debug_toolbar/panels/sql_profile.html:12
 #: templates/debug_toolbar/panels/sql_select.html:11
 msgid "Time"
-msgstr "Aika"
+msgstr "Waktu"
 
-#: panels/timer.py:42
+#: panels/timer.py:44
 msgid "User CPU time"
-msgstr "Käyttäjän CPU-aika"
+msgstr "CPU time pengguna"
 
-#: panels/timer.py:42
+#: panels/timer.py:44
 #, python-format
 msgid "%(utime)0.3f msec"
-msgstr "%(utime)0.3f msek"
+msgstr ""
 
-#: panels/timer.py:43
+#: panels/timer.py:45
 msgid "System CPU time"
-msgstr "Järjestelmän CPU-aika"
+msgstr "CPU time sistem"
 
-#: panels/timer.py:43
+#: panels/timer.py:45
 #, python-format
 msgid "%(stime)0.3f msec"
-msgstr "%(stime)0.3f msek"
+msgstr ""
 
-#: panels/timer.py:44
+#: panels/timer.py:46
 msgid "Total CPU time"
-msgstr "CPU-aika yhteensä"
+msgstr "CPU time total"
 
-#: panels/timer.py:44
+#: panels/timer.py:46
 #, python-format
 msgid "%(total)0.3f msec"
-msgstr "%(total)0.3f msek"
+msgstr ""
 
-#: panels/timer.py:45
+#: panels/timer.py:47
 msgid "Elapsed time"
-msgstr "Kulunut aika"
+msgstr "Waktu terlampaui"
 
-#: panels/timer.py:45
+#: panels/timer.py:47
 #, python-format
 msgid "%(total_time)0.3f msec"
-msgstr "%(total_time)0.3f msek"
+msgstr ""
 
-#: panels/timer.py:46
+#: panels/timer.py:49
 msgid "Context switches"
-msgstr "Kontekstin vivut"
+msgstr ""
 
-#: panels/timer.py:46
+#: panels/timer.py:50
 #, python-format
 msgid "%(vcsw)d voluntary, %(ivcsw)d involuntary"
 msgstr ""
 
-#: panels/versions.py:25
+#: panels/versions.py:19
 msgid "Versions"
-msgstr "Versiot"
-
-#: panels/sql/panel.py:22
-msgid "Autocommit"
-msgstr "Autocommit"
-
-#: panels/sql/panel.py:23
-msgid "Read uncommitted"
-msgstr ""
-
-#: panels/sql/panel.py:24
-msgid "Read committed"
-msgstr ""
-
-#: panels/sql/panel.py:25
-msgid "Repeatable read"
-msgstr ""
-
-#: panels/sql/panel.py:26
-msgid "Serializable"
-msgstr "Muuttuja"
-
-#: panels/sql/panel.py:37
-msgid "Idle"
-msgstr ""
-
-#: panels/sql/panel.py:38
-msgid "Active"
-msgstr "Tapahtuma"
-
-#: panels/sql/panel.py:39
-msgid "In transaction"
-msgstr "Tapahtuman tila:"
-
-#: panels/sql/panel.py:40
-msgid "In error"
-msgstr "Virhe"
-
-#: panels/sql/panel.py:41
-msgid "Unknown"
-msgstr "(tuntematon)"
-
-#: panels/sql/panel.py:105
-msgid "SQL"
-msgstr "SQL"
-
-#: panels/templates/panel.py:141
-msgid "Templates"
-msgstr "Asettelupohjat"
-
-#: panels/templates/panel.py:146
-#, python-format
-msgid "Templates (%(num_templates)s rendered)"
-msgstr "Asetttelupohjat (%(num_templates)s renderöity)"
+msgstr "Versi"
 
-#: templates/debug_toolbar/base.html:19
+#: templates/debug_toolbar/base.html:22
 msgid "Hide toolbar"
 msgstr ""
 
-#: templates/debug_toolbar/base.html:19
+#: templates/debug_toolbar/base.html:22
 msgid "Hide"
-msgstr "Piilota"
-
-#: templates/debug_toolbar/base.html:25
-msgid "Disable for next and successive requests"
-msgstr ""
-
-#: templates/debug_toolbar/base.html:25
-msgid "Enable for next and successive requests"
-msgstr ""
+msgstr "Menyembunyikan"
 
-#: templates/debug_toolbar/base.html:47
+#: templates/debug_toolbar/base.html:29
 msgid "Show toolbar"
 msgstr ""
 
-#: templates/debug_toolbar/base.html:53
-msgid "Close"
-msgstr "Sulje"
-
-#: templates/debug_toolbar/redirect.html:8
-msgid "Location:"
+#: templates/debug_toolbar/includes/panel_button.html:4
+msgid "Disable for next and successive requests"
 msgstr ""
 
-#: templates/debug_toolbar/redirect.html:10
-msgid ""
-"The Django Debug Toolbar has intercepted a redirect to the above URL for "
-"debug viewing purposes. You can click the above link to continue with the "
-"redirect as normal."
+#: templates/debug_toolbar/includes/panel_button.html:4
+msgid "Enable for next and successive requests"
 msgstr ""
 
 #: templates/debug_toolbar/panels/cache.html:2
 msgid "Summary"
 msgstr ""
 
 #: templates/debug_toolbar/panels/cache.html:6
@@ -307,21 +288,21 @@
 msgstr ""
 
 #: templates/debug_toolbar/panels/cache.html:39
 msgid "Calls"
 msgstr ""
 
 #: templates/debug_toolbar/panels/cache.html:43
-#: templates/debug_toolbar/panels/sql.html:20
+#: templates/debug_toolbar/panels/sql.html:36
 msgid "Time (ms)"
-msgstr "Aika (ms)"
+msgstr "Waktu (milidetik)"
 
 #: templates/debug_toolbar/panels/cache.html:44
 msgid "Type"
-msgstr "Tyyppi"
+msgstr "Jenis"
 
 #: templates/debug_toolbar/panels/cache.html:45
 #: templates/debug_toolbar/panels/request.html:8
 msgid "Arguments"
 msgstr ""
 
 #: templates/debug_toolbar/panels/cache.html:46
@@ -337,27 +318,25 @@
 msgid "Request headers"
 msgstr ""
 
 #: templates/debug_toolbar/panels/headers.html:8
 #: templates/debug_toolbar/panels/headers.html:27
 #: templates/debug_toolbar/panels/headers.html:48
 msgid "Key"
-msgstr "Avain"
+msgstr "Kunci"
 
 #: templates/debug_toolbar/panels/headers.html:9
 #: templates/debug_toolbar/panels/headers.html:28
 #: templates/debug_toolbar/panels/headers.html:49
-#: templates/debug_toolbar/panels/request.html:33
-#: templates/debug_toolbar/panels/request.html:59
-#: templates/debug_toolbar/panels/request.html:85
-#: templates/debug_toolbar/panels/request.html:110
+#: templates/debug_toolbar/panels/history_tr.html:23
+#: templates/debug_toolbar/panels/request_variables.html:12
 #: templates/debug_toolbar/panels/settings.html:6
 #: templates/debug_toolbar/panels/timer.html:11
 msgid "Value"
-msgstr "Arvo"
+msgstr "Nilai"
 
 #: templates/debug_toolbar/panels/headers.html:22
 msgid "Response headers"
 msgstr ""
 
 #: templates/debug_toolbar/panels/headers.html:41
 msgid "WSGI environ"
@@ -365,292 +344,317 @@
 
 #: templates/debug_toolbar/panels/headers.html:43
 msgid ""
 "Since the WSGI environ inherits the environment of the server, only a "
 "significant subset is shown below."
 msgstr ""
 
-#: templates/debug_toolbar/panels/logging.html:6
-msgid "Level"
-msgstr "Taso"
-
-#: templates/debug_toolbar/panels/logging.html:8
-msgid "Channel"
-msgstr "Kanava"
-
-#: templates/debug_toolbar/panels/logging.html:9
-msgid "Message"
-msgstr "Viesti"
+#: templates/debug_toolbar/panels/history.html:10
+msgid "Method"
+msgstr ""
+
+#: templates/debug_toolbar/panels/history.html:11
+#: templates/debug_toolbar/panels/staticfiles.html:43
+msgid "Path"
+msgstr ""
+
+#: templates/debug_toolbar/panels/history.html:12
+#, fuzzy
+#| msgid "Variable"
+msgid "Request Variables"
+msgstr "Variabel"
 
-#: templates/debug_toolbar/panels/logging.html:10
-#: templates/debug_toolbar/panels/staticfiles.html:45
-msgid "Location"
-msgstr "Sijainti"
+#: templates/debug_toolbar/panels/history.html:13
+msgid "Status"
+msgstr ""
 
-#: templates/debug_toolbar/panels/logging.html:26
-msgid "No messages logged"
-msgstr "Ei viestejä lokissa"
+#: templates/debug_toolbar/panels/history.html:14
+#: templates/debug_toolbar/panels/sql.html:37
+msgid "Action"
+msgstr "Aksi"
+
+#: templates/debug_toolbar/panels/history_tr.html:22
+#: templates/debug_toolbar/panels/request_variables.html:11
+msgid "Variable"
+msgstr "Variabel"
 
 #: templates/debug_toolbar/panels/profiling.html:5
 msgid "Call"
-msgstr "Kutsu"
+msgstr "Panggil"
 
 #: templates/debug_toolbar/panels/profiling.html:6
 msgid "CumTime"
 msgstr "CumTime"
 
 #: templates/debug_toolbar/panels/profiling.html:7
 #: templates/debug_toolbar/panels/profiling.html:9
 msgid "Per"
-msgstr "/"
+msgstr "Per"
 
 #: templates/debug_toolbar/panels/profiling.html:8
 msgid "TotTime"
 msgstr "TotTime"
 
 #: templates/debug_toolbar/panels/profiling.html:10
 msgid "Count"
-msgstr "Määrä"
+msgstr "Hitung"
 
 #: templates/debug_toolbar/panels/request.html:3
 msgid "View information"
-msgstr "Näkymän tiedot"
+msgstr "Lihat informasi"
 
 #: templates/debug_toolbar/panels/request.html:7
 msgid "View function"
 msgstr ""
 
 #: templates/debug_toolbar/panels/request.html:10
 msgid "URL name"
 msgstr ""
 
 #: templates/debug_toolbar/panels/request.html:24
 msgid "Cookies"
 msgstr ""
 
-#: templates/debug_toolbar/panels/request.html:32
-#: templates/debug_toolbar/panels/request.html:58
-#: templates/debug_toolbar/panels/request.html:84
-#: templates/debug_toolbar/panels/request.html:109
-msgid "Variable"
-msgstr "Muuttuja"
-
-#: templates/debug_toolbar/panels/request.html:46
+#: templates/debug_toolbar/panels/request.html:27
 msgid "No cookies"
 msgstr ""
 
-#: templates/debug_toolbar/panels/request.html:50
+#: templates/debug_toolbar/panels/request.html:31
 msgid "Session data"
 msgstr ""
 
-#: templates/debug_toolbar/panels/request.html:72
+#: templates/debug_toolbar/panels/request.html:34
 msgid "No session data"
 msgstr ""
 
-#: templates/debug_toolbar/panels/request.html:76
+#: templates/debug_toolbar/panels/request.html:38
 msgid "GET data"
 msgstr ""
 
-#: templates/debug_toolbar/panels/request.html:98
+#: templates/debug_toolbar/panels/request.html:41
 msgid "No GET data"
-msgstr "Ei GET-dataa"
+msgstr "Tidak ada data GET"
 
-#: templates/debug_toolbar/panels/request.html:102
+#: templates/debug_toolbar/panels/request.html:45
 msgid "POST data"
 msgstr ""
 
-#: templates/debug_toolbar/panels/request.html:123
+#: templates/debug_toolbar/panels/request.html:48
 msgid "No POST data"
-msgstr "Ei POST-dataa"
+msgstr "Tidak ada data POST"
 
 #: templates/debug_toolbar/panels/settings.html:5
 msgid "Setting"
-msgstr "Asetus"
+msgstr "Pengaturan"
 
 #: templates/debug_toolbar/panels/signals.html:5
 msgid "Signal"
-msgstr "Signaali"
+msgstr "Sinyal"
 
 #: templates/debug_toolbar/panels/signals.html:6
-msgid "Providing"
-msgstr ""
-
-#: templates/debug_toolbar/panels/signals.html:7
 msgid "Receivers"
-msgstr "Vastaanottimet"
+msgstr "Penerima"
 
-#: templates/debug_toolbar/panels/sql.html:7
+#: templates/debug_toolbar/panels/sql.html:6
 #, python-format
 msgid "%(num)s query"
 msgid_plural "%(num)s queries"
-msgstr[0] "%(num)s kysely"
-msgstr[1] "%(num)s kyselyä"
+msgstr[0] ""
+
+#: templates/debug_toolbar/panels/sql.html:8
+#, python-format
+msgid ""
+"including <abbr title=\"Similar queries are queries with the same SQL, but "
+"potentially different parameters.\">%(count)s similar</abbr>"
+msgstr ""
 
-#: templates/debug_toolbar/panels/sql.html:18
+#: templates/debug_toolbar/panels/sql.html:12
+#, python-format
+msgid ""
+"and <abbr title=\"Duplicate queries are identical to each other: they "
+"execute exactly the same SQL and parameters.\">%(dupes)s duplicates</abbr>"
+msgstr ""
+
+#: templates/debug_toolbar/panels/sql.html:34
 msgid "Query"
-msgstr "Kysely"
+msgstr ""
 
-#: templates/debug_toolbar/panels/sql.html:19
+#: templates/debug_toolbar/panels/sql.html:35
 #: templates/debug_toolbar/panels/timer.html:36
 msgid "Timeline"
-msgstr "Aikajana"
+msgstr ""
 
-#: templates/debug_toolbar/panels/sql.html:21
-msgid "Action"
-msgstr "Tapahtuma"
+#: templates/debug_toolbar/panels/sql.html:52
+#, fuzzy, python-format
+#| msgid "%(count)s message"
+#| msgid_plural "%(count)s messages"
+msgid "%(count)s similar queries."
+msgstr "%(count)s pesan"
+
+#: templates/debug_toolbar/panels/sql.html:58
+#, python-format
+msgid "Duplicated %(dupes)s times."
+msgstr ""
 
-#: templates/debug_toolbar/panels/sql.html:64
+#: templates/debug_toolbar/panels/sql.html:95
 msgid "Connection:"
-msgstr "Yhteys:"
+msgstr "Koneksi:"
 
-#: templates/debug_toolbar/panels/sql.html:66
+#: templates/debug_toolbar/panels/sql.html:97
 msgid "Isolation level:"
-msgstr "Eristystaso:"
+msgstr "Tingkat isolasi:"
 
-#: templates/debug_toolbar/panels/sql.html:69
+#: templates/debug_toolbar/panels/sql.html:100
 msgid "Transaction status:"
-msgstr "Tapahtuman status:"
+msgstr "Status transaksi:"
 
-#: templates/debug_toolbar/panels/sql.html:83
+#: templates/debug_toolbar/panels/sql.html:114
 msgid "(unknown)"
-msgstr "(tuntematon)"
+msgstr "(tidak diketahui)"
 
-#: templates/debug_toolbar/panels/sql.html:92
+#: templates/debug_toolbar/panels/sql.html:123
 msgid "No SQL queries were recorded during this request."
-msgstr "Tämän pyynnön aikana ei tehty yhtään SQL-kyselyä."
-
-#: templates/debug_toolbar/panels/sql_explain.html:3
-#: templates/debug_toolbar/panels/sql_profile.html:3
-#: templates/debug_toolbar/panels/sql_select.html:3
-#: templates/debug_toolbar/panels/template_source.html:3
-msgid "Back"
-msgstr "Takaisin"
+msgstr ""
 
 #: templates/debug_toolbar/panels/sql_explain.html:4
 msgid "SQL explained"
 msgstr ""
 
 #: templates/debug_toolbar/panels/sql_explain.html:9
 #: templates/debug_toolbar/panels/sql_profile.html:10
 #: templates/debug_toolbar/panels/sql_select.html:9
 msgid "Executed SQL"
-msgstr "Suoritettu SQL"
+msgstr "SQL Tereksekusi"
 
 #: templates/debug_toolbar/panels/sql_explain.html:13
 #: templates/debug_toolbar/panels/sql_profile.html:14
 #: templates/debug_toolbar/panels/sql_select.html:13
 msgid "Database"
-msgstr "Tietokanta"
+msgstr "Basis data"
 
 #: templates/debug_toolbar/panels/sql_profile.html:4
 msgid "SQL profiled"
 msgstr ""
 
 #: templates/debug_toolbar/panels/sql_profile.html:37
 msgid "Error"
-msgstr "Virhe"
+msgstr ""
 
 #: templates/debug_toolbar/panels/sql_select.html:4
 msgid "SQL selected"
 msgstr ""
 
 #: templates/debug_toolbar/panels/sql_select.html:36
 msgid "Empty set"
-msgstr "Tyhjä joukko"
+msgstr "Himpunan kosong"
 
-#: templates/debug_toolbar/panels/staticfiles.html:4
+#: templates/debug_toolbar/panels/staticfiles.html:3
 msgid "Static file path"
 msgid_plural "Static file paths"
 msgstr[0] ""
-msgstr[1] ""
 
-#: templates/debug_toolbar/panels/staticfiles.html:8
+#: templates/debug_toolbar/panels/staticfiles.html:7
 #, python-format
 msgid "(prefix %(prefix)s)"
 msgstr ""
 
-#: templates/debug_toolbar/panels/staticfiles.html:12
-#: templates/debug_toolbar/panels/staticfiles.html:23
-#: templates/debug_toolbar/panels/staticfiles.html:35
+#: templates/debug_toolbar/panels/staticfiles.html:11
+#: templates/debug_toolbar/panels/staticfiles.html:22
+#: templates/debug_toolbar/panels/staticfiles.html:34
 #: templates/debug_toolbar/panels/templates.html:10
-#: templates/debug_toolbar/panels/templates.html:28
-#: templates/debug_toolbar/panels/templates.html:43
+#: templates/debug_toolbar/panels/templates.html:30
+#: templates/debug_toolbar/panels/templates.html:47
 msgid "None"
-msgstr "None"
+msgstr "Tidak ada"
 
-#: templates/debug_toolbar/panels/staticfiles.html:15
+#: templates/debug_toolbar/panels/staticfiles.html:14
 msgid "Static file app"
 msgid_plural "Static file apps"
 msgstr[0] ""
-msgstr[1] ""
 
-#: templates/debug_toolbar/panels/staticfiles.html:26
+#: templates/debug_toolbar/panels/staticfiles.html:25
 msgid "Static file"
 msgid_plural "Static files"
-msgstr[0] ""
-msgstr[1] "Staattiset tiedostot"
+msgstr[0] "Berkas statik"
 
-#: templates/debug_toolbar/panels/staticfiles.html:40
+#: templates/debug_toolbar/panels/staticfiles.html:39
 #, python-format
 msgid "%(payload_count)s file"
 msgid_plural "%(payload_count)s files"
 msgstr[0] ""
-msgstr[1] ""
 
 #: templates/debug_toolbar/panels/staticfiles.html:44
-msgid "Path"
-msgstr "Polku"
+msgid "Location"
+msgstr "Lokasi"
 
 #: templates/debug_toolbar/panels/template_source.html:4
 msgid "Template source:"
 msgstr ""
 
 #: templates/debug_toolbar/panels/templates.html:2
 msgid "Template path"
 msgid_plural "Template paths"
-msgstr[0] "Sivupohjan polku"
-msgstr[1] "Sivupohjan polku"
+msgstr[0] "Template path"
 
 #: templates/debug_toolbar/panels/templates.html:13
 msgid "Template"
 msgid_plural "Templates"
-msgstr[0] "Sivupohja"
-msgstr[1] "Sivupohja"
+msgstr[0] ""
 
-#: templates/debug_toolbar/panels/templates.html:21
-#: templates/debug_toolbar/panels/templates.html:37
+#: templates/debug_toolbar/panels/templates.html:22
+#: templates/debug_toolbar/panels/templates.html:40
 msgid "Toggle context"
 msgstr ""
 
-#: templates/debug_toolbar/panels/templates.html:31
+#: templates/debug_toolbar/panels/templates.html:33
 msgid "Context processor"
 msgid_plural "Context processors"
-msgstr[0] "Kontekstiprosessori"
-msgstr[1] "Kontekstiprosessori"
+msgstr[0] ""
 
 #: templates/debug_toolbar/panels/timer.html:2
 msgid "Resource usage"
 msgstr ""
 
 #: templates/debug_toolbar/panels/timer.html:10
 msgid "Resource"
-msgstr "Resurssi"
+msgstr "Sumber daya"
 
 #: templates/debug_toolbar/panels/timer.html:26
 msgid "Browser timing"
 msgstr ""
 
 #: templates/debug_toolbar/panels/timer.html:35
 msgid "Timing attribute"
 msgstr ""
 
 #: templates/debug_toolbar/panels/timer.html:37
 msgid "Milliseconds since navigation start (+length)"
 msgstr ""
 
-#: templates/debug_toolbar/panels/versions.html:5
+#: templates/debug_toolbar/panels/versions.html:10
+msgid "Package"
+msgstr ""
+
+#: templates/debug_toolbar/panels/versions.html:11
 msgid "Name"
-msgstr "Nimi"
+msgstr ""
 
-#: templates/debug_toolbar/panels/versions.html:6
+#: templates/debug_toolbar/panels/versions.html:12
 msgid "Version"
-msgstr "Versio"
+msgstr "Versi"
+
+#: templates/debug_toolbar/redirect.html:10
+msgid "Location:"
+msgstr ""
+
+#: templates/debug_toolbar/redirect.html:12
+msgid ""
+"The Django Debug Toolbar has intercepted a redirect to the above URL for "
+"debug viewing purposes. You can click the above link to continue with the "
+"redirect as normal."
+msgstr ""
+
+#: views.py:16
+msgid ""
+"Data for this panel isn't available anymore. Please reload the page and "
+"retry."
+msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/locale/fr/LC_MESSAGES/django.mo` & `django_debug_toolbar-4.0.0/debug_toolbar/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/locale/fr/LC_MESSAGES/django.po` & `django_debug_toolbar-4.0.0/debug_toolbar/locale/de/LC_MESSAGES/django.po`

 * *Files 4% similar despite different names*

```diff
@@ -1,708 +1,682 @@
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 #
 #
 # Translators:
-# Anthony Jorion <pingax@gmail.com>, 2013
-# Aymeric Augustin <aymeric.augustin@m4x.org>, 2014
-# Claude Paroz <claude@2xlibre.net>, 2013
-# Colin O'Brien <colin@things.be>, 2021
-# David Paccoud, 2009
-# Dominick Rivard <dominick.rivard@gmail.com>, 2013
-# Maxime Abry <maxime.abry@critizr.com>, 2016
+# Jannis Leidel <jannis@leidel.info>, 2012-2014,2021
+# Matthias Kestenholz <mk@feinheit.ch>, 2021
 msgid ""
 msgstr ""
 "Project-Id-Version: Django Debug Toolbar\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-08-14 10:25-0500\n"
-"PO-Revision-Date: 2021-09-30 09:21+0000\n"
-"Last-Translator: Colin O'Brien <colin@things.be>\n"
-"Language-Team: French (http://www.transifex.com/django-debug-toolbar/django-debug-toolbar/language/fr/)\n"
+"POT-Creation-Date: 2023-01-20 17:23+0100\n"
+"PO-Revision-Date: 2021-12-04 17:38+0000\n"
+"Last-Translator: Tim Schilling\n"
+"Language-Team: German (http://www.transifex.com/django-debug-toolbar/django-"
+"debug-toolbar/language/de/)\n"
+"Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: fr\n"
-"Plural-Forms: nplurals=2; plural=(n > 1);\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: apps.py:15
 msgid "Debug Toolbar"
-msgstr "Barre d'outils de débogage"
+msgstr "Debug Toolbar"
 
-#: panels/cache.py:227
+#: panels/cache.py:180
 msgid "Cache"
 msgstr "Cache"
 
-#: panels/cache.py:234
+#: panels/cache.py:186
 #, python-format
 msgid "%(cache_calls)d call in %(time).2fms"
 msgid_plural "%(cache_calls)d calls in %(time).2fms"
-msgstr[0] "%(cache_calls)d appel en %(time).2fms"
-msgstr[1] "%(cache_calls)d appels en %(time).2fms"
+msgstr[0] "%(cache_calls)d Abfrage in %(time).2fms"
+msgstr[1] "%(cache_calls)d Abfragen in %(time).2fms"
 
-#: panels/cache.py:246
+#: panels/cache.py:195
 #, python-format
 msgid "Cache calls from %(count)d backend"
 msgid_plural "Cache calls from %(count)d backends"
-msgstr[0] "Appels au cache depuis %(count)d moteur"
-msgstr[1] "Appels au cache depuis %(count)d moteurs"
+msgstr[0] "Cache-Aufrufe von %(count)d Backend"
+msgstr[1] "Cache-Aufrufe von %(count)d Backends"
 
-#: panels/headers.py:33
+#: panels/headers.py:31
 msgid "Headers"
-msgstr "En-têtes"
+msgstr "Header"
 
-#: panels/history/panel.py:20 panels/history/panel.py:21
+#: panels/history/panel.py:18 panels/history/panel.py:19
 msgid "History"
-msgstr "Historique"
+msgstr "Geschichte"
 
-#: panels/logging.py:63
-msgid "Logging"
-msgstr "Journaux"
-
-#: panels/logging.py:69
-#, python-format
-msgid "%(count)s message"
-msgid_plural "%(count)s messages"
-msgstr[0] "%(count)s message"
-msgstr[1] "%(count)s messages"
-
-#: panels/logging.py:73
-msgid "Log messages"
-msgstr "Messages du journal"
-
-#: panels/profiling.py:150
+#: panels/profiling.py:140
 msgid "Profiling"
-msgstr "Profilage"
+msgstr "Profiling"
 
 #: panels/redirects.py:14
 msgid "Intercept redirects"
-msgstr "Interception des redirections"
+msgstr "Umleitungen abfangen"
 
 #: panels/request.py:16
 msgid "Request"
-msgstr "Requête"
+msgstr "Anfrage"
 
 #: panels/request.py:36
 msgid "<no view>"
-msgstr "<pas de vue>"
+msgstr "<kein View>"
 
 #: panels/request.py:53
 msgid "<unavailable>"
-msgstr "<indisponible>"
+msgstr "<nicht verfügbar>"
 
-#: panels/settings.py:24
+#: panels/settings.py:17
 msgid "Settings"
-msgstr "Paramètres"
+msgstr "Einstellungen"
 
-#: panels/settings.py:27
+#: panels/settings.py:20
 #, python-format
 msgid "Settings from %s"
-msgstr "Paramètres de %s"
+msgstr "Einstellungen von %s"
 
-#: panels/signals.py:58
+#: panels/signals.py:57
 #, python-format
 msgid "%(num_receivers)d receiver of 1 signal"
 msgid_plural "%(num_receivers)d receivers of 1 signal"
-msgstr[0] "%(num_receivers)d receveur d'un signal"
-msgstr[1] "%(num_receivers)d receveurs d'un signal"
+msgstr[0] "%(num_receivers)d Empfänger von einem Signal"
+msgstr[1] "%(num_receivers)d Empfänger von einem Signal"
 
-#: panels/signals.py:66
+#: panels/signals.py:62
 #, python-format
 msgid "%(num_receivers)d receiver of %(num_signals)d signals"
 msgid_plural "%(num_receivers)d receivers of %(num_signals)d signals"
-msgstr[0] "%(num_receivers)d receveur de %(num_signals)d signaux"
-msgstr[1] "%(num_receivers)d receveurs de %(num_signals)d signaux"
+msgstr[0] "%(num_receivers)d Empfänger von %(num_signals)d Signalen"
+msgstr[1] "%(num_receivers)d Empfänger von %(num_signals)d Signalen"
 
-#: panels/signals.py:73
+#: panels/signals.py:67
 msgid "Signals"
-msgstr "Signaux"
+msgstr "Signale"
 
-#: panels/sql/panel.py:24
+#: panels/sql/panel.py:23
 msgid "Autocommit"
-msgstr "Auto validation"
+msgstr "Autocommit"
 
-#: panels/sql/panel.py:25
+#: panels/sql/panel.py:24
 msgid "Read uncommitted"
-msgstr "Lecture non validée"
+msgstr "Read uncommitted"
 
-#: panels/sql/panel.py:26
+#: panels/sql/panel.py:25
 msgid "Read committed"
-msgstr "Lecture validée"
+msgstr "Read committed"
 
-#: panels/sql/panel.py:27
+#: panels/sql/panel.py:26
 msgid "Repeatable read"
-msgstr "Lecture répétable"
+msgstr "Repeatable read"
 
-#: panels/sql/panel.py:28
+#: panels/sql/panel.py:27
 msgid "Serializable"
-msgstr "Sérialisable"
+msgstr "Serializable"
 
-#: panels/sql/panel.py:40
+#: panels/sql/panel.py:39
 msgid "Idle"
-msgstr "Inactif"
+msgstr "Wartet"
 
-#: panels/sql/panel.py:41
+#: panels/sql/panel.py:40
 msgid "Active"
-msgstr "Actif"
+msgstr "Aktiv"
 
-#: panels/sql/panel.py:42
+#: panels/sql/panel.py:41
 msgid "In transaction"
-msgstr "Transaction en cours"
+msgstr "In einer Transaktion"
 
-#: panels/sql/panel.py:43
+#: panels/sql/panel.py:42
 msgid "In error"
-msgstr "Erreur"
+msgstr "Fehler"
 
-#: panels/sql/panel.py:44
+#: panels/sql/panel.py:43
 msgid "Unknown"
-msgstr "Indéterminé"
+msgstr "Unbekannt"
 
-#: panels/sql/panel.py:109
+#: panels/sql/panel.py:130
 msgid "SQL"
 msgstr "SQL"
 
-#: panels/sql/panel.py:114
+#: panels/sql/panel.py:135
 #, python-format
 msgid "%(query_count)d query in %(sql_time).2fms"
 msgid_plural "%(query_count)d queries in %(sql_time).2fms"
-msgstr[0] "%(query_count)d requête en %(sql_time).2f ms"
-msgstr[1] "%(query_count)d requêtes en %(sql_time).2f ms"
+msgstr[0] "%(query_count)d Abfrage in %(sql_time).2f ms"
+msgstr[1] "%(query_count)d Abfragen in %(sql_time).2f ms"
 
-#: panels/sql/panel.py:127
+#: panels/sql/panel.py:147
 #, python-format
 msgid "SQL queries from %(count)d connection"
 msgid_plural "SQL queries from %(count)d connections"
-msgstr[0] "requêtes SQL venant de %(count)d connexion"
-msgstr[1] "Requêtes SQL venant de %(count)d connexions"
+msgstr[0] "SQL-Abfragen von %(count)d Verbindung"
+msgstr[1] "SQL-Abfragen von %(count)d Verbindungen"
 
-#: panels/staticfiles.py:85
+#: panels/staticfiles.py:84
 #, python-format
 msgid "Static files (%(num_found)s found, %(num_used)s used)"
-msgstr "Fichiers statiques (%(num_found)s trouvé(s), %(num_used)s utilisé(s))"
+msgstr "Statische Dateien (%(num_found)s gefunden, %(num_used)s benutzt)"
 
-#: panels/staticfiles.py:106
+#: panels/staticfiles.py:105
 msgid "Static files"
-msgstr "Fichiers statiques"
+msgstr "Statische Dateien"
 
-#: panels/staticfiles.py:112
+#: panels/staticfiles.py:111
 #, python-format
 msgid "%(num_used)s file used"
 msgid_plural "%(num_used)s files used"
-msgstr[0] "%(num_used)s fichier utilisé"
-msgstr[1] "%(num_used)s fichiers utilisés"
+msgstr[0] "%(num_used)s Datei benutzt"
+msgstr[1] "%(num_used)s Dateien benutzt"
 
-#: panels/templates/panel.py:144
+#: panels/templates/panel.py:143
 msgid "Templates"
-msgstr "Gabarits"
+msgstr "Templates"
 
-#: panels/templates/panel.py:149
+#: panels/templates/panel.py:148
 #, python-format
 msgid "Templates (%(num_templates)s rendered)"
-msgstr "Gabarits (%(num_templates)s affichés)"
+msgstr "Templates (%(num_templates)s gerendert)"
 
-#: panels/templates/panel.py:181
+#: panels/templates/panel.py:180
 msgid "No origin"
-msgstr "Sans Origine"
+msgstr "Kein Ursprung"
 
 #: panels/timer.py:25
 #, python-format
 msgid "CPU: %(cum)0.2fms (%(total)0.2fms)"
 msgstr "CPU: %(cum)0.2fms (%(total)0.2fms)"
 
 #: panels/timer.py:30
 #, python-format
 msgid "Total: %0.2fms"
-msgstr "Total : %0.2fms"
+msgstr "Gesamt: %0.2fms"
 
 #: panels/timer.py:36 templates/debug_toolbar/panels/history.html:9
-#: templates/debug_toolbar/panels/logging.html:7
 #: templates/debug_toolbar/panels/sql_explain.html:11
 #: templates/debug_toolbar/panels/sql_profile.html:12
 #: templates/debug_toolbar/panels/sql_select.html:11
 msgid "Time"
-msgstr "Temps"
+msgstr "Zeit"
 
 #: panels/timer.py:44
 msgid "User CPU time"
-msgstr "Temps CPU de l'utilisateur"
+msgstr "CPU-Zeit Benutzer"
 
 #: panels/timer.py:44
 #, python-format
 msgid "%(utime)0.3f msec"
 msgstr "%(utime)0.3f ms"
 
 #: panels/timer.py:45
 msgid "System CPU time"
-msgstr "Temps CPU du système"
+msgstr "CPU-Zeit System"
 
 #: panels/timer.py:45
 #, python-format
 msgid "%(stime)0.3f msec"
 msgstr "%(stime)0.3f ms"
 
 #: panels/timer.py:46
 msgid "Total CPU time"
-msgstr "Temps total du CPU"
+msgstr "CPU-Zeit gesamt"
 
 #: panels/timer.py:46
 #, python-format
 msgid "%(total)0.3f msec"
 msgstr "%(total)0.3f ms"
 
 #: panels/timer.py:47
 msgid "Elapsed time"
-msgstr "Temps écoulé"
+msgstr "Verstrichene Zeit"
 
 #: panels/timer.py:47
 #, python-format
 msgid "%(total_time)0.3f msec"
 msgstr "%(total_time)0.3f ms"
 
 #: panels/timer.py:49
 msgid "Context switches"
-msgstr "Basculements de contexte"
+msgstr "Kontextwechsel"
 
 #: panels/timer.py:50
 #, python-format
 msgid "%(vcsw)d voluntary, %(ivcsw)d involuntary"
-msgstr "%(vcsw)d volontaire, %(ivcsw)d involontaire"
+msgstr "%(vcsw)d freiwillig, %(ivcsw)d unfreiwillig"
 
 #: panels/versions.py:19
 msgid "Versions"
-msgstr "Versions"
+msgstr "Versionen"
 
-#: templates/debug_toolbar/base.html:18
+#: templates/debug_toolbar/base.html:22
 msgid "Hide toolbar"
-msgstr "Masquer la barre d'outils"
+msgstr "Toolbar ausblenden"
 
-#: templates/debug_toolbar/base.html:18
+#: templates/debug_toolbar/base.html:22
 msgid "Hide"
-msgstr "Masquer"
+msgstr "Ausblenden"
 
-#: templates/debug_toolbar/base.html:25
+#: templates/debug_toolbar/base.html:29
 msgid "Show toolbar"
-msgstr "Afficher la barre d'outils"
+msgstr "Toolbar einblenden"
 
 #: templates/debug_toolbar/includes/panel_button.html:4
 msgid "Disable for next and successive requests"
-msgstr "Désactiver pour les requêtes suivantes"
+msgstr "Für nächste und die darauffolgenden Anfragen deaktivieren"
 
 #: templates/debug_toolbar/includes/panel_button.html:4
 msgid "Enable for next and successive requests"
-msgstr "Activer pour les requêtes suivantes"
+msgstr "Für nächste und die darauffolgenden Anfragen aktivieren"
 
 #: templates/debug_toolbar/panels/cache.html:2
 msgid "Summary"
-msgstr "Résumé"
+msgstr "Zusammenfassung"
 
 #: templates/debug_toolbar/panels/cache.html:6
 msgid "Total calls"
-msgstr "Nombre total d'appels"
+msgstr "Aufrufe gesamt"
 
 #: templates/debug_toolbar/panels/cache.html:7
 msgid "Total time"
-msgstr "Temps total"
+msgstr "Zeit gesamt"
 
 #: templates/debug_toolbar/panels/cache.html:8
 msgid "Cache hits"
-msgstr "Succès de cache"
+msgstr "Cache erfolgreich"
 
 #: templates/debug_toolbar/panels/cache.html:9
 msgid "Cache misses"
-msgstr "Défauts de cache"
+msgstr "Cache verfehlt"
 
 #: templates/debug_toolbar/panels/cache.html:21
 msgid "Commands"
-msgstr "Commandes"
+msgstr "Befehle"
 
 #: templates/debug_toolbar/panels/cache.html:39
 msgid "Calls"
-msgstr "Appels"
+msgstr "Aufrufe"
 
 #: templates/debug_toolbar/panels/cache.html:43
 #: templates/debug_toolbar/panels/sql.html:36
 msgid "Time (ms)"
-msgstr "Temps (ms)"
+msgstr "Zeit (ms)"
 
 #: templates/debug_toolbar/panels/cache.html:44
 msgid "Type"
-msgstr "Type"
+msgstr "Typ"
 
 #: templates/debug_toolbar/panels/cache.html:45
 #: templates/debug_toolbar/panels/request.html:8
 msgid "Arguments"
-msgstr "Paramètres"
+msgstr "Argumente"
 
 #: templates/debug_toolbar/panels/cache.html:46
 #: templates/debug_toolbar/panels/request.html:9
 msgid "Keyword arguments"
-msgstr "Paramètres nommés"
+msgstr "Schlüsselwort-Argumente"
 
 #: templates/debug_toolbar/panels/cache.html:47
 msgid "Backend"
-msgstr "Moteur"
+msgstr "Backend"
 
 #: templates/debug_toolbar/panels/headers.html:3
 msgid "Request headers"
-msgstr "En-têtes de requête"
+msgstr "Anfrage-Header"
 
 #: templates/debug_toolbar/panels/headers.html:8
 #: templates/debug_toolbar/panels/headers.html:27
 #: templates/debug_toolbar/panels/headers.html:48
 msgid "Key"
-msgstr "Clé"
+msgstr "Schlüssel"
 
 #: templates/debug_toolbar/panels/headers.html:9
 #: templates/debug_toolbar/panels/headers.html:28
 #: templates/debug_toolbar/panels/headers.html:49
 #: templates/debug_toolbar/panels/history_tr.html:23
-#: templates/debug_toolbar/panels/request_variables.html:11
+#: templates/debug_toolbar/panels/request_variables.html:12
 #: templates/debug_toolbar/panels/settings.html:6
 #: templates/debug_toolbar/panels/timer.html:11
 msgid "Value"
-msgstr "Valeur"
+msgstr "Wert"
 
 #: templates/debug_toolbar/panels/headers.html:22
 msgid "Response headers"
-msgstr "En-têtes de réponse"
+msgstr "Antwort-Header"
 
 #: templates/debug_toolbar/panels/headers.html:41
 msgid "WSGI environ"
-msgstr "Environnement WSGI"
+msgstr "WSGI-Umgebung"
 
 #: templates/debug_toolbar/panels/headers.html:43
 msgid ""
 "Since the WSGI environ inherits the environment of the server, only a "
 "significant subset is shown below."
-msgstr "Comme l'environnement WSGI hérite de celui du serveur, seul un sous-ensemble pertinent est affiché ci-dessous."
+msgstr ""
+"Da sich die WSGI-Umgebung von der Umgebung des Servers ableitet, wird nur "
+"eine notwendige Teilmenge dargestellt."
 
 #: templates/debug_toolbar/panels/history.html:10
 msgid "Method"
-msgstr "Méthode"
+msgstr "Methode"
 
 #: templates/debug_toolbar/panels/history.html:11
 #: templates/debug_toolbar/panels/staticfiles.html:43
 msgid "Path"
-msgstr "Chemin"
+msgstr "Pfad"
 
 #: templates/debug_toolbar/panels/history.html:12
 msgid "Request Variables"
-msgstr "Variables de Requête"
+msgstr "Anfrage-Variablen"
 
 #: templates/debug_toolbar/panels/history.html:13
 msgid "Status"
-msgstr "État"
+msgstr "Status"
 
 #: templates/debug_toolbar/panels/history.html:14
 #: templates/debug_toolbar/panels/sql.html:37
 msgid "Action"
-msgstr "Action"
+msgstr "Aktion"
 
 #: templates/debug_toolbar/panels/history_tr.html:22
-#: templates/debug_toolbar/panels/request_variables.html:10
+#: templates/debug_toolbar/panels/request_variables.html:11
 msgid "Variable"
 msgstr "Variable"
 
-#: templates/debug_toolbar/panels/logging.html:6
-msgid "Level"
-msgstr "Niveau"
-
-#: templates/debug_toolbar/panels/logging.html:8
-msgid "Channel"
-msgstr "Canal"
-
-#: templates/debug_toolbar/panels/logging.html:9
-msgid "Message"
-msgstr "Message"
-
-#: templates/debug_toolbar/panels/logging.html:10
-#: templates/debug_toolbar/panels/staticfiles.html:44
-msgid "Location"
-msgstr "Emplacement"
-
-#: templates/debug_toolbar/panels/logging.html:26
-msgid "No messages logged"
-msgstr "Aucun message dans le journal"
-
 #: templates/debug_toolbar/panels/profiling.html:5
 msgid "Call"
-msgstr "Appel"
+msgstr "Aufruf"
 
 #: templates/debug_toolbar/panels/profiling.html:6
 msgid "CumTime"
-msgstr "Temps cumulé"
+msgstr "Gesamt"
 
 #: templates/debug_toolbar/panels/profiling.html:7
 #: templates/debug_toolbar/panels/profiling.html:9
 msgid "Per"
-msgstr "Par"
+msgstr "Per"
 
 #: templates/debug_toolbar/panels/profiling.html:8
 msgid "TotTime"
-msgstr "Temps total"
+msgstr "Total"
 
 #: templates/debug_toolbar/panels/profiling.html:10
 msgid "Count"
-msgstr "Compte"
+msgstr "Anzahl"
 
 #: templates/debug_toolbar/panels/request.html:3
 msgid "View information"
-msgstr "Afficher l'information"
+msgstr "View-Informationen"
 
 #: templates/debug_toolbar/panels/request.html:7
 msgid "View function"
-msgstr "Fonction de vue"
+msgstr "View-Funktion"
 
 #: templates/debug_toolbar/panels/request.html:10
 msgid "URL name"
-msgstr "Nom d'URL"
+msgstr "URL-Name"
 
 #: templates/debug_toolbar/panels/request.html:24
 msgid "Cookies"
 msgstr "Cookies"
 
 #: templates/debug_toolbar/panels/request.html:27
 msgid "No cookies"
-msgstr "Pas de cookies"
+msgstr "Keine Cookies"
 
 #: templates/debug_toolbar/panels/request.html:31
 msgid "Session data"
-msgstr "Données de session"
+msgstr "Sitzungsdaten"
 
 #: templates/debug_toolbar/panels/request.html:34
 msgid "No session data"
-msgstr "Pas de données de session"
+msgstr "Keine Sitzungsdaten"
 
 #: templates/debug_toolbar/panels/request.html:38
 msgid "GET data"
-msgstr "Données GET"
+msgstr "GET-Daten"
 
 #: templates/debug_toolbar/panels/request.html:41
 msgid "No GET data"
-msgstr "Aucune donnée GET"
+msgstr "Keine GET-Daten"
 
 #: templates/debug_toolbar/panels/request.html:45
 msgid "POST data"
-msgstr "Données POST"
+msgstr "POST-Daten"
 
 #: templates/debug_toolbar/panels/request.html:48
 msgid "No POST data"
-msgstr "Aucune donnée POST"
+msgstr "Keine POST-Daten"
 
 #: templates/debug_toolbar/panels/settings.html:5
 msgid "Setting"
-msgstr "Paramètre"
+msgstr "Einstellung"
 
 #: templates/debug_toolbar/panels/signals.html:5
 msgid "Signal"
 msgstr "Signal"
 
 #: templates/debug_toolbar/panels/signals.html:6
 msgid "Receivers"
-msgstr "Receveurs"
+msgstr "Empfänger"
 
 #: templates/debug_toolbar/panels/sql.html:6
 #, python-format
 msgid "%(num)s query"
 msgid_plural "%(num)s queries"
-msgstr[0] "%(num)s requête"
-msgstr[1] "%(num)s requêtes"
+msgstr[0] "%(num)s Abfrage"
+msgstr[1] "%(num)s Abfragen"
 
 #: templates/debug_toolbar/panels/sql.html:8
 #, python-format
 msgid ""
 "including <abbr title=\"Similar queries are queries with the same SQL, but "
 "potentially different parameters.\">%(count)s similar</abbr>"
-msgstr "comprenant <abbr title=\"Similar queries are queries with the same SQL, but potentially different parameters.\">%(count)s similaires</abbr>"
+msgstr ""
+"inklusive <abbr title=\"Similar queries are queries with the same SQL, but "
+"potentially different parameters.\">%(count)s ähnlich</abbr>"
 
 #: templates/debug_toolbar/panels/sql.html:12
 #, python-format
 msgid ""
 "and <abbr title=\"Duplicate queries are identical to each other: they "
 "execute exactly the same SQL and parameters.\">%(dupes)s duplicates</abbr>"
-msgstr "et <abbr title=\"Duplicate queries are identical to each other: they execute exactly the same SQL and parameters.\">%(dupes)s en double</abbr>"
+msgstr ""
+"und <abbr title=\"Duplicate queries are identical to each other: they "
+"execute exactly the same SQL and parameters.\">%(dupes)s dupliziert</abbr>"
 
 #: templates/debug_toolbar/panels/sql.html:34
 msgid "Query"
-msgstr "Requête"
+msgstr "Abfrage"
 
 #: templates/debug_toolbar/panels/sql.html:35
 #: templates/debug_toolbar/panels/timer.html:36
 msgid "Timeline"
-msgstr "Chronologie"
+msgstr "Verlauf"
 
 #: templates/debug_toolbar/panels/sql.html:52
 #, python-format
 msgid "%(count)s similar queries."
-msgstr "%(count)s requêtes similaires."
+msgstr "%(count)s ähnliche Abfragen."
 
 #: templates/debug_toolbar/panels/sql.html:58
 #, python-format
 msgid "Duplicated %(dupes)s times."
-msgstr "Dupliqué %(dupes)s fois."
+msgstr "%(dupes)s-mal dupliziert."
 
 #: templates/debug_toolbar/panels/sql.html:95
 msgid "Connection:"
-msgstr "Connexion :"
+msgstr "Verbindung:"
 
 #: templates/debug_toolbar/panels/sql.html:97
 msgid "Isolation level:"
-msgstr "Niveau d'isolation :"
+msgstr "Isolationsebene:"
 
 #: templates/debug_toolbar/panels/sql.html:100
 msgid "Transaction status:"
-msgstr "État de la transaction :"
+msgstr "Transaktionsstatus:"
 
 #: templates/debug_toolbar/panels/sql.html:114
 msgid "(unknown)"
-msgstr "(indéterminé)"
+msgstr "(unbekannt)"
 
 #: templates/debug_toolbar/panels/sql.html:123
 msgid "No SQL queries were recorded during this request."
-msgstr "Aucune requête SQL n'a été enregistrée durant cette requête."
+msgstr "Es wurde keine SQL-Abfrage während dieses Vorgangs aufgezeichnet."
 
 #: templates/debug_toolbar/panels/sql_explain.html:4
 msgid "SQL explained"
-msgstr "SQL expliqué"
+msgstr "SQL erklärt"
 
 #: templates/debug_toolbar/panels/sql_explain.html:9
 #: templates/debug_toolbar/panels/sql_profile.html:10
 #: templates/debug_toolbar/panels/sql_select.html:9
 msgid "Executed SQL"
-msgstr "SQL Exécuté"
+msgstr "Ausgeführtes SQL"
 
 #: templates/debug_toolbar/panels/sql_explain.html:13
 #: templates/debug_toolbar/panels/sql_profile.html:14
 #: templates/debug_toolbar/panels/sql_select.html:13
 msgid "Database"
-msgstr "Base de données"
+msgstr "Datenbank"
 
 #: templates/debug_toolbar/panels/sql_profile.html:4
 msgid "SQL profiled"
-msgstr "SQL profilé"
+msgstr "SQL durchleuchtet"
 
 #: templates/debug_toolbar/panels/sql_profile.html:37
 msgid "Error"
-msgstr "Erreur"
+msgstr "Fehler"
 
 #: templates/debug_toolbar/panels/sql_select.html:4
 msgid "SQL selected"
-msgstr "SQL sélectionné"
+msgstr "SQL ausgewählt"
 
 #: templates/debug_toolbar/panels/sql_select.html:36
 msgid "Empty set"
-msgstr "Ensemble vide"
+msgstr "Leeres Set"
 
 #: templates/debug_toolbar/panels/staticfiles.html:3
 msgid "Static file path"
 msgid_plural "Static file paths"
-msgstr[0] "Chemin de fichier statique"
-msgstr[1] "Chemins de fichiers statiques"
+msgstr[0] "Pfad mit statischen Dateien"
+msgstr[1] "Pfade mit statischen Dateien"
 
 #: templates/debug_toolbar/panels/staticfiles.html:7
 #, python-format
 msgid "(prefix %(prefix)s)"
-msgstr "(préfixe %(prefix)s)"
+msgstr "(Präfix %(prefix)s)"
 
 #: templates/debug_toolbar/panels/staticfiles.html:11
 #: templates/debug_toolbar/panels/staticfiles.html:22
 #: templates/debug_toolbar/panels/staticfiles.html:34
 #: templates/debug_toolbar/panels/templates.html:10
 #: templates/debug_toolbar/panels/templates.html:30
 #: templates/debug_toolbar/panels/templates.html:47
 msgid "None"
-msgstr "Aucun"
+msgstr "-"
 
 #: templates/debug_toolbar/panels/staticfiles.html:14
 msgid "Static file app"
 msgid_plural "Static file apps"
-msgstr[0] "Application de fichiers statiques"
-msgstr[1] "Applications de fichiers statiques"
+msgstr[0] "App mit statischen Dateien"
+msgstr[1] "Apps mit statischen Dateien"
 
 #: templates/debug_toolbar/panels/staticfiles.html:25
 msgid "Static file"
 msgid_plural "Static files"
-msgstr[0] ""
-msgstr[1] "Fichiers statiques"
+msgstr[0] "Statische Datei"
+msgstr[1] "Statische Dateien"
 
 #: templates/debug_toolbar/panels/staticfiles.html:39
 #, python-format
 msgid "%(payload_count)s file"
 msgid_plural "%(payload_count)s files"
-msgstr[0] "%(payload_count)s fichier"
-msgstr[1] "%(payload_count)s fichiers"
+msgstr[0] "%(payload_count)s Datei"
+msgstr[1] "%(payload_count)s Dateien"
+
+#: templates/debug_toolbar/panels/staticfiles.html:44
+msgid "Location"
+msgstr "Ort"
 
 #: templates/debug_toolbar/panels/template_source.html:4
 msgid "Template source:"
-msgstr "Source du gabarit :"
+msgstr "Template-Quelle:"
 
 #: templates/debug_toolbar/panels/templates.html:2
 msgid "Template path"
 msgid_plural "Template paths"
-msgstr[0] ""
-msgstr[1] "Chemin du gabarit"
+msgstr[0] "Template-Pfad"
+msgstr[1] "Template-Pfade"
 
 #: templates/debug_toolbar/panels/templates.html:13
 msgid "Template"
 msgid_plural "Templates"
-msgstr[0] ""
-msgstr[1] "Gabarit"
+msgstr[0] "Template"
+msgstr[1] "Templates"
 
 #: templates/debug_toolbar/panels/templates.html:22
 #: templates/debug_toolbar/panels/templates.html:40
 msgid "Toggle context"
-msgstr "Afficher/masquer le contexte"
+msgstr "Context zeigen"
 
 #: templates/debug_toolbar/panels/templates.html:33
 msgid "Context processor"
 msgid_plural "Context processors"
-msgstr[0] "Processeur de contexte"
-msgstr[1] "Processeurs de contexte"
+msgstr[0] "Context-Prozessor"
+msgstr[1] "Context-Prozessoren"
 
 #: templates/debug_toolbar/panels/timer.html:2
 msgid "Resource usage"
-msgstr "Utilisation des ressources"
+msgstr "Ressourcenverwendung"
 
 #: templates/debug_toolbar/panels/timer.html:10
 msgid "Resource"
 msgstr "Ressource"
 
 #: templates/debug_toolbar/panels/timer.html:26
 msgid "Browser timing"
-msgstr "Chronologie du navigateur"
+msgstr "Browserzeit"
 
 #: templates/debug_toolbar/panels/timer.html:35
 msgid "Timing attribute"
-msgstr "Attribut mesuré"
+msgstr "Timing-Attribut"
 
 #: templates/debug_toolbar/panels/timer.html:37
 msgid "Milliseconds since navigation start (+length)"
-msgstr "Millisecondes depuis le début de la navigation (+longueur)"
+msgstr "Millisekunden seit Seitenaufruf (plus Dauer)"
 
 #: templates/debug_toolbar/panels/versions.html:10
 msgid "Package"
-msgstr "Paquet"
+msgstr "Paket"
 
 #: templates/debug_toolbar/panels/versions.html:11
 msgid "Name"
-msgstr "Nom"
+msgstr "Name"
 
 #: templates/debug_toolbar/panels/versions.html:12
 msgid "Version"
 msgstr "Version"
 
 #: templates/debug_toolbar/redirect.html:10
 msgid "Location:"
-msgstr "Emplacement :"
+msgstr "Ziel:"
 
 #: templates/debug_toolbar/redirect.html:12
 msgid ""
 "The Django Debug Toolbar has intercepted a redirect to the above URL for "
 "debug viewing purposes. You can click the above link to continue with the "
 "redirect as normal."
-msgstr "La barre de débogage Django a intercepté une redirection vers l'URL ci-dessus afin de permettre la consultation des messages de débogage.  Vous pouvez cliquer sur le lien ci-dessus pour continuer normalement avec la redirection."
+msgstr ""
+"Die Django Debug Toolbar hat eine Weiterleitung an die obenstehende URL zur "
+"weiteren Überprüfung abgefangen. Klicken Sie den Link, um wie gewohnt "
+"weitergeleitet zu werden."
 
-#: views.py:15
+#: views.py:16
 msgid ""
 "Data for this panel isn't available anymore. Please reload the page and "
 "retry."
-msgstr "Les données de ce panneau ne sont plus disponibles. Rechargez la page et essayez à nouveau."
+msgstr ""
+"Die Daten für dieses Panel sind nicht mehr verfügbar. Bitte laden Sie die "
+"Seite neu."
```

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/locale/he/LC_MESSAGES/django.mo` & `django_debug_toolbar-4.0.0/debug_toolbar/locale/he/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/locale/he/LC_MESSAGES/django.po` & `django_debug_toolbar-4.0.0/debug_toolbar/locale/he/LC_MESSAGES/django.po`

 * *Files 6% similar despite different names*

```diff
@@ -4,286 +4,273 @@
 #
 # Translators:
 # shaib <shai@platonix.com>, 2012
 msgid ""
 msgstr ""
 "Project-Id-Version: Django Debug Toolbar\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2014-04-25 21:52+0200\n"
+"POT-Creation-Date: 2023-01-20 17:23+0100\n"
 "PO-Revision-Date: 2014-04-25 19:53+0000\n"
 "Last-Translator: Aymeric Augustin <aymeric.augustin@m4x.org>\n"
-"Language-Team: Hebrew (http://www.transifex.com/projects/p/django-debug-toolbar/language/he/)\n"
+"Language-Team: Hebrew (http://www.transifex.com/projects/p/django-debug-"
+"toolbar/language/he/)\n"
+"Language: he\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: he\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: apps.py:11
+#: apps.py:15
 msgid "Debug Toolbar"
 msgstr ""
 
-#: views.py:14
-msgid ""
-"Data for this panel isn't available anymore. Please reload the page and "
-"retry."
-msgstr ""
-
-#: panels/cache.py:191
+#: panels/cache.py:180
 msgid "Cache"
 msgstr ""
 
-#: panels/cache.py:196
+#: panels/cache.py:186
 #, python-format
 msgid "%(cache_calls)d call in %(time).2fms"
 msgid_plural "%(cache_calls)d calls in %(time).2fms"
 msgstr[0] ""
 msgstr[1] ""
 
-#: panels/cache.py:204
+#: panels/cache.py:195
 #, python-format
 msgid "Cache calls from %(count)d backend"
 msgid_plural "Cache calls from %(count)d backends"
 msgstr[0] ""
 msgstr[1] ""
 
-#: panels/headers.py:35
+#: panels/headers.py:31
 msgid "Headers"
 msgstr ""
 
-#: panels/logging.py:64
-msgid "Logging"
-msgstr "רישום יומן"
-
-#: panels/logging.py:70
-#, python-format
-msgid "%(count)s message"
-msgid_plural "%(count)s messages"
-msgstr[0] ""
-msgstr[1] ""
-
-#: panels/logging.py:73
-msgid "Log messages"
+#: panels/history/panel.py:18 panels/history/panel.py:19
+msgid "History"
 msgstr ""
 
-#: panels/profiling.py:127
+#: panels/profiling.py:140
 msgid "Profiling"
 msgstr ""
 
-#: panels/redirects.py:17
+#: panels/redirects.py:14
 msgid "Intercept redirects"
 msgstr ""
 
-#: panels/request.py:18
+#: panels/request.py:16
 msgid "Request"
 msgstr ""
 
-#: panels/request.py:35
+#: panels/request.py:36
 msgid "<no view>"
 msgstr ""
 
-#: panels/request.py:47
+#: panels/request.py:53
 msgid "<unavailable>"
 msgstr ""
 
-#: panels/settings.py:20
+#: panels/settings.py:17
 msgid "Settings"
 msgstr ""
 
-#: panels/settings.py:23
+#: panels/settings.py:20
 #, python-format
-msgid "Settings from <code>%s</code>"
+msgid "Settings from %s"
 msgstr ""
 
-#: panels/signals.py:45
+#: panels/signals.py:57
 #, python-format
 msgid "%(num_receivers)d receiver of 1 signal"
 msgid_plural "%(num_receivers)d receivers of 1 signal"
 msgstr[0] ""
 msgstr[1] ""
 
-#: panels/signals.py:48
+#: panels/signals.py:62
 #, python-format
 msgid "%(num_receivers)d receiver of %(num_signals)d signals"
 msgid_plural "%(num_receivers)d receivers of %(num_signals)d signals"
 msgstr[0] ""
 msgstr[1] ""
 
-#: panels/signals.py:53
+#: panels/signals.py:67
 msgid "Signals"
 msgstr "סיגנלים"
 
-#: panels/staticfiles.py:89
+#: panels/sql/panel.py:23
+msgid "Autocommit"
+msgstr ""
+
+#: panels/sql/panel.py:24
+msgid "Read uncommitted"
+msgstr ""
+
+#: panels/sql/panel.py:25
+msgid "Read committed"
+msgstr ""
+
+#: panels/sql/panel.py:26
+msgid "Repeatable read"
+msgstr ""
+
+#: panels/sql/panel.py:27
+msgid "Serializable"
+msgstr "משתנה"
+
+#: panels/sql/panel.py:39
+msgid "Idle"
+msgstr ""
+
+#: panels/sql/panel.py:40
+msgid "Active"
+msgstr "פעילות"
+
+#: panels/sql/panel.py:41
+msgid "In transaction"
+msgstr ""
+
+#: panels/sql/panel.py:42
+msgid "In error"
+msgstr "שגיאה"
+
+#: panels/sql/panel.py:43
+msgid "Unknown"
+msgstr ""
+
+#: panels/sql/panel.py:130
+msgid "SQL"
+msgstr ""
+
+#: panels/sql/panel.py:135
+#, python-format
+msgid "%(query_count)d query in %(sql_time).2fms"
+msgid_plural "%(query_count)d queries in %(sql_time).2fms"
+msgstr[0] ""
+msgstr[1] ""
+
+#: panels/sql/panel.py:147
+#, python-format
+msgid "SQL queries from %(count)d connection"
+msgid_plural "SQL queries from %(count)d connections"
+msgstr[0] ""
+msgstr[1] ""
+
+#: panels/staticfiles.py:84
 #, python-format
 msgid "Static files (%(num_found)s found, %(num_used)s used)"
 msgstr ""
 
-#: panels/staticfiles.py:107
+#: panels/staticfiles.py:105
 msgid "Static files"
 msgstr ""
 
-#: panels/staticfiles.py:112
+#: panels/staticfiles.py:111
 #, python-format
 msgid "%(num_used)s file used"
 msgid_plural "%(num_used)s files used"
 msgstr[0] ""
 msgstr[1] ""
 
-#: panels/timer.py:23
+#: panels/templates/panel.py:143
+msgid "Templates"
+msgstr "תבניות"
+
+#: panels/templates/panel.py:148
+#, python-format
+msgid "Templates (%(num_templates)s rendered)"
+msgstr ""
+
+#: panels/templates/panel.py:180
+msgid "No origin"
+msgstr ""
+
+#: panels/timer.py:25
 #, python-format
 msgid "CPU: %(cum)0.2fms (%(total)0.2fms)"
 msgstr ""
 
-#: panels/timer.py:28
+#: panels/timer.py:30
 #, python-format
 msgid "Total: %0.2fms"
 msgstr ""
 
-#: panels/timer.py:34 templates/debug_toolbar/panels/logging.html:7
+#: panels/timer.py:36 templates/debug_toolbar/panels/history.html:9
 #: templates/debug_toolbar/panels/sql_explain.html:11
 #: templates/debug_toolbar/panels/sql_profile.html:12
 #: templates/debug_toolbar/panels/sql_select.html:11
 msgid "Time"
 msgstr "זמן"
 
-#: panels/timer.py:42
+#: panels/timer.py:44
 msgid "User CPU time"
 msgstr ""
 
-#: panels/timer.py:42
+#: panels/timer.py:44
 #, python-format
 msgid "%(utime)0.3f msec"
 msgstr ""
 
-#: panels/timer.py:43
+#: panels/timer.py:45
 msgid "System CPU time"
 msgstr ""
 
-#: panels/timer.py:43
+#: panels/timer.py:45
 #, python-format
 msgid "%(stime)0.3f msec"
 msgstr ""
 
-#: panels/timer.py:44
+#: panels/timer.py:46
 msgid "Total CPU time"
 msgstr ""
 
-#: panels/timer.py:44
+#: panels/timer.py:46
 #, python-format
 msgid "%(total)0.3f msec"
 msgstr ""
 
-#: panels/timer.py:45
+#: panels/timer.py:47
 msgid "Elapsed time"
 msgstr ""
 
-#: panels/timer.py:45
+#: panels/timer.py:47
 #, python-format
 msgid "%(total_time)0.3f msec"
 msgstr ""
 
-#: panels/timer.py:46
+#: panels/timer.py:49
 msgid "Context switches"
 msgstr ""
 
-#: panels/timer.py:46
+#: panels/timer.py:50
 #, python-format
 msgid "%(vcsw)d voluntary, %(ivcsw)d involuntary"
 msgstr ""
 
-#: panels/versions.py:25
+#: panels/versions.py:19
 msgid "Versions"
 msgstr "גירסאות"
 
-#: panels/sql/panel.py:22
-msgid "Autocommit"
-msgstr ""
-
-#: panels/sql/panel.py:23
-msgid "Read uncommitted"
-msgstr ""
-
-#: panels/sql/panel.py:24
-msgid "Read committed"
-msgstr ""
-
-#: panels/sql/panel.py:25
-msgid "Repeatable read"
-msgstr ""
-
-#: panels/sql/panel.py:26
-msgid "Serializable"
-msgstr "משתנה"
-
-#: panels/sql/panel.py:37
-msgid "Idle"
-msgstr ""
-
-#: panels/sql/panel.py:38
-msgid "Active"
-msgstr "פעילות"
-
-#: panels/sql/panel.py:39
-msgid "In transaction"
-msgstr ""
-
-#: panels/sql/panel.py:40
-msgid "In error"
-msgstr "שגיאה"
-
-#: panels/sql/panel.py:41
-msgid "Unknown"
-msgstr ""
-
-#: panels/sql/panel.py:105
-msgid "SQL"
-msgstr ""
-
-#: panels/templates/panel.py:141
-msgid "Templates"
-msgstr "תבניות"
-
-#: panels/templates/panel.py:146
-#, python-format
-msgid "Templates (%(num_templates)s rendered)"
-msgstr ""
-
-#: templates/debug_toolbar/base.html:19
+#: templates/debug_toolbar/base.html:22
 msgid "Hide toolbar"
 msgstr ""
 
-#: templates/debug_toolbar/base.html:19
+#: templates/debug_toolbar/base.html:22
 msgid "Hide"
 msgstr "הסתר"
 
-#: templates/debug_toolbar/base.html:25
-msgid "Disable for next and successive requests"
-msgstr ""
-
-#: templates/debug_toolbar/base.html:25
-msgid "Enable for next and successive requests"
-msgstr ""
-
-#: templates/debug_toolbar/base.html:47
+#: templates/debug_toolbar/base.html:29
 msgid "Show toolbar"
 msgstr ""
 
-#: templates/debug_toolbar/base.html:53
-msgid "Close"
-msgstr "סגור"
-
-#: templates/debug_toolbar/redirect.html:8
-msgid "Location:"
+#: templates/debug_toolbar/includes/panel_button.html:4
+msgid "Disable for next and successive requests"
 msgstr ""
 
-#: templates/debug_toolbar/redirect.html:10
-msgid ""
-"The Django Debug Toolbar has intercepted a redirect to the above URL for "
-"debug viewing purposes. You can click the above link to continue with the "
-"redirect as normal."
+#: templates/debug_toolbar/includes/panel_button.html:4
+msgid "Enable for next and successive requests"
 msgstr ""
 
 #: templates/debug_toolbar/panels/cache.html:2
 msgid "Summary"
 msgstr ""
 
 #: templates/debug_toolbar/panels/cache.html:6
@@ -307,15 +294,15 @@
 msgstr ""
 
 #: templates/debug_toolbar/panels/cache.html:39
 msgid "Calls"
 msgstr ""
 
 #: templates/debug_toolbar/panels/cache.html:43
-#: templates/debug_toolbar/panels/sql.html:20
+#: templates/debug_toolbar/panels/sql.html:36
 msgid "Time (ms)"
 msgstr ""
 
 #: templates/debug_toolbar/panels/cache.html:44
 msgid "Type"
 msgstr "סוג"
 
@@ -342,18 +329,16 @@
 #: templates/debug_toolbar/panels/headers.html:48
 msgid "Key"
 msgstr "מפתח"
 
 #: templates/debug_toolbar/panels/headers.html:9
 #: templates/debug_toolbar/panels/headers.html:28
 #: templates/debug_toolbar/panels/headers.html:49
-#: templates/debug_toolbar/panels/request.html:33
-#: templates/debug_toolbar/panels/request.html:59
-#: templates/debug_toolbar/panels/request.html:85
-#: templates/debug_toolbar/panels/request.html:110
+#: templates/debug_toolbar/panels/history_tr.html:23
+#: templates/debug_toolbar/panels/request_variables.html:12
 #: templates/debug_toolbar/panels/settings.html:6
 #: templates/debug_toolbar/panels/timer.html:11
 msgid "Value"
 msgstr "ערך"
 
 #: templates/debug_toolbar/panels/headers.html:22
 msgid "Response headers"
@@ -365,34 +350,42 @@
 
 #: templates/debug_toolbar/panels/headers.html:43
 msgid ""
 "Since the WSGI environ inherits the environment of the server, only a "
 "significant subset is shown below."
 msgstr ""
 
-#: templates/debug_toolbar/panels/logging.html:6
-msgid "Level"
-msgstr "רמה"
+#: templates/debug_toolbar/panels/history.html:10
+msgid "Method"
+msgstr ""
 
-#: templates/debug_toolbar/panels/logging.html:8
-msgid "Channel"
+#: templates/debug_toolbar/panels/history.html:11
+#: templates/debug_toolbar/panels/staticfiles.html:43
+msgid "Path"
 msgstr ""
 
-#: templates/debug_toolbar/panels/logging.html:9
-msgid "Message"
-msgstr "הודעה"
+#: templates/debug_toolbar/panels/history.html:12
+#, fuzzy
+#| msgid "Variable"
+msgid "Request Variables"
+msgstr "משתנה"
 
-#: templates/debug_toolbar/panels/logging.html:10
-#: templates/debug_toolbar/panels/staticfiles.html:45
-msgid "Location"
-msgstr "מקום"
+#: templates/debug_toolbar/panels/history.html:13
+msgid "Status"
+msgstr ""
 
-#: templates/debug_toolbar/panels/logging.html:26
-msgid "No messages logged"
-msgstr "אין הודעות"
+#: templates/debug_toolbar/panels/history.html:14
+#: templates/debug_toolbar/panels/sql.html:37
+msgid "Action"
+msgstr "פעילות"
+
+#: templates/debug_toolbar/panels/history_tr.html:22
+#: templates/debug_toolbar/panels/request_variables.html:11
+msgid "Variable"
+msgstr "משתנה"
 
 #: templates/debug_toolbar/panels/profiling.html:5
 msgid "Call"
 msgstr ""
 
 #: templates/debug_toolbar/panels/profiling.html:6
 msgid "CumTime"
@@ -423,112 +416,114 @@
 msgid "URL name"
 msgstr ""
 
 #: templates/debug_toolbar/panels/request.html:24
 msgid "Cookies"
 msgstr ""
 
-#: templates/debug_toolbar/panels/request.html:32
-#: templates/debug_toolbar/panels/request.html:58
-#: templates/debug_toolbar/panels/request.html:84
-#: templates/debug_toolbar/panels/request.html:109
-msgid "Variable"
-msgstr "משתנה"
-
-#: templates/debug_toolbar/panels/request.html:46
+#: templates/debug_toolbar/panels/request.html:27
 msgid "No cookies"
 msgstr ""
 
-#: templates/debug_toolbar/panels/request.html:50
+#: templates/debug_toolbar/panels/request.html:31
 msgid "Session data"
 msgstr ""
 
-#: templates/debug_toolbar/panels/request.html:72
+#: templates/debug_toolbar/panels/request.html:34
 msgid "No session data"
 msgstr ""
 
-#: templates/debug_toolbar/panels/request.html:76
+#: templates/debug_toolbar/panels/request.html:38
 msgid "GET data"
 msgstr ""
 
-#: templates/debug_toolbar/panels/request.html:98
+#: templates/debug_toolbar/panels/request.html:41
 msgid "No GET data"
 msgstr "אין נתוני GET"
 
-#: templates/debug_toolbar/panels/request.html:102
+#: templates/debug_toolbar/panels/request.html:45
 msgid "POST data"
 msgstr ""
 
-#: templates/debug_toolbar/panels/request.html:123
+#: templates/debug_toolbar/panels/request.html:48
 msgid "No POST data"
 msgstr "אין נתוני POST"
 
 #: templates/debug_toolbar/panels/settings.html:5
 msgid "Setting"
 msgstr ""
 
 #: templates/debug_toolbar/panels/signals.html:5
 msgid "Signal"
 msgstr "סיגנל"
 
 #: templates/debug_toolbar/panels/signals.html:6
-msgid "Providing"
-msgstr ""
-
-#: templates/debug_toolbar/panels/signals.html:7
 msgid "Receivers"
 msgstr ""
 
-#: templates/debug_toolbar/panels/sql.html:7
+#: templates/debug_toolbar/panels/sql.html:6
 #, python-format
 msgid "%(num)s query"
 msgid_plural "%(num)s queries"
 msgstr[0] ""
 msgstr[1] ""
 
-#: templates/debug_toolbar/panels/sql.html:18
+#: templates/debug_toolbar/panels/sql.html:8
+#, python-format
+msgid ""
+"including <abbr title=\"Similar queries are queries with the same SQL, but "
+"potentially different parameters.\">%(count)s similar</abbr>"
+msgstr ""
+
+#: templates/debug_toolbar/panels/sql.html:12
+#, python-format
+msgid ""
+"and <abbr title=\"Duplicate queries are identical to each other: they "
+"execute exactly the same SQL and parameters.\">%(dupes)s duplicates</abbr>"
+msgstr ""
+
+#: templates/debug_toolbar/panels/sql.html:34
 msgid "Query"
 msgstr ""
 
-#: templates/debug_toolbar/panels/sql.html:19
+#: templates/debug_toolbar/panels/sql.html:35
 #: templates/debug_toolbar/panels/timer.html:36
 msgid "Timeline"
 msgstr ""
 
-#: templates/debug_toolbar/panels/sql.html:21
-msgid "Action"
-msgstr "פעילות"
+#: templates/debug_toolbar/panels/sql.html:52
+#, python-format
+msgid "%(count)s similar queries."
+msgstr ""
 
-#: templates/debug_toolbar/panels/sql.html:64
+#: templates/debug_toolbar/panels/sql.html:58
+#, python-format
+msgid "Duplicated %(dupes)s times."
+msgstr ""
+
+#: templates/debug_toolbar/panels/sql.html:95
 msgid "Connection:"
 msgstr ""
 
-#: templates/debug_toolbar/panels/sql.html:66
+#: templates/debug_toolbar/panels/sql.html:97
 msgid "Isolation level:"
 msgstr ""
 
-#: templates/debug_toolbar/panels/sql.html:69
+#: templates/debug_toolbar/panels/sql.html:100
 msgid "Transaction status:"
 msgstr ""
 
-#: templates/debug_toolbar/panels/sql.html:83
+#: templates/debug_toolbar/panels/sql.html:114
 msgid "(unknown)"
 msgstr ""
 
-#: templates/debug_toolbar/panels/sql.html:92
+#: templates/debug_toolbar/panels/sql.html:123
 msgid "No SQL queries were recorded during this request."
 msgstr ""
 
-#: templates/debug_toolbar/panels/sql_explain.html:3
-#: templates/debug_toolbar/panels/sql_profile.html:3
-#: templates/debug_toolbar/panels/sql_select.html:3
-#: templates/debug_toolbar/panels/template_source.html:3
-msgid "Back"
-msgstr "חזרה"
-
 #: templates/debug_toolbar/panels/sql_explain.html:4
 msgid "SQL explained"
 msgstr ""
 
 #: templates/debug_toolbar/panels/sql_explain.html:9
 #: templates/debug_toolbar/panels/sql_profile.html:10
 #: templates/debug_toolbar/panels/sql_select.html:9
@@ -553,56 +548,56 @@
 msgid "SQL selected"
 msgstr ""
 
 #: templates/debug_toolbar/panels/sql_select.html:36
 msgid "Empty set"
 msgstr "קבוצה ריקה"
 
-#: templates/debug_toolbar/panels/staticfiles.html:4
+#: templates/debug_toolbar/panels/staticfiles.html:3
 msgid "Static file path"
 msgid_plural "Static file paths"
 msgstr[0] ""
 msgstr[1] ""
 
-#: templates/debug_toolbar/panels/staticfiles.html:8
+#: templates/debug_toolbar/panels/staticfiles.html:7
 #, python-format
 msgid "(prefix %(prefix)s)"
 msgstr ""
 
-#: templates/debug_toolbar/panels/staticfiles.html:12
-#: templates/debug_toolbar/panels/staticfiles.html:23
-#: templates/debug_toolbar/panels/staticfiles.html:35
+#: templates/debug_toolbar/panels/staticfiles.html:11
+#: templates/debug_toolbar/panels/staticfiles.html:22
+#: templates/debug_toolbar/panels/staticfiles.html:34
 #: templates/debug_toolbar/panels/templates.html:10
-#: templates/debug_toolbar/panels/templates.html:28
-#: templates/debug_toolbar/panels/templates.html:43
+#: templates/debug_toolbar/panels/templates.html:30
+#: templates/debug_toolbar/panels/templates.html:47
 msgid "None"
 msgstr ""
 
-#: templates/debug_toolbar/panels/staticfiles.html:15
+#: templates/debug_toolbar/panels/staticfiles.html:14
 msgid "Static file app"
 msgid_plural "Static file apps"
 msgstr[0] ""
 msgstr[1] ""
 
-#: templates/debug_toolbar/panels/staticfiles.html:26
+#: templates/debug_toolbar/panels/staticfiles.html:25
 msgid "Static file"
 msgid_plural "Static files"
 msgstr[0] ""
 msgstr[1] ""
 
-#: templates/debug_toolbar/panels/staticfiles.html:40
+#: templates/debug_toolbar/panels/staticfiles.html:39
 #, python-format
 msgid "%(payload_count)s file"
 msgid_plural "%(payload_count)s files"
 msgstr[0] ""
 msgstr[1] ""
 
 #: templates/debug_toolbar/panels/staticfiles.html:44
-msgid "Path"
-msgstr ""
+msgid "Location"
+msgstr "מקום"
 
 #: templates/debug_toolbar/panels/template_source.html:4
 msgid "Template source:"
 msgstr ""
 
 #: templates/debug_toolbar/panels/templates.html:2
 msgid "Template path"
@@ -612,20 +607,20 @@
 
 #: templates/debug_toolbar/panels/templates.html:13
 msgid "Template"
 msgid_plural "Templates"
 msgstr[0] ""
 msgstr[1] "תבנית"
 
-#: templates/debug_toolbar/panels/templates.html:21
-#: templates/debug_toolbar/panels/templates.html:37
+#: templates/debug_toolbar/panels/templates.html:22
+#: templates/debug_toolbar/panels/templates.html:40
 msgid "Toggle context"
 msgstr ""
 
-#: templates/debug_toolbar/panels/templates.html:31
+#: templates/debug_toolbar/panels/templates.html:33
 msgid "Context processor"
 msgid_plural "Context processors"
 msgstr[0] ""
 msgstr[1] ""
 
 #: templates/debug_toolbar/panels/timer.html:2
 msgid "Resource usage"
@@ -643,14 +638,35 @@
 msgid "Timing attribute"
 msgstr ""
 
 #: templates/debug_toolbar/panels/timer.html:37
 msgid "Milliseconds since navigation start (+length)"
 msgstr ""
 
-#: templates/debug_toolbar/panels/versions.html:5
+#: templates/debug_toolbar/panels/versions.html:10
+msgid "Package"
+msgstr ""
+
+#: templates/debug_toolbar/panels/versions.html:11
 msgid "Name"
 msgstr ""
 
-#: templates/debug_toolbar/panels/versions.html:6
+#: templates/debug_toolbar/panels/versions.html:12
 msgid "Version"
 msgstr ""
+
+#: templates/debug_toolbar/redirect.html:10
+msgid "Location:"
+msgstr ""
+
+#: templates/debug_toolbar/redirect.html:12
+msgid ""
+"The Django Debug Toolbar has intercepted a redirect to the above URL for "
+"debug viewing purposes. You can click the above link to continue with the "
+"redirect as normal."
+msgstr ""
+
+#: views.py:16
+msgid ""
+"Data for this panel isn't available anymore. Please reload the page and "
+"retry."
+msgstr ""
```

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/locale/id/LC_MESSAGES/django.mo` & `django_debug_toolbar-4.0.0/debug_toolbar/locale/id/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/locale/id/LC_MESSAGES/django.po` & `django_debug_toolbar-4.0.0/debug_toolbar/locale/ca/LC_MESSAGES/django.po`

 * *Files 10% similar despite different names*

```diff
@@ -1,357 +1,349 @@
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 #
 #
 # Translators:
-# Muhammad Panji <sumodirjo@gmail.com>, 2012
+# Libre El Chaval <el.libre@gmail.com>, 2013
 msgid ""
 msgstr ""
 "Project-Id-Version: Django Debug Toolbar\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2014-04-25 21:52+0200\n"
+"POT-Creation-Date: 2023-01-20 17:23+0100\n"
 "PO-Revision-Date: 2014-04-25 19:53+0000\n"
 "Last-Translator: Aymeric Augustin <aymeric.augustin@m4x.org>\n"
-"Language-Team: Indonesian (http://www.transifex.com/projects/p/django-debug-toolbar/language/id/)\n"
+"Language-Team: Catalan (http://www.transifex.com/projects/p/django-debug-"
+"toolbar/language/ca/)\n"
+"Language: ca\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: id\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: apps.py:11
+#: apps.py:15
 msgid "Debug Toolbar"
 msgstr ""
 
-#: views.py:14
-msgid ""
-"Data for this panel isn't available anymore. Please reload the page and "
-"retry."
-msgstr ""
-
-#: panels/cache.py:191
+#: panels/cache.py:180
 msgid "Cache"
-msgstr ""
+msgstr "Caxè"
 
-#: panels/cache.py:196
+#: panels/cache.py:186
 #, python-format
 msgid "%(cache_calls)d call in %(time).2fms"
 msgid_plural "%(cache_calls)d calls in %(time).2fms"
 msgstr[0] ""
+msgstr[1] ""
 
-#: panels/cache.py:204
+#: panels/cache.py:195
 #, python-format
 msgid "Cache calls from %(count)d backend"
 msgid_plural "Cache calls from %(count)d backends"
 msgstr[0] ""
+msgstr[1] ""
 
-#: panels/headers.py:35
+#: panels/headers.py:31
 msgid "Headers"
-msgstr ""
+msgstr "Encapçalaments"
 
-#: panels/logging.py:64
-msgid "Logging"
+#: panels/history/panel.py:18 panels/history/panel.py:19
+msgid "History"
 msgstr ""
 
-#: panels/logging.py:70
-#, python-format
-msgid "%(count)s message"
-msgid_plural "%(count)s messages"
-msgstr[0] "%(count)s pesan"
-
-#: panels/logging.py:73
-msgid "Log messages"
-msgstr ""
-
-#: panels/profiling.py:127
+#: panels/profiling.py:140
 msgid "Profiling"
 msgstr ""
 
-#: panels/redirects.py:17
+#: panels/redirects.py:14
 msgid "Intercept redirects"
 msgstr ""
 
-#: panels/request.py:18
+#: panels/request.py:16
 msgid "Request"
-msgstr ""
+msgstr "Demanar"
 
-#: panels/request.py:35
+#: panels/request.py:36
 msgid "<no view>"
 msgstr ""
 
-#: panels/request.py:47
+#: panels/request.py:53
 msgid "<unavailable>"
 msgstr ""
 
-#: panels/settings.py:20
+#: panels/settings.py:17
 msgid "Settings"
-msgstr "Pengaturan"
+msgstr "Configuració"
 
-#: panels/settings.py:23
-#, python-format
-msgid "Settings from <code>%s</code>"
-msgstr "Pengaturan dari <code>%s</code>"
+#: panels/settings.py:20
+#, fuzzy, python-format
+#| msgid "Settings"
+msgid "Settings from %s"
+msgstr "Configuració"
 
-#: panels/signals.py:45
+#: panels/signals.py:57
 #, python-format
 msgid "%(num_receivers)d receiver of 1 signal"
 msgid_plural "%(num_receivers)d receivers of 1 signal"
 msgstr[0] ""
+msgstr[1] ""
 
-#: panels/signals.py:48
+#: panels/signals.py:62
 #, python-format
 msgid "%(num_receivers)d receiver of %(num_signals)d signals"
 msgid_plural "%(num_receivers)d receivers of %(num_signals)d signals"
 msgstr[0] ""
+msgstr[1] ""
 
-#: panels/signals.py:53
+#: panels/signals.py:67
 msgid "Signals"
-msgstr "Sinyal"
+msgstr "Senyals"
+
+#: panels/sql/panel.py:23
+msgid "Autocommit"
+msgstr ""
+
+#: panels/sql/panel.py:24
+msgid "Read uncommitted"
+msgstr ""
+
+#: panels/sql/panel.py:25
+msgid "Read committed"
+msgstr ""
+
+#: panels/sql/panel.py:26
+msgid "Repeatable read"
+msgstr ""
+
+#: panels/sql/panel.py:27
+msgid "Serializable"
+msgstr "Seriable"
+
+#: panels/sql/panel.py:39
+msgid "Idle"
+msgstr ""
+
+#: panels/sql/panel.py:40
+msgid "Active"
+msgstr "Actiu"
+
+#: panels/sql/panel.py:41
+msgid "In transaction"
+msgstr "En transacció"
+
+#: panels/sql/panel.py:42
+msgid "In error"
+msgstr ""
+
+#: panels/sql/panel.py:43
+msgid "Unknown"
+msgstr "Desconegut"
+
+#: panels/sql/panel.py:130
+msgid "SQL"
+msgstr "SQL"
 
-#: panels/staticfiles.py:89
+#: panels/sql/panel.py:135
+#, python-format
+msgid "%(query_count)d query in %(sql_time).2fms"
+msgid_plural "%(query_count)d queries in %(sql_time).2fms"
+msgstr[0] ""
+msgstr[1] ""
+
+#: panels/sql/panel.py:147
+#, python-format
+msgid "SQL queries from %(count)d connection"
+msgid_plural "SQL queries from %(count)d connections"
+msgstr[0] ""
+msgstr[1] ""
+
+#: panels/staticfiles.py:84
 #, python-format
 msgid "Static files (%(num_found)s found, %(num_used)s used)"
 msgstr ""
 
-#: panels/staticfiles.py:107
+#: panels/staticfiles.py:105
 msgid "Static files"
-msgstr "Berkas statik"
+msgstr ""
 
-#: panels/staticfiles.py:112
+#: panels/staticfiles.py:111
 #, python-format
 msgid "%(num_used)s file used"
 msgid_plural "%(num_used)s files used"
 msgstr[0] ""
+msgstr[1] ""
+
+#: panels/templates/panel.py:143
+msgid "Templates"
+msgstr "Plantilles"
+
+#: panels/templates/panel.py:148
+#, python-format
+msgid "Templates (%(num_templates)s rendered)"
+msgstr ""
 
-#: panels/timer.py:23
+#: panels/templates/panel.py:180
+msgid "No origin"
+msgstr ""
+
+#: panels/timer.py:25
 #, python-format
 msgid "CPU: %(cum)0.2fms (%(total)0.2fms)"
-msgstr "CPU: %(cum)0.2fms (%(total)0.2fms)"
+msgstr ""
 
-#: panels/timer.py:28
+#: panels/timer.py:30
 #, python-format
 msgid "Total: %0.2fms"
-msgstr ""
+msgstr "Total: %0.2fms"
 
-#: panels/timer.py:34 templates/debug_toolbar/panels/logging.html:7
+#: panels/timer.py:36 templates/debug_toolbar/panels/history.html:9
 #: templates/debug_toolbar/panels/sql_explain.html:11
 #: templates/debug_toolbar/panels/sql_profile.html:12
 #: templates/debug_toolbar/panels/sql_select.html:11
 msgid "Time"
-msgstr "Waktu"
+msgstr "Hora"
 
-#: panels/timer.py:42
+#: panels/timer.py:44
 msgid "User CPU time"
-msgstr "CPU time pengguna"
+msgstr ""
 
-#: panels/timer.py:42
+#: panels/timer.py:44
 #, python-format
 msgid "%(utime)0.3f msec"
 msgstr ""
 
-#: panels/timer.py:43
+#: panels/timer.py:45
 msgid "System CPU time"
-msgstr "CPU time sistem"
+msgstr ""
 
-#: panels/timer.py:43
+#: panels/timer.py:45
 #, python-format
 msgid "%(stime)0.3f msec"
 msgstr ""
 
-#: panels/timer.py:44
+#: panels/timer.py:46
 msgid "Total CPU time"
-msgstr "CPU time total"
+msgstr ""
 
-#: panels/timer.py:44
+#: panels/timer.py:46
 #, python-format
 msgid "%(total)0.3f msec"
 msgstr ""
 
-#: panels/timer.py:45
+#: panels/timer.py:47
 msgid "Elapsed time"
-msgstr "Waktu terlampaui"
+msgstr "Temps emprat"
 
-#: panels/timer.py:45
+#: panels/timer.py:47
 #, python-format
 msgid "%(total_time)0.3f msec"
 msgstr ""
 
-#: panels/timer.py:46
+#: panels/timer.py:49
 msgid "Context switches"
 msgstr ""
 
-#: panels/timer.py:46
+#: panels/timer.py:50
 #, python-format
 msgid "%(vcsw)d voluntary, %(ivcsw)d involuntary"
 msgstr ""
 
-#: panels/versions.py:25
+#: panels/versions.py:19
 msgid "Versions"
-msgstr "Versi"
-
-#: panels/sql/panel.py:22
-msgid "Autocommit"
-msgstr ""
-
-#: panels/sql/panel.py:23
-msgid "Read uncommitted"
-msgstr ""
-
-#: panels/sql/panel.py:24
-msgid "Read committed"
-msgstr ""
-
-#: panels/sql/panel.py:25
-msgid "Repeatable read"
-msgstr ""
-
-#: panels/sql/panel.py:26
-msgid "Serializable"
-msgstr "Variabel"
-
-#: panels/sql/panel.py:37
-msgid "Idle"
-msgstr ""
-
-#: panels/sql/panel.py:38
-msgid "Active"
-msgstr "Aksi"
-
-#: panels/sql/panel.py:39
-msgid "In transaction"
-msgstr "Status transaksi:"
-
-#: panels/sql/panel.py:40
-msgid "In error"
-msgstr ""
-
-#: panels/sql/panel.py:41
-msgid "Unknown"
-msgstr "(tidak diketahui)"
-
-#: panels/sql/panel.py:105
-msgid "SQL"
-msgstr "SQL"
+msgstr "Versions"
 
-#: panels/templates/panel.py:141
-msgid "Templates"
-msgstr "Template"
-
-#: panels/templates/panel.py:146
-#, python-format
-msgid "Templates (%(num_templates)s rendered)"
-msgstr ""
-
-#: templates/debug_toolbar/base.html:19
+#: templates/debug_toolbar/base.html:22
 msgid "Hide toolbar"
-msgstr ""
+msgstr "Amagar barra d'eina"
 
-#: templates/debug_toolbar/base.html:19
+#: templates/debug_toolbar/base.html:22
 msgid "Hide"
-msgstr "Menyembunyikan"
+msgstr "Amagar"
 
-#: templates/debug_toolbar/base.html:25
-msgid "Disable for next and successive requests"
-msgstr ""
-
-#: templates/debug_toolbar/base.html:25
-msgid "Enable for next and successive requests"
-msgstr ""
-
-#: templates/debug_toolbar/base.html:47
+#: templates/debug_toolbar/base.html:29
 msgid "Show toolbar"
-msgstr ""
-
-#: templates/debug_toolbar/base.html:53
-msgid "Close"
-msgstr "Menutup"
+msgstr "Mostrar barra d'eines"
 
-#: templates/debug_toolbar/redirect.html:8
-msgid "Location:"
+#: templates/debug_toolbar/includes/panel_button.html:4
+msgid "Disable for next and successive requests"
 msgstr ""
 
-#: templates/debug_toolbar/redirect.html:10
-msgid ""
-"The Django Debug Toolbar has intercepted a redirect to the above URL for "
-"debug viewing purposes. You can click the above link to continue with the "
-"redirect as normal."
+#: templates/debug_toolbar/includes/panel_button.html:4
+msgid "Enable for next and successive requests"
 msgstr ""
 
 #: templates/debug_toolbar/panels/cache.html:2
 msgid "Summary"
-msgstr ""
+msgstr "Resum"
 
 #: templates/debug_toolbar/panels/cache.html:6
 msgid "Total calls"
-msgstr ""
+msgstr "Total crides"
 
 #: templates/debug_toolbar/panels/cache.html:7
 msgid "Total time"
-msgstr ""
+msgstr "Total temps"
 
 #: templates/debug_toolbar/panels/cache.html:8
 msgid "Cache hits"
 msgstr ""
 
 #: templates/debug_toolbar/panels/cache.html:9
 msgid "Cache misses"
 msgstr ""
 
 #: templates/debug_toolbar/panels/cache.html:21
 msgid "Commands"
-msgstr ""
+msgstr "Comandes"
 
 #: templates/debug_toolbar/panels/cache.html:39
 msgid "Calls"
-msgstr ""
+msgstr "Crides"
 
 #: templates/debug_toolbar/panels/cache.html:43
-#: templates/debug_toolbar/panels/sql.html:20
+#: templates/debug_toolbar/panels/sql.html:36
 msgid "Time (ms)"
-msgstr "Waktu (milidetik)"
+msgstr "Temps (ms)"
 
 #: templates/debug_toolbar/panels/cache.html:44
 msgid "Type"
-msgstr "Jenis"
+msgstr "Tipus"
 
 #: templates/debug_toolbar/panels/cache.html:45
 #: templates/debug_toolbar/panels/request.html:8
 msgid "Arguments"
 msgstr ""
 
 #: templates/debug_toolbar/panels/cache.html:46
 #: templates/debug_toolbar/panels/request.html:9
 msgid "Keyword arguments"
 msgstr ""
 
 #: templates/debug_toolbar/panels/cache.html:47
 msgid "Backend"
-msgstr ""
+msgstr "Administració"
 
 #: templates/debug_toolbar/panels/headers.html:3
 msgid "Request headers"
 msgstr ""
 
 #: templates/debug_toolbar/panels/headers.html:8
 #: templates/debug_toolbar/panels/headers.html:27
 #: templates/debug_toolbar/panels/headers.html:48
 msgid "Key"
-msgstr "Kunci"
+msgstr "Clau"
 
 #: templates/debug_toolbar/panels/headers.html:9
 #: templates/debug_toolbar/panels/headers.html:28
 #: templates/debug_toolbar/panels/headers.html:49
-#: templates/debug_toolbar/panels/request.html:33
-#: templates/debug_toolbar/panels/request.html:59
-#: templates/debug_toolbar/panels/request.html:85
-#: templates/debug_toolbar/panels/request.html:110
+#: templates/debug_toolbar/panels/history_tr.html:23
+#: templates/debug_toolbar/panels/request_variables.html:12
 #: templates/debug_toolbar/panels/settings.html:6
 #: templates/debug_toolbar/panels/timer.html:11
 msgid "Value"
-msgstr "Nilai"
+msgstr "Valor"
 
 #: templates/debug_toolbar/panels/headers.html:22
 msgid "Response headers"
 msgstr ""
 
 #: templates/debug_toolbar/panels/headers.html:41
 msgid "WSGI environ"
@@ -359,284 +351,323 @@
 
 #: templates/debug_toolbar/panels/headers.html:43
 msgid ""
 "Since the WSGI environ inherits the environment of the server, only a "
 "significant subset is shown below."
 msgstr ""
 
-#: templates/debug_toolbar/panels/logging.html:6
-msgid "Level"
-msgstr "Tingkat"
-
-#: templates/debug_toolbar/panels/logging.html:8
-msgid "Channel"
-msgstr "Kanal"
-
-#: templates/debug_toolbar/panels/logging.html:9
-msgid "Message"
-msgstr "Pesan"
+#: templates/debug_toolbar/panels/history.html:10
+msgid "Method"
+msgstr ""
 
-#: templates/debug_toolbar/panels/logging.html:10
-#: templates/debug_toolbar/panels/staticfiles.html:45
-msgid "Location"
-msgstr "Lokasi"
+#: templates/debug_toolbar/panels/history.html:11
+#: templates/debug_toolbar/panels/staticfiles.html:43
+msgid "Path"
+msgstr ""
+
+#: templates/debug_toolbar/panels/history.html:12
+#, fuzzy
+#| msgid "Variable"
+msgid "Request Variables"
+msgstr "Variable"
 
-#: templates/debug_toolbar/panels/logging.html:26
-msgid "No messages logged"
-msgstr "Tidak ada pesan yang dicatat"
+#: templates/debug_toolbar/panels/history.html:13
+msgid "Status"
+msgstr ""
+
+#: templates/debug_toolbar/panels/history.html:14
+#: templates/debug_toolbar/panels/sql.html:37
+msgid "Action"
+msgstr "Acció"
+
+#: templates/debug_toolbar/panels/history_tr.html:22
+#: templates/debug_toolbar/panels/request_variables.html:11
+msgid "Variable"
+msgstr "Variable"
 
 #: templates/debug_toolbar/panels/profiling.html:5
 msgid "Call"
-msgstr "Panggil"
+msgstr "Cridar"
 
 #: templates/debug_toolbar/panels/profiling.html:6
 msgid "CumTime"
-msgstr "CumTime"
+msgstr ""
 
 #: templates/debug_toolbar/panels/profiling.html:7
 #: templates/debug_toolbar/panels/profiling.html:9
 msgid "Per"
 msgstr "Per"
 
 #: templates/debug_toolbar/panels/profiling.html:8
 msgid "TotTime"
-msgstr "TotTime"
+msgstr "TempsTotal"
 
 #: templates/debug_toolbar/panels/profiling.html:10
 msgid "Count"
-msgstr "Hitung"
+msgstr "Recomptar"
 
 #: templates/debug_toolbar/panels/request.html:3
 msgid "View information"
-msgstr "Lihat informasi"
+msgstr "Veure informació"
 
 #: templates/debug_toolbar/panels/request.html:7
 msgid "View function"
 msgstr ""
 
 #: templates/debug_toolbar/panels/request.html:10
 msgid "URL name"
 msgstr ""
 
 #: templates/debug_toolbar/panels/request.html:24
 msgid "Cookies"
 msgstr ""
 
-#: templates/debug_toolbar/panels/request.html:32
-#: templates/debug_toolbar/panels/request.html:58
-#: templates/debug_toolbar/panels/request.html:84
-#: templates/debug_toolbar/panels/request.html:109
-msgid "Variable"
-msgstr "Variabel"
-
-#: templates/debug_toolbar/panels/request.html:46
+#: templates/debug_toolbar/panels/request.html:27
 msgid "No cookies"
 msgstr ""
 
-#: templates/debug_toolbar/panels/request.html:50
+#: templates/debug_toolbar/panels/request.html:31
 msgid "Session data"
 msgstr ""
 
-#: templates/debug_toolbar/panels/request.html:72
+#: templates/debug_toolbar/panels/request.html:34
 msgid "No session data"
 msgstr ""
 
-#: templates/debug_toolbar/panels/request.html:76
+#: templates/debug_toolbar/panels/request.html:38
 msgid "GET data"
 msgstr ""
 
-#: templates/debug_toolbar/panels/request.html:98
+#: templates/debug_toolbar/panels/request.html:41
 msgid "No GET data"
-msgstr "Tidak ada data GET"
+msgstr "Sense dades GET"
 
-#: templates/debug_toolbar/panels/request.html:102
+#: templates/debug_toolbar/panels/request.html:45
 msgid "POST data"
 msgstr ""
 
-#: templates/debug_toolbar/panels/request.html:123
+#: templates/debug_toolbar/panels/request.html:48
 msgid "No POST data"
-msgstr "Tidak ada data POST"
+msgstr "Sense dades POST"
 
 #: templates/debug_toolbar/panels/settings.html:5
 msgid "Setting"
-msgstr "Pengaturan"
+msgstr "Configuració"
 
 #: templates/debug_toolbar/panels/signals.html:5
 msgid "Signal"
-msgstr "Sinyal"
+msgstr "Senyal"
 
 #: templates/debug_toolbar/panels/signals.html:6
-msgid "Providing"
-msgstr ""
-
-#: templates/debug_toolbar/panels/signals.html:7
 msgid "Receivers"
-msgstr "Penerima"
+msgstr "Destinataris"
 
-#: templates/debug_toolbar/panels/sql.html:7
+#: templates/debug_toolbar/panels/sql.html:6
 #, python-format
 msgid "%(num)s query"
 msgid_plural "%(num)s queries"
 msgstr[0] ""
+msgstr[1] ""
 
-#: templates/debug_toolbar/panels/sql.html:18
-msgid "Query"
+#: templates/debug_toolbar/panels/sql.html:8
+#, python-format
+msgid ""
+"including <abbr title=\"Similar queries are queries with the same SQL, but "
+"potentially different parameters.\">%(count)s similar</abbr>"
 msgstr ""
 
-#: templates/debug_toolbar/panels/sql.html:19
+#: templates/debug_toolbar/panels/sql.html:12
+#, python-format
+msgid ""
+"and <abbr title=\"Duplicate queries are identical to each other: they "
+"execute exactly the same SQL and parameters.\">%(dupes)s duplicates</abbr>"
+msgstr ""
+
+#: templates/debug_toolbar/panels/sql.html:34
+msgid "Query"
+msgstr "Petició"
+
+#: templates/debug_toolbar/panels/sql.html:35
 #: templates/debug_toolbar/panels/timer.html:36
 msgid "Timeline"
+msgstr "Línia temporal"
+
+#: templates/debug_toolbar/panels/sql.html:52
+#, python-format
+msgid "%(count)s similar queries."
 msgstr ""
 
-#: templates/debug_toolbar/panels/sql.html:21
-msgid "Action"
-msgstr "Aksi"
+#: templates/debug_toolbar/panels/sql.html:58
+#, python-format
+msgid "Duplicated %(dupes)s times."
+msgstr ""
 
-#: templates/debug_toolbar/panels/sql.html:64
+#: templates/debug_toolbar/panels/sql.html:95
 msgid "Connection:"
-msgstr "Koneksi:"
+msgstr "Connexió:"
 
-#: templates/debug_toolbar/panels/sql.html:66
+#: templates/debug_toolbar/panels/sql.html:97
 msgid "Isolation level:"
-msgstr "Tingkat isolasi:"
+msgstr ""
 
-#: templates/debug_toolbar/panels/sql.html:69
+#: templates/debug_toolbar/panels/sql.html:100
 msgid "Transaction status:"
-msgstr "Status transaksi:"
+msgstr ""
 
-#: templates/debug_toolbar/panels/sql.html:83
+#: templates/debug_toolbar/panels/sql.html:114
 msgid "(unknown)"
-msgstr "(tidak diketahui)"
+msgstr "(desconegut)"
 
-#: templates/debug_toolbar/panels/sql.html:92
+#: templates/debug_toolbar/panels/sql.html:123
 msgid "No SQL queries were recorded during this request."
 msgstr ""
 
-#: templates/debug_toolbar/panels/sql_explain.html:3
-#: templates/debug_toolbar/panels/sql_profile.html:3
-#: templates/debug_toolbar/panels/sql_select.html:3
-#: templates/debug_toolbar/panels/template_source.html:3
-msgid "Back"
-msgstr "Kembali"
-
 #: templates/debug_toolbar/panels/sql_explain.html:4
 msgid "SQL explained"
 msgstr ""
 
 #: templates/debug_toolbar/panels/sql_explain.html:9
 #: templates/debug_toolbar/panels/sql_profile.html:10
 #: templates/debug_toolbar/panels/sql_select.html:9
 msgid "Executed SQL"
-msgstr "SQL Tereksekusi"
+msgstr "SQL Executat"
 
 #: templates/debug_toolbar/panels/sql_explain.html:13
 #: templates/debug_toolbar/panels/sql_profile.html:14
 #: templates/debug_toolbar/panels/sql_select.html:13
 msgid "Database"
-msgstr "Basis data"
+msgstr "Base de dades"
 
 #: templates/debug_toolbar/panels/sql_profile.html:4
 msgid "SQL profiled"
 msgstr ""
 
 #: templates/debug_toolbar/panels/sql_profile.html:37
 msgid "Error"
-msgstr ""
+msgstr "Error"
 
 #: templates/debug_toolbar/panels/sql_select.html:4
 msgid "SQL selected"
 msgstr ""
 
 #: templates/debug_toolbar/panels/sql_select.html:36
 msgid "Empty set"
-msgstr "Himpunan kosong"
+msgstr ""
 
-#: templates/debug_toolbar/panels/staticfiles.html:4
+#: templates/debug_toolbar/panels/staticfiles.html:3
 msgid "Static file path"
 msgid_plural "Static file paths"
 msgstr[0] ""
+msgstr[1] ""
 
-#: templates/debug_toolbar/panels/staticfiles.html:8
+#: templates/debug_toolbar/panels/staticfiles.html:7
 #, python-format
 msgid "(prefix %(prefix)s)"
 msgstr ""
 
-#: templates/debug_toolbar/panels/staticfiles.html:12
-#: templates/debug_toolbar/panels/staticfiles.html:23
-#: templates/debug_toolbar/panels/staticfiles.html:35
+#: templates/debug_toolbar/panels/staticfiles.html:11
+#: templates/debug_toolbar/panels/staticfiles.html:22
+#: templates/debug_toolbar/panels/staticfiles.html:34
 #: templates/debug_toolbar/panels/templates.html:10
-#: templates/debug_toolbar/panels/templates.html:28
-#: templates/debug_toolbar/panels/templates.html:43
+#: templates/debug_toolbar/panels/templates.html:30
+#: templates/debug_toolbar/panels/templates.html:47
 msgid "None"
-msgstr "Tidak ada"
+msgstr "Cap"
 
-#: templates/debug_toolbar/panels/staticfiles.html:15
+#: templates/debug_toolbar/panels/staticfiles.html:14
 msgid "Static file app"
 msgid_plural "Static file apps"
 msgstr[0] ""
+msgstr[1] ""
 
-#: templates/debug_toolbar/panels/staticfiles.html:26
+#: templates/debug_toolbar/panels/staticfiles.html:25
 msgid "Static file"
 msgid_plural "Static files"
-msgstr[0] "Berkas statik"
+msgstr[0] ""
+msgstr[1] ""
 
-#: templates/debug_toolbar/panels/staticfiles.html:40
+#: templates/debug_toolbar/panels/staticfiles.html:39
 #, python-format
 msgid "%(payload_count)s file"
 msgid_plural "%(payload_count)s files"
 msgstr[0] ""
+msgstr[1] ""
 
 #: templates/debug_toolbar/panels/staticfiles.html:44
-msgid "Path"
-msgstr ""
+msgid "Location"
+msgstr "Ubicació"
 
 #: templates/debug_toolbar/panels/template_source.html:4
 msgid "Template source:"
 msgstr ""
 
 #: templates/debug_toolbar/panels/templates.html:2
 msgid "Template path"
 msgid_plural "Template paths"
-msgstr[0] "Template path"
+msgstr[0] ""
+msgstr[1] ""
 
 #: templates/debug_toolbar/panels/templates.html:13
 msgid "Template"
 msgid_plural "Templates"
 msgstr[0] ""
+msgstr[1] "Plantilles"
 
-#: templates/debug_toolbar/panels/templates.html:21
-#: templates/debug_toolbar/panels/templates.html:37
+#: templates/debug_toolbar/panels/templates.html:22
+#: templates/debug_toolbar/panels/templates.html:40
 msgid "Toggle context"
 msgstr ""
 
-#: templates/debug_toolbar/panels/templates.html:31
+#: templates/debug_toolbar/panels/templates.html:33
 msgid "Context processor"
 msgid_plural "Context processors"
 msgstr[0] ""
+msgstr[1] ""
 
 #: templates/debug_toolbar/panels/timer.html:2
 msgid "Resource usage"
 msgstr ""
 
 #: templates/debug_toolbar/panels/timer.html:10
 msgid "Resource"
-msgstr "Sumber daya"
+msgstr "Font"
 
 #: templates/debug_toolbar/panels/timer.html:26
 msgid "Browser timing"
 msgstr ""
 
 #: templates/debug_toolbar/panels/timer.html:35
 msgid "Timing attribute"
 msgstr ""
 
 #: templates/debug_toolbar/panels/timer.html:37
 msgid "Milliseconds since navigation start (+length)"
 msgstr ""
 
-#: templates/debug_toolbar/panels/versions.html:5
-msgid "Name"
+#: templates/debug_toolbar/panels/versions.html:10
+msgid "Package"
 msgstr ""
 
-#: templates/debug_toolbar/panels/versions.html:6
+#: templates/debug_toolbar/panels/versions.html:11
+msgid "Name"
+msgstr "Nom"
+
+#: templates/debug_toolbar/panels/versions.html:12
 msgid "Version"
-msgstr "Versi"
+msgstr "Versió"
+
+#: templates/debug_toolbar/redirect.html:10
+msgid "Location:"
+msgstr "Ubicació:"
+
+#: templates/debug_toolbar/redirect.html:12
+msgid ""
+"The Django Debug Toolbar has intercepted a redirect to the above URL for "
+"debug viewing purposes. You can click the above link to continue with the "
+"redirect as normal."
+msgstr ""
+
+#: views.py:16
+msgid ""
+"Data for this panel isn't available anymore. Please reload the page and "
+"retry."
+msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/locale/it/LC_MESSAGES/django.mo` & `django_debug_toolbar-4.0.0/debug_toolbar/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/locale/it/LC_MESSAGES/django.po` & `django_debug_toolbar-4.0.0/debug_toolbar/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files 4% similar despite different names*

```diff
@@ -1,431 +1,402 @@
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 #
 #
 # Translators:
-# Dario Agliottone <dario.agliottone@gmail.com>, 2012
-# Flavio Curella <flavio.curella@gmail.com>, 2013
-# yakky <i.spalletti@nephila.it>, 2013-2014
+# Fábio <bnafta@gmail.com>, 2013-2014
+# Percy Pérez-Pinedo, 2009
 msgid ""
 msgstr ""
 "Project-Id-Version: Django Debug Toolbar\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-08-14 10:25-0500\n"
-"PO-Revision-Date: 2021-08-14 15:25+0000\n"
-"Last-Translator: Tim Schilling\n"
-"Language-Team: Italian (http://www.transifex.com/django-debug-toolbar/django-debug-toolbar/language/it/)\n"
+"POT-Creation-Date: 2023-01-20 17:23+0100\n"
+"PO-Revision-Date: 2014-04-25 19:53+0000\n"
+"Last-Translator: Aymeric Augustin <aymeric.augustin@m4x.org>\n"
+"Language-Team: Portuguese (Brazil) (http://www.transifex.com/projects/p/"
+"django-debug-toolbar/language/pt_BR/)\n"
+"Language: pt_BR\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: it\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
 #: apps.py:15
 msgid "Debug Toolbar"
 msgstr ""
 
-#: panels/cache.py:227
+#: panels/cache.py:180
 msgid "Cache"
 msgstr "Cache"
 
-#: panels/cache.py:234
+#: panels/cache.py:186
 #, python-format
 msgid "%(cache_calls)d call in %(time).2fms"
 msgid_plural "%(cache_calls)d calls in %(time).2fms"
-msgstr[0] "%(cache_calls)d chiamata in %(time).2fms"
-msgstr[1] "%(cache_calls)d chiamate in %(time).2fms"
+msgstr[0] "%(cache_calls)d chamada em %(time).2fms"
+msgstr[1] "%(cache_calls)d chamadas em %(time).2fms"
 
-#: panels/cache.py:246
+#: panels/cache.py:195
 #, python-format
 msgid "Cache calls from %(count)d backend"
 msgid_plural "Cache calls from %(count)d backends"
-msgstr[0] "Chiamate alla cache da %(count)d backend"
-msgstr[1] "Chiamate alla cache da %(count)d backend"
+msgstr[0] "Chamadas ao cache de %(count)d backend"
+msgstr[1] "Chamadas ao cache de %(count)d backends"
 
-#: panels/headers.py:33
+#: panels/headers.py:31
 msgid "Headers"
-msgstr "Intestazioni"
+msgstr "Cabeçalhos"
 
-#: panels/history/panel.py:20 panels/history/panel.py:21
+#: panels/history/panel.py:18 panels/history/panel.py:19
 msgid "History"
 msgstr ""
 
-#: panels/logging.py:63
-msgid "Logging"
-msgstr "Logging"
-
-#: panels/logging.py:69
-#, python-format
-msgid "%(count)s message"
-msgid_plural "%(count)s messages"
-msgstr[0] "%(count)s messaggio"
-msgstr[1] "%(count)s messaggi"
-
-#: panels/logging.py:73
-msgid "Log messages"
-msgstr "Messaggi di log"
-
-#: panels/profiling.py:150
+#: panels/profiling.py:140
 msgid "Profiling"
-msgstr "Profilazione"
+msgstr "Profiling"
 
 #: panels/redirects.py:14
 msgid "Intercept redirects"
-msgstr "Intercetta ridirezioni"
+msgstr "Interceptar redirecionamentos"
 
 #: panels/request.py:16
 msgid "Request"
-msgstr "Request"
+msgstr "Requisição"
 
 #: panels/request.py:36
 msgid "<no view>"
-msgstr "<nessuna view>"
+msgstr "<nenhuma vista>"
 
 #: panels/request.py:53
 msgid "<unavailable>"
-msgstr "<non disponibile>"
+msgstr "<indisponível>"
 
-#: panels/settings.py:24
+#: panels/settings.py:17
 msgid "Settings"
-msgstr "Impostazioni"
+msgstr "Configurações"
 
-#: panels/settings.py:27
-#, python-format
+#: panels/settings.py:20
+#, fuzzy, python-format
+#| msgid "Settings from <code>%s</code>"
 msgid "Settings from %s"
-msgstr ""
+msgstr "Configurações em: <code>%s</code>"
 
-#: panels/signals.py:58
+#: panels/signals.py:57
 #, python-format
 msgid "%(num_receivers)d receiver of 1 signal"
 msgid_plural "%(num_receivers)d receivers of 1 signal"
-msgstr[0] "%(num_receivers)d ricevitore di 1 segnale"
-msgstr[1] "%(num_receivers)d ricevitori di 1 segnale"
+msgstr[0] "%(num_receivers)d receptor de 1 sinal"
+msgstr[1] "%(num_receivers)d receptores de 1 sinal"
 
-#: panels/signals.py:66
+#: panels/signals.py:62
 #, python-format
 msgid "%(num_receivers)d receiver of %(num_signals)d signals"
 msgid_plural "%(num_receivers)d receivers of %(num_signals)d signals"
-msgstr[0] "%(num_receivers)d ricevitore di %(num_signals)d segnali"
-msgstr[1] "%(num_receivers)d ricevitori di %(num_signals)d segnali"
+msgstr[0] "%(num_receivers)d receptor de %(num_signals)d sinais"
+msgstr[1] "%(num_receivers)d receptores de %(num_signals)d sinais"
 
-#: panels/signals.py:73
+#: panels/signals.py:67
 msgid "Signals"
-msgstr "Segnali"
+msgstr "Sinais"
 
-#: panels/sql/panel.py:24
+#: panels/sql/panel.py:23
 msgid "Autocommit"
 msgstr "Autocommit"
 
-#: panels/sql/panel.py:25
+#: panels/sql/panel.py:24
 msgid "Read uncommitted"
 msgstr "Read uncommitted"
 
-#: panels/sql/panel.py:26
+#: panels/sql/panel.py:25
 msgid "Read committed"
 msgstr "Read committed"
 
-#: panels/sql/panel.py:27
+#: panels/sql/panel.py:26
 msgid "Repeatable read"
-msgstr "Repeatable read"
+msgstr "Leitura repetida"
 
-#: panels/sql/panel.py:28
+#: panels/sql/panel.py:27
 msgid "Serializable"
-msgstr "Serializable"
+msgstr "Variável"
 
-#: panels/sql/panel.py:40
+#: panels/sql/panel.py:39
 msgid "Idle"
-msgstr "Idle"
+msgstr "Ocioso"
 
-#: panels/sql/panel.py:41
+#: panels/sql/panel.py:40
 msgid "Active"
-msgstr "Azione"
+msgstr "Ação"
 
-#: panels/sql/panel.py:42
+#: panels/sql/panel.py:41
 msgid "In transaction"
-msgstr "Stato transazione:"
+msgstr "Na transação"
 
-#: panels/sql/panel.py:43
+#: panels/sql/panel.py:42
 msgid "In error"
-msgstr "Errore"
+msgstr "Erro"
 
-#: panels/sql/panel.py:44
+#: panels/sql/panel.py:43
 msgid "Unknown"
-msgstr "(sconosciuto)"
+msgstr "Desconhecido"
 
-#: panels/sql/panel.py:109
+#: panels/sql/panel.py:130
 msgid "SQL"
 msgstr "SQL"
 
-#: panels/sql/panel.py:114
-#, python-format
+#: panels/sql/panel.py:135
+#, fuzzy, python-format
+#| msgid "%(cache_calls)d call in %(time).2fms"
+#| msgid_plural "%(cache_calls)d calls in %(time).2fms"
 msgid "%(query_count)d query in %(sql_time).2fms"
 msgid_plural "%(query_count)d queries in %(sql_time).2fms"
-msgstr[0] ""
-msgstr[1] ""
+msgstr[0] "%(cache_calls)d chamada em %(time).2fms"
+msgstr[1] "%(cache_calls)d chamadas em %(time).2fms"
 
-#: panels/sql/panel.py:127
+#: panels/sql/panel.py:147
 #, python-format
 msgid "SQL queries from %(count)d connection"
 msgid_plural "SQL queries from %(count)d connections"
 msgstr[0] ""
 msgstr[1] ""
 
-#: panels/staticfiles.py:85
+#: panels/staticfiles.py:84
 #, python-format
 msgid "Static files (%(num_found)s found, %(num_used)s used)"
-msgstr "File statici (%(num_found)s trovati, %(num_used)s usati)"
+msgstr ""
+"Arquivos estáticos (%(num_found)s encontrados, %(num_used)s sendo utilizados)"
 
-#: panels/staticfiles.py:106
+#: panels/staticfiles.py:105
 msgid "Static files"
-msgstr "Files statici"
+msgstr "Arquivos estáticos"
 
-#: panels/staticfiles.py:112
+#: panels/staticfiles.py:111
 #, python-format
 msgid "%(num_used)s file used"
 msgid_plural "%(num_used)s files used"
-msgstr[0] "%(num_used)s file usato"
-msgstr[1] "%(num_used)s file usati"
+msgstr[0] "%(num_used)s arquivo utilizado"
+msgstr[1] "%(num_used)s arquivos utilizados"
 
-#: panels/templates/panel.py:144
+#: panels/templates/panel.py:143
 msgid "Templates"
-msgstr "Template"
+msgstr "Templates"
 
-#: panels/templates/panel.py:149
+#: panels/templates/panel.py:148
 #, python-format
 msgid "Templates (%(num_templates)s rendered)"
-msgstr "Templates (%(num_templates)s rendered)"
+msgstr "Templates (%(num_templates)s renderizados)"
 
-#: panels/templates/panel.py:181
+#: panels/templates/panel.py:180
 msgid "No origin"
 msgstr ""
 
 #: panels/timer.py:25
 #, python-format
 msgid "CPU: %(cum)0.2fms (%(total)0.2fms)"
 msgstr "CPU: %(cum)0.2fms (%(total)0.2fms)"
 
 #: panels/timer.py:30
 #, python-format
 msgid "Total: %0.2fms"
-msgstr "Totale: %0.2fms"
+msgstr "Total: %0.2fms"
 
 #: panels/timer.py:36 templates/debug_toolbar/panels/history.html:9
-#: templates/debug_toolbar/panels/logging.html:7
 #: templates/debug_toolbar/panels/sql_explain.html:11
 #: templates/debug_toolbar/panels/sql_profile.html:12
 #: templates/debug_toolbar/panels/sql_select.html:11
 msgid "Time"
 msgstr "Tempo"
 
 #: panels/timer.py:44
 msgid "User CPU time"
-msgstr "Tempo CPU utente"
+msgstr "Tempo de CPU do usuário"
 
 #: panels/timer.py:44
 #, python-format
 msgid "%(utime)0.3f msec"
-msgstr "%(utime)0.3f msec"
+msgstr "%(utime)0.3f ms"
 
 #: panels/timer.py:45
 msgid "System CPU time"
-msgstr "Tempo CPU sistema"
+msgstr "Tempo de CPU do sistema"
 
 #: panels/timer.py:45
 #, python-format
 msgid "%(stime)0.3f msec"
-msgstr "%(stime)0.3f msec"
+msgstr "%(stime)0.3f ms"
 
 #: panels/timer.py:46
 msgid "Total CPU time"
-msgstr "Tempo Totale CPU"
+msgstr "Tempo total de CPU"
 
 #: panels/timer.py:46
 #, python-format
 msgid "%(total)0.3f msec"
-msgstr "%(total)0.3f msec"
+msgstr "%(total)0.3f ms"
 
 #: panels/timer.py:47
 msgid "Elapsed time"
-msgstr "Tempo Trascorso"
+msgstr "Tempo decorrido"
 
 #: panels/timer.py:47
 #, python-format
 msgid "%(total_time)0.3f msec"
-msgstr "%(total_time)0.3f msec"
+msgstr "%(total_time)0.3f ms"
 
 #: panels/timer.py:49
 msgid "Context switches"
-msgstr "Cambi di contesto"
+msgstr "Mudanças de contexto"
 
 #: panels/timer.py:50
 #, python-format
 msgid "%(vcsw)d voluntary, %(ivcsw)d involuntary"
-msgstr "%(vcsw)d volontario, %(ivcsw)d involontario"
+msgstr "%(vcsw)d voluntário, %(ivcsw)d involuntário"
 
 #: panels/versions.py:19
 msgid "Versions"
-msgstr "Versioni"
+msgstr "Versões"
 
-#: templates/debug_toolbar/base.html:18
+#: templates/debug_toolbar/base.html:22
 msgid "Hide toolbar"
-msgstr "Nascondi Toolbar"
+msgstr "Ocultar barra de ferramentas"
 
-#: templates/debug_toolbar/base.html:18
+#: templates/debug_toolbar/base.html:22
 msgid "Hide"
-msgstr "Nascondi"
+msgstr "Esconder"
 
-#: templates/debug_toolbar/base.html:25
+#: templates/debug_toolbar/base.html:29
 msgid "Show toolbar"
-msgstr "Mostra Toolbar"
+msgstr "Mostrar barra de ferramentas"
 
 #: templates/debug_toolbar/includes/panel_button.html:4
 msgid "Disable for next and successive requests"
-msgstr "Disattiva per la prossima requests e le successive"
+msgstr "Desativar para próximas requisições"
 
 #: templates/debug_toolbar/includes/panel_button.html:4
 msgid "Enable for next and successive requests"
-msgstr "Abilita per la prossima requests e le successive"
+msgstr "Habilitar para próximas requisições"
 
 #: templates/debug_toolbar/panels/cache.html:2
 msgid "Summary"
-msgstr "Sommario"
+msgstr "Resumo"
 
 #: templates/debug_toolbar/panels/cache.html:6
 msgid "Total calls"
-msgstr "Chiamate totali"
+msgstr "Total de chamadas"
 
 #: templates/debug_toolbar/panels/cache.html:7
 msgid "Total time"
-msgstr "Tempo Totale"
+msgstr "Tempo total"
 
 #: templates/debug_toolbar/panels/cache.html:8
 msgid "Cache hits"
-msgstr "Trovati in cache"
+msgstr "Acessos ao cache"
 
 #: templates/debug_toolbar/panels/cache.html:9
 msgid "Cache misses"
-msgstr "Non trovati in cache"
+msgstr "Falhas de cache"
 
 #: templates/debug_toolbar/panels/cache.html:21
 msgid "Commands"
-msgstr "Comandi"
+msgstr "Comandos"
 
 #: templates/debug_toolbar/panels/cache.html:39
 msgid "Calls"
-msgstr "Chiamate"
+msgstr "Chamadas"
 
 #: templates/debug_toolbar/panels/cache.html:43
 #: templates/debug_toolbar/panels/sql.html:36
 msgid "Time (ms)"
-msgstr "Durata (ms)"
+msgstr "Tempo (ms)"
 
 #: templates/debug_toolbar/panels/cache.html:44
 msgid "Type"
 msgstr "Tipo"
 
 #: templates/debug_toolbar/panels/cache.html:45
 #: templates/debug_toolbar/panels/request.html:8
 msgid "Arguments"
-msgstr "Argomenti"
+msgstr "Argumentos"
 
 #: templates/debug_toolbar/panels/cache.html:46
 #: templates/debug_toolbar/panels/request.html:9
 msgid "Keyword arguments"
-msgstr "Parole chiave"
+msgstr "Argumentos"
 
 #: templates/debug_toolbar/panels/cache.html:47
 msgid "Backend"
 msgstr "Backend"
 
 #: templates/debug_toolbar/panels/headers.html:3
 msgid "Request headers"
-msgstr "Header della request"
+msgstr "Cabeçalhos de Requisição"
 
 #: templates/debug_toolbar/panels/headers.html:8
 #: templates/debug_toolbar/panels/headers.html:27
 #: templates/debug_toolbar/panels/headers.html:48
 msgid "Key"
-msgstr "Nome"
+msgstr "Chave"
 
 #: templates/debug_toolbar/panels/headers.html:9
 #: templates/debug_toolbar/panels/headers.html:28
 #: templates/debug_toolbar/panels/headers.html:49
 #: templates/debug_toolbar/panels/history_tr.html:23
-#: templates/debug_toolbar/panels/request_variables.html:11
+#: templates/debug_toolbar/panels/request_variables.html:12
 #: templates/debug_toolbar/panels/settings.html:6
 #: templates/debug_toolbar/panels/timer.html:11
 msgid "Value"
-msgstr "Valore"
+msgstr "Valor"
 
 #: templates/debug_toolbar/panels/headers.html:22
 msgid "Response headers"
-msgstr "Header della response"
+msgstr "Cabeçalhos de Resposta"
 
 #: templates/debug_toolbar/panels/headers.html:41
 msgid "WSGI environ"
 msgstr "Ambiente WSGI"
 
 #: templates/debug_toolbar/panels/headers.html:43
 msgid ""
 "Since the WSGI environ inherits the environment of the server, only a "
 "significant subset is shown below."
-msgstr "Visto che l'ambiente WSGI è ereditato dal server, sotto è mostrata solo la parte significativa."
+msgstr ""
+"Uma vez que o ambiente WSGI herda o ambiente do servidor, apenas um "
+"subconjunto significativo é mostrado abaixo."
 
 #: templates/debug_toolbar/panels/history.html:10
 msgid "Method"
 msgstr ""
 
 #: templates/debug_toolbar/panels/history.html:11
 #: templates/debug_toolbar/panels/staticfiles.html:43
 msgid "Path"
-msgstr "Percorso"
+msgstr "Caminho"
 
 #: templates/debug_toolbar/panels/history.html:12
+#, fuzzy
+#| msgid "Request headers"
 msgid "Request Variables"
-msgstr ""
+msgstr "Cabeçalhos de Requisição"
 
 #: templates/debug_toolbar/panels/history.html:13
 msgid "Status"
 msgstr ""
 
 #: templates/debug_toolbar/panels/history.html:14
 #: templates/debug_toolbar/panels/sql.html:37
 msgid "Action"
-msgstr "Azione"
+msgstr "Ação"
 
 #: templates/debug_toolbar/panels/history_tr.html:22
-#: templates/debug_toolbar/panels/request_variables.html:10
+#: templates/debug_toolbar/panels/request_variables.html:11
 msgid "Variable"
-msgstr "Variabile"
-
-#: templates/debug_toolbar/panels/logging.html:6
-msgid "Level"
-msgstr "Livello"
-
-#: templates/debug_toolbar/panels/logging.html:8
-msgid "Channel"
-msgstr "Canale"
-
-#: templates/debug_toolbar/panels/logging.html:9
-msgid "Message"
-msgstr "Messaggio"
-
-#: templates/debug_toolbar/panels/logging.html:10
-#: templates/debug_toolbar/panels/staticfiles.html:44
-msgid "Location"
-msgstr "Location"
-
-#: templates/debug_toolbar/panels/logging.html:26
-msgid "No messages logged"
-msgstr "Nessun messaggio registrato"
+msgstr "Variável"
 
 #: templates/debug_toolbar/panels/profiling.html:5
 msgid "Call"
-msgstr "Chiamata"
+msgstr "Chamar"
 
 #: templates/debug_toolbar/panels/profiling.html:6
 msgid "CumTime"
 msgstr "CumTime"
 
 #: templates/debug_toolbar/panels/profiling.html:7
 #: templates/debug_toolbar/panels/profiling.html:9
@@ -434,78 +405,78 @@
 
 #: templates/debug_toolbar/panels/profiling.html:8
 msgid "TotTime"
 msgstr "TotTime"
 
 #: templates/debug_toolbar/panels/profiling.html:10
 msgid "Count"
-msgstr "Numero"
+msgstr "Contagem"
 
 #: templates/debug_toolbar/panels/request.html:3
 msgid "View information"
-msgstr "Vedi Informazioni"
+msgstr "Ver informação"
 
 #: templates/debug_toolbar/panels/request.html:7
 msgid "View function"
-msgstr "Funzione View"
+msgstr "Função View"
 
 #: templates/debug_toolbar/panels/request.html:10
 msgid "URL name"
-msgstr "Nome URL"
+msgstr "Nome da URL"
 
 #: templates/debug_toolbar/panels/request.html:24
 msgid "Cookies"
 msgstr "Cookies"
 
 #: templates/debug_toolbar/panels/request.html:27
 msgid "No cookies"
-msgstr "Nessun cookie"
+msgstr "Sem Cookies"
 
 #: templates/debug_toolbar/panels/request.html:31
 msgid "Session data"
-msgstr "Dati di sessione"
+msgstr "Dados de Sessão"
 
 #: templates/debug_toolbar/panels/request.html:34
 msgid "No session data"
-msgstr "Nessun dato in sessione"
+msgstr "Sem dados de Sessão"
 
 #: templates/debug_toolbar/panels/request.html:38
 msgid "GET data"
-msgstr "Dati GET"
+msgstr "Dados de GET"
 
 #: templates/debug_toolbar/panels/request.html:41
 msgid "No GET data"
-msgstr "Nessun dato in GET"
+msgstr "Não há dados de GET"
 
 #: templates/debug_toolbar/panels/request.html:45
 msgid "POST data"
-msgstr "Dati POST"
+msgstr "Dados de POST"
 
 #: templates/debug_toolbar/panels/request.html:48
 msgid "No POST data"
-msgstr "Nessuno dato in POST"
+msgstr "Não há dados de POST"
 
 #: templates/debug_toolbar/panels/settings.html:5
 msgid "Setting"
-msgstr "Impostazione"
+msgstr "Configuração"
 
 #: templates/debug_toolbar/panels/signals.html:5
 msgid "Signal"
-msgstr "Segnale"
+msgstr "Sinais"
 
 #: templates/debug_toolbar/panels/signals.html:6
 msgid "Receivers"
-msgstr "Ricevitori"
+msgstr "Recebedores"
 
 #: templates/debug_toolbar/panels/sql.html:6
 #, python-format
 msgid "%(num)s query"
 msgid_plural "%(num)s queries"
-msgstr[0] "%(num)s query"
-msgstr[1] "%(num)s query"
+msgstr[0] "%(num)s consulta"
+msgstr[1] "%(num)s consultas"
 
 #: templates/debug_toolbar/panels/sql.html:8
 #, python-format
 msgid ""
 "including <abbr title=\"Similar queries are queries with the same SQL, but "
 "potentially different parameters.\">%(count)s similar</abbr>"
 msgstr ""
@@ -520,185 +491,196 @@
 #: templates/debug_toolbar/panels/sql.html:34
 msgid "Query"
 msgstr "Query"
 
 #: templates/debug_toolbar/panels/sql.html:35
 #: templates/debug_toolbar/panels/timer.html:36
 msgid "Timeline"
-msgstr "Timeline"
+msgstr "Linha do tempo"
 
 #: templates/debug_toolbar/panels/sql.html:52
-#, python-format
+#, fuzzy, python-format
+#| msgid "%(count)s message"
+#| msgid_plural "%(count)s messages"
 msgid "%(count)s similar queries."
-msgstr ""
+msgstr "%(count)s mensagem"
 
 #: templates/debug_toolbar/panels/sql.html:58
 #, python-format
 msgid "Duplicated %(dupes)s times."
 msgstr ""
 
 #: templates/debug_toolbar/panels/sql.html:95
 msgid "Connection:"
-msgstr "Connessione:"
+msgstr "Conexão:"
 
 #: templates/debug_toolbar/panels/sql.html:97
 msgid "Isolation level:"
-msgstr "Isolation level:"
+msgstr "Nível de isolamento:"
 
 #: templates/debug_toolbar/panels/sql.html:100
 msgid "Transaction status:"
-msgstr "Stato transazione:"
+msgstr "Status da transação:"
 
 #: templates/debug_toolbar/panels/sql.html:114
 msgid "(unknown)"
-msgstr "(sconosciuto)"
+msgstr "(unknown)"
 
 #: templates/debug_toolbar/panels/sql.html:123
 msgid "No SQL queries were recorded during this request."
-msgstr "Nessuna Query SQL è stata registrata durante questa richiesta"
+msgstr "Nenhuma consulta SQL foi registrada durante esta requisição."
 
 #: templates/debug_toolbar/panels/sql_explain.html:4
 msgid "SQL explained"
-msgstr "SQL spigato"
+msgstr "SQL explicada"
 
 #: templates/debug_toolbar/panels/sql_explain.html:9
 #: templates/debug_toolbar/panels/sql_profile.html:10
 #: templates/debug_toolbar/panels/sql_select.html:9
 msgid "Executed SQL"
-msgstr "SQL eseguita"
+msgstr "SQL Executada"
 
 #: templates/debug_toolbar/panels/sql_explain.html:13
 #: templates/debug_toolbar/panels/sql_profile.html:14
 #: templates/debug_toolbar/panels/sql_select.html:13
 msgid "Database"
-msgstr "Database"
+msgstr "Banco de dados"
 
 #: templates/debug_toolbar/panels/sql_profile.html:4
 msgid "SQL profiled"
-msgstr "SQL profilato"
+msgstr "SQL perfilado"
 
 #: templates/debug_toolbar/panels/sql_profile.html:37
 msgid "Error"
-msgstr "Errore"
+msgstr "Erro"
 
 #: templates/debug_toolbar/panels/sql_select.html:4
 msgid "SQL selected"
-msgstr "SQL selezionato"
+msgstr "SQL selecionada"
 
 #: templates/debug_toolbar/panels/sql_select.html:36
 msgid "Empty set"
-msgstr "Insieme vuoto"
+msgstr "Conjunto vazio"
 
 #: templates/debug_toolbar/panels/staticfiles.html:3
 msgid "Static file path"
 msgid_plural "Static file paths"
-msgstr[0] "Percorso file statici"
-msgstr[1] "Percorsi file statici"
+msgstr[0] "Caminho do arquivo estático"
+msgstr[1] "Caminho dos arquivos estáticos"
 
 #: templates/debug_toolbar/panels/staticfiles.html:7
 #, python-format
 msgid "(prefix %(prefix)s)"
-msgstr "(prefisso %(prefix)s)"
+msgstr "(prefixo %(prefix)s)"
 
 #: templates/debug_toolbar/panels/staticfiles.html:11
 #: templates/debug_toolbar/panels/staticfiles.html:22
 #: templates/debug_toolbar/panels/staticfiles.html:34
 #: templates/debug_toolbar/panels/templates.html:10
 #: templates/debug_toolbar/panels/templates.html:30
 #: templates/debug_toolbar/panels/templates.html:47
 msgid "None"
-msgstr "Nessuno"
+msgstr "Nenhum"
 
 #: templates/debug_toolbar/panels/staticfiles.html:14
 msgid "Static file app"
 msgid_plural "Static file apps"
-msgstr[0] "App file statici"
-msgstr[1] "App file statici"
+msgstr[0] "Arquivo estático de app"
+msgstr[1] "Arquivos estáticos de apps"
 
 #: templates/debug_toolbar/panels/staticfiles.html:25
 msgid "Static file"
 msgid_plural "Static files"
-msgstr[0] ""
-msgstr[1] "Files statici"
+msgstr[0] "Arquivo estático"
+msgstr[1] "Arquivos estáticos"
 
 #: templates/debug_toolbar/panels/staticfiles.html:39
 #, python-format
 msgid "%(payload_count)s file"
 msgid_plural "%(payload_count)s files"
-msgstr[0] "%(payload_count)s file"
-msgstr[1] "%(payload_count)s file"
+msgstr[0] "%(payload_count)s arquivo"
+msgstr[1] "%(payload_count)s arquivos"
+
+#: templates/debug_toolbar/panels/staticfiles.html:44
+msgid "Location"
+msgstr "Localização"
 
 #: templates/debug_toolbar/panels/template_source.html:4
 msgid "Template source:"
-msgstr "Sorgente del template"
+msgstr "Origem do Template:"
 
 #: templates/debug_toolbar/panels/templates.html:2
 msgid "Template path"
 msgid_plural "Template paths"
-msgstr[0] "Percorso dei template"
-msgstr[1] "Percorsi dei template"
+msgstr[0] "Caminho do Template"
+msgstr[1] "Caminho do Templates"
 
 #: templates/debug_toolbar/panels/templates.html:13
 msgid "Template"
 msgid_plural "Templates"
-msgstr[0] ""
-msgstr[1] "Template"
+msgstr[0] "Template"
+msgstr[1] "Templates"
 
 #: templates/debug_toolbar/panels/templates.html:22
 #: templates/debug_toolbar/panels/templates.html:40
 msgid "Toggle context"
-msgstr "Cambia contesto"
+msgstr "Alternar contexto"
 
 #: templates/debug_toolbar/panels/templates.html:33
 msgid "Context processor"
 msgid_plural "Context processors"
-msgstr[0] "Context processor"
-msgstr[1] "Context processors"
+msgstr[0] ""
+msgstr[1] "Processador do Contexto"
 
 #: templates/debug_toolbar/panels/timer.html:2
 msgid "Resource usage"
-msgstr "Uso risorsa"
+msgstr "Uso de recursos"
 
 #: templates/debug_toolbar/panels/timer.html:10
 msgid "Resource"
-msgstr "Risorsa"
+msgstr "Recurso"
 
 #: templates/debug_toolbar/panels/timer.html:26
 msgid "Browser timing"
-msgstr "Tempo browser"
+msgstr "Cronometragem do Navegador"
 
 #: templates/debug_toolbar/panels/timer.html:35
 msgid "Timing attribute"
-msgstr "Attributo"
+msgstr "Atributo de Cronometragem"
 
 #: templates/debug_toolbar/panels/timer.html:37
 msgid "Milliseconds since navigation start (+length)"
-msgstr "Millisecondi dall'inizio della navigazione (+lunghezza)"
+msgstr "Milissegundos desde início de navegação (+length)"
 
 #: templates/debug_toolbar/panels/versions.html:10
 msgid "Package"
 msgstr ""
 
 #: templates/debug_toolbar/panels/versions.html:11
 msgid "Name"
 msgstr "Nome"
 
 #: templates/debug_toolbar/panels/versions.html:12
 msgid "Version"
-msgstr "Versione"
+msgstr "Versão"
 
 #: templates/debug_toolbar/redirect.html:10
 msgid "Location:"
-msgstr "Location:"
+msgstr "Localização:"
 
 #: templates/debug_toolbar/redirect.html:12
 msgid ""
 "The Django Debug Toolbar has intercepted a redirect to the above URL for "
 "debug viewing purposes. You can click the above link to continue with the "
 "redirect as normal."
-msgstr "Django Debug Toolbar ha intercettato un redirect verso la URL indicata per visualizzare il debug, Puoi cliccare sul link sopra per continuare normalmente con la redirezione."
+msgstr ""
+"O Django Debug Toolbar interceptou um redirecionamento para a URL acima para "
+"fins de visualização de depuração. Você pode clicar no link acima para "
+"continuar com o redirecionamento normalmente."
 
-#: views.py:15
+#: views.py:16
 msgid ""
 "Data for this panel isn't available anymore. Please reload the page and "
 "retry."
-msgstr "Non sono più disponibili dati per questo pannello. Ricarica la pagina e riprova."
+msgstr ""
+"Os dados para este painel não está mais disponível. Por favor, recarregue a "
+"página e tente novamente."
```

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/locale/ja/LC_MESSAGES/django.mo` & `django_debug_toolbar-4.0.0/debug_toolbar/locale/ja/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/locale/ja/LC_MESSAGES/django.po` & `django_debug_toolbar-4.0.0/debug_toolbar/locale/ja/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,67 +4,54 @@
 #
 # Translators:
 # Shinya Okano <tokibito@gmail.com>, 2012,2014,2020
 msgid ""
 msgstr ""
 "Project-Id-Version: Django Debug Toolbar\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-08-14 10:25-0500\n"
+"POT-Creation-Date: 2023-01-20 17:23+0100\n"
 "PO-Revision-Date: 2021-08-14 15:25+0000\n"
 "Last-Translator: Tim Schilling\n"
-"Language-Team: Japanese (http://www.transifex.com/django-debug-toolbar/django-debug-toolbar/language/ja/)\n"
+"Language-Team: Japanese (http://www.transifex.com/django-debug-toolbar/"
+"django-debug-toolbar/language/ja/)\n"
+"Language: ja\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: ja\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 
 #: apps.py:15
 msgid "Debug Toolbar"
 msgstr "デバッグツールバー"
 
-#: panels/cache.py:227
+#: panels/cache.py:180
 msgid "Cache"
 msgstr "キャッシュ"
 
-#: panels/cache.py:234
+#: panels/cache.py:186
 #, python-format
 msgid "%(cache_calls)d call in %(time).2fms"
 msgid_plural "%(cache_calls)d calls in %(time).2fms"
 msgstr[0] ""
 
-#: panels/cache.py:246
+#: panels/cache.py:195
 #, python-format
 msgid "Cache calls from %(count)d backend"
 msgid_plural "Cache calls from %(count)d backends"
 msgstr[0] ""
 
-#: panels/headers.py:33
+#: panels/headers.py:31
 msgid "Headers"
 msgstr "ヘッダー"
 
-#: panels/history/panel.py:20 panels/history/panel.py:21
+#: panels/history/panel.py:18 panels/history/panel.py:19
 msgid "History"
 msgstr ""
 
-#: panels/logging.py:63
-msgid "Logging"
-msgstr "ロギング"
-
-#: panels/logging.py:69
-#, python-format
-msgid "%(count)s message"
-msgid_plural "%(count)s messages"
-msgstr[0] "%(count)s個のメッセージ"
-
-#: panels/logging.py:73
-msgid "Log messages"
-msgstr "ログメッセージ"
-
-#: panels/profiling.py:150
+#: panels/profiling.py:140
 msgid "Profiling"
 msgstr "プロファイル"
 
 #: panels/redirects.py:14
 msgid "Intercept redirects"
 msgstr "リダイレクトに割込み"
 
@@ -76,135 +63,134 @@
 msgid "<no view>"
 msgstr ""
 
 #: panels/request.py:53
 msgid "<unavailable>"
 msgstr "<利用不可>"
 
-#: panels/settings.py:24
+#: panels/settings.py:17
 msgid "Settings"
 msgstr "設定"
 
-#: panels/settings.py:27
+#: panels/settings.py:20
 #, python-format
 msgid "Settings from %s"
 msgstr ""
 
-#: panels/signals.py:58
+#: panels/signals.py:57
 #, python-format
 msgid "%(num_receivers)d receiver of 1 signal"
 msgid_plural "%(num_receivers)d receivers of 1 signal"
 msgstr[0] ""
 
-#: panels/signals.py:66
+#: panels/signals.py:62
 #, python-format
 msgid "%(num_receivers)d receiver of %(num_signals)d signals"
 msgid_plural "%(num_receivers)d receivers of %(num_signals)d signals"
 msgstr[0] ""
 
-#: panels/signals.py:73
+#: panels/signals.py:67
 msgid "Signals"
 msgstr "シグナル"
 
-#: panels/sql/panel.py:24
+#: panels/sql/panel.py:23
 msgid "Autocommit"
 msgstr ""
 
-#: panels/sql/panel.py:25
+#: panels/sql/panel.py:24
 msgid "Read uncommitted"
 msgstr ""
 
-#: panels/sql/panel.py:26
+#: panels/sql/panel.py:25
 msgid "Read committed"
 msgstr ""
 
-#: panels/sql/panel.py:27
+#: panels/sql/panel.py:26
 msgid "Repeatable read"
 msgstr ""
 
-#: panels/sql/panel.py:28
+#: panels/sql/panel.py:27
 msgid "Serializable"
 msgstr ""
 
-#: panels/sql/panel.py:40
+#: panels/sql/panel.py:39
 msgid "Idle"
 msgstr ""
 
-#: panels/sql/panel.py:41
+#: panels/sql/panel.py:40
 msgid "Active"
 msgstr ""
 
-#: panels/sql/panel.py:42
+#: panels/sql/panel.py:41
 msgid "In transaction"
 msgstr ""
 
-#: panels/sql/panel.py:43
+#: panels/sql/panel.py:42
 msgid "In error"
 msgstr ""
 
-#: panels/sql/panel.py:44
+#: panels/sql/panel.py:43
 msgid "Unknown"
 msgstr ""
 
-#: panels/sql/panel.py:109
+#: panels/sql/panel.py:130
 msgid "SQL"
 msgstr "SQL"
 
-#: panels/sql/panel.py:114
+#: panels/sql/panel.py:135
 #, python-format
 msgid "%(query_count)d query in %(sql_time).2fms"
 msgid_plural "%(query_count)d queries in %(sql_time).2fms"
 msgstr[0] ""
 
-#: panels/sql/panel.py:127
+#: panels/sql/panel.py:147
 #, python-format
 msgid "SQL queries from %(count)d connection"
 msgid_plural "SQL queries from %(count)d connections"
 msgstr[0] ""
 
-#: panels/staticfiles.py:85
+#: panels/staticfiles.py:84
 #, python-format
 msgid "Static files (%(num_found)s found, %(num_used)s used)"
 msgstr ""
 
-#: panels/staticfiles.py:106
+#: panels/staticfiles.py:105
 msgid "Static files"
 msgstr "静的ファイル"
 
-#: panels/staticfiles.py:112
+#: panels/staticfiles.py:111
 #, python-format
 msgid "%(num_used)s file used"
 msgid_plural "%(num_used)s files used"
 msgstr[0] ""
 
-#: panels/templates/panel.py:144
+#: panels/templates/panel.py:143
 msgid "Templates"
 msgstr "テンプレート"
 
-#: panels/templates/panel.py:149
+#: panels/templates/panel.py:148
 #, python-format
 msgid "Templates (%(num_templates)s rendered)"
 msgstr ""
 
-#: panels/templates/panel.py:181
+#: panels/templates/panel.py:180
 msgid "No origin"
 msgstr ""
 
 #: panels/timer.py:25
 #, python-format
 msgid "CPU: %(cum)0.2fms (%(total)0.2fms)"
 msgstr ""
 
 #: panels/timer.py:30
 #, python-format
 msgid "Total: %0.2fms"
 msgstr ""
 
 #: panels/timer.py:36 templates/debug_toolbar/panels/history.html:9
-#: templates/debug_toolbar/panels/logging.html:7
 #: templates/debug_toolbar/panels/sql_explain.html:11
 #: templates/debug_toolbar/panels/sql_profile.html:12
 #: templates/debug_toolbar/panels/sql_select.html:11
 msgid "Time"
 msgstr "時間"
 
 #: panels/timer.py:44
@@ -252,23 +238,23 @@
 msgid "%(vcsw)d voluntary, %(ivcsw)d involuntary"
 msgstr ""
 
 #: panels/versions.py:19
 msgid "Versions"
 msgstr "バージョン"
 
-#: templates/debug_toolbar/base.html:18
+#: templates/debug_toolbar/base.html:22
 msgid "Hide toolbar"
 msgstr "ツールバーを隠す"
 
-#: templates/debug_toolbar/base.html:18
+#: templates/debug_toolbar/base.html:22
 msgid "Hide"
 msgstr "隠す"
 
-#: templates/debug_toolbar/base.html:25
+#: templates/debug_toolbar/base.html:29
 msgid "Show toolbar"
 msgstr "ツールバーを表示"
 
 #: templates/debug_toolbar/includes/panel_button.html:4
 msgid "Disable for next and successive requests"
 msgstr ""
 
@@ -337,15 +323,15 @@
 msgid "Key"
 msgstr "キー"
 
 #: templates/debug_toolbar/panels/headers.html:9
 #: templates/debug_toolbar/panels/headers.html:28
 #: templates/debug_toolbar/panels/headers.html:49
 #: templates/debug_toolbar/panels/history_tr.html:23
-#: templates/debug_toolbar/panels/request_variables.html:11
+#: templates/debug_toolbar/panels/request_variables.html:12
 #: templates/debug_toolbar/panels/settings.html:6
 #: templates/debug_toolbar/panels/timer.html:11
 msgid "Value"
 msgstr "値"
 
 #: templates/debug_toolbar/panels/headers.html:22
 msgid "Response headers"
@@ -380,39 +366,18 @@
 
 #: templates/debug_toolbar/panels/history.html:14
 #: templates/debug_toolbar/panels/sql.html:37
 msgid "Action"
 msgstr ""
 
 #: templates/debug_toolbar/panels/history_tr.html:22
-#: templates/debug_toolbar/panels/request_variables.html:10
+#: templates/debug_toolbar/panels/request_variables.html:11
 msgid "Variable"
 msgstr "変数"
 
-#: templates/debug_toolbar/panels/logging.html:6
-msgid "Level"
-msgstr "レベル"
-
-#: templates/debug_toolbar/panels/logging.html:8
-msgid "Channel"
-msgstr ""
-
-#: templates/debug_toolbar/panels/logging.html:9
-msgid "Message"
-msgstr "メッセージ"
-
-#: templates/debug_toolbar/panels/logging.html:10
-#: templates/debug_toolbar/panels/staticfiles.html:44
-msgid "Location"
-msgstr ""
-
-#: templates/debug_toolbar/panels/logging.html:26
-msgid "No messages logged"
-msgstr "ロギングされたメッセージはありません"
-
 #: templates/debug_toolbar/panels/profiling.html:5
 msgid "Call"
 msgstr ""
 
 #: templates/debug_toolbar/panels/profiling.html:6
 msgid "CumTime"
 msgstr ""
@@ -608,14 +573,18 @@
 
 #: templates/debug_toolbar/panels/staticfiles.html:39
 #, python-format
 msgid "%(payload_count)s file"
 msgid_plural "%(payload_count)s files"
 msgstr[0] ""
 
+#: templates/debug_toolbar/panels/staticfiles.html:44
+msgid "Location"
+msgstr ""
+
 #: templates/debug_toolbar/panels/template_source.html:4
 msgid "Template source:"
 msgstr ""
 
 #: templates/debug_toolbar/panels/templates.html:2
 msgid "Template path"
 msgid_plural "Template paths"
@@ -675,12 +644,12 @@
 #: templates/debug_toolbar/redirect.html:12
 msgid ""
 "The Django Debug Toolbar has intercepted a redirect to the above URL for "
 "debug viewing purposes. You can click the above link to continue with the "
 "redirect as normal."
 msgstr ""
 
-#: views.py:15
+#: views.py:16
 msgid ""
 "Data for this panel isn't available anymore. Please reload the page and "
 "retry."
 msgstr ""
```

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/locale/nl/LC_MESSAGES/django.mo` & `django_debug_toolbar-4.0.0/debug_toolbar/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/locale/nl/LC_MESSAGES/django.po` & `django_debug_toolbar-4.0.0/debug_toolbar/locale/sv_SE/LC_MESSAGES/django.po`

 * *Files 18% similar despite different names*

```diff
@@ -1,294 +1,283 @@
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 #
 #
 # Translators:
-# Ingo Berben <ingoberben@gmail.com>, 2012-2013
+# Alex Nordlund <deep.alexander@gmail.com>, 2012-2013
+# Alex Nordlund <deep.alexander@gmail.com>, 2012
 msgid ""
 msgstr ""
 "Project-Id-Version: Django Debug Toolbar\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2014-04-25 21:52+0200\n"
+"POT-Creation-Date: 2023-01-20 17:23+0100\n"
 "PO-Revision-Date: 2014-04-25 19:53+0000\n"
 "Last-Translator: Aymeric Augustin <aymeric.augustin@m4x.org>\n"
-"Language-Team: Dutch (http://www.transifex.com/projects/p/django-debug-toolbar/language/nl/)\n"
+"Language-Team: Swedish (Sweden) (http://www.transifex.com/projects/p/django-"
+"debug-toolbar/language/sv_SE/)\n"
+"Language: sv_SE\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: nl\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: apps.py:11
+#: apps.py:15
 msgid "Debug Toolbar"
 msgstr ""
 
-#: views.py:14
-msgid ""
-"Data for this panel isn't available anymore. Please reload the page and "
-"retry."
-msgstr ""
-
-#: panels/cache.py:191
+#: panels/cache.py:180
 msgid "Cache"
 msgstr "Cache"
 
-#: panels/cache.py:196
+#: panels/cache.py:186
 #, python-format
 msgid "%(cache_calls)d call in %(time).2fms"
 msgid_plural "%(cache_calls)d calls in %(time).2fms"
 msgstr[0] ""
 msgstr[1] ""
 
-#: panels/cache.py:204
+#: panels/cache.py:195
 #, python-format
 msgid "Cache calls from %(count)d backend"
 msgid_plural "Cache calls from %(count)d backends"
 msgstr[0] ""
 msgstr[1] ""
 
-#: panels/headers.py:35
+#: panels/headers.py:31
 msgid "Headers"
 msgstr ""
 
-#: panels/logging.py:64
-msgid "Logging"
+#: panels/history/panel.py:18 panels/history/panel.py:19
+msgid "History"
 msgstr ""
 
-#: panels/logging.py:70
-#, python-format
-msgid "%(count)s message"
-msgid_plural "%(count)s messages"
-msgstr[0] "%(count)s bericht"
-msgstr[1] "%(count)s berichten"
-
-#: panels/logging.py:73
-msgid "Log messages"
-msgstr ""
-
-#: panels/profiling.py:127
+#: panels/profiling.py:140
 msgid "Profiling"
 msgstr "Profilering"
 
-#: panels/redirects.py:17
+#: panels/redirects.py:14
 msgid "Intercept redirects"
 msgstr ""
 
-#: panels/request.py:18
+#: panels/request.py:16
 msgid "Request"
 msgstr ""
 
-#: panels/request.py:35
+#: panels/request.py:36
 msgid "<no view>"
-msgstr "<niet bekeken>"
+msgstr ""
 
-#: panels/request.py:47
+#: panels/request.py:53
 msgid "<unavailable>"
-msgstr "<niet beschikbaar>"
+msgstr ""
 
-#: panels/settings.py:20
+#: panels/settings.py:17
 msgid "Settings"
-msgstr "Instellingen"
+msgstr "Inställningar"
 
-#: panels/settings.py:23
-#, python-format
-msgid "Settings from <code>%s</code>"
-msgstr "Instellingen van <code>%s</code>"
+#: panels/settings.py:20
+#, fuzzy, python-format
+#| msgid "Settings"
+msgid "Settings from %s"
+msgstr "Inställningar"
 
-#: panels/signals.py:45
+#: panels/signals.py:57
 #, python-format
 msgid "%(num_receivers)d receiver of 1 signal"
 msgid_plural "%(num_receivers)d receivers of 1 signal"
-msgstr[0] "%(num_receivers)d ontvanger van 1 signaal"
-msgstr[1] "%(num_receivers)d ontvangers van 1 signaal"
+msgstr[0] ""
+msgstr[1] ""
 
-#: panels/signals.py:48
+#: panels/signals.py:62
 #, python-format
 msgid "%(num_receivers)d receiver of %(num_signals)d signals"
 msgid_plural "%(num_receivers)d receivers of %(num_signals)d signals"
-msgstr[0] "%(num_receivers)d ontvanger van %(num_signals)d signalen"
-msgstr[1] "%(num_receivers)d ontvangers van %(num_signals)d signalen"
+msgstr[0] ""
+msgstr[1] ""
 
-#: panels/signals.py:53
+#: panels/signals.py:67
 msgid "Signals"
-msgstr "Signalen"
+msgstr "Signaler"
+
+#: panels/sql/panel.py:23
+msgid "Autocommit"
+msgstr ""
+
+#: panels/sql/panel.py:24
+msgid "Read uncommitted"
+msgstr ""
+
+#: panels/sql/panel.py:25
+msgid "Read committed"
+msgstr ""
+
+#: panels/sql/panel.py:26
+msgid "Repeatable read"
+msgstr ""
+
+#: panels/sql/panel.py:27
+msgid "Serializable"
+msgstr "Variabel"
+
+#: panels/sql/panel.py:39
+msgid "Idle"
+msgstr ""
+
+#: panels/sql/panel.py:40
+msgid "Active"
+msgstr "Åtgärd"
+
+#: panels/sql/panel.py:41
+msgid "In transaction"
+msgstr ""
+
+#: panels/sql/panel.py:42
+msgid "In error"
+msgstr "Felmeddelande"
+
+#: panels/sql/panel.py:43
+msgid "Unknown"
+msgstr "(okänd)"
+
+#: panels/sql/panel.py:130
+msgid "SQL"
+msgstr "SQL"
 
-#: panels/staticfiles.py:89
+#: panels/sql/panel.py:135
+#, python-format
+msgid "%(query_count)d query in %(sql_time).2fms"
+msgid_plural "%(query_count)d queries in %(sql_time).2fms"
+msgstr[0] ""
+msgstr[1] ""
+
+#: panels/sql/panel.py:147
+#, python-format
+msgid "SQL queries from %(count)d connection"
+msgid_plural "SQL queries from %(count)d connections"
+msgstr[0] ""
+msgstr[1] ""
+
+#: panels/staticfiles.py:84
 #, python-format
 msgid "Static files (%(num_found)s found, %(num_used)s used)"
 msgstr ""
 
-#: panels/staticfiles.py:107
+#: panels/staticfiles.py:105
 msgid "Static files"
-msgstr ""
+msgstr "Statiska filer"
 
-#: panels/staticfiles.py:112
+#: panels/staticfiles.py:111
 #, python-format
 msgid "%(num_used)s file used"
 msgid_plural "%(num_used)s files used"
 msgstr[0] ""
 msgstr[1] ""
 
-#: panels/timer.py:23
+#: panels/templates/panel.py:143
+msgid "Templates"
+msgstr "Mallar"
+
+#: panels/templates/panel.py:148
+#, python-format
+msgid "Templates (%(num_templates)s rendered)"
+msgstr ""
+
+#: panels/templates/panel.py:180
+msgid "No origin"
+msgstr ""
+
+#: panels/timer.py:25
 #, python-format
 msgid "CPU: %(cum)0.2fms (%(total)0.2fms)"
-msgstr "CPU: %(cum)0.2fms (%(total)0.2fms)"
+msgstr ""
 
-#: panels/timer.py:28
+#: panels/timer.py:30
 #, python-format
 msgid "Total: %0.2fms"
-msgstr "Totaal: %0.2fms"
+msgstr ""
 
-#: panels/timer.py:34 templates/debug_toolbar/panels/logging.html:7
+#: panels/timer.py:36 templates/debug_toolbar/panels/history.html:9
 #: templates/debug_toolbar/panels/sql_explain.html:11
 #: templates/debug_toolbar/panels/sql_profile.html:12
 #: templates/debug_toolbar/panels/sql_select.html:11
 msgid "Time"
-msgstr "Tijd"
+msgstr "Tid"
 
-#: panels/timer.py:42
+#: panels/timer.py:44
 msgid "User CPU time"
-msgstr "Gebruikers CPU tijd"
+msgstr ""
 
-#: panels/timer.py:42
+#: panels/timer.py:44
 #, python-format
 msgid "%(utime)0.3f msec"
-msgstr "%(utime)0.3f msec"
+msgstr ""
 
-#: panels/timer.py:43
+#: panels/timer.py:45
 msgid "System CPU time"
-msgstr "Systeem CPU tijd"
+msgstr ""
 
-#: panels/timer.py:43
+#: panels/timer.py:45
 #, python-format
 msgid "%(stime)0.3f msec"
-msgstr "%(stime)0.3f msec"
+msgstr ""
 
-#: panels/timer.py:44
+#: panels/timer.py:46
 msgid "Total CPU time"
-msgstr "Totaal CPU tijd"
+msgstr ""
 
-#: panels/timer.py:44
+#: panels/timer.py:46
 #, python-format
 msgid "%(total)0.3f msec"
-msgstr "%(total)0.3f msec"
+msgstr ""
 
-#: panels/timer.py:45
+#: panels/timer.py:47
 msgid "Elapsed time"
-msgstr "Verlopen tijd"
+msgstr ""
 
-#: panels/timer.py:45
+#: panels/timer.py:47
 #, python-format
 msgid "%(total_time)0.3f msec"
-msgstr "%(total_time)0.3f msec"
+msgstr ""
 
-#: panels/timer.py:46
+#: panels/timer.py:49
 msgid "Context switches"
 msgstr ""
 
-#: panels/timer.py:46
+#: panels/timer.py:50
 #, python-format
 msgid "%(vcsw)d voluntary, %(ivcsw)d involuntary"
-msgstr "%(vcsw)d vrijwillig, %(ivcsw)d niet vrijwillig"
-
-#: panels/versions.py:25
-msgid "Versions"
-msgstr "Versies"
-
-#: panels/sql/panel.py:22
-msgid "Autocommit"
 msgstr ""
 
-#: panels/sql/panel.py:23
-msgid "Read uncommitted"
-msgstr ""
-
-#: panels/sql/panel.py:24
-msgid "Read committed"
-msgstr ""
-
-#: panels/sql/panel.py:25
-msgid "Repeatable read"
-msgstr ""
-
-#: panels/sql/panel.py:26
-msgid "Serializable"
-msgstr "Serializeerbaar"
+#: panels/versions.py:19
+msgid "Versions"
+msgstr "Versioner"
 
-#: panels/sql/panel.py:37
-msgid "Idle"
+#: templates/debug_toolbar/base.html:22
+msgid "Hide toolbar"
 msgstr ""
 
-#: panels/sql/panel.py:38
-msgid "Active"
-msgstr "Actief"
+#: templates/debug_toolbar/base.html:22
+msgid "Hide"
+msgstr "Dölj"
 
-#: panels/sql/panel.py:39
-msgid "In transaction"
+#: templates/debug_toolbar/base.html:29
+msgid "Show toolbar"
 msgstr ""
 
-#: panels/sql/panel.py:40
-msgid "In error"
-msgstr "Foutief"
-
-#: panels/sql/panel.py:41
-msgid "Unknown"
-msgstr "Niet gekend"
-
-#: panels/sql/panel.py:105
-msgid "SQL"
-msgstr "SQL"
-
-#: panels/templates/panel.py:141
-msgid "Templates"
-msgstr "Templates"
-
-#: panels/templates/panel.py:146
-#, python-format
-msgid "Templates (%(num_templates)s rendered)"
-msgstr "Templates (%(num_templates)s gerenderd)"
-
-#: templates/debug_toolbar/base.html:19
-msgid "Hide toolbar"
-msgstr "Verberg toolbar"
-
-#: templates/debug_toolbar/base.html:19
-msgid "Hide"
-msgstr "Verbergen"
-
-#: templates/debug_toolbar/base.html:25
+#: templates/debug_toolbar/includes/panel_button.html:4
 msgid "Disable for next and successive requests"
 msgstr ""
 
-#: templates/debug_toolbar/base.html:25
+#: templates/debug_toolbar/includes/panel_button.html:4
 msgid "Enable for next and successive requests"
 msgstr ""
 
-#: templates/debug_toolbar/base.html:47
-msgid "Show toolbar"
-msgstr "Bekijk toolbar"
-
-#: templates/debug_toolbar/base.html:53
-msgid "Close"
-msgstr "Sluiten"
-
-#: templates/debug_toolbar/redirect.html:8
-msgid "Location:"
-msgstr ""
-
-#: templates/debug_toolbar/redirect.html:10
-msgid ""
-"The Django Debug Toolbar has intercepted a redirect to the above URL for "
-"debug viewing purposes. You can click the above link to continue with the "
-"redirect as normal."
-msgstr ""
-
 #: templates/debug_toolbar/panels/cache.html:2
 msgid "Summary"
-msgstr "Samenvatting"
+msgstr "Sammanfattning"
 
 #: templates/debug_toolbar/panels/cache.html:6
 msgid "Total calls"
 msgstr ""
 
 #: templates/debug_toolbar/panels/cache.html:7
 msgid "Total time"
@@ -307,21 +296,21 @@
 msgstr ""
 
 #: templates/debug_toolbar/panels/cache.html:39
 msgid "Calls"
 msgstr ""
 
 #: templates/debug_toolbar/panels/cache.html:43
-#: templates/debug_toolbar/panels/sql.html:20
+#: templates/debug_toolbar/panels/sql.html:36
 msgid "Time (ms)"
-msgstr "Tijd (ms)"
+msgstr "Tid (ms)"
 
 #: templates/debug_toolbar/panels/cache.html:44
 msgid "Type"
-msgstr "Type"
+msgstr ""
 
 #: templates/debug_toolbar/panels/cache.html:45
 #: templates/debug_toolbar/panels/request.html:8
 msgid "Arguments"
 msgstr ""
 
 #: templates/debug_toolbar/panels/cache.html:46
@@ -337,27 +326,25 @@
 msgid "Request headers"
 msgstr ""
 
 #: templates/debug_toolbar/panels/headers.html:8
 #: templates/debug_toolbar/panels/headers.html:27
 #: templates/debug_toolbar/panels/headers.html:48
 msgid "Key"
-msgstr "Sleutel"
+msgstr "Nyckel"
 
 #: templates/debug_toolbar/panels/headers.html:9
 #: templates/debug_toolbar/panels/headers.html:28
 #: templates/debug_toolbar/panels/headers.html:49
-#: templates/debug_toolbar/panels/request.html:33
-#: templates/debug_toolbar/panels/request.html:59
-#: templates/debug_toolbar/panels/request.html:85
-#: templates/debug_toolbar/panels/request.html:110
+#: templates/debug_toolbar/panels/history_tr.html:23
+#: templates/debug_toolbar/panels/request_variables.html:12
 #: templates/debug_toolbar/panels/settings.html:6
 #: templates/debug_toolbar/panels/timer.html:11
 msgid "Value"
-msgstr "Waarde"
+msgstr "Värde"
 
 #: templates/debug_toolbar/panels/headers.html:22
 msgid "Response headers"
 msgstr ""
 
 #: templates/debug_toolbar/panels/headers.html:41
 msgid "WSGI environ"
@@ -365,292 +352,325 @@
 
 #: templates/debug_toolbar/panels/headers.html:43
 msgid ""
 "Since the WSGI environ inherits the environment of the server, only a "
 "significant subset is shown below."
 msgstr ""
 
-#: templates/debug_toolbar/panels/logging.html:6
-msgid "Level"
-msgstr "Niveau"
-
-#: templates/debug_toolbar/panels/logging.html:8
-msgid "Channel"
-msgstr "Kanaal"
-
-#: templates/debug_toolbar/panels/logging.html:9
-msgid "Message"
-msgstr "Bericht"
+#: templates/debug_toolbar/panels/history.html:10
+msgid "Method"
+msgstr ""
 
-#: templates/debug_toolbar/panels/logging.html:10
-#: templates/debug_toolbar/panels/staticfiles.html:45
-msgid "Location"
-msgstr "Locatie"
+#: templates/debug_toolbar/panels/history.html:11
+#: templates/debug_toolbar/panels/staticfiles.html:43
+msgid "Path"
+msgstr "Sökväg"
+
+#: templates/debug_toolbar/panels/history.html:12
+#, fuzzy
+#| msgid "Variable"
+msgid "Request Variables"
+msgstr "Variabel"
 
-#: templates/debug_toolbar/panels/logging.html:26
-msgid "No messages logged"
-msgstr "Geen berichten gelogd"
+#: templates/debug_toolbar/panels/history.html:13
+msgid "Status"
+msgstr ""
+
+#: templates/debug_toolbar/panels/history.html:14
+#: templates/debug_toolbar/panels/sql.html:37
+msgid "Action"
+msgstr "Åtgärd"
+
+#: templates/debug_toolbar/panels/history_tr.html:22
+#: templates/debug_toolbar/panels/request_variables.html:11
+msgid "Variable"
+msgstr "Variabel"
 
 #: templates/debug_toolbar/panels/profiling.html:5
 msgid "Call"
-msgstr "Oproepen"
+msgstr ""
 
 #: templates/debug_toolbar/panels/profiling.html:6
 msgid "CumTime"
 msgstr ""
 
 #: templates/debug_toolbar/panels/profiling.html:7
 #: templates/debug_toolbar/panels/profiling.html:9
 msgid "Per"
 msgstr ""
 
 #: templates/debug_toolbar/panels/profiling.html:8
 msgid "TotTime"
-msgstr "TotTijd"
+msgstr ""
 
 #: templates/debug_toolbar/panels/profiling.html:10
 msgid "Count"
-msgstr "Aantal"
+msgstr "Räkna"
 
 #: templates/debug_toolbar/panels/request.html:3
 msgid "View information"
-msgstr "Bekijk informatie"
+msgstr "Visa informationen"
 
 #: templates/debug_toolbar/panels/request.html:7
 msgid "View function"
 msgstr ""
 
 #: templates/debug_toolbar/panels/request.html:10
 msgid "URL name"
 msgstr ""
 
 #: templates/debug_toolbar/panels/request.html:24
 msgid "Cookies"
 msgstr ""
 
-#: templates/debug_toolbar/panels/request.html:32
-#: templates/debug_toolbar/panels/request.html:58
-#: templates/debug_toolbar/panels/request.html:84
-#: templates/debug_toolbar/panels/request.html:109
-msgid "Variable"
-msgstr "Parameter"
-
-#: templates/debug_toolbar/panels/request.html:46
+#: templates/debug_toolbar/panels/request.html:27
 msgid "No cookies"
 msgstr ""
 
-#: templates/debug_toolbar/panels/request.html:50
+#: templates/debug_toolbar/panels/request.html:31
 msgid "Session data"
 msgstr ""
 
-#: templates/debug_toolbar/panels/request.html:72
+#: templates/debug_toolbar/panels/request.html:34
 msgid "No session data"
 msgstr ""
 
-#: templates/debug_toolbar/panels/request.html:76
+#: templates/debug_toolbar/panels/request.html:38
 msgid "GET data"
-msgstr "GET data"
+msgstr ""
 
-#: templates/debug_toolbar/panels/request.html:98
+#: templates/debug_toolbar/panels/request.html:41
 msgid "No GET data"
-msgstr "Geen GET data"
+msgstr "Ingen GET data"
 
-#: templates/debug_toolbar/panels/request.html:102
+#: templates/debug_toolbar/panels/request.html:45
 msgid "POST data"
-msgstr "POST data"
+msgstr ""
 
-#: templates/debug_toolbar/panels/request.html:123
+#: templates/debug_toolbar/panels/request.html:48
 msgid "No POST data"
-msgstr "Geen POST data"
+msgstr "Ingen POST data"
 
 #: templates/debug_toolbar/panels/settings.html:5
 msgid "Setting"
-msgstr "Instelling"
+msgstr "Inställning"
 
 #: templates/debug_toolbar/panels/signals.html:5
 msgid "Signal"
-msgstr "Signaal"
+msgstr "Signal"
 
 #: templates/debug_toolbar/panels/signals.html:6
-msgid "Providing"
-msgstr ""
-
-#: templates/debug_toolbar/panels/signals.html:7
 msgid "Receivers"
-msgstr "Ontvangers"
+msgstr "Mottagare"
 
-#: templates/debug_toolbar/panels/sql.html:7
+#: templates/debug_toolbar/panels/sql.html:6
 #, python-format
 msgid "%(num)s query"
 msgid_plural "%(num)s queries"
 msgstr[0] ""
 msgstr[1] ""
 
-#: templates/debug_toolbar/panels/sql.html:18
+#: templates/debug_toolbar/panels/sql.html:8
+#, python-format
+msgid ""
+"including <abbr title=\"Similar queries are queries with the same SQL, but "
+"potentially different parameters.\">%(count)s similar</abbr>"
+msgstr ""
+
+#: templates/debug_toolbar/panels/sql.html:12
+#, python-format
+msgid ""
+"and <abbr title=\"Duplicate queries are identical to each other: they "
+"execute exactly the same SQL and parameters.\">%(dupes)s duplicates</abbr>"
+msgstr ""
+
+#: templates/debug_toolbar/panels/sql.html:34
 msgid "Query"
-msgstr "Query"
+msgstr "Fråga"
 
-#: templates/debug_toolbar/panels/sql.html:19
+#: templates/debug_toolbar/panels/sql.html:35
 #: templates/debug_toolbar/panels/timer.html:36
 msgid "Timeline"
-msgstr "Tijdslijn"
+msgstr ""
 
-#: templates/debug_toolbar/panels/sql.html:21
-msgid "Action"
-msgstr "Actie"
+#: templates/debug_toolbar/panels/sql.html:52
+#, fuzzy, python-format
+#| msgid "%(count)s message"
+#| msgid_plural "%(count)s messages"
+msgid "%(count)s similar queries."
+msgstr "%(count)s meddelande"
+
+#: templates/debug_toolbar/panels/sql.html:58
+#, python-format
+msgid "Duplicated %(dupes)s times."
+msgstr ""
 
-#: templates/debug_toolbar/panels/sql.html:64
+#: templates/debug_toolbar/panels/sql.html:95
 msgid "Connection:"
-msgstr "Verbinding:"
+msgstr "Anslutning:"
 
-#: templates/debug_toolbar/panels/sql.html:66
+#: templates/debug_toolbar/panels/sql.html:97
 msgid "Isolation level:"
 msgstr ""
 
-#: templates/debug_toolbar/panels/sql.html:69
+#: templates/debug_toolbar/panels/sql.html:100
 msgid "Transaction status:"
-msgstr "Transactiestatus:"
+msgstr ""
 
-#: templates/debug_toolbar/panels/sql.html:83
+#: templates/debug_toolbar/panels/sql.html:114
 msgid "(unknown)"
-msgstr "(niet gekend)"
+msgstr "(okänd)"
 
-#: templates/debug_toolbar/panels/sql.html:92
+#: templates/debug_toolbar/panels/sql.html:123
 msgid "No SQL queries were recorded during this request."
 msgstr ""
 
-#: templates/debug_toolbar/panels/sql_explain.html:3
-#: templates/debug_toolbar/panels/sql_profile.html:3
-#: templates/debug_toolbar/panels/sql_select.html:3
-#: templates/debug_toolbar/panels/template_source.html:3
-msgid "Back"
-msgstr "Terug"
-
 #: templates/debug_toolbar/panels/sql_explain.html:4
 msgid "SQL explained"
-msgstr "SQL uitgelegd"
+msgstr ""
 
 #: templates/debug_toolbar/panels/sql_explain.html:9
 #: templates/debug_toolbar/panels/sql_profile.html:10
 #: templates/debug_toolbar/panels/sql_select.html:9
 msgid "Executed SQL"
-msgstr "Uitgevoerde SQL"
+msgstr "Utförd SQL"
 
 #: templates/debug_toolbar/panels/sql_explain.html:13
 #: templates/debug_toolbar/panels/sql_profile.html:14
 #: templates/debug_toolbar/panels/sql_select.html:13
 msgid "Database"
-msgstr "Database"
+msgstr "Databas"
 
 #: templates/debug_toolbar/panels/sql_profile.html:4
 msgid "SQL profiled"
 msgstr ""
 
 #: templates/debug_toolbar/panels/sql_profile.html:37
 msgid "Error"
-msgstr "Fout"
+msgstr "Felmeddelande"
 
 #: templates/debug_toolbar/panels/sql_select.html:4
 msgid "SQL selected"
 msgstr ""
 
 #: templates/debug_toolbar/panels/sql_select.html:36
 msgid "Empty set"
-msgstr "Lege set"
+msgstr "Tomt set"
 
-#: templates/debug_toolbar/panels/staticfiles.html:4
+#: templates/debug_toolbar/panels/staticfiles.html:3
 msgid "Static file path"
 msgid_plural "Static file paths"
 msgstr[0] ""
 msgstr[1] ""
 
-#: templates/debug_toolbar/panels/staticfiles.html:8
+#: templates/debug_toolbar/panels/staticfiles.html:7
 #, python-format
 msgid "(prefix %(prefix)s)"
 msgstr ""
 
-#: templates/debug_toolbar/panels/staticfiles.html:12
-#: templates/debug_toolbar/panels/staticfiles.html:23
-#: templates/debug_toolbar/panels/staticfiles.html:35
+#: templates/debug_toolbar/panels/staticfiles.html:11
+#: templates/debug_toolbar/panels/staticfiles.html:22
+#: templates/debug_toolbar/panels/staticfiles.html:34
 #: templates/debug_toolbar/panels/templates.html:10
-#: templates/debug_toolbar/panels/templates.html:28
-#: templates/debug_toolbar/panels/templates.html:43
+#: templates/debug_toolbar/panels/templates.html:30
+#: templates/debug_toolbar/panels/templates.html:47
 msgid "None"
-msgstr "None"
+msgstr "Inget"
 
-#: templates/debug_toolbar/panels/staticfiles.html:15
+#: templates/debug_toolbar/panels/staticfiles.html:14
 msgid "Static file app"
 msgid_plural "Static file apps"
 msgstr[0] ""
 msgstr[1] ""
 
-#: templates/debug_toolbar/panels/staticfiles.html:26
+#: templates/debug_toolbar/panels/staticfiles.html:25
 msgid "Static file"
 msgid_plural "Static files"
 msgstr[0] ""
-msgstr[1] ""
+msgstr[1] "Statiska filer"
 
-#: templates/debug_toolbar/panels/staticfiles.html:40
+#: templates/debug_toolbar/panels/staticfiles.html:39
 #, python-format
 msgid "%(payload_count)s file"
 msgid_plural "%(payload_count)s files"
 msgstr[0] ""
 msgstr[1] ""
 
 #: templates/debug_toolbar/panels/staticfiles.html:44
-msgid "Path"
-msgstr ""
+msgid "Location"
+msgstr "Plats"
 
 #: templates/debug_toolbar/panels/template_source.html:4
 msgid "Template source:"
 msgstr ""
 
 #: templates/debug_toolbar/panels/templates.html:2
 msgid "Template path"
 msgid_plural "Template paths"
-msgstr[0] "Templatepad"
-msgstr[1] "Templatepaden"
+msgstr[0] ""
+msgstr[1] ""
 
 #: templates/debug_toolbar/panels/templates.html:13
 msgid "Template"
 msgid_plural "Templates"
-msgstr[0] "Template"
-msgstr[1] "Templates"
+msgstr[0] "Mall"
+msgstr[1] "Mallar"
 
-#: templates/debug_toolbar/panels/templates.html:21
-#: templates/debug_toolbar/panels/templates.html:37
+#: templates/debug_toolbar/panels/templates.html:22
+#: templates/debug_toolbar/panels/templates.html:40
 msgid "Toggle context"
 msgstr ""
 
-#: templates/debug_toolbar/panels/templates.html:31
+#: templates/debug_toolbar/panels/templates.html:33
 msgid "Context processor"
 msgid_plural "Context processors"
 msgstr[0] ""
 msgstr[1] ""
 
 #: templates/debug_toolbar/panels/timer.html:2
 msgid "Resource usage"
 msgstr ""
 
 #: templates/debug_toolbar/panels/timer.html:10
 msgid "Resource"
-msgstr "Bron"
+msgstr "Resurs"
 
 #: templates/debug_toolbar/panels/timer.html:26
 msgid "Browser timing"
 msgstr ""
 
 #: templates/debug_toolbar/panels/timer.html:35
 msgid "Timing attribute"
 msgstr ""
 
 #: templates/debug_toolbar/panels/timer.html:37
 msgid "Milliseconds since navigation start (+length)"
 msgstr ""
 
-#: templates/debug_toolbar/panels/versions.html:5
+#: templates/debug_toolbar/panels/versions.html:10
+msgid "Package"
+msgstr ""
+
+#: templates/debug_toolbar/panels/versions.html:11
 msgid "Name"
-msgstr "Naam"
+msgstr "Namn"
 
-#: templates/debug_toolbar/panels/versions.html:6
+#: templates/debug_toolbar/panels/versions.html:12
 msgid "Version"
-msgstr "Versie"
+msgstr "Version"
+
+#: templates/debug_toolbar/redirect.html:10
+msgid "Location:"
+msgstr ""
+
+#: templates/debug_toolbar/redirect.html:12
+msgid ""
+"The Django Debug Toolbar has intercepted a redirect to the above URL for "
+"debug viewing purposes. You can click the above link to continue with the "
+"redirect as normal."
+msgstr ""
+
+#: views.py:16
+msgid ""
+"Data for this panel isn't available anymore. Please reload the page and "
+"retry."
+msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/locale/pl/LC_MESSAGES/django.mo` & `django_debug_toolbar-4.0.0/debug_toolbar/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/locale/pl/LC_MESSAGES/django.po` & `django_debug_toolbar-4.0.0/debug_toolbar/locale/fi/LC_MESSAGES/django.po`

 * *Files 4% similar despite different names*

```diff
@@ -1,300 +1,284 @@
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 #
 #
 # Translators:
-# Konrad Mosoń <mosonkonrad@gmail.com>, 2013
+# nanook <klaus.dahlen@gmail.com>, 2012
 msgid ""
 msgstr ""
 "Project-Id-Version: Django Debug Toolbar\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2014-04-25 21:52+0200\n"
+"POT-Creation-Date: 2023-01-20 17:23+0100\n"
 "PO-Revision-Date: 2014-04-25 19:53+0000\n"
 "Last-Translator: Aymeric Augustin <aymeric.augustin@m4x.org>\n"
-"Language-Team: Polish (http://www.transifex.com/projects/p/django-debug-toolbar/language/pl/)\n"
+"Language-Team: Finnish (http://www.transifex.com/projects/p/django-debug-"
+"toolbar/language/fi/)\n"
+"Language: fi\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: pl\n"
-"Plural-Forms: nplurals=3; plural=(n==1 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: apps.py:11
+#: apps.py:15
 msgid "Debug Toolbar"
 msgstr ""
 
-#: views.py:14
-msgid ""
-"Data for this panel isn't available anymore. Please reload the page and "
-"retry."
-msgstr ""
-
-#: panels/cache.py:191
+#: panels/cache.py:180
 msgid "Cache"
-msgstr "Cache"
+msgstr "Välimuisti"
 
-#: panels/cache.py:196
+#: panels/cache.py:186
 #, python-format
 msgid "%(cache_calls)d call in %(time).2fms"
 msgid_plural "%(cache_calls)d calls in %(time).2fms"
-msgstr[0] "%(cache_calls)d wywołanie w %(time).2fms"
-msgstr[1] "%(cache_calls)d wywołania w %(time).2fms"
-msgstr[2] "%(cache_calls)d wywołań w %(time).2fms"
+msgstr[0] "%(cache_calls)d kutsu %(time).2fms"
+msgstr[1] "%(cache_calls)d kutsua %(time).2fms"
 
-#: panels/cache.py:204
+#: panels/cache.py:195
 #, python-format
 msgid "Cache calls from %(count)d backend"
 msgid_plural "Cache calls from %(count)d backends"
-msgstr[0] "Wywołań z cache z %(count)d backendu"
-msgstr[1] "Wywołań z cache z %(count)d backendów"
-msgstr[2] "Wywołań z cache z %(count)d backendów"
+msgstr[0] ""
+msgstr[1] ""
 
-#: panels/headers.py:35
+#: panels/headers.py:31
 msgid "Headers"
 msgstr ""
 
-#: panels/logging.py:64
-msgid "Logging"
-msgstr "Logi"
-
-#: panels/logging.py:70
-#, python-format
-msgid "%(count)s message"
-msgid_plural "%(count)s messages"
-msgstr[0] "%(count)s wiadomość"
-msgstr[1] "%(count)s wiadomości"
-msgstr[2] "%(count)s wiadomości"
-
-#: panels/logging.py:73
-msgid "Log messages"
+#: panels/history/panel.py:18 panels/history/panel.py:19
+msgid "History"
 msgstr ""
 
-#: panels/profiling.py:127
+#: panels/profiling.py:140
 msgid "Profiling"
-msgstr "Profilowanie"
+msgstr "Profilointi"
 
-#: panels/redirects.py:17
+#: panels/redirects.py:14
 msgid "Intercept redirects"
 msgstr ""
 
-#: panels/request.py:18
+#: panels/request.py:16
 msgid "Request"
 msgstr ""
 
-#: panels/request.py:35
+#: panels/request.py:36
 msgid "<no view>"
-msgstr "<brak widoku>"
+msgstr ""
 
-#: panels/request.py:47
+#: panels/request.py:53
 msgid "<unavailable>"
-msgstr "<niedostępny>"
+msgstr ""
 
-#: panels/settings.py:20
+#: panels/settings.py:17
 msgid "Settings"
-msgstr "Ustawienia"
+msgstr "Asetukset"
 
-#: panels/settings.py:23
-#, python-format
-msgid "Settings from <code>%s</code>"
-msgstr "Ustawienia z <code>%s</code>"
+#: panels/settings.py:20
+#, fuzzy, python-format
+#| msgid "Settings from <code>%s</code>"
+msgid "Settings from %s"
+msgstr "Asetukset tiedostosta <code>%s</code>"
 
-#: panels/signals.py:45
+#: panels/signals.py:57
 #, python-format
 msgid "%(num_receivers)d receiver of 1 signal"
 msgid_plural "%(num_receivers)d receivers of 1 signal"
-msgstr[0] "%(num_receivers)d orbiorca 1 sygnału"
-msgstr[1] "%(num_receivers)d odbiorców 1 sygnału"
-msgstr[2] "%(num_receivers)d odbiorców 1 sygnału"
+msgstr[0] "%(num_receivers)d vastaanotin 1 signaalille"
+msgstr[1] "%(num_receivers)d vastaanotinta 1 signaalille"
 
-#: panels/signals.py:48
+#: panels/signals.py:62
 #, python-format
 msgid "%(num_receivers)d receiver of %(num_signals)d signals"
 msgid_plural "%(num_receivers)d receivers of %(num_signals)d signals"
-msgstr[0] "%(num_receivers)d odbiora %(num_signals)d sygnału"
-msgstr[1] "%(num_receivers)d odbiorców %(num_signals)d sygnałów"
-msgstr[2] "%(num_receivers)d odbiorców %(num_signals)d sygnałów"
+msgstr[0] "%(num_receivers)d vastaanotin %(num_signals)d signaalille"
+msgstr[1] "%(num_receivers)d vastaanotinta %(num_signals)d signaalille"
 
-#: panels/signals.py:53
+#: panels/signals.py:67
 msgid "Signals"
-msgstr "Sygnały"
+msgstr "Signaalit"
+
+#: panels/sql/panel.py:23
+msgid "Autocommit"
+msgstr "Autocommit"
+
+#: panels/sql/panel.py:24
+msgid "Read uncommitted"
+msgstr ""
+
+#: panels/sql/panel.py:25
+msgid "Read committed"
+msgstr ""
+
+#: panels/sql/panel.py:26
+msgid "Repeatable read"
+msgstr ""
+
+#: panels/sql/panel.py:27
+msgid "Serializable"
+msgstr "Muuttuja"
+
+#: panels/sql/panel.py:39
+msgid "Idle"
+msgstr ""
+
+#: panels/sql/panel.py:40
+msgid "Active"
+msgstr "Tapahtuma"
+
+#: panels/sql/panel.py:41
+msgid "In transaction"
+msgstr "Tapahtuman tila:"
+
+#: panels/sql/panel.py:42
+msgid "In error"
+msgstr "Virhe"
+
+#: panels/sql/panel.py:43
+msgid "Unknown"
+msgstr "(tuntematon)"
+
+#: panels/sql/panel.py:130
+msgid "SQL"
+msgstr "SQL"
+
+#: panels/sql/panel.py:135
+#, fuzzy, python-format
+#| msgid "%(cache_calls)d call in %(time).2fms"
+#| msgid_plural "%(cache_calls)d calls in %(time).2fms"
+msgid "%(query_count)d query in %(sql_time).2fms"
+msgid_plural "%(query_count)d queries in %(sql_time).2fms"
+msgstr[0] "%(cache_calls)d kutsu %(time).2fms"
+msgstr[1] "%(cache_calls)d kutsua %(time).2fms"
+
+#: panels/sql/panel.py:147
+#, python-format
+msgid "SQL queries from %(count)d connection"
+msgid_plural "SQL queries from %(count)d connections"
+msgstr[0] ""
+msgstr[1] ""
 
-#: panels/staticfiles.py:89
+#: panels/staticfiles.py:84
 #, python-format
 msgid "Static files (%(num_found)s found, %(num_used)s used)"
 msgstr ""
 
-#: panels/staticfiles.py:107
+#: panels/staticfiles.py:105
 msgid "Static files"
-msgstr ""
+msgstr "Staattiset tiedostot"
 
-#: panels/staticfiles.py:112
+#: panels/staticfiles.py:111
 #, python-format
 msgid "%(num_used)s file used"
 msgid_plural "%(num_used)s files used"
 msgstr[0] ""
 msgstr[1] ""
-msgstr[2] ""
 
-#: panels/timer.py:23
+#: panels/templates/panel.py:143
+msgid "Templates"
+msgstr "Asettelupohjat"
+
+#: panels/templates/panel.py:148
+#, python-format
+msgid "Templates (%(num_templates)s rendered)"
+msgstr "Asetttelupohjat (%(num_templates)s renderöity)"
+
+#: panels/templates/panel.py:180
+msgid "No origin"
+msgstr ""
+
+#: panels/timer.py:25
 #, python-format
 msgid "CPU: %(cum)0.2fms (%(total)0.2fms)"
 msgstr "CPU: %(cum)0.2fms (%(total)0.2fms)"
 
-#: panels/timer.py:28
+#: panels/timer.py:30
 #, python-format
 msgid "Total: %0.2fms"
 msgstr ""
 
-#: panels/timer.py:34 templates/debug_toolbar/panels/logging.html:7
+#: panels/timer.py:36 templates/debug_toolbar/panels/history.html:9
 #: templates/debug_toolbar/panels/sql_explain.html:11
 #: templates/debug_toolbar/panels/sql_profile.html:12
 #: templates/debug_toolbar/panels/sql_select.html:11
 msgid "Time"
-msgstr "Czas"
+msgstr "Aika"
 
-#: panels/timer.py:42
+#: panels/timer.py:44
 msgid "User CPU time"
-msgstr ""
+msgstr "Käyttäjän CPU-aika"
 
-#: panels/timer.py:42
+#: panels/timer.py:44
 #, python-format
 msgid "%(utime)0.3f msec"
-msgstr "%(utime)0.3f msec"
+msgstr "%(utime)0.3f msek"
 
-#: panels/timer.py:43
+#: panels/timer.py:45
 msgid "System CPU time"
-msgstr ""
+msgstr "Järjestelmän CPU-aika"
 
-#: panels/timer.py:43
+#: panels/timer.py:45
 #, python-format
 msgid "%(stime)0.3f msec"
-msgstr "%(stime)0.3f msec"
+msgstr "%(stime)0.3f msek"
 
-#: panels/timer.py:44
+#: panels/timer.py:46
 msgid "Total CPU time"
-msgstr ""
+msgstr "CPU-aika yhteensä"
 
-#: panels/timer.py:44
+#: panels/timer.py:46
 #, python-format
 msgid "%(total)0.3f msec"
-msgstr "%(total)0.3f msec"
+msgstr "%(total)0.3f msek"
 
-#: panels/timer.py:45
+#: panels/timer.py:47
 msgid "Elapsed time"
-msgstr ""
+msgstr "Kulunut aika"
 
-#: panels/timer.py:45
+#: panels/timer.py:47
 #, python-format
 msgid "%(total_time)0.3f msec"
-msgstr "%(total_time)0.3f msec"
+msgstr "%(total_time)0.3f msek"
 
-#: panels/timer.py:46
+#: panels/timer.py:49
 msgid "Context switches"
-msgstr ""
+msgstr "Kontekstin vivut"
 
-#: panels/timer.py:46
+#: panels/timer.py:50
 #, python-format
 msgid "%(vcsw)d voluntary, %(ivcsw)d involuntary"
 msgstr ""
 
-#: panels/versions.py:25
+#: panels/versions.py:19
 msgid "Versions"
-msgstr "Wersje"
-
-#: panels/sql/panel.py:22
-msgid "Autocommit"
-msgstr "Autocommit"
-
-#: panels/sql/panel.py:23
-msgid "Read uncommitted"
-msgstr ""
-
-#: panels/sql/panel.py:24
-msgid "Read committed"
-msgstr ""
-
-#: panels/sql/panel.py:25
-msgid "Repeatable read"
-msgstr ""
-
-#: panels/sql/panel.py:26
-msgid "Serializable"
-msgstr ""
-
-#: panels/sql/panel.py:37
-msgid "Idle"
-msgstr ""
-
-#: panels/sql/panel.py:38
-msgid "Active"
-msgstr "Aktywne"
-
-#: panels/sql/panel.py:39
-msgid "In transaction"
-msgstr "W transakcji"
-
-#: panels/sql/panel.py:40
-msgid "In error"
-msgstr "W błędzie"
-
-#: panels/sql/panel.py:41
-msgid "Unknown"
-msgstr "Nieznane"
-
-#: panels/sql/panel.py:105
-msgid "SQL"
-msgstr "SQL"
-
-#: panels/templates/panel.py:141
-msgid "Templates"
-msgstr "Templatki"
-
-#: panels/templates/panel.py:146
-#, python-format
-msgid "Templates (%(num_templates)s rendered)"
-msgstr "Templatki (%(num_templates)s wyrenderowano)"
+msgstr "Versiot"
 
-#: templates/debug_toolbar/base.html:19
+#: templates/debug_toolbar/base.html:22
 msgid "Hide toolbar"
 msgstr ""
 
-#: templates/debug_toolbar/base.html:19
+#: templates/debug_toolbar/base.html:22
 msgid "Hide"
-msgstr "Ukryj"
-
-#: templates/debug_toolbar/base.html:25
-msgid "Disable for next and successive requests"
-msgstr ""
-
-#: templates/debug_toolbar/base.html:25
-msgid "Enable for next and successive requests"
-msgstr ""
+msgstr "Piilota"
 
-#: templates/debug_toolbar/base.html:47
+#: templates/debug_toolbar/base.html:29
 msgid "Show toolbar"
 msgstr ""
 
-#: templates/debug_toolbar/base.html:53
-msgid "Close"
-msgstr "Zamknij"
-
-#: templates/debug_toolbar/redirect.html:8
-msgid "Location:"
+#: templates/debug_toolbar/includes/panel_button.html:4
+msgid "Disable for next and successive requests"
 msgstr ""
 
-#: templates/debug_toolbar/redirect.html:10
-msgid ""
-"The Django Debug Toolbar has intercepted a redirect to the above URL for "
-"debug viewing purposes. You can click the above link to continue with the "
-"redirect as normal."
+#: templates/debug_toolbar/includes/panel_button.html:4
+msgid "Enable for next and successive requests"
 msgstr ""
 
 #: templates/debug_toolbar/panels/cache.html:2
 msgid "Summary"
-msgstr "Podsumowanie"
+msgstr ""
 
 #: templates/debug_toolbar/panels/cache.html:6
 msgid "Total calls"
 msgstr ""
 
 #: templates/debug_toolbar/panels/cache.html:7
 msgid "Total time"
@@ -306,64 +290,62 @@
 
 #: templates/debug_toolbar/panels/cache.html:9
 msgid "Cache misses"
 msgstr ""
 
 #: templates/debug_toolbar/panels/cache.html:21
 msgid "Commands"
-msgstr "Polecenia"
+msgstr ""
 
 #: templates/debug_toolbar/panels/cache.html:39
 msgid "Calls"
-msgstr "Wywołania"
+msgstr ""
 
 #: templates/debug_toolbar/panels/cache.html:43
-#: templates/debug_toolbar/panels/sql.html:20
+#: templates/debug_toolbar/panels/sql.html:36
 msgid "Time (ms)"
-msgstr "Czas (ms)"
+msgstr "Aika (ms)"
 
 #: templates/debug_toolbar/panels/cache.html:44
 msgid "Type"
-msgstr "Typ"
+msgstr "Tyyppi"
 
 #: templates/debug_toolbar/panels/cache.html:45
 #: templates/debug_toolbar/panels/request.html:8
 msgid "Arguments"
 msgstr ""
 
 #: templates/debug_toolbar/panels/cache.html:46
 #: templates/debug_toolbar/panels/request.html:9
 msgid "Keyword arguments"
 msgstr ""
 
 #: templates/debug_toolbar/panels/cache.html:47
 msgid "Backend"
-msgstr "Backend"
+msgstr ""
 
 #: templates/debug_toolbar/panels/headers.html:3
 msgid "Request headers"
 msgstr ""
 
 #: templates/debug_toolbar/panels/headers.html:8
 #: templates/debug_toolbar/panels/headers.html:27
 #: templates/debug_toolbar/panels/headers.html:48
 msgid "Key"
-msgstr "Klucz"
+msgstr "Avain"
 
 #: templates/debug_toolbar/panels/headers.html:9
 #: templates/debug_toolbar/panels/headers.html:28
 #: templates/debug_toolbar/panels/headers.html:49
-#: templates/debug_toolbar/panels/request.html:33
-#: templates/debug_toolbar/panels/request.html:59
-#: templates/debug_toolbar/panels/request.html:85
-#: templates/debug_toolbar/panels/request.html:110
+#: templates/debug_toolbar/panels/history_tr.html:23
+#: templates/debug_toolbar/panels/request_variables.html:12
 #: templates/debug_toolbar/panels/settings.html:6
 #: templates/debug_toolbar/panels/timer.html:11
 msgid "Value"
-msgstr "Wartość"
+msgstr "Arvo"
 
 #: templates/debug_toolbar/panels/headers.html:22
 msgid "Response headers"
 msgstr ""
 
 #: templates/debug_toolbar/panels/headers.html:41
 msgid "WSGI environ"
@@ -371,300 +353,325 @@
 
 #: templates/debug_toolbar/panels/headers.html:43
 msgid ""
 "Since the WSGI environ inherits the environment of the server, only a "
 "significant subset is shown below."
 msgstr ""
 
-#: templates/debug_toolbar/panels/logging.html:6
-msgid "Level"
-msgstr "Poziom"
-
-#: templates/debug_toolbar/panels/logging.html:8
-msgid "Channel"
-msgstr "Kanał"
-
-#: templates/debug_toolbar/panels/logging.html:9
-msgid "Message"
-msgstr "Wiadomość"
+#: templates/debug_toolbar/panels/history.html:10
+msgid "Method"
+msgstr ""
+
+#: templates/debug_toolbar/panels/history.html:11
+#: templates/debug_toolbar/panels/staticfiles.html:43
+msgid "Path"
+msgstr "Polku"
 
-#: templates/debug_toolbar/panels/logging.html:10
-#: templates/debug_toolbar/panels/staticfiles.html:45
-msgid "Location"
-msgstr "Lokalizacja"
+#: templates/debug_toolbar/panels/history.html:12
+#, fuzzy
+#| msgid "Variable"
+msgid "Request Variables"
+msgstr "Muuttuja"
 
-#: templates/debug_toolbar/panels/logging.html:26
-msgid "No messages logged"
-msgstr "Nie zalogowano żadnych wiadomości"
+#: templates/debug_toolbar/panels/history.html:13
+msgid "Status"
+msgstr ""
+
+#: templates/debug_toolbar/panels/history.html:14
+#: templates/debug_toolbar/panels/sql.html:37
+msgid "Action"
+msgstr "Tapahtuma"
+
+#: templates/debug_toolbar/panels/history_tr.html:22
+#: templates/debug_toolbar/panels/request_variables.html:11
+msgid "Variable"
+msgstr "Muuttuja"
 
 #: templates/debug_toolbar/panels/profiling.html:5
 msgid "Call"
-msgstr "Wywołanie"
+msgstr "Kutsu"
 
 #: templates/debug_toolbar/panels/profiling.html:6
 msgid "CumTime"
-msgstr ""
+msgstr "CumTime"
 
 #: templates/debug_toolbar/panels/profiling.html:7
 #: templates/debug_toolbar/panels/profiling.html:9
 msgid "Per"
-msgstr ""
+msgstr "/"
 
 #: templates/debug_toolbar/panels/profiling.html:8
 msgid "TotTime"
-msgstr ""
+msgstr "TotTime"
 
 #: templates/debug_toolbar/panels/profiling.html:10
 msgid "Count"
-msgstr "Ilość"
+msgstr "Määrä"
 
 #: templates/debug_toolbar/panels/request.html:3
 msgid "View information"
-msgstr "Pokaż informacje"
+msgstr "Näkymän tiedot"
 
 #: templates/debug_toolbar/panels/request.html:7
 msgid "View function"
 msgstr ""
 
 #: templates/debug_toolbar/panels/request.html:10
 msgid "URL name"
 msgstr ""
 
 #: templates/debug_toolbar/panels/request.html:24
 msgid "Cookies"
 msgstr ""
 
-#: templates/debug_toolbar/panels/request.html:32
-#: templates/debug_toolbar/panels/request.html:58
-#: templates/debug_toolbar/panels/request.html:84
-#: templates/debug_toolbar/panels/request.html:109
-msgid "Variable"
-msgstr "Zmienna"
-
-#: templates/debug_toolbar/panels/request.html:46
+#: templates/debug_toolbar/panels/request.html:27
 msgid "No cookies"
 msgstr ""
 
-#: templates/debug_toolbar/panels/request.html:50
+#: templates/debug_toolbar/panels/request.html:31
 msgid "Session data"
 msgstr ""
 
-#: templates/debug_toolbar/panels/request.html:72
+#: templates/debug_toolbar/panels/request.html:34
 msgid "No session data"
 msgstr ""
 
-#: templates/debug_toolbar/panels/request.html:76
+#: templates/debug_toolbar/panels/request.html:38
 msgid "GET data"
 msgstr ""
 
-#: templates/debug_toolbar/panels/request.html:98
+#: templates/debug_toolbar/panels/request.html:41
 msgid "No GET data"
-msgstr "Brak danych GET"
+msgstr "Ei GET-dataa"
 
-#: templates/debug_toolbar/panels/request.html:102
+#: templates/debug_toolbar/panels/request.html:45
 msgid "POST data"
 msgstr ""
 
-#: templates/debug_toolbar/panels/request.html:123
+#: templates/debug_toolbar/panels/request.html:48
 msgid "No POST data"
-msgstr "Brak danych POST"
+msgstr "Ei POST-dataa"
 
 #: templates/debug_toolbar/panels/settings.html:5
 msgid "Setting"
-msgstr "Ustawienie"
+msgstr "Asetus"
 
 #: templates/debug_toolbar/panels/signals.html:5
 msgid "Signal"
-msgstr "Sygnał"
+msgstr "Signaali"
 
 #: templates/debug_toolbar/panels/signals.html:6
-msgid "Providing"
-msgstr ""
-
-#: templates/debug_toolbar/panels/signals.html:7
 msgid "Receivers"
-msgstr "Odbiorcy"
+msgstr "Vastaanottimet"
 
-#: templates/debug_toolbar/panels/sql.html:7
+#: templates/debug_toolbar/panels/sql.html:6
 #, python-format
 msgid "%(num)s query"
 msgid_plural "%(num)s queries"
-msgstr[0] "%(num)s zapytanie"
-msgstr[1] "%(num)s zapytania"
-msgstr[2] "%(num)s zapytań"
+msgstr[0] "%(num)s kysely"
+msgstr[1] "%(num)s kyselyä"
 
-#: templates/debug_toolbar/panels/sql.html:18
+#: templates/debug_toolbar/panels/sql.html:8
+#, python-format
+msgid ""
+"including <abbr title=\"Similar queries are queries with the same SQL, but "
+"potentially different parameters.\">%(count)s similar</abbr>"
+msgstr ""
+
+#: templates/debug_toolbar/panels/sql.html:12
+#, python-format
+msgid ""
+"and <abbr title=\"Duplicate queries are identical to each other: they "
+"execute exactly the same SQL and parameters.\">%(dupes)s duplicates</abbr>"
+msgstr ""
+
+#: templates/debug_toolbar/panels/sql.html:34
 msgid "Query"
-msgstr "Zapytanie"
+msgstr "Kysely"
 
-#: templates/debug_toolbar/panels/sql.html:19
+#: templates/debug_toolbar/panels/sql.html:35
 #: templates/debug_toolbar/panels/timer.html:36
 msgid "Timeline"
-msgstr "Oś czasu"
+msgstr "Aikajana"
 
-#: templates/debug_toolbar/panels/sql.html:21
-msgid "Action"
-msgstr "Akcja"
+#: templates/debug_toolbar/panels/sql.html:52
+#, fuzzy, python-format
+#| msgid "%(count)s message"
+#| msgid_plural "%(count)s messages"
+msgid "%(count)s similar queries."
+msgstr "%(count)s viesti"
+
+#: templates/debug_toolbar/panels/sql.html:58
+#, python-format
+msgid "Duplicated %(dupes)s times."
+msgstr ""
 
-#: templates/debug_toolbar/panels/sql.html:64
+#: templates/debug_toolbar/panels/sql.html:95
 msgid "Connection:"
-msgstr "Połączenie:"
+msgstr "Yhteys:"
 
-#: templates/debug_toolbar/panels/sql.html:66
+#: templates/debug_toolbar/panels/sql.html:97
 msgid "Isolation level:"
-msgstr "Poziom izolacji:"
+msgstr "Eristystaso:"
 
-#: templates/debug_toolbar/panels/sql.html:69
+#: templates/debug_toolbar/panels/sql.html:100
 msgid "Transaction status:"
-msgstr "Status transakcji:"
+msgstr "Tapahtuman status:"
 
-#: templates/debug_toolbar/panels/sql.html:83
+#: templates/debug_toolbar/panels/sql.html:114
 msgid "(unknown)"
-msgstr "(nieznany)"
+msgstr "(tuntematon)"
 
-#: templates/debug_toolbar/panels/sql.html:92
+#: templates/debug_toolbar/panels/sql.html:123
 msgid "No SQL queries were recorded during this request."
-msgstr "Żadne zapytania SQL nie zostały odnotowane podczas tego zapytania."
-
-#: templates/debug_toolbar/panels/sql_explain.html:3
-#: templates/debug_toolbar/panels/sql_profile.html:3
-#: templates/debug_toolbar/panels/sql_select.html:3
-#: templates/debug_toolbar/panels/template_source.html:3
-msgid "Back"
-msgstr "Wstecz"
+msgstr "Tämän pyynnön aikana ei tehty yhtään SQL-kyselyä."
 
 #: templates/debug_toolbar/panels/sql_explain.html:4
 msgid "SQL explained"
 msgstr ""
 
 #: templates/debug_toolbar/panels/sql_explain.html:9
 #: templates/debug_toolbar/panels/sql_profile.html:10
 #: templates/debug_toolbar/panels/sql_select.html:9
 msgid "Executed SQL"
-msgstr "Wykonane zapytanie SQL"
+msgstr "Suoritettu SQL"
 
 #: templates/debug_toolbar/panels/sql_explain.html:13
 #: templates/debug_toolbar/panels/sql_profile.html:14
 #: templates/debug_toolbar/panels/sql_select.html:13
 msgid "Database"
-msgstr "Baza danych"
+msgstr "Tietokanta"
 
 #: templates/debug_toolbar/panels/sql_profile.html:4
 msgid "SQL profiled"
 msgstr ""
 
 #: templates/debug_toolbar/panels/sql_profile.html:37
 msgid "Error"
-msgstr "Błąd"
+msgstr "Virhe"
 
 #: templates/debug_toolbar/panels/sql_select.html:4
 msgid "SQL selected"
 msgstr ""
 
 #: templates/debug_toolbar/panels/sql_select.html:36
 msgid "Empty set"
-msgstr "Pusty zbiór"
+msgstr "Tyhjä joukko"
 
-#: templates/debug_toolbar/panels/staticfiles.html:4
+#: templates/debug_toolbar/panels/staticfiles.html:3
 msgid "Static file path"
 msgid_plural "Static file paths"
 msgstr[0] ""
 msgstr[1] ""
-msgstr[2] ""
 
-#: templates/debug_toolbar/panels/staticfiles.html:8
+#: templates/debug_toolbar/panels/staticfiles.html:7
 #, python-format
 msgid "(prefix %(prefix)s)"
 msgstr ""
 
-#: templates/debug_toolbar/panels/staticfiles.html:12
-#: templates/debug_toolbar/panels/staticfiles.html:23
-#: templates/debug_toolbar/panels/staticfiles.html:35
+#: templates/debug_toolbar/panels/staticfiles.html:11
+#: templates/debug_toolbar/panels/staticfiles.html:22
+#: templates/debug_toolbar/panels/staticfiles.html:34
 #: templates/debug_toolbar/panels/templates.html:10
-#: templates/debug_toolbar/panels/templates.html:28
-#: templates/debug_toolbar/panels/templates.html:43
+#: templates/debug_toolbar/panels/templates.html:30
+#: templates/debug_toolbar/panels/templates.html:47
 msgid "None"
-msgstr "Brak"
+msgstr "None"
 
-#: templates/debug_toolbar/panels/staticfiles.html:15
+#: templates/debug_toolbar/panels/staticfiles.html:14
 msgid "Static file app"
 msgid_plural "Static file apps"
 msgstr[0] ""
 msgstr[1] ""
-msgstr[2] ""
 
-#: templates/debug_toolbar/panels/staticfiles.html:26
+#: templates/debug_toolbar/panels/staticfiles.html:25
 msgid "Static file"
 msgid_plural "Static files"
 msgstr[0] ""
-msgstr[1] ""
-msgstr[2] ""
+msgstr[1] "Staattiset tiedostot"
 
-#: templates/debug_toolbar/panels/staticfiles.html:40
+#: templates/debug_toolbar/panels/staticfiles.html:39
 #, python-format
 msgid "%(payload_count)s file"
 msgid_plural "%(payload_count)s files"
 msgstr[0] ""
 msgstr[1] ""
-msgstr[2] ""
 
 #: templates/debug_toolbar/panels/staticfiles.html:44
-msgid "Path"
-msgstr ""
+msgid "Location"
+msgstr "Sijainti"
 
 #: templates/debug_toolbar/panels/template_source.html:4
 msgid "Template source:"
 msgstr ""
 
 #: templates/debug_toolbar/panels/templates.html:2
 msgid "Template path"
 msgid_plural "Template paths"
-msgstr[0] "Ścieżka templatki"
-msgstr[1] "Ścieżki templatek"
-msgstr[2] "Ścieżki templatek"
+msgstr[0] "Sivupohjan polku"
+msgstr[1] "Sivupohjan polku"
 
 #: templates/debug_toolbar/panels/templates.html:13
 msgid "Template"
 msgid_plural "Templates"
-msgstr[0] "Templatki"
-msgstr[1] "Templatki"
-msgstr[2] "Templatki"
+msgstr[0] "Sivupohja"
+msgstr[1] "Sivupohja"
 
-#: templates/debug_toolbar/panels/templates.html:21
-#: templates/debug_toolbar/panels/templates.html:37
+#: templates/debug_toolbar/panels/templates.html:22
+#: templates/debug_toolbar/panels/templates.html:40
 msgid "Toggle context"
 msgstr ""
 
-#: templates/debug_toolbar/panels/templates.html:31
+#: templates/debug_toolbar/panels/templates.html:33
 msgid "Context processor"
 msgid_plural "Context processors"
-msgstr[0] ""
-msgstr[1] ""
-msgstr[2] ""
+msgstr[0] "Kontekstiprosessori"
+msgstr[1] "Kontekstiprosessori"
 
 #: templates/debug_toolbar/panels/timer.html:2
 msgid "Resource usage"
 msgstr ""
 
 #: templates/debug_toolbar/panels/timer.html:10
 msgid "Resource"
-msgstr "Zasób"
+msgstr "Resurssi"
 
 #: templates/debug_toolbar/panels/timer.html:26
 msgid "Browser timing"
 msgstr ""
 
 #: templates/debug_toolbar/panels/timer.html:35
 msgid "Timing attribute"
 msgstr ""
 
 #: templates/debug_toolbar/panels/timer.html:37
 msgid "Milliseconds since navigation start (+length)"
 msgstr ""
 
-#: templates/debug_toolbar/panels/versions.html:5
+#: templates/debug_toolbar/panels/versions.html:10
+msgid "Package"
+msgstr ""
+
+#: templates/debug_toolbar/panels/versions.html:11
 msgid "Name"
-msgstr "Nazwa"
+msgstr "Nimi"
 
-#: templates/debug_toolbar/panels/versions.html:6
+#: templates/debug_toolbar/panels/versions.html:12
 msgid "Version"
-msgstr "Wersja"
+msgstr "Versio"
+
+#: templates/debug_toolbar/redirect.html:10
+msgid "Location:"
+msgstr ""
+
+#: templates/debug_toolbar/redirect.html:12
+msgid ""
+"The Django Debug Toolbar has intercepted a redirect to the above URL for "
+"debug viewing purposes. You can click the above link to continue with the "
+"redirect as normal."
+msgstr ""
+
+#: views.py:16
+msgid ""
+"Data for this panel isn't available anymore. Please reload the page and "
+"retry."
+msgstr ""
```

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/locale/pt/LC_MESSAGES/django.mo` & `django_debug_toolbar-4.0.0/debug_toolbar/locale/pt/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/locale/pt/LC_MESSAGES/django.po` & `django_debug_toolbar-4.0.0/debug_toolbar/locale/nl/LC_MESSAGES/django.po`

 * *Files 18% similar despite different names*

```diff
@@ -1,294 +1,282 @@
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 #
 #
 # Translators:
-# joseduraes <jdmduraes@gmail.com>, 2014
+# Ingo Berben <ingoberben@gmail.com>, 2012-2013
 msgid ""
 msgstr ""
 "Project-Id-Version: Django Debug Toolbar\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2014-04-25 21:52+0200\n"
+"POT-Creation-Date: 2023-01-20 17:23+0100\n"
 "PO-Revision-Date: 2014-04-25 19:53+0000\n"
 "Last-Translator: Aymeric Augustin <aymeric.augustin@m4x.org>\n"
-"Language-Team: Portuguese (http://www.transifex.com/projects/p/django-debug-toolbar/language/pt/)\n"
+"Language-Team: Dutch (http://www.transifex.com/projects/p/django-debug-"
+"toolbar/language/nl/)\n"
+"Language: nl\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: pt\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: apps.py:11
+#: apps.py:15
 msgid "Debug Toolbar"
 msgstr ""
 
-#: views.py:14
-msgid ""
-"Data for this panel isn't available anymore. Please reload the page and "
-"retry."
-msgstr ""
-
-#: panels/cache.py:191
+#: panels/cache.py:180
 msgid "Cache"
-msgstr ""
+msgstr "Cache"
 
-#: panels/cache.py:196
+#: panels/cache.py:186
 #, python-format
 msgid "%(cache_calls)d call in %(time).2fms"
 msgid_plural "%(cache_calls)d calls in %(time).2fms"
 msgstr[0] ""
 msgstr[1] ""
 
-#: panels/cache.py:204
+#: panels/cache.py:195
 #, python-format
 msgid "Cache calls from %(count)d backend"
 msgid_plural "Cache calls from %(count)d backends"
 msgstr[0] ""
 msgstr[1] ""
 
-#: panels/headers.py:35
+#: panels/headers.py:31
 msgid "Headers"
 msgstr ""
 
-#: panels/logging.py:64
-msgid "Logging"
-msgstr "Registo"
-
-#: panels/logging.py:70
-#, python-format
-msgid "%(count)s message"
-msgid_plural "%(count)s messages"
-msgstr[0] ""
-msgstr[1] ""
-
-#: panels/logging.py:73
-msgid "Log messages"
+#: panels/history/panel.py:18 panels/history/panel.py:19
+msgid "History"
 msgstr ""
 
-#: panels/profiling.py:127
+#: panels/profiling.py:140
 msgid "Profiling"
-msgstr ""
+msgstr "Profilering"
 
-#: panels/redirects.py:17
+#: panels/redirects.py:14
 msgid "Intercept redirects"
-msgstr "Intercetar redirecionamentos"
+msgstr ""
 
-#: panels/request.py:18
+#: panels/request.py:16
 msgid "Request"
-msgstr "Pedido"
+msgstr ""
 
-#: panels/request.py:35
+#: panels/request.py:36
 msgid "<no view>"
-msgstr ""
+msgstr "<niet bekeken>"
 
-#: panels/request.py:47
+#: panels/request.py:53
 msgid "<unavailable>"
-msgstr "<indisponível>"
+msgstr "<niet beschikbaar>"
 
-#: panels/settings.py:20
+#: panels/settings.py:17
 msgid "Settings"
-msgstr "Configurações"
+msgstr "Instellingen"
 
-#: panels/settings.py:23
-#, python-format
-msgid "Settings from <code>%s</code>"
-msgstr ""
+#: panels/settings.py:20
+#, fuzzy, python-format
+#| msgid "Settings from <code>%s</code>"
+msgid "Settings from %s"
+msgstr "Instellingen van <code>%s</code>"
 
-#: panels/signals.py:45
+#: panels/signals.py:57
 #, python-format
 msgid "%(num_receivers)d receiver of 1 signal"
 msgid_plural "%(num_receivers)d receivers of 1 signal"
-msgstr[0] ""
-msgstr[1] ""
+msgstr[0] "%(num_receivers)d ontvanger van 1 signaal"
+msgstr[1] "%(num_receivers)d ontvangers van 1 signaal"
 
-#: panels/signals.py:48
+#: panels/signals.py:62
 #, python-format
 msgid "%(num_receivers)d receiver of %(num_signals)d signals"
 msgid_plural "%(num_receivers)d receivers of %(num_signals)d signals"
+msgstr[0] "%(num_receivers)d ontvanger van %(num_signals)d signalen"
+msgstr[1] "%(num_receivers)d ontvangers van %(num_signals)d signalen"
+
+#: panels/signals.py:67
+msgid "Signals"
+msgstr "Signalen"
+
+#: panels/sql/panel.py:23
+msgid "Autocommit"
+msgstr ""
+
+#: panels/sql/panel.py:24
+msgid "Read uncommitted"
+msgstr ""
+
+#: panels/sql/panel.py:25
+msgid "Read committed"
+msgstr ""
+
+#: panels/sql/panel.py:26
+msgid "Repeatable read"
+msgstr ""
+
+#: panels/sql/panel.py:27
+msgid "Serializable"
+msgstr "Serializeerbaar"
+
+#: panels/sql/panel.py:39
+msgid "Idle"
+msgstr ""
+
+#: panels/sql/panel.py:40
+msgid "Active"
+msgstr "Actief"
+
+#: panels/sql/panel.py:41
+msgid "In transaction"
+msgstr ""
+
+#: panels/sql/panel.py:42
+msgid "In error"
+msgstr "Foutief"
+
+#: panels/sql/panel.py:43
+msgid "Unknown"
+msgstr "Niet gekend"
+
+#: panels/sql/panel.py:130
+msgid "SQL"
+msgstr "SQL"
+
+#: panels/sql/panel.py:135
+#, python-format
+msgid "%(query_count)d query in %(sql_time).2fms"
+msgid_plural "%(query_count)d queries in %(sql_time).2fms"
 msgstr[0] ""
 msgstr[1] ""
 
-#: panels/signals.py:53
-msgid "Signals"
-msgstr "Sinais"
+#: panels/sql/panel.py:147
+#, python-format
+msgid "SQL queries from %(count)d connection"
+msgid_plural "SQL queries from %(count)d connections"
+msgstr[0] ""
+msgstr[1] ""
 
-#: panels/staticfiles.py:89
+#: panels/staticfiles.py:84
 #, python-format
 msgid "Static files (%(num_found)s found, %(num_used)s used)"
 msgstr ""
 
-#: panels/staticfiles.py:107
+#: panels/staticfiles.py:105
 msgid "Static files"
-msgstr "Ficheiros estáticos"
+msgstr ""
 
-#: panels/staticfiles.py:112
+#: panels/staticfiles.py:111
 #, python-format
 msgid "%(num_used)s file used"
 msgid_plural "%(num_used)s files used"
 msgstr[0] ""
 msgstr[1] ""
 
-#: panels/timer.py:23
+#: panels/templates/panel.py:143
+msgid "Templates"
+msgstr "Templates"
+
+#: panels/templates/panel.py:148
 #, python-format
-msgid "CPU: %(cum)0.2fms (%(total)0.2fms)"
+msgid "Templates (%(num_templates)s rendered)"
+msgstr "Templates (%(num_templates)s gerenderd)"
+
+#: panels/templates/panel.py:180
+msgid "No origin"
 msgstr ""
 
-#: panels/timer.py:28
+#: panels/timer.py:25
+#, python-format
+msgid "CPU: %(cum)0.2fms (%(total)0.2fms)"
+msgstr "CPU: %(cum)0.2fms (%(total)0.2fms)"
+
+#: panels/timer.py:30
 #, python-format
 msgid "Total: %0.2fms"
-msgstr "Total: %0.2fms"
+msgstr "Totaal: %0.2fms"
 
-#: panels/timer.py:34 templates/debug_toolbar/panels/logging.html:7
+#: panels/timer.py:36 templates/debug_toolbar/panels/history.html:9
 #: templates/debug_toolbar/panels/sql_explain.html:11
 #: templates/debug_toolbar/panels/sql_profile.html:12
 #: templates/debug_toolbar/panels/sql_select.html:11
 msgid "Time"
-msgstr "Tempo"
+msgstr "Tijd"
 
-#: panels/timer.py:42
+#: panels/timer.py:44
 msgid "User CPU time"
-msgstr ""
+msgstr "Gebruikers CPU tijd"
 
-#: panels/timer.py:42
+#: panels/timer.py:44
 #, python-format
 msgid "%(utime)0.3f msec"
-msgstr ""
+msgstr "%(utime)0.3f msec"
 
-#: panels/timer.py:43
+#: panels/timer.py:45
 msgid "System CPU time"
-msgstr ""
+msgstr "Systeem CPU tijd"
 
-#: panels/timer.py:43
+#: panels/timer.py:45
 #, python-format
 msgid "%(stime)0.3f msec"
-msgstr ""
+msgstr "%(stime)0.3f msec"
 
-#: panels/timer.py:44
+#: panels/timer.py:46
 msgid "Total CPU time"
-msgstr ""
+msgstr "Totaal CPU tijd"
 
-#: panels/timer.py:44
+#: panels/timer.py:46
 #, python-format
 msgid "%(total)0.3f msec"
-msgstr ""
+msgstr "%(total)0.3f msec"
 
-#: panels/timer.py:45
+#: panels/timer.py:47
 msgid "Elapsed time"
-msgstr ""
+msgstr "Verlopen tijd"
 
-#: panels/timer.py:45
+#: panels/timer.py:47
 #, python-format
 msgid "%(total_time)0.3f msec"
-msgstr ""
+msgstr "%(total_time)0.3f msec"
 
-#: panels/timer.py:46
+#: panels/timer.py:49
 msgid "Context switches"
 msgstr ""
 
-#: panels/timer.py:46
+#: panels/timer.py:50
 #, python-format
 msgid "%(vcsw)d voluntary, %(ivcsw)d involuntary"
-msgstr ""
+msgstr "%(vcsw)d vrijwillig, %(ivcsw)d niet vrijwillig"
 
-#: panels/versions.py:25
+#: panels/versions.py:19
 msgid "Versions"
-msgstr "Versões"
+msgstr "Versies"
 
-#: panels/sql/panel.py:22
-msgid "Autocommit"
-msgstr ""
-
-#: panels/sql/panel.py:23
-msgid "Read uncommitted"
-msgstr ""
-
-#: panels/sql/panel.py:24
-msgid "Read committed"
-msgstr ""
-
-#: panels/sql/panel.py:25
-msgid "Repeatable read"
-msgstr ""
-
-#: panels/sql/panel.py:26
-msgid "Serializable"
-msgstr "Variável"
-
-#: panels/sql/panel.py:37
-msgid "Idle"
-msgstr ""
-
-#: panels/sql/panel.py:38
-msgid "Active"
-msgstr "Acção"
-
-#: panels/sql/panel.py:39
-msgid "In transaction"
-msgstr ""
-
-#: panels/sql/panel.py:40
-msgid "In error"
-msgstr "Erro"
-
-#: panels/sql/panel.py:41
-msgid "Unknown"
-msgstr "Desconhecido"
-
-#: panels/sql/panel.py:105
-msgid "SQL"
-msgstr ""
-
-#: panels/templates/panel.py:141
-msgid "Templates"
-msgstr "Templates"
-
-#: panels/templates/panel.py:146
-#, python-format
-msgid "Templates (%(num_templates)s rendered)"
-msgstr "Templates (%(num_templates)s renderizados)"
-
-#: templates/debug_toolbar/base.html:19
+#: templates/debug_toolbar/base.html:22
 msgid "Hide toolbar"
-msgstr "Ocultar barra"
+msgstr "Verberg toolbar"
 
-#: templates/debug_toolbar/base.html:19
+#: templates/debug_toolbar/base.html:22
 msgid "Hide"
-msgstr "Ocultar"
-
-#: templates/debug_toolbar/base.html:25
-msgid "Disable for next and successive requests"
-msgstr "Desactivar para o seguinte e sucessivos pedidos"
+msgstr "Verbergen"
 
-#: templates/debug_toolbar/base.html:25
-msgid "Enable for next and successive requests"
-msgstr "Activar para o próximo e sucessivos pedidos"
-
-#: templates/debug_toolbar/base.html:47
+#: templates/debug_toolbar/base.html:29
 msgid "Show toolbar"
-msgstr "Mostrar barra"
-
-#: templates/debug_toolbar/base.html:53
-msgid "Close"
-msgstr "Fechar"
+msgstr "Bekijk toolbar"
 
-#: templates/debug_toolbar/redirect.html:8
-msgid "Location:"
-msgstr "Localização"
+#: templates/debug_toolbar/includes/panel_button.html:4
+msgid "Disable for next and successive requests"
+msgstr ""
 
-#: templates/debug_toolbar/redirect.html:10
-msgid ""
-"The Django Debug Toolbar has intercepted a redirect to the above URL for "
-"debug viewing purposes. You can click the above link to continue with the "
-"redirect as normal."
+#: templates/debug_toolbar/includes/panel_button.html:4
+msgid "Enable for next and successive requests"
 msgstr ""
 
 #: templates/debug_toolbar/panels/cache.html:2
 msgid "Summary"
-msgstr "Resumo"
+msgstr "Samenvatting"
 
 #: templates/debug_toolbar/panels/cache.html:6
 msgid "Total calls"
 msgstr ""
 
 #: templates/debug_toolbar/panels/cache.html:7
 msgid "Total time"
@@ -300,28 +288,28 @@
 
 #: templates/debug_toolbar/panels/cache.html:9
 msgid "Cache misses"
 msgstr ""
 
 #: templates/debug_toolbar/panels/cache.html:21
 msgid "Commands"
-msgstr "Comandos"
+msgstr ""
 
 #: templates/debug_toolbar/panels/cache.html:39
 msgid "Calls"
 msgstr ""
 
 #: templates/debug_toolbar/panels/cache.html:43
-#: templates/debug_toolbar/panels/sql.html:20
+#: templates/debug_toolbar/panels/sql.html:36
 msgid "Time (ms)"
-msgstr ""
+msgstr "Tijd (ms)"
 
 #: templates/debug_toolbar/panels/cache.html:44
 msgid "Type"
-msgstr "Tipo"
+msgstr "Type"
 
 #: templates/debug_toolbar/panels/cache.html:45
 #: templates/debug_toolbar/panels/request.html:8
 msgid "Arguments"
 msgstr ""
 
 #: templates/debug_toolbar/panels/cache.html:46
@@ -337,27 +325,25 @@
 msgid "Request headers"
 msgstr ""
 
 #: templates/debug_toolbar/panels/headers.html:8
 #: templates/debug_toolbar/panels/headers.html:27
 #: templates/debug_toolbar/panels/headers.html:48
 msgid "Key"
-msgstr "Chave"
+msgstr "Sleutel"
 
 #: templates/debug_toolbar/panels/headers.html:9
 #: templates/debug_toolbar/panels/headers.html:28
 #: templates/debug_toolbar/panels/headers.html:49
-#: templates/debug_toolbar/panels/request.html:33
-#: templates/debug_toolbar/panels/request.html:59
-#: templates/debug_toolbar/panels/request.html:85
-#: templates/debug_toolbar/panels/request.html:110
+#: templates/debug_toolbar/panels/history_tr.html:23
+#: templates/debug_toolbar/panels/request_variables.html:12
 #: templates/debug_toolbar/panels/settings.html:6
 #: templates/debug_toolbar/panels/timer.html:11
 msgid "Value"
-msgstr "Valor"
+msgstr "Waarde"
 
 #: templates/debug_toolbar/panels/headers.html:22
 msgid "Response headers"
 msgstr ""
 
 #: templates/debug_toolbar/panels/headers.html:41
 msgid "WSGI environ"
@@ -365,292 +351,325 @@
 
 #: templates/debug_toolbar/panels/headers.html:43
 msgid ""
 "Since the WSGI environ inherits the environment of the server, only a "
 "significant subset is shown below."
 msgstr ""
 
-#: templates/debug_toolbar/panels/logging.html:6
-msgid "Level"
-msgstr "Nível"
+#: templates/debug_toolbar/panels/history.html:10
+msgid "Method"
+msgstr ""
 
-#: templates/debug_toolbar/panels/logging.html:8
-msgid "Channel"
+#: templates/debug_toolbar/panels/history.html:11
+#: templates/debug_toolbar/panels/staticfiles.html:43
+msgid "Path"
 msgstr ""
 
-#: templates/debug_toolbar/panels/logging.html:9
-msgid "Message"
-msgstr "Mensagem"
+#: templates/debug_toolbar/panels/history.html:12
+#, fuzzy
+#| msgid "Variable"
+msgid "Request Variables"
+msgstr "Parameter"
 
-#: templates/debug_toolbar/panels/logging.html:10
-#: templates/debug_toolbar/panels/staticfiles.html:45
-msgid "Location"
-msgstr "Localização"
+#: templates/debug_toolbar/panels/history.html:13
+msgid "Status"
+msgstr ""
+
+#: templates/debug_toolbar/panels/history.html:14
+#: templates/debug_toolbar/panels/sql.html:37
+msgid "Action"
+msgstr "Actie"
 
-#: templates/debug_toolbar/panels/logging.html:26
-msgid "No messages logged"
-msgstr "Nenhuma mensagem registada"
+#: templates/debug_toolbar/panels/history_tr.html:22
+#: templates/debug_toolbar/panels/request_variables.html:11
+msgid "Variable"
+msgstr "Parameter"
 
 #: templates/debug_toolbar/panels/profiling.html:5
 msgid "Call"
-msgstr ""
+msgstr "Oproepen"
 
 #: templates/debug_toolbar/panels/profiling.html:6
 msgid "CumTime"
 msgstr ""
 
 #: templates/debug_toolbar/panels/profiling.html:7
 #: templates/debug_toolbar/panels/profiling.html:9
 msgid "Per"
 msgstr ""
 
 #: templates/debug_toolbar/panels/profiling.html:8
 msgid "TotTime"
-msgstr ""
+msgstr "TotTijd"
 
 #: templates/debug_toolbar/panels/profiling.html:10
 msgid "Count"
-msgstr ""
+msgstr "Aantal"
 
 #: templates/debug_toolbar/panels/request.html:3
 msgid "View information"
-msgstr ""
+msgstr "Bekijk informatie"
 
 #: templates/debug_toolbar/panels/request.html:7
 msgid "View function"
 msgstr ""
 
 #: templates/debug_toolbar/panels/request.html:10
 msgid "URL name"
 msgstr ""
 
 #: templates/debug_toolbar/panels/request.html:24
 msgid "Cookies"
 msgstr ""
 
-#: templates/debug_toolbar/panels/request.html:32
-#: templates/debug_toolbar/panels/request.html:58
-#: templates/debug_toolbar/panels/request.html:84
-#: templates/debug_toolbar/panels/request.html:109
-msgid "Variable"
-msgstr "Variável"
-
-#: templates/debug_toolbar/panels/request.html:46
+#: templates/debug_toolbar/panels/request.html:27
 msgid "No cookies"
 msgstr ""
 
-#: templates/debug_toolbar/panels/request.html:50
+#: templates/debug_toolbar/panels/request.html:31
 msgid "Session data"
 msgstr ""
 
-#: templates/debug_toolbar/panels/request.html:72
+#: templates/debug_toolbar/panels/request.html:34
 msgid "No session data"
 msgstr ""
 
-#: templates/debug_toolbar/panels/request.html:76
+#: templates/debug_toolbar/panels/request.html:38
 msgid "GET data"
-msgstr ""
+msgstr "GET data"
 
-#: templates/debug_toolbar/panels/request.html:98
+#: templates/debug_toolbar/panels/request.html:41
 msgid "No GET data"
-msgstr "Sem dados GET"
+msgstr "Geen GET data"
 
-#: templates/debug_toolbar/panels/request.html:102
+#: templates/debug_toolbar/panels/request.html:45
 msgid "POST data"
-msgstr "dados POST"
+msgstr "POST data"
 
-#: templates/debug_toolbar/panels/request.html:123
+#: templates/debug_toolbar/panels/request.html:48
 msgid "No POST data"
-msgstr "Sem variáveis POST"
+msgstr "Geen POST data"
 
 #: templates/debug_toolbar/panels/settings.html:5
 msgid "Setting"
-msgstr "Configurações"
+msgstr "Instelling"
 
 #: templates/debug_toolbar/panels/signals.html:5
 msgid "Signal"
-msgstr "Sinal"
+msgstr "Signaal"
 
 #: templates/debug_toolbar/panels/signals.html:6
-msgid "Providing"
-msgstr ""
-
-#: templates/debug_toolbar/panels/signals.html:7
 msgid "Receivers"
-msgstr "Receptores"
+msgstr "Ontvangers"
 
-#: templates/debug_toolbar/panels/sql.html:7
+#: templates/debug_toolbar/panels/sql.html:6
 #, python-format
 msgid "%(num)s query"
 msgid_plural "%(num)s queries"
 msgstr[0] ""
 msgstr[1] ""
 
-#: templates/debug_toolbar/panels/sql.html:18
-msgid "Query"
+#: templates/debug_toolbar/panels/sql.html:8
+#, python-format
+msgid ""
+"including <abbr title=\"Similar queries are queries with the same SQL, but "
+"potentially different parameters.\">%(count)s similar</abbr>"
+msgstr ""
+
+#: templates/debug_toolbar/panels/sql.html:12
+#, python-format
+msgid ""
+"and <abbr title=\"Duplicate queries are identical to each other: they "
+"execute exactly the same SQL and parameters.\">%(dupes)s duplicates</abbr>"
 msgstr ""
 
-#: templates/debug_toolbar/panels/sql.html:19
+#: templates/debug_toolbar/panels/sql.html:34
+msgid "Query"
+msgstr "Query"
+
+#: templates/debug_toolbar/panels/sql.html:35
 #: templates/debug_toolbar/panels/timer.html:36
 msgid "Timeline"
-msgstr ""
+msgstr "Tijdslijn"
 
-#: templates/debug_toolbar/panels/sql.html:21
-msgid "Action"
-msgstr "Acção"
+#: templates/debug_toolbar/panels/sql.html:52
+#, fuzzy, python-format
+#| msgid "%(count)s message"
+#| msgid_plural "%(count)s messages"
+msgid "%(count)s similar queries."
+msgstr "%(count)s bericht"
 
-#: templates/debug_toolbar/panels/sql.html:64
-msgid "Connection:"
+#: templates/debug_toolbar/panels/sql.html:58
+#, python-format
+msgid "Duplicated %(dupes)s times."
 msgstr ""
 
-#: templates/debug_toolbar/panels/sql.html:66
+#: templates/debug_toolbar/panels/sql.html:95
+msgid "Connection:"
+msgstr "Verbinding:"
+
+#: templates/debug_toolbar/panels/sql.html:97
 msgid "Isolation level:"
 msgstr ""
 
-#: templates/debug_toolbar/panels/sql.html:69
+#: templates/debug_toolbar/panels/sql.html:100
 msgid "Transaction status:"
-msgstr "Estado da transacção:"
+msgstr "Transactiestatus:"
 
-#: templates/debug_toolbar/panels/sql.html:83
+#: templates/debug_toolbar/panels/sql.html:114
 msgid "(unknown)"
-msgstr "(desconhecido)"
+msgstr "(niet gekend)"
 
-#: templates/debug_toolbar/panels/sql.html:92
+#: templates/debug_toolbar/panels/sql.html:123
 msgid "No SQL queries were recorded during this request."
-msgstr "Nenhuma query SQL foi registada durante este pedido."
-
-#: templates/debug_toolbar/panels/sql_explain.html:3
-#: templates/debug_toolbar/panels/sql_profile.html:3
-#: templates/debug_toolbar/panels/sql_select.html:3
-#: templates/debug_toolbar/panels/template_source.html:3
-msgid "Back"
-msgstr "Voltar"
+msgstr ""
 
 #: templates/debug_toolbar/panels/sql_explain.html:4
 msgid "SQL explained"
-msgstr ""
+msgstr "SQL uitgelegd"
 
 #: templates/debug_toolbar/panels/sql_explain.html:9
 #: templates/debug_toolbar/panels/sql_profile.html:10
 #: templates/debug_toolbar/panels/sql_select.html:9
 msgid "Executed SQL"
-msgstr "SQL Executado"
+msgstr "Uitgevoerde SQL"
 
 #: templates/debug_toolbar/panels/sql_explain.html:13
 #: templates/debug_toolbar/panels/sql_profile.html:14
 #: templates/debug_toolbar/panels/sql_select.html:13
 msgid "Database"
-msgstr ""
+msgstr "Database"
 
 #: templates/debug_toolbar/panels/sql_profile.html:4
 msgid "SQL profiled"
 msgstr ""
 
 #: templates/debug_toolbar/panels/sql_profile.html:37
 msgid "Error"
-msgstr "Erro"
+msgstr "Fout"
 
 #: templates/debug_toolbar/panels/sql_select.html:4
 msgid "SQL selected"
 msgstr ""
 
 #: templates/debug_toolbar/panels/sql_select.html:36
 msgid "Empty set"
-msgstr "Set vazio"
+msgstr "Lege set"
 
-#: templates/debug_toolbar/panels/staticfiles.html:4
+#: templates/debug_toolbar/panels/staticfiles.html:3
 msgid "Static file path"
 msgid_plural "Static file paths"
 msgstr[0] ""
 msgstr[1] ""
 
-#: templates/debug_toolbar/panels/staticfiles.html:8
+#: templates/debug_toolbar/panels/staticfiles.html:7
 #, python-format
 msgid "(prefix %(prefix)s)"
-msgstr "(prefixo %(prefix)s)"
+msgstr ""
 
-#: templates/debug_toolbar/panels/staticfiles.html:12
-#: templates/debug_toolbar/panels/staticfiles.html:23
-#: templates/debug_toolbar/panels/staticfiles.html:35
+#: templates/debug_toolbar/panels/staticfiles.html:11
+#: templates/debug_toolbar/panels/staticfiles.html:22
+#: templates/debug_toolbar/panels/staticfiles.html:34
 #: templates/debug_toolbar/panels/templates.html:10
-#: templates/debug_toolbar/panels/templates.html:28
-#: templates/debug_toolbar/panels/templates.html:43
+#: templates/debug_toolbar/panels/templates.html:30
+#: templates/debug_toolbar/panels/templates.html:47
 msgid "None"
-msgstr "Nenhum"
+msgstr "None"
 
-#: templates/debug_toolbar/panels/staticfiles.html:15
+#: templates/debug_toolbar/panels/staticfiles.html:14
 msgid "Static file app"
 msgid_plural "Static file apps"
 msgstr[0] ""
 msgstr[1] ""
 
-#: templates/debug_toolbar/panels/staticfiles.html:26
+#: templates/debug_toolbar/panels/staticfiles.html:25
 msgid "Static file"
 msgid_plural "Static files"
-msgstr[0] "Ficheiro estático"
-msgstr[1] "Ficheiros estáticos"
+msgstr[0] ""
+msgstr[1] ""
 
-#: templates/debug_toolbar/panels/staticfiles.html:40
+#: templates/debug_toolbar/panels/staticfiles.html:39
 #, python-format
 msgid "%(payload_count)s file"
 msgid_plural "%(payload_count)s files"
 msgstr[0] ""
 msgstr[1] ""
 
 #: templates/debug_toolbar/panels/staticfiles.html:44
-msgid "Path"
-msgstr ""
+msgid "Location"
+msgstr "Locatie"
 
 #: templates/debug_toolbar/panels/template_source.html:4
 msgid "Template source:"
 msgstr ""
 
 #: templates/debug_toolbar/panels/templates.html:2
 msgid "Template path"
 msgid_plural "Template paths"
-msgstr[0] ""
-msgstr[1] "Caminho da Template"
+msgstr[0] "Templatepad"
+msgstr[1] "Templatepaden"
 
 #: templates/debug_toolbar/panels/templates.html:13
 msgid "Template"
 msgid_plural "Templates"
-msgstr[0] ""
-msgstr[1] ""
+msgstr[0] "Template"
+msgstr[1] "Templates"
 
-#: templates/debug_toolbar/panels/templates.html:21
-#: templates/debug_toolbar/panels/templates.html:37
+#: templates/debug_toolbar/panels/templates.html:22
+#: templates/debug_toolbar/panels/templates.html:40
 msgid "Toggle context"
 msgstr ""
 
-#: templates/debug_toolbar/panels/templates.html:31
+#: templates/debug_toolbar/panels/templates.html:33
 msgid "Context processor"
 msgid_plural "Context processors"
 msgstr[0] ""
-msgstr[1] "Processador de Contexto"
+msgstr[1] ""
 
 #: templates/debug_toolbar/panels/timer.html:2
 msgid "Resource usage"
 msgstr ""
 
 #: templates/debug_toolbar/panels/timer.html:10
 msgid "Resource"
-msgstr "Recurso"
+msgstr "Bron"
 
 #: templates/debug_toolbar/panels/timer.html:26
 msgid "Browser timing"
 msgstr ""
 
 #: templates/debug_toolbar/panels/timer.html:35
 msgid "Timing attribute"
 msgstr ""
 
 #: templates/debug_toolbar/panels/timer.html:37
 msgid "Milliseconds since navigation start (+length)"
 msgstr ""
 
-#: templates/debug_toolbar/panels/versions.html:5
+#: templates/debug_toolbar/panels/versions.html:10
+msgid "Package"
+msgstr ""
+
+#: templates/debug_toolbar/panels/versions.html:11
 msgid "Name"
-msgstr "Nome"
+msgstr "Naam"
 
-#: templates/debug_toolbar/panels/versions.html:6
+#: templates/debug_toolbar/panels/versions.html:12
 msgid "Version"
-msgstr "Versão"
+msgstr "Versie"
+
+#: templates/debug_toolbar/redirect.html:10
+msgid "Location:"
+msgstr ""
+
+#: templates/debug_toolbar/redirect.html:12
+msgid ""
+"The Django Debug Toolbar has intercepted a redirect to the above URL for "
+"debug viewing purposes. You can click the above link to continue with the "
+"redirect as normal."
+msgstr ""
+
+#: views.py:16
+msgid ""
+"Data for this panel isn't available anymore. Please reload the page and "
+"retry."
+msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/locale/pt_BR/LC_MESSAGES/django.mo` & `django_debug_toolbar-4.0.0/debug_toolbar/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/locale/pt_BR/LC_MESSAGES/django.po` & `django_debug_toolbar-4.0.0/debug_toolbar/locale/pl/LC_MESSAGES/django.po`

 * *Files 8% similar despite different names*

```diff
@@ -1,657 +1,693 @@
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 #
 #
 # Translators:
-# Fábio <bnafta@gmail.com>, 2013-2014
-# Percy Pérez-Pinedo, 2009
+# Konrad Mosoń <mosonkonrad@gmail.com>, 2013
 msgid ""
 msgstr ""
 "Project-Id-Version: Django Debug Toolbar\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2014-04-25 21:52+0200\n"
+"POT-Creation-Date: 2023-01-20 17:23+0100\n"
 "PO-Revision-Date: 2014-04-25 19:53+0000\n"
 "Last-Translator: Aymeric Augustin <aymeric.augustin@m4x.org>\n"
-"Language-Team: Portuguese (Brazil) (http://www.transifex.com/projects/p/django-debug-toolbar/language/pt_BR/)\n"
+"Language-Team: Polish (http://www.transifex.com/projects/p/django-debug-"
+"toolbar/language/pl/)\n"
+"Language: pl\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: pt_BR\n"
-"Plural-Forms: nplurals=2; plural=(n > 1);\n"
+"Plural-Forms: nplurals=3; plural=(n==1 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 "
+"|| n%100>=20) ? 1 : 2);\n"
 
-#: apps.py:11
+#: apps.py:15
 msgid "Debug Toolbar"
 msgstr ""
 
-#: views.py:14
-msgid ""
-"Data for this panel isn't available anymore. Please reload the page and "
-"retry."
-msgstr "Os dados para este painel não está mais disponível. Por favor, recarregue a página e tente novamente."
-
-#: panels/cache.py:191
+#: panels/cache.py:180
 msgid "Cache"
 msgstr "Cache"
 
-#: panels/cache.py:196
+#: panels/cache.py:186
 #, python-format
 msgid "%(cache_calls)d call in %(time).2fms"
 msgid_plural "%(cache_calls)d calls in %(time).2fms"
-msgstr[0] "%(cache_calls)d chamada em %(time).2fms"
-msgstr[1] "%(cache_calls)d chamadas em %(time).2fms"
+msgstr[0] "%(cache_calls)d wywołanie w %(time).2fms"
+msgstr[1] "%(cache_calls)d wywołania w %(time).2fms"
+msgstr[2] "%(cache_calls)d wywołań w %(time).2fms"
 
-#: panels/cache.py:204
+#: panels/cache.py:195
 #, python-format
 msgid "Cache calls from %(count)d backend"
 msgid_plural "Cache calls from %(count)d backends"
-msgstr[0] "Chamadas ao cache de %(count)d backend"
-msgstr[1] "Chamadas ao cache de %(count)d backends"
+msgstr[0] "Wywołań z cache z %(count)d backendu"
+msgstr[1] "Wywołań z cache z %(count)d backendów"
+msgstr[2] "Wywołań z cache z %(count)d backendów"
 
-#: panels/headers.py:35
+#: panels/headers.py:31
 msgid "Headers"
-msgstr "Cabeçalhos"
-
-#: panels/logging.py:64
-msgid "Logging"
-msgstr "Logs"
-
-#: panels/logging.py:70
-#, python-format
-msgid "%(count)s message"
-msgid_plural "%(count)s messages"
-msgstr[0] "%(count)s mensagem"
-msgstr[1] "%(count)s mensagens"
+msgstr ""
 
-#: panels/logging.py:73
-msgid "Log messages"
-msgstr "Mensagens de log"
+#: panels/history/panel.py:18 panels/history/panel.py:19
+msgid "History"
+msgstr ""
 
-#: panels/profiling.py:127
+#: panels/profiling.py:140
 msgid "Profiling"
-msgstr "Profiling"
+msgstr "Profilowanie"
 
-#: panels/redirects.py:17
+#: panels/redirects.py:14
 msgid "Intercept redirects"
-msgstr "Interceptar redirecionamentos"
+msgstr ""
 
-#: panels/request.py:18
+#: panels/request.py:16
 msgid "Request"
-msgstr "Requisição"
+msgstr ""
 
-#: panels/request.py:35
+#: panels/request.py:36
 msgid "<no view>"
-msgstr "<nenhuma vista>"
+msgstr "<brak widoku>"
 
-#: panels/request.py:47
+#: panels/request.py:53
 msgid "<unavailable>"
-msgstr "<indisponível>"
+msgstr "<niedostępny>"
 
-#: panels/settings.py:20
+#: panels/settings.py:17
 msgid "Settings"
-msgstr "Configurações"
+msgstr "Ustawienia"
 
-#: panels/settings.py:23
-#, python-format
-msgid "Settings from <code>%s</code>"
-msgstr "Configurações em: <code>%s</code>"
+#: panels/settings.py:20
+#, fuzzy, python-format
+#| msgid "Settings from <code>%s</code>"
+msgid "Settings from %s"
+msgstr "Ustawienia z <code>%s</code>"
 
-#: panels/signals.py:45
+#: panels/signals.py:57
 #, python-format
 msgid "%(num_receivers)d receiver of 1 signal"
 msgid_plural "%(num_receivers)d receivers of 1 signal"
-msgstr[0] "%(num_receivers)d receptor de 1 sinal"
-msgstr[1] "%(num_receivers)d receptores de 1 sinal"
+msgstr[0] "%(num_receivers)d orbiorca 1 sygnału"
+msgstr[1] "%(num_receivers)d odbiorców 1 sygnału"
+msgstr[2] "%(num_receivers)d odbiorców 1 sygnału"
 
-#: panels/signals.py:48
+#: panels/signals.py:62
 #, python-format
 msgid "%(num_receivers)d receiver of %(num_signals)d signals"
 msgid_plural "%(num_receivers)d receivers of %(num_signals)d signals"
-msgstr[0] "%(num_receivers)d receptor de %(num_signals)d sinais"
-msgstr[1] "%(num_receivers)d receptores de %(num_signals)d sinais"
+msgstr[0] "%(num_receivers)d odbiora %(num_signals)d sygnału"
+msgstr[1] "%(num_receivers)d odbiorców %(num_signals)d sygnałów"
+msgstr[2] "%(num_receivers)d odbiorców %(num_signals)d sygnałów"
 
-#: panels/signals.py:53
+#: panels/signals.py:67
 msgid "Signals"
-msgstr "Sinais"
+msgstr "Sygnały"
+
+#: panels/sql/panel.py:23
+msgid "Autocommit"
+msgstr "Autocommit"
+
+#: panels/sql/panel.py:24
+msgid "Read uncommitted"
+msgstr ""
+
+#: panels/sql/panel.py:25
+msgid "Read committed"
+msgstr ""
+
+#: panels/sql/panel.py:26
+msgid "Repeatable read"
+msgstr ""
+
+#: panels/sql/panel.py:27
+msgid "Serializable"
+msgstr ""
+
+#: panels/sql/panel.py:39
+msgid "Idle"
+msgstr ""
+
+#: panels/sql/panel.py:40
+msgid "Active"
+msgstr "Aktywne"
+
+#: panels/sql/panel.py:41
+msgid "In transaction"
+msgstr "W transakcji"
+
+#: panels/sql/panel.py:42
+msgid "In error"
+msgstr "W błędzie"
+
+#: panels/sql/panel.py:43
+msgid "Unknown"
+msgstr "Nieznane"
+
+#: panels/sql/panel.py:130
+msgid "SQL"
+msgstr "SQL"
+
+#: panels/sql/panel.py:135
+#, fuzzy, python-format
+#| msgid "%(cache_calls)d call in %(time).2fms"
+#| msgid_plural "%(cache_calls)d calls in %(time).2fms"
+msgid "%(query_count)d query in %(sql_time).2fms"
+msgid_plural "%(query_count)d queries in %(sql_time).2fms"
+msgstr[0] "%(cache_calls)d wywołanie w %(time).2fms"
+msgstr[1] "%(cache_calls)d wywołania w %(time).2fms"
+msgstr[2] "%(cache_calls)d wywołań w %(time).2fms"
+
+#: panels/sql/panel.py:147
+#, python-format
+msgid "SQL queries from %(count)d connection"
+msgid_plural "SQL queries from %(count)d connections"
+msgstr[0] ""
+msgstr[1] ""
+msgstr[2] ""
 
-#: panels/staticfiles.py:89
+#: panels/staticfiles.py:84
 #, python-format
 msgid "Static files (%(num_found)s found, %(num_used)s used)"
-msgstr "Arquivos estáticos (%(num_found)s encontrados, %(num_used)s sendo utilizados)"
+msgstr ""
 
-#: panels/staticfiles.py:107
+#: panels/staticfiles.py:105
 msgid "Static files"
-msgstr "Arquivos estáticos"
+msgstr ""
 
-#: panels/staticfiles.py:112
+#: panels/staticfiles.py:111
 #, python-format
 msgid "%(num_used)s file used"
 msgid_plural "%(num_used)s files used"
-msgstr[0] "%(num_used)s arquivo utilizado"
-msgstr[1] "%(num_used)s arquivos utilizados"
+msgstr[0] ""
+msgstr[1] ""
+msgstr[2] ""
+
+#: panels/templates/panel.py:143
+msgid "Templates"
+msgstr "Templatki"
+
+#: panels/templates/panel.py:148
+#, python-format
+msgid "Templates (%(num_templates)s rendered)"
+msgstr "Templatki (%(num_templates)s wyrenderowano)"
+
+#: panels/templates/panel.py:180
+msgid "No origin"
+msgstr ""
 
-#: panels/timer.py:23
+#: panels/timer.py:25
 #, python-format
 msgid "CPU: %(cum)0.2fms (%(total)0.2fms)"
 msgstr "CPU: %(cum)0.2fms (%(total)0.2fms)"
 
-#: panels/timer.py:28
+#: panels/timer.py:30
 #, python-format
 msgid "Total: %0.2fms"
-msgstr "Total: %0.2fms"
+msgstr ""
 
-#: panels/timer.py:34 templates/debug_toolbar/panels/logging.html:7
+#: panels/timer.py:36 templates/debug_toolbar/panels/history.html:9
 #: templates/debug_toolbar/panels/sql_explain.html:11
 #: templates/debug_toolbar/panels/sql_profile.html:12
 #: templates/debug_toolbar/panels/sql_select.html:11
 msgid "Time"
-msgstr "Tempo"
+msgstr "Czas"
 
-#: panels/timer.py:42
+#: panels/timer.py:44
 msgid "User CPU time"
-msgstr "Tempo de CPU do usuário"
+msgstr ""
 
-#: panels/timer.py:42
+#: panels/timer.py:44
 #, python-format
 msgid "%(utime)0.3f msec"
-msgstr "%(utime)0.3f ms"
+msgstr "%(utime)0.3f msec"
 
-#: panels/timer.py:43
+#: panels/timer.py:45
 msgid "System CPU time"
-msgstr "Tempo de CPU do sistema"
+msgstr ""
 
-#: panels/timer.py:43
+#: panels/timer.py:45
 #, python-format
 msgid "%(stime)0.3f msec"
-msgstr "%(stime)0.3f ms"
+msgstr "%(stime)0.3f msec"
 
-#: panels/timer.py:44
+#: panels/timer.py:46
 msgid "Total CPU time"
-msgstr "Tempo total de CPU"
+msgstr ""
 
-#: panels/timer.py:44
+#: panels/timer.py:46
 #, python-format
 msgid "%(total)0.3f msec"
-msgstr "%(total)0.3f ms"
+msgstr "%(total)0.3f msec"
 
-#: panels/timer.py:45
+#: panels/timer.py:47
 msgid "Elapsed time"
-msgstr "Tempo decorrido"
+msgstr ""
 
-#: panels/timer.py:45
+#: panels/timer.py:47
 #, python-format
 msgid "%(total_time)0.3f msec"
-msgstr "%(total_time)0.3f ms"
+msgstr "%(total_time)0.3f msec"
 
-#: panels/timer.py:46
+#: panels/timer.py:49
 msgid "Context switches"
-msgstr "Mudanças de contexto"
+msgstr ""
 
-#: panels/timer.py:46
+#: panels/timer.py:50
 #, python-format
 msgid "%(vcsw)d voluntary, %(ivcsw)d involuntary"
-msgstr "%(vcsw)d voluntário, %(ivcsw)d involuntário"
+msgstr ""
 
-#: panels/versions.py:25
+#: panels/versions.py:19
 msgid "Versions"
-msgstr "Versões"
-
-#: panels/sql/panel.py:22
-msgid "Autocommit"
-msgstr "Autocommit"
-
-#: panels/sql/panel.py:23
-msgid "Read uncommitted"
-msgstr "Read uncommitted"
-
-#: panels/sql/panel.py:24
-msgid "Read committed"
-msgstr "Read committed"
-
-#: panels/sql/panel.py:25
-msgid "Repeatable read"
-msgstr "Leitura repetida"
-
-#: panels/sql/panel.py:26
-msgid "Serializable"
-msgstr "Variável"
-
-#: panels/sql/panel.py:37
-msgid "Idle"
-msgstr "Ocioso"
-
-#: panels/sql/panel.py:38
-msgid "Active"
-msgstr "Ação"
-
-#: panels/sql/panel.py:39
-msgid "In transaction"
-msgstr "Na transação"
-
-#: panels/sql/panel.py:40
-msgid "In error"
-msgstr "Erro"
+msgstr "Wersje"
 
-#: panels/sql/panel.py:41
-msgid "Unknown"
-msgstr "Desconhecido"
-
-#: panels/sql/panel.py:105
-msgid "SQL"
-msgstr "SQL"
-
-#: panels/templates/panel.py:141
-msgid "Templates"
-msgstr "Templates"
-
-#: panels/templates/panel.py:146
-#, python-format
-msgid "Templates (%(num_templates)s rendered)"
-msgstr "Templates (%(num_templates)s renderizados)"
-
-#: templates/debug_toolbar/base.html:19
+#: templates/debug_toolbar/base.html:22
 msgid "Hide toolbar"
-msgstr "Ocultar barra de ferramentas"
+msgstr ""
 
-#: templates/debug_toolbar/base.html:19
+#: templates/debug_toolbar/base.html:22
 msgid "Hide"
-msgstr "Esconder"
-
-#: templates/debug_toolbar/base.html:25
-msgid "Disable for next and successive requests"
-msgstr "Desativar para próximas requisições"
+msgstr "Ukryj"
 
-#: templates/debug_toolbar/base.html:25
-msgid "Enable for next and successive requests"
-msgstr "Habilitar para próximas requisições"
-
-#: templates/debug_toolbar/base.html:47
+#: templates/debug_toolbar/base.html:29
 msgid "Show toolbar"
-msgstr "Mostrar barra de ferramentas"
-
-#: templates/debug_toolbar/base.html:53
-msgid "Close"
-msgstr "Fechar"
+msgstr ""
 
-#: templates/debug_toolbar/redirect.html:8
-msgid "Location:"
-msgstr "Localização:"
+#: templates/debug_toolbar/includes/panel_button.html:4
+msgid "Disable for next and successive requests"
+msgstr ""
 
-#: templates/debug_toolbar/redirect.html:10
-msgid ""
-"The Django Debug Toolbar has intercepted a redirect to the above URL for "
-"debug viewing purposes. You can click the above link to continue with the "
-"redirect as normal."
-msgstr "O Django Debug Toolbar interceptou um redirecionamento para a URL acima para fins de visualização de depuração. Você pode clicar no link acima para continuar com o redirecionamento normalmente."
+#: templates/debug_toolbar/includes/panel_button.html:4
+msgid "Enable for next and successive requests"
+msgstr ""
 
 #: templates/debug_toolbar/panels/cache.html:2
 msgid "Summary"
-msgstr "Resumo"
+msgstr "Podsumowanie"
 
 #: templates/debug_toolbar/panels/cache.html:6
 msgid "Total calls"
-msgstr "Total de chamadas"
+msgstr ""
 
 #: templates/debug_toolbar/panels/cache.html:7
 msgid "Total time"
-msgstr "Tempo total"
+msgstr ""
 
 #: templates/debug_toolbar/panels/cache.html:8
 msgid "Cache hits"
-msgstr "Acessos ao cache"
+msgstr ""
 
 #: templates/debug_toolbar/panels/cache.html:9
 msgid "Cache misses"
-msgstr "Falhas de cache"
+msgstr ""
 
 #: templates/debug_toolbar/panels/cache.html:21
 msgid "Commands"
-msgstr "Comandos"
+msgstr "Polecenia"
 
 #: templates/debug_toolbar/panels/cache.html:39
 msgid "Calls"
-msgstr "Chamadas"
+msgstr "Wywołania"
 
 #: templates/debug_toolbar/panels/cache.html:43
-#: templates/debug_toolbar/panels/sql.html:20
+#: templates/debug_toolbar/panels/sql.html:36
 msgid "Time (ms)"
-msgstr "Tempo (ms)"
+msgstr "Czas (ms)"
 
 #: templates/debug_toolbar/panels/cache.html:44
 msgid "Type"
-msgstr "Tipo"
+msgstr "Typ"
 
 #: templates/debug_toolbar/panels/cache.html:45
 #: templates/debug_toolbar/panels/request.html:8
 msgid "Arguments"
-msgstr "Argumentos"
+msgstr ""
 
 #: templates/debug_toolbar/panels/cache.html:46
 #: templates/debug_toolbar/panels/request.html:9
 msgid "Keyword arguments"
-msgstr "Argumentos"
+msgstr ""
 
 #: templates/debug_toolbar/panels/cache.html:47
 msgid "Backend"
 msgstr "Backend"
 
 #: templates/debug_toolbar/panels/headers.html:3
 msgid "Request headers"
-msgstr "Cabeçalhos de Requisição"
+msgstr ""
 
 #: templates/debug_toolbar/panels/headers.html:8
 #: templates/debug_toolbar/panels/headers.html:27
 #: templates/debug_toolbar/panels/headers.html:48
 msgid "Key"
-msgstr "Chave"
+msgstr "Klucz"
 
 #: templates/debug_toolbar/panels/headers.html:9
 #: templates/debug_toolbar/panels/headers.html:28
 #: templates/debug_toolbar/panels/headers.html:49
-#: templates/debug_toolbar/panels/request.html:33
-#: templates/debug_toolbar/panels/request.html:59
-#: templates/debug_toolbar/panels/request.html:85
-#: templates/debug_toolbar/panels/request.html:110
+#: templates/debug_toolbar/panels/history_tr.html:23
+#: templates/debug_toolbar/panels/request_variables.html:12
 #: templates/debug_toolbar/panels/settings.html:6
 #: templates/debug_toolbar/panels/timer.html:11
 msgid "Value"
-msgstr "Valor"
+msgstr "Wartość"
 
 #: templates/debug_toolbar/panels/headers.html:22
 msgid "Response headers"
-msgstr "Cabeçalhos de Resposta"
+msgstr ""
 
 #: templates/debug_toolbar/panels/headers.html:41
 msgid "WSGI environ"
-msgstr "Ambiente WSGI"
+msgstr ""
 
 #: templates/debug_toolbar/panels/headers.html:43
 msgid ""
 "Since the WSGI environ inherits the environment of the server, only a "
 "significant subset is shown below."
-msgstr "Uma vez que o ambiente WSGI herda o ambiente do servidor, apenas um subconjunto significativo é mostrado abaixo."
+msgstr ""
 
-#: templates/debug_toolbar/panels/logging.html:6
-msgid "Level"
-msgstr "Nível"
-
-#: templates/debug_toolbar/panels/logging.html:8
-msgid "Channel"
-msgstr "Canal"
-
-#: templates/debug_toolbar/panels/logging.html:9
-msgid "Message"
-msgstr "Mensagem"
+#: templates/debug_toolbar/panels/history.html:10
+msgid "Method"
+msgstr ""
 
-#: templates/debug_toolbar/panels/logging.html:10
-#: templates/debug_toolbar/panels/staticfiles.html:45
-msgid "Location"
-msgstr "Localização"
+#: templates/debug_toolbar/panels/history.html:11
+#: templates/debug_toolbar/panels/staticfiles.html:43
+msgid "Path"
+msgstr ""
+
+#: templates/debug_toolbar/panels/history.html:12
+#, fuzzy
+#| msgid "Variable"
+msgid "Request Variables"
+msgstr "Zmienna"
+
+#: templates/debug_toolbar/panels/history.html:13
+msgid "Status"
+msgstr ""
 
-#: templates/debug_toolbar/panels/logging.html:26
-msgid "No messages logged"
-msgstr "Nenhuma mensagem logada"
+#: templates/debug_toolbar/panels/history.html:14
+#: templates/debug_toolbar/panels/sql.html:37
+msgid "Action"
+msgstr "Akcja"
+
+#: templates/debug_toolbar/panels/history_tr.html:22
+#: templates/debug_toolbar/panels/request_variables.html:11
+msgid "Variable"
+msgstr "Zmienna"
 
 #: templates/debug_toolbar/panels/profiling.html:5
 msgid "Call"
-msgstr "Chamar"
+msgstr "Wywołanie"
 
 #: templates/debug_toolbar/panels/profiling.html:6
 msgid "CumTime"
-msgstr "CumTime"
+msgstr ""
 
 #: templates/debug_toolbar/panels/profiling.html:7
 #: templates/debug_toolbar/panels/profiling.html:9
 msgid "Per"
-msgstr "Per"
+msgstr ""
 
 #: templates/debug_toolbar/panels/profiling.html:8
 msgid "TotTime"
-msgstr "TotTime"
+msgstr ""
 
 #: templates/debug_toolbar/panels/profiling.html:10
 msgid "Count"
-msgstr "Contagem"
+msgstr "Ilość"
 
 #: templates/debug_toolbar/panels/request.html:3
 msgid "View information"
-msgstr "Ver informação"
+msgstr "Pokaż informacje"
 
 #: templates/debug_toolbar/panels/request.html:7
 msgid "View function"
-msgstr "Função View"
+msgstr ""
 
 #: templates/debug_toolbar/panels/request.html:10
 msgid "URL name"
-msgstr "Nome da URL"
+msgstr ""
 
 #: templates/debug_toolbar/panels/request.html:24
 msgid "Cookies"
-msgstr "Cookies"
-
-#: templates/debug_toolbar/panels/request.html:32
-#: templates/debug_toolbar/panels/request.html:58
-#: templates/debug_toolbar/panels/request.html:84
-#: templates/debug_toolbar/panels/request.html:109
-msgid "Variable"
-msgstr "Variável"
+msgstr ""
 
-#: templates/debug_toolbar/panels/request.html:46
+#: templates/debug_toolbar/panels/request.html:27
 msgid "No cookies"
-msgstr "Sem Cookies"
+msgstr ""
 
-#: templates/debug_toolbar/panels/request.html:50
+#: templates/debug_toolbar/panels/request.html:31
 msgid "Session data"
-msgstr "Dados de Sessão"
+msgstr ""
 
-#: templates/debug_toolbar/panels/request.html:72
+#: templates/debug_toolbar/panels/request.html:34
 msgid "No session data"
-msgstr "Sem dados de Sessão"
+msgstr ""
 
-#: templates/debug_toolbar/panels/request.html:76
+#: templates/debug_toolbar/panels/request.html:38
 msgid "GET data"
-msgstr "Dados de GET"
+msgstr ""
 
-#: templates/debug_toolbar/panels/request.html:98
+#: templates/debug_toolbar/panels/request.html:41
 msgid "No GET data"
-msgstr "Não há dados de GET"
+msgstr "Brak danych GET"
 
-#: templates/debug_toolbar/panels/request.html:102
+#: templates/debug_toolbar/panels/request.html:45
 msgid "POST data"
-msgstr "Dados de POST"
+msgstr ""
 
-#: templates/debug_toolbar/panels/request.html:123
+#: templates/debug_toolbar/panels/request.html:48
 msgid "No POST data"
-msgstr "Não há dados de POST"
+msgstr "Brak danych POST"
 
 #: templates/debug_toolbar/panels/settings.html:5
 msgid "Setting"
-msgstr "Configuração"
+msgstr "Ustawienie"
 
 #: templates/debug_toolbar/panels/signals.html:5
 msgid "Signal"
-msgstr "Sinais"
+msgstr "Sygnał"
 
 #: templates/debug_toolbar/panels/signals.html:6
-msgid "Providing"
-msgstr "Fornecendo"
-
-#: templates/debug_toolbar/panels/signals.html:7
 msgid "Receivers"
-msgstr "Recebedores"
+msgstr "Odbiorcy"
 
-#: templates/debug_toolbar/panels/sql.html:7
+#: templates/debug_toolbar/panels/sql.html:6
 #, python-format
 msgid "%(num)s query"
 msgid_plural "%(num)s queries"
-msgstr[0] "%(num)s consulta"
-msgstr[1] "%(num)s consultas"
+msgstr[0] "%(num)s zapytanie"
+msgstr[1] "%(num)s zapytania"
+msgstr[2] "%(num)s zapytań"
 
-#: templates/debug_toolbar/panels/sql.html:18
+#: templates/debug_toolbar/panels/sql.html:8
+#, python-format
+msgid ""
+"including <abbr title=\"Similar queries are queries with the same SQL, but "
+"potentially different parameters.\">%(count)s similar</abbr>"
+msgstr ""
+
+#: templates/debug_toolbar/panels/sql.html:12
+#, python-format
+msgid ""
+"and <abbr title=\"Duplicate queries are identical to each other: they "
+"execute exactly the same SQL and parameters.\">%(dupes)s duplicates</abbr>"
+msgstr ""
+
+#: templates/debug_toolbar/panels/sql.html:34
 msgid "Query"
-msgstr "Query"
+msgstr "Zapytanie"
 
-#: templates/debug_toolbar/panels/sql.html:19
+#: templates/debug_toolbar/panels/sql.html:35
 #: templates/debug_toolbar/panels/timer.html:36
 msgid "Timeline"
-msgstr "Linha do tempo"
+msgstr "Oś czasu"
 
-#: templates/debug_toolbar/panels/sql.html:21
-msgid "Action"
-msgstr "Ação"
+#: templates/debug_toolbar/panels/sql.html:52
+#, fuzzy, python-format
+#| msgid "%(count)s message"
+#| msgid_plural "%(count)s messages"
+msgid "%(count)s similar queries."
+msgstr "%(count)s wiadomość"
 
-#: templates/debug_toolbar/panels/sql.html:64
+#: templates/debug_toolbar/panels/sql.html:58
+#, python-format
+msgid "Duplicated %(dupes)s times."
+msgstr ""
+
+#: templates/debug_toolbar/panels/sql.html:95
 msgid "Connection:"
-msgstr "Conexão:"
+msgstr "Połączenie:"
 
-#: templates/debug_toolbar/panels/sql.html:66
+#: templates/debug_toolbar/panels/sql.html:97
 msgid "Isolation level:"
-msgstr "Nível de isolamento:"
+msgstr "Poziom izolacji:"
 
-#: templates/debug_toolbar/panels/sql.html:69
+#: templates/debug_toolbar/panels/sql.html:100
 msgid "Transaction status:"
-msgstr "Status da transação:"
+msgstr "Status transakcji:"
 
-#: templates/debug_toolbar/panels/sql.html:83
+#: templates/debug_toolbar/panels/sql.html:114
 msgid "(unknown)"
-msgstr "(unknown)"
+msgstr "(nieznany)"
 
-#: templates/debug_toolbar/panels/sql.html:92
+#: templates/debug_toolbar/panels/sql.html:123
 msgid "No SQL queries were recorded during this request."
-msgstr "Nenhuma consulta SQL foi registrada durante esta requisição."
-
-#: templates/debug_toolbar/panels/sql_explain.html:3
-#: templates/debug_toolbar/panels/sql_profile.html:3
-#: templates/debug_toolbar/panels/sql_select.html:3
-#: templates/debug_toolbar/panels/template_source.html:3
-msgid "Back"
-msgstr "Voltar"
+msgstr "Żadne zapytania SQL nie zostały odnotowane podczas tego zapytania."
 
 #: templates/debug_toolbar/panels/sql_explain.html:4
 msgid "SQL explained"
-msgstr "SQL explicada"
+msgstr ""
 
 #: templates/debug_toolbar/panels/sql_explain.html:9
 #: templates/debug_toolbar/panels/sql_profile.html:10
 #: templates/debug_toolbar/panels/sql_select.html:9
 msgid "Executed SQL"
-msgstr "SQL Executada"
+msgstr "Wykonane zapytanie SQL"
 
 #: templates/debug_toolbar/panels/sql_explain.html:13
 #: templates/debug_toolbar/panels/sql_profile.html:14
 #: templates/debug_toolbar/panels/sql_select.html:13
 msgid "Database"
-msgstr "Banco de dados"
+msgstr "Baza danych"
 
 #: templates/debug_toolbar/panels/sql_profile.html:4
 msgid "SQL profiled"
-msgstr "SQL perfilado"
+msgstr ""
 
 #: templates/debug_toolbar/panels/sql_profile.html:37
 msgid "Error"
-msgstr "Erro"
+msgstr "Błąd"
 
 #: templates/debug_toolbar/panels/sql_select.html:4
 msgid "SQL selected"
-msgstr "SQL selecionada"
+msgstr ""
 
 #: templates/debug_toolbar/panels/sql_select.html:36
 msgid "Empty set"
-msgstr "Conjunto vazio"
+msgstr "Pusty zbiór"
 
-#: templates/debug_toolbar/panels/staticfiles.html:4
+#: templates/debug_toolbar/panels/staticfiles.html:3
 msgid "Static file path"
 msgid_plural "Static file paths"
-msgstr[0] "Caminho do arquivo estático"
-msgstr[1] "Caminho dos arquivos estáticos"
+msgstr[0] ""
+msgstr[1] ""
+msgstr[2] ""
 
-#: templates/debug_toolbar/panels/staticfiles.html:8
+#: templates/debug_toolbar/panels/staticfiles.html:7
 #, python-format
 msgid "(prefix %(prefix)s)"
-msgstr "(prefixo %(prefix)s)"
+msgstr ""
 
-#: templates/debug_toolbar/panels/staticfiles.html:12
-#: templates/debug_toolbar/panels/staticfiles.html:23
-#: templates/debug_toolbar/panels/staticfiles.html:35
+#: templates/debug_toolbar/panels/staticfiles.html:11
+#: templates/debug_toolbar/panels/staticfiles.html:22
+#: templates/debug_toolbar/panels/staticfiles.html:34
 #: templates/debug_toolbar/panels/templates.html:10
-#: templates/debug_toolbar/panels/templates.html:28
-#: templates/debug_toolbar/panels/templates.html:43
+#: templates/debug_toolbar/panels/templates.html:30
+#: templates/debug_toolbar/panels/templates.html:47
 msgid "None"
-msgstr "Nenhum"
+msgstr "Brak"
 
-#: templates/debug_toolbar/panels/staticfiles.html:15
+#: templates/debug_toolbar/panels/staticfiles.html:14
 msgid "Static file app"
 msgid_plural "Static file apps"
-msgstr[0] "Arquivo estático de app"
-msgstr[1] "Arquivos estáticos de apps"
+msgstr[0] ""
+msgstr[1] ""
+msgstr[2] ""
 
-#: templates/debug_toolbar/panels/staticfiles.html:26
+#: templates/debug_toolbar/panels/staticfiles.html:25
 msgid "Static file"
 msgid_plural "Static files"
-msgstr[0] "Arquivo estático"
-msgstr[1] "Arquivos estáticos"
+msgstr[0] ""
+msgstr[1] ""
+msgstr[2] ""
 
-#: templates/debug_toolbar/panels/staticfiles.html:40
+#: templates/debug_toolbar/panels/staticfiles.html:39
 #, python-format
 msgid "%(payload_count)s file"
 msgid_plural "%(payload_count)s files"
-msgstr[0] "%(payload_count)s arquivo"
-msgstr[1] "%(payload_count)s arquivos"
+msgstr[0] ""
+msgstr[1] ""
+msgstr[2] ""
 
 #: templates/debug_toolbar/panels/staticfiles.html:44
-msgid "Path"
-msgstr "Caminho"
+msgid "Location"
+msgstr "Lokalizacja"
 
 #: templates/debug_toolbar/panels/template_source.html:4
 msgid "Template source:"
-msgstr "Origem do Template:"
+msgstr ""
 
 #: templates/debug_toolbar/panels/templates.html:2
 msgid "Template path"
 msgid_plural "Template paths"
-msgstr[0] "Caminho do Template"
-msgstr[1] "Caminho do Templates"
+msgstr[0] "Ścieżka templatki"
+msgstr[1] "Ścieżki templatek"
+msgstr[2] "Ścieżki templatek"
 
 #: templates/debug_toolbar/panels/templates.html:13
 msgid "Template"
 msgid_plural "Templates"
-msgstr[0] "Template"
-msgstr[1] "Templates"
+msgstr[0] "Templatki"
+msgstr[1] "Templatki"
+msgstr[2] "Templatki"
 
-#: templates/debug_toolbar/panels/templates.html:21
-#: templates/debug_toolbar/panels/templates.html:37
+#: templates/debug_toolbar/panels/templates.html:22
+#: templates/debug_toolbar/panels/templates.html:40
 msgid "Toggle context"
-msgstr "Alternar contexto"
+msgstr ""
 
-#: templates/debug_toolbar/panels/templates.html:31
+#: templates/debug_toolbar/panels/templates.html:33
 msgid "Context processor"
 msgid_plural "Context processors"
 msgstr[0] ""
-msgstr[1] "Processador do Contexto"
+msgstr[1] ""
+msgstr[2] ""
 
 #: templates/debug_toolbar/panels/timer.html:2
 msgid "Resource usage"
-msgstr "Uso de recursos"
+msgstr ""
 
 #: templates/debug_toolbar/panels/timer.html:10
 msgid "Resource"
-msgstr "Recurso"
+msgstr "Zasób"
 
 #: templates/debug_toolbar/panels/timer.html:26
 msgid "Browser timing"
-msgstr "Cronometragem do Navegador"
+msgstr ""
 
 #: templates/debug_toolbar/panels/timer.html:35
 msgid "Timing attribute"
-msgstr "Atributo de Cronometragem"
+msgstr ""
 
 #: templates/debug_toolbar/panels/timer.html:37
 msgid "Milliseconds since navigation start (+length)"
-msgstr "Milissegundos desde início de navegação (+length)"
+msgstr ""
 
-#: templates/debug_toolbar/panels/versions.html:5
+#: templates/debug_toolbar/panels/versions.html:10
+msgid "Package"
+msgstr ""
+
+#: templates/debug_toolbar/panels/versions.html:11
 msgid "Name"
-msgstr "Nome"
+msgstr "Nazwa"
 
-#: templates/debug_toolbar/panels/versions.html:6
+#: templates/debug_toolbar/panels/versions.html:12
 msgid "Version"
-msgstr "Versão"
+msgstr "Wersja"
+
+#: templates/debug_toolbar/redirect.html:10
+msgid "Location:"
+msgstr ""
+
+#: templates/debug_toolbar/redirect.html:12
+msgid ""
+"The Django Debug Toolbar has intercepted a redirect to the above URL for "
+"debug viewing purposes. You can click the above link to continue with the "
+"redirect as normal."
+msgstr ""
+
+#: views.py:16
+msgid ""
+"Data for this panel isn't available anymore. Please reload the page and "
+"retry."
+msgstr ""
```

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/locale/ru/LC_MESSAGES/django.mo` & `django_debug_toolbar-4.0.0/debug_toolbar/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/locale/ru/LC_MESSAGES/django.po` & `django_debug_toolbar-4.0.0/debug_toolbar/locale/ru/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -7,76 +7,62 @@
 # Ilya Baryshev <baryshev@gmail.com>, 2013
 # Mikhail Korobov, 2009
 # Алексей Борискин <sun.void@gmail.com>, 2013,2015
 msgid ""
 msgstr ""
 "Project-Id-Version: Django Debug Toolbar\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-08-14 10:25-0500\n"
+"POT-Creation-Date: 2023-01-20 17:23+0100\n"
 "PO-Revision-Date: 2021-08-14 15:25+0000\n"
 "Last-Translator: Tim Schilling\n"
-"Language-Team: Russian (http://www.transifex.com/django-debug-toolbar/django-debug-toolbar/language/ru/)\n"
+"Language-Team: Russian (http://www.transifex.com/django-debug-toolbar/django-"
+"debug-toolbar/language/ru/)\n"
+"Language: ru\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: ru\n"
-"Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && n%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || (n%100>=11 && n%100<=14)? 2 : 3);\n"
+"Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
+"n%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || "
+"(n%100>=11 && n%100<=14)? 2 : 3);\n"
 
 #: apps.py:15
 msgid "Debug Toolbar"
 msgstr "Панель отладки"
 
-#: panels/cache.py:227
+#: panels/cache.py:180
 msgid "Cache"
 msgstr "Кэш"
 
-#: panels/cache.py:234
+#: panels/cache.py:186
 #, python-format
 msgid "%(cache_calls)d call in %(time).2fms"
 msgid_plural "%(cache_calls)d calls in %(time).2fms"
 msgstr[0] "%(cache_calls)d обращение за %(time).2fms"
 msgstr[1] "%(cache_calls)d обращения за %(time).2fms"
 msgstr[2] "%(cache_calls)d обращений за %(time).2fms"
 msgstr[3] "%(cache_calls)d обращений за %(time).2fms"
 
-#: panels/cache.py:246
+#: panels/cache.py:195
 #, python-format
 msgid "Cache calls from %(count)d backend"
 msgid_plural "Cache calls from %(count)d backends"
 msgstr[0] "Обращения к кэшу от %(count)d бэкенда"
 msgstr[1] "Обращения к кэшу от %(count)d бэкендов"
 msgstr[2] "Обращения к кэшу от %(count)d бэкендов"
 msgstr[3] "Обращения к кэшу от %(count)d бэкендов"
 
-#: panels/headers.py:33
+#: panels/headers.py:31
 msgid "Headers"
 msgstr "Заголовки"
 
-#: panels/history/panel.py:20 panels/history/panel.py:21
+#: panels/history/panel.py:18 panels/history/panel.py:19
 msgid "History"
 msgstr ""
 
-#: panels/logging.py:63
-msgid "Logging"
-msgstr "Логи"
-
-#: panels/logging.py:69
-#, python-format
-msgid "%(count)s message"
-msgid_plural "%(count)s messages"
-msgstr[0] "%(count)s сообщение"
-msgstr[1] "%(count)s сообщений"
-msgstr[2] "%(count)s сообщений"
-msgstr[3] "%(count)s сообщений"
-
-#: panels/logging.py:73
-msgid "Log messages"
-msgstr "Сообщения в логе"
-
-#: panels/profiling.py:150
+#: panels/profiling.py:140
 msgid "Profiling"
 msgstr "Профилирование"
 
 #: panels/redirects.py:14
 msgid "Intercept redirects"
 msgstr "Перехват редиректов"
 
@@ -88,150 +74,149 @@
 msgid "<no view>"
 msgstr "<нет view>"
 
 #: panels/request.py:53
 msgid "<unavailable>"
 msgstr "<недоступно>"
 
-#: panels/settings.py:24
+#: panels/settings.py:17
 msgid "Settings"
 msgstr "Настройки"
 
-#: panels/settings.py:27
+#: panels/settings.py:20
 #, python-format
 msgid "Settings from %s"
 msgstr ""
 
-#: panels/signals.py:58
+#: panels/signals.py:57
 #, python-format
 msgid "%(num_receivers)d receiver of 1 signal"
 msgid_plural "%(num_receivers)d receivers of 1 signal"
 msgstr[0] "%(num_receivers)d получатель 1 сигнала"
 msgstr[1] "%(num_receivers)d получателя 1 сигнала"
 msgstr[2] "%(num_receivers)d получателей 1 сигнала"
 msgstr[3] "%(num_receivers)d получателей 1 сигнала"
 
-#: panels/signals.py:66
+#: panels/signals.py:62
 #, python-format
 msgid "%(num_receivers)d receiver of %(num_signals)d signals"
 msgid_plural "%(num_receivers)d receivers of %(num_signals)d signals"
 msgstr[0] "%(num_receivers)d получатель %(num_signals)d сигнала(ов)"
 msgstr[1] "%(num_receivers)d получателя %(num_signals)d сигнала(ов)"
 msgstr[2] "%(num_receivers)d получателей %(num_signals)d сигнала(ов)"
 msgstr[3] "%(num_receivers)d получателей %(num_signals)d сигнала(ов)"
 
-#: panels/signals.py:73
+#: panels/signals.py:67
 msgid "Signals"
 msgstr "Сигналы"
 
-#: panels/sql/panel.py:24
+#: panels/sql/panel.py:23
 msgid "Autocommit"
 msgstr "Autocommit"
 
-#: panels/sql/panel.py:25
+#: panels/sql/panel.py:24
 msgid "Read uncommitted"
 msgstr "Read uncommitted"
 
-#: panels/sql/panel.py:26
+#: panels/sql/panel.py:25
 msgid "Read committed"
 msgstr "Read committed"
 
-#: panels/sql/panel.py:27
+#: panels/sql/panel.py:26
 msgid "Repeatable read"
 msgstr "Repeatable read"
 
-#: panels/sql/panel.py:28
+#: panels/sql/panel.py:27
 msgid "Serializable"
 msgstr "Serializable"
 
-#: panels/sql/panel.py:40
+#: panels/sql/panel.py:39
 msgid "Idle"
 msgstr "Ожидание"
 
-#: panels/sql/panel.py:41
+#: panels/sql/panel.py:40
 msgid "Active"
 msgstr "Действие"
 
-#: panels/sql/panel.py:42
+#: panels/sql/panel.py:41
 msgid "In transaction"
 msgstr "В транзакции"
 
-#: panels/sql/panel.py:43
+#: panels/sql/panel.py:42
 msgid "In error"
 msgstr "Ошибка"
 
-#: panels/sql/panel.py:44
+#: panels/sql/panel.py:43
 msgid "Unknown"
 msgstr "Неизвестно"
 
-#: panels/sql/panel.py:109
+#: panels/sql/panel.py:130
 msgid "SQL"
 msgstr "SQL"
 
-#: panels/sql/panel.py:114
+#: panels/sql/panel.py:135
 #, python-format
 msgid "%(query_count)d query in %(sql_time).2fms"
 msgid_plural "%(query_count)d queries in %(sql_time).2fms"
 msgstr[0] ""
 msgstr[1] ""
 msgstr[2] ""
 msgstr[3] ""
 
-#: panels/sql/panel.py:127
+#: panels/sql/panel.py:147
 #, python-format
 msgid "SQL queries from %(count)d connection"
 msgid_plural "SQL queries from %(count)d connections"
 msgstr[0] ""
 msgstr[1] ""
 msgstr[2] ""
 msgstr[3] ""
 
-#: panels/staticfiles.py:85
+#: panels/staticfiles.py:84
 #, python-format
 msgid "Static files (%(num_found)s found, %(num_used)s used)"
 msgstr "Статические файлы (найдено %(num_found)s, используется %(num_used)s)"
 
-#: panels/staticfiles.py:106
+#: panels/staticfiles.py:105
 msgid "Static files"
 msgstr "Статические файлы"
 
-#: panels/staticfiles.py:112
+#: panels/staticfiles.py:111
 #, python-format
 msgid "%(num_used)s file used"
 msgid_plural "%(num_used)s files used"
 msgstr[0] "%(num_used)s файл используется"
 msgstr[1] " %(num_used)s файла используется"
 msgstr[2] "%(num_used)s файлов используется"
 msgstr[3] "%(num_used)s файлов используется"
 
-#: panels/templates/panel.py:144
+#: panels/templates/panel.py:143
 msgid "Templates"
 msgstr "Шаблоны"
 
-#: panels/templates/panel.py:149
+#: panels/templates/panel.py:148
 #, python-format
 msgid "Templates (%(num_templates)s rendered)"
 msgstr "Шаблоны (обработано %(num_templates)s)"
 
-#: panels/templates/panel.py:181
+#: panels/templates/panel.py:180
 msgid "No origin"
 msgstr ""
 
 #: panels/timer.py:25
 #, python-format
 msgid "CPU: %(cum)0.2fms (%(total)0.2fms)"
 msgstr "CPU: %(cum)0.2fms (%(total)0.2fms)"
 
 #: panels/timer.py:30
 #, python-format
 msgid "Total: %0.2fms"
 msgstr "Итого: %0.2fms"
 
 #: panels/timer.py:36 templates/debug_toolbar/panels/history.html:9
-#: templates/debug_toolbar/panels/logging.html:7
 #: templates/debug_toolbar/panels/sql_explain.html:11
 #: templates/debug_toolbar/panels/sql_profile.html:12
 #: templates/debug_toolbar/panels/sql_select.html:11
 msgid "Time"
 msgstr "Время"
 
 #: panels/timer.py:44
@@ -279,23 +264,23 @@
 msgid "%(vcsw)d voluntary, %(ivcsw)d involuntary"
 msgstr "%(vcsw)d намеренных, %(ivcsw)d вынужденных"
 
 #: panels/versions.py:19
 msgid "Versions"
 msgstr "Версии"
 
-#: templates/debug_toolbar/base.html:18
+#: templates/debug_toolbar/base.html:22
 msgid "Hide toolbar"
 msgstr "Скрыть панель"
 
-#: templates/debug_toolbar/base.html:18
+#: templates/debug_toolbar/base.html:22
 msgid "Hide"
 msgstr "Скрыть"
 
-#: templates/debug_toolbar/base.html:25
+#: templates/debug_toolbar/base.html:29
 msgid "Show toolbar"
 msgstr "Показать панель"
 
 #: templates/debug_toolbar/includes/panel_button.html:4
 msgid "Disable for next and successive requests"
 msgstr "Отключить для последующих запросов"
 
@@ -364,15 +349,15 @@
 msgid "Key"
 msgstr "Заголовок"
 
 #: templates/debug_toolbar/panels/headers.html:9
 #: templates/debug_toolbar/panels/headers.html:28
 #: templates/debug_toolbar/panels/headers.html:49
 #: templates/debug_toolbar/panels/history_tr.html:23
-#: templates/debug_toolbar/panels/request_variables.html:11
+#: templates/debug_toolbar/panels/request_variables.html:12
 #: templates/debug_toolbar/panels/settings.html:6
 #: templates/debug_toolbar/panels/timer.html:11
 msgid "Value"
 msgstr "Значение"
 
 #: templates/debug_toolbar/panels/headers.html:22
 msgid "Response headers"
@@ -382,15 +367,17 @@
 msgid "WSGI environ"
 msgstr "WSGI-окружение"
 
 #: templates/debug_toolbar/panels/headers.html:43
 msgid ""
 "Since the WSGI environ inherits the environment of the server, only a "
 "significant subset is shown below."
-msgstr "Так как WSGI-окружение наследует окружение сервера, ниже отображены лишь те из переменных, которые важны для нужд отладки."
+msgstr ""
+"Так как WSGI-окружение наследует окружение сервера, ниже отображены лишь те "
+"из переменных, которые важны для нужд отладки."
 
 #: templates/debug_toolbar/panels/history.html:10
 msgid "Method"
 msgstr "Метод"
 
 #: templates/debug_toolbar/panels/history.html:11
 #: templates/debug_toolbar/panels/staticfiles.html:43
@@ -407,39 +394,18 @@
 
 #: templates/debug_toolbar/panels/history.html:14
 #: templates/debug_toolbar/panels/sql.html:37
 msgid "Action"
 msgstr "Действие"
 
 #: templates/debug_toolbar/panels/history_tr.html:22
-#: templates/debug_toolbar/panels/request_variables.html:10
+#: templates/debug_toolbar/panels/request_variables.html:11
 msgid "Variable"
 msgstr "Переменная"
 
-#: templates/debug_toolbar/panels/logging.html:6
-msgid "Level"
-msgstr "Уровень"
-
-#: templates/debug_toolbar/panels/logging.html:8
-msgid "Channel"
-msgstr "Канал"
-
-#: templates/debug_toolbar/panels/logging.html:9
-msgid "Message"
-msgstr "Сообщение"
-
-#: templates/debug_toolbar/panels/logging.html:10
-#: templates/debug_toolbar/panels/staticfiles.html:44
-msgid "Location"
-msgstr "Место"
-
-#: templates/debug_toolbar/panels/logging.html:26
-msgid "No messages logged"
-msgstr "Сообщений нет"
-
 #: templates/debug_toolbar/panels/profiling.html:5
 msgid "Call"
 msgstr "Вызов"
 
 #: templates/debug_toolbar/panels/profiling.html:6
 msgid "CumTime"
 msgstr "КумулВрем"
@@ -569,15 +535,16 @@
 
 #: templates/debug_toolbar/panels/sql.html:114
 msgid "(unknown)"
 msgstr "(неизвестно)"
 
 #: templates/debug_toolbar/panels/sql.html:123
 msgid "No SQL queries were recorded during this request."
-msgstr "Во время обработки этого HTTP-запроса не было записано ни одного SQL-запроса."
+msgstr ""
+"Во время обработки этого HTTP-запроса не было записано ни одного SQL-запроса."
 
 #: templates/debug_toolbar/panels/sql_explain.html:4
 msgid "SQL explained"
 msgstr "SQL Explain"
 
 #: templates/debug_toolbar/panels/sql_explain.html:9
 #: templates/debug_toolbar/panels/sql_profile.html:10
@@ -650,14 +617,18 @@
 msgid "%(payload_count)s file"
 msgid_plural "%(payload_count)s files"
 msgstr[0] "%(payload_count)s файл"
 msgstr[1] "%(payload_count)s файла"
 msgstr[2] "%(payload_count)s файлов"
 msgstr[3] "%(payload_count)s файлов"
 
+#: templates/debug_toolbar/panels/staticfiles.html:44
+msgid "Location"
+msgstr "Место"
+
 #: templates/debug_toolbar/panels/template_source.html:4
 msgid "Template source:"
 msgstr "Источник шаблона:"
 
 #: templates/debug_toolbar/panels/templates.html:2
 msgid "Template path"
 msgid_plural "Template paths"
@@ -724,14 +695,18 @@
 msgstr "Адрес:"
 
 #: templates/debug_toolbar/redirect.html:12
 msgid ""
 "The Django Debug Toolbar has intercepted a redirect to the above URL for "
 "debug viewing purposes. You can click the above link to continue with the "
 "redirect as normal."
-msgstr "Django Debug Toolbar в перехватил редирект на адрес, указанный выше. Вы можете нажать на ссылку, чтобы выполнить переход самостоятельно."
+msgstr ""
+"Django Debug Toolbar в перехватил редирект на адрес, указанный выше. Вы "
+"можете нажать на ссылку, чтобы выполнить переход самостоятельно."
 
-#: views.py:15
+#: views.py:16
 msgid ""
 "Data for this panel isn't available anymore. Please reload the page and "
 "retry."
-msgstr "Данные этой панели больше недоступны. Пожалуйста, перезагрузите страницу и попробуйте ещё раз."
+msgstr ""
+"Данные этой панели больше недоступны. Пожалуйста, перезагрузите страницу и "
+"попробуйте ещё раз."
```

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/locale/sk/LC_MESSAGES/django.mo` & `django_debug_toolbar-4.0.0/debug_toolbar/locale/sk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/locale/sk/LC_MESSAGES/django.po` & `django_debug_toolbar-4.0.0/debug_toolbar/locale/sk/LC_MESSAGES/django.po`

 * *Files 4% similar despite different names*

```diff
@@ -6,296 +6,294 @@
 # Juraj Bubniak <translations@jbub.eu>, 2012
 # Juraj Bubniak <translations@jbub.eu>, 2013
 # Rastislav Kober <kybiky@gmail.com>, 2012
 msgid ""
 msgstr ""
 "Project-Id-Version: Django Debug Toolbar\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2014-04-25 21:52+0200\n"
+"POT-Creation-Date: 2023-01-20 17:23+0100\n"
 "PO-Revision-Date: 2021-06-24 13:37+0200\n"
 "Last-Translator: Aymeric Augustin <aymeric.augustin@m4x.org>\n"
-"Language-Team: Slovak (http://www.transifex.com/projects/p/django-debug-toolbar/language/sk/)\n"
+"Language-Team: Slovak (http://www.transifex.com/projects/p/django-debug-"
+"toolbar/language/sk/)\n"
+"Language: sk\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: sk\n"
-"Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n == 1 ? 0 : n % 1 == 0 && n >= 2 && n <= 4 ? 1 : n % 1 != 0 ? 2: 3);\n"
+"Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n == 1 ? 0 : n % 1 == 0 && n "
+">= 2 && n <= 4 ? 1 : n % 1 != 0 ? 2: 3);\n"
 "X-Generator: Poedit 2.4.2\n"
 
-#: apps.py:11
+#: apps.py:15
 msgid "Debug Toolbar"
 msgstr "Debug Toolbar"
 
-#: views.py:14
-msgid "Data for this panel isn't available anymore. Please reload the page and retry."
-msgstr "Dáta pre tento panel už nie sú k dispozícii. Načítajte si prosím stránku a skúste to znova."
-
-#: panels/cache.py:191
+#: panels/cache.py:180
 msgid "Cache"
 msgstr "Cache"
 
-#: panels/cache.py:196
+#: panels/cache.py:186
 #, python-format
 msgid "%(cache_calls)d call in %(time).2fms"
 msgid_plural "%(cache_calls)d calls in %(time).2fms"
 msgstr[0] "%(cache_calls)d volanie za %(time).2fms"
 msgstr[1] "%(cache_calls)d volania za %(time).2fms"
 msgstr[2] "%(cache_calls)d volaní za %(time).2fms"
 msgstr[3] "%(cache_calls)d volaní za %(time).2fms"
 
-#: panels/cache.py:204
+#: panels/cache.py:195
 #, python-format
 msgid "Cache calls from %(count)d backend"
 msgid_plural "Cache calls from %(count)d backends"
 msgstr[0] "Cache volania z %(count)d backendu"
 msgstr[1] "Cache volania z %(count)d backendov"
 msgstr[2] "Cache volania z %(count)d backendu"
 msgstr[3] "Cache volania z %(count)d backendov"
 
-#: panels/headers.py:35
+#: panels/headers.py:31
 msgid "Headers"
 msgstr "Hlavičky"
 
-#: panels/logging.py:64
-msgid "Logging"
-msgstr "Zápis"
-
-#: panels/logging.py:70
-#, python-format
-msgid "%(count)s message"
-msgid_plural "%(count)s messages"
-msgstr[0] "%(count)s správa"
-msgstr[1] "%(count)s správy"
-msgstr[2] "%(count)s správy"
-msgstr[3] "%(count)s správ"
-
-#: panels/logging.py:73
-msgid "Log messages"
-msgstr "Správy zápisu"
+#: panels/history/panel.py:18 panels/history/panel.py:19
+msgid "History"
+msgstr ""
 
-#: panels/profiling.py:127
+#: panels/profiling.py:140
 msgid "Profiling"
 msgstr "Analýza"
 
-#: panels/redirects.py:17
+#: panels/redirects.py:14
 msgid "Intercept redirects"
 msgstr "Zachytiť presmerovania"
 
-#: panels/request.py:18
+#: panels/request.py:16
 msgid "Request"
 msgstr "Požiadavka"
 
-#: panels/request.py:35
+#: panels/request.py:36
 msgid "<no view>"
 msgstr "<ziadne zobrazenie>"
 
-#: panels/request.py:47
+#: panels/request.py:53
 msgid "<unavailable>"
 msgstr "<nedostupny>"
 
-#: panels/settings.py:20
+#: panels/settings.py:17
 msgid "Settings"
 msgstr "Nastavenia"
 
-#: panels/settings.py:23
-#, python-format
-msgid "Settings from <code>%s</code>"
+#: panels/settings.py:20
+#, fuzzy, python-format
+#| msgid "Settings from <code>%s</code>"
+msgid "Settings from %s"
 msgstr "Nastavenia z <code>%s</code>"
 
-#: panels/signals.py:45
+#: panels/signals.py:57
 #, python-format
 msgid "%(num_receivers)d receiver of 1 signal"
 msgid_plural "%(num_receivers)d receivers of 1 signal"
 msgstr[0] "%(num_receivers)d príjemca 1 signálu"
 msgstr[1] "%(num_receivers)d príjemcovia 1 signálu"
 msgstr[2] "%(num_receivers)d príjemcov 1 signálu"
 msgstr[3] "%(num_receivers)d príjemcov 1 signálu"
 
-#: panels/signals.py:48
+#: panels/signals.py:62
 #, python-format
 msgid "%(num_receivers)d receiver of %(num_signals)d signals"
 msgid_plural "%(num_receivers)d receivers of %(num_signals)d signals"
 msgstr[0] "%(num_receivers)d príjemca %(num_signals)d signálu"
 msgstr[1] "%(num_receivers)d príjemcov %(num_signals)d signálov"
 msgstr[2] "%(num_receivers)d príjemcu %(num_signals)d signálu"
 msgstr[3] "%(num_receivers)d príjemcov %(num_signals)d signálov"
 
-#: panels/signals.py:53
+#: panels/signals.py:67
 msgid "Signals"
 msgstr "Signály"
 
-#: panels/staticfiles.py:89
+#: panels/sql/panel.py:23
+msgid "Autocommit"
+msgstr "Autocommit"
+
+#: panels/sql/panel.py:24
+msgid "Read uncommitted"
+msgstr "Read uncommitted"
+
+#: panels/sql/panel.py:25
+msgid "Read committed"
+msgstr "Read committed"
+
+#: panels/sql/panel.py:26
+msgid "Repeatable read"
+msgstr "Opakovateľné čítanie"
+
+#: panels/sql/panel.py:27
+msgid "Serializable"
+msgstr "Premenná"
+
+#: panels/sql/panel.py:39
+msgid "Idle"
+msgstr "Nečinný"
+
+#: panels/sql/panel.py:40
+msgid "Active"
+msgstr "Aktívne"
+
+#: panels/sql/panel.py:41
+msgid "In transaction"
+msgstr "V transakcii"
+
+#: panels/sql/panel.py:42
+msgid "In error"
+msgstr "Chyba"
+
+#: panels/sql/panel.py:43
+msgid "Unknown"
+msgstr "(neznámy)"
+
+#: panels/sql/panel.py:130
+msgid "SQL"
+msgstr "SQL"
+
+#: panels/sql/panel.py:135
+#, fuzzy, python-format
+#| msgid "%(cache_calls)d call in %(time).2fms"
+#| msgid_plural "%(cache_calls)d calls in %(time).2fms"
+msgid "%(query_count)d query in %(sql_time).2fms"
+msgid_plural "%(query_count)d queries in %(sql_time).2fms"
+msgstr[0] "%(cache_calls)d volanie za %(time).2fms"
+msgstr[1] "%(cache_calls)d volania za %(time).2fms"
+msgstr[2] "%(cache_calls)d volaní za %(time).2fms"
+msgstr[3] "%(cache_calls)d volaní za %(time).2fms"
+
+#: panels/sql/panel.py:147
+#, python-format
+msgid "SQL queries from %(count)d connection"
+msgid_plural "SQL queries from %(count)d connections"
+msgstr[0] ""
+msgstr[1] ""
+msgstr[2] ""
+msgstr[3] ""
+
+#: panels/staticfiles.py:84
 #, python-format
 msgid "Static files (%(num_found)s found, %(num_used)s used)"
 msgstr "Statické súbory (%(num_found)s nájdených, %(num_used)s použitých)"
 
-#: panels/staticfiles.py:107
+#: panels/staticfiles.py:105
 msgid "Static files"
 msgstr "Statické súbory"
 
-#: panels/staticfiles.py:112
+#: panels/staticfiles.py:111
 #, python-format
 msgid "%(num_used)s file used"
 msgid_plural "%(num_used)s files used"
 msgstr[0] "%(num_used)s použitý súbor"
 msgstr[1] "%(num_used)s použité súbory"
 msgstr[2] "%(num_used)s použitých súborov"
 msgstr[3] "%(num_used)s použitých súborov"
 
-#: panels/timer.py:23
+#: panels/templates/panel.py:143
+msgid "Templates"
+msgstr "Šablóny"
+
+#: panels/templates/panel.py:148
+#, python-format
+msgid "Templates (%(num_templates)s rendered)"
+msgstr "Šablóny (%(num_templates)s spracovaných)"
+
+#: panels/templates/panel.py:180
+msgid "No origin"
+msgstr ""
+
+#: panels/timer.py:25
 #, python-format
 msgid "CPU: %(cum)0.2fms (%(total)0.2fms)"
 msgstr "CPU: %(cum)0.2fms (%(total)0.2fms)"
 
-#: panels/timer.py:28
+#: panels/timer.py:30
 #, python-format
 msgid "Total: %0.2fms"
 msgstr "Celkovo: %0.2fms"
 
-#: panels/timer.py:34 templates/debug_toolbar/panels/logging.html:7 templates/debug_toolbar/panels/sql_explain.html:11
-#: templates/debug_toolbar/panels/sql_profile.html:12 templates/debug_toolbar/panels/sql_select.html:11
+#: panels/timer.py:36 templates/debug_toolbar/panels/history.html:9
+#: templates/debug_toolbar/panels/sql_explain.html:11
+#: templates/debug_toolbar/panels/sql_profile.html:12
+#: templates/debug_toolbar/panels/sql_select.html:11
 msgid "Time"
 msgstr "Čas"
 
-#: panels/timer.py:42
+#: panels/timer.py:44
 msgid "User CPU time"
 msgstr "Užívateľský čas CPU"
 
-#: panels/timer.py:42
+#: panels/timer.py:44
 #, python-format
 msgid "%(utime)0.3f msec"
 msgstr "%(utime)0.3f msek"
 
-#: panels/timer.py:43
+#: panels/timer.py:45
 msgid "System CPU time"
 msgstr "Systémový čas CPU"
 
-#: panels/timer.py:43
+#: panels/timer.py:45
 #, python-format
 msgid "%(stime)0.3f msec"
 msgstr "%(stime)0.3f msek"
 
-#: panels/timer.py:44
+#: panels/timer.py:46
 msgid "Total CPU time"
 msgstr "Celkový čas CPU"
 
-#: panels/timer.py:44
+#: panels/timer.py:46
 #, python-format
 msgid "%(total)0.3f msec"
 msgstr "%(total)0.3f msek"
 
-#: panels/timer.py:45
+#: panels/timer.py:47
 msgid "Elapsed time"
 msgstr "Uplynutý čas"
 
-#: panels/timer.py:45
+#: panels/timer.py:47
 #, python-format
 msgid "%(total_time)0.3f msec"
 msgstr "%(total_time)0.3f msek"
 
-#: panels/timer.py:46
+#: panels/timer.py:49
 msgid "Context switches"
 msgstr "Prepnutí kontextu"
 
-#: panels/timer.py:46
+#: panels/timer.py:50
 #, python-format
 msgid "%(vcsw)d voluntary, %(ivcsw)d involuntary"
 msgstr "%(vcsw)d dobrovoľných, %(ivcsw)d nedobrovoľných"
 
-#: panels/versions.py:25
+#: panels/versions.py:19
 msgid "Versions"
 msgstr "Verzie"
 
-#: panels/sql/panel.py:22
-msgid "Autocommit"
-msgstr "Autocommit"
-
-#: panels/sql/panel.py:23
-msgid "Read uncommitted"
-msgstr "Read uncommitted"
-
-#: panels/sql/panel.py:24
-msgid "Read committed"
-msgstr "Read committed"
-
-#: panels/sql/panel.py:25
-msgid "Repeatable read"
-msgstr "Opakovateľné čítanie"
-
-#: panels/sql/panel.py:26
-msgid "Serializable"
-msgstr "Premenná"
-
-#: panels/sql/panel.py:37
-msgid "Idle"
-msgstr "Nečinný"
-
-#: panels/sql/panel.py:38
-msgid "Active"
-msgstr "Aktívne"
-
-#: panels/sql/panel.py:39
-msgid "In transaction"
-msgstr "V transakcii"
-
-#: panels/sql/panel.py:40
-msgid "In error"
-msgstr "Chyba"
-
-#: panels/sql/panel.py:41
-msgid "Unknown"
-msgstr "(neznámy)"
-
-#: panels/sql/panel.py:105
-msgid "SQL"
-msgstr "SQL"
-
-#: panels/templates/panel.py:141
-msgid "Templates"
-msgstr "Šablóny"
-
-#: panels/templates/panel.py:146
-#, python-format
-msgid "Templates (%(num_templates)s rendered)"
-msgstr "Šablóny (%(num_templates)s spracovaných)"
-
-#: templates/debug_toolbar/base.html:19
+#: templates/debug_toolbar/base.html:22
 msgid "Hide toolbar"
 msgstr "Skryť panel nástrojov"
 
-#: templates/debug_toolbar/base.html:19
+#: templates/debug_toolbar/base.html:22
 msgid "Hide"
 msgstr "Skryť"
 
-#: templates/debug_toolbar/base.html:25
+#: templates/debug_toolbar/base.html:29
+msgid "Show toolbar"
+msgstr "Zobraziť panel nástrojov"
+
+#: templates/debug_toolbar/includes/panel_button.html:4
 msgid "Disable for next and successive requests"
 msgstr "Zakázať pre ďalšie a nasledujúce požiadavky"
 
-#: templates/debug_toolbar/base.html:25
+#: templates/debug_toolbar/includes/panel_button.html:4
 msgid "Enable for next and successive requests"
 msgstr "Povoliť pre ďalšie a nasledujúce požiadavky"
 
-#: templates/debug_toolbar/base.html:47
-msgid "Show toolbar"
-msgstr "Zobraziť panel nástrojov"
-
-#: templates/debug_toolbar/base.html:53
-msgid "Close"
-msgstr "Zatvoriť"
-
-#: templates/debug_toolbar/redirect.html:8
-msgid "Location:"
-msgstr "Poloha:"
-
-#: templates/debug_toolbar/redirect.html:10
-msgid ""
-"The Django Debug Toolbar has intercepted a redirect to the above URL for debug viewing purposes. You can click the above link to continue with the redirect "
-"as normal."
-msgstr "Django Debug Toolbar zachytil presmerovanie na vyššie uvedenú URL pre účely ladenia. Pre normálne presmerovanie môžete kliknúť na vyššie uvedený odkaz."
-
 #: templates/debug_toolbar/panels/cache.html:2
 msgid "Summary"
 msgstr "Zhrnutie"
 
 #: templates/debug_toolbar/panels/cache.html:6
 msgid "Total calls"
 msgstr "Celkovo volaní"
@@ -316,89 +314,112 @@
 msgid "Commands"
 msgstr "Príkazy"
 
 #: templates/debug_toolbar/panels/cache.html:39
 msgid "Calls"
 msgstr "Volania"
 
-#: templates/debug_toolbar/panels/cache.html:43 templates/debug_toolbar/panels/sql.html:20
+#: templates/debug_toolbar/panels/cache.html:43
+#: templates/debug_toolbar/panels/sql.html:36
 msgid "Time (ms)"
 msgstr "Čas (ms)"
 
 #: templates/debug_toolbar/panels/cache.html:44
 msgid "Type"
 msgstr "Typ"
 
-#: templates/debug_toolbar/panels/cache.html:45 templates/debug_toolbar/panels/request.html:8
+#: templates/debug_toolbar/panels/cache.html:45
+#: templates/debug_toolbar/panels/request.html:8
 msgid "Arguments"
 msgstr "Argumenty"
 
-#: templates/debug_toolbar/panels/cache.html:46 templates/debug_toolbar/panels/request.html:9
+#: templates/debug_toolbar/panels/cache.html:46
+#: templates/debug_toolbar/panels/request.html:9
 msgid "Keyword arguments"
 msgstr "Kľúčové argumenty"
 
 #: templates/debug_toolbar/panels/cache.html:47
 msgid "Backend"
 msgstr "Backend"
 
 #: templates/debug_toolbar/panels/headers.html:3
 msgid "Request headers"
 msgstr "Hlavičky požiadavky"
 
-#: templates/debug_toolbar/panels/headers.html:8 templates/debug_toolbar/panels/headers.html:27 templates/debug_toolbar/panels/headers.html:48
+#: templates/debug_toolbar/panels/headers.html:8
+#: templates/debug_toolbar/panels/headers.html:27
+#: templates/debug_toolbar/panels/headers.html:48
 msgid "Key"
 msgstr "Kľúč"
 
-#: templates/debug_toolbar/panels/headers.html:9 templates/debug_toolbar/panels/headers.html:28 templates/debug_toolbar/panels/headers.html:49
-#: templates/debug_toolbar/panels/request.html:33 templates/debug_toolbar/panels/request.html:59 templates/debug_toolbar/panels/request.html:85
-#: templates/debug_toolbar/panels/request.html:110 templates/debug_toolbar/panels/settings.html:6 templates/debug_toolbar/panels/timer.html:11
+#: templates/debug_toolbar/panels/headers.html:9
+#: templates/debug_toolbar/panels/headers.html:28
+#: templates/debug_toolbar/panels/headers.html:49
+#: templates/debug_toolbar/panels/history_tr.html:23
+#: templates/debug_toolbar/panels/request_variables.html:12
+#: templates/debug_toolbar/panels/settings.html:6
+#: templates/debug_toolbar/panels/timer.html:11
 msgid "Value"
 msgstr "Hodnota"
 
 #: templates/debug_toolbar/panels/headers.html:22
 msgid "Response headers"
 msgstr "Hlavičky odpovede"
 
 #: templates/debug_toolbar/panels/headers.html:41
 msgid "WSGI environ"
 msgstr "WSGI prostredie"
 
 #: templates/debug_toolbar/panels/headers.html:43
-msgid "Since the WSGI environ inherits the environment of the server, only a significant subset is shown below."
-msgstr "Keďže WSGI prostredie dedí z prostredia servera, je nižšie zobrazená iba významná podmnožina."
+msgid ""
+"Since the WSGI environ inherits the environment of the server, only a "
+"significant subset is shown below."
+msgstr ""
+"Keďže WSGI prostredie dedí z prostredia servera, je nižšie zobrazená iba "
+"významná podmnožina."
 
-#: templates/debug_toolbar/panels/logging.html:6
-msgid "Level"
-msgstr "Úroveň"
-
-#: templates/debug_toolbar/panels/logging.html:8
-msgid "Channel"
-msgstr "Kanál"
-
-#: templates/debug_toolbar/panels/logging.html:9
-msgid "Message"
-msgstr "Správa"
+#: templates/debug_toolbar/panels/history.html:10
+msgid "Method"
+msgstr ""
 
-#: templates/debug_toolbar/panels/logging.html:10 templates/debug_toolbar/panels/staticfiles.html:45
-msgid "Location"
-msgstr "Poloha"
+#: templates/debug_toolbar/panels/history.html:11
+#: templates/debug_toolbar/panels/staticfiles.html:43
+msgid "Path"
+msgstr "Cesta"
+
+#: templates/debug_toolbar/panels/history.html:12
+#, fuzzy
+#| msgid "Request headers"
+msgid "Request Variables"
+msgstr "Hlavičky požiadavky"
+
+#: templates/debug_toolbar/panels/history.html:13
+msgid "Status"
+msgstr ""
+
+#: templates/debug_toolbar/panels/history.html:14
+#: templates/debug_toolbar/panels/sql.html:37
+msgid "Action"
+msgstr "Akcia"
 
-#: templates/debug_toolbar/panels/logging.html:26
-msgid "No messages logged"
-msgstr "Žiadne správy neboli zaznamenané"
+#: templates/debug_toolbar/panels/history_tr.html:22
+#: templates/debug_toolbar/panels/request_variables.html:11
+msgid "Variable"
+msgstr "Premenná"
 
 #: templates/debug_toolbar/panels/profiling.html:5
 msgid "Call"
 msgstr "Volanie"
 
 #: templates/debug_toolbar/panels/profiling.html:6
 msgid "CumTime"
 msgstr "CumTime"
 
-#: templates/debug_toolbar/panels/profiling.html:7 templates/debug_toolbar/panels/profiling.html:9
+#: templates/debug_toolbar/panels/profiling.html:7
+#: templates/debug_toolbar/panels/profiling.html:9
 msgid "Per"
 msgstr "Za"
 
 #: templates/debug_toolbar/panels/profiling.html:8
 msgid "TotTime"
 msgstr "TotTime"
 
@@ -418,118 +439,131 @@
 msgid "URL name"
 msgstr "URL meno"
 
 #: templates/debug_toolbar/panels/request.html:24
 msgid "Cookies"
 msgstr "Cookies"
 
-#: templates/debug_toolbar/panels/request.html:32 templates/debug_toolbar/panels/request.html:58 templates/debug_toolbar/panels/request.html:84
-#: templates/debug_toolbar/panels/request.html:109
-msgid "Variable"
-msgstr "Premenná"
-
-#: templates/debug_toolbar/panels/request.html:46
+#: templates/debug_toolbar/panels/request.html:27
 msgid "No cookies"
 msgstr "Žiadne cookies"
 
-#: templates/debug_toolbar/panels/request.html:50
+#: templates/debug_toolbar/panels/request.html:31
 msgid "Session data"
 msgstr "Dáta relácie"
 
-#: templates/debug_toolbar/panels/request.html:72
+#: templates/debug_toolbar/panels/request.html:34
 msgid "No session data"
 msgstr "Žiadne dáta relácie"
 
-#: templates/debug_toolbar/panels/request.html:76
+#: templates/debug_toolbar/panels/request.html:38
 msgid "GET data"
 msgstr "GET dáta"
 
-#: templates/debug_toolbar/panels/request.html:98
+#: templates/debug_toolbar/panels/request.html:41
 msgid "No GET data"
 msgstr "Žiadne GET dáta"
 
-#: templates/debug_toolbar/panels/request.html:102
+#: templates/debug_toolbar/panels/request.html:45
 msgid "POST data"
 msgstr "POST dáta"
 
-#: templates/debug_toolbar/panels/request.html:123
+#: templates/debug_toolbar/panels/request.html:48
 msgid "No POST data"
 msgstr "Žiadne POST dáta"
 
 #: templates/debug_toolbar/panels/settings.html:5
 msgid "Setting"
 msgstr "Nastavenie"
 
 #: templates/debug_toolbar/panels/signals.html:5
 msgid "Signal"
 msgstr "Signál"
 
 #: templates/debug_toolbar/panels/signals.html:6
-msgid "Providing"
-msgstr "Poskytuje"
-
-#: templates/debug_toolbar/panels/signals.html:7
 msgid "Receivers"
 msgstr "Príjemcovia"
 
-#: templates/debug_toolbar/panels/sql.html:7
+#: templates/debug_toolbar/panels/sql.html:6
 #, python-format
 msgid "%(num)s query"
 msgid_plural "%(num)s queries"
 msgstr[0] "%(num)s dopyt"
 msgstr[1] "%(num)s dopyty"
 msgstr[2] "%(num)s dopytu"
 msgstr[3] "%(num)s dopytov"
 
-#: templates/debug_toolbar/panels/sql.html:18
+#: templates/debug_toolbar/panels/sql.html:8
+#, python-format
+msgid ""
+"including <abbr title=\"Similar queries are queries with the same SQL, but "
+"potentially different parameters.\">%(count)s similar</abbr>"
+msgstr ""
+
+#: templates/debug_toolbar/panels/sql.html:12
+#, python-format
+msgid ""
+"and <abbr title=\"Duplicate queries are identical to each other: they "
+"execute exactly the same SQL and parameters.\">%(dupes)s duplicates</abbr>"
+msgstr ""
+
+#: templates/debug_toolbar/panels/sql.html:34
 msgid "Query"
 msgstr "Dopyt"
 
-#: templates/debug_toolbar/panels/sql.html:19 templates/debug_toolbar/panels/timer.html:36
+#: templates/debug_toolbar/panels/sql.html:35
+#: templates/debug_toolbar/panels/timer.html:36
 msgid "Timeline"
 msgstr "Časová os"
 
-#: templates/debug_toolbar/panels/sql.html:21
-msgid "Action"
-msgstr "Akcia"
+#: templates/debug_toolbar/panels/sql.html:52
+#, fuzzy, python-format
+#| msgid "%(count)s message"
+#| msgid_plural "%(count)s messages"
+msgid "%(count)s similar queries."
+msgstr "%(count)s správa"
+
+#: templates/debug_toolbar/panels/sql.html:58
+#, python-format
+msgid "Duplicated %(dupes)s times."
+msgstr ""
 
-#: templates/debug_toolbar/panels/sql.html:64
+#: templates/debug_toolbar/panels/sql.html:95
 msgid "Connection:"
 msgstr "Pripojenie:"
 
-#: templates/debug_toolbar/panels/sql.html:66
+#: templates/debug_toolbar/panels/sql.html:97
 msgid "Isolation level:"
 msgstr "Úroveň izolácie:"
 
-#: templates/debug_toolbar/panels/sql.html:69
+#: templates/debug_toolbar/panels/sql.html:100
 msgid "Transaction status:"
 msgstr "Stav transakcie:"
 
-#: templates/debug_toolbar/panels/sql.html:83
+#: templates/debug_toolbar/panels/sql.html:114
 msgid "(unknown)"
 msgstr "(neznámy)"
 
-#: templates/debug_toolbar/panels/sql.html:92
+#: templates/debug_toolbar/panels/sql.html:123
 msgid "No SQL queries were recorded during this request."
 msgstr "V priebehu tejto požiadavky neboli zaznamenané žiadne SQL dopyty."
 
-#: templates/debug_toolbar/panels/sql_explain.html:3 templates/debug_toolbar/panels/sql_profile.html:3 templates/debug_toolbar/panels/sql_select.html:3
-#: templates/debug_toolbar/panels/template_source.html:3
-msgid "Back"
-msgstr "Späť"
-
 #: templates/debug_toolbar/panels/sql_explain.html:4
 msgid "SQL explained"
 msgstr "SQL vysvetlené"
 
-#: templates/debug_toolbar/panels/sql_explain.html:9 templates/debug_toolbar/panels/sql_profile.html:10 templates/debug_toolbar/panels/sql_select.html:9
+#: templates/debug_toolbar/panels/sql_explain.html:9
+#: templates/debug_toolbar/panels/sql_profile.html:10
+#: templates/debug_toolbar/panels/sql_select.html:9
 msgid "Executed SQL"
 msgstr "Vykonané SQL"
 
-#: templates/debug_toolbar/panels/sql_explain.html:13 templates/debug_toolbar/panels/sql_profile.html:14 templates/debug_toolbar/panels/sql_select.html:13
+#: templates/debug_toolbar/panels/sql_explain.html:13
+#: templates/debug_toolbar/panels/sql_profile.html:14
+#: templates/debug_toolbar/panels/sql_select.html:13
 msgid "Database"
 msgstr "Databáza"
 
 #: templates/debug_toolbar/panels/sql_profile.html:4
 msgid "SQL profiled"
 msgstr "SQL profilované"
 
@@ -541,60 +575,64 @@
 msgid "SQL selected"
 msgstr "SQL označené"
 
 #: templates/debug_toolbar/panels/sql_select.html:36
 msgid "Empty set"
 msgstr "Prázdny rad"
 
-#: templates/debug_toolbar/panels/staticfiles.html:4
+#: templates/debug_toolbar/panels/staticfiles.html:3
 msgid "Static file path"
 msgid_plural "Static file paths"
 msgstr[0] "Cesta k statickému súboru"
 msgstr[1] "Cesty k statickým súborom"
 msgstr[2] "Cesty k statickým súborom"
 msgstr[3] "Ciest k statickým súborom"
 
-#: templates/debug_toolbar/panels/staticfiles.html:8
+#: templates/debug_toolbar/panels/staticfiles.html:7
 #, python-format
 msgid "(prefix %(prefix)s)"
 msgstr "(prefix %(prefix)s)"
 
-#: templates/debug_toolbar/panels/staticfiles.html:12 templates/debug_toolbar/panels/staticfiles.html:23 templates/debug_toolbar/panels/staticfiles.html:35
-#: templates/debug_toolbar/panels/templates.html:10 templates/debug_toolbar/panels/templates.html:28 templates/debug_toolbar/panels/templates.html:43
+#: templates/debug_toolbar/panels/staticfiles.html:11
+#: templates/debug_toolbar/panels/staticfiles.html:22
+#: templates/debug_toolbar/panels/staticfiles.html:34
+#: templates/debug_toolbar/panels/templates.html:10
+#: templates/debug_toolbar/panels/templates.html:30
+#: templates/debug_toolbar/panels/templates.html:47
 msgid "None"
 msgstr "Žiadny"
 
-#: templates/debug_toolbar/panels/staticfiles.html:15
+#: templates/debug_toolbar/panels/staticfiles.html:14
 msgid "Static file app"
 msgid_plural "Static file apps"
 msgstr[0] "Aplikácia pre statické súbory"
 msgstr[1] "Aplikácie pre statické súbory"
 msgstr[2] "Aplikácie pre statické súbory"
 msgstr[3] "Aplikácií pre statické súbory"
 
-#: templates/debug_toolbar/panels/staticfiles.html:26
+#: templates/debug_toolbar/panels/staticfiles.html:25
 msgid "Static file"
 msgid_plural "Static files"
 msgstr[0] "Statický súbor"
 msgstr[1] "Statické súbory"
 msgstr[2] "Statického súbora"
 msgstr[3] "Statických súborov"
 
-#: templates/debug_toolbar/panels/staticfiles.html:40
+#: templates/debug_toolbar/panels/staticfiles.html:39
 #, python-format
 msgid "%(payload_count)s file"
 msgid_plural "%(payload_count)s files"
 msgstr[0] "%(payload_count)s súbor"
 msgstr[1] "%(payload_count)s súbory"
 msgstr[2] "%(payload_count)s súbora"
 msgstr[3] "%(payload_count)s súborov"
 
 #: templates/debug_toolbar/panels/staticfiles.html:44
-msgid "Path"
-msgstr "Cesta"
+msgid "Location"
+msgstr "Poloha"
 
 #: templates/debug_toolbar/panels/template_source.html:4
 msgid "Template source:"
 msgstr "Zdrojový kód šablóny:"
 
 #: templates/debug_toolbar/panels/templates.html:2
 msgid "Template path"
@@ -608,19 +646,20 @@
 msgid "Template"
 msgid_plural "Templates"
 msgstr[0] "Šablóna"
 msgstr[1] "Šablóny"
 msgstr[2] "Šablóny"
 msgstr[3] "Šablón"
 
-#: templates/debug_toolbar/panels/templates.html:21 templates/debug_toolbar/panels/templates.html:37
+#: templates/debug_toolbar/panels/templates.html:22
+#: templates/debug_toolbar/panels/templates.html:40
 msgid "Toggle context"
 msgstr "Prepnúť kontext"
 
-#: templates/debug_toolbar/panels/templates.html:31
+#: templates/debug_toolbar/panels/templates.html:33
 msgid "Context processor"
 msgid_plural "Context processors"
 msgstr[0] "Spracovateľ kontextu"
 msgstr[1] "Spracovatelia kontextu"
 msgstr[2] "Spracovateľa kontextu"
 msgstr[3] "Spracovateľov kontextu"
 
@@ -640,14 +679,39 @@
 msgid "Timing attribute"
 msgstr "Časový atribút"
 
 #: templates/debug_toolbar/panels/timer.html:37
 msgid "Milliseconds since navigation start (+length)"
 msgstr "Milisekúnd od spustenia navigácie (+dĺžka)"
 
-#: templates/debug_toolbar/panels/versions.html:5
+#: templates/debug_toolbar/panels/versions.html:10
+msgid "Package"
+msgstr ""
+
+#: templates/debug_toolbar/panels/versions.html:11
 msgid "Name"
 msgstr "Meno"
 
-#: templates/debug_toolbar/panels/versions.html:6
+#: templates/debug_toolbar/panels/versions.html:12
 msgid "Version"
 msgstr "Verzia"
+
+#: templates/debug_toolbar/redirect.html:10
+msgid "Location:"
+msgstr "Poloha:"
+
+#: templates/debug_toolbar/redirect.html:12
+msgid ""
+"The Django Debug Toolbar has intercepted a redirect to the above URL for "
+"debug viewing purposes. You can click the above link to continue with the "
+"redirect as normal."
+msgstr ""
+"Django Debug Toolbar zachytil presmerovanie na vyššie uvedenú URL pre účely "
+"ladenia. Pre normálne presmerovanie môžete kliknúť na vyššie uvedený odkaz."
+
+#: views.py:16
+msgid ""
+"Data for this panel isn't available anymore. Please reload the page and "
+"retry."
+msgstr ""
+"Dáta pre tento panel už nie sú k dispozícii. Načítajte si prosím stránku a "
+"skúste to znova."
```

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/locale/sv_SE/LC_MESSAGES/django.mo` & `django_debug_toolbar-4.0.0/debug_toolbar/locale/sv_SE/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/locale/sv_SE/LC_MESSAGES/django.po` & `django_debug_toolbar-4.0.0/debug_toolbar/locale/uk/LC_MESSAGES/django.po`

 * *Files 18% similar despite different names*

```diff
@@ -1,295 +1,290 @@
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 #
 #
 # Translators:
-# Alex Nordlund <deep.alexander@gmail.com>, 2012-2013
-# Alex Nordlund <deep.alexander@gmail.com>, 2012
+# Sergey Lysach <sergikoff88@gmail.com>, 2013
 msgid ""
 msgstr ""
 "Project-Id-Version: Django Debug Toolbar\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2014-04-25 21:52+0200\n"
+"POT-Creation-Date: 2023-01-20 17:23+0100\n"
 "PO-Revision-Date: 2014-04-25 19:53+0000\n"
 "Last-Translator: Aymeric Augustin <aymeric.augustin@m4x.org>\n"
-"Language-Team: Swedish (Sweden) (http://www.transifex.com/projects/p/django-debug-toolbar/language/sv_SE/)\n"
+"Language-Team: Ukrainian (http://www.transifex.com/projects/p/django-debug-"
+"toolbar/language/uk/)\n"
+"Language: uk\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: sv_SE\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
+"n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
 
-#: apps.py:11
+#: apps.py:15
 msgid "Debug Toolbar"
 msgstr ""
 
-#: views.py:14
-msgid ""
-"Data for this panel isn't available anymore. Please reload the page and "
-"retry."
-msgstr ""
-
-#: panels/cache.py:191
+#: panels/cache.py:180
 msgid "Cache"
-msgstr "Cache"
+msgstr "Кеш"
 
-#: panels/cache.py:196
+#: panels/cache.py:186
 #, python-format
 msgid "%(cache_calls)d call in %(time).2fms"
 msgid_plural "%(cache_calls)d calls in %(time).2fms"
 msgstr[0] ""
 msgstr[1] ""
+msgstr[2] ""
 
-#: panels/cache.py:204
+#: panels/cache.py:195
 #, python-format
 msgid "Cache calls from %(count)d backend"
 msgid_plural "Cache calls from %(count)d backends"
 msgstr[0] ""
 msgstr[1] ""
+msgstr[2] ""
 
-#: panels/headers.py:35
+#: panels/headers.py:31
 msgid "Headers"
 msgstr ""
 
-#: panels/logging.py:64
-msgid "Logging"
+#: panels/history/panel.py:18 panels/history/panel.py:19
+msgid "History"
 msgstr ""
 
-#: panels/logging.py:70
-#, python-format
-msgid "%(count)s message"
-msgid_plural "%(count)s messages"
-msgstr[0] "%(count)s meddelande"
-msgstr[1] "%(count)s meddelanden"
-
-#: panels/logging.py:73
-msgid "Log messages"
-msgstr ""
-
-#: panels/profiling.py:127
+#: panels/profiling.py:140
 msgid "Profiling"
-msgstr "Profilering"
+msgstr ""
 
-#: panels/redirects.py:17
+#: panels/redirects.py:14
 msgid "Intercept redirects"
 msgstr ""
 
-#: panels/request.py:18
+#: panels/request.py:16
 msgid "Request"
 msgstr ""
 
-#: panels/request.py:35
+#: panels/request.py:36
 msgid "<no view>"
 msgstr ""
 
-#: panels/request.py:47
+#: panels/request.py:53
 msgid "<unavailable>"
 msgstr ""
 
-#: panels/settings.py:20
+#: panels/settings.py:17
 msgid "Settings"
-msgstr "Inställningar"
+msgstr "Налаштування"
 
-#: panels/settings.py:23
-#, python-format
-msgid "Settings from <code>%s</code>"
-msgstr ""
+#: panels/settings.py:20
+#, fuzzy, python-format
+#| msgid "Settings"
+msgid "Settings from %s"
+msgstr "Налаштування"
 
-#: panels/signals.py:45
+#: panels/signals.py:57
 #, python-format
 msgid "%(num_receivers)d receiver of 1 signal"
 msgid_plural "%(num_receivers)d receivers of 1 signal"
 msgstr[0] ""
 msgstr[1] ""
+msgstr[2] ""
 
-#: panels/signals.py:48
+#: panels/signals.py:62
 #, python-format
 msgid "%(num_receivers)d receiver of %(num_signals)d signals"
 msgid_plural "%(num_receivers)d receivers of %(num_signals)d signals"
 msgstr[0] ""
 msgstr[1] ""
+msgstr[2] ""
 
-#: panels/signals.py:53
+#: panels/signals.py:67
 msgid "Signals"
-msgstr "Signaler"
+msgstr "Сигнали"
+
+#: panels/sql/panel.py:23
+msgid "Autocommit"
+msgstr ""
+
+#: panels/sql/panel.py:24
+msgid "Read uncommitted"
+msgstr ""
+
+#: panels/sql/panel.py:25
+msgid "Read committed"
+msgstr ""
 
-#: panels/staticfiles.py:89
+#: panels/sql/panel.py:26
+msgid "Repeatable read"
+msgstr ""
+
+#: panels/sql/panel.py:27
+msgid "Serializable"
+msgstr ""
+
+#: panels/sql/panel.py:39
+msgid "Idle"
+msgstr ""
+
+#: panels/sql/panel.py:40
+msgid "Active"
+msgstr ""
+
+#: panels/sql/panel.py:41
+msgid "In transaction"
+msgstr ""
+
+#: panels/sql/panel.py:42
+msgid "In error"
+msgstr ""
+
+#: panels/sql/panel.py:43
+msgid "Unknown"
+msgstr ""
+
+#: panels/sql/panel.py:130
+msgid "SQL"
+msgstr ""
+
+#: panels/sql/panel.py:135
+#, python-format
+msgid "%(query_count)d query in %(sql_time).2fms"
+msgid_plural "%(query_count)d queries in %(sql_time).2fms"
+msgstr[0] ""
+msgstr[1] ""
+msgstr[2] ""
+
+#: panels/sql/panel.py:147
+#, python-format
+msgid "SQL queries from %(count)d connection"
+msgid_plural "SQL queries from %(count)d connections"
+msgstr[0] ""
+msgstr[1] ""
+msgstr[2] ""
+
+#: panels/staticfiles.py:84
 #, python-format
 msgid "Static files (%(num_found)s found, %(num_used)s used)"
 msgstr ""
 
-#: panels/staticfiles.py:107
+#: panels/staticfiles.py:105
 msgid "Static files"
-msgstr "Statiska filer"
+msgstr ""
 
-#: panels/staticfiles.py:112
+#: panels/staticfiles.py:111
 #, python-format
 msgid "%(num_used)s file used"
 msgid_plural "%(num_used)s files used"
 msgstr[0] ""
 msgstr[1] ""
+msgstr[2] ""
 
-#: panels/timer.py:23
+#: panels/templates/panel.py:143
+msgid "Templates"
+msgstr "Шаблони"
+
+#: panels/templates/panel.py:148
+#, python-format
+msgid "Templates (%(num_templates)s rendered)"
+msgstr "Шаблони (оброблено %(num_templates)s)"
+
+#: panels/templates/panel.py:180
+msgid "No origin"
+msgstr ""
+
+#: panels/timer.py:25
 #, python-format
 msgid "CPU: %(cum)0.2fms (%(total)0.2fms)"
 msgstr ""
 
-#: panels/timer.py:28
+#: panels/timer.py:30
 #, python-format
 msgid "Total: %0.2fms"
 msgstr ""
 
-#: panels/timer.py:34 templates/debug_toolbar/panels/logging.html:7
+#: panels/timer.py:36 templates/debug_toolbar/panels/history.html:9
 #: templates/debug_toolbar/panels/sql_explain.html:11
 #: templates/debug_toolbar/panels/sql_profile.html:12
 #: templates/debug_toolbar/panels/sql_select.html:11
 msgid "Time"
-msgstr "Tid"
+msgstr "Час"
 
-#: panels/timer.py:42
+#: panels/timer.py:44
 msgid "User CPU time"
 msgstr ""
 
-#: panels/timer.py:42
+#: panels/timer.py:44
 #, python-format
 msgid "%(utime)0.3f msec"
 msgstr ""
 
-#: panels/timer.py:43
+#: panels/timer.py:45
 msgid "System CPU time"
 msgstr ""
 
-#: panels/timer.py:43
+#: panels/timer.py:45
 #, python-format
 msgid "%(stime)0.3f msec"
 msgstr ""
 
-#: panels/timer.py:44
+#: panels/timer.py:46
 msgid "Total CPU time"
 msgstr ""
 
-#: panels/timer.py:44
+#: panels/timer.py:46
 #, python-format
 msgid "%(total)0.3f msec"
 msgstr ""
 
-#: panels/timer.py:45
+#: panels/timer.py:47
 msgid "Elapsed time"
 msgstr ""
 
-#: panels/timer.py:45
+#: panels/timer.py:47
 #, python-format
 msgid "%(total_time)0.3f msec"
 msgstr ""
 
-#: panels/timer.py:46
+#: panels/timer.py:49
 msgid "Context switches"
 msgstr ""
 
-#: panels/timer.py:46
+#: panels/timer.py:50
 #, python-format
 msgid "%(vcsw)d voluntary, %(ivcsw)d involuntary"
 msgstr ""
 
-#: panels/versions.py:25
+#: panels/versions.py:19
 msgid "Versions"
-msgstr "Versioner"
-
-#: panels/sql/panel.py:22
-msgid "Autocommit"
-msgstr ""
-
-#: panels/sql/panel.py:23
-msgid "Read uncommitted"
-msgstr ""
-
-#: panels/sql/panel.py:24
-msgid "Read committed"
-msgstr ""
+msgstr "Версії"
 
-#: panels/sql/panel.py:25
-msgid "Repeatable read"
-msgstr ""
-
-#: panels/sql/panel.py:26
-msgid "Serializable"
-msgstr "Variabel"
-
-#: panels/sql/panel.py:37
-msgid "Idle"
-msgstr ""
-
-#: panels/sql/panel.py:38
-msgid "Active"
-msgstr "Åtgärd"
-
-#: panels/sql/panel.py:39
-msgid "In transaction"
-msgstr ""
-
-#: panels/sql/panel.py:40
-msgid "In error"
-msgstr "Felmeddelande"
-
-#: panels/sql/panel.py:41
-msgid "Unknown"
-msgstr "(okänd)"
-
-#: panels/sql/panel.py:105
-msgid "SQL"
-msgstr "SQL"
-
-#: panels/templates/panel.py:141
-msgid "Templates"
-msgstr "Mallar"
-
-#: panels/templates/panel.py:146
-#, python-format
-msgid "Templates (%(num_templates)s rendered)"
-msgstr ""
-
-#: templates/debug_toolbar/base.html:19
+#: templates/debug_toolbar/base.html:22
 msgid "Hide toolbar"
 msgstr ""
 
-#: templates/debug_toolbar/base.html:19
+#: templates/debug_toolbar/base.html:22
 msgid "Hide"
-msgstr "Dölj"
+msgstr "Сховати"
 
-#: templates/debug_toolbar/base.html:25
-msgid "Disable for next and successive requests"
-msgstr ""
-
-#: templates/debug_toolbar/base.html:25
-msgid "Enable for next and successive requests"
-msgstr ""
-
-#: templates/debug_toolbar/base.html:47
+#: templates/debug_toolbar/base.html:29
 msgid "Show toolbar"
 msgstr ""
 
-#: templates/debug_toolbar/base.html:53
-msgid "Close"
-msgstr "Stäng"
-
-#: templates/debug_toolbar/redirect.html:8
-msgid "Location:"
+#: templates/debug_toolbar/includes/panel_button.html:4
+msgid "Disable for next and successive requests"
 msgstr ""
 
-#: templates/debug_toolbar/redirect.html:10
-msgid ""
-"The Django Debug Toolbar has intercepted a redirect to the above URL for "
-"debug viewing purposes. You can click the above link to continue with the "
-"redirect as normal."
+#: templates/debug_toolbar/includes/panel_button.html:4
+msgid "Enable for next and successive requests"
 msgstr ""
 
 #: templates/debug_toolbar/panels/cache.html:2
 msgid "Summary"
-msgstr "Sammanfattning"
+msgstr ""
 
 #: templates/debug_toolbar/panels/cache.html:6
 msgid "Total calls"
 msgstr ""
 
 #: templates/debug_toolbar/panels/cache.html:7
 msgid "Total time"
@@ -308,21 +303,21 @@
 msgstr ""
 
 #: templates/debug_toolbar/panels/cache.html:39
 msgid "Calls"
 msgstr ""
 
 #: templates/debug_toolbar/panels/cache.html:43
-#: templates/debug_toolbar/panels/sql.html:20
+#: templates/debug_toolbar/panels/sql.html:36
 msgid "Time (ms)"
-msgstr "Tid (ms)"
+msgstr "Час (мс)"
 
 #: templates/debug_toolbar/panels/cache.html:44
 msgid "Type"
-msgstr ""
+msgstr "Тип"
 
 #: templates/debug_toolbar/panels/cache.html:45
 #: templates/debug_toolbar/panels/request.html:8
 msgid "Arguments"
 msgstr ""
 
 #: templates/debug_toolbar/panels/cache.html:46
@@ -338,27 +333,25 @@
 msgid "Request headers"
 msgstr ""
 
 #: templates/debug_toolbar/panels/headers.html:8
 #: templates/debug_toolbar/panels/headers.html:27
 #: templates/debug_toolbar/panels/headers.html:48
 msgid "Key"
-msgstr "Nyckel"
+msgstr "Ключ"
 
 #: templates/debug_toolbar/panels/headers.html:9
 #: templates/debug_toolbar/panels/headers.html:28
 #: templates/debug_toolbar/panels/headers.html:49
-#: templates/debug_toolbar/panels/request.html:33
-#: templates/debug_toolbar/panels/request.html:59
-#: templates/debug_toolbar/panels/request.html:85
-#: templates/debug_toolbar/panels/request.html:110
+#: templates/debug_toolbar/panels/history_tr.html:23
+#: templates/debug_toolbar/panels/request_variables.html:12
 #: templates/debug_toolbar/panels/settings.html:6
 #: templates/debug_toolbar/panels/timer.html:11
 msgid "Value"
-msgstr "Värde"
+msgstr "Значення"
 
 #: templates/debug_toolbar/panels/headers.html:22
 msgid "Response headers"
 msgstr ""
 
 #: templates/debug_toolbar/panels/headers.html:41
 msgid "WSGI environ"
@@ -366,35 +359,43 @@
 
 #: templates/debug_toolbar/panels/headers.html:43
 msgid ""
 "Since the WSGI environ inherits the environment of the server, only a "
 "significant subset is shown below."
 msgstr ""
 
-#: templates/debug_toolbar/panels/logging.html:6
-msgid "Level"
-msgstr "Nivå"
-
-#: templates/debug_toolbar/panels/logging.html:8
-msgid "Channel"
+#: templates/debug_toolbar/panels/history.html:10
+msgid "Method"
 msgstr ""
 
-#: templates/debug_toolbar/panels/logging.html:9
-msgid "Message"
-msgstr "Meddelande"
+#: templates/debug_toolbar/panels/history.html:11
+#: templates/debug_toolbar/panels/staticfiles.html:43
+msgid "Path"
+msgstr ""
 
-#: templates/debug_toolbar/panels/logging.html:10
-#: templates/debug_toolbar/panels/staticfiles.html:45
-msgid "Location"
-msgstr "Plats"
+#: templates/debug_toolbar/panels/history.html:12
+#, fuzzy
+#| msgid "Variable"
+msgid "Request Variables"
+msgstr "Змінна"
 
-#: templates/debug_toolbar/panels/logging.html:26
-msgid "No messages logged"
+#: templates/debug_toolbar/panels/history.html:13
+msgid "Status"
 msgstr ""
 
+#: templates/debug_toolbar/panels/history.html:14
+#: templates/debug_toolbar/panels/sql.html:37
+msgid "Action"
+msgstr "Подія"
+
+#: templates/debug_toolbar/panels/history_tr.html:22
+#: templates/debug_toolbar/panels/request_variables.html:11
+msgid "Variable"
+msgstr "Змінна"
+
 #: templates/debug_toolbar/panels/profiling.html:5
 msgid "Call"
 msgstr ""
 
 #: templates/debug_toolbar/panels/profiling.html:6
 msgid "CumTime"
 msgstr ""
@@ -406,252 +407,283 @@
 
 #: templates/debug_toolbar/panels/profiling.html:8
 msgid "TotTime"
 msgstr ""
 
 #: templates/debug_toolbar/panels/profiling.html:10
 msgid "Count"
-msgstr "Räkna"
+msgstr ""
 
 #: templates/debug_toolbar/panels/request.html:3
 msgid "View information"
-msgstr "Visa informationen"
+msgstr ""
 
 #: templates/debug_toolbar/panels/request.html:7
 msgid "View function"
 msgstr ""
 
 #: templates/debug_toolbar/panels/request.html:10
 msgid "URL name"
 msgstr ""
 
 #: templates/debug_toolbar/panels/request.html:24
 msgid "Cookies"
 msgstr ""
 
-#: templates/debug_toolbar/panels/request.html:32
-#: templates/debug_toolbar/panels/request.html:58
-#: templates/debug_toolbar/panels/request.html:84
-#: templates/debug_toolbar/panels/request.html:109
-msgid "Variable"
-msgstr "Variabel"
-
-#: templates/debug_toolbar/panels/request.html:46
+#: templates/debug_toolbar/panels/request.html:27
 msgid "No cookies"
 msgstr ""
 
-#: templates/debug_toolbar/panels/request.html:50
+#: templates/debug_toolbar/panels/request.html:31
 msgid "Session data"
 msgstr ""
 
-#: templates/debug_toolbar/panels/request.html:72
+#: templates/debug_toolbar/panels/request.html:34
 msgid "No session data"
 msgstr ""
 
-#: templates/debug_toolbar/panels/request.html:76
+#: templates/debug_toolbar/panels/request.html:38
 msgid "GET data"
 msgstr ""
 
-#: templates/debug_toolbar/panels/request.html:98
+#: templates/debug_toolbar/panels/request.html:41
 msgid "No GET data"
-msgstr "Ingen GET data"
+msgstr "Немає GET даних"
 
-#: templates/debug_toolbar/panels/request.html:102
+#: templates/debug_toolbar/panels/request.html:45
 msgid "POST data"
 msgstr ""
 
-#: templates/debug_toolbar/panels/request.html:123
+#: templates/debug_toolbar/panels/request.html:48
 msgid "No POST data"
-msgstr "Ingen POST data"
+msgstr "Немає POST даних"
 
 #: templates/debug_toolbar/panels/settings.html:5
 msgid "Setting"
-msgstr "Inställning"
+msgstr ""
 
 #: templates/debug_toolbar/panels/signals.html:5
 msgid "Signal"
-msgstr "Signal"
+msgstr "Сигнал"
 
 #: templates/debug_toolbar/panels/signals.html:6
-msgid "Providing"
-msgstr ""
-
-#: templates/debug_toolbar/panels/signals.html:7
 msgid "Receivers"
-msgstr "Mottagare"
+msgstr "Отримувачі сигнала"
 
-#: templates/debug_toolbar/panels/sql.html:7
+#: templates/debug_toolbar/panels/sql.html:6
 #, python-format
 msgid "%(num)s query"
 msgid_plural "%(num)s queries"
 msgstr[0] ""
 msgstr[1] ""
+msgstr[2] ""
 
-#: templates/debug_toolbar/panels/sql.html:18
+#: templates/debug_toolbar/panels/sql.html:8
+#, python-format
+msgid ""
+"including <abbr title=\"Similar queries are queries with the same SQL, but "
+"potentially different parameters.\">%(count)s similar</abbr>"
+msgstr ""
+
+#: templates/debug_toolbar/panels/sql.html:12
+#, python-format
+msgid ""
+"and <abbr title=\"Duplicate queries are identical to each other: they "
+"execute exactly the same SQL and parameters.\">%(dupes)s duplicates</abbr>"
+msgstr ""
+
+#: templates/debug_toolbar/panels/sql.html:34
 msgid "Query"
-msgstr "Fråga"
+msgstr "Запит"
 
-#: templates/debug_toolbar/panels/sql.html:19
+#: templates/debug_toolbar/panels/sql.html:35
 #: templates/debug_toolbar/panels/timer.html:36
 msgid "Timeline"
 msgstr ""
 
-#: templates/debug_toolbar/panels/sql.html:21
-msgid "Action"
-msgstr "Åtgärd"
+#: templates/debug_toolbar/panels/sql.html:52
+#, python-format
+msgid "%(count)s similar queries."
+msgstr ""
+
+#: templates/debug_toolbar/panels/sql.html:58
+#, python-format
+msgid "Duplicated %(dupes)s times."
+msgstr ""
 
-#: templates/debug_toolbar/panels/sql.html:64
+#: templates/debug_toolbar/panels/sql.html:95
 msgid "Connection:"
-msgstr "Anslutning:"
+msgstr ""
 
-#: templates/debug_toolbar/panels/sql.html:66
+#: templates/debug_toolbar/panels/sql.html:97
 msgid "Isolation level:"
 msgstr ""
 
-#: templates/debug_toolbar/panels/sql.html:69
+#: templates/debug_toolbar/panels/sql.html:100
 msgid "Transaction status:"
 msgstr ""
 
-#: templates/debug_toolbar/panels/sql.html:83
+#: templates/debug_toolbar/panels/sql.html:114
 msgid "(unknown)"
-msgstr "(okänd)"
+msgstr ""
 
-#: templates/debug_toolbar/panels/sql.html:92
+#: templates/debug_toolbar/panels/sql.html:123
 msgid "No SQL queries were recorded during this request."
 msgstr ""
 
-#: templates/debug_toolbar/panels/sql_explain.html:3
-#: templates/debug_toolbar/panels/sql_profile.html:3
-#: templates/debug_toolbar/panels/sql_select.html:3
-#: templates/debug_toolbar/panels/template_source.html:3
-msgid "Back"
-msgstr "Bakåt"
-
 #: templates/debug_toolbar/panels/sql_explain.html:4
 msgid "SQL explained"
 msgstr ""
 
 #: templates/debug_toolbar/panels/sql_explain.html:9
 #: templates/debug_toolbar/panels/sql_profile.html:10
 #: templates/debug_toolbar/panels/sql_select.html:9
 msgid "Executed SQL"
-msgstr "Utförd SQL"
+msgstr ""
 
 #: templates/debug_toolbar/panels/sql_explain.html:13
 #: templates/debug_toolbar/panels/sql_profile.html:14
 #: templates/debug_toolbar/panels/sql_select.html:13
 msgid "Database"
-msgstr "Databas"
+msgstr "База даних"
 
 #: templates/debug_toolbar/panels/sql_profile.html:4
 msgid "SQL profiled"
 msgstr ""
 
 #: templates/debug_toolbar/panels/sql_profile.html:37
 msgid "Error"
-msgstr "Felmeddelande"
+msgstr "Помилка"
 
 #: templates/debug_toolbar/panels/sql_select.html:4
 msgid "SQL selected"
 msgstr ""
 
 #: templates/debug_toolbar/panels/sql_select.html:36
 msgid "Empty set"
-msgstr "Tomt set"
+msgstr ""
 
-#: templates/debug_toolbar/panels/staticfiles.html:4
+#: templates/debug_toolbar/panels/staticfiles.html:3
 msgid "Static file path"
 msgid_plural "Static file paths"
 msgstr[0] ""
 msgstr[1] ""
+msgstr[2] ""
 
-#: templates/debug_toolbar/panels/staticfiles.html:8
+#: templates/debug_toolbar/panels/staticfiles.html:7
 #, python-format
 msgid "(prefix %(prefix)s)"
 msgstr ""
 
-#: templates/debug_toolbar/panels/staticfiles.html:12
-#: templates/debug_toolbar/panels/staticfiles.html:23
-#: templates/debug_toolbar/panels/staticfiles.html:35
+#: templates/debug_toolbar/panels/staticfiles.html:11
+#: templates/debug_toolbar/panels/staticfiles.html:22
+#: templates/debug_toolbar/panels/staticfiles.html:34
 #: templates/debug_toolbar/panels/templates.html:10
-#: templates/debug_toolbar/panels/templates.html:28
-#: templates/debug_toolbar/panels/templates.html:43
+#: templates/debug_toolbar/panels/templates.html:30
+#: templates/debug_toolbar/panels/templates.html:47
 msgid "None"
-msgstr "Inget"
+msgstr ""
 
-#: templates/debug_toolbar/panels/staticfiles.html:15
+#: templates/debug_toolbar/panels/staticfiles.html:14
 msgid "Static file app"
 msgid_plural "Static file apps"
 msgstr[0] ""
 msgstr[1] ""
+msgstr[2] ""
 
-#: templates/debug_toolbar/panels/staticfiles.html:26
+#: templates/debug_toolbar/panels/staticfiles.html:25
 msgid "Static file"
 msgid_plural "Static files"
 msgstr[0] ""
-msgstr[1] "Statiska filer"
+msgstr[1] ""
+msgstr[2] ""
 
-#: templates/debug_toolbar/panels/staticfiles.html:40
+#: templates/debug_toolbar/panels/staticfiles.html:39
 #, python-format
 msgid "%(payload_count)s file"
 msgid_plural "%(payload_count)s files"
 msgstr[0] ""
 msgstr[1] ""
+msgstr[2] ""
 
 #: templates/debug_toolbar/panels/staticfiles.html:44
-msgid "Path"
-msgstr "Sökväg"
+msgid "Location"
+msgstr "Місце"
 
 #: templates/debug_toolbar/panels/template_source.html:4
 msgid "Template source:"
 msgstr ""
 
 #: templates/debug_toolbar/panels/templates.html:2
 msgid "Template path"
 msgid_plural "Template paths"
 msgstr[0] ""
 msgstr[1] ""
+msgstr[2] ""
 
 #: templates/debug_toolbar/panels/templates.html:13
 msgid "Template"
 msgid_plural "Templates"
-msgstr[0] "Mall"
-msgstr[1] "Mallar"
+msgstr[0] "Шаблон"
+msgstr[1] "Шаблони"
+msgstr[2] "Шаблонів"
 
-#: templates/debug_toolbar/panels/templates.html:21
-#: templates/debug_toolbar/panels/templates.html:37
+#: templates/debug_toolbar/panels/templates.html:22
+#: templates/debug_toolbar/panels/templates.html:40
 msgid "Toggle context"
 msgstr ""
 
-#: templates/debug_toolbar/panels/templates.html:31
+#: templates/debug_toolbar/panels/templates.html:33
 msgid "Context processor"
 msgid_plural "Context processors"
 msgstr[0] ""
 msgstr[1] ""
+msgstr[2] ""
 
 #: templates/debug_toolbar/panels/timer.html:2
 msgid "Resource usage"
 msgstr ""
 
 #: templates/debug_toolbar/panels/timer.html:10
 msgid "Resource"
-msgstr "Resurs"
+msgstr ""
 
 #: templates/debug_toolbar/panels/timer.html:26
 msgid "Browser timing"
 msgstr ""
 
 #: templates/debug_toolbar/panels/timer.html:35
 msgid "Timing attribute"
 msgstr ""
 
 #: templates/debug_toolbar/panels/timer.html:37
 msgid "Milliseconds since navigation start (+length)"
 msgstr ""
 
-#: templates/debug_toolbar/panels/versions.html:5
+#: templates/debug_toolbar/panels/versions.html:10
+msgid "Package"
+msgstr ""
+
+#: templates/debug_toolbar/panels/versions.html:11
 msgid "Name"
-msgstr "Namn"
+msgstr ""
 
-#: templates/debug_toolbar/panels/versions.html:6
+#: templates/debug_toolbar/panels/versions.html:12
 msgid "Version"
-msgstr "Version"
+msgstr "Версія"
+
+#: templates/debug_toolbar/redirect.html:10
+msgid "Location:"
+msgstr ""
+
+#: templates/debug_toolbar/redirect.html:12
+msgid ""
+"The Django Debug Toolbar has intercepted a redirect to the above URL for "
+"debug viewing purposes. You can click the above link to continue with the "
+"redirect as normal."
+msgstr ""
+
+#: views.py:16
+msgid ""
+"Data for this panel isn't available anymore. Please reload the page and "
+"retry."
+msgstr ""
```

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/locale/uk/LC_MESSAGES/django.mo` & `django_debug_toolbar-4.0.0/debug_toolbar/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/locale/uk/LC_MESSAGES/django.po` & `django_debug_toolbar-4.0.0/debug_toolbar/locale/it/LC_MESSAGES/django.po`

 * *Files 24% similar despite different names*

```diff
@@ -1,670 +1,679 @@
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 #
 #
 # Translators:
-# Sergey Lysach <sergikoff88@gmail.com>, 2013
+# Dario Agliottone <dario.agliottone@gmail.com>, 2012
+# Flavio Curella <flavio.curella@gmail.com>, 2013
+# yakky <i.spalletti@nephila.it>, 2013-2014
 msgid ""
 msgstr ""
 "Project-Id-Version: Django Debug Toolbar\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2014-04-25 21:52+0200\n"
-"PO-Revision-Date: 2014-04-25 19:53+0000\n"
-"Last-Translator: Aymeric Augustin <aymeric.augustin@m4x.org>\n"
-"Language-Team: Ukrainian (http://www.transifex.com/projects/p/django-debug-toolbar/language/uk/)\n"
+"POT-Creation-Date: 2023-01-20 17:23+0100\n"
+"PO-Revision-Date: 2021-08-14 15:25+0000\n"
+"Last-Translator: Tim Schilling\n"
+"Language-Team: Italian (http://www.transifex.com/django-debug-toolbar/django-"
+"debug-toolbar/language/it/)\n"
+"Language: it\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: uk\n"
-"Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: apps.py:11
+#: apps.py:15
 msgid "Debug Toolbar"
 msgstr ""
 
-#: views.py:14
-msgid ""
-"Data for this panel isn't available anymore. Please reload the page and "
-"retry."
-msgstr ""
-
-#: panels/cache.py:191
+#: panels/cache.py:180
 msgid "Cache"
-msgstr "Кеш"
+msgstr "Cache"
 
-#: panels/cache.py:196
+#: panels/cache.py:186
 #, python-format
 msgid "%(cache_calls)d call in %(time).2fms"
 msgid_plural "%(cache_calls)d calls in %(time).2fms"
-msgstr[0] ""
-msgstr[1] ""
-msgstr[2] ""
+msgstr[0] "%(cache_calls)d chiamata in %(time).2fms"
+msgstr[1] "%(cache_calls)d chiamate in %(time).2fms"
 
-#: panels/cache.py:204
+#: panels/cache.py:195
 #, python-format
 msgid "Cache calls from %(count)d backend"
 msgid_plural "Cache calls from %(count)d backends"
-msgstr[0] ""
-msgstr[1] ""
-msgstr[2] ""
+msgstr[0] "Chiamate alla cache da %(count)d backend"
+msgstr[1] "Chiamate alla cache da %(count)d backend"
 
-#: panels/headers.py:35
+#: panels/headers.py:31
 msgid "Headers"
-msgstr ""
-
-#: panels/logging.py:64
-msgid "Logging"
-msgstr "Логи"
-
-#: panels/logging.py:70
-#, python-format
-msgid "%(count)s message"
-msgid_plural "%(count)s messages"
-msgstr[0] ""
-msgstr[1] ""
-msgstr[2] ""
+msgstr "Intestazioni"
 
-#: panels/logging.py:73
-msgid "Log messages"
+#: panels/history/panel.py:18 panels/history/panel.py:19
+msgid "History"
 msgstr ""
 
-#: panels/profiling.py:127
+#: panels/profiling.py:140
 msgid "Profiling"
-msgstr ""
+msgstr "Profilazione"
 
-#: panels/redirects.py:17
+#: panels/redirects.py:14
 msgid "Intercept redirects"
-msgstr ""
+msgstr "Intercetta ridirezioni"
 
-#: panels/request.py:18
+#: panels/request.py:16
 msgid "Request"
-msgstr ""
+msgstr "Request"
 
-#: panels/request.py:35
+#: panels/request.py:36
 msgid "<no view>"
-msgstr ""
+msgstr "<nessuna view>"
 
-#: panels/request.py:47
+#: panels/request.py:53
 msgid "<unavailable>"
-msgstr ""
+msgstr "<non disponibile>"
 
-#: panels/settings.py:20
+#: panels/settings.py:17
 msgid "Settings"
-msgstr "Налаштування"
+msgstr "Impostazioni"
 
-#: panels/settings.py:23
+#: panels/settings.py:20
 #, python-format
-msgid "Settings from <code>%s</code>"
+msgid "Settings from %s"
 msgstr ""
 
-#: panels/signals.py:45
+#: panels/signals.py:57
 #, python-format
 msgid "%(num_receivers)d receiver of 1 signal"
 msgid_plural "%(num_receivers)d receivers of 1 signal"
-msgstr[0] ""
-msgstr[1] ""
-msgstr[2] ""
+msgstr[0] "%(num_receivers)d ricevitore di 1 segnale"
+msgstr[1] "%(num_receivers)d ricevitori di 1 segnale"
 
-#: panels/signals.py:48
+#: panels/signals.py:62
 #, python-format
 msgid "%(num_receivers)d receiver of %(num_signals)d signals"
 msgid_plural "%(num_receivers)d receivers of %(num_signals)d signals"
+msgstr[0] "%(num_receivers)d ricevitore di %(num_signals)d segnali"
+msgstr[1] "%(num_receivers)d ricevitori di %(num_signals)d segnali"
+
+#: panels/signals.py:67
+msgid "Signals"
+msgstr "Segnali"
+
+#: panels/sql/panel.py:23
+msgid "Autocommit"
+msgstr "Autocommit"
+
+#: panels/sql/panel.py:24
+msgid "Read uncommitted"
+msgstr "Read uncommitted"
+
+#: panels/sql/panel.py:25
+msgid "Read committed"
+msgstr "Read committed"
+
+#: panels/sql/panel.py:26
+msgid "Repeatable read"
+msgstr "Repeatable read"
+
+#: panels/sql/panel.py:27
+msgid "Serializable"
+msgstr "Serializable"
+
+#: panels/sql/panel.py:39
+msgid "Idle"
+msgstr "Idle"
+
+#: panels/sql/panel.py:40
+msgid "Active"
+msgstr "Azione"
+
+#: panels/sql/panel.py:41
+msgid "In transaction"
+msgstr "Stato transazione:"
+
+#: panels/sql/panel.py:42
+msgid "In error"
+msgstr "Errore"
+
+#: panels/sql/panel.py:43
+msgid "Unknown"
+msgstr "(sconosciuto)"
+
+#: panels/sql/panel.py:130
+msgid "SQL"
+msgstr "SQL"
+
+#: panels/sql/panel.py:135
+#, python-format
+msgid "%(query_count)d query in %(sql_time).2fms"
+msgid_plural "%(query_count)d queries in %(sql_time).2fms"
 msgstr[0] ""
 msgstr[1] ""
-msgstr[2] ""
 
-#: panels/signals.py:53
-msgid "Signals"
-msgstr "Сигнали"
+#: panels/sql/panel.py:147
+#, python-format
+msgid "SQL queries from %(count)d connection"
+msgid_plural "SQL queries from %(count)d connections"
+msgstr[0] ""
+msgstr[1] ""
 
-#: panels/staticfiles.py:89
+#: panels/staticfiles.py:84
 #, python-format
 msgid "Static files (%(num_found)s found, %(num_used)s used)"
-msgstr ""
+msgstr "File statici (%(num_found)s trovati, %(num_used)s usati)"
 
-#: panels/staticfiles.py:107
+#: panels/staticfiles.py:105
 msgid "Static files"
-msgstr ""
+msgstr "Files statici"
 
-#: panels/staticfiles.py:112
+#: panels/staticfiles.py:111
 #, python-format
 msgid "%(num_used)s file used"
 msgid_plural "%(num_used)s files used"
-msgstr[0] ""
-msgstr[1] ""
-msgstr[2] ""
+msgstr[0] "%(num_used)s file usato"
+msgstr[1] "%(num_used)s file usati"
+
+#: panels/templates/panel.py:143
+msgid "Templates"
+msgstr "Template"
 
-#: panels/timer.py:23
+#: panels/templates/panel.py:148
 #, python-format
-msgid "CPU: %(cum)0.2fms (%(total)0.2fms)"
+msgid "Templates (%(num_templates)s rendered)"
+msgstr "Templates (%(num_templates)s rendered)"
+
+#: panels/templates/panel.py:180
+msgid "No origin"
 msgstr ""
 
-#: panels/timer.py:28
+#: panels/timer.py:25
+#, python-format
+msgid "CPU: %(cum)0.2fms (%(total)0.2fms)"
+msgstr "CPU: %(cum)0.2fms (%(total)0.2fms)"
+
+#: panels/timer.py:30
 #, python-format
 msgid "Total: %0.2fms"
-msgstr ""
+msgstr "Totale: %0.2fms"
 
-#: panels/timer.py:34 templates/debug_toolbar/panels/logging.html:7
+#: panels/timer.py:36 templates/debug_toolbar/panels/history.html:9
 #: templates/debug_toolbar/panels/sql_explain.html:11
 #: templates/debug_toolbar/panels/sql_profile.html:12
 #: templates/debug_toolbar/panels/sql_select.html:11
 msgid "Time"
-msgstr "Час"
+msgstr "Tempo"
 
-#: panels/timer.py:42
+#: panels/timer.py:44
 msgid "User CPU time"
-msgstr ""
+msgstr "Tempo CPU utente"
 
-#: panels/timer.py:42
+#: panels/timer.py:44
 #, python-format
 msgid "%(utime)0.3f msec"
-msgstr ""
+msgstr "%(utime)0.3f msec"
 
-#: panels/timer.py:43
+#: panels/timer.py:45
 msgid "System CPU time"
-msgstr ""
+msgstr "Tempo CPU sistema"
 
-#: panels/timer.py:43
+#: panels/timer.py:45
 #, python-format
 msgid "%(stime)0.3f msec"
-msgstr ""
+msgstr "%(stime)0.3f msec"
 
-#: panels/timer.py:44
+#: panels/timer.py:46
 msgid "Total CPU time"
-msgstr ""
+msgstr "Tempo Totale CPU"
 
-#: panels/timer.py:44
+#: panels/timer.py:46
 #, python-format
 msgid "%(total)0.3f msec"
-msgstr ""
+msgstr "%(total)0.3f msec"
 
-#: panels/timer.py:45
+#: panels/timer.py:47
 msgid "Elapsed time"
-msgstr ""
+msgstr "Tempo Trascorso"
 
-#: panels/timer.py:45
+#: panels/timer.py:47
 #, python-format
 msgid "%(total_time)0.3f msec"
-msgstr ""
+msgstr "%(total_time)0.3f msec"
 
-#: panels/timer.py:46
+#: panels/timer.py:49
 msgid "Context switches"
-msgstr ""
+msgstr "Cambi di contesto"
 
-#: panels/timer.py:46
+#: panels/timer.py:50
 #, python-format
 msgid "%(vcsw)d voluntary, %(ivcsw)d involuntary"
-msgstr ""
+msgstr "%(vcsw)d volontario, %(ivcsw)d involontario"
 
-#: panels/versions.py:25
+#: panels/versions.py:19
 msgid "Versions"
-msgstr "Версії"
-
-#: panels/sql/panel.py:22
-msgid "Autocommit"
-msgstr ""
-
-#: panels/sql/panel.py:23
-msgid "Read uncommitted"
-msgstr ""
-
-#: panels/sql/panel.py:24
-msgid "Read committed"
-msgstr ""
-
-#: panels/sql/panel.py:25
-msgid "Repeatable read"
-msgstr ""
-
-#: panels/sql/panel.py:26
-msgid "Serializable"
-msgstr ""
-
-#: panels/sql/panel.py:37
-msgid "Idle"
-msgstr ""
-
-#: panels/sql/panel.py:38
-msgid "Active"
-msgstr ""
-
-#: panels/sql/panel.py:39
-msgid "In transaction"
-msgstr ""
-
-#: panels/sql/panel.py:40
-msgid "In error"
-msgstr ""
-
-#: panels/sql/panel.py:41
-msgid "Unknown"
-msgstr ""
-
-#: panels/sql/panel.py:105
-msgid "SQL"
-msgstr ""
-
-#: panels/templates/panel.py:141
-msgid "Templates"
-msgstr "Шаблони"
-
-#: panels/templates/panel.py:146
-#, python-format
-msgid "Templates (%(num_templates)s rendered)"
-msgstr "Шаблони (оброблено %(num_templates)s)"
+msgstr "Versioni"
 
-#: templates/debug_toolbar/base.html:19
+#: templates/debug_toolbar/base.html:22
 msgid "Hide toolbar"
-msgstr ""
+msgstr "Nascondi Toolbar"
 
-#: templates/debug_toolbar/base.html:19
+#: templates/debug_toolbar/base.html:22
 msgid "Hide"
-msgstr "Сховати"
-
-#: templates/debug_toolbar/base.html:25
-msgid "Disable for next and successive requests"
-msgstr ""
+msgstr "Nascondi"
 
-#: templates/debug_toolbar/base.html:25
-msgid "Enable for next and successive requests"
-msgstr ""
-
-#: templates/debug_toolbar/base.html:47
+#: templates/debug_toolbar/base.html:29
 msgid "Show toolbar"
-msgstr ""
+msgstr "Mostra Toolbar"
 
-#: templates/debug_toolbar/base.html:53
-msgid "Close"
-msgstr "Закрити"
-
-#: templates/debug_toolbar/redirect.html:8
-msgid "Location:"
-msgstr ""
+#: templates/debug_toolbar/includes/panel_button.html:4
+msgid "Disable for next and successive requests"
+msgstr "Disattiva per la prossima requests e le successive"
 
-#: templates/debug_toolbar/redirect.html:10
-msgid ""
-"The Django Debug Toolbar has intercepted a redirect to the above URL for "
-"debug viewing purposes. You can click the above link to continue with the "
-"redirect as normal."
-msgstr ""
+#: templates/debug_toolbar/includes/panel_button.html:4
+msgid "Enable for next and successive requests"
+msgstr "Abilita per la prossima requests e le successive"
 
 #: templates/debug_toolbar/panels/cache.html:2
 msgid "Summary"
-msgstr ""
+msgstr "Sommario"
 
 #: templates/debug_toolbar/panels/cache.html:6
 msgid "Total calls"
-msgstr ""
+msgstr "Chiamate totali"
 
 #: templates/debug_toolbar/panels/cache.html:7
 msgid "Total time"
-msgstr ""
+msgstr "Tempo Totale"
 
 #: templates/debug_toolbar/panels/cache.html:8
 msgid "Cache hits"
-msgstr ""
+msgstr "Trovati in cache"
 
 #: templates/debug_toolbar/panels/cache.html:9
 msgid "Cache misses"
-msgstr ""
+msgstr "Non trovati in cache"
 
 #: templates/debug_toolbar/panels/cache.html:21
 msgid "Commands"
-msgstr ""
+msgstr "Comandi"
 
 #: templates/debug_toolbar/panels/cache.html:39
 msgid "Calls"
-msgstr ""
+msgstr "Chiamate"
 
 #: templates/debug_toolbar/panels/cache.html:43
-#: templates/debug_toolbar/panels/sql.html:20
+#: templates/debug_toolbar/panels/sql.html:36
 msgid "Time (ms)"
-msgstr "Час (мс)"
+msgstr "Durata (ms)"
 
 #: templates/debug_toolbar/panels/cache.html:44
 msgid "Type"
-msgstr "Тип"
+msgstr "Tipo"
 
 #: templates/debug_toolbar/panels/cache.html:45
 #: templates/debug_toolbar/panels/request.html:8
 msgid "Arguments"
-msgstr ""
+msgstr "Argomenti"
 
 #: templates/debug_toolbar/panels/cache.html:46
 #: templates/debug_toolbar/panels/request.html:9
 msgid "Keyword arguments"
-msgstr ""
+msgstr "Parole chiave"
 
 #: templates/debug_toolbar/panels/cache.html:47
 msgid "Backend"
-msgstr ""
+msgstr "Backend"
 
 #: templates/debug_toolbar/panels/headers.html:3
 msgid "Request headers"
-msgstr ""
+msgstr "Header della request"
 
 #: templates/debug_toolbar/panels/headers.html:8
 #: templates/debug_toolbar/panels/headers.html:27
 #: templates/debug_toolbar/panels/headers.html:48
 msgid "Key"
-msgstr "Ключ"
+msgstr "Nome"
 
 #: templates/debug_toolbar/panels/headers.html:9
 #: templates/debug_toolbar/panels/headers.html:28
 #: templates/debug_toolbar/panels/headers.html:49
-#: templates/debug_toolbar/panels/request.html:33
-#: templates/debug_toolbar/panels/request.html:59
-#: templates/debug_toolbar/panels/request.html:85
-#: templates/debug_toolbar/panels/request.html:110
+#: templates/debug_toolbar/panels/history_tr.html:23
+#: templates/debug_toolbar/panels/request_variables.html:12
 #: templates/debug_toolbar/panels/settings.html:6
 #: templates/debug_toolbar/panels/timer.html:11
 msgid "Value"
-msgstr "Значення"
+msgstr "Valore"
 
 #: templates/debug_toolbar/panels/headers.html:22
 msgid "Response headers"
-msgstr ""
+msgstr "Header della response"
 
 #: templates/debug_toolbar/panels/headers.html:41
 msgid "WSGI environ"
-msgstr ""
+msgstr "Ambiente WSGI"
 
 #: templates/debug_toolbar/panels/headers.html:43
 msgid ""
 "Since the WSGI environ inherits the environment of the server, only a "
 "significant subset is shown below."
 msgstr ""
+"Visto che l'ambiente WSGI è ereditato dal server, sotto è mostrata solo la "
+"parte significativa."
 
-#: templates/debug_toolbar/panels/logging.html:6
-msgid "Level"
-msgstr "Рівень"
+#: templates/debug_toolbar/panels/history.html:10
+msgid "Method"
+msgstr ""
 
-#: templates/debug_toolbar/panels/logging.html:8
-msgid "Channel"
+#: templates/debug_toolbar/panels/history.html:11
+#: templates/debug_toolbar/panels/staticfiles.html:43
+msgid "Path"
+msgstr "Percorso"
+
+#: templates/debug_toolbar/panels/history.html:12
+msgid "Request Variables"
 msgstr ""
 
-#: templates/debug_toolbar/panels/logging.html:9
-msgid "Message"
-msgstr "Повідомлення"
+#: templates/debug_toolbar/panels/history.html:13
+msgid "Status"
+msgstr ""
 
-#: templates/debug_toolbar/panels/logging.html:10
-#: templates/debug_toolbar/panels/staticfiles.html:45
-msgid "Location"
-msgstr "Місце"
+#: templates/debug_toolbar/panels/history.html:14
+#: templates/debug_toolbar/panels/sql.html:37
+msgid "Action"
+msgstr "Azione"
 
-#: templates/debug_toolbar/panels/logging.html:26
-msgid "No messages logged"
-msgstr "Повідомлень немає"
+#: templates/debug_toolbar/panels/history_tr.html:22
+#: templates/debug_toolbar/panels/request_variables.html:11
+msgid "Variable"
+msgstr "Variabile"
 
 #: templates/debug_toolbar/panels/profiling.html:5
 msgid "Call"
-msgstr ""
+msgstr "Chiamata"
 
 #: templates/debug_toolbar/panels/profiling.html:6
 msgid "CumTime"
-msgstr ""
+msgstr "CumTime"
 
 #: templates/debug_toolbar/panels/profiling.html:7
 #: templates/debug_toolbar/panels/profiling.html:9
 msgid "Per"
-msgstr ""
+msgstr "Per"
 
 #: templates/debug_toolbar/panels/profiling.html:8
 msgid "TotTime"
-msgstr ""
+msgstr "TotTime"
 
 #: templates/debug_toolbar/panels/profiling.html:10
 msgid "Count"
-msgstr ""
+msgstr "Numero"
 
 #: templates/debug_toolbar/panels/request.html:3
 msgid "View information"
-msgstr ""
+msgstr "Vedi Informazioni"
 
 #: templates/debug_toolbar/panels/request.html:7
 msgid "View function"
-msgstr ""
+msgstr "Funzione View"
 
 #: templates/debug_toolbar/panels/request.html:10
 msgid "URL name"
-msgstr ""
+msgstr "Nome URL"
 
 #: templates/debug_toolbar/panels/request.html:24
 msgid "Cookies"
-msgstr ""
-
-#: templates/debug_toolbar/panels/request.html:32
-#: templates/debug_toolbar/panels/request.html:58
-#: templates/debug_toolbar/panels/request.html:84
-#: templates/debug_toolbar/panels/request.html:109
-msgid "Variable"
-msgstr "Змінна"
+msgstr "Cookies"
 
-#: templates/debug_toolbar/panels/request.html:46
+#: templates/debug_toolbar/panels/request.html:27
 msgid "No cookies"
-msgstr ""
+msgstr "Nessun cookie"
 
-#: templates/debug_toolbar/panels/request.html:50
+#: templates/debug_toolbar/panels/request.html:31
 msgid "Session data"
-msgstr ""
+msgstr "Dati di sessione"
 
-#: templates/debug_toolbar/panels/request.html:72
+#: templates/debug_toolbar/panels/request.html:34
 msgid "No session data"
-msgstr ""
+msgstr "Nessun dato in sessione"
 
-#: templates/debug_toolbar/panels/request.html:76
+#: templates/debug_toolbar/panels/request.html:38
 msgid "GET data"
-msgstr ""
+msgstr "Dati GET"
 
-#: templates/debug_toolbar/panels/request.html:98
+#: templates/debug_toolbar/panels/request.html:41
 msgid "No GET data"
-msgstr "Немає GET даних"
+msgstr "Nessun dato in GET"
 
-#: templates/debug_toolbar/panels/request.html:102
+#: templates/debug_toolbar/panels/request.html:45
 msgid "POST data"
-msgstr ""
+msgstr "Dati POST"
 
-#: templates/debug_toolbar/panels/request.html:123
+#: templates/debug_toolbar/panels/request.html:48
 msgid "No POST data"
-msgstr "Немає POST даних"
+msgstr "Nessuno dato in POST"
 
 #: templates/debug_toolbar/panels/settings.html:5
 msgid "Setting"
-msgstr ""
+msgstr "Impostazione"
 
 #: templates/debug_toolbar/panels/signals.html:5
 msgid "Signal"
-msgstr "Сигнал"
+msgstr "Segnale"
 
 #: templates/debug_toolbar/panels/signals.html:6
-msgid "Providing"
-msgstr ""
-
-#: templates/debug_toolbar/panels/signals.html:7
 msgid "Receivers"
-msgstr "Отримувачі сигнала"
+msgstr "Ricevitori"
 
-#: templates/debug_toolbar/panels/sql.html:7
+#: templates/debug_toolbar/panels/sql.html:6
 #, python-format
 msgid "%(num)s query"
 msgid_plural "%(num)s queries"
-msgstr[0] ""
-msgstr[1] ""
-msgstr[2] ""
+msgstr[0] "%(num)s query"
+msgstr[1] "%(num)s query"
 
-#: templates/debug_toolbar/panels/sql.html:18
+#: templates/debug_toolbar/panels/sql.html:8
+#, python-format
+msgid ""
+"including <abbr title=\"Similar queries are queries with the same SQL, but "
+"potentially different parameters.\">%(count)s similar</abbr>"
+msgstr ""
+
+#: templates/debug_toolbar/panels/sql.html:12
+#, python-format
+msgid ""
+"and <abbr title=\"Duplicate queries are identical to each other: they "
+"execute exactly the same SQL and parameters.\">%(dupes)s duplicates</abbr>"
+msgstr ""
+
+#: templates/debug_toolbar/panels/sql.html:34
 msgid "Query"
-msgstr "Запит"
+msgstr "Query"
 
-#: templates/debug_toolbar/panels/sql.html:19
+#: templates/debug_toolbar/panels/sql.html:35
 #: templates/debug_toolbar/panels/timer.html:36
 msgid "Timeline"
+msgstr "Timeline"
+
+#: templates/debug_toolbar/panels/sql.html:52
+#, python-format
+msgid "%(count)s similar queries."
 msgstr ""
 
-#: templates/debug_toolbar/panels/sql.html:21
-msgid "Action"
-msgstr "Подія"
+#: templates/debug_toolbar/panels/sql.html:58
+#, python-format
+msgid "Duplicated %(dupes)s times."
+msgstr ""
 
-#: templates/debug_toolbar/panels/sql.html:64
+#: templates/debug_toolbar/panels/sql.html:95
 msgid "Connection:"
-msgstr ""
+msgstr "Connessione:"
 
-#: templates/debug_toolbar/panels/sql.html:66
+#: templates/debug_toolbar/panels/sql.html:97
 msgid "Isolation level:"
-msgstr ""
+msgstr "Isolation level:"
 
-#: templates/debug_toolbar/panels/sql.html:69
+#: templates/debug_toolbar/panels/sql.html:100
 msgid "Transaction status:"
-msgstr ""
+msgstr "Stato transazione:"
 
-#: templates/debug_toolbar/panels/sql.html:83
+#: templates/debug_toolbar/panels/sql.html:114
 msgid "(unknown)"
-msgstr ""
+msgstr "(sconosciuto)"
 
-#: templates/debug_toolbar/panels/sql.html:92
+#: templates/debug_toolbar/panels/sql.html:123
 msgid "No SQL queries were recorded during this request."
-msgstr ""
-
-#: templates/debug_toolbar/panels/sql_explain.html:3
-#: templates/debug_toolbar/panels/sql_profile.html:3
-#: templates/debug_toolbar/panels/sql_select.html:3
-#: templates/debug_toolbar/panels/template_source.html:3
-msgid "Back"
-msgstr "Назад"
+msgstr "Nessuna Query SQL è stata registrata durante questa richiesta"
 
 #: templates/debug_toolbar/panels/sql_explain.html:4
 msgid "SQL explained"
-msgstr ""
+msgstr "SQL spigato"
 
 #: templates/debug_toolbar/panels/sql_explain.html:9
 #: templates/debug_toolbar/panels/sql_profile.html:10
 #: templates/debug_toolbar/panels/sql_select.html:9
 msgid "Executed SQL"
-msgstr ""
+msgstr "SQL eseguita"
 
 #: templates/debug_toolbar/panels/sql_explain.html:13
 #: templates/debug_toolbar/panels/sql_profile.html:14
 #: templates/debug_toolbar/panels/sql_select.html:13
 msgid "Database"
-msgstr "База даних"
+msgstr "Database"
 
 #: templates/debug_toolbar/panels/sql_profile.html:4
 msgid "SQL profiled"
-msgstr ""
+msgstr "SQL profilato"
 
 #: templates/debug_toolbar/panels/sql_profile.html:37
 msgid "Error"
-msgstr "Помилка"
+msgstr "Errore"
 
 #: templates/debug_toolbar/panels/sql_select.html:4
 msgid "SQL selected"
-msgstr ""
+msgstr "SQL selezionato"
 
 #: templates/debug_toolbar/panels/sql_select.html:36
 msgid "Empty set"
-msgstr ""
+msgstr "Insieme vuoto"
 
-#: templates/debug_toolbar/panels/staticfiles.html:4
+#: templates/debug_toolbar/panels/staticfiles.html:3
 msgid "Static file path"
 msgid_plural "Static file paths"
-msgstr[0] ""
-msgstr[1] ""
-msgstr[2] ""
+msgstr[0] "Percorso file statici"
+msgstr[1] "Percorsi file statici"
 
-#: templates/debug_toolbar/panels/staticfiles.html:8
+#: templates/debug_toolbar/panels/staticfiles.html:7
 #, python-format
 msgid "(prefix %(prefix)s)"
-msgstr ""
+msgstr "(prefisso %(prefix)s)"
 
-#: templates/debug_toolbar/panels/staticfiles.html:12
-#: templates/debug_toolbar/panels/staticfiles.html:23
-#: templates/debug_toolbar/panels/staticfiles.html:35
+#: templates/debug_toolbar/panels/staticfiles.html:11
+#: templates/debug_toolbar/panels/staticfiles.html:22
+#: templates/debug_toolbar/panels/staticfiles.html:34
 #: templates/debug_toolbar/panels/templates.html:10
-#: templates/debug_toolbar/panels/templates.html:28
-#: templates/debug_toolbar/panels/templates.html:43
+#: templates/debug_toolbar/panels/templates.html:30
+#: templates/debug_toolbar/panels/templates.html:47
 msgid "None"
-msgstr ""
+msgstr "Nessuno"
 
-#: templates/debug_toolbar/panels/staticfiles.html:15
+#: templates/debug_toolbar/panels/staticfiles.html:14
 msgid "Static file app"
 msgid_plural "Static file apps"
-msgstr[0] ""
-msgstr[1] ""
-msgstr[2] ""
+msgstr[0] "App file statici"
+msgstr[1] "App file statici"
 
-#: templates/debug_toolbar/panels/staticfiles.html:26
+#: templates/debug_toolbar/panels/staticfiles.html:25
 msgid "Static file"
 msgid_plural "Static files"
 msgstr[0] ""
-msgstr[1] ""
-msgstr[2] ""
+msgstr[1] "Files statici"
 
-#: templates/debug_toolbar/panels/staticfiles.html:40
+#: templates/debug_toolbar/panels/staticfiles.html:39
 #, python-format
 msgid "%(payload_count)s file"
 msgid_plural "%(payload_count)s files"
-msgstr[0] ""
-msgstr[1] ""
-msgstr[2] ""
+msgstr[0] "%(payload_count)s file"
+msgstr[1] "%(payload_count)s file"
 
 #: templates/debug_toolbar/panels/staticfiles.html:44
-msgid "Path"
-msgstr ""
+msgid "Location"
+msgstr "Location"
 
 #: templates/debug_toolbar/panels/template_source.html:4
 msgid "Template source:"
-msgstr ""
+msgstr "Sorgente del template"
 
 #: templates/debug_toolbar/panels/templates.html:2
 msgid "Template path"
 msgid_plural "Template paths"
-msgstr[0] ""
-msgstr[1] ""
-msgstr[2] ""
+msgstr[0] "Percorso dei template"
+msgstr[1] "Percorsi dei template"
 
 #: templates/debug_toolbar/panels/templates.html:13
 msgid "Template"
 msgid_plural "Templates"
-msgstr[0] "Шаблон"
-msgstr[1] "Шаблони"
-msgstr[2] "Шаблонів"
+msgstr[0] ""
+msgstr[1] "Template"
 
-#: templates/debug_toolbar/panels/templates.html:21
-#: templates/debug_toolbar/panels/templates.html:37
+#: templates/debug_toolbar/panels/templates.html:22
+#: templates/debug_toolbar/panels/templates.html:40
 msgid "Toggle context"
-msgstr ""
+msgstr "Cambia contesto"
 
-#: templates/debug_toolbar/panels/templates.html:31
+#: templates/debug_toolbar/panels/templates.html:33
 msgid "Context processor"
 msgid_plural "Context processors"
-msgstr[0] ""
-msgstr[1] ""
-msgstr[2] ""
+msgstr[0] "Context processor"
+msgstr[1] "Context processors"
 
 #: templates/debug_toolbar/panels/timer.html:2
 msgid "Resource usage"
-msgstr ""
+msgstr "Uso risorsa"
 
 #: templates/debug_toolbar/panels/timer.html:10
 msgid "Resource"
-msgstr ""
+msgstr "Risorsa"
 
 #: templates/debug_toolbar/panels/timer.html:26
 msgid "Browser timing"
-msgstr ""
+msgstr "Tempo browser"
 
 #: templates/debug_toolbar/panels/timer.html:35
 msgid "Timing attribute"
-msgstr ""
+msgstr "Attributo"
 
 #: templates/debug_toolbar/panels/timer.html:37
 msgid "Milliseconds since navigation start (+length)"
+msgstr "Millisecondi dall'inizio della navigazione (+lunghezza)"
+
+#: templates/debug_toolbar/panels/versions.html:10
+msgid "Package"
 msgstr ""
 
-#: templates/debug_toolbar/panels/versions.html:5
+#: templates/debug_toolbar/panels/versions.html:11
 msgid "Name"
-msgstr ""
+msgstr "Nome"
 
-#: templates/debug_toolbar/panels/versions.html:6
+#: templates/debug_toolbar/panels/versions.html:12
 msgid "Version"
-msgstr "Версія"
+msgstr "Versione"
+
+#: templates/debug_toolbar/redirect.html:10
+msgid "Location:"
+msgstr "Location:"
+
+#: templates/debug_toolbar/redirect.html:12
+msgid ""
+"The Django Debug Toolbar has intercepted a redirect to the above URL for "
+"debug viewing purposes. You can click the above link to continue with the "
+"redirect as normal."
+msgstr ""
+"Django Debug Toolbar ha intercettato un redirect verso la URL indicata per "
+"visualizzare il debug, Puoi cliccare sul link sopra per continuare "
+"normalmente con la redirezione."
+
+#: views.py:16
+msgid ""
+"Data for this panel isn't available anymore. Please reload the page and "
+"retry."
+msgstr ""
+"Non sono più disponibili dati per questo pannello. Ricarica la pagina e "
+"riprova."
```

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/locale/zh_CN/LC_MESSAGES/django.mo` & `django_debug_toolbar-4.0.0/debug_toolbar/locale/zh_CN/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/locale/zh_CN/LC_MESSAGES/django.po` & `django_debug_toolbar-4.0.0/debug_toolbar/locale/zh_CN/LC_MESSAGES/django.po`

 * *Files 9% similar despite different names*

```diff
@@ -4,282 +4,271 @@
 #
 # Translators:
 # mozillazg <opensource.mozillazg@gmail.com>, 2013-2014
 msgid ""
 msgstr ""
 "Project-Id-Version: Django Debug Toolbar\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2014-04-25 21:52+0200\n"
+"POT-Creation-Date: 2023-01-20 17:23+0100\n"
 "PO-Revision-Date: 2014-04-25 19:53+0000\n"
 "Last-Translator: Aymeric Augustin <aymeric.augustin@m4x.org>\n"
-"Language-Team: Chinese (China) (http://www.transifex.com/projects/p/django-debug-toolbar/language/zh_CN/)\n"
+"Language-Team: Chinese (China) (http://www.transifex.com/projects/p/django-"
+"debug-toolbar/language/zh_CN/)\n"
+"Language: zh_CN\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: zh_CN\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 
-#: apps.py:11
+#: apps.py:15
 msgid "Debug Toolbar"
 msgstr ""
 
-#: views.py:14
-msgid ""
-"Data for this panel isn't available anymore. Please reload the page and "
-"retry."
-msgstr "当前面板的数据暂不可用。请刷新页面并重试。"
-
-#: panels/cache.py:191
+#: panels/cache.py:180
 msgid "Cache"
 msgstr "缓存"
 
-#: panels/cache.py:196
+#: panels/cache.py:186
 #, python-format
 msgid "%(cache_calls)d call in %(time).2fms"
 msgid_plural "%(cache_calls)d calls in %(time).2fms"
 msgstr[0] "%(time).2f 毫秒内 %(cache_calls)d 次调用"
 
-#: panels/cache.py:204
+#: panels/cache.py:195
 #, python-format
 msgid "Cache calls from %(count)d backend"
 msgid_plural "Cache calls from %(count)d backends"
 msgstr[0] "来自 %(count)d 个后端的缓存调用"
 
-#: panels/headers.py:35
+#: panels/headers.py:31
 msgid "Headers"
 msgstr "HTTP 头"
 
-#: panels/logging.py:64
-msgid "Logging"
-msgstr "日志"
-
-#: panels/logging.py:70
-#, python-format
-msgid "%(count)s message"
-msgid_plural "%(count)s messages"
-msgstr[0] "%(count)s 条消息"
-
-#: panels/logging.py:73
-msgid "Log messages"
-msgstr "日志信息"
+#: panels/history/panel.py:18 panels/history/panel.py:19
+msgid "History"
+msgstr ""
 
-#: panels/profiling.py:127
+#: panels/profiling.py:140
 msgid "Profiling"
 msgstr "性能分析"
 
-#: panels/redirects.py:17
+#: panels/redirects.py:14
 msgid "Intercept redirects"
 msgstr "拦截重定向"
 
-#: panels/request.py:18
+#: panels/request.py:16
 msgid "Request"
 msgstr "请求"
 
-#: panels/request.py:35
+#: panels/request.py:36
 msgid "<no view>"
 msgstr "<没有 view>"
 
-#: panels/request.py:47
+#: panels/request.py:53
 msgid "<unavailable>"
 msgstr "<不可用>"
 
-#: panels/settings.py:20
+#: panels/settings.py:17
 msgid "Settings"
 msgstr "设置"
 
-#: panels/settings.py:23
-#, python-format
-msgid "Settings from <code>%s</code>"
+#: panels/settings.py:20
+#, fuzzy, python-format
+#| msgid "Settings from <code>%s</code>"
+msgid "Settings from %s"
 msgstr "来自 <code>%s</code> 的设置"
 
-#: panels/signals.py:45
+#: panels/signals.py:57
 #, python-format
 msgid "%(num_receivers)d receiver of 1 signal"
 msgid_plural "%(num_receivers)d receivers of 1 signal"
 msgstr[0] "1个信号 %(num_receivers)d 个接收者"
 
-#: panels/signals.py:48
+#: panels/signals.py:62
 #, python-format
 msgid "%(num_receivers)d receiver of %(num_signals)d signals"
 msgid_plural "%(num_receivers)d receivers of %(num_signals)d signals"
 msgstr[0] "%(num_signals)d 个信号 %(num_receivers)d 个接收者"
 
-#: panels/signals.py:53
+#: panels/signals.py:67
 msgid "Signals"
 msgstr "信号"
 
-#: panels/staticfiles.py:89
+#: panels/sql/panel.py:23
+msgid "Autocommit"
+msgstr "自动提交"
+
+#: panels/sql/panel.py:24
+msgid "Read uncommitted"
+msgstr "读取未提交的"
+
+#: panels/sql/panel.py:25
+msgid "Read committed"
+msgstr "读取已提交的"
+
+#: panels/sql/panel.py:26
+msgid "Repeatable read"
+msgstr "可重复读取"
+
+#: panels/sql/panel.py:27
+msgid "Serializable"
+msgstr "可序列化"
+
+#: panels/sql/panel.py:39
+msgid "Idle"
+msgstr "空闲"
+
+#: panels/sql/panel.py:40
+msgid "Active"
+msgstr "活跃"
+
+#: panels/sql/panel.py:41
+msgid "In transaction"
+msgstr "事务"
+
+#: panels/sql/panel.py:42
+msgid "In error"
+msgstr "错误"
+
+#: panels/sql/panel.py:43
+msgid "Unknown"
+msgstr "未知"
+
+#: panels/sql/panel.py:130
+msgid "SQL"
+msgstr "SQL"
+
+#: panels/sql/panel.py:135
+#, fuzzy, python-format
+#| msgid "%(cache_calls)d call in %(time).2fms"
+#| msgid_plural "%(cache_calls)d calls in %(time).2fms"
+msgid "%(query_count)d query in %(sql_time).2fms"
+msgid_plural "%(query_count)d queries in %(sql_time).2fms"
+msgstr[0] "%(time).2f 毫秒内 %(cache_calls)d 次调用"
+
+#: panels/sql/panel.py:147
+#, python-format
+msgid "SQL queries from %(count)d connection"
+msgid_plural "SQL queries from %(count)d connections"
+msgstr[0] ""
+
+#: panels/staticfiles.py:84
 #, python-format
 msgid "Static files (%(num_found)s found, %(num_used)s used)"
 msgstr "静态文件 (%(num_found)s 个找到，%(num_used)s 个被使用)"
 
-#: panels/staticfiles.py:107
+#: panels/staticfiles.py:105
 msgid "Static files"
 msgstr "静态文件"
 
-#: panels/staticfiles.py:112
+#: panels/staticfiles.py:111
 #, python-format
 msgid "%(num_used)s file used"
 msgid_plural "%(num_used)s files used"
 msgstr[0] "%(num_used)s 个文件被使用"
 
-#: panels/timer.py:23
+#: panels/templates/panel.py:143
+msgid "Templates"
+msgstr "模板"
+
+#: panels/templates/panel.py:148
+#, python-format
+msgid "Templates (%(num_templates)s rendered)"
+msgstr "模板 (%(num_templates)s 个被渲染)"
+
+#: panels/templates/panel.py:180
+msgid "No origin"
+msgstr ""
+
+#: panels/timer.py:25
 #, python-format
 msgid "CPU: %(cum)0.2fms (%(total)0.2fms)"
 msgstr "CPU: %(cum)0.2f 毫秒 (总耗时: %(total)0.2f 毫秒)"
 
-#: panels/timer.py:28
+#: panels/timer.py:30
 #, python-format
 msgid "Total: %0.2fms"
 msgstr "总共：%0.2f 毫秒"
 
-#: panels/timer.py:34 templates/debug_toolbar/panels/logging.html:7
+#: panels/timer.py:36 templates/debug_toolbar/panels/history.html:9
 #: templates/debug_toolbar/panels/sql_explain.html:11
 #: templates/debug_toolbar/panels/sql_profile.html:12
 #: templates/debug_toolbar/panels/sql_select.html:11
 msgid "Time"
 msgstr "时间"
 
-#: panels/timer.py:42
+#: panels/timer.py:44
 msgid "User CPU time"
 msgstr "用户 CPU 时间"
 
-#: panels/timer.py:42
+#: panels/timer.py:44
 #, python-format
 msgid "%(utime)0.3f msec"
 msgstr "%(utime)0.3f 毫秒"
 
-#: panels/timer.py:43
+#: panels/timer.py:45
 msgid "System CPU time"
 msgstr "系统 CPU 时间"
 
-#: panels/timer.py:43
+#: panels/timer.py:45
 #, python-format
 msgid "%(stime)0.3f msec"
 msgstr "%(stime)0.3f 毫秒"
 
-#: panels/timer.py:44
+#: panels/timer.py:46
 msgid "Total CPU time"
 msgstr "总的 CPU 时间"
 
-#: panels/timer.py:44
+#: panels/timer.py:46
 #, python-format
 msgid "%(total)0.3f msec"
 msgstr "%(total)0.3f 毫秒"
 
-#: panels/timer.py:45
+#: panels/timer.py:47
 msgid "Elapsed time"
 msgstr "耗时"
 
-#: panels/timer.py:45
+#: panels/timer.py:47
 #, python-format
 msgid "%(total_time)0.3f msec"
 msgstr "%(total_time)0.3f 毫秒"
 
-#: panels/timer.py:46
+#: panels/timer.py:49
 msgid "Context switches"
 msgstr "上下文切换"
 
-#: panels/timer.py:46
+#: panels/timer.py:50
 #, python-format
 msgid "%(vcsw)d voluntary, %(ivcsw)d involuntary"
 msgstr "%(vcsw)d 主动, %(ivcsw)d 被动"
 
-#: panels/versions.py:25
+#: panels/versions.py:19
 msgid "Versions"
 msgstr "版本"
 
-#: panels/sql/panel.py:22
-msgid "Autocommit"
-msgstr "自动提交"
-
-#: panels/sql/panel.py:23
-msgid "Read uncommitted"
-msgstr "读取未提交的"
-
-#: panels/sql/panel.py:24
-msgid "Read committed"
-msgstr "读取已提交的"
-
-#: panels/sql/panel.py:25
-msgid "Repeatable read"
-msgstr "可重复读取"
-
-#: panels/sql/panel.py:26
-msgid "Serializable"
-msgstr "可序列化"
-
-#: panels/sql/panel.py:37
-msgid "Idle"
-msgstr "空闲"
-
-#: panels/sql/panel.py:38
-msgid "Active"
-msgstr "活跃"
-
-#: panels/sql/panel.py:39
-msgid "In transaction"
-msgstr "事务"
-
-#: panels/sql/panel.py:40
-msgid "In error"
-msgstr "错误"
-
-#: panels/sql/panel.py:41
-msgid "Unknown"
-msgstr "未知"
-
-#: panels/sql/panel.py:105
-msgid "SQL"
-msgstr "SQL"
-
-#: panels/templates/panel.py:141
-msgid "Templates"
-msgstr "模板"
-
-#: panels/templates/panel.py:146
-#, python-format
-msgid "Templates (%(num_templates)s rendered)"
-msgstr "模板 (%(num_templates)s 个被渲染)"
-
-#: templates/debug_toolbar/base.html:19
+#: templates/debug_toolbar/base.html:22
 msgid "Hide toolbar"
 msgstr "隐藏工具栏"
 
-#: templates/debug_toolbar/base.html:19
+#: templates/debug_toolbar/base.html:22
 msgid "Hide"
 msgstr "隐藏"
 
-#: templates/debug_toolbar/base.html:25
+#: templates/debug_toolbar/base.html:29
+msgid "Show toolbar"
+msgstr "显示工具栏"
+
+#: templates/debug_toolbar/includes/panel_button.html:4
 msgid "Disable for next and successive requests"
 msgstr "针对下一个连续的请求禁用该功能"
 
-#: templates/debug_toolbar/base.html:25
+#: templates/debug_toolbar/includes/panel_button.html:4
 msgid "Enable for next and successive requests"
 msgstr "针对下一个连续的请求启用该功能"
 
-#: templates/debug_toolbar/base.html:47
-msgid "Show toolbar"
-msgstr "显示工具栏"
-
-#: templates/debug_toolbar/base.html:53
-msgid "Close"
-msgstr "关闭"
-
-#: templates/debug_toolbar/redirect.html:8
-msgid "Location:"
-msgstr "位置："
-
-#: templates/debug_toolbar/redirect.html:10
-msgid ""
-"The Django Debug Toolbar has intercepted a redirect to the above URL for "
-"debug viewing purposes. You can click the above link to continue with the "
-"redirect as normal."
-msgstr "Django Debug Toolbar 为了调试目的拦截了一个重定向到上面 URL 的请求。  您可以点击上面的链接继续执行重定向操作。"
-
 #: templates/debug_toolbar/panels/cache.html:2
 msgid "Summary"
 msgstr "摘要"
 
 #: templates/debug_toolbar/panels/cache.html:6
 msgid "Total calls"
 msgstr "总调用次数"
@@ -301,15 +290,15 @@
 msgstr "命令"
 
 #: templates/debug_toolbar/panels/cache.html:39
 msgid "Calls"
 msgstr "调用"
 
 #: templates/debug_toolbar/panels/cache.html:43
-#: templates/debug_toolbar/panels/sql.html:20
+#: templates/debug_toolbar/panels/sql.html:36
 msgid "Time (ms)"
 msgstr "时间(毫秒)"
 
 #: templates/debug_toolbar/panels/cache.html:44
 msgid "Type"
 msgstr "类型"
 
@@ -336,18 +325,16 @@
 #: templates/debug_toolbar/panels/headers.html:48
 msgid "Key"
 msgstr "键"
 
 #: templates/debug_toolbar/panels/headers.html:9
 #: templates/debug_toolbar/panels/headers.html:28
 #: templates/debug_toolbar/panels/headers.html:49
-#: templates/debug_toolbar/panels/request.html:33
-#: templates/debug_toolbar/panels/request.html:59
-#: templates/debug_toolbar/panels/request.html:85
-#: templates/debug_toolbar/panels/request.html:110
+#: templates/debug_toolbar/panels/history_tr.html:23
+#: templates/debug_toolbar/panels/request_variables.html:12
 #: templates/debug_toolbar/panels/settings.html:6
 #: templates/debug_toolbar/panels/timer.html:11
 msgid "Value"
 msgstr "值"
 
 #: templates/debug_toolbar/panels/headers.html:22
 msgid "Response headers"
@@ -359,34 +346,42 @@
 
 #: templates/debug_toolbar/panels/headers.html:43
 msgid ""
 "Since the WSGI environ inherits the environment of the server, only a "
 "significant subset is shown below."
 msgstr "由于 WSGI 的环境变量继承自 server，所以下面只显示了一些重要的子集。"
 
-#: templates/debug_toolbar/panels/logging.html:6
-msgid "Level"
-msgstr "级别"
-
-#: templates/debug_toolbar/panels/logging.html:8
-msgid "Channel"
-msgstr "频道"
-
-#: templates/debug_toolbar/panels/logging.html:9
-msgid "Message"
-msgstr "消息"
+#: templates/debug_toolbar/panels/history.html:10
+msgid "Method"
+msgstr ""
 
-#: templates/debug_toolbar/panels/logging.html:10
-#: templates/debug_toolbar/panels/staticfiles.html:45
-msgid "Location"
-msgstr "位置"
+#: templates/debug_toolbar/panels/history.html:11
+#: templates/debug_toolbar/panels/staticfiles.html:43
+msgid "Path"
+msgstr "路径"
 
-#: templates/debug_toolbar/panels/logging.html:26
-msgid "No messages logged"
-msgstr "没有消息被记录"
+#: templates/debug_toolbar/panels/history.html:12
+#, fuzzy
+#| msgid "Request headers"
+msgid "Request Variables"
+msgstr "请求头"
+
+#: templates/debug_toolbar/panels/history.html:13
+msgid "Status"
+msgstr ""
+
+#: templates/debug_toolbar/panels/history.html:14
+#: templates/debug_toolbar/panels/sql.html:37
+msgid "Action"
+msgstr "功能"
+
+#: templates/debug_toolbar/panels/history_tr.html:22
+#: templates/debug_toolbar/panels/request_variables.html:11
+msgid "Variable"
+msgstr "变量"
 
 #: templates/debug_toolbar/panels/profiling.html:5
 msgid "Call"
 msgstr "调用"
 
 #: templates/debug_toolbar/panels/profiling.html:6
 msgid "CumTime"
@@ -417,111 +412,115 @@
 msgid "URL name"
 msgstr "URL 名称"
 
 #: templates/debug_toolbar/panels/request.html:24
 msgid "Cookies"
 msgstr "Cookies"
 
-#: templates/debug_toolbar/panels/request.html:32
-#: templates/debug_toolbar/panels/request.html:58
-#: templates/debug_toolbar/panels/request.html:84
-#: templates/debug_toolbar/panels/request.html:109
-msgid "Variable"
-msgstr "变量"
-
-#: templates/debug_toolbar/panels/request.html:46
+#: templates/debug_toolbar/panels/request.html:27
 msgid "No cookies"
 msgstr "没有 cookies"
 
-#: templates/debug_toolbar/panels/request.html:50
+#: templates/debug_toolbar/panels/request.html:31
 msgid "Session data"
 msgstr "Session 数据"
 
-#: templates/debug_toolbar/panels/request.html:72
+#: templates/debug_toolbar/panels/request.html:34
 msgid "No session data"
 msgstr "没有 session 数据"
 
-#: templates/debug_toolbar/panels/request.html:76
+#: templates/debug_toolbar/panels/request.html:38
 msgid "GET data"
 msgstr "GET 请求数据"
 
-#: templates/debug_toolbar/panels/request.html:98
+#: templates/debug_toolbar/panels/request.html:41
 msgid "No GET data"
 msgstr "没有 GET 请求数据"
 
-#: templates/debug_toolbar/panels/request.html:102
+#: templates/debug_toolbar/panels/request.html:45
 msgid "POST data"
 msgstr "POST 请求数据"
 
-#: templates/debug_toolbar/panels/request.html:123
+#: templates/debug_toolbar/panels/request.html:48
 msgid "No POST data"
 msgstr "没有 POST 请求数据"
 
 #: templates/debug_toolbar/panels/settings.html:5
 msgid "Setting"
 msgstr "设置项"
 
 #: templates/debug_toolbar/panels/signals.html:5
 msgid "Signal"
 msgstr "信号"
 
 #: templates/debug_toolbar/panels/signals.html:6
-msgid "Providing"
-msgstr "提供"
-
-#: templates/debug_toolbar/panels/signals.html:7
 msgid "Receivers"
 msgstr "接收者"
 
-#: templates/debug_toolbar/panels/sql.html:7
+#: templates/debug_toolbar/panels/sql.html:6
 #, python-format
 msgid "%(num)s query"
 msgid_plural "%(num)s queries"
 msgstr[0] "%(num)s 个查询"
 
-#: templates/debug_toolbar/panels/sql.html:18
+#: templates/debug_toolbar/panels/sql.html:8
+#, python-format
+msgid ""
+"including <abbr title=\"Similar queries are queries with the same SQL, but "
+"potentially different parameters.\">%(count)s similar</abbr>"
+msgstr ""
+
+#: templates/debug_toolbar/panels/sql.html:12
+#, python-format
+msgid ""
+"and <abbr title=\"Duplicate queries are identical to each other: they "
+"execute exactly the same SQL and parameters.\">%(dupes)s duplicates</abbr>"
+msgstr ""
+
+#: templates/debug_toolbar/panels/sql.html:34
 msgid "Query"
 msgstr "查询"
 
-#: templates/debug_toolbar/panels/sql.html:19
+#: templates/debug_toolbar/panels/sql.html:35
 #: templates/debug_toolbar/panels/timer.html:36
 msgid "Timeline"
 msgstr "时间线"
 
-#: templates/debug_toolbar/panels/sql.html:21
-msgid "Action"
-msgstr "功能"
+#: templates/debug_toolbar/panels/sql.html:52
+#, fuzzy, python-format
+#| msgid "%(count)s message"
+#| msgid_plural "%(count)s messages"
+msgid "%(count)s similar queries."
+msgstr "%(count)s 条消息"
+
+#: templates/debug_toolbar/panels/sql.html:58
+#, python-format
+msgid "Duplicated %(dupes)s times."
+msgstr ""
 
-#: templates/debug_toolbar/panels/sql.html:64
+#: templates/debug_toolbar/panels/sql.html:95
 msgid "Connection:"
 msgstr "连接："
 
-#: templates/debug_toolbar/panels/sql.html:66
+#: templates/debug_toolbar/panels/sql.html:97
 msgid "Isolation level:"
 msgstr "隔离级别"
 
-#: templates/debug_toolbar/panels/sql.html:69
+#: templates/debug_toolbar/panels/sql.html:100
 msgid "Transaction status:"
 msgstr "事务状态："
 
-#: templates/debug_toolbar/panels/sql.html:83
+#: templates/debug_toolbar/panels/sql.html:114
 msgid "(unknown)"
 msgstr "(未知)"
 
-#: templates/debug_toolbar/panels/sql.html:92
+#: templates/debug_toolbar/panels/sql.html:123
 msgid "No SQL queries were recorded during this request."
 msgstr "在处理这个请求期间没有记录到 SQL 查询。"
 
-#: templates/debug_toolbar/panels/sql_explain.html:3
-#: templates/debug_toolbar/panels/sql_profile.html:3
-#: templates/debug_toolbar/panels/sql_select.html:3
-#: templates/debug_toolbar/panels/template_source.html:3
-msgid "Back"
-msgstr "返回"
-
 #: templates/debug_toolbar/panels/sql_explain.html:4
 msgid "SQL explained"
 msgstr "SQL explain 分析"
 
 #: templates/debug_toolbar/panels/sql_explain.html:9
 #: templates/debug_toolbar/panels/sql_profile.html:10
 #: templates/debug_toolbar/panels/sql_select.html:9
@@ -546,52 +545,52 @@
 msgid "SQL selected"
 msgstr "选中的 SQL 语句"
 
 #: templates/debug_toolbar/panels/sql_select.html:36
 msgid "Empty set"
 msgstr "空集合"
 
-#: templates/debug_toolbar/panels/staticfiles.html:4
+#: templates/debug_toolbar/panels/staticfiles.html:3
 msgid "Static file path"
 msgid_plural "Static file paths"
 msgstr[0] "静态文件路径"
 
-#: templates/debug_toolbar/panels/staticfiles.html:8
+#: templates/debug_toolbar/panels/staticfiles.html:7
 #, python-format
 msgid "(prefix %(prefix)s)"
 msgstr "(前缀 %(prefix)s)"
 
-#: templates/debug_toolbar/panels/staticfiles.html:12
-#: templates/debug_toolbar/panels/staticfiles.html:23
-#: templates/debug_toolbar/panels/staticfiles.html:35
+#: templates/debug_toolbar/panels/staticfiles.html:11
+#: templates/debug_toolbar/panels/staticfiles.html:22
+#: templates/debug_toolbar/panels/staticfiles.html:34
 #: templates/debug_toolbar/panels/templates.html:10
-#: templates/debug_toolbar/panels/templates.html:28
-#: templates/debug_toolbar/panels/templates.html:43
+#: templates/debug_toolbar/panels/templates.html:30
+#: templates/debug_toolbar/panels/templates.html:47
 msgid "None"
 msgstr "空"
 
-#: templates/debug_toolbar/panels/staticfiles.html:15
+#: templates/debug_toolbar/panels/staticfiles.html:14
 msgid "Static file app"
 msgid_plural "Static file apps"
 msgstr[0] "包含静态文件的应用"
 
-#: templates/debug_toolbar/panels/staticfiles.html:26
+#: templates/debug_toolbar/panels/staticfiles.html:25
 msgid "Static file"
 msgid_plural "Static files"
 msgstr[0] "静态文件"
 
-#: templates/debug_toolbar/panels/staticfiles.html:40
+#: templates/debug_toolbar/panels/staticfiles.html:39
 #, python-format
 msgid "%(payload_count)s file"
 msgid_plural "%(payload_count)s files"
 msgstr[0] "%(payload_count)s 个文件"
 
 #: templates/debug_toolbar/panels/staticfiles.html:44
-msgid "Path"
-msgstr "路径"
+msgid "Location"
+msgstr "位置"
 
 #: templates/debug_toolbar/panels/template_source.html:4
 msgid "Template source:"
 msgstr "模板源："
 
 #: templates/debug_toolbar/panels/templates.html:2
 msgid "Template path"
@@ -599,20 +598,20 @@
 msgstr[0] "模板路径"
 
 #: templates/debug_toolbar/panels/templates.html:13
 msgid "Template"
 msgid_plural "Templates"
 msgstr[0] "模板"
 
-#: templates/debug_toolbar/panels/templates.html:21
-#: templates/debug_toolbar/panels/templates.html:37
+#: templates/debug_toolbar/panels/templates.html:22
+#: templates/debug_toolbar/panels/templates.html:40
 msgid "Toggle context"
 msgstr "切换上下文"
 
-#: templates/debug_toolbar/panels/templates.html:31
+#: templates/debug_toolbar/panels/templates.html:33
 msgid "Context processor"
 msgid_plural "Context processors"
 msgstr[0] "Context processors"
 
 #: templates/debug_toolbar/panels/timer.html:2
 msgid "Resource usage"
 msgstr "资源使用"
@@ -629,14 +628,37 @@
 msgid "Timing attribute"
 msgstr "计时属性"
 
 #: templates/debug_toolbar/panels/timer.html:37
 msgid "Milliseconds since navigation start (+length)"
 msgstr "导航开始后的毫秒 (+长度)"
 
-#: templates/debug_toolbar/panels/versions.html:5
+#: templates/debug_toolbar/panels/versions.html:10
+msgid "Package"
+msgstr ""
+
+#: templates/debug_toolbar/panels/versions.html:11
 msgid "Name"
 msgstr "名称"
 
-#: templates/debug_toolbar/panels/versions.html:6
+#: templates/debug_toolbar/panels/versions.html:12
 msgid "Version"
 msgstr "版本"
+
+#: templates/debug_toolbar/redirect.html:10
+msgid "Location:"
+msgstr "位置："
+
+#: templates/debug_toolbar/redirect.html:12
+msgid ""
+"The Django Debug Toolbar has intercepted a redirect to the above URL for "
+"debug viewing purposes. You can click the above link to continue with the "
+"redirect as normal."
+msgstr ""
+"Django Debug Toolbar 为了调试目的拦截了一个重定向到上面 URL 的请求。  您可以"
+"点击上面的链接继续执行重定向操作。"
+
+#: views.py:16
+msgid ""
+"Data for this panel isn't available anymore. Please reload the page and "
+"retry."
+msgstr "当前面板的数据暂不可用。请刷新页面并重试。"
```

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/management/commands/debugsqlshell.py` & `django_debug_toolbar-4.0.0/debug_toolbar/management/commands/debugsqlshell.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/panels/__init__.py` & `django_debug_toolbar-4.0.0/debug_toolbar/panels/__init__.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/panels/cache.py` & `django_debug_toolbar-4.0.0/debug_toolbar/panels/cache.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/panels/headers.py` & `django_debug_toolbar-4.0.0/debug_toolbar/panels/headers.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/panels/profiling.py` & `django_debug_toolbar-4.0.0/debug_toolbar/panels/profiling.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/panels/redirects.py` & `django_debug_toolbar-4.0.0/debug_toolbar/panels/redirects.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/panels/request.py` & `django_debug_toolbar-4.0.0/debug_toolbar/panels/request.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/panels/settings.py` & `django_debug_toolbar-4.0.0/debug_toolbar/panels/settings.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/panels/signals.py` & `django_debug_toolbar-4.0.0/debug_toolbar/panels/signals.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/panels/staticfiles.py` & `django_debug_toolbar-4.0.0/debug_toolbar/panels/staticfiles.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,14 @@
     """
     A staticfiles storage class to be used for collecting which paths
     are resolved by using the {% static %} template tag (which uses the
     `url` method).
     """
 
     def _setup(self):
-
         configured_storage_cls = get_storage_class(settings.STATICFILES_STORAGE)
 
         class DebugStaticFilesStorage(configured_storage_cls):
             def __init__(self, collector, *args, **kwargs):
                 super().__init__(*args, **kwargs)
                 self.collector = collector
```

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/panels/timer.py` & `django_debug_toolbar-4.0.0/debug_toolbar/panels/timer.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/panels/versions.py` & `django_debug_toolbar-4.0.0/debug_toolbar/panels/versions.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/panels/history/panel.py` & `django_debug_toolbar-4.0.0/debug_toolbar/panels/history/panel.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/panels/history/views.py` & `django_debug_toolbar-4.0.0/debug_toolbar/panels/history/views.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from django.http import HttpResponseBadRequest, JsonResponse
 from django.template.loader import render_to_string
 
-from debug_toolbar.decorators import require_show_toolbar
+from debug_toolbar.decorators import render_with_toolbar_language, require_show_toolbar
 from debug_toolbar.panels.history.forms import HistoryStoreForm
 from debug_toolbar.toolbar import DebugToolbar
 
 
 @require_show_toolbar
+@render_with_toolbar_language
 def history_sidebar(request):
     """Returns the selected debug toolbar history snapshot."""
     form = HistoryStoreForm(request.GET)
 
     if form.is_valid():
         store_id = form.cleaned_data["store_id"]
         toolbar = DebugToolbar.fetch(store_id)
@@ -33,14 +34,15 @@
                 ),
             }
         return JsonResponse(context)
     return HttpResponseBadRequest("Form errors")
 
 
 @require_show_toolbar
+@render_with_toolbar_language
 def history_refresh(request):
     """Returns the refreshed list of table rows for the History Panel."""
     form = HistoryStoreForm(request.GET)
 
     if form.is_valid():
         requests = []
         # Convert to list to handle mutations happening in parallel
```

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/panels/sql/forms.py` & `django_debug_toolbar-4.0.0/debug_toolbar/panels/sql/forms.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/panels/sql/panel.py` & `django_debug_toolbar-4.0.0/debug_toolbar/panels/sql/panel.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,39 +13,67 @@
 from debug_toolbar.panels.sql.tracking import unwrap_cursor, wrap_cursor
 from debug_toolbar.panels.sql.utils import contrasting_color_generator, reformat_sql
 from debug_toolbar.utils import render_stacktrace
 
 
 def get_isolation_level_display(vendor, level):
     if vendor == "postgresql":
-        import psycopg2.extensions
+        try:
+            import psycopg
+
+            choices = {
+                # AUTOCOMMIT level does not exists in psycopg3
+                psycopg.IsolationLevel.READ_UNCOMMITTED: _("Read uncommitted"),
+                psycopg.IsolationLevel.READ_COMMITTED: _("Read committed"),
+                psycopg.IsolationLevel.REPEATABLE_READ: _("Repeatable read"),
+                psycopg.IsolationLevel.SERIALIZABLE: _("Serializable"),
+            }
+        except ImportError:
+            import psycopg2.extensions
+
+            choices = {
+                psycopg2.extensions.ISOLATION_LEVEL_AUTOCOMMIT: _("Autocommit"),
+                psycopg2.extensions.ISOLATION_LEVEL_READ_UNCOMMITTED: _(
+                    "Read uncommitted"
+                ),
+                psycopg2.extensions.ISOLATION_LEVEL_READ_COMMITTED: _("Read committed"),
+                psycopg2.extensions.ISOLATION_LEVEL_REPEATABLE_READ: _(
+                    "Repeatable read"
+                ),
+                psycopg2.extensions.ISOLATION_LEVEL_SERIALIZABLE: _("Serializable"),
+            }
 
-        choices = {
-            psycopg2.extensions.ISOLATION_LEVEL_AUTOCOMMIT: _("Autocommit"),
-            psycopg2.extensions.ISOLATION_LEVEL_READ_UNCOMMITTED: _("Read uncommitted"),
-            psycopg2.extensions.ISOLATION_LEVEL_READ_COMMITTED: _("Read committed"),
-            psycopg2.extensions.ISOLATION_LEVEL_REPEATABLE_READ: _("Repeatable read"),
-            psycopg2.extensions.ISOLATION_LEVEL_SERIALIZABLE: _("Serializable"),
-        }
     else:
         raise ValueError(vendor)
     return choices.get(level)
 
 
 def get_transaction_status_display(vendor, level):
     if vendor == "postgresql":
-        import psycopg2.extensions
+        try:
+            import psycopg
+
+            choices = {
+                psycopg.pq.TransactionStatus.IDLE: _("Idle"),
+                psycopg.pq.TransactionStatus.ACTIVE: _("Active"),
+                psycopg.pq.TransactionStatus.INTRANS: _("In transaction"),
+                psycopg.pq.TransactionStatus.INERROR: _("In error"),
+                psycopg.pq.TransactionStatus.UNKNOWN: _("Unknown"),
+            }
+        except ImportError:
+            import psycopg2.extensions
+
+            choices = {
+                psycopg2.extensions.TRANSACTION_STATUS_IDLE: _("Idle"),
+                psycopg2.extensions.TRANSACTION_STATUS_ACTIVE: _("Active"),
+                psycopg2.extensions.TRANSACTION_STATUS_INTRANS: _("In transaction"),
+                psycopg2.extensions.TRANSACTION_STATUS_INERROR: _("In error"),
+                psycopg2.extensions.TRANSACTION_STATUS_UNKNOWN: _("Unknown"),
+            }
 
-        choices = {
-            psycopg2.extensions.TRANSACTION_STATUS_IDLE: _("Idle"),
-            psycopg2.extensions.TRANSACTION_STATUS_ACTIVE: _("Active"),
-            psycopg2.extensions.TRANSACTION_STATUS_INTRANS: _("In transaction"),
-            psycopg2.extensions.TRANSACTION_STATUS_INERROR: _("In error"),
-            psycopg2.extensions.TRANSACTION_STATUS_UNKNOWN: _("Unknown"),
-        }
     else:
         raise ValueError(vendor)
     return choices.get(level)
 
 
 def _similar_query_key(query):
     return query["raw_sql"]
```

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/panels/sql/tracking.py` & `django_debug_toolbar-4.0.0/debug_toolbar/panels/sql/tracking.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,19 +5,25 @@
 
 from django.utils.encoding import force_str
 
 from debug_toolbar import settings as dt_settings
 from debug_toolbar.utils import get_stack_trace, get_template_info
 
 try:
-    from psycopg2._json import Json as PostgresJson
-    from psycopg2.extensions import STATUS_IN_TRANSACTION
+    import psycopg
+
+    PostgresJson = psycopg.types.json.Jsonb
+    STATUS_IN_TRANSACTION = psycopg.pq.TransactionStatus.INTRANS
 except ImportError:
-    PostgresJson = None
-    STATUS_IN_TRANSACTION = None
+    try:
+        from psycopg2._json import Json as PostgresJson
+        from psycopg2.extensions import STATUS_IN_TRANSACTION
+    except ImportError:
+        PostgresJson = None
+        STATUS_IN_TRANSACTION = None
 
 # Prevents SQL queries from being sent to the DB. It's used
 # by the TemplatePanel to prevent the toolbar from issuing
 # additional queries.
 allow_sql = contextvars.ContextVar("debug-toolbar-allow-sql", default=True)
 
 
@@ -116,19 +122,27 @@
             return repr(element)
 
     def _quote_params(self, params):
         if not params:
             return params
         if isinstance(params, dict):
             return {key: self._quote_expr(value) for key, value in params.items()}
+        if isinstance(params, tuple):
+            return tuple(self._quote_expr(p) for p in params)
         return [self._quote_expr(p) for p in params]
 
     def _decode(self, param):
         if PostgresJson and isinstance(param, PostgresJson):
-            return param.dumps(param.adapted)
+            # psycopg3
+            if hasattr(param, "obj"):
+                return param.dumps(param.obj)
+            # psycopg2
+            if hasattr(param, "adapted"):
+                return param.dumps(param.adapted)
+
         # If a sequence type, decode each element separately
         if isinstance(param, (tuple, list)):
             return [self._decode(element) for element in param]
 
         # If a dictionary type, decode each value separately
         if isinstance(param, dict):
             return {key: self._decode(value) for key, value in param.items()}
@@ -143,15 +157,15 @@
     def _record(self, method, sql, params):
         alias = self.db.alias
         vendor = self.db.vendor
 
         if vendor == "postgresql":
             # The underlying DB connection (as opposed to Django's wrapper)
             conn = self.db.connection
-            initial_conn_status = conn.status
+            initial_conn_status = conn.info.transaction_status
 
         start_time = time()
         try:
             return method(sql, params)
         finally:
             stop_time = time()
             duration = (stop_time - start_time) * 1000
@@ -160,15 +174,18 @@
                 _params = json.dumps(self._decode(params))
             except TypeError:
                 pass  # object not JSON serializable
             template_info = get_template_info()
 
             # Sql might be an object (such as psycopg Composed).
             # For logging purposes, make sure it's str.
-            sql = str(sql)
+            if vendor == "postgresql" and not isinstance(sql, str):
+                sql = sql.as_string(conn)
+            else:
+                sql = str(sql)
 
             params = {
                 "vendor": vendor,
                 "alias": alias,
                 "sql": self.db.ops.last_executed_query(
                     self.cursor, sql, self._quote_params(params)
                 ),
@@ -199,27 +216,27 @@
                 # a new transaction ID from logger.new_transaction_id().  If the query
                 # was in a transaction both before and after executing, make the
                 # assumption that it is the same transaction and get the current
                 # transaction ID from logger.current_transaction_id().  There is an edge
                 # case where Django can start a transaction before the first query
                 # executes, so in that case logger.current_transaction_id() will
                 # generate a new transaction ID since one does not already exist.
-                final_conn_status = conn.status
+                final_conn_status = conn.info.transaction_status
                 if final_conn_status == STATUS_IN_TRANSACTION:
                     if initial_conn_status == STATUS_IN_TRANSACTION:
                         trans_id = self.logger.current_transaction_id(alias)
                     else:
                         trans_id = self.logger.new_transaction_id(alias)
                 else:
                     trans_id = None
 
                 params.update(
                     {
                         "trans_id": trans_id,
-                        "trans_status": conn.get_transaction_status(),
+                        "trans_status": conn.info.transaction_status,
                         "iso_level": iso_level,
                     }
                 )
 
             # We keep `sql` to maintain backwards compatibility
             self.logger.record(**params)
```

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/panels/sql/utils.py` & `django_debug_toolbar-4.0.0/debug_toolbar/panels/sql/utils.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/panels/sql/views.py` & `django_debug_toolbar-4.0.0/debug_toolbar/panels/sql/views.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from django.http import HttpResponseBadRequest, JsonResponse
 from django.template.loader import render_to_string
 from django.views.decorators.csrf import csrf_exempt
 
-from debug_toolbar.decorators import require_show_toolbar
+from debug_toolbar.decorators import render_with_toolbar_language, require_show_toolbar
 from debug_toolbar.forms import SignedDataForm
 from debug_toolbar.panels.sql.forms import SQLSelectForm
 
 
 def get_signed_data(request):
     """Unpack a signed data form, if invalid returns None"""
     data = request.GET if request.method == "GET" else request.POST
@@ -14,14 +14,15 @@
     if signed_form.is_valid():
         return signed_form.verified_data()
     return None
 
 
 @csrf_exempt
 @require_show_toolbar
+@render_with_toolbar_language
 def sql_select(request):
     """Returns the output of the SQL SELECT statement"""
     verified_data = get_signed_data(request)
     if not verified_data:
         return HttpResponseBadRequest("Invalid signature")
     form = SQLSelectForm(verified_data)
 
@@ -43,14 +44,15 @@
         content = render_to_string("debug_toolbar/panels/sql_select.html", context)
         return JsonResponse({"content": content})
     return HttpResponseBadRequest("Form errors")
 
 
 @csrf_exempt
 @require_show_toolbar
+@render_with_toolbar_language
 def sql_explain(request):
     """Returns the output of the SQL EXPLAIN on the given query"""
     verified_data = get_signed_data(request)
     if not verified_data:
         return HttpResponseBadRequest("Invalid signature")
     form = SQLSelectForm(verified_data)
 
@@ -81,14 +83,15 @@
         content = render_to_string("debug_toolbar/panels/sql_explain.html", context)
         return JsonResponse({"content": content})
     return HttpResponseBadRequest("Form errors")
 
 
 @csrf_exempt
 @require_show_toolbar
+@render_with_toolbar_language
 def sql_profile(request):
     """Returns the output of running the SQL and getting the profiling statistics"""
     verified_data = get_signed_data(request)
     if not verified_data:
         return HttpResponseBadRequest("Invalid signature")
     form = SQLSelectForm(verified_data)
```

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/panels/templates/panel.py` & `django_debug_toolbar-4.0.0/debug_toolbar/panels/templates/panel.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/panels/templates/views.py` & `django_debug_toolbar-4.0.0/debug_toolbar/panels/templates/views.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from django.core import signing
 from django.http import HttpResponseBadRequest, JsonResponse
 from django.template import Origin, TemplateDoesNotExist
 from django.template.engine import Engine
 from django.template.loader import render_to_string
 from django.utils.html import format_html, mark_safe
 
-from debug_toolbar.decorators import require_show_toolbar
+from debug_toolbar.decorators import render_with_toolbar_language, require_show_toolbar
 
 
 @require_show_toolbar
+@render_with_toolbar_language
 def template_source(request):
     """
     Return the source of a template, syntax-highlighted by Pygments if
     it's available.
     """
     template_origin_name = request.GET.get("template_origin")
     if template_origin_name is None:
```

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/static/debug_toolbar/css/toolbar.css` & `django_debug_toolbar-4.0.0/debug_toolbar/static/debug_toolbar/css/toolbar.css`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/static/debug_toolbar/js/history.js` & `django_debug_toolbar-4.0.0/debug_toolbar/static/debug_toolbar/js/history.js`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/static/debug_toolbar/js/timer.js` & `django_debug_toolbar-4.0.0/debug_toolbar/static/debug_toolbar/js/timer.js`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/static/debug_toolbar/js/toolbar.js` & `django_debug_toolbar-4.0.0/debug_toolbar/static/debug_toolbar/js/toolbar.js`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/static/debug_toolbar/js/utils.js` & `django_debug_toolbar-4.0.0/debug_toolbar/static/debug_toolbar/js/utils.js`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/templates/debug_toolbar/base.html` & `django_debug_toolbar-4.0.0/debug_toolbar/templates/debug_toolbar/base.html`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/templates/debug_toolbar/redirect.html` & `django_debug_toolbar-4.0.0/debug_toolbar/templates/debug_toolbar/redirect.html`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/templates/debug_toolbar/includes/panel_button.html` & `django_debug_toolbar-4.0.0/debug_toolbar/templates/debug_toolbar/includes/panel_button.html`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/templates/debug_toolbar/includes/panel_content.html` & `django_debug_toolbar-4.0.0/debug_toolbar/templates/debug_toolbar/includes/panel_content.html`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/templates/debug_toolbar/panels/cache.html` & `django_debug_toolbar-4.0.0/debug_toolbar/templates/debug_toolbar/panels/cache.html`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/templates/debug_toolbar/panels/headers.html` & `django_debug_toolbar-4.0.0/debug_toolbar/templates/debug_toolbar/panels/headers.html`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/templates/debug_toolbar/panels/history.html` & `django_debug_toolbar-4.0.0/debug_toolbar/templates/debug_toolbar/panels/history.html`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/templates/debug_toolbar/panels/history_tr.html` & `django_debug_toolbar-4.0.0/debug_toolbar/templates/debug_toolbar/panels/history_tr.html`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/templates/debug_toolbar/panels/profiling.html` & `django_debug_toolbar-4.0.0/debug_toolbar/templates/debug_toolbar/panels/profiling.html`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/templates/debug_toolbar/panels/request.html` & `django_debug_toolbar-4.0.0/debug_toolbar/templates/debug_toolbar/panels/request.html`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/templates/debug_toolbar/panels/request_variables.html` & `django_debug_toolbar-4.0.0/debug_toolbar/templates/debug_toolbar/panels/request_variables.html`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/templates/debug_toolbar/panels/sql.html` & `django_debug_toolbar-4.0.0/debug_toolbar/templates/debug_toolbar/panels/sql.html`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/templates/debug_toolbar/panels/sql_explain.html` & `django_debug_toolbar-4.0.0/debug_toolbar/templates/debug_toolbar/panels/sql_explain.html`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/templates/debug_toolbar/panels/sql_profile.html` & `django_debug_toolbar-4.0.0/debug_toolbar/templates/debug_toolbar/panels/sql_profile.html`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/templates/debug_toolbar/panels/sql_select.html` & `django_debug_toolbar-4.0.0/debug_toolbar/templates/debug_toolbar/panels/sql_select.html`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/templates/debug_toolbar/panels/staticfiles.html` & `django_debug_toolbar-4.0.0/debug_toolbar/templates/debug_toolbar/panels/staticfiles.html`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/templates/debug_toolbar/panels/templates.html` & `django_debug_toolbar-4.0.0/debug_toolbar/templates/debug_toolbar/panels/templates.html`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-3.8.1/debug_toolbar/templates/debug_toolbar/panels/timer.html` & `django_debug_toolbar-4.0.0/debug_toolbar/templates/debug_toolbar/panels/timer.html`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-3.8.1/LICENSE` & `django_debug_toolbar-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-3.8.1/README.rst` & `django_debug_toolbar-4.0.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
 .. image:: https://raw.github.com/jazzband/django-debug-toolbar/main/example/django-debug-toolbar.png
    :alt: Django Debug Toolbar screenshot
 
 In addition to the built-in panels, a number of third-party panels are
 contributed by the community.
 
-The current stable version of the Debug Toolbar is 3.8.1. It works on
+The current stable version of the Debug Toolbar is 4.0.0. It works on
 Django ≥ 3.2.4.
 
 Documentation, including installation and configuration instructions, is
 available at https://django-debug-toolbar.readthedocs.io/.
 
 The Django Debug Toolbar is released under the BSD license, like Django
 itself. If you like it, please consider contributing!
```

### Comparing `django_debug_toolbar-3.8.1/pyproject.toml` & `django_debug_toolbar-4.0.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,53 +1,68 @@
 [build-system]
 build-backend = "hatchling.build"
 requires = [
   "hatchling",
 ]
 
 [project]
-name = "django_debug_toolbar"
+name = "django-debug-toolbar"
 description = "A configurable set of panels that display various debug information about the current request/response."
 readme = "README.rst"
 license = {text = "BSD-3-Clause"}
 authors = [
     { name = "Rob Hudson" },
 ]
-requires-python = ">=3.7"
-dependencies = [
-  "Django>=3.2.4",
-  "sqlparse>=0.2",
-]
-dynamic = [
-  "version",
-]
+requires-python = ">=3.8"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Web Environment",
     "Framework :: Django",
     "Framework :: Django :: 3.2",
     "Framework :: Django :: 4.0",
     "Framework :: Django :: 4.1",
+    "Framework :: Django :: 4.2",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: BSD License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
+dynamic = [
+  "version",
+]
+dependencies = [
+  "Django>=3.2.4",
+  "sqlparse>=0.2",
+]
 [project.urls]
 Download = "https://pypi.org/project/django-debug-toolbar/"
 Homepage = "https://github.com/jazzband/django-debug-toolbar"
 
+[tool.hatch.build.targets.sdist]
+include = [
+    "/debug_toolbar",
+    "/CONTRIBUTING.md",
+]
+
+[tool.hatch.build.targets.wheel]
+packages = ["debug_toolbar"]
+
+[tool.hatch.version]
+path = "debug_toolbar/__init__.py"
+
+[tool.isort]
+combine_as_imports = true
+profile = "black"
 
 [tool.coverage.html]
 skip_covered = true
 skip_empty = true
 
 [tool.coverage.run]
 branch = true
@@ -57,23 +72,7 @@
 [tool.coverage.paths]
 source = ["src", ".tox/*/site-packages"]
 
 [tool.coverage.report]
 # Update coverage badge link in README.rst when fail_under changes
 fail_under = 93
 show_missing = true
-
-[tool.hatch.build.targets.sdist]
-include = [
-    "/debug_toolbar",
-    "/CONTRIBUTING.md",
-]
-
-[tool.hatch.build.targets.wheel]
-packages = ["debug_toolbar"]
-
-[tool.hatch.version]
-path = "debug_toolbar/__init__.py"
-
-[tool.isort]
-combine_as_imports = true
-profile = "black"
```

### Comparing `django_debug_toolbar-3.8.1/PKG-INFO` & `django_debug_toolbar-4.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 Metadata-Version: 2.1
-Name: django_debug_toolbar
-Version: 3.8.1
+Name: django-debug-toolbar
+Version: 4.0.0
 Summary: A configurable set of panels that display various debug information about the current request/response.
 Project-URL: Download, https://pypi.org/project/django-debug-toolbar/
 Project-URL: Homepage, https://github.com/jazzband/django-debug-toolbar
 Author: Rob Hudson
 License: BSD-3-Clause
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Requires-Dist: django>=3.2.4
 Requires-Dist: sqlparse>=0.2
 Description-Content-Type: text/x-rst
 
 =====================================
 Django Debug Toolbar |latest-version|
 =====================================
@@ -72,15 +72,15 @@
 
 .. image:: https://raw.github.com/jazzband/django-debug-toolbar/main/example/django-debug-toolbar.png
    :alt: Django Debug Toolbar screenshot
 
 In addition to the built-in panels, a number of third-party panels are
 contributed by the community.
 
-The current stable version of the Debug Toolbar is 3.8.1. It works on
+The current stable version of the Debug Toolbar is 4.0.0. It works on
 Django ≥ 3.2.4.
 
 Documentation, including installation and configuration instructions, is
 available at https://django-debug-toolbar.readthedocs.io/.
 
 The Django Debug Toolbar is released under the BSD license, like Django
 itself. If you like it, please consider contributing!
```

