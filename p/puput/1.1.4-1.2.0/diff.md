# Comparing `tmp/puput-1.1.4.tar.gz` & `tmp/puput-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/puput-1.1.4.tar", last modified: Wed Dec 14 14:59:25 2022, max compression
+gzip compressed data, was "dist/puput-1.2.0.tar", last modified: Fri Dec 16 09:24:45 2022, max compression
```

## Comparing `puput-1.1.4.tar` & `puput-1.2.0.tar`

### file list

```diff
@@ -1,148 +1,148 @@
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-14 14:59:25.021893 puput-1.1.4/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      214 2022-12-07 09:41:08.000000 puput-1.1.4/AUTHORS
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     4253 2022-12-14 14:36:35.000000 puput-1.1.4/CHANGELOG
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1063 2022-12-07 09:41:08.000000 puput-1.1.4/LICENSE
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      264 2022-12-07 09:41:08.000000 puput-1.1.4/MANIFEST.in
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     3676 2022-12-14 14:59:25.021893 puput-1.1.4/PKG-INFO
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     2753 2022-12-14 11:49:38.000000 puput-1.1.4/README.rst
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-14 14:59:24.981893 puput-1.1.4/puput/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      650 2022-12-14 11:53:14.000000 puput-1.1.4/puput/__init__.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     4931 2022-12-07 09:41:08.000000 puput-1.1.4/puput/abstracts.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      234 2022-12-07 09:41:08.000000 puput-1.1.4/puput/apps.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     2217 2022-12-07 09:41:08.000000 puput-1.1.4/puput/comments.py
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-14 14:59:24.981893 puput-1.1.4/puput/conf/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      553 2022-12-07 09:41:08.000000 puput-1.1.4/puput/conf/__init__.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)       66 2022-12-07 09:41:08.000000 puput-1.1.4/puput/conf/defaults.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     3172 2022-12-07 09:41:08.000000 puput-1.1.4/puput/feeds.py
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-14 14:59:24.969893 puput-1.1.4/puput/locale/
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-14 14:59:24.965893 puput-1.1.4/puput/locale/ar/
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-14 14:59:24.985893 puput-1.1.4/puput/locale/ar/LC_MESSAGES/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     4400 2022-12-07 09:41:08.000000 puput-1.1.4/puput/locale/ar/LC_MESSAGES/django.mo
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     5912 2022-12-07 09:41:08.000000 puput-1.1.4/puput/locale/ar/LC_MESSAGES/django.po
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-14 14:59:24.965893 puput-1.1.4/puput/locale/ca/
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-14 14:59:24.985893 puput-1.1.4/puput/locale/ca/LC_MESSAGES/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     3278 2022-12-07 09:41:08.000000 puput-1.1.4/puput/locale/ca/LC_MESSAGES/django.mo
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     4949 2022-12-07 09:41:08.000000 puput-1.1.4/puput/locale/ca/LC_MESSAGES/django.po
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-14 14:59:24.965893 puput-1.1.4/puput/locale/de/
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-14 14:59:24.985893 puput-1.1.4/puput/locale/de/LC_MESSAGES/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     3323 2022-12-07 09:41:08.000000 puput-1.1.4/puput/locale/de/LC_MESSAGES/django.mo
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     4974 2022-12-07 09:41:08.000000 puput-1.1.4/puput/locale/de/LC_MESSAGES/django.po
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-14 14:59:24.965893 puput-1.1.4/puput/locale/en/
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-14 14:59:24.985893 puput-1.1.4/puput/locale/en/LC_MESSAGES/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      378 2022-12-07 09:41:08.000000 puput-1.1.4/puput/locale/en/LC_MESSAGES/django.mo
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     3975 2022-12-07 09:41:08.000000 puput-1.1.4/puput/locale/en/LC_MESSAGES/django.po
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-14 14:59:24.965893 puput-1.1.4/puput/locale/es/
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-14 14:59:24.989893 puput-1.1.4/puput/locale/es/LC_MESSAGES/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     3025 2022-12-07 09:41:08.000000 puput-1.1.4/puput/locale/es/LC_MESSAGES/django.mo
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     4909 2022-12-07 09:41:08.000000 puput-1.1.4/puput/locale/es/LC_MESSAGES/django.po
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-14 14:59:24.965893 puput-1.1.4/puput/locale/fr/
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-14 14:59:24.989893 puput-1.1.4/puput/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     3187 2022-12-07 09:41:08.000000 puput-1.1.4/puput/locale/fr/LC_MESSAGES/django.mo
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     5029 2022-12-07 09:41:08.000000 puput-1.1.4/puput/locale/fr/LC_MESSAGES/django.po
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-14 14:59:24.965893 puput-1.1.4/puput/locale/it/
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-14 14:59:24.989893 puput-1.1.4/puput/locale/it/LC_MESSAGES/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     3299 2022-12-07 09:41:08.000000 puput-1.1.4/puput/locale/it/LC_MESSAGES/django.mo
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     4970 2022-12-07 09:41:08.000000 puput-1.1.4/puput/locale/it/LC_MESSAGES/django.po
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-14 14:59:24.969893 puput-1.1.4/puput/locale/ja/
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-14 14:59:24.989893 puput-1.1.4/puput/locale/ja/LC_MESSAGES/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     3789 2022-12-07 09:41:08.000000 puput-1.1.4/puput/locale/ja/LC_MESSAGES/django.mo
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     5365 2022-12-07 09:41:08.000000 puput-1.1.4/puput/locale/ja/LC_MESSAGES/django.po
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-14 14:59:24.969893 puput-1.1.4/puput/locale/nl/
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-14 14:59:24.993893 puput-1.1.4/puput/locale/nl/LC_MESSAGES/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      421 2022-12-07 09:41:08.000000 puput-1.1.4/puput/locale/nl/LC_MESSAGES/django.mo
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     4022 2022-12-07 09:41:08.000000 puput-1.1.4/puput/locale/nl/LC_MESSAGES/django.po
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-14 14:59:24.969893 puput-1.1.4/puput/locale/pl/
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-14 14:59:24.993893 puput-1.1.4/puput/locale/pl/LC_MESSAGES/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     3432 2022-12-07 09:41:08.000000 puput-1.1.4/puput/locale/pl/LC_MESSAGES/django.mo
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     5006 2022-12-07 09:41:08.000000 puput-1.1.4/puput/locale/pl/LC_MESSAGES/django.po
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-14 14:59:24.969893 puput-1.1.4/puput/locale/pt_BR/
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-14 14:59:24.993893 puput-1.1.4/puput/locale/pt_BR/LC_MESSAGES/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     3319 2022-12-07 09:41:08.000000 puput-1.1.4/puput/locale/pt_BR/LC_MESSAGES/django.mo
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     5053 2022-12-07 09:41:08.000000 puput-1.1.4/puput/locale/pt_BR/LC_MESSAGES/django.po
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-14 14:59:24.969893 puput-1.1.4/puput/locale/pt_PT/
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-14 14:59:24.993893 puput-1.1.4/puput/locale/pt_PT/LC_MESSAGES/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      378 2022-12-07 09:41:08.000000 puput-1.1.4/puput/locale/pt_PT/LC_MESSAGES/django.mo
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     3975 2022-12-07 09:41:08.000000 puput-1.1.4/puput/locale/pt_PT/LC_MESSAGES/django.po
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-14 14:59:24.969893 puput-1.1.4/puput/locale/ru/
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-14 14:59:24.993893 puput-1.1.4/puput/locale/ru/LC_MESSAGES/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     3249 2022-12-07 09:41:08.000000 puput-1.1.4/puput/locale/ru/LC_MESSAGES/django.mo
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     5278 2022-12-07 09:41:08.000000 puput-1.1.4/puput/locale/ru/LC_MESSAGES/django.po
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-14 14:59:24.997893 puput-1.1.4/puput/management/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)        0 2022-12-07 09:41:08.000000 puput-1.1.4/puput/management/__init__.py
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-14 14:59:24.997893 puput-1.1.4/puput/management/commands/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)        0 2022-12-07 09:41:08.000000 puput-1.1.4/puput/management/commands/__init__.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1142 2022-12-07 09:41:08.000000 puput-1.1.4/puput/management/commands/puput_initial_data.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      966 2022-12-07 09:41:08.000000 puput-1.1.4/puput/managers.py
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-14 14:59:24.997893 puput-1.1.4/puput/migrations/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     7008 2022-12-07 09:41:08.000000 puput-1.1.4/puput/migrations/0001_initial.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1504 2022-12-07 09:41:08.000000 puput-1.1.4/puput/migrations/0002_auto_20150919_0925.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      441 2022-12-07 09:41:08.000000 puput-1.1.4/puput/migrations/0003_add_short_feed_description_to_blog_page.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      521 2022-12-07 09:41:08.000000 puput-1.1.4/puput/migrations/0004_auto_20170912_0928.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      517 2022-12-07 09:41:08.000000 puput-1.1.4/puput/migrations/0005_blogpage_main_color.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)        0 2022-12-07 09:41:08.000000 puput-1.1.4/puput/migrations/__init__.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     5695 2022-12-07 09:41:08.000000 puput-1.1.4/puput/models.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     3332 2022-12-14 11:49:38.000000 puput-1.1.4/puput/routes.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      632 2022-12-07 09:41:08.000000 puput-1.1.4/puput/signals.py
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-14 14:59:24.969893 puput-1.1.4/puput/static/
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-14 14:59:25.001893 puput-1.1.4/puput/static/colorful/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      111 2022-12-07 09:41:08.000000 puput-1.1.4/puput/static/colorful/arrow.gif
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      965 2022-12-07 09:41:08.000000 puput-1.1.4/puput/static/colorful/colorPicker.css
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-14 14:59:24.969893 puput-1.1.4/puput/static/puput/
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-14 14:59:25.001893 puput-1.1.4/puput/static/puput/css/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)   110143 2022-12-07 09:41:08.000000 puput-1.1.4/puput/static/puput/css/bootstrap.min.css
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    21984 2022-12-07 09:41:08.000000 puput-1.1.4/puput/static/puput/css/font-awesome.min.css
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    10929 2022-12-07 09:41:08.000000 puput-1.1.4/puput/static/puput/css/puput.css
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-14 14:59:25.005893 puput-1.1.4/puput/static/puput/fonts/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    85908 2022-12-07 09:41:08.000000 puput-1.1.4/puput/static/puput/fonts/FontAwesome.otf
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    56006 2022-12-07 09:41:08.000000 puput-1.1.4/puput/static/puput/fonts/fontawesome-webfont.eot
--rw-rw-r--   0 carlos    (1000) carlos    (1000)   287007 2022-12-07 09:41:08.000000 puput-1.1.4/puput/static/puput/fonts/fontawesome-webfont.svg
--rw-rw-r--   0 carlos    (1000) carlos    (1000)   112160 2022-12-07 09:41:08.000000 puput-1.1.4/puput/static/puput/fonts/fontawesome-webfont.ttf
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    65452 2022-12-07 09:41:08.000000 puput-1.1.4/puput/static/puput/fonts/fontawesome-webfont.woff
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-14 14:59:25.009893 puput-1.1.4/puput/static/puput/js/
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-14 14:59:25.009893 puput-1.1.4/puput/static/puput/js/comments/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      103 2022-12-07 09:41:08.000000 puput-1.1.4/puput/static/puput/js/comments/disqus.js
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      376 2022-12-07 09:41:08.000000 puput-1.1.4/puput/static/puput/js/comments/update_entry_comments.js
--rwxrwxr-x   0 carlos    (1000) carlos    (1000)    93868 2022-12-07 09:41:08.000000 puput-1.1.4/puput/static/puput/js/jquery.min.js
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     3285 2022-12-07 09:41:08.000000 puput-1.1.4/puput/static/puput/js/js.cookie.js
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      558 2022-12-07 09:41:08.000000 puput-1.1.4/puput/static/puput/js/puput.js
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-14 14:59:25.009893 puput-1.1.4/puput/templates/
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-14 14:59:25.009893 puput-1.1.4/puput/templates/el_pagination/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)       87 2022-12-07 09:41:08.000000 puput-1.1.4/puput/templates/el_pagination/current_link.html
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      159 2022-12-07 09:41:08.000000 puput-1.1.4/puput/templates/el_pagination/page_link.html
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      409 2022-12-07 09:41:08.000000 puput-1.1.4/puput/templates/el_pagination/show_more.html
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      117 2022-12-07 09:41:08.000000 puput-1.1.4/puput/templates/el_pagination/show_pages.html
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-14 14:59:25.013893 puput-1.1.4/puput/templates/puput/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     5957 2022-12-07 09:41:08.000000 puput-1.1.4/puput/templates/puput/base.html
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     4098 2022-12-07 09:41:08.000000 puput-1.1.4/puput/templates/puput/blog_page.html
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-14 14:59:25.017893 puput-1.1.4/puput/templates/puput/comments/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1127 2022-12-07 09:41:08.000000 puput-1.1.4/puput/templates/puput/comments/disqus.html
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      136 2022-12-07 09:41:08.000000 puput-1.1.4/puput/templates/puput/comments/django_comments.html
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      901 2022-12-07 09:41:08.000000 puput-1.1.4/puput/templates/puput/entry_links.html
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     3613 2022-12-07 09:41:08.000000 puput-1.1.4/puput/templates/puput/entry_page.html
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      150 2022-12-07 09:41:08.000000 puput-1.1.4/puput/templates/puput/entry_page_header.html
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1235 2022-12-07 09:41:08.000000 puput-1.1.4/puput/templates/puput/related_entries.html
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-14 14:59:25.017893 puput-1.1.4/puput/templates/puput/tags/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      977 2022-12-07 09:41:08.000000 puput-1.1.4/puput/templates/puput/tags/archives_list.html
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      303 2022-12-07 09:41:08.000000 puput-1.1.4/puput/templates/puput/tags/categories_list.html
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1215 2022-12-07 09:41:08.000000 puput-1.1.4/puput/templates/puput/tags/entries_list.html
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      121 2022-12-07 09:41:08.000000 puput-1.1.4/puput/templates/puput/tags/post_to_linkedin.html
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      278 2022-12-07 09:41:08.000000 puput-1.1.4/puput/templates/puput/tags/tags_list.html
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      385 2022-12-07 09:41:08.000000 puput-1.1.4/puput/templates/sitemap.xml
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-14 14:59:24.973894 puput-1.1.4/puput/templates/wagtailadmin/
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-14 14:59:25.017893 puput-1.1.4/puput/templates/wagtailadmin/pages/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      541 2022-12-07 09:41:08.000000 puput-1.1.4/puput/templates/wagtailadmin/pages/_editor_css.html
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-14 14:59:25.021893 puput-1.1.4/puput/templatetags/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)        0 2022-12-07 09:41:08.000000 puput-1.1.4/puput/templatetags/__init__.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     4379 2022-12-07 09:41:08.000000 puput-1.1.4/puput/templatetags/puput_tags.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     3219 2022-12-07 09:41:08.000000 puput-1.1.4/puput/urls.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1729 2022-12-07 09:41:08.000000 puput-1.1.4/puput/utils.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     2834 2022-12-07 09:41:08.000000 puput-1.1.4/puput/views.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1802 2022-12-07 09:41:08.000000 puput-1.1.4/puput/wagtail_hooks.py
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-14 14:59:24.981893 puput-1.1.4/puput.egg-info/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     3676 2022-12-14 14:59:24.000000 puput-1.1.4/puput.egg-info/PKG-INFO
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     3352 2022-12-14 14:59:24.000000 puput-1.1.4/puput.egg-info/SOURCES.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)        1 2022-12-14 14:59:24.000000 puput-1.1.4/puput.egg-info/dependency_links.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      111 2022-12-14 14:59:24.000000 puput-1.1.4/puput.egg-info/requires.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)        6 2022-12-14 14:59:24.000000 puput-1.1.4/puput.egg-info/top_level.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)       38 2022-12-14 14:59:25.021893 puput-1.1.4/setup.cfg
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1832 2022-12-14 11:49:38.000000 puput-1.1.4/setup.py
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-16 09:24:45.018647 puput-1.2.0/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      214 2022-12-07 09:41:08.000000 puput-1.2.0/AUTHORS
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     4453 2022-12-16 09:20:08.000000 puput-1.2.0/CHANGELOG
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1063 2022-12-07 09:41:08.000000 puput-1.2.0/LICENSE
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      264 2022-12-07 09:41:08.000000 puput-1.2.0/MANIFEST.in
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     3688 2022-12-16 09:24:45.018647 puput-1.2.0/PKG-INFO
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     2753 2022-12-14 11:49:38.000000 puput-1.2.0/README.rst
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-16 09:24:44.994646 puput-1.2.0/puput/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      650 2022-12-16 09:20:08.000000 puput-1.2.0/puput/__init__.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     5025 2022-12-16 08:22:36.000000 puput-1.2.0/puput/abstracts.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      234 2022-12-16 08:22:36.000000 puput-1.2.0/puput/apps.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     2159 2022-12-16 08:22:36.000000 puput-1.2.0/puput/comments.py
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-16 09:24:44.994646 puput-1.2.0/puput/conf/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      553 2022-12-07 09:41:08.000000 puput-1.2.0/puput/conf/__init__.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       66 2022-12-16 08:22:36.000000 puput-1.2.0/puput/conf/defaults.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     3152 2022-12-16 08:22:36.000000 puput-1.2.0/puput/feeds.py
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-16 09:24:44.982645 puput-1.2.0/puput/locale/
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-16 09:24:44.978645 puput-1.2.0/puput/locale/ar/
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-16 09:24:44.994646 puput-1.2.0/puput/locale/ar/LC_MESSAGES/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     4400 2022-12-07 09:41:08.000000 puput-1.2.0/puput/locale/ar/LC_MESSAGES/django.mo
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     5912 2022-12-07 09:41:08.000000 puput-1.2.0/puput/locale/ar/LC_MESSAGES/django.po
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-16 09:24:44.978645 puput-1.2.0/puput/locale/ca/
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-16 09:24:44.998646 puput-1.2.0/puput/locale/ca/LC_MESSAGES/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     3278 2022-12-07 09:41:08.000000 puput-1.2.0/puput/locale/ca/LC_MESSAGES/django.mo
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     4949 2022-12-07 09:41:08.000000 puput-1.2.0/puput/locale/ca/LC_MESSAGES/django.po
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-16 09:24:44.978645 puput-1.2.0/puput/locale/de/
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-16 09:24:44.998646 puput-1.2.0/puput/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     3323 2022-12-07 09:41:08.000000 puput-1.2.0/puput/locale/de/LC_MESSAGES/django.mo
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     4974 2022-12-07 09:41:08.000000 puput-1.2.0/puput/locale/de/LC_MESSAGES/django.po
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-16 09:24:44.978645 puput-1.2.0/puput/locale/en/
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-16 09:24:44.998646 puput-1.2.0/puput/locale/en/LC_MESSAGES/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      378 2022-12-07 09:41:08.000000 puput-1.2.0/puput/locale/en/LC_MESSAGES/django.mo
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     3975 2022-12-07 09:41:08.000000 puput-1.2.0/puput/locale/en/LC_MESSAGES/django.po
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-16 09:24:44.978645 puput-1.2.0/puput/locale/es/
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-16 09:24:44.998646 puput-1.2.0/puput/locale/es/LC_MESSAGES/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     3025 2022-12-07 09:41:08.000000 puput-1.2.0/puput/locale/es/LC_MESSAGES/django.mo
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     4909 2022-12-07 09:41:08.000000 puput-1.2.0/puput/locale/es/LC_MESSAGES/django.po
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-16 09:24:44.978645 puput-1.2.0/puput/locale/fr/
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-16 09:24:44.998646 puput-1.2.0/puput/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     3187 2022-12-07 09:41:08.000000 puput-1.2.0/puput/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     5029 2022-12-07 09:41:08.000000 puput-1.2.0/puput/locale/fr/LC_MESSAGES/django.po
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-16 09:24:44.978645 puput-1.2.0/puput/locale/it/
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-16 09:24:44.998646 puput-1.2.0/puput/locale/it/LC_MESSAGES/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     3299 2022-12-07 09:41:08.000000 puput-1.2.0/puput/locale/it/LC_MESSAGES/django.mo
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     4970 2022-12-07 09:41:08.000000 puput-1.2.0/puput/locale/it/LC_MESSAGES/django.po
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-16 09:24:44.982645 puput-1.2.0/puput/locale/ja/
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-16 09:24:44.998646 puput-1.2.0/puput/locale/ja/LC_MESSAGES/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     3789 2022-12-07 09:41:08.000000 puput-1.2.0/puput/locale/ja/LC_MESSAGES/django.mo
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     5365 2022-12-07 09:41:08.000000 puput-1.2.0/puput/locale/ja/LC_MESSAGES/django.po
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-16 09:24:44.982645 puput-1.2.0/puput/locale/nl/
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-16 09:24:45.002646 puput-1.2.0/puput/locale/nl/LC_MESSAGES/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      421 2022-12-07 09:41:08.000000 puput-1.2.0/puput/locale/nl/LC_MESSAGES/django.mo
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     4022 2022-12-07 09:41:08.000000 puput-1.2.0/puput/locale/nl/LC_MESSAGES/django.po
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-16 09:24:44.982645 puput-1.2.0/puput/locale/pl/
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-16 09:24:45.002646 puput-1.2.0/puput/locale/pl/LC_MESSAGES/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     3432 2022-12-07 09:41:08.000000 puput-1.2.0/puput/locale/pl/LC_MESSAGES/django.mo
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     5006 2022-12-07 09:41:08.000000 puput-1.2.0/puput/locale/pl/LC_MESSAGES/django.po
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-16 09:24:44.982645 puput-1.2.0/puput/locale/pt_BR/
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-16 09:24:45.002646 puput-1.2.0/puput/locale/pt_BR/LC_MESSAGES/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     3319 2022-12-07 09:41:08.000000 puput-1.2.0/puput/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     5053 2022-12-07 09:41:08.000000 puput-1.2.0/puput/locale/pt_BR/LC_MESSAGES/django.po
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-16 09:24:44.982645 puput-1.2.0/puput/locale/pt_PT/
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-16 09:24:45.002646 puput-1.2.0/puput/locale/pt_PT/LC_MESSAGES/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      378 2022-12-07 09:41:08.000000 puput-1.2.0/puput/locale/pt_PT/LC_MESSAGES/django.mo
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     3975 2022-12-07 09:41:08.000000 puput-1.2.0/puput/locale/pt_PT/LC_MESSAGES/django.po
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-16 09:24:44.982645 puput-1.2.0/puput/locale/ru/
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-16 09:24:45.002646 puput-1.2.0/puput/locale/ru/LC_MESSAGES/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     3249 2022-12-07 09:41:08.000000 puput-1.2.0/puput/locale/ru/LC_MESSAGES/django.mo
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     5278 2022-12-07 09:41:08.000000 puput-1.2.0/puput/locale/ru/LC_MESSAGES/django.po
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-16 09:24:45.002646 puput-1.2.0/puput/management/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)        0 2022-12-07 09:41:08.000000 puput-1.2.0/puput/management/__init__.py
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-16 09:24:45.006646 puput-1.2.0/puput/management/commands/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)        0 2022-12-07 09:41:08.000000 puput-1.2.0/puput/management/commands/__init__.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1118 2022-12-16 08:22:36.000000 puput-1.2.0/puput/management/commands/puput_initial_data.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      964 2022-12-16 08:22:36.000000 puput-1.2.0/puput/managers.py
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-16 09:24:45.006646 puput-1.2.0/puput/migrations/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     7008 2022-12-07 09:41:08.000000 puput-1.2.0/puput/migrations/0001_initial.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1504 2022-12-07 09:41:08.000000 puput-1.2.0/puput/migrations/0002_auto_20150919_0925.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      441 2022-12-07 09:41:08.000000 puput-1.2.0/puput/migrations/0003_add_short_feed_description_to_blog_page.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      521 2022-12-07 09:41:08.000000 puput-1.2.0/puput/migrations/0004_auto_20170912_0928.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      517 2022-12-07 09:41:08.000000 puput-1.2.0/puput/migrations/0005_blogpage_main_color.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)        0 2022-12-07 09:41:08.000000 puput-1.2.0/puput/migrations/__init__.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     5736 2022-12-16 08:22:36.000000 puput-1.2.0/puput/models.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     3331 2022-12-16 08:22:36.000000 puput-1.2.0/puput/routes.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      632 2022-12-16 08:22:36.000000 puput-1.2.0/puput/signals.py
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-16 09:24:44.982645 puput-1.2.0/puput/static/
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-16 09:24:45.006646 puput-1.2.0/puput/static/colorful/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      111 2022-12-07 09:41:08.000000 puput-1.2.0/puput/static/colorful/arrow.gif
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      965 2022-12-07 09:41:08.000000 puput-1.2.0/puput/static/colorful/colorPicker.css
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-16 09:24:44.982645 puput-1.2.0/puput/static/puput/
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-16 09:24:45.010646 puput-1.2.0/puput/static/puput/css/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)   110143 2022-12-07 09:41:08.000000 puput-1.2.0/puput/static/puput/css/bootstrap.min.css
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    21984 2022-12-07 09:41:08.000000 puput-1.2.0/puput/static/puput/css/font-awesome.min.css
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    10929 2022-12-07 09:41:08.000000 puput-1.2.0/puput/static/puput/css/puput.css
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-16 09:24:45.010646 puput-1.2.0/puput/static/puput/fonts/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    85908 2022-12-07 09:41:08.000000 puput-1.2.0/puput/static/puput/fonts/FontAwesome.otf
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    56006 2022-12-07 09:41:08.000000 puput-1.2.0/puput/static/puput/fonts/fontawesome-webfont.eot
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)   287007 2022-12-07 09:41:08.000000 puput-1.2.0/puput/static/puput/fonts/fontawesome-webfont.svg
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)   112160 2022-12-07 09:41:08.000000 puput-1.2.0/puput/static/puput/fonts/fontawesome-webfont.ttf
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    65452 2022-12-07 09:41:08.000000 puput-1.2.0/puput/static/puput/fonts/fontawesome-webfont.woff
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-16 09:24:45.014646 puput-1.2.0/puput/static/puput/js/
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-16 09:24:45.014646 puput-1.2.0/puput/static/puput/js/comments/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      103 2022-12-07 09:41:08.000000 puput-1.2.0/puput/static/puput/js/comments/disqus.js
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      376 2022-12-07 09:41:08.000000 puput-1.2.0/puput/static/puput/js/comments/update_entry_comments.js
+-rwxrwxr-x   0 carlos    (1000) carlos    (1000)    93868 2022-12-07 09:41:08.000000 puput-1.2.0/puput/static/puput/js/jquery.min.js
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     3285 2022-12-07 09:41:08.000000 puput-1.2.0/puput/static/puput/js/js.cookie.js
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      558 2022-12-07 09:41:08.000000 puput-1.2.0/puput/static/puput/js/puput.js
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-16 09:24:45.014646 puput-1.2.0/puput/templates/
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-16 09:24:45.014646 puput-1.2.0/puput/templates/el_pagination/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       87 2022-12-07 09:41:08.000000 puput-1.2.0/puput/templates/el_pagination/current_link.html
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      159 2022-12-07 09:41:08.000000 puput-1.2.0/puput/templates/el_pagination/page_link.html
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      409 2022-12-07 09:41:08.000000 puput-1.2.0/puput/templates/el_pagination/show_more.html
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      117 2022-12-07 09:41:08.000000 puput-1.2.0/puput/templates/el_pagination/show_pages.html
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-16 09:24:45.018647 puput-1.2.0/puput/templates/puput/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     5957 2022-12-07 09:41:08.000000 puput-1.2.0/puput/templates/puput/base.html
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     4098 2022-12-07 09:41:08.000000 puput-1.2.0/puput/templates/puput/blog_page.html
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-16 09:24:45.018647 puput-1.2.0/puput/templates/puput/comments/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1127 2022-12-07 09:41:08.000000 puput-1.2.0/puput/templates/puput/comments/disqus.html
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      136 2022-12-07 09:41:08.000000 puput-1.2.0/puput/templates/puput/comments/django_comments.html
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      901 2022-12-07 09:41:08.000000 puput-1.2.0/puput/templates/puput/entry_links.html
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     3613 2022-12-07 09:41:08.000000 puput-1.2.0/puput/templates/puput/entry_page.html
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      150 2022-12-07 09:41:08.000000 puput-1.2.0/puput/templates/puput/entry_page_header.html
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1235 2022-12-07 09:41:08.000000 puput-1.2.0/puput/templates/puput/related_entries.html
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-16 09:24:45.018647 puput-1.2.0/puput/templates/puput/tags/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      977 2022-12-07 09:41:08.000000 puput-1.2.0/puput/templates/puput/tags/archives_list.html
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      303 2022-12-07 09:41:08.000000 puput-1.2.0/puput/templates/puput/tags/categories_list.html
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1215 2022-12-07 09:41:08.000000 puput-1.2.0/puput/templates/puput/tags/entries_list.html
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      121 2022-12-07 09:41:08.000000 puput-1.2.0/puput/templates/puput/tags/post_to_linkedin.html
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      278 2022-12-07 09:41:08.000000 puput-1.2.0/puput/templates/puput/tags/tags_list.html
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      385 2022-12-07 09:41:08.000000 puput-1.2.0/puput/templates/sitemap.xml
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-16 09:24:44.986646 puput-1.2.0/puput/templates/wagtailadmin/
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-16 09:24:45.018647 puput-1.2.0/puput/templates/wagtailadmin/pages/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      541 2022-12-07 09:41:08.000000 puput-1.2.0/puput/templates/wagtailadmin/pages/_editor_css.html
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-16 09:24:45.018647 puput-1.2.0/puput/templatetags/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)        0 2022-12-07 09:41:08.000000 puput-1.2.0/puput/templatetags/__init__.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     4351 2022-12-16 09:18:53.000000 puput-1.2.0/puput/templatetags/puput_tags.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     3147 2022-12-16 08:22:36.000000 puput-1.2.0/puput/urls.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1730 2022-12-16 08:22:36.000000 puput-1.2.0/puput/utils.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     2833 2022-12-16 08:22:36.000000 puput-1.2.0/puput/views.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1759 2022-12-16 08:22:36.000000 puput-1.2.0/puput/wagtail_hooks.py
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2022-12-16 09:24:44.994646 puput-1.2.0/puput.egg-info/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     3688 2022-12-16 09:24:44.000000 puput-1.2.0/puput.egg-info/PKG-INFO
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     3352 2022-12-16 09:24:44.000000 puput-1.2.0/puput.egg-info/SOURCES.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)        1 2022-12-16 09:24:44.000000 puput-1.2.0/puput.egg-info/dependency_links.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      111 2022-12-16 09:24:44.000000 puput-1.2.0/puput.egg-info/requires.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)        6 2022-12-16 09:24:44.000000 puput-1.2.0/puput.egg-info/top_level.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       38 2022-12-16 09:24:45.018647 puput-1.2.0/setup.cfg
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1844 2022-12-16 09:18:53.000000 puput-1.2.0/setup.py
```

### Comparing `puput-1.1.4/CHANGELOG` & `puput-1.2.0/CHANGELOG`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 Changelog
 =========
 
+1.2.0 (2022-12-16)
+----------
+* Add Wagtail 4 support. Drop Wagtail <3 support.
+* Drop Django <2.2 support.
+* Update requirements-test.
+* Update tox.
+* Fix: include Python 3.10 on setup classifiers.
+
 1.1.4 (2022-12-14)
 ------------------
 * Add Wagtail 3 support.
 * Add Python 3.10 support. Drop Python 3.6 support.
 * Remove travis.
 * Fix tests suite and apply flake8.
 * Updated some docs.
```

