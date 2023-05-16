# Comparing `tmp/frasco-3.3.2.tar.gz` & `tmp/frasco-3.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frasco-3.3.2.tar", last modified: Mon Apr  3 11:52:39 2023, max compression
+gzip compressed data, was "frasco-3.3.3.tar", last modified: Tue May 16 09:10:11 2023, max compression
```

## Comparing `frasco-3.3.2.tar` & `frasco-3.3.3.tar`

### file list

```diff
@@ -1,171 +1,171 @@
-drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-04-03 11:52:39.448579 frasco-3.3.2/
--rw-rw-r--   0 maxime    (1000) maxime    (1000)      274 2023-04-03 11:52:39.448579 frasco-3.3.2/PKG-INFO
--rw-rw-r--   0 maxime    (1000) maxime    (1000)       58 2022-06-08 12:10:52.000000 frasco-3.3.2/README.md
-drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-04-03 11:52:39.416579 frasco-3.3.2/frasco/
--rw-rw-r--   0 maxime    (1000) maxime    (1000)      661 2023-03-10 13:43:06.000000 frasco-3.3.2/frasco/__init__.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)       34 2022-06-08 12:10:52.000000 frasco-3.3.2/frasco/__main__.py
-drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-04-03 11:52:39.420579 frasco-3.3.2/frasco/api/
--rw-rw-r--   0 maxime    (1000) maxime    (1000)       23 2022-06-08 12:10:52.000000 frasco-3.3.2/frasco/api/__init__.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     2979 2022-06-08 12:10:52.000000 frasco-3.3.2/frasco/api/auth.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)      830 2022-06-08 12:10:52.000000 frasco-3.3.2/frasco/api/errors.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     7575 2023-03-13 16:39:26.000000 frasco-3.3.2/frasco/api/service.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     9731 2023-03-14 11:06:34.000000 frasco-3.3.2/frasco/api/spec.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     1387 2023-03-10 13:43:06.000000 frasco-3.3.2/frasco/app.py
-drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-04-03 11:52:39.420579 frasco-3.3.2/frasco/assets/
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     6556 2023-03-10 13:43:06.000000 frasco-3.3.2/frasco/assets/__init__.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     1197 2022-06-08 12:10:52.000000 frasco-3.3.2/frasco/assets/macros.html
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     1776 2022-06-08 12:10:52.000000 frasco-3.3.2/frasco/assets/service-worker.js
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     1966 2022-06-08 12:10:52.000000 frasco-3.3.2/frasco/assets/sw_cache.py
-drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-04-03 11:52:39.424579 frasco-3.3.2/frasco/babel/
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     6149 2023-03-10 13:43:06.000000 frasco-3.3.2/frasco/babel/__init__.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     5100 2022-06-08 12:10:52.000000 frasco-3.3.2/frasco/babel/cli.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     4199 2023-03-10 13:43:06.000000 frasco-3.3.2/frasco/babel/ctx.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     2868 2022-06-08 12:10:52.000000 frasco-3.3.2/frasco/babel/extract.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)      250 2022-06-08 12:10:52.000000 frasco-3.3.2/frasco/babel/signals.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)      595 2022-06-08 12:10:52.000000 frasco-3.3.2/frasco/babel/user.py
-drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-04-03 11:52:39.424579 frasco-3.3.2/frasco/billing/
--rw-rw-r--   0 maxime    (1000) maxime    (1000)        0 2022-06-08 12:10:52.000000 frasco-3.3.2/frasco/billing/__init__.py
-drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-04-03 11:52:39.424579 frasco-3.3.2/frasco/billing/eu_vat/
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     2354 2022-06-08 12:10:52.000000 frasco-3.3.2/frasco/billing/eu_vat/__init__.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     5059 2022-06-08 12:10:52.000000 frasco-3.3.2/frasco/billing/eu_vat/data.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     1261 2022-06-08 12:10:52.000000 frasco-3.3.2/frasco/billing/eu_vat/model.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     2530 2022-06-08 12:10:52.000000 frasco-3.3.2/frasco/billing/eu_vat/service.py
-drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-04-03 11:52:39.424579 frasco-3.3.2/frasco/billing/invoicing/
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     3112 2022-06-08 12:10:52.000000 frasco-3.3.2/frasco/billing/invoicing/__init__.py
-drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-04-03 11:52:39.424579 frasco-3.3.2/frasco/billing/invoicing/emails/
--rw-rw-r--   0 maxime    (1000) maxime    (1000)      162 2022-06-08 12:10:52.000000 frasco-3.3.2/frasco/billing/invoicing/emails/failed_invoice.html
--rw-rw-r--   0 maxime    (1000) maxime    (1000)       76 2022-06-08 12:10:52.000000 frasco-3.3.2/frasco/billing/invoicing/emails/invoice.html
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     1128 2022-06-08 12:10:52.000000 frasco-3.3.2/frasco/billing/invoicing/model.py
-drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-04-03 11:52:39.424579 frasco-3.3.2/frasco/billing/stripe/
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     6714 2022-07-19 16:54:36.000000 frasco-3.3.2/frasco/billing/stripe/__init__.py
-drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-04-03 11:52:39.424579 frasco-3.3.2/frasco/billing/stripe/emails/
--rw-rw-r--   0 maxime    (1000) maxime    (1000)      143 2022-06-08 12:10:52.000000 frasco-3.3.2/frasco/billing/stripe/emails/trial_will_end.txt
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     4228 2022-06-08 12:10:52.000000 frasco-3.3.2/frasco/billing/stripe/invoice.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    23809 2022-07-21 16:30:23.000000 frasco-3.3.2/frasco/billing/stripe/model.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)      680 2022-07-19 16:54:36.000000 frasco-3.3.2/frasco/billing/stripe/signals.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)      621 2022-06-08 12:10:52.000000 frasco-3.3.2/frasco/billing/stripe/webhook.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)      271 2022-06-08 12:10:52.000000 frasco-3.3.2/frasco/cli.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     3080 2023-03-10 13:43:06.000000 frasco-3.3.2/frasco/config.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     3868 2023-03-10 13:43:06.000000 frasco-3.3.2/frasco/ctx.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     6186 2022-06-08 12:10:52.000000 frasco-3.3.2/frasco/ext.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     3435 2022-06-08 12:10:52.000000 frasco-3.3.2/frasco/geoip.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     1586 2023-03-10 13:43:06.000000 frasco-3.3.2/frasco/helpers.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     2323 2022-06-08 12:10:52.000000 frasco-3.3.2/frasco/i18n.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)      380 2022-06-08 12:10:52.000000 frasco-3.3.2/frasco/json_decoder.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     1412 2022-06-08 12:10:52.000000 frasco-3.3.2/frasco/logging.py
-drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-04-03 11:52:39.428579 frasco-3.3.2/frasco/mail/
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     6412 2022-06-08 12:10:52.000000 frasco-3.3.2/frasco/mail/__init__.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     6446 2022-06-08 12:10:52.000000 frasco-3.3.2/frasco/mail/message.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     1339 2022-06-08 12:10:52.000000 frasco-3.3.2/frasco/mail/provider.py
-drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-04-03 11:52:39.428579 frasco-3.3.2/frasco/mail/providers/
--rw-rw-r--   0 maxime    (1000) maxime    (1000)        0 2022-06-08 12:10:52.000000 frasco-3.3.2/frasco/mail/providers/__init__.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)      478 2022-06-08 12:10:52.000000 frasco-3.3.2/frasco/mail/providers/mailgun.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     1146 2022-06-08 12:10:52.000000 frasco-3.3.2/frasco/mail/providers/smtp.py
-drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-04-03 11:52:39.428579 frasco-3.3.2/frasco/mail/templates/
--rw-rw-r--   0 maxime    (1000) maxime    (1000)       33 2022-06-08 12:10:52.000000 frasco-3.3.2/frasco/mail/templates/layout.html
-drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-04-03 11:52:39.428579 frasco-3.3.2/frasco/mail/templates/layouts/
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     1074 2022-06-08 12:10:52.000000 frasco-3.3.2/frasco/mail/templates/layouts/MAILGUN_LICENSE
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     2108 2022-06-08 12:10:52.000000 frasco-3.3.2/frasco/mail/templates/layouts/MAILGUN_README.md
--rw-rw-r--   0 maxime    (1000) maxime    (1000)      164 2022-06-08 12:10:52.000000 frasco-3.3.2/frasco/mail/templates/layouts/alert.html
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     4586 2022-06-08 12:10:52.000000 frasco-3.3.2/frasco/mail/templates/layouts/base.html
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     5887 2022-06-08 12:10:52.000000 frasco-3.3.2/frasco/mail/templates/layouts/invoice.html
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     2861 2022-06-08 12:10:52.000000 frasco-3.3.2/frasco/mail/templates/layouts/macros.html
--rw-rw-r--   0 maxime    (1000) maxime    (1000)       60 2022-06-08 12:10:52.000000 frasco-3.3.2/frasco/mail/templates/layouts/markdown.html
--rw-rw-r--   0 maxime    (1000) maxime    (1000)       79 2022-06-08 12:10:52.000000 frasco-3.3.2/frasco/mail/templates/layouts/text.html
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     3384 2023-03-14 11:06:44.000000 frasco-3.3.2/frasco/marshaller.py
-drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-04-03 11:52:39.432579 frasco-3.3.2/frasco/models/
--rw-rw-r--   0 maxime    (1000) maxime    (1000)       69 2022-06-08 12:10:52.000000 frasco-3.3.2/frasco/models/__init__.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)      194 2022-06-08 12:10:52.000000 frasco-3.3.2/frasco/models/cache.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     1553 2022-06-08 12:10:52.000000 frasco-3.3.2/frasco/models/decorators.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)      942 2022-06-08 12:10:52.000000 frasco-3.3.2/frasco/models/ext.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     8504 2022-06-08 12:10:52.000000 frasco-3.3.2/frasco/models/serializer.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     2475 2023-03-10 13:43:06.000000 frasco-3.3.2/frasco/models/transactions.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     4262 2022-06-08 12:10:52.000000 frasco-3.3.2/frasco/models/utils.py
-drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-04-03 11:52:39.432579 frasco-3.3.2/frasco/push/
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     6770 2022-08-01 06:58:55.000000 frasco-3.3.2/frasco/push/__init__.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     2130 2023-03-14 13:17:54.000000 frasco-3.3.2/frasco/push/exposed_signals.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     8822 2022-06-08 12:10:52.000000 frasco-3.3.2/frasco/push/server.py
-drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-04-03 11:52:39.432579 frasco-3.3.2/frasco/push/static/
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     5398 2022-06-08 12:10:52.000000 frasco-3.3.2/frasco/push/static/push-client.js
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    41370 2022-06-08 12:10:53.000000 frasco-3.3.2/frasco/push/static/socketio-client.js
-drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-04-03 11:52:39.436579 frasco-3.3.2/frasco/redis/
--rw-rw-r--   0 maxime    (1000) maxime    (1000)       83 2022-06-08 12:10:53.000000 frasco-3.3.2/frasco/redis/__init__.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     6849 2022-06-08 12:10:53.000000 frasco-3.3.2/frasco/redis/attr.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)      768 2022-06-08 12:10:53.000000 frasco-3.3.2/frasco/redis/ext.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     5737 2022-06-08 12:10:53.000000 frasco-3.3.2/frasco/redis/objects.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)      486 2022-06-08 12:10:53.000000 frasco-3.3.2/frasco/redis/templating.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     3279 2022-06-08 12:10:53.000000 frasco-3.3.2/frasco/redis/utils.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    13767 2023-03-15 10:12:02.000000 frasco-3.3.2/frasco/request_params.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)      608 2022-06-08 12:10:53.000000 frasco-3.3.2/frasco/subdomains.py
-drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-04-03 11:52:39.436579 frasco-3.3.2/frasco/tasks/
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     4683 2022-06-08 12:10:53.000000 frasco-3.3.2/frasco/tasks/__init__.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     1966 2022-10-13 14:50:34.000000 frasco-3.3.2/frasco/tasks/helpers.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     4914 2023-03-10 13:43:06.000000 frasco-3.3.2/frasco/tasks/job.py
-drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-04-03 11:52:39.436579 frasco-3.3.2/frasco/templating/
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     1598 2023-03-10 13:43:06.000000 frasco-3.3.2/frasco/templating/__init__.py
-drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-04-03 11:52:39.436579 frasco-3.3.2/frasco/templating/bootstrap/
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     2545 2022-06-08 12:10:53.000000 frasco-3.3.2/frasco/templating/bootstrap/dropdown.html
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     7151 2022-06-08 12:10:53.000000 frasco-3.3.2/frasco/templating/bootstrap/form.html
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     1293 2022-06-08 12:10:53.000000 frasco-3.3.2/frasco/templating/bootstrap/menu.html
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     7923 2022-06-08 12:10:53.000000 frasco-3.3.2/frasco/templating/bootstrap/ui.html
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     3787 2022-06-08 12:10:53.000000 frasco-3.3.2/frasco/templating/extensions.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     1250 2022-06-17 01:47:53.000000 frasco-3.3.2/frasco/templating/helpers.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)      821 2022-06-08 12:10:53.000000 frasco-3.3.2/frasco/templating/layout.html
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     1843 2022-06-08 12:10:53.000000 frasco-3.3.2/frasco/templating/macros.html
-drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-04-03 11:52:39.440579 frasco-3.3.2/frasco/upload/
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     4607 2022-06-08 12:10:53.000000 frasco-3.3.2/frasco/upload/__init__.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)      980 2022-06-08 12:10:53.000000 frasco-3.3.2/frasco/upload/backend.py
-drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-04-03 11:52:39.440579 frasco-3.3.2/frasco/upload/backends/
--rw-rw-r--   0 maxime    (1000) maxime    (1000)        0 2022-06-08 12:10:53.000000 frasco-3.3.2/frasco/upload/backends/__init__.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)      234 2022-06-08 12:10:53.000000 frasco-3.3.2/frasco/upload/backends/http.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)      236 2022-06-08 12:10:53.000000 frasco-3.3.2/frasco/upload/backends/https.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)      986 2022-07-21 21:25:52.000000 frasco-3.3.2/frasco/upload/backends/local.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     6427 2022-06-08 12:10:53.000000 frasco-3.3.2/frasco/upload/backends/s3.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     3230 2022-06-08 12:10:53.000000 frasco-3.3.2/frasco/upload/form.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     3470 2022-06-08 12:10:53.000000 frasco-3.3.2/frasco/upload/utils.py
-drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-04-03 11:52:39.444579 frasco-3.3.2/frasco/users/
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    10934 2022-06-08 12:10:53.000000 frasco-3.3.2/frasco/users/__init__.py
-drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-04-03 11:52:39.444579 frasco-3.3.2/frasco/users/auth/
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     1100 2022-06-08 12:10:53.000000 frasco-3.3.2/frasco/users/auth/__init__.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     7479 2023-03-10 13:43:06.000000 frasco-3.3.2/frasco/users/auth/oauth.py
-drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-04-03 11:52:39.444579 frasco-3.3.2/frasco/users/avatars/
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     4387 2023-03-10 13:43:06.000000 frasco-3.3.2/frasco/users/avatars/__init__.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     1930 2022-06-08 12:10:53.000000 frasco-3.3.2/frasco/users/avatars/first_letter_avatar.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    17533 2023-04-03 10:12:50.000000 frasco-3.3.2/frasco/users/blueprint.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)      956 2022-06-08 12:10:53.000000 frasco-3.3.2/frasco/users/captcha.py
-drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-04-03 11:52:39.412579 frasco-3.3.2/frasco/users/emails/
-drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-04-03 11:52:39.444579 frasco-3.3.2/frasco/users/emails/users/
--rw-rw-r--   0 maxime    (1000) maxime    (1000)      119 2022-06-08 12:10:53.000000 frasco-3.3.2/frasco/users/emails/users/2fa_disabled.txt
--rw-rw-r--   0 maxime    (1000) maxime    (1000)      124 2022-06-08 12:10:53.000000 frasco-3.3.2/frasco/users/emails/users/2fa_enabled.txt
--rw-rw-r--   0 maxime    (1000) maxime    (1000)      310 2022-06-08 12:10:53.000000 frasco-3.3.2/frasco/users/emails/users/reset_password.html
--rw-rw-r--   0 maxime    (1000) maxime    (1000)      201 2022-06-08 12:10:53.000000 frasco-3.3.2/frasco/users/emails/users/reset_password.txt
--rw-rw-r--   0 maxime    (1000) maxime    (1000)      207 2022-06-08 12:10:53.000000 frasco-3.3.2/frasco/users/emails/users/reset_password_done.txt
--rw-rw-r--   0 maxime    (1000) maxime    (1000)      173 2022-06-08 12:10:53.000000 frasco-3.3.2/frasco/users/emails/users/validate_email.html
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     2136 2022-06-08 12:10:53.000000 frasco-3.3.2/frasco/users/forms.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     1365 2022-06-08 12:10:53.000000 frasco-3.3.2/frasco/users/jinja_ext.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     4080 2022-06-08 12:10:53.000000 frasco-3.3.2/frasco/users/model.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     1340 2022-06-08 12:10:53.000000 frasco-3.3.2/frasco/users/otp.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     5254 2022-06-08 12:10:53.000000 frasco-3.3.2/frasco/users/password.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)      389 2022-06-08 12:10:53.000000 frasco-3.3.2/frasco/users/signals.py
-drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-04-03 11:52:39.412579 frasco-3.3.2/frasco/users/templates/
-drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-04-03 11:52:39.444579 frasco-3.3.2/frasco/users/templates/users/
--rw-rw-r--   0 maxime    (1000) maxime    (1000)      153 2022-06-08 12:10:53.000000 frasco-3.3.2/frasco/users/templates/users/layout.html
--rw-rw-r--   0 maxime    (1000) maxime    (1000)      698 2022-06-08 12:10:53.000000 frasco-3.3.2/frasco/users/templates/users/login.html
--rw-rw-r--   0 maxime    (1000) maxime    (1000)      329 2022-06-08 12:10:53.000000 frasco-3.3.2/frasco/users/templates/users/login_2fa.html
--rw-rw-r--   0 maxime    (1000) maxime    (1000)      427 2022-06-08 12:10:53.000000 frasco-3.3.2/frasco/users/templates/users/non_email_validated_users_block_page.html
--rw-rw-r--   0 maxime    (1000) maxime    (1000)      309 2022-06-08 12:10:53.000000 frasco-3.3.2/frasco/users/templates/users/reset_password.html
--rw-rw-r--   0 maxime    (1000) maxime    (1000)      281 2022-06-08 12:10:53.000000 frasco-3.3.2/frasco/users/templates/users/send_reset_password.html
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     1034 2022-06-08 12:10:53.000000 frasco-3.3.2/frasco/users/templates/users/signup.html
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     1376 2022-06-08 12:10:53.000000 frasco-3.3.2/frasco/users/tokens.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    11220 2022-06-08 12:10:53.000000 frasco-3.3.2/frasco/users/user.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     7245 2022-06-08 12:10:53.000000 frasco-3.3.2/frasco/utils.py
-drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-04-03 11:52:39.420579 frasco-3.3.2/frasco.egg-info/
--rw-rw-r--   0 maxime    (1000) maxime    (1000)      274 2023-04-03 11:52:39.000000 frasco-3.3.2/frasco.egg-info/PKG-INFO
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     4042 2023-04-03 11:52:39.000000 frasco-3.3.2/frasco.egg-info/SOURCES.txt
--rw-rw-r--   0 maxime    (1000) maxime    (1000)        1 2023-04-03 11:52:39.000000 frasco-3.3.2/frasco.egg-info/dependency_links.txt
--rw-rw-r--   0 maxime    (1000) maxime    (1000)       61 2023-04-03 11:52:39.000000 frasco-3.3.2/frasco.egg-info/entry_points.txt
--rw-rw-r--   0 maxime    (1000) maxime    (1000)        1 2022-06-17 01:50:31.000000 frasco-3.3.2/frasco.egg-info/not-zip-safe
--rw-rw-r--   0 maxime    (1000) maxime    (1000)      614 2023-04-03 11:52:39.000000 frasco-3.3.2/frasco.egg-info/requires.txt
--rw-rw-r--   0 maxime    (1000) maxime    (1000)        7 2023-04-03 11:52:39.000000 frasco-3.3.2/frasco.egg-info/top_level.txt
--rw-rw-r--   0 maxime    (1000) maxime    (1000)       38 2023-04-03 11:52:39.448579 frasco-3.3.2/setup.cfg
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     2046 2023-04-03 11:52:28.000000 frasco-3.3.2/setup.py
+drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-05-16 09:10:11.070645 frasco-3.3.3/
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)      274 2023-05-16 09:10:11.070645 frasco-3.3.3/PKG-INFO
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)       58 2022-06-08 12:10:52.000000 frasco-3.3.3/README.md
+drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-05-16 09:10:11.046645 frasco-3.3.3/frasco/
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)      661 2023-03-10 13:43:06.000000 frasco-3.3.3/frasco/__init__.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)       34 2022-06-08 12:10:52.000000 frasco-3.3.3/frasco/__main__.py
+drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-05-16 09:10:11.046645 frasco-3.3.3/frasco/api/
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)       23 2022-06-08 12:10:52.000000 frasco-3.3.3/frasco/api/__init__.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     2979 2022-06-08 12:10:52.000000 frasco-3.3.3/frasco/api/auth.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)      830 2022-06-08 12:10:52.000000 frasco-3.3.3/frasco/api/errors.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     7575 2023-03-13 16:39:26.000000 frasco-3.3.3/frasco/api/service.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     9731 2023-03-14 11:06:34.000000 frasco-3.3.3/frasco/api/spec.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     1387 2023-03-10 13:43:06.000000 frasco-3.3.3/frasco/app.py
+drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-05-16 09:10:11.046645 frasco-3.3.3/frasco/assets/
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     6556 2023-03-10 13:43:06.000000 frasco-3.3.3/frasco/assets/__init__.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     1197 2022-06-08 12:10:52.000000 frasco-3.3.3/frasco/assets/macros.html
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     1776 2022-06-08 12:10:52.000000 frasco-3.3.3/frasco/assets/service-worker.js
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     1966 2022-06-08 12:10:52.000000 frasco-3.3.3/frasco/assets/sw_cache.py
+drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-05-16 09:10:11.050645 frasco-3.3.3/frasco/babel/
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     6105 2023-04-07 13:34:19.000000 frasco-3.3.3/frasco/babel/__init__.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     5100 2022-06-08 12:10:52.000000 frasco-3.3.3/frasco/babel/cli.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     4199 2023-03-10 13:43:06.000000 frasco-3.3.3/frasco/babel/ctx.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     2868 2022-06-08 12:10:52.000000 frasco-3.3.3/frasco/babel/extract.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)      250 2022-06-08 12:10:52.000000 frasco-3.3.3/frasco/babel/signals.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)      595 2022-06-08 12:10:52.000000 frasco-3.3.3/frasco/babel/user.py
+drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-05-16 09:10:11.050645 frasco-3.3.3/frasco/billing/
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)        0 2022-06-08 12:10:52.000000 frasco-3.3.3/frasco/billing/__init__.py
+drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-05-16 09:10:11.050645 frasco-3.3.3/frasco/billing/eu_vat/
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     2354 2022-06-08 12:10:52.000000 frasco-3.3.3/frasco/billing/eu_vat/__init__.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     5240 2023-05-16 09:08:12.000000 frasco-3.3.3/frasco/billing/eu_vat/data.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     1261 2022-06-08 12:10:52.000000 frasco-3.3.3/frasco/billing/eu_vat/model.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     2530 2022-06-08 12:10:52.000000 frasco-3.3.3/frasco/billing/eu_vat/service.py
+drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-05-16 09:10:11.050645 frasco-3.3.3/frasco/billing/invoicing/
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     3112 2022-06-08 12:10:52.000000 frasco-3.3.3/frasco/billing/invoicing/__init__.py
+drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-05-16 09:10:11.050645 frasco-3.3.3/frasco/billing/invoicing/emails/
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)      162 2022-06-08 12:10:52.000000 frasco-3.3.3/frasco/billing/invoicing/emails/failed_invoice.html
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)       76 2022-06-08 12:10:52.000000 frasco-3.3.3/frasco/billing/invoicing/emails/invoice.html
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     1128 2022-06-08 12:10:52.000000 frasco-3.3.3/frasco/billing/invoicing/model.py
+drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-05-16 09:10:11.050645 frasco-3.3.3/frasco/billing/stripe/
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     6714 2022-07-19 16:54:36.000000 frasco-3.3.3/frasco/billing/stripe/__init__.py
+drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-05-16 09:10:11.050645 frasco-3.3.3/frasco/billing/stripe/emails/
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)      143 2022-06-08 12:10:52.000000 frasco-3.3.3/frasco/billing/stripe/emails/trial_will_end.txt
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     4228 2022-06-08 12:10:52.000000 frasco-3.3.3/frasco/billing/stripe/invoice.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    23809 2022-07-21 16:30:23.000000 frasco-3.3.3/frasco/billing/stripe/model.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)      680 2022-07-19 16:54:36.000000 frasco-3.3.3/frasco/billing/stripe/signals.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)      621 2022-06-08 12:10:52.000000 frasco-3.3.3/frasco/billing/stripe/webhook.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)      271 2022-06-08 12:10:52.000000 frasco-3.3.3/frasco/cli.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     3080 2023-03-10 13:43:06.000000 frasco-3.3.3/frasco/config.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     3868 2023-03-10 13:43:06.000000 frasco-3.3.3/frasco/ctx.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     6186 2022-06-08 12:10:52.000000 frasco-3.3.3/frasco/ext.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     3435 2022-06-08 12:10:52.000000 frasco-3.3.3/frasco/geoip.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     1586 2023-03-10 13:43:06.000000 frasco-3.3.3/frasco/helpers.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     2323 2022-06-08 12:10:52.000000 frasco-3.3.3/frasco/i18n.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)      380 2022-06-08 12:10:52.000000 frasco-3.3.3/frasco/json_decoder.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     1412 2022-06-08 12:10:52.000000 frasco-3.3.3/frasco/logging.py
+drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-05-16 09:10:11.050645 frasco-3.3.3/frasco/mail/
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     6412 2022-06-08 12:10:52.000000 frasco-3.3.3/frasco/mail/__init__.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     6446 2022-06-08 12:10:52.000000 frasco-3.3.3/frasco/mail/message.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     1339 2022-06-08 12:10:52.000000 frasco-3.3.3/frasco/mail/provider.py
+drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-05-16 09:10:11.054645 frasco-3.3.3/frasco/mail/providers/
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)        0 2022-06-08 12:10:52.000000 frasco-3.3.3/frasco/mail/providers/__init__.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)      478 2022-06-08 12:10:52.000000 frasco-3.3.3/frasco/mail/providers/mailgun.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     1146 2022-06-08 12:10:52.000000 frasco-3.3.3/frasco/mail/providers/smtp.py
+drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-05-16 09:10:11.054645 frasco-3.3.3/frasco/mail/templates/
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)       33 2022-06-08 12:10:52.000000 frasco-3.3.3/frasco/mail/templates/layout.html
+drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-05-16 09:10:11.054645 frasco-3.3.3/frasco/mail/templates/layouts/
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     1074 2022-06-08 12:10:52.000000 frasco-3.3.3/frasco/mail/templates/layouts/MAILGUN_LICENSE
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     2108 2022-06-08 12:10:52.000000 frasco-3.3.3/frasco/mail/templates/layouts/MAILGUN_README.md
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)      164 2022-06-08 12:10:52.000000 frasco-3.3.3/frasco/mail/templates/layouts/alert.html
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     4586 2022-06-08 12:10:52.000000 frasco-3.3.3/frasco/mail/templates/layouts/base.html
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     5887 2022-06-08 12:10:52.000000 frasco-3.3.3/frasco/mail/templates/layouts/invoice.html
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     2861 2022-06-08 12:10:52.000000 frasco-3.3.3/frasco/mail/templates/layouts/macros.html
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)       60 2022-06-08 12:10:52.000000 frasco-3.3.3/frasco/mail/templates/layouts/markdown.html
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)       79 2022-06-08 12:10:52.000000 frasco-3.3.3/frasco/mail/templates/layouts/text.html
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     3384 2023-03-14 11:06:44.000000 frasco-3.3.3/frasco/marshaller.py
+drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-05-16 09:10:11.054645 frasco-3.3.3/frasco/models/
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)       69 2022-06-08 12:10:52.000000 frasco-3.3.3/frasco/models/__init__.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)      194 2022-06-08 12:10:52.000000 frasco-3.3.3/frasco/models/cache.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     1553 2022-06-08 12:10:52.000000 frasco-3.3.3/frasco/models/decorators.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)      942 2022-06-08 12:10:52.000000 frasco-3.3.3/frasco/models/ext.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     8504 2022-06-08 12:10:52.000000 frasco-3.3.3/frasco/models/serializer.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     2475 2023-03-10 13:43:06.000000 frasco-3.3.3/frasco/models/transactions.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     4262 2022-06-08 12:10:52.000000 frasco-3.3.3/frasco/models/utils.py
+drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-05-16 09:10:11.058645 frasco-3.3.3/frasco/push/
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     6770 2022-08-01 06:58:55.000000 frasco-3.3.3/frasco/push/__init__.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     2130 2023-03-14 13:17:54.000000 frasco-3.3.3/frasco/push/exposed_signals.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     8822 2022-06-08 12:10:52.000000 frasco-3.3.3/frasco/push/server.py
+drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-05-16 09:10:11.058645 frasco-3.3.3/frasco/push/static/
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     5398 2022-06-08 12:10:52.000000 frasco-3.3.3/frasco/push/static/push-client.js
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    41370 2022-06-08 12:10:53.000000 frasco-3.3.3/frasco/push/static/socketio-client.js
+drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-05-16 09:10:11.058645 frasco-3.3.3/frasco/redis/
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)       83 2022-06-08 12:10:53.000000 frasco-3.3.3/frasco/redis/__init__.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     6849 2022-06-08 12:10:53.000000 frasco-3.3.3/frasco/redis/attr.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)      768 2022-06-08 12:10:53.000000 frasco-3.3.3/frasco/redis/ext.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     5737 2022-06-08 12:10:53.000000 frasco-3.3.3/frasco/redis/objects.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)      486 2022-06-08 12:10:53.000000 frasco-3.3.3/frasco/redis/templating.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     3279 2022-06-08 12:10:53.000000 frasco-3.3.3/frasco/redis/utils.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    13767 2023-03-15 10:12:02.000000 frasco-3.3.3/frasco/request_params.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)      608 2022-06-08 12:10:53.000000 frasco-3.3.3/frasco/subdomains.py
+drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-05-16 09:10:11.058645 frasco-3.3.3/frasco/tasks/
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     4683 2022-06-08 12:10:53.000000 frasco-3.3.3/frasco/tasks/__init__.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     1966 2022-10-13 14:50:34.000000 frasco-3.3.3/frasco/tasks/helpers.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     4914 2023-03-10 13:43:06.000000 frasco-3.3.3/frasco/tasks/job.py
+drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-05-16 09:10:11.062645 frasco-3.3.3/frasco/templating/
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     1598 2023-03-10 13:43:06.000000 frasco-3.3.3/frasco/templating/__init__.py
+drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-05-16 09:10:11.062645 frasco-3.3.3/frasco/templating/bootstrap/
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     2545 2022-06-08 12:10:53.000000 frasco-3.3.3/frasco/templating/bootstrap/dropdown.html
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     7151 2022-06-08 12:10:53.000000 frasco-3.3.3/frasco/templating/bootstrap/form.html
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     1293 2022-06-08 12:10:53.000000 frasco-3.3.3/frasco/templating/bootstrap/menu.html
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     7923 2022-06-08 12:10:53.000000 frasco-3.3.3/frasco/templating/bootstrap/ui.html
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     3787 2022-06-08 12:10:53.000000 frasco-3.3.3/frasco/templating/extensions.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     1250 2022-06-17 01:47:53.000000 frasco-3.3.3/frasco/templating/helpers.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)      821 2022-06-08 12:10:53.000000 frasco-3.3.3/frasco/templating/layout.html
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     1843 2022-06-08 12:10:53.000000 frasco-3.3.3/frasco/templating/macros.html
+drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-05-16 09:10:11.062645 frasco-3.3.3/frasco/upload/
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     4607 2022-06-08 12:10:53.000000 frasco-3.3.3/frasco/upload/__init__.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)      980 2022-06-08 12:10:53.000000 frasco-3.3.3/frasco/upload/backend.py
+drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-05-16 09:10:11.062645 frasco-3.3.3/frasco/upload/backends/
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)        0 2022-06-08 12:10:53.000000 frasco-3.3.3/frasco/upload/backends/__init__.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)      234 2022-06-08 12:10:53.000000 frasco-3.3.3/frasco/upload/backends/http.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)      236 2022-06-08 12:10:53.000000 frasco-3.3.3/frasco/upload/backends/https.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)      986 2022-07-21 21:25:52.000000 frasco-3.3.3/frasco/upload/backends/local.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     6427 2022-06-08 12:10:53.000000 frasco-3.3.3/frasco/upload/backends/s3.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     3230 2022-06-08 12:10:53.000000 frasco-3.3.3/frasco/upload/form.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     3470 2022-06-08 12:10:53.000000 frasco-3.3.3/frasco/upload/utils.py
+drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-05-16 09:10:11.066645 frasco-3.3.3/frasco/users/
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    10934 2022-06-08 12:10:53.000000 frasco-3.3.3/frasco/users/__init__.py
+drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-05-16 09:10:11.066645 frasco-3.3.3/frasco/users/auth/
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     1100 2022-06-08 12:10:53.000000 frasco-3.3.3/frasco/users/auth/__init__.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     7479 2023-03-10 13:43:06.000000 frasco-3.3.3/frasco/users/auth/oauth.py
+drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-05-16 09:10:11.070645 frasco-3.3.3/frasco/users/avatars/
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     4387 2023-03-10 13:43:06.000000 frasco-3.3.3/frasco/users/avatars/__init__.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     1930 2022-06-08 12:10:53.000000 frasco-3.3.3/frasco/users/avatars/first_letter_avatar.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    17533 2023-04-03 10:12:50.000000 frasco-3.3.3/frasco/users/blueprint.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)      956 2022-06-08 12:10:53.000000 frasco-3.3.3/frasco/users/captcha.py
+drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-05-16 09:10:11.042645 frasco-3.3.3/frasco/users/emails/
+drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-05-16 09:10:11.070645 frasco-3.3.3/frasco/users/emails/users/
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)      119 2022-06-08 12:10:53.000000 frasco-3.3.3/frasco/users/emails/users/2fa_disabled.txt
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)      124 2022-06-08 12:10:53.000000 frasco-3.3.3/frasco/users/emails/users/2fa_enabled.txt
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)      310 2022-06-08 12:10:53.000000 frasco-3.3.3/frasco/users/emails/users/reset_password.html
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)      201 2022-06-08 12:10:53.000000 frasco-3.3.3/frasco/users/emails/users/reset_password.txt
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)      207 2022-06-08 12:10:53.000000 frasco-3.3.3/frasco/users/emails/users/reset_password_done.txt
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)      173 2022-06-08 12:10:53.000000 frasco-3.3.3/frasco/users/emails/users/validate_email.html
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     2136 2022-06-08 12:10:53.000000 frasco-3.3.3/frasco/users/forms.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     1365 2022-06-08 12:10:53.000000 frasco-3.3.3/frasco/users/jinja_ext.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     4080 2022-06-08 12:10:53.000000 frasco-3.3.3/frasco/users/model.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     1340 2022-06-08 12:10:53.000000 frasco-3.3.3/frasco/users/otp.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     5254 2022-06-08 12:10:53.000000 frasco-3.3.3/frasco/users/password.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)      389 2022-06-08 12:10:53.000000 frasco-3.3.3/frasco/users/signals.py
+drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-05-16 09:10:11.042645 frasco-3.3.3/frasco/users/templates/
+drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-05-16 09:10:11.070645 frasco-3.3.3/frasco/users/templates/users/
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)      153 2022-06-08 12:10:53.000000 frasco-3.3.3/frasco/users/templates/users/layout.html
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)      698 2022-06-08 12:10:53.000000 frasco-3.3.3/frasco/users/templates/users/login.html
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)      329 2022-06-08 12:10:53.000000 frasco-3.3.3/frasco/users/templates/users/login_2fa.html
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)      427 2022-06-08 12:10:53.000000 frasco-3.3.3/frasco/users/templates/users/non_email_validated_users_block_page.html
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)      309 2022-06-08 12:10:53.000000 frasco-3.3.3/frasco/users/templates/users/reset_password.html
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)      281 2022-06-08 12:10:53.000000 frasco-3.3.3/frasco/users/templates/users/send_reset_password.html
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     1034 2022-06-08 12:10:53.000000 frasco-3.3.3/frasco/users/templates/users/signup.html
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     1376 2022-06-08 12:10:53.000000 frasco-3.3.3/frasco/users/tokens.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    11220 2022-06-08 12:10:53.000000 frasco-3.3.3/frasco/users/user.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     7245 2022-06-08 12:10:53.000000 frasco-3.3.3/frasco/utils.py
+drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-05-16 09:10:11.046645 frasco-3.3.3/frasco.egg-info/
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)      274 2023-05-16 09:10:10.000000 frasco-3.3.3/frasco.egg-info/PKG-INFO
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     4042 2023-05-16 09:10:11.000000 frasco-3.3.3/frasco.egg-info/SOURCES.txt
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)        1 2023-05-16 09:10:10.000000 frasco-3.3.3/frasco.egg-info/dependency_links.txt
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)       61 2023-05-16 09:10:10.000000 frasco-3.3.3/frasco.egg-info/entry_points.txt
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)        1 2022-06-17 01:50:31.000000 frasco-3.3.3/frasco.egg-info/not-zip-safe
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)      614 2023-05-16 09:10:10.000000 frasco-3.3.3/frasco.egg-info/requires.txt
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)        7 2023-05-16 09:10:10.000000 frasco-3.3.3/frasco.egg-info/top_level.txt
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)       38 2023-05-16 09:10:11.070645 frasco-3.3.3/setup.cfg
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     2046 2023-05-16 09:08:31.000000 frasco-3.3.3/setup.py
```

### Comparing `frasco-3.3.2/frasco/__init__.py` & `frasco-3.3.3/frasco/__init__.py`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco/api/auth.py` & `frasco-3.3.3/frasco/api/auth.py`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco/api/errors.py` & `frasco-3.3.3/frasco/api/errors.py`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco/api/service.py` & `frasco-3.3.3/frasco/api/service.py`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco/api/spec.py` & `frasco-3.3.3/frasco/api/spec.py`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco/app.py` & `frasco-3.3.3/frasco/app.py`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco/assets/__init__.py` & `frasco-3.3.3/frasco/assets/__init__.py`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco/assets/macros.html` & `frasco-3.3.3/frasco/assets/macros.html`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco/assets/service-worker.js` & `frasco-3.3.3/frasco/assets/service-worker.js`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco/assets/sw_cache.py` & `frasco-3.3.3/frasco/assets/sw_cache.py`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco/babel/__init__.py` & `frasco-3.3.3/frasco/babel/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
                 "extract_locale_from_request": False,
                 "always_add_locale_to_urls": True,
                 "store_request_locale_in_session": False,
                 "request_arg": "locale",
                 "extractors": [],
                 "extract_keywords": [],
                 "extract_jinja_dirs": ["templates", "emails"],