### Comparing `puput-1.1.4/LICENSE` & `puput-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `puput-1.1.4/PKG-INFO` & `puput-1.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: puput
-Version: 1.1.4
+Version: 1.2.0
 Summary: A Django blog app implemented in Wagtail.
 Home-page: http://github.com/APSL/puput
 Author: Marc Tudurí
 Author-email: marctc@gmail.com
 Keywords: django wagtail puput blog cms app
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS
 
 Puput
```

### Comparing `puput-1.1.4/README.rst` & `puput-1.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `puput-1.1.4/puput/__init__.py` & `puput-1.2.0/puput/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 __author__ = "Marc Tudurí"
 __email__ = "marctc@gmail.com"
-__version__ = "1.1.4"
+__version__ = "1.2.0"
 
 PUPUT_APPS = (
     # Wagtail apps
     "wagtail.contrib.legacy.richtext",
     "wagtail.core",
     "wagtail.admin",
     "wagtail.documents",
```

### Comparing `puput-1.1.4/puput/abstracts.py` & `puput-1.2.0/puput/abstracts.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,129 +1,137 @@
 import datetime
 
 from django.db import models
 from django.utils.translation import gettext_lazy as _
 
 from wagtail.admin.edit_handlers import FieldPanel, MultiFieldPanel, InlinePanel, PageChooserPanel
-from wagtail.images.edit_handlers import ImageChooserPanel
 from wagtail.core.fields import RichTextField
 from modelcluster.contrib.taggit import ClusterTaggableManager
 
 from colorful.fields import RGBColorField
 
 from .utils import get_image_model_path
 
 
 class BlogAbstract(models.Model):
     description = models.CharField(
-        verbose_name=_('Description'),
+        verbose_name=_("Description"),
         max_length=255,
         blank=True,
-        help_text=_("The blog description that will appear under the title.")
+        help_text=_("The blog description that will appear under the title."),
     )
     header_image = models.ForeignKey(
         get_image_model_path(),
-        verbose_name=_('Header image'),
+        verbose_name=_("Header image"),
         null=True,
         blank=True,
         on_delete=models.SET_NULL,
-        related_name='+'
+        related_name="+",
     )
 
-    main_color = RGBColorField(_('Blog Main Color'), default="#4D6AE0")
+    main_color = RGBColorField(_("Blog Main Color"), default="#4D6AE0")
 
-    display_comments = models.BooleanField(default=False, verbose_name=_('Display comments'))
-    display_categories = models.BooleanField(default=True, verbose_name=_('Display categories'))
-    display_tags = models.BooleanField(default=True, verbose_name=_('Display tags'))
-    display_popular_entries = models.BooleanField(default=True, verbose_name=_('Display popular entries'))
-    display_last_entries = models.BooleanField(default=True, verbose_name=_('Display last entries'))
-    display_archive = models.BooleanField(default=True, verbose_name=_('Display archive'))
+    display_comments = models.BooleanField(default=False, verbose_name=_("Display comments"))
+    display_categories = models.BooleanField(default=True, verbose_name=_("Display categories"))
+    display_tags = models.BooleanField(default=True, verbose_name=_("Display tags"))
+    display_popular_entries = models.BooleanField(default=True, verbose_name=_("Display popular entries"))
+    display_last_entries = models.BooleanField(default=True, verbose_name=_("Display last entries"))
+    display_archive = models.BooleanField(default=True, verbose_name=_("Display archive"))
 
     disqus_api_secret = models.TextField(blank=True)
     disqus_shortname = models.CharField(max_length=128, blank=True)
 