-                "extract_with_jinja_exts": ["jinja2.ext.autoescape", "jinja2.ext.with_",
+                "extract_with_jinja_exts": [
                     "jinja2.ext.do", "jinja_layout.LayoutExtension", "jinja_macro_tags.LoadMacroExtension",
                     "jinja_macro_tags.CallMacroTagExtension", "jinja_macro_tags.JinjaMacroTagsExtension",
                     "jinja_macro_tags.HtmlMacroTagsExtension", "frasco.templating.FlashMessagesExtension"],
                 "request_locale_arg_ignore_endpoints": ["static", "static_upload"],
                 "compile_to_json": False,
                 "compile_to_js": False,
                 "js_catalog_varname": "LOCALE_%s_CATALOG",
```

### Comparing `frasco-3.3.2/frasco/babel/cli.py` & `frasco-3.3.3/frasco/babel/cli.py`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco/babel/ctx.py` & `frasco-3.3.3/frasco/babel/ctx.py`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco/babel/extract.py` & `frasco-3.3.3/frasco/babel/extract.py`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco/babel/user.py` & `frasco-3.3.3/frasco/babel/user.py`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco/billing/eu_vat/__init__.py` & `frasco-3.3.3/frasco/billing/eu_vat/__init__.py`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco/billing/eu_vat/data.py` & `frasco-3.3.3/frasco/billing/eu_vat/data.py`

 * *Files 4% similar despite different names*

```diff
@@ -104,30 +104,33 @@
     return TICClient
 
 
 class EUVATError(Exception):
     pass
 
 
-def get_vat_rate(country_code, rate_type='standard'):
+def get_vat_rate(country_code, rate_type='standard', fallback_on_known_rates=True):
     country_code = country_code.upper()
     if not is_eu_country(country_code):
         raise EUVATError('Not an EU country')
     if country_code not in _vat_rates_cache:
         _vat_rates_cache[country_code] = {}
         try:
             r = get_ticc_soap_client().service.getRates(dict(memberState=country_code,
                 requestDate=datetime.date.today().isoformat()))
             for rate in r.ratesResponse.rate:
                 _vat_rates_cache[country_code][rate.type.lower()] = float(rate.value)
         except Exception as e:
             current_app.logger.debug(e)
             _vat_rates_cache.pop(country_code)
-            return KNOWN_VAT_RATES.get(country_code)
-    return _vat_rates_cache[country_code].get(rate_type.lower())
+            return KNOWN_VAT_RATES.get(country_code) if fallback_on_known_rates else None
+    rate = _vat_rates_cache[country_code].get(rate_type.lower())
+    if rate is None and fallback_on_known_rates:
+        return KNOWN_VAT_RATES.get(country_code)
+    return rate
 
 
 def validate_vat_number(vat_number, invalid_format_raise_error=False):
     if len(vat_number) < 3:
         if invalid_format_raise_error:
             raise EUVATError('VAT number too short')
         return False
```

### Comparing `frasco-3.3.2/frasco/billing/eu_vat/model.py` & `frasco-3.3.3/frasco/billing/eu_vat/model.py`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco/billing/eu_vat/service.py` & `frasco-3.3.3/frasco/billing/eu_vat/service.py`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco/billing/invoicing/__init__.py` & `frasco-3.3.3/frasco/billing/invoicing/__init__.py`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco/billing/invoicing/model.py` & `frasco-3.3.3/frasco/billing/invoicing/model.py`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco/billing/stripe/__init__.py` & `frasco-3.3.3/frasco/billing/stripe/__init__.py`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco/billing/stripe/invoice.py` & `frasco-3.3.3/frasco/billing/stripe/invoice.py`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco/billing/stripe/model.py` & `frasco-3.3.3/frasco/billing/stripe/model.py`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco/billing/stripe/signals.py` & `frasco-3.3.3/frasco/billing/stripe/signals.py`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco/billing/stripe/webhook.py` & `frasco-3.3.3/frasco/billing/stripe/webhook.py`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco/config.py` & `frasco-3.3.3/frasco/config.py`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco/ctx.py` & `frasco-3.3.3/frasco/ctx.py`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco/ext.py` & `frasco-3.3.3/frasco/ext.py`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco/geoip.py` & `frasco-3.3.3/frasco/geoip.py`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco/helpers.py` & `frasco-3.3.3/frasco/helpers.py`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco/i18n.py` & `frasco-3.3.3/frasco/i18n.py`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco/logging.py` & `frasco-3.3.3/frasco/logging.py`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco/mail/__init__.py` & `frasco-3.3.3/frasco/mail/__init__.py`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco/mail/message.py` & `frasco-3.3.3/frasco/mail/message.py`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco/mail/provider.py` & `frasco-3.3.3/frasco/mail/provider.py`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco/mail/providers/smtp.py` & `frasco-3.3.3/frasco/mail/providers/smtp.py`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco/mail/templates/layouts/MAILGUN_LICENSE` & `frasco-3.3.3/frasco/mail/templates/layouts/MAILGUN_LICENSE`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco/mail/templates/layouts/MAILGUN_README.md` & `frasco-3.3.3/frasco/mail/templates/layouts/MAILGUN_README.md`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco/mail/templates/layouts/base.html` & `frasco-3.3.3/frasco/mail/templates/layouts/base.html`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco/mail/templates/layouts/invoice.html` & `frasco-3.3.3/frasco/mail/templates/layouts/invoice.html`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco/mail/templates/layouts/macros.html` & `frasco-3.3.3/frasco/mail/templates/layouts/macros.html`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco/marshaller.py` & `frasco-3.3.3/frasco/marshaller.py`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco/models/decorators.py` & `frasco-3.3.3/frasco/models/decorators.py`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco/models/ext.py` & `frasco-3.3.3/frasco/models/ext.py`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco/models/serializer.py` & `frasco-3.3.3/frasco/models/serializer.py`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco/models/transactions.py` & `frasco-3.3.3/frasco/models/transactions.py`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco/models/utils.py` & `frasco-3.3.3/frasco/models/utils.py`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco/push/__init__.py` & `frasco-3.3.3/frasco/push/__init__.py`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco/push/exposed_signals.py` & `frasco-3.3.3/frasco/push/exposed_signals.py`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco/push/server.py` & `frasco-3.3.3/frasco/push/server.py`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco/push/static/push-client.js` & `frasco-3.3.3/frasco/push/static/push-client.js`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco/push/static/socketio-client.js` & `frasco-3.3.3/frasco/push/static/socketio-client.js`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco/redis/attr.py` & `frasco-3.3.3/frasco/redis/attr.py`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco/redis/ext.py` & `frasco-3.3.3/frasco/redis/ext.py`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco/redis/objects.py` & `frasco-3.3.3/frasco/redis/objects.py`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco/redis/utils.py` & `frasco-3.3.3/frasco/redis/utils.py`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco/request_params.py` & `frasco-3.3.3/frasco/request_params.py`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco/subdomains.py` & `frasco-3.3.3/frasco/subdomains.py`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco/tasks/__init__.py` & `frasco-3.3.3/frasco/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco/tasks/helpers.py` & `frasco-3.3.3/frasco/tasks/helpers.py`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco/tasks/job.py` & `frasco-3.3.3/frasco/tasks/job.py`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco/templating/__init__.py` & `frasco-3.3.3/frasco/templating/__init__.py`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco/templating/bootstrap/dropdown.html` & `frasco-3.3.3/frasco/templating/bootstrap/dropdown.html`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco/templating/bootstrap/form.html` & `frasco-3.3.3/frasco/templating/bootstrap/form.html`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco/templating/bootstrap/menu.html` & `frasco-3.3.3/frasco/templating/bootstrap/menu.html`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco/templating/bootstrap/ui.html` & `frasco-3.3.3/frasco/templating/bootstrap/ui.html`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco/templating/extensions.py` & `frasco-3.3.3/frasco/templating/extensions.py`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco/templating/helpers.py` & `frasco-3.3.3/frasco/templating/helpers.py`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco/templating/layout.html` & `frasco-3.3.3/frasco/templating/layout.html`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco/templating/macros.html` & `frasco-3.3.3/frasco/templating/macros.html`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco/upload/__init__.py` & `frasco-3.3.3/frasco/upload/__init__.py`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco/upload/backend.py` & `frasco-3.3.3/frasco/upload/backend.py`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco/upload/backends/local.py` & `frasco-3.3.3/frasco/upload/backends/local.py`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco/upload/backends/s3.py` & `frasco-3.3.3/frasco/upload/backends/s3.py`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco/upload/form.py` & `frasco-3.3.3/frasco/upload/form.py`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco/upload/utils.py` & `frasco-3.3.3/frasco/upload/utils.py`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco/users/__init__.py` & `frasco-3.3.3/frasco/users/__init__.py`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco/users/auth/__init__.py` & `frasco-3.3.3/frasco/users/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco/users/auth/oauth.py` & `frasco-3.3.3/frasco/users/auth/oauth.py`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco/users/avatars/__init__.py` & `frasco-3.3.3/frasco/users/avatars/__init__.py`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco/users/avatars/first_letter_avatar.py` & `frasco-3.3.3/frasco/users/avatars/first_letter_avatar.py`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco/users/blueprint.py` & `frasco-3.3.3/frasco/users/blueprint.py`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco/users/captcha.py` & `frasco-3.3.3/frasco/users/captcha.py`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco/users/forms.py` & `frasco-3.3.3/frasco/users/forms.py`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco/users/jinja_ext.py` & `frasco-3.3.3/frasco/users/jinja_ext.py`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco/users/model.py` & `frasco-3.3.3/frasco/users/model.py`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco/users/otp.py` & `frasco-3.3.3/frasco/users/otp.py`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco/users/password.py` & `frasco-3.3.3/frasco/users/password.py`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco/users/templates/users/login.html` & `frasco-3.3.3/frasco/users/templates/users/login.html`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco/users/templates/users/signup.html` & `frasco-3.3.3/frasco/users/templates/users/signup.html`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco/users/tokens.py` & `frasco-3.3.3/frasco/users/tokens.py`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco/users/user.py` & `frasco-3.3.3/frasco/users/user.py`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco/utils.py` & `frasco-3.3.3/frasco/utils.py`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco.egg-info/SOURCES.txt` & `frasco-3.3.3/frasco.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/frasco.egg-info/requires.txt` & `frasco-3.3.3/frasco.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `frasco-3.3.2/setup.py` & `frasco-3.3.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='frasco',
-    version='3.3.2',
+    version='3.3.3',
     url='http://github.com/frascoweb/frasco',
     license='MIT',
     author='Maxime Bouroumeau-Fuseau',
     author_email='maxime.bouroumeau@gmail.com',
     description='Set of extensions for Flask to develop SaaS applications',
     packages=find_packages(),
     package_data={
```