-    num_entries_page = models.IntegerField(default=5, verbose_name=_('Entries per page'))
-    num_last_entries = models.IntegerField(default=3, verbose_name=_('Last entries limit'))
-    num_popular_entries = models.IntegerField(default=3, verbose_name=_('Popular entries limit'))
-    num_tags_entry_header = models.IntegerField(default=5, verbose_name=_('Tags limit entry header'))
+    num_entries_page = models.IntegerField(default=5, verbose_name=_("Entries per page"))
+    num_last_entries = models.IntegerField(default=3, verbose_name=_("Last entries limit"))
+    num_popular_entries = models.IntegerField(default=3, verbose_name=_("Popular entries limit"))
+    num_tags_entry_header = models.IntegerField(default=5, verbose_name=_("Tags limit entry header"))
 
-    short_feed_description = models.BooleanField(default=True, verbose_name=_('Use short description in feeds'))
+    short_feed_description = models.BooleanField(default=True, verbose_name=_("Use short description in feeds"))
 
-    content_panels = [
-        FieldPanel('description', classname="full"),
-        ImageChooserPanel('header_image'),
-        FieldPanel('main_color')
-    ]
+    content_panels = [FieldPanel("description", classname="full"), FieldPanel("header_image"), FieldPanel("main_color")]
     settings_panels = [
-        MultiFieldPanel([
-            FieldPanel('display_categories'),
-            FieldPanel('display_tags'),
-            FieldPanel('display_popular_entries'),
-            FieldPanel('display_last_entries'),
-            FieldPanel('display_archive'),
-        ], heading=_("Widgets")),
-        MultiFieldPanel([
-            FieldPanel('num_entries_page'),
-            FieldPanel('num_last_entries'),
-            FieldPanel('num_popular_entries'),
-            FieldPanel('num_tags_entry_header'),
-        ], heading=_("Parameters")),
-        MultiFieldPanel([
-            FieldPanel('display_comments'),
-            FieldPanel('disqus_api_secret'),
-            FieldPanel('disqus_shortname'),
-        ], heading=_("Comments")),
-        MultiFieldPanel([
-            FieldPanel('short_feed_description'),
-        ], heading=_("Feeds")),
+        MultiFieldPanel(
+            [
+                FieldPanel("display_categories"),
+                FieldPanel("display_tags"),
+                FieldPanel("display_popular_entries"),
+                FieldPanel("display_last_entries"),
+                FieldPanel("display_archive"),
+            ],
+            heading=_("Widgets"),
+        ),
+        MultiFieldPanel(
+            [
+                FieldPanel("num_entries_page"),
+                FieldPanel("num_last_entries"),
+                FieldPanel("num_popular_entries"),
+                FieldPanel("num_tags_entry_header"),
+            ],
+            heading=_("Parameters"),
+        ),
+        MultiFieldPanel(
+            [
+                FieldPanel("display_comments"),
+                FieldPanel("disqus_api_secret"),
+                FieldPanel("disqus_shortname"),
+            ],
+            heading=_("Comments"),
+        ),
+        MultiFieldPanel(
+            [
+                FieldPanel("short_feed_description"),
+            ],
+            heading=_("Feeds"),
+        ),
     ]
 
     class Meta:
         abstract = True
 
 
 class EntryAbstract(models.Model):
-    body = RichTextField(verbose_name=_('body'))
-    tags = ClusterTaggableManager(through='puput.TagEntryPage', blank=True)
+    body = RichTextField(verbose_name=_("body"))
+    tags = ClusterTaggableManager(through="puput.TagEntryPage", blank=True)
     date = models.DateTimeField(verbose_name=_("Post date"), default=datetime.datetime.today)
     header_image = models.ForeignKey(
         get_image_model_path(),
-        verbose_name=_('Header image'),
+        verbose_name=_("Header image"),
         null=True,
         blank=True,
         on_delete=models.SET_NULL,
-        related_name='+'
+        related_name="+",
     )
-    categories = models.ManyToManyField('puput.Category', through='puput.CategoryEntryPage', blank=True)
+    categories = models.ManyToManyField("puput.Category", through="puput.CategoryEntryPage", blank=True)
     excerpt = RichTextField(
-        verbose_name=_('excerpt'),
+        verbose_name=_("excerpt"),
         blank=True,
-        help_text=_("Entry excerpt to be displayed on entries list. "
-                    "If this field is not filled, a truncate version of body text will be used.")
+        help_text=_(
+            "Entry excerpt to be displayed on entries list. "
+            "If this field is not filled, a truncate version of body text will be used."
+        ),
     )
     num_comments = models.IntegerField(default=0, editable=False)
 
     content_panels = [
         MultiFieldPanel(
             [
-                FieldPanel('title', classname="title"),
-                ImageChooserPanel('header_image'),
-                FieldPanel('body', classname="full"),
-                FieldPanel('excerpt', classname="full"),
+                FieldPanel("title", classname="title"),
+                FieldPanel("header_image"),
+                FieldPanel("body", classname="full"),
+                FieldPanel("excerpt", classname="full"),
             ],
-            heading=_("Content")
+            heading=_("Content"),
         ),
         MultiFieldPanel(
             [
-                FieldPanel('tags'),
-                InlinePanel('entry_categories', label=_("Categories")),
+                FieldPanel("tags"),
+                InlinePanel("entry_categories", label=_("Categories")),
                 InlinePanel(
-                    'related_entrypage_from',
-                    label=_("Related Entries"),
-                    panels=[PageChooserPanel('entrypage_to')]
+                    "related_entrypage_from", label=_("Related Entries"), panels=[PageChooserPanel("entrypage_to")]
                 ),
             ],
-            heading=_("Metadata")),
+            heading=_("Metadata"),
+        ),
     ]
 
     class Meta:
         abstract = True
```

### Comparing `puput-1.1.4/puput/comments.py` & `puput-1.2.0/puput/comments.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,58 +11,51 @@
         raise NotImplementedError()
 
     def get_num_comments(self):
         raise NotImplementedError()
 
 
 class DisqusCommentsProvider(CommentsProvider):
-
     @property
     def template(self):
-        return 'puput/comments/disqus.html'
+        return "puput/comments/disqus.html"
 
     def get_context(self):
         if not self.blog_page.disqus_shortname:
             return {}
-        return {
-            'disqus_shortname': self.blog_page.disqus_shortname,
-            'disqus_identifier': self.entry_page.id
-        }
+        return {"disqus_shortname": self.blog_page.disqus_shortname, "disqus_identifier": self.entry_page.id}
 
     def get_num_comments(self):
         if not self.blog_page.disqus_api_secret:
             return 0
         try:
             from tapioca.exceptions import ClientError
             from tapioca_disqus import Disqus
 
             disqus_client = Disqus(api_secret=self.blog_page.disqus_api_secret)
             try:
-                params = {'forum': self.blog_page.disqus_shortname, 'thread': 'ident:{}'.format(self.entry_page.id)}
+                params = {"forum": self.blog_page.disqus_shortname, "thread": "ident:{}".format(self.entry_page.id)}
                 thread = disqus_client.threads_details().get(params=params)
                 return thread.response.posts().data()
             except ClientError:
                 return 0
         except ImportError:
-            raise Exception('You need to install tapioca-disqus before using Disqus as comment system.')
+            raise Exception("You need to install tapioca-disqus before using Disqus as comment system.")
 
 
 class DjangoCommentsProvider(CommentsProvider):
-
     @property
     def template(self):
-        return 'puput/comments/django_comments.html'
+        return "puput/comments/django_comments.html"
 
     def get_context(self):
-        return {
-            'entry': self.entry_page
-        }
+        return {"entry": self.entry_page}
 
     def get_num_comments(self):
         try:
             from django_comments.models import Comment
             from django.contrib.contenttypes.models import ContentType
 
-            entry_page_type = ContentType.objects.get(app_label='puput', model='entrypage')
+            entry_page_type = ContentType.objects.get(app_label="puput", model="entrypage")
             return Comment.objects.filter(content_type=entry_page_type, object_pk=self.entry_page.pk).count()
         except ImportError:
-            raise Exception('You need to install django-comments before using it as comment system.')
+            raise Exception("You need to install django-comments before using it as comment system.")
```

### Comparing `puput-1.1.4/puput/conf/__init__.py` & `puput-1.2.0/puput/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `puput-1.1.4/puput/feeds.py` & `puput-1.2.0/puput/feeds.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,32 +9,32 @@
 
 from .models import BlogPage
 
 
 class BlogPageFeedGenerator(Rss201rev2Feed):
     def add_root_elements(self, handler):
         super(BlogPageFeedGenerator, self).add_root_elements(handler)
-        if self.feed['image_link']:
+        if self.feed["image_link"]:
             handler.addQuickElement(
-                'image',
-                '',
+                "image",
+                "",
                 {
-                    'url': self.feed['image_link'],
-                    'title': self.feed['title'],
-                    'link': self.feed['link'],
-                }
+                    "url": self.feed["image_link"],
+                    "title": self.feed["title"],
+                    "link": self.feed["link"],
+                },
             )
 
 
 class BlogPageFeed(Feed):
     feed_type = BlogPageFeedGenerator
 
     def __call__(self, request, *args, **kwargs):
-        if request.resolver_match.url_name == 'blog_page_feed_slug':
-            self.blog_page = BlogPage.extra.get_by_path(kwargs['blog_path'])
+        if request.resolver_match.url_name == "blog_page_feed_slug":
+            self.blog_page = BlogPage.extra.get_by_path(kwargs["blog_path"])
             if not self.blog_page:
                 raise http.Http404
         else:
             self.blog_page = BlogPage.objects.first()
         self.request = request
         return super(BlogPageFeed, self).__call__(request, *args, **kwargs)
 
@@ -50,29 +50,30 @@
     def items(self):
         return self.blog_page.get_entries()[:20]
 
     def item_title(self, item):
         return item.title
 
     def _item_short_description(self, item):
-        if item.excerpt and item.excerpt.strip() != '':
+        if item.excerpt and item.excerpt.strip() != "":
             return item.excerpt
         else:
             return truncatewords_html(item.body, 70)
 
     def item_description(self, item):
         if self.blog_page.short_feed_description:
             return self._item_short_description(item)
         return item.body
 
     def item_pubdate(self, item):
         return item.date
 
     def item_link(self, item):
         from .urls import get_entry_url
+
         entry_url = get_entry_url(item, self.blog_page.page_ptr, Site.find_for_request(self.request).root_page)
         return self.request.build_absolute_uri(entry_url)
 
     def item_enclosure_url(self, item):
         if item.header_image:
             site = Site.find_for_request(self.request)
             return urljoin(site.root_url, item.header_image.file.url)
@@ -91,10 +92,8 @@
 
     def _channel_image_link(self):
         if self.blog_page.header_image:
             site = Site.find_for_request(self.request)
             return urljoin(site.root_url, self.blog_page.header_image.file.url)
 
     def feed_extra_kwargs(self, obj):
-        return {
-            'image_link': self._channel_image_link()
-        }
+        return {"image_link": self._channel_image_link()}
```

### Comparing `puput-1.1.4/puput/locale/ar/LC_MESSAGES/django.mo` & `puput-1.2.0/puput/locale/ar/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `puput-1.1.4/puput/locale/ar/LC_MESSAGES/django.po` & `puput-1.2.0/puput/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `puput-1.1.4/puput/locale/ca/LC_MESSAGES/django.mo` & `puput-1.2.0/puput/locale/ca/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `puput-1.1.4/puput/locale/ca/LC_MESSAGES/django.po` & `puput-1.2.0/puput/locale/ca/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `puput-1.1.4/puput/locale/de/LC_MESSAGES/django.mo` & `puput-1.2.0/puput/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `puput-1.1.4/puput/locale/de/LC_MESSAGES/django.po` & `puput-1.2.0/puput/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `puput-1.1.4/puput/locale/en/LC_MESSAGES/django.po` & `puput-1.2.0/puput/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `puput-1.1.4/puput/locale/es/LC_MESSAGES/django.mo` & `puput-1.2.0/puput/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `puput-1.1.4/puput/locale/es/LC_MESSAGES/django.po` & `puput-1.2.0/puput/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `puput-1.1.4/puput/locale/fr/LC_MESSAGES/django.mo` & `puput-1.2.0/puput/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `puput-1.1.4/puput/locale/fr/LC_MESSAGES/django.po` & `puput-1.2.0/puput/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `puput-1.1.4/puput/locale/it/LC_MESSAGES/django.mo` & `puput-1.2.0/puput/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `puput-1.1.4/puput/locale/it/LC_MESSAGES/django.po` & `puput-1.2.0/puput/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `puput-1.1.4/puput/locale/ja/LC_MESSAGES/django.mo` & `puput-1.2.0/puput/locale/ja/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `puput-1.1.4/puput/locale/ja/LC_MESSAGES/django.po` & `puput-1.2.0/puput/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `puput-1.1.4/puput/locale/nl/LC_MESSAGES/django.po` & `puput-1.2.0/puput/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `puput-1.1.4/puput/locale/pl/LC_MESSAGES/django.mo` & `puput-1.2.0/puput/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `puput-1.1.4/puput/locale/pl/LC_MESSAGES/django.po` & `puput-1.2.0/puput/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `puput-1.1.4/puput/locale/pt_BR/LC_MESSAGES/django.mo` & `puput-1.2.0/puput/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `puput-1.1.4/puput/locale/pt_BR/LC_MESSAGES/django.po` & `puput-1.2.0/puput/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `puput-1.1.4/puput/locale/pt_PT/LC_MESSAGES/django.po` & `puput-1.2.0/puput/locale/pt_PT/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `puput-1.1.4/puput/locale/ru/LC_MESSAGES/django.mo` & `puput-1.2.0/puput/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `puput-1.1.4/puput/locale/ru/LC_MESSAGES/django.po` & `puput-1.2.0/puput/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `puput-1.1.4/puput/management/commands/puput_initial_data.py` & `puput-1.2.0/puput/management/commands/puput_initial_data.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,31 +8,29 @@
 
 class Command(BaseCommand):
     help = "Load Puput initial dummy data"
 
     def handle(self, *args, **options):
         # Get blogpage content type
         blogpage_content_type, created = ContentType.objects.get_or_create(
-            model='blogpage',
-            app_label='puput',
-            defaults={'name': 'page'} if DJANGO_VERSION < (1, 8) else {}
+            model="blogpage", app_label="puput", defaults={"name": "page"} if DJANGO_VERSION < (1, 8) else {}
         )
 
         # Get root page
         rootpage = Page.objects.first()
 
         # Set site root page as root site page
         site = Site.objects.first()
         site.root_page = rootpage
         site.save()
 
         # Create example blog page
         blogpage = BlogPage(
             title="Blog",
             content_type=blogpage_content_type,
-            slug='blog',
+            slug="blog",
         )
 
         # Add blog page as a child for homepage
         rootpage.add_child(instance=blogpage)
         revision = blogpage.save_revision()
         revision.publish()
```

### Comparing `puput-1.1.4/puput/managers.py` & `puput-1.2.0/puput/managers.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,30 +2,28 @@
 from django.db.models import Count
 from wagtail.core.models import PageManager
 
 from .utils import strip_prefix_and_ending_slash
 
 
 class TagManager(models.Manager):
-
     def most_common(self, blog_page):
         entries = blog_page.get_entries()
-        return self.filter(entrypage__in=entries).annotate(num_times=Count('entrypage')).order_by('-num_times')
+        return self.filter(entrypage__in=entries).annotate(num_times=Count("entrypage")).order_by("-num_times")
 
 
 class CategoryManager(models.Manager):
-
     def with_uses(self, blog_page):
         entries = blog_page.get_entries()
         return self.filter(entrypage__in=entries).distinct()
 
 
 class BlogManager(PageManager):
-
     def get_by_path(self, blog_path):
         # Look for the blog checking all the path
         from .models import BlogPage
+
         blogs = BlogPage.objects.filter(slug=blog_path.split("/")[-1])
         for blog in blogs:
             if strip_prefix_and_ending_slash(blog.specific.last_url_part) == blog_path:
                 return blog.specific
         return
```

### Comparing `puput-1.1.4/puput/migrations/0001_initial.py` & `puput-1.2.0/puput/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `puput-1.1.4/puput/migrations/0002_auto_20150919_0925.py` & `puput-1.2.0/puput/migrations/0002_auto_20150919_0925.py`

 * *Files identical despite different names*

### Comparing `puput-1.1.4/puput/migrations/0004_auto_20170912_0928.py` & `puput-1.2.0/puput/migrations/0004_auto_20170912_0928.py`

 * *Files identical despite different names*

### Comparing `puput-1.1.4/puput/migrations/0005_blogpage_main_color.py` & `puput-1.2.0/puput/migrations/0005_blogpage_main_color.py`

 * *Files identical despite different names*

### Comparing `puput-1.1.4/puput/models.py` & `puput-1.2.0/puput/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,148 +12,152 @@
 from modelcluster.fields import ParentalKey
 
 from .abstracts import EntryAbstract, BlogAbstract
 from .utils import import_model
 from .routes import BlogRoutes
 from .managers import TagManager, CategoryManager, BlogManager
 
-Entry = import_model(getattr(settings, 'PUPUT_ENTRY_MODEL', EntryAbstract))
-Blog = import_model(getattr(settings, 'PUPUT_BLOG_MODEL', BlogAbstract))
+Entry = import_model(getattr(settings, "PUPUT_ENTRY_MODEL", EntryAbstract))
+Blog = import_model(getattr(settings, "PUPUT_BLOG_MODEL", BlogAbstract))
 
 
 class BlogPage(BlogRoutes, Page, Blog):
     extra = BlogManager()
 
-    content_panels = Page.content_panels + getattr(Blog, 'content_panels', [])
-    settings_panels = Page.settings_panels + getattr(Blog, 'settings_panels', [])
+    content_panels = Page.content_panels + getattr(Blog, "content_panels", [])
+    settings_panels = Page.settings_panels + getattr(Blog, "settings_panels", [])
 
-    subpage_types = ['puput.EntryPage']
+    subpage_types = ["puput.EntryPage"]
 
     def get_entries(self):
-        return EntryPage.objects.descendant_of(self).live().order_by('-date').select_related('owner')
+        return EntryPage.objects.descendant_of(self).live().order_by("-date").select_related("owner")
 
     def get_context(self, request, *args, **kwargs):
         context = super(BlogPage, self).get_context(request, *args, **kwargs)
-        context['entries'] = self.entries
-        context['blog_page'] = self
-        context['search_type'] = getattr(self, 'search_type', "")
-        context['search_term'] = getattr(self, 'search_term', "")
+        context["entries"] = self.entries
+        context["blog_page"] = self
+        context["search_type"] = getattr(self, "search_type", "")
+        context["search_term"] = getattr(self, "search_term", "")
         return context
 
     @property
     def last_url_part(self):
         """
         Get the BlogPage url without the domain
         """
         return self.get_url_parts()[-1]
 
     class Meta:
-        verbose_name = _('Blog')
+        verbose_name = _("Blog")
 
 
 @register_snippet
 class Category(models.Model):
-    name = models.CharField(max_length=80, unique=True, verbose_name=_('Category name'))
+    name = models.CharField(max_length=80, unique=True, verbose_name=_("Category name"))
     slug = models.SlugField(unique=True, max_length=80)
     parent = models.ForeignKey(
-        'self',
+        "self",
         blank=True,
         null=True,
         related_name="children",
-        verbose_name=_('Parent category'),
-        on_delete=models.SET_NULL
+        verbose_name=_("Parent category"),
+        on_delete=models.SET_NULL,
     )
-    description = models.CharField(max_length=500, blank=True, verbose_name=_('Description'))
+    description = models.CharField(max_length=500, blank=True, verbose_name=_("Description"))
 
     objects = CategoryManager()
 
     def __str__(self):
         return self.name
 
     def clean(self):
         if self.parent:
             parent = self.parent
             if self.parent == self:
-                raise ValidationError(_('Parent category cannot be self.'))
+                raise ValidationError(_("Parent category cannot be self."))
             if parent.parent and parent.parent == self:
-                raise ValidationError(_('Cannot have circular Parents.'))
+                raise ValidationError(_("Cannot have circular Parents."))
 
     def save(self, *args, **kwargs):
         if not self.slug:
             self.slug = slugify(self.name)
         return super(Category, self).save(*args, **kwargs)
 
     class Meta:
-        ordering = ['name']
+        ordering = ["name"]
         verbose_name = _("Category")
         verbose_name_plural = _("Categories")
 
 
 class CategoryEntryPage(models.Model):
-    category = models.ForeignKey(Category, related_name="+", verbose_name=_('Category'), on_delete=models.CASCADE)
-    page = ParentalKey('EntryPage', related_name='entry_categories')
-    panels = [
-        FieldPanel('category')
-    ]
+    category = models.ForeignKey(Category, related_name="+", verbose_name=_("Category"), on_delete=models.CASCADE)
+    page = ParentalKey("EntryPage", related_name="entry_categories")
+    panels = [FieldPanel("category")]
 
     def __str__(self):
         return str(self.category)
 
 
 class TagEntryPage(TaggedItemBase):
-    content_object = ParentalKey('EntryPage', related_name='entry_tags')
+    content_object = ParentalKey("EntryPage", related_name="entry_tags")
 
 
 @register_snippet
 class Tag(TaggitTag):
     objects = TagManager()
 
     class Meta:
         proxy = True
 
 
 class EntryPageRelated(models.Model):
-    entrypage_from = ParentalKey('EntryPage', verbose_name=_("Entry"), related_name='related_entrypage_from')
-    entrypage_to = ParentalKey('EntryPage', verbose_name=_("Entry"), related_name='related_entrypage_to')
+    entrypage_from = ParentalKey("EntryPage", verbose_name=_("Entry"), related_name="related_entrypage_from")
+    entrypage_to = ParentalKey("EntryPage", verbose_name=_("Entry"), related_name="related_entrypage_to")
 
     def __str__(self):
         return str(self.entrypage_to)
 
 
 class EntryPage(Entry, Page):
     # Search
     search_fields = Page.search_fields + [
-        index.SearchField('body'),
-        index.SearchField('excerpt'),
-        index.FilterField('page_ptr_id')
+        index.SearchField("body"),
+        index.SearchField("excerpt"),
+        index.FilterField("page_ptr_id"),
     ]
 
     # Panels
-    content_panels = getattr(Entry, 'content_panels', [])
+    content_panels = getattr(Entry, "content_panels", [])
 
-    promote_panels = Page.promote_panels + getattr(Entry, 'promote_panels', [])
+    promote_panels = Page.promote_panels + getattr(Entry, "promote_panels", [])
 
-    settings_panels = Page.settings_panels + [
-        FieldPanel('date'), FieldPanel('owner'),
-    ] + getattr(Entry, 'settings_panels', [])
+    settings_panels = (
+        Page.settings_panels
+        + [
+            FieldPanel("date"),
+            FieldPanel("owner"),
+        ]
+        + getattr(Entry, "settings_panels", [])
+    )
 
     # Parent and child settings
-    parent_page_types = ['puput.BlogPage']
+    parent_page_types = ["puput.BlogPage"]
     subpage_types = []
 
     def get_sitemap_urls(self, request=None):
         from .urls import get_entry_url
+
         root_url = self.get_url_parts()[1]
         entry_url = get_entry_url(self, self.blog_page.page_ptr, root_url)
         return [
             {
-                'location': root_url + entry_url,
+                "location": root_url + entry_url,
                 # fall back on latest_revision_created_at if last_published_at is null
                 # (for backwards compatibility from before last_published_at was added)
-                'lastmod': (self.last_published_at or self.latest_revision_created_at),
+                "lastmod": (self.last_published_at or self.latest_revision_created_at),
             }
         ]
 
     @property
     def blog_page(self):
         return self.get_parent().specific
 
@@ -166,13 +170,13 @@
         return self.related_entrypage_from.count() > 0
 
     def get_absolute_url(self):
         return self.full_url
 
     def get_context(self, request, *args, **kwargs):
         context = super(EntryPage, self).get_context(request, *args, **kwargs)
-        context['blog_page'] = self.blog_page
+        context["blog_page"] = self.blog_page
         return context
 
     class Meta:
-        verbose_name = _('Entry')
-        verbose_name_plural = _('Entries')
+        verbose_name = _("Entry")
+        verbose_name_plural = _("Entries")
```

### Comparing `puput-1.1.4/puput/routes.py` & `puput-1.2.0/puput/routes.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,72 +8,71 @@
 
 from wagtail.contrib.routable_page.models import RoutablePageMixin, route
 from wagtail.core.models import Page
 from wagtail.search.models import Query
 
 from .utils import get_object_or_None
 
-USERNAME_REGEX = getattr(settings, 'PUPUT_USERNAME_REGEX', '\\w+')
-USERNAME_FIELD = getattr(settings, 'PUPUT_USERNAME_FIELD', 'username')
+USERNAME_REGEX = getattr(settings, "PUPUT_USERNAME_REGEX", "\\w+")
+USERNAME_FIELD = getattr(settings, "PUPUT_USERNAME_FIELD", "username")
 
 
 class BlogRoutes(RoutablePageMixin):
-
-    @route(r'^(\d{4})/$')
-    @route(r'^(\d{4})/(\d{2})/$')
-    @route(r'^(\d{4})/(\d{2})/(\d{2})/$')
+    @route(r"^(\d{4})/$")
+    @route(r"^(\d{4})/(\d{2})/$")
+    @route(r"^(\d{4})/(\d{2})/(\d{2})/$")
     def entries_by_date(self, request, year, month=None, day=None, *args, **kwargs):
         self.entries = self.get_entries().filter(date__year=year)
-        self.search_type = _('date')
+        self.search_type = _("date")
         self.search_term = year
         if month:
             self.entries = self.entries.filter(date__month=month)
             df = DateFormat(date(int(year), int(month), 1))
-            self.search_term = df.format('F Y')
+            self.search_term = df.format("F Y")
         if day:
             self.entries = self.entries.filter(date__day=day)
             self.search_term = date_format(date(int(year), int(month), int(day)))
         return Page.serve(self, request, *args, **kwargs)
 
-    @route(r'^tag/(?P<tag>[-\w]+)/$')
+    @route(r"^tag/(?P<tag>[-\w]+)/$")
     def entries_by_tag(self, request, tag, *args, **kwargs):
         from puput.models import Tag
 
-        self.search_type = _('tag')
+        self.search_type = _("tag")
         object_or_slug = get_object_or_None(Tag, slug=tag) or tag
         self.search_term = str(object_or_slug)
         self.entries = self.get_entries().filter(tags__slug=tag)
         return Page.serve(self, request, *args, **kwargs)
 
-    @route(r'^category/(?P<category>[-\w]+)/$')
+    @route(r"^category/(?P<category>[-\w]+)/$")
     def entries_by_category(self, request, category, *args, **kwargs):
         from puput.models import Category
 
-        self.search_type = _('category')
+        self.search_type = _("category")
         object_or_slug = get_object_or_None(Category, slug=category) or category
         self.search_term = str(object_or_slug)
         self.entries = self.get_entries().filter(entry_categories__category__slug=category)
         return Page.serve(self, request, *args, **kwargs)
 
-    @route(r'^author/(?P<author>%s)/$' % USERNAME_REGEX)
+    @route(r"^author/(?P<author>%s)/$" % USERNAME_REGEX)
     def entries_by_author(self, request, author, *args, **kwargs):
-        self.search_type = _('author')
+        self.search_type = _("author")
         object_or_slug = get_object_or_None(get_user_model(), **{USERNAME_FIELD: author}) or author
         self.search_term = str(object_or_slug)
-        self.entries = self.get_entries().filter(**{'owner__%s' % USERNAME_FIELD: author})
+        self.entries = self.get_entries().filter(**{"owner__%s" % USERNAME_FIELD: author})
         return Page.serve(self, request, *args, **kwargs)
 
-    @route(r'^search/$')
+    @route(r"^search/$")
     def entries_search(self, request, *args, **kwargs):
-        search_query = request.GET.get('q', None)
+        search_query = request.GET.get("q", None)
         self.entries = self.get_entries()
         if search_query:
             self.entries = self.entries.search(search_query)
             self.search_term = search_query
-            self.search_type = _('search')
+            self.search_type = _("search")
             Query.get(search_query).add_hit()
         return Page.serve(self, request, *args, **kwargs)
 
-    @route(r'^$')
+    @route(r"^$")
     def entries_list(self, request, *args, **kwargs):
         self.entries = self.get_entries()
         return Page.serve(self, request, *args, **kwargs)
```

### Comparing `puput-1.1.4/puput/signals.py` & `puput-1.2.0/puput/signals.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from django.conf import settings
 
 from .utils import import_model
 
 
 def update_comment_count(sender, **kwargs):
-    comment = kwargs['comment']
+    comment = kwargs["comment"]
     entry_page = comment.content_object
     comment_class = import_model(settings.PUPUT_COMMENTS_PROVIDER)(entry_page.blog_page, entry_page)
     num_comments = comment_class.get_num_comments()
     entry_page.num_comments = num_comments
-    entry_page.save(update_fields=('num_comments',))
+    entry_page.save(update_fields=("num_comments",))
 
 
 try:
     from django_comments_xtd.signals import confirmation_received
 
     confirmation_received.connect(update_comment_count, dispatch_uid="puput_comment_posted_id")
 except ImportError:
```

### Comparing `puput-1.1.4/puput/static/colorful/colorPicker.css` & `puput-1.2.0/puput/static/colorful/colorPicker.css`

 * *Files identical despite different names*

### Comparing `puput-1.1.4/puput/static/puput/css/bootstrap.min.css` & `puput-1.2.0/puput/static/puput/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `puput-1.1.4/puput/static/puput/css/font-awesome.min.css` & `puput-1.2.0/puput/static/puput/css/font-awesome.min.css`

 * *Files identical despite different names*

### Comparing `puput-1.1.4/puput/static/puput/css/puput.css` & `puput-1.2.0/puput/static/puput/css/puput.css`

 * *Files identical despite different names*

### Comparing `puput-1.1.4/puput/static/puput/fonts/FontAwesome.otf` & `puput-1.2.0/puput/static/puput/fonts/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `puput-1.1.4/puput/static/puput/fonts/fontawesome-webfont.eot` & `puput-1.2.0/puput/static/puput/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `puput-1.1.4/puput/static/puput/fonts/fontawesome-webfont.svg` & `puput-1.2.0/puput/static/puput/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `puput-1.1.4/puput/static/puput/fonts/fontawesome-webfont.ttf` & `puput-1.2.0/puput/static/puput/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `puput-1.1.4/puput/static/puput/fonts/fontawesome-webfont.woff` & `puput-1.2.0/puput/static/puput/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `puput-1.1.4/puput/static/puput/js/jquery.min.js` & `puput-1.2.0/puput/static/puput/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `puput-1.1.4/puput/static/puput/js/js.cookie.js` & `puput-1.2.0/puput/static/puput/js/js.cookie.js`

 * *Files identical despite different names*

### Comparing `puput-1.1.4/puput/static/puput/js/puput.js` & `puput-1.2.0/puput/static/puput/js/puput.js`

 * *Files identical despite different names*

### Comparing `puput-1.1.4/puput/templates/puput/base.html` & `puput-1.2.0/puput/templates/puput/base.html`

 * *Files identical despite different names*

### Comparing `puput-1.1.4/puput/templates/puput/blog_page.html` & `puput-1.2.0/puput/templates/puput/blog_page.html`

 * *Files identical despite different names*

### Comparing `puput-1.1.4/puput/templates/puput/comments/disqus.html` & `puput-1.2.0/puput/templates/puput/comments/disqus.html`

 * *Files identical despite different names*

### Comparing `puput-1.1.4/puput/templates/puput/entry_links.html` & `puput-1.2.0/puput/templates/puput/entry_links.html`

 * *Files identical despite different names*

### Comparing `puput-1.1.4/puput/templates/puput/entry_page.html` & `puput-1.2.0/puput/templates/puput/entry_page.html`

 * *Files identical despite different names*

### Comparing `puput-1.1.4/puput/templates/puput/related_entries.html` & `puput-1.2.0/puput/templates/puput/related_entries.html`

 * *Files identical despite different names*

### Comparing `puput-1.1.4/puput/templates/puput/tags/archives_list.html` & `puput-1.2.0/puput/templates/puput/tags/archives_list.html`

 * *Files identical despite different names*

### Comparing `puput-1.1.4/puput/templates/puput/tags/entries_list.html` & `puput-1.2.0/puput/templates/puput/tags/entries_list.html`

 * *Files identical despite different names*

### Comparing `puput-1.1.4/puput/templates/wagtailadmin/pages/_editor_css.html` & `puput-1.2.0/puput/templates/wagtailadmin/pages/_editor_css.html`

 * *Files identical despite different names*

### Comparing `puput-1.1.4/puput/templatetags/puput_tags.py` & `puput-1.2.0/puput/templatetags/puput_tags.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,119 +10,118 @@
 from ..models import Category, Tag
 
 from wagtail.core.models import Site
 
 register = Library()
 
 
-@register.inclusion_tag('puput/tags/entries_list.html', takes_context=True)
+@register.inclusion_tag("puput/tags/entries_list.html", takes_context=True)
 def recent_entries(context, limit=None):
-    blog_page = context['blog_page']
-    entries = blog_page.get_entries().order_by('-date')
+    blog_page = context["blog_page"]
+    entries = blog_page.get_entries().order_by("-date")
     if limit:
         entries = entries[:limit]
-    context['entries'] = entries
+    context["entries"] = entries
     return context
 
 
-@register.inclusion_tag('puput/tags/entries_list.html', takes_context=True)
+@register.inclusion_tag("puput/tags/entries_list.html", takes_context=True)
 def popular_entries(context, limit=None):
-    blog_page = context['blog_page']
-    entries = blog_page.get_entries().order_by('-num_comments', '-date')
+    blog_page = context["blog_page"]
+    entries = blog_page.get_entries().order_by("-num_comments", "-date")
     if limit:
         entries = entries[:limit]
-    context['entries'] = entries
+    context["entries"] = entries
     return context
 
 
-@register.inclusion_tag('puput/tags/tags_list.html', takes_context=True)
+@register.inclusion_tag("puput/tags/tags_list.html", takes_context=True)
 def tags_list(context, limit=None, tags_qs=None):
-    blog_page = context['blog_page']
+    blog_page = context["blog_page"]
     if tags_qs:
         tags = tags_qs.all()
     else:
         tags = Tag.objects.most_common(blog_page)
     if limit:
         tags = tags[:limit]
-    context['tags'] = tags
+    context["tags"] = tags
     return context
 
 
-@register.inclusion_tag('puput/tags/categories_list.html', takes_context=True)
+@register.inclusion_tag("puput/tags/categories_list.html", takes_context=True)
 def categories_list(context, categories_qs=None):
-    blog_page = context['blog_page']
+    blog_page = context["blog_page"]
     if categories_qs:
         categories = categories_qs.all()
     else:
         categories = Category.objects.with_uses(blog_page).filter(parent=None)
-    context['categories'] = categories
+    context["categories"] = categories
     return context
 
 
-@register.inclusion_tag('puput/tags/archives_list.html', takes_context=True)
+@register.inclusion_tag("puput/tags/archives_list.html", takes_context=True)
 def archives_list(context):
-    blog_page = context['blog_page']
-    context['archives'] = blog_page.get_entries().datetimes('date', 'day', order='DESC')
+    blog_page = context["blog_page"]
+    context["archives"] = blog_page.get_entries().datetimes("date", "day", order="DESC")
     return context
 
 
 @register.simple_tag(takes_context=True)
 def entry_url(context, entry, blog_page):
     from ..urls import get_entry_url
 
-    return get_entry_url(entry, blog_page.page_ptr, Site.find_for_request(context['request']).root_page)
+    return get_entry_url(entry, blog_page.page_ptr, Site.find_for_request(context["request"]).root_page)
 
 
 @register.simple_tag(takes_context=True)
 def canonical_url(context, entry=None):
-    if entry and resolve(context.request.path_info).url_name == 'wagtail_serve':
+    if entry and resolve(context.request.path_info).url_name == "wagtail_serve":
         return context.request.build_absolute_uri(entry_url(context, entry, entry.blog_page))
     return context.request.build_absolute_uri()
 
 
 @register.simple_tag(takes_context=True)
 def image_url(context, url):
     return context.request.build_absolute_uri(url)
 
 
 @register.simple_tag(takes_context=True)
 def feeds_url(context, blog_page):
     from ..urls import get_feeds_url
 
-    return get_feeds_url(blog_page.page_ptr, Site.find_for_request(context['request']).root_page)
+    return get_feeds_url(blog_page.page_ptr, Site.find_for_request(context["request"]).root_page)
 
 
 @register.simple_tag(takes_context=True)
 def show_comments(context):
-    blog_page = context['blog_page']
-    entry = context['self']
+    blog_page = context["blog_page"]
+    entry = context["self"]
     if blog_page.display_comments:
         try:
             comment_class = import_model(settings.PUPUT_COMMENTS_PROVIDER)(blog_page, entry)
             comment_context = comment_class.get_context()
             comment_context.update(context.flatten())
             return render_to_string(comment_class.template, context=comment_context)
         except AttributeError:
-            raise Exception('To use comments you need to specify '
-                            'PUPUT_COMMENTS_PROVIDER in settings.')
+            raise Exception("To use comments you need to specify " "PUPUT_COMMENTS_PROVIDER in settings.")
     return ""
 
 
 # Avoid to import endless_pagination in installed_apps and in the templates
-register.tag('show_paginator', show_pages)
-register.tag('paginate', paginate)
+register.tag("show_paginator", show_pages)
+register.tag("paginate", paginate)
 
 
 @register.simple_tag(takes_context=True)
 def post_to_linkendin_url(context, obj_or_url=None):
-    request = context.get('request')
+    request = context.get("request")
     if request:
         url = _build_url(request, obj_or_url)
-        context['linkendin_url'] = 'https://www.linkedin.com/shareArticle?url={}'.format(urlencode(url))
+        context["linkendin_url"] = "https://www.linkedin.com/shareArticle?url={}".format(urlencode(url))
     return context
 
 
-@register.inclusion_tag('puput/tags/post_to_linkedin.html', takes_context=True)
-def post_to_linkendin(context, obj_or_url=None, link_text='Post to LinkedIn'):
+@register.inclusion_tag("puput/tags/post_to_linkedin.html", takes_context=True)
+def post_to_linkendin(context, obj_or_url=None, link_text="Post to LinkedIn"):
     context = post_to_linkendin_url(context, obj_or_url)
-    context['link_text'] = link_text
+    context["link_text"] = link_text
     return context
```

### Comparing `puput-1.1.4/puput/urls.py` & `puput-1.2.0/puput/urls.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,97 +4,81 @@
 from .feeds import BlogPageFeed
 from .views import EntryPageServe, EntryPageUpdateCommentsView
 from .utils import strip_prefix_and_ending_slash
 
 
 urlpatterns = [
     path(
-        route='entry_page/<entry_page_id>/update_comments/',
+        route="entry_page/<entry_page_id>/update_comments/",
         view=EntryPageUpdateCommentsView.as_view(),
-        name='entry_page_update_comments'
+        name="entry_page_update_comments",
     ),
     path(
-        route='<path:blog_path>/<int:year>/<int:month>/<int:day>/<str:slug>/',
+        route="<path:blog_path>/<int:year>/<int:month>/<int:day>/<str:slug>/",
         view=EntryPageServe.as_view(),
-        name='entry_page_serve_slug'
+        name="entry_page_serve_slug",
     ),
-    path(
-        route='<int:year>/<int:month>/<int:day>/<str:slug>/',
-        view=EntryPageServe.as_view(),
-        name='entry_page_serve'
-    ),
-    path(
-        route='<path:blog_path>/feed/',
-        view=BlogPageFeed(),
-        name='blog_page_feed_slug'
-    ),
-    path(
-        route='feed/',
-        view=BlogPageFeed(),
-        name='blog_page_feed'
-    )
+    path(route="<int:year>/<int:month>/<int:day>/<str:slug>/", view=EntryPageServe.as_view(), name="entry_page_serve"),
+    path(route="<path:blog_path>/feed/", view=BlogPageFeed(), name="blog_page_feed_slug"),
+    path(route="feed/", view=BlogPageFeed(), name="blog_page_feed"),
 ]
 
-if not getattr(settings, 'PUPUT_AS_PLUGIN', False):
+if not getattr(settings, "PUPUT_AS_PLUGIN", False):
     from wagtail.core import urls as wagtail_urls
     from wagtail.admin import urls as wagtailadmin_urls
     from wagtail.documents import urls as wagtaildocs_urls
     from wagtail.contrib.sitemaps.views import sitemap
 
-    urlpatterns.extend([
-        path(
-            route='blog_admin/',
-            view=include(wagtailadmin_urls)
-        ),
-        path(
-            route='',
-            view=include(wagtail_urls)
-        ),
-        path(
-            route='documents/',
-            view=include(wagtaildocs_urls)
-        ),
-        path(
-            route='sitemap.xml',
-            view=sitemap
-        )
-    ])
+    urlpatterns.extend(
+        [
+            path(route="blog_admin/", view=include(wagtailadmin_urls)),
+            path(route="", view=include(wagtail_urls)),
+            path(route="documents/", view=include(wagtaildocs_urls)),
+            path(route="sitemap.xml", view=sitemap),
+        ]
+    )
 
 
 def get_entry_url(entry, blog_page, root_page):
     """
     Get the entry url given and entry page a blog page instances.
     It will use an url or another depending if blog_page is the root page.
     """
     if root_page == blog_page:
-        return reverse('entry_page_serve', kwargs={
-            'year': entry.date.strftime('%Y'),
-            'month': entry.date.strftime('%m'),
-            'day': entry.date.strftime('%d'),
-            'slug': entry.slug
-        })
+        return reverse(
+            "entry_page_serve",
+            kwargs={
+                "year": entry.date.strftime("%Y"),
+                "month": entry.date.strftime("%m"),
+                "day": entry.date.strftime("%d"),
+                "slug": entry.slug,
+            },
+        )
     else:
         # The method get_url_parts provides a tuple with a custom URL routing
         # scheme. In the last position it finds the subdomain of the blog, which
         # it is used to construct the entry url.
         # Using the stripped subdomain it allows Puput to generate the urls for
         # every sitemap level
         blog_path = strip_prefix_and_ending_slash(blog_page.specific.last_url_part)
-        return reverse('entry_page_serve_slug', kwargs={
-            'blog_path': blog_path,
-            'year': entry.date.strftime('%Y'),
-            'month': entry.date.strftime('%m'),
-            'day': entry.date.strftime('%d'),
-            'slug': entry.slug
-        })
+        return reverse(
+            "entry_page_serve_slug",
+            kwargs={
+                "blog_path": blog_path,
+                "year": entry.date.strftime("%Y"),
+                "month": entry.date.strftime("%m"),
+                "day": entry.date.strftime("%d"),
+                "slug": entry.slug,
+            },
+        )
 
 
 def get_feeds_url(blog_page, root_page):
     """
     Get the feeds urls a blog page instance.
     It will use an url or another depending if blog_page is the root page.
     """
     if root_page == blog_page:
-        return reverse('blog_page_feed')
+        return reverse("blog_page_feed")
     else:
         blog_path = strip_prefix_and_ending_slash(blog_page.specific.last_url_part)
-        return reverse('blog_page_feed_slug', kwargs={'blog_path': blog_path})
+        return reverse("blog_page_feed_slug", kwargs={"blog_path": blog_path})
```

### Comparing `puput-1.1.4/puput/utils.py` & `puput-1.2.0/puput/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 from importlib import import_module
 from django.urls import reverse
 from django.shortcuts import _get_queryset
 
 
 def import_model(path_or_callable):
-    if hasattr(path_or_callable, '__call__'):
+    if hasattr(path_or_callable, "__call__"):
         return path_or_callable
     else:
         assert isinstance(path_or_callable, str)
-        package, attr = path_or_callable.rsplit('.', 1)
+        package, attr = path_or_callable.rsplit(".", 1)
         return getattr(import_module(package), attr)
 
 
 def get_image_model_path():
     from django.conf import settings
-    return getattr(settings, 'WAGTAILIMAGES_IMAGE_MODEL', 'wagtailimages.Image')
+
+    return getattr(settings, "WAGTAILIMAGES_IMAGE_MODEL", "wagtailimages.Image")
 
 
 def strip_prefix_and_ending_slash(path):
     """
     If puput and wagtail are registered with a prefix, it needs to be removed
     so the 'entry_page_serve_slug' or 'blog_page_feed_slug' resolutions can work.
     Ex, here with a dynamic (i18n_patterns()) + a static prefix :
     urlpatterns += i18n_patterns(
         url(r'^blah/', include('puput.urls')),
         url(r'^blah/', include(wagtail_urls)),
     )
     The prefix is simply the root where Wagtail page are served.
     https://github.com/torchbox/wagtail/blob/stable/1.8.x/wagtail/wagtailcore/urls.py#L36
     """
-    return path.replace(reverse('wagtail_serve', args=[""]), '', 1).rstrip("/")
+    return path.replace(reverse("wagtail_serve", args=[""]), "", 1).rstrip("/")
 
 
 def get_object_or_None(klass, *args, **kwargs):
     """
     Uses get() to return an object or None if the object does not exist.
     klass may be a Model, Manager, or QuerySet object. All other passed
     arguments and keyword arguments are used in the get() query.
```

### Comparing `puput-1.1.4/puput/views.py` & `puput-1.2.0/puput/views.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,43 +24,42 @@
     """
 
     @method_decorator(ensure_csrf_cookie)
     def get(self, request, *args, **kwargs):
         site = Site.find_for_request(request)
         if not site:
             raise Http404
-        if request.resolver_match.url_name == 'entry_page_serve_slug':
+        if request.resolver_match.url_name == "entry_page_serve_slug":
             # Splitting the request path and obtaining the path_components
             # this way allows you to place the blog at the level you want on
             # your sitemap.
             # Example:
             # splited_path =  ['es', 'blog', '2016', '06', '23', 'blog-entry']
             # slicing this way you obtain:
             # path_components =  ['es', 'blog', 'blog-entry']
             # with the oldest solution you'll get ['es', 'blog-entry']
             # and a 404 will be raised
             splited_path = strip_prefix_and_ending_slash(request.path).split("/")
             path_components = splited_path[:-4] + splited_path[-1:]
         else:
-            path_components = [strip_prefix_and_ending_slash(request.path).split('/')[-1]]
+            path_components = [strip_prefix_and_ending_slash(request.path).split("/")[-1]]
         page, args, kwargs = site.root_page.specific.route(request, path_components)
 
-        for fn in hooks.get_hooks('before_serve_page'):
+        for fn in hooks.get_hooks("before_serve_page"):
             result = fn(page, request, args, kwargs)
             if isinstance(result, HttpResponse):
                 return result
         return page.serve(request, *args, **kwargs)
 
 
 class EntryPageUpdateCommentsView(View):
-
     def post(self, request, entry_page_id, *args, **kwargs):
         try:
             entry_page = EntryPage.objects.get(pk=entry_page_id)
             blog_page = entry_page.blog_page
             comment_class = import_model(settings.PUPUT_COMMENTS_PROVIDER)(blog_page, entry_page)
             num_comments = comment_class.get_num_comments()
             entry_page.num_comments = num_comments
-            entry_page.save(update_fields=('num_comments',))
+            entry_page.save(update_fields=("num_comments",))
             return HttpResponse()
         except EntryPage.DoesNotExist:
             raise Http404
```

### Comparing `puput-1.1.4/puput.egg-info/PKG-INFO` & `puput-1.2.0/puput.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: puput
-Version: 1.1.4
+Version: 1.2.0
 Summary: A Django blog app implemented in Wagtail.
 Home-page: http://github.com/APSL/puput
 Author: Marc Tudurí
 Author-email: marctc@gmail.com
 Keywords: django wagtail puput blog cms app
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS
 
 Puput
```

### Comparing `puput-1.1.4/puput.egg-info/SOURCES.txt` & `puput-1.2.0/puput.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `puput-1.1.4/setup.py` & `puput-1.2.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,34 +21,34 @@
     version=get_metadata('puput', 'version'),
     packages=find_packages(exclude=("example*", "tests*")),
     include_package_data=True,
     keywords="django wagtail puput blog cms app",
     description='A Django blog app implemented in Wagtail.',
     long_description=codecs.open(os.path.join(os.path.dirname(__file__), 'README.rst'), encoding='utf-8').read(),
     install_requires=[
-        'Django>=2.0,<4.0',
-        'wagtail>=2.7,<4.0',
+        'Django>=3.0,<4.0',
+        'wagtail>=3.0,<5.0',
         'django-el-pagination>=3.2.4',
         'django-social-share>=1.3.0',
         'django-colorful>=1.3'
     ],
     url='http://github.com/APSL/puput',
     author=get_metadata('puput', 'author'),
     author_email=get_metadata('puput', 'email'),
     long_description_content_type='text/x-rst',
     classifiers=[
         'Environment :: Web Environment',
         'Framework :: Django',
-        'Framework :: Django :: 2.2',
         'Framework :: Django :: 3.0',
         'Framework :: Django :: 3.1',
         'Framework :: Django :: 3.2',
         'Intended Audience :: Developers',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
         'Operating System :: OS Independent',
         'Topic :: Software Development'
     ]
 )
```

