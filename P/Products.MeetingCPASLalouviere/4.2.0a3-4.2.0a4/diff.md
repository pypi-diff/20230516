# Comparing `tmp/Products.MeetingCPASLalouviere-4.2.0a3.tar.gz` & `tmp/Products.MeetingCPASLalouviere-4.2.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Products.MeetingCPASLalouviere-4.2.0a3.tar", last modified: Mon May 15 10:51:15 2023, max compression
+gzip compressed data, was "Products.MeetingCPASLalouviere-4.2.0a4.tar", last modified: Tue May 16 14:32:29 2023, max compression
```

## Comparing `Products.MeetingCPASLalouviere-4.2.0a3.tar` & `Products.MeetingCPASLalouviere-4.2.0a4.tar`

### file list

```diff
@@ -1,201 +1,202 @@
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-05-15 10:51:15.035923 Products.MeetingCPASLalouviere-4.2.0a3/
--rw-rw-r--   0 oli       (1000) oli       (1000)     2811 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/CHANGES.rst
--rw-rw-r--   0 oli       (1000) oli       (1000)      353 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/MANIFEST.in
--rw-rw-r--   0 oli       (1000) oli       (1000)     3451 2023-05-15 10:51:15.035923 Products.MeetingCPASLalouviere-4.2.0a3/PKG-INFO
--rw-rw-r--   0 oli       (1000) oli       (1000)       23 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/README.rst
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-05-15 10:51:15.015922 Products.MeetingCPASLalouviere-4.2.0a3/docs/
--rw-rw-r--   0 oli       (1000) oli       (1000)    18092 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/docs/LICENSE.GPL
--rw-rw-r--   0 oli       (1000) oli       (1000)      734 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/docs/LICENSE.txt
--rw-rw-r--   0 oli       (1000) oli       (1000)     1121 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/docs/MIGRATION.txt
--rw-rw-r--   0 oli       (1000) oli       (1000)       38 2023-05-15 10:51:15.035923 Products.MeetingCPASLalouviere-4.2.0a3/setup.cfg
--rw-rw-r--   0 oli       (1000) oli       (1000)     1248 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/setup.py
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-05-15 10:51:15.011922 Products.MeetingCPASLalouviere-4.2.0a3/src/
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-05-15 10:51:15.015922 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-05-15 10:51:15.019923 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/
--rw-rw-r--   0 oli       (1000) oli       (1000)      981 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/README.txt
--rw-rw-r--   0 oli       (1000) oli       (1000)     1773 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/__init__.py
--rw-rw-r--   0 oli       (1000) oli       (1000)    13219 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/adapters.py
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-05-15 10:51:15.019923 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/browser/
--rw-rw-r--   0 oli       (1000) oli       (1000)        0 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/browser/__init__.py
--rw-rw-r--   0 oli       (1000) oli       (1000)      177 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/browser/configure.zcml
--rw-rw-r--   0 oli       (1000) oli       (1000)      120 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/browser/overrides.py
--rw-rw-r--   0 oli       (1000) oli       (1000)      805 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/browser/views.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     3386 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/config.py
--rw-rw-r--   0 oli       (1000) oli       (1000)      724 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/configure.zcml
--rw-rw-r--   0 oli       (1000) oli       (1000)      615 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/events.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     3719 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/interfaces.py
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-05-15 10:51:15.019923 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/locales/
--rw-rw-r--   0 oli       (1000) oli       (1000)     1897 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/locales/PloneMeeting.pot
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-05-15 10:51:15.011922 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/locales/en/
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-05-15 10:51:15.019923 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/locales/en/LC_MESSAGES/
--rw-rw-r--   0 oli       (1000) oli       (1000)     1206 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/locales/en/LC_MESSAGES/PloneMeeting.po
--rw-rw-r--   0 oli       (1000) oli       (1000)     2089 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/locales/en/LC_MESSAGES/plone.po
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-05-15 10:51:15.011922 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/locales/fr/
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-05-15 10:51:15.019923 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/locales/fr/LC_MESSAGES/
--rw-rw-r--   0 oli       (1000) oli       (1000)     2383 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/locales/fr/LC_MESSAGES/PloneMeeting.po
--rw-rw-r--   0 oli       (1000) oli       (1000)     2939 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/locales/fr/LC_MESSAGES/plone.po
--rw-rw-r--   0 oli       (1000) oli       (1000)     1970 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/locales/plone.pot
--rwxrwxr-x   0 oli       (1000) oli       (1000)      267 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/locales/sync_pos.sh
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-05-15 10:51:15.019923 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/migrations/
--rw-rw-r--   0 oli       (1000) oli       (1000)        0 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/migrations/__init__.py
--rw-rw-r--   0 oli       (1000) oli       (1000)    10476 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/migrations/migrate_to_4200.py
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-05-15 10:51:15.019923 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/model/
--rw-rw-r--   0 oli       (1000) oli       (1000)        0 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/model/__init__.py
--rw-rw-r--   0 oli       (1000) oli       (1000)        0 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/model/pm_updates.py
--rw-rw-r--   0 oli       (1000) oli       (1000)      946 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/overrides.zcml
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-05-15 10:51:15.019923 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/
--rw-rw-r--   0 oli       (1000) oli       (1000)       23 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/__init__.py
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-05-15 10:51:15.019923 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/default/
--rw-rw-r--   0 oli       (1000) oli       (1000)      177 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/default/MeetingCPASLalouviere_marker.txt
--rw-rw-r--   0 oli       (1000) oli       (1000)        0 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/default/__init__.py
--rw-rw-r--   0 oli       (1000) oli       (1000)      768 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/default/cssregistry.xml
--rw-rw-r--   0 oli       (1000) oli       (1000)      824 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/default/import_steps.xml
--rw-rw-r--   0 oli       (1000) oli       (1000)      423 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/default/jsregistry.xml
--rw-rw-r--   0 oli       (1000) oli       (1000)      246 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/default/metadata.xml
--rw-rw-r--   0 oli       (1000) oli       (1000)      601 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/default/rolemap.xml
--rw-rw-r--   0 oli       (1000) oli       (1000)      999 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/default/skins.xml
--rw-rw-r--   0 oli       (1000) oli       (1000)      167 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/default/toolset.xml
--rw-rw-r--   0 oli       (1000) oli       (1000)      931 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/default/workflows.xml
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-05-15 10:51:15.023923 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/testing/
--rw-rw-r--   0 oli       (1000) oli       (1000)      177 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/testing/MeetingCPASLalouviere_testing_marker.txt
--rw-rw-r--   0 oli       (1000) oli       (1000)        0 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/testing/__init__.py
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-05-15 10:51:15.023923 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/testing/images/
--rw-rw-r--   0 oli       (1000) oli       (1000)     3352 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/testing/images/attach.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      630 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/testing/images/budget.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      492 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/testing/images/budgetAnalysis.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      731 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/testing/images/cahier.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      216 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/testing/images/decisionAnnex.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      742 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/testing/images/financialAnalysis.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      216 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/testing/images/itemAnnex.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      332 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/testing/images/legalAnalysis.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      411 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/testing/images/negative.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      880 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/testing/images/overheadAnalysis.png
--rw-rw-r--   0 oli       (1000) oli       (1000)     1147 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/testing/images/positive.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      355 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/testing/images/remarks.png
--rwxrwxr-x   0 oli       (1000) oli       (1000)     2791 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/testing/import_data.py
--rwxrwxr-x   0 oli       (1000) oli       (1000)      361 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/testing/import_steps.xml
--rw-rw-r--   0 oli       (1000) oli       (1000)      180 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/testing/metadata.xml
--rwxrwxr-x   0 oli       (1000) oli       (1000)      167 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/testing/toolset.xml
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-05-15 10:51:15.023923 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/
--rw-rw-r--   0 oli       (1000) oli       (1000)      177 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/MeetingCPASLalouviere_lalouviere_marker.txt
--rw-rw-r--   0 oli       (1000) oli       (1000)        0 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/__init__.py
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-05-15 10:51:15.027922 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/
--rw-rw-r--   0 oli       (1000) oli       (1000)     3352 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/attach.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      630 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/budget.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      492 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/budgetAnalysis.png
--rw-rw-r--   0 oli       (1000) oli       (1000)     1032 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/cahier.gif
--rw-rw-r--   0 oli       (1000) oli       (1000)      731 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/cahier.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      216 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/decisionAnnex.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      742 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/financialAnalysis.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      216 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/itemAnnex.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      761 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/legalAdvice.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      332 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/legalAnalysis.png
--rw-rw-r--   0 oli       (1000) oli       (1000)     3555 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/logo.gif
--rw-rw-r--   0 oli       (1000) oli       (1000)      885 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/negative.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      305 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/nil.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      880 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/overheadAnalysis.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      583 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/positive.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      705 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/remarks.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      730 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/secretary_remarks.png
--rwxrwxr-x   0 oli       (1000) oli       (1000)     1663 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/import_data.py
--rwxrwxr-x   0 oli       (1000) oli       (1000)     1015 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/import_steps.xml
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-05-15 10:51:15.027922 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/
--rw-rw-r--   0 oli       (1000) oli       (1000)     9511 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/all_delib.odt
--rw-rw-r--   0 oli       (1000) oli       (1000)     9909 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/all_delib_recto_verso.odt
--rw-rw-r--   0 oli       (1000) oli       (1000)     9605 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/all_pv.odt
--rw-rw-r--   0 oli       (1000) oli       (1000)    12386 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/attendance-stats.ods
--rw-rw-r--   0 oli       (1000) oli       (1000)    17906 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/attendees.odt
--rw-rw-r--   0 oli       (1000) oli       (1000)    18256 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/avis-df.odt
--rw-rw-r--   0 oli       (1000) oli       (1000)    22380 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/council-oj.odt
--rw-rw-r--   0 oli       (1000) oli       (1000)    22958 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/council-pv.odt
--rw-rw-r--   0 oli       (1000) oli       (1000)    12890 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/council-rapport.odt
--rw-rw-r--   0 oli       (1000) oli       (1000)    13154 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/dashboard.ods
--rw-rw-r--   0 oli       (1000) oli       (1000)    32698 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/deliberation.odt
--rw-rw-r--   0 oli       (1000) oli       (1000)    32449 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/deliberation_recto_verso.odt
--rw-rw-r--   0 oli       (1000) oli       (1000)     9652 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/history.odt
--rw-rw-r--   0 oli       (1000) oli       (1000)    12705 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/meeting_assemblies.odt
--rw-rw-r--   0 oli       (1000) oli       (1000)    24785 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/oj-avec-annexes.odt
--rw-rw-r--   0 oli       (1000) oli       (1000)    24316 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/oj-avec-table-des-matieres.odt
--rw-rw-r--   0 oli       (1000) oli       (1000)    24585 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/oj.odt
--rw-rw-r--   0 oli       (1000) oli       (1000)    12170 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/organizations-export.ods
--rw-rw-r--   0 oli       (1000) oli       (1000)    16342 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/publications.odt
--rw-rw-r--   0 oli       (1000) oli       (1000)    23881 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/pv.odt
--rw-rw-r--   0 oli       (1000) oli       (1000)    12630 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/recapitulatif-tb.ods
--rw-rw-r--   0 oli       (1000) oli       (1000)    11565 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/recapitulatif-tb.odt
--rw-rw-r--   0 oli       (1000) oli       (1000)    13706 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/report.odt
--rw-rw-r--   0 oli       (1000) oli       (1000)    10369 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/styles1.odt
--rw-rw-r--   0 oli       (1000) oli       (1000)    12815 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/styles2.odt
--rw-rw-r--   0 oli       (1000) oli       (1000)    18137 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/synthese-avis-df.odt
--rw-rw-r--   0 oli       (1000) oli       (1000)    14290 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/synthese-df-tb.ods
--rw-rw-r--   0 oli       (1000) oli       (1000)    13865 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/users-groups-export.ods
--rw-rw-r--   0 oli       (1000) oli       (1000)    14862 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/votes.odt
--rwxrwxr-x   0 oli       (1000) oli       (1000)      167 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/toolset.xml
--rw-rw-r--   0 oli       (1000) oli       (1000)     1360 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles.zcml
--rw-rw-r--   0 oli       (1000) oli       (1000)        0 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/refresh.txt
--rw-rw-r--   0 oli       (1000) oli       (1000)     4388 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/setuphandlers.py
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-05-15 10:51:15.011922 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/skins/
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-05-15 10:51:15.031922 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/
--rw-rw-r--   0 oli       (1000) oli       (1000)      329 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/ask_advices_by_itemcreator.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      649 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/backToPresented.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      649 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/backToProposedToN1.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      649 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/backToProposedToN2.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      649 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/backToProposedToPresident.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      649 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/backToProposedToSecretaire.png
--rw-rw-r--   0 oli       (1000) oli       (1000)     6337 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/backTo_itemcreated_from_proposed_to_budget_reviewer.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      343 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/cdld.gif
--rw-rw-r--   0 oli       (1000) oli       (1000)      737 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/proposeToBudgetImpactReviewer.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      638 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/proposeToN1.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      608 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/proposeToN2.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      626 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/proposeToPresident.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      626 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/proposeToSecretaire.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      610 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/validate.png
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-05-15 10:51:15.031922 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_styles/
--rw-rw-r--   0 oli       (1000) oli       (1000)     1557 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_styles/imioapps_properties.props
--rw-rw-r--   0 oli       (1000) oli       (1000)     1425 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_styles/meetingcpaslalouviere.css
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-05-15 10:51:15.031922 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_templates/
--rw-rw-r--   0 oli       (1000) oli       (1000)      424 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_templates/isAReviewer.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     1044 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/testing.py
--rw-rw-r--   0 oli       (1000) oli       (1000)      624 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/testing.zcml
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-05-15 10:51:15.035923 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/tests/
--rwxrwxr-x   0 oli       (1000) oli       (1000)     1447 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/tests/MeetingCPASLalouviereTestCase.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     1293 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/tests/__init__.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     4864 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/tests/helpers.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     1392 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/tests/testAdvices.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     1259 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/tests/testAnnexes.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     1362 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/tests/testChangeItemOrderView.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     1253 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/tests/testColumns.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     1298 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/tests/testContacts.py
--rwxrwxr-x   0 oli       (1000) oli       (1000)      537 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/tests/testCustomMeeting.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     1281 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/tests/testCustomMeetingConfig.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     1351 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/tests/testCustomMeetingItem.py
--rw-rw-r--   0 oli       (1000) oli       (1000)      365 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/tests/testCustomSearches.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     1376 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/tests/testCustomToolPloneMeeting.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     1318 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/tests/testCustomUtils.py
--rw-rw-r--   0 oli       (1000) oli       (1000)      506 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/tests/testCustomViews.py
--rw-rw-r--   0 oli       (1000) oli       (1000)      497 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/tests/testCustomWFAdaptations.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     1365 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/tests/testCustomWorkflows.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     1286 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/tests/testFaceted.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     1311 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/tests/testMeeting.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     1339 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/tests/testMeetingCategory.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     4834 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/tests/testMeetingConfig.py
--rwxrwxr-x   0 oli       (1000) oli       (1000)     1655 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/tests/testMeetingItem.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     1299 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/tests/testPortlets.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     9198 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/tests/testSearches.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     1290 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/tests/testSetup.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     1344 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/tests/testToolPloneMeeting.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     2862 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/tests/testUtils.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     1302 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/tests/testValidators.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     1248 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/tests/testViews.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     1246 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/tests/testVotes.py
--rw-rw-r--   0 oli       (1000) oli       (1000)    16671 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/tests/testWFAdaptations.py
--rwxrwxr-x   0 oli       (1000) oli       (1000)     7170 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/tests/testWorkflows.py
--rw-rw-r--   0 oli       (1000) oli       (1000)       11 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/version.txt
--rw-rw-r--   0 oli       (1000) oli       (1000)       56 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products/__init__.py
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-05-15 10:51:15.015922 Products.MeetingCPASLalouviere-4.2.0a3/src/Products.MeetingCPASLalouviere.egg-info/
--rw-rw-r--   0 oli       (1000) oli       (1000)     3451 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products.MeetingCPASLalouviere.egg-info/PKG-INFO
--rw-rw-r--   0 oli       (1000) oli       (1000)    12001 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products.MeetingCPASLalouviere.egg-info/SOURCES.txt
--rw-rw-r--   0 oli       (1000) oli       (1000)        1 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products.MeetingCPASLalouviere.egg-info/dependency_links.txt
--rw-rw-r--   0 oli       (1000) oli       (1000)        9 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products.MeetingCPASLalouviere.egg-info/namespace_packages.txt
--rw-rw-r--   0 oli       (1000) oli       (1000)        1 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products.MeetingCPASLalouviere.egg-info/not-zip-safe
--rw-rw-r--   0 oli       (1000) oli       (1000)      139 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products.MeetingCPASLalouviere.egg-info/requires.txt
--rw-rw-r--   0 oli       (1000) oli       (1000)        9 2023-05-15 10:51:14.000000 Products.MeetingCPASLalouviere-4.2.0a3/src/Products.MeetingCPASLalouviere.egg-info/top_level.txt
+drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-05-16 14:32:29.986252 Products.MeetingCPASLalouviere-4.2.0a4/
+-rw-rw-r--   0 oli       (1000) oli       (1000)     2992 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/CHANGES.rst
+-rw-rw-r--   0 oli       (1000) oli       (1000)      353 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/MANIFEST.in
+-rw-rw-r--   0 oli       (1000) oli       (1000)     3632 2023-05-16 14:32:29.986252 Products.MeetingCPASLalouviere-4.2.0a4/PKG-INFO
+-rw-rw-r--   0 oli       (1000) oli       (1000)       23 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/README.rst
+drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-05-16 14:32:29.974252 Products.MeetingCPASLalouviere-4.2.0a4/docs/
+-rw-rw-r--   0 oli       (1000) oli       (1000)    18092 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/docs/LICENSE.GPL
+-rw-rw-r--   0 oli       (1000) oli       (1000)      734 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/docs/LICENSE.txt
+-rw-rw-r--   0 oli       (1000) oli       (1000)     1121 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/docs/MIGRATION.txt
+-rw-rw-r--   0 oli       (1000) oli       (1000)       38 2023-05-16 14:32:29.986252 Products.MeetingCPASLalouviere-4.2.0a4/setup.cfg
+-rw-rw-r--   0 oli       (1000) oli       (1000)     1248 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/setup.py
+drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-05-16 14:32:29.970252 Products.MeetingCPASLalouviere-4.2.0a4/src/
+drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-05-16 14:32:29.974252 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/
+drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-05-16 14:32:29.974252 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/
+-rw-rw-r--   0 oli       (1000) oli       (1000)      981 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/README.txt
+-rw-rw-r--   0 oli       (1000) oli       (1000)     1773 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/__init__.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)    14191 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/adapters.py
+drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-05-16 14:32:29.974252 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/browser/
+-rw-rw-r--   0 oli       (1000) oli       (1000)        0 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/browser/__init__.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)      177 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/browser/configure.zcml
+-rw-rw-r--   0 oli       (1000) oli       (1000)      120 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/browser/overrides.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)      805 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/browser/views.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)     3223 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/config.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)      724 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/configure.zcml
+-rw-rw-r--   0 oli       (1000) oli       (1000)      615 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/events.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)     3719 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/interfaces.py
+drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-05-16 14:32:29.974252 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/locales/
+-rw-rw-r--   0 oli       (1000) oli       (1000)     1794 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/locales/PloneMeeting.pot
+drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-05-16 14:32:29.970252 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/locales/en/
+drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-05-16 14:32:29.974252 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/locales/en/LC_MESSAGES/
+-rw-rw-r--   0 oli       (1000) oli       (1000)     1206 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/locales/en/LC_MESSAGES/PloneMeeting.po
+-rw-rw-r--   0 oli       (1000) oli       (1000)     2089 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/locales/en/LC_MESSAGES/plone.po
+drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-05-16 14:32:29.970252 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/locales/fr/
+drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-05-16 14:32:29.974252 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/locales/fr/LC_MESSAGES/
+-rw-rw-r--   0 oli       (1000) oli       (1000)     2226 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/locales/fr/LC_MESSAGES/PloneMeeting.po
+-rw-rw-r--   0 oli       (1000) oli       (1000)     2939 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/locales/fr/LC_MESSAGES/plone.po
+-rw-rw-r--   0 oli       (1000) oli       (1000)     1970 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/locales/plone.pot
+-rwxrwxr-x   0 oli       (1000) oli       (1000)      267 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/locales/sync_pos.sh
+drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-05-16 14:32:29.974252 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/migrations/
+-rw-rw-r--   0 oli       (1000) oli       (1000)        0 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/migrations/__init__.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)    10643 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/migrations/migrate_to_4200.py
+drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-05-16 14:32:29.974252 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/model/
+-rw-rw-r--   0 oli       (1000) oli       (1000)        0 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/model/__init__.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)     1627 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/model/pm_updates.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)      946 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/overrides.zcml
+drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-05-16 14:32:29.974252 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/
+-rw-rw-r--   0 oli       (1000) oli       (1000)       23 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/__init__.py
+drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-05-16 14:32:29.974252 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/default/
+-rw-rw-r--   0 oli       (1000) oli       (1000)      177 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/default/MeetingCPASLalouviere_marker.txt
+-rw-rw-r--   0 oli       (1000) oli       (1000)        0 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/default/__init__.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)      768 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/default/cssregistry.xml
+-rw-rw-r--   0 oli       (1000) oli       (1000)      824 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/default/import_steps.xml
+-rw-rw-r--   0 oli       (1000) oli       (1000)      423 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/default/jsregistry.xml
+-rw-rw-r--   0 oli       (1000) oli       (1000)      246 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/default/metadata.xml
+-rw-rw-r--   0 oli       (1000) oli       (1000)      601 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/default/rolemap.xml
+-rw-rw-r--   0 oli       (1000) oli       (1000)      999 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/default/skins.xml
+-rw-rw-r--   0 oli       (1000) oli       (1000)      167 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/default/toolset.xml
+-rw-rw-r--   0 oli       (1000) oli       (1000)      931 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/default/workflows.xml
+drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-05-16 14:32:29.978252 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/testing/
+-rw-rw-r--   0 oli       (1000) oli       (1000)      177 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/testing/MeetingCPASLalouviere_testing_marker.txt
+-rw-rw-r--   0 oli       (1000) oli       (1000)        0 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/testing/__init__.py
+drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-05-16 14:32:29.978252 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/testing/images/
+-rw-rw-r--   0 oli       (1000) oli       (1000)     3352 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/testing/images/attach.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      630 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/testing/images/budget.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      492 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/testing/images/budgetAnalysis.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      731 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/testing/images/cahier.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      216 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/testing/images/decisionAnnex.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      742 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/testing/images/financialAnalysis.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      216 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/testing/images/itemAnnex.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      332 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/testing/images/legalAnalysis.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      411 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/testing/images/negative.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      880 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/testing/images/overheadAnalysis.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)     1147 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/testing/images/positive.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      355 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/testing/images/remarks.png
+-rwxrwxr-x   0 oli       (1000) oli       (1000)     2669 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/testing/import_data.py
+-rwxrwxr-x   0 oli       (1000) oli       (1000)      361 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/testing/import_steps.xml
+-rw-rw-r--   0 oli       (1000) oli       (1000)      180 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/testing/metadata.xml
+-rwxrwxr-x   0 oli       (1000) oli       (1000)      167 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/testing/toolset.xml
+drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-05-16 14:32:29.978252 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/
+-rw-rw-r--   0 oli       (1000) oli       (1000)      177 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/MeetingCPASLalouviere_lalouviere_marker.txt
+-rw-rw-r--   0 oli       (1000) oli       (1000)        0 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/__init__.py
+drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-05-16 14:32:29.978252 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/
+-rw-rw-r--   0 oli       (1000) oli       (1000)     3352 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/attach.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      630 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/budget.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      492 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/budgetAnalysis.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)     1032 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/cahier.gif
+-rw-rw-r--   0 oli       (1000) oli       (1000)      731 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/cahier.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      216 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/decisionAnnex.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      742 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/financialAnalysis.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      216 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/itemAnnex.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      761 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/legalAdvice.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      332 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/legalAnalysis.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)     3555 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/logo.gif
+-rw-rw-r--   0 oli       (1000) oli       (1000)      885 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/negative.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      305 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/nil.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      880 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/overheadAnalysis.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      583 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/positive.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      705 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/remarks.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      730 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/secretary_remarks.png
+-rwxrwxr-x   0 oli       (1000) oli       (1000)     1663 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/import_data.py
+-rwxrwxr-x   0 oli       (1000) oli       (1000)     1015 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/import_steps.xml
+drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-05-16 14:32:29.982252 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/
+-rw-rw-r--   0 oli       (1000) oli       (1000)     9511 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/all_delib.odt
+-rw-rw-r--   0 oli       (1000) oli       (1000)     9909 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/all_delib_recto_verso.odt
+-rw-rw-r--   0 oli       (1000) oli       (1000)     9605 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/all_pv.odt
+-rw-rw-r--   0 oli       (1000) oli       (1000)    12386 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/attendance-stats.ods
+-rw-rw-r--   0 oli       (1000) oli       (1000)    17906 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/attendees.odt
+-rw-rw-r--   0 oli       (1000) oli       (1000)    18256 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/avis-df.odt
+-rw-rw-r--   0 oli       (1000) oli       (1000)    22380 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/council-oj.odt
+-rw-rw-r--   0 oli       (1000) oli       (1000)    22958 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/council-pv.odt
+-rw-rw-r--   0 oli       (1000) oli       (1000)    12890 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/council-rapport.odt
+-rw-rw-r--   0 oli       (1000) oli       (1000)    13154 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/dashboard.ods
+-rw-rw-r--   0 oli       (1000) oli       (1000)    32698 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/deliberation.odt
+-rw-rw-r--   0 oli       (1000) oli       (1000)    32449 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/deliberation_recto_verso.odt
+-rw-rw-r--   0 oli       (1000) oli       (1000)     9652 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/history.odt
+-rw-rw-r--   0 oli       (1000) oli       (1000)    12705 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/meeting_assemblies.odt
+-rw-rw-r--   0 oli       (1000) oli       (1000)    24785 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/oj-avec-annexes.odt
+-rw-rw-r--   0 oli       (1000) oli       (1000)    24316 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/oj-avec-table-des-matieres.odt
+-rw-rw-r--   0 oli       (1000) oli       (1000)    24585 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/oj.odt
+-rw-rw-r--   0 oli       (1000) oli       (1000)    12170 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/organizations-export.ods
+-rw-rw-r--   0 oli       (1000) oli       (1000)    16342 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/publications.odt
+-rw-rw-r--   0 oli       (1000) oli       (1000)    23881 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/pv.odt
+-rw-rw-r--   0 oli       (1000) oli       (1000)    12630 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/recapitulatif-tb.ods
+-rw-rw-r--   0 oli       (1000) oli       (1000)    11565 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/recapitulatif-tb.odt
+-rw-rw-r--   0 oli       (1000) oli       (1000)    13706 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/report.odt
+-rw-rw-r--   0 oli       (1000) oli       (1000)    10369 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/styles1.odt
+-rw-rw-r--   0 oli       (1000) oli       (1000)    12815 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/styles2.odt
+-rw-rw-r--   0 oli       (1000) oli       (1000)    18137 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/synthese-avis-df.odt
+-rw-rw-r--   0 oli       (1000) oli       (1000)    14290 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/synthese-df-tb.ods
+-rw-rw-r--   0 oli       (1000) oli       (1000)    13865 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/users-groups-export.ods
+-rw-rw-r--   0 oli       (1000) oli       (1000)    14862 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/votes.odt
+-rwxrwxr-x   0 oli       (1000) oli       (1000)      167 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/toolset.xml
+-rw-rw-r--   0 oli       (1000) oli       (1000)     1361 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles.zcml
+-rw-rw-r--   0 oli       (1000) oli       (1000)        0 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/refresh.txt
+-rw-rw-r--   0 oli       (1000) oli       (1000)     4388 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/setuphandlers.py
+drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-05-16 14:32:29.970252 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/skins/
+drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-05-16 14:32:29.982252 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/
+-rw-rw-r--   0 oli       (1000) oli       (1000)      329 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/ask_advices_by_itemcreator.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      649 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/backToPresented.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      649 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/backToProposedToN1.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      649 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/backToProposedToN2.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      649 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/backToProposedToPresident.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      649 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/backToProposedToSecretaire.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)     6337 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/backTo_itemcreated_from_proposed_to_budget_reviewer.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      343 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/cdld.gif
+-rw-rw-r--   0 oli       (1000) oli       (1000)      737 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/proposeToBudgetImpactReviewer.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      638 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/proposeToN1.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      608 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/proposeToN2.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      626 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/proposeToPresident.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      626 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/proposeToSecretaire.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      610 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/validate.png
+drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-05-16 14:32:29.982252 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_styles/
+-rw-rw-r--   0 oli       (1000) oli       (1000)     1557 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_styles/imioapps_properties.props
+-rw-rw-r--   0 oli       (1000) oli       (1000)     1425 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_styles/meetingcpaslalouviere.css
+drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-05-16 14:32:29.982252 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_templates/
+-rw-rw-r--   0 oli       (1000) oli       (1000)     7737 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_templates/meetingitem_edit.pt
+-rw-rw-r--   0 oli       (1000) oli       (1000)    40254 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_templates/meetingitem_view.pt
+-rw-rw-r--   0 oli       (1000) oli       (1000)     1044 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/testing.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)      624 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/testing.zcml
+drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-05-16 14:32:29.986252 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/tests/
+-rwxrwxr-x   0 oli       (1000) oli       (1000)     1447 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/tests/MeetingCPASLalouviereTestCase.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)     1293 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/tests/__init__.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)     4864 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/tests/helpers.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)     1392 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/tests/testAdvices.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)     1259 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/tests/testAnnexes.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)     1362 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/tests/testChangeItemOrderView.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)     1253 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/tests/testColumns.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)     1298 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/tests/testContacts.py
+-rwxrwxr-x   0 oli       (1000) oli       (1000)      537 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/tests/testCustomMeeting.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)     1281 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/tests/testCustomMeetingConfig.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)     1351 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/tests/testCustomMeetingItem.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)      365 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/tests/testCustomSearches.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)     1376 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/tests/testCustomToolPloneMeeting.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)     1318 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/tests/testCustomUtils.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)      506 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/tests/testCustomViews.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)      497 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/tests/testCustomWFAdaptations.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)     1365 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/tests/testCustomWorkflows.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)     1286 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/tests/testFaceted.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)     1311 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/tests/testMeeting.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)     1339 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/tests/testMeetingCategory.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)     4834 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/tests/testMeetingConfig.py
+-rwxrwxr-x   0 oli       (1000) oli       (1000)     1729 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/tests/testMeetingItem.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)     1299 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/tests/testPortlets.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)     9198 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/tests/testSearches.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)     1290 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/tests/testSetup.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)     1344 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/tests/testToolPloneMeeting.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)     2862 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/tests/testUtils.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)     1302 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/tests/testValidators.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)     1248 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/tests/testViews.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)     1246 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/tests/testVotes.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)    17692 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/tests/testWFAdaptations.py
+-rwxrwxr-x   0 oli       (1000) oli       (1000)     7170 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/tests/testWorkflows.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)       11 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/version.txt
+-rw-rw-r--   0 oli       (1000) oli       (1000)       56 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products/__init__.py
+drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-05-16 14:32:29.974252 Products.MeetingCPASLalouviere-4.2.0a4/src/Products.MeetingCPASLalouviere.egg-info/
+-rw-rw-r--   0 oli       (1000) oli       (1000)     3632 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products.MeetingCPASLalouviere.egg-info/PKG-INFO
+-rw-rw-r--   0 oli       (1000) oli       (1000)    12099 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products.MeetingCPASLalouviere.egg-info/SOURCES.txt
+-rw-rw-r--   0 oli       (1000) oli       (1000)        1 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products.MeetingCPASLalouviere.egg-info/dependency_links.txt
+-rw-rw-r--   0 oli       (1000) oli       (1000)        9 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products.MeetingCPASLalouviere.egg-info/namespace_packages.txt
+-rw-rw-r--   0 oli       (1000) oli       (1000)        1 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products.MeetingCPASLalouviere.egg-info/not-zip-safe
+-rw-rw-r--   0 oli       (1000) oli       (1000)      139 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products.MeetingCPASLalouviere.egg-info/requires.txt
+-rw-rw-r--   0 oli       (1000) oli       (1000)        9 2023-05-16 14:32:29.000000 Products.MeetingCPASLalouviere-4.2.0a4/src/Products.MeetingCPASLalouviere.egg-info/top_level.txt
```

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/CHANGES.rst` & `Products.MeetingCPASLalouviere-4.2.0a4/CHANGES.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,23 @@
 Products.MeetingCPASLalouviere Changelog
 ====================================
 
 The Products.MeetingCommunes version must be the same as the Products.PloneMeeting version
 
+4.2.0a4 (2023-05-16)
+--------------------
+
+- Fix custom searches filters.
+  [odelaere]
+- Use legacy reviewers suffix.
+  [odelaere]
+- Added emergencyMotivation field.
+  [odelaere]
+
+
 4.2.0a3 (2023-05-15)
 --------------------
 
 - Fix proposed_to_budgetimpact_reviewer transition_mappings.
   [odelaere]
 - Added missing icon and translation.
   [odelaere]
```

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/PKG-INFO` & `Products.MeetingCPASLalouviere-4.2.0a4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Products.MeetingCPASLalouviere
-Version: 4.2.0a3
+Version: 4.2.0a4
 Summary: PloneMeeting profile for CPAS of La Louviere.
 Home-page: http://www.imio.be/produits/gestion-des-deliberations
 Author: Olivier Delaere
 Author-email: olivier.delaere@imio.be
 License: GPL
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
@@ -18,14 +18,25 @@
 
 Check 'docs/README.txt'
 Products.MeetingCPASLalouviere Changelog
 ====================================
 
 The Products.MeetingCommunes version must be the same as the Products.PloneMeeting version
 
+4.2.0a4 (2023-05-16)
+--------------------
+
+- Fix custom searches filters.
+  [odelaere]
+- Use legacy reviewers suffix.
+  [odelaere]
+- Added emergencyMotivation field.
+  [odelaere]
+
+
 4.2.0a3 (2023-05-15)
 --------------------
 
 - Fix proposed_to_budgetimpact_reviewer transition_mappings.
   [odelaere]
 - Added missing icon and translation.
   [odelaere]
```

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/docs/LICENSE.GPL` & `Products.MeetingCPASLalouviere-4.2.0a4/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/docs/LICENSE.txt` & `Products.MeetingCPASLalouviere-4.2.0a4/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/docs/MIGRATION.txt` & `Products.MeetingCPASLalouviere-4.2.0a4/docs/MIGRATION.txt`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/setup.py` & `Products.MeetingCPASLalouviere-4.2.0a4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-version = "4.2.0a3"
+version = "4.2.0a4"
 
 setup(name='Products.MeetingCPASLalouviere',
       version=version,
       description="PloneMeeting profile for CPAS of La Louviere.",
       long_description=open("README.rst").read() + "\n" + open("CHANGES.rst").read(),
       classifiers=[
           "Environment :: Web Environment",
```

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/README.txt` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/README.txt`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/__init__.py` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/__init__.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/adapters.py` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/adapters.py`

 * *Files 6% similar despite different names*

```diff
@@ -101,19 +101,24 @@
                             "v": [itemType, ],
                         },
                         {
                             "i": "review_state",
                             "o": "plone.app.querystring.operation.selection.is",
                             "v": ["proposed_to_n1"],
                         },
+                        {
+                            'i': 'CompoundCriterion',
+                            'o': 'plone.app.querystring.operation.compound.is',
+                            'v': ['items-of-my-groups']
+                        },
                     ],
                     "sort_on": u"modified",
                     "sort_reversed": True,
                     "showNumberOfItems": True,
-                    "tal_condition": "python:tool.userIsAmong(['n1', 'n2', 'secretaire', 'president'])",
+                    "tal_condition": "python:tool.userIsAmong(['n1', 'n2', 'secretaire', 'reviewers'])",
                     "roles_bypassing_talcondition": ["Manager", ],
                 },
             ),
             (
                 "searchproposedton2",
                 {
                     "subFolderId": "searches_items",
@@ -125,19 +130,24 @@
                             "v": [itemType, ],
                         },
                         {
                             "i": "review_state",
                             "o": "plone.app.querystring.operation.selection.is",
                             "v": ["proposed_to_n2"],
                         },
+                        {
+                            'i': 'CompoundCriterion',
+                            'o': 'plone.app.querystring.operation.compound.is',
+                            'v': ['items-of-my-groups']
+                        },
                     ],
                     "sort_on": u"modified",
                     "sort_reversed": True,
                     "showNumberOfItems": True,
-                    "tal_condition": "python:tool.userIsAmong(['n2', 'secretaire', 'president'])",
+                    "tal_condition": "python:tool.userIsAmong(['n2', 'secretaire', 'reviewers'])",
                     "roles_bypassing_talcondition": ["Manager", ],
                 },
             ),
             (
                 "searchproposedtosecretaire",
                 {
                     "subFolderId": "searches_items",
@@ -149,19 +159,24 @@
                             "v": [itemType, ],
                         },
                         {
                             "i": "review_state",
                             "o": "plone.app.querystring.operation.selection.is",
                             "v": ["proposed_to_secretaire"],
                         },
+                        {
+                            'i': 'CompoundCriterion',
+                            'o': 'plone.app.querystring.operation.compound.is',
+                            'v': ['items-of-my-groups']
+                        },
                     ],
                     "sort_on": u"modified",
                     "sort_reversed": True,
                     "showNumberOfItems": True,
-                    "tal_condition": "python:tool.userIsAmong(['secretaire', 'president'])",
+                    "tal_condition": "python:tool.userIsAmong(['secretaire', 'reviewers'])",
                     "roles_bypassing_talcondition": ["Manager", ],
                 },
             ),
             (
                 "searchproposedtopresident",
                 {
                     "subFolderId": "searches_items",
@@ -173,32 +188,37 @@
                             "v": [itemType, ],
                         },
                         {
                             "i": "review_state",
                             "o": "plone.app.querystring.operation.selection.is",
                             "v": ["proposed_to_president"],
                         },
+                        {
+                            'i': 'CompoundCriterion',
+                            'o': 'plone.app.querystring.operation.compound.is',
+                            'v': ['items-of-my-groups']
+                        },
                     ],
                     "sort_on": u"modified",
                     "sort_reversed": True,
                     "showNumberOfItems": True,
-                    "tal_condition": "python:tool.userIsAmong(['president'])",
+                    "tal_condition": "python:tool.userIsAmong(['reviewers'])",
                     "roles_bypassing_talcondition": ["Manager", ],
                 },
             ),
         ]
         infos.update(OrderedDict(extra_infos))
         return infos
 
     def _custom_reviewersFor(self):
         '''Manage reviewersFor Bourgmestre because as some 'creators' suffixes are
            used after reviewers levels, this break the _highestReviewerLevel and other
            related hierarchic level functionalities.'''
         reviewers = [
-            ('president', ['proposed_to_president',
+            ('reviewers', ['proposed_to_president',
                            'proposed_to_secretaire',
                            'proposed_to_n2',
                            'proposed_to_n1',
                            ]),
             ('secretaire',
              ['proposed_to_secretaire',
               'proposed_to_n2',
```

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/browser/views.py` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/browser/views.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/config.py` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/config.py`

 * *Files 13% similar despite different names*

```diff
@@ -36,71 +36,64 @@
     {
         "fct_id": u"secretaire",
         "fct_title": u"Secrétaire",
         "fct_orgs": [],
         "enabled": True,
         "fct_management": False,
     },
-    {
-        "fct_id": u"president",
-        "fct_title": u"Président",
-        "fct_orgs": [],
-        "enabled": True,
-        "fct_management": False,
-    },
 ]
 
 LLO_ITEM_CPAS_WF_VALIDATION_LEVELS = (
     {'state': 'itemcreated',
      'state_title': 'itemcreated',
      'leading_transition': '-',
      'leading_transition_title': '-',
      'back_transition': 'backToItemCreated',
      'back_transition_title': 'backToItemCreated',
      'suffix': 'creators',
-     'extra_suffixes': ['n1', 'n2', 'secretaire', 'president'],
+     'extra_suffixes': ['n1', 'n2', 'secretaire', 'reviewers'],
      'enabled': '1',
      },
     {'state': 'proposed_to_n1',
      'state_title': 'proposed_to_n1',
      'leading_transition': 'proposeToN1',
      'leading_transition_title': 'proposeToN1',
      'back_transition': 'backToProposedToN1',
      'back_transition_title': 'backToProposedToN1',
      'suffix': 'n1',
-     'extra_suffixes': ['n2', 'secretaire', 'president'],
+     'extra_suffixes': ['n2', 'secretaire', 'reviewers'],
      'enabled': '1',
      },
     {'state': 'proposed_to_n2',
      'state_title': 'proposed_to_n2',
      'leading_transition': 'proposeToN2',
      'leading_transition_title': 'proposeToN2',
      'back_transition': 'backToProposedToN2',
      'back_transition_title': 'backToProposedToN2',
      'suffix': 'n2',
      'enabled': '1',
-     'extra_suffixes': ['secretaire', 'president'],
+     'extra_suffixes': ['secretaire', 'reviewers'],
      },
     {'state': 'proposed_to_secretaire',
      'state_title': 'proposed_to_secretaire',
      'leading_transition': 'proposeToSecretaire',
      'leading_transition_title': 'proposeToSecretaire',
      'back_transition': 'backToProposedToSecretaire',
      'back_transition_title': 'backToProposedToSecretaire',
      'suffix': 'secretaire',
      'enabled': '1',
-     'extra_suffixes': ['president'],
+     'extra_suffixes': ['reviewers'],
      },
     {'state': 'proposed_to_president',
      'state_title': 'proposed_to_president',
      'leading_transition': 'proposeToPresident',
      'leading_transition_title': 'proposeToPresident',
      'back_transition': 'backToProposedToPresident',
      'back_transition_title': 'backToProposedToPresident',
-     'suffix': 'president',
+     'suffix': 'reviewers',
      'enabled': '1',
      'extra_suffixes': [],
      },
 )
 
 LLO_APPLYED_CPAS_WFA = (
     "accepted_but_modified",
```

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/configure.zcml` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/configure.zcml`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/events.py` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/events.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/interfaces.py` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/interfaces.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/locales/PloneMeeting.pot` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/locales/PloneMeeting.pot`

 * *Files 3% similar despite different names*

```diff
@@ -36,22 +36,14 @@
 msgid "n2"
 msgstr ""
 
 # Suffix
 msgid "secretaire"
 msgstr ""
 
-#. Default: "Default value for the 'motivation' field"
-msgid "PloneMeeting_label_defaultMeetingItemMotivation"
-msgstr ""
-
-#. Default: "Motivation"
-msgid "PloneMeeting_label_emergency_motivation"
-msgstr ""
-
 #. Default: "Define here some predefined text that will be present in field 'motivation' every time a user creates a new item."
 msgid "config_default_meetingitem_motivation_descr"
 msgstr ""
 
 #. Default: "Items proposed to budget"
 msgid "searchproposedtobudgetreviewer"
 msgstr ""
@@ -86,8 +78,12 @@
 
 #. Default: "Items proposed to ceo"
 msgid "searchproposedtosecretaire"
 msgstr ""
 
 #. Default: "Items proposed to president"
 msgid "searchproposedtopresident"
-msgstr ""
+msgstr ""
+
+#. Default: "Emergency Motivation"
+msgid "MeetingCPASLalouviere_label_emergencyMotivation"
+msgstr ""
```

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/locales/en/LC_MESSAGES/PloneMeeting.po` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/locales/en/LC_MESSAGES/PloneMeeting.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/locales/en/LC_MESSAGES/plone.po` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/locales/en/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/locales/fr/LC_MESSAGES/PloneMeeting.po` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/locales/fr/LC_MESSAGES/PloneMeeting.po`

 * *Files 6% similar despite different names*

```diff
@@ -14,22 +14,14 @@
 "Preferred-Encodings: utf-8 latin1\n"
 "Domain: PloneMeeting\n"
 "Language-code: fr\n"
 "Language-name: French\n"
 "Preferred-encodings: utf-8 latin1\n"
 "X-is-fallback-for: fr-be fr-ca fr-lu fr-mc fr-ch fr-fr\n"
 
-#. Default: "Default value for the 'motivation' field"
-msgid "PloneMeeting_label_defaultMeetingItemMotivation"
-msgstr "Valeur par défaut du champ 'Motivation de l'urgence'"
-
-#. Default: "Motivation"
-msgid "PloneMeeting_label_emergency_motivation"
-msgstr "Motivation de l'urgence"
-
 # Suffix
 #. Default: "budget impact reviewers"
 msgid "budgetimpactreviewers"
 msgstr "correspondants financier"
 
 #. Default: "Define here some predefined text that will be present in field 'motivation' every time a user creates a new item."
 msgid "config_default_meetingitem_motivation_descr"
@@ -78,8 +70,12 @@
 
 #. Default: "Items proposed to ceo"
 msgid "searchproposedtosecretaire"
 msgstr "Points proposés au Secrétaire"
 
 #. Default: "Items proposed to president"
 msgid "searchproposedtopresident"
-msgstr "Points proposés au Président"
+msgstr "Points proposés au Président"
+
+#. Default: "Emergency Motivation"
+msgid "MeetingCPASLalouviere_label_emergencyMotivation"
+msgstr "Motivation de l'urgence"
```

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/locales/fr/LC_MESSAGES/plone.po` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/locales/fr/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/locales/plone.pot` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/locales/plone.pot`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/migrations/migrate_to_4200.py` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/migrations/migrate_to_4200.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,25 +7,30 @@
 from Products.MeetingCommunes.migrations.migrate_to_4200 import Migrate_To_4200 as MCMigrate_To_4200
 from Products.MeetingCPASLalouviere.config import LLO_APPLYED_CPAS_WFA
 from Products.MeetingCPASLalouviere.config import LLO_ITEM_CPAS_WF_VALIDATION_LEVELS
 import logging
 
 logger = logging.getLogger('MeetingCPASLalouviere')
 
+# TODO patch item to use emergencyMotivation instead of motivation
 
 class Migrate_To_4200(MCMigrate_To_4200):
 
     def _applyMeetingConfig_fixtures(self):
         logger.info('applying meetingconfig fixtures...')
         self.updateTALConditions("year()", "year")
         self.updateTALConditions("month()", "month")
         logger.info("Adapting 'meetingWorkflow/meetingItemWorkflow' for every MeetingConfigs...")
         for cfg in self.tool.objectValues('MeetingConfig'):
             used_item_attr = list(cfg.getUsedItemAttributes())
             used_item_attr.append("votesResult")
+
+            if "cas" in cfg.getId():
+                used_item_attr.append("emergencyMotivation")
+
             cfg.setUsedItemAttributes(tuple(used_item_attr))
             cfg.setWorkflowAdaptations(LLO_APPLYED_CPAS_WFA)
             # replace action and review_state column by async actions
             self.updateColumns(to_replace={'actions': 'async_actions',
                                            'review_state': 'review_state_title',})
             # cfg.setItemBudgetInfosStates(self.replace_in_list(u'proposed_to_budgetimpact_reviewer',
             #                                                   u'proposed_to_budget_reviewer',
```

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/overrides.zcml` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/overrides.zcml`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/default/cssregistry.xml` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/default/cssregistry.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/default/import_steps.xml` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/default/import_steps.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/default/rolemap.xml` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/default/rolemap.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/default/skins.xml` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/default/skins.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/default/workflows.xml` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/default/workflows.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/testing/images/attach.png` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/testing/images/attach.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/testing/images/budget.png` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/testing/images/budget.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/testing/images/cahier.png` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/testing/images/cahier.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/testing/images/financialAnalysis.png` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/testing/images/financialAnalysis.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/testing/images/overheadAnalysis.png` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/testing/images/overheadAnalysis.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/testing/images/positive.png` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/testing/images/positive.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/testing/import_data.py` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/testing/import_data.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 
 from Products.MeetingCPASLalouviere.config import LLO_ITEM_CPAS_WF_VALIDATION_LEVELS
 
 data = deepcopy(mc_import_data.data)
 
 # Inherited users
 pmReviewer1 = pm_import_data.pmReviewer1
-pmReviewer2 = pm_import_data.pmReviewer2
 pmReviewerLevel1 = pm_import_data.pmReviewerLevel1
 pmReviewerLevel2 = pm_import_data.pmReviewerLevel2
 pmManager = pm_import_data.pmManager
 # xxx specific to CPAS La louvière
 pmN1 = UserDescriptor('pmN1', [])
 pmN2 = UserDescriptor('pmN2', [])
 pmSecretaire = UserDescriptor('pmSecretaire', [])
@@ -29,25 +28,23 @@
 developers.budgetimpactreviewers.append(pmBudgetReviewer1)
 developers.n1.append(pmReviewerLevel1)
 developers.n1.append(pmN1)
 developers.n2.append(pmN2)
 developers.n2.append(pmManager)
 developers.secretaire.append(pmSecretaire)
 developers.secretaire.append(pmManager)
-developers.president.append(pmReviewer1)
-developers.president.append(pmReviewerLevel2)
-developers.president.append(pmManager)
-developers.president.append(pmPresident)
+developers.reviewers.append(pmReviewer1)
+developers.reviewers.append(pmReviewerLevel2)
+developers.reviewers.append(pmManager)
+developers.reviewers.append(pmPresident)
 
 vendors = data.orgs[1]
 vendors.budgetimpactreviewers.append(pmBudgetReviewer2)
 vendors.n1.append(pmReviewerLevel1)
 vendors.secretaire.append(pmSecretaire)
-vendors.president.append(pmReviewerLevel2)
-vendors.president.append(pmReviewer2)
 
 # Meeting configurations -------------------------------------------------------
 # College communal
 bpMeeting = deepcopy(mc_import_data.collegeMeeting)
 bpMeeting.id = 'meeting-config-bp'
 bpMeeting.title = 'Bureau Permanent'
 bpMeeting.folderTitle = 'Bureau Permanent'
```

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/attach.png` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/attach.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/budget.png` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/budget.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/cahier.gif` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/cahier.gif`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/cahier.png` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/cahier.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/financialAnalysis.png` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/financialAnalysis.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/legalAdvice.png` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/legalAdvice.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/logo.gif` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/logo.gif`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/negative.png` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/negative.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/overheadAnalysis.png` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/overheadAnalysis.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/positive.png` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/positive.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/remarks.png` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/remarks.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/secretary_remarks.png` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/secretary_remarks.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/import_data.py` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/import_data.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/import_steps.xml` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/import_steps.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/all_delib.odt` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/all_delib.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/all_delib_recto_verso.odt` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/all_delib_recto_verso.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/all_pv.odt` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/all_pv.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/attendance-stats.ods` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/attendance-stats.ods`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/attendees.odt` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/attendees.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/avis-df.odt` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/avis-df.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/council-oj.odt` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/council-oj.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/council-pv.odt` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/council-pv.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/council-rapport.odt` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/council-rapport.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/dashboard.ods` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/dashboard.ods`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/deliberation.odt` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/deliberation.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/deliberation_recto_verso.odt` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/deliberation_recto_verso.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/history.odt` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/history.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/meeting_assemblies.odt` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/meeting_assemblies.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/oj-avec-annexes.odt` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/oj-avec-annexes.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/oj-avec-table-des-matieres.odt` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/oj-avec-table-des-matieres.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/oj.odt` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/oj.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/organizations-export.ods` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/organizations-export.ods`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/publications.odt` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/publications.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/pv.odt` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/pv.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/recapitulatif-tb.ods` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/recapitulatif-tb.ods`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/recapitulatif-tb.odt` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/recapitulatif-tb.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/report.odt` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/report.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/styles1.odt` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/styles1.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/styles2.odt` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/styles2.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/synthese-avis-df.odt` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/synthese-avis-df.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/synthese-df-tb.ods` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/synthese-df-tb.ods`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/users-groups-export.ods` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/users-groups-export.ods`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/votes.odt` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/votes.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/profiles.zcml` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/profiles.zcml`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
       title="PloneMeeting / For CPAS La Louviere"
       directory="profiles/zlalouvierecpas"
       description="PloneMeeting for BP and CAS of La Louviere"
       provides="Products.GenericSetup.interfaces.EXTENSION"
       for="Products.CMFPlone.interfaces.IPloneSiteRoot"/>
 
   <genericsetup:upgradeStep
-      title="Go to MeetingCPASLalouviere 4.1"
+      title="Go to MeetingCPASLalouviere 4200"
       description=""
       source="4.1.1rc1"
       destination="4200"
       handler="Products.MeetingCPASLalouviere.migrations.migrate_to_4200.migrate"
       profile="Products.MeetingCPASLalouviere:default"/>
 
   <!-- ##/code-section profiles.zcml-bottom -->
```

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/setuphandlers.py` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/backToPresented.png` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/backToPresented.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/backToProposedToN1.png` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/backToProposedToN1.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/backToProposedToN2.png` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/backToProposedToN2.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/backToProposedToPresident.png` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/backToProposedToPresident.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/backToProposedToSecretaire.png` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/backToProposedToSecretaire.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/backTo_itemcreated_from_proposed_to_budget_reviewer.png` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/backTo_itemcreated_from_proposed_to_budget_reviewer.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/proposeToBudgetImpactReviewer.png` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/proposeToBudgetImpactReviewer.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/proposeToN1.png` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/proposeToN1.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/proposeToN2.png` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/proposeToN2.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/proposeToPresident.png` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/proposeToPresident.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/proposeToSecretaire.png` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/proposeToSecretaire.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/validate.png` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/validate.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_styles/imioapps_properties.props` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_styles/imioapps_properties.props`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_styles/meetingcpaslalouviere.css` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_styles/meetingcpaslalouviere.css`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/testing.py` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/testing.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/testing.zcml` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/testing.zcml`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/tests/MeetingCPASLalouviereTestCase.py` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/tests/MeetingCPASLalouviereTestCase.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/tests/__init__.py` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/tests/helpers.py` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/tests/testAdvices.py` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/tests/testAdvices.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/tests/testAnnexes.py` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/tests/testAnnexes.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/tests/testChangeItemOrderView.py` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/tests/testChangeItemOrderView.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/tests/testColumns.py` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/tests/testColumns.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/tests/testContacts.py` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/tests/testContacts.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/tests/testCustomMeeting.py` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/tests/testCustomMeeting.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/tests/testCustomMeetingConfig.py` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/tests/testCustomMeetingConfig.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/tests/testCustomMeetingItem.py` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/tests/testCustomMeetingItem.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/tests/testCustomToolPloneMeeting.py` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/tests/testCustomToolPloneMeeting.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/tests/testCustomUtils.py` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/tests/testCustomUtils.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/tests/testCustomWorkflows.py` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/tests/testCustomWorkflows.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/tests/testFaceted.py` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/tests/testFaceted.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/tests/testMeeting.py` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/tests/testMeeting.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/tests/testMeetingCategory.py` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/tests/testMeetingCategory.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/tests/testMeetingConfig.py` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/tests/testMeetingConfig.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/tests/testMeetingItem.py` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/tests/testMeetingItem.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,14 +26,16 @@
 from Products.MeetingCommunes.tests.testMeetingItem import testMeetingItem as mctmi
 
 
 class testMeetingItem(MeetingCPASLalouviereTestCase, mctmi):
     """
         Tests the MeetingItem class methods.
     """
+    def _extraNeutralFields(self):
+        return ["emergencyMotivation"]
     def _reviewers_may_edit_itemcreated(self):
         return True
 
     def _users_to_remove_for_mailling_list(self):
         return ["pmBudgetReviewer1", "pmBudgetReviewer2", "pmSecretaire", "pmN1", "pmN2", "pmPresident"]
 
 def test_suite():
```

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/tests/testPortlets.py` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/tests/testPortlets.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/tests/testSearches.py` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/tests/testSearches.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/tests/testSetup.py` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/tests/testSetup.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/tests/testToolPloneMeeting.py` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/tests/testToolPloneMeeting.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/tests/testUtils.py` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/tests/testUtils.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/tests/testValidators.py` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/tests/testValidators.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/tests/testViews.py` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/tests/testViews.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/tests/testVotes.py` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/tests/testVotes.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/tests/testWFAdaptations.py` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/tests/testWFAdaptations.py`

 * *Files 6% similar despite different names*

```diff
@@ -116,15 +116,14 @@
         self.changeUser('pmManager')
         self.do(item, 'goTo_returned_to_proposing_group_proposed_to_president')
 
     def _get_developers_reviewers_groups(self):
         return [self.developers_n1,
                 self.developers_n2,
                 self.developers_secretaire,
-                self.developers_president,
                 self.developers_reviewers]
 
     def test_pm_WFA_pre_validation(self):
         pass
 
     def test_pm_WFA_waiting_advices_with_prevalidation(self):
         pass
@@ -319,13 +318,29 @@
         self.addAdvice(item)
         self.do(item, self._wait_advice_from_proposed_state_back_transition())
         self.assertEqual(self.transitions(item), [])
         self.changeUser('pmReviewer1')
         self.assertEqual(self.transitions(item),
                          ['backToProposedToSecretaire', 'validate'])
 
+    def _no_validation_active(self):
+        '''Test when no item validation levels are enabled,
+           item is created in state "validated".'''
+        item = self.create('MeetingItem')
+        self.assertEqual(item.query_state(), 'validated')
+        # disabled item validation levels does not have access
+        # adding decision annex may be adapted
+        creators_roles = ['Reader']
+        if item.may_add_annex_decision(self.meetingConfig, item.query_state()):
+            creators_roles.append('Contributor')
+        self.assertEqual(item.__ac_local_roles__[self.developers_creators], creators_roles)
+        self.assertEqual(item.__ac_local_roles__[self.developers_n1], creators_roles)
+        self.assertEqual(item.__ac_local_roles__[self.developers_n2], creators_roles)
+        self.assertEqual(item.__ac_local_roles__[self.developers_secretaire], creators_roles)
+        self.assertEqual(item.__ac_local_roles__[self.developers_reviewers], creators_roles)
+        self.assertEqual(item.__ac_local_roles__[self.developers_observers], ['Reader'])
 
 def test_suite():
     from unittest import TestSuite, makeSuite
     suite = TestSuite()
     suite.addTest(makeSuite(testWFAdaptations, prefix='test_pm_'))
     return suite
```

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products/MeetingCPASLalouviere/tests/testWorkflows.py` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products/MeetingCPASLalouviere/tests/testWorkflows.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,15 @@
         self.failIf(self.hasPermission('PloneMeeting: Add annex', item1))
         # the secretariat validation level
         self.changeUser('pmSecretaire')
         self._check_users_can_modify(item1)
         self.do(item1, 'proposeToPresident')
         self.failIf(self.transitions(item1))  # He may trigger no more action
         self.failIf(self.hasPermission('PloneMeeting: Add annex', item1))
-        # the president validation level
+        # the reviewers validation level
         self.changeUser('pmPresident')
         self._check_users_can_modify(item1)
         self.do(item1, 'validate')
         self.failIf(self.transitions(item1))  # He may trigger no more action
         self.failIf(self.hasPermission('PloneMeeting: Add annex', item1))
         # pmManager creates a meeting
         self.changeUser('pmManager')
```

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products.MeetingCPASLalouviere.egg-info/PKG-INFO` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products.MeetingCPASLalouviere.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Products.MeetingCPASLalouviere
-Version: 4.2.0a3
+Version: 4.2.0a4
 Summary: PloneMeeting profile for CPAS of La Louviere.
 Home-page: http://www.imio.be/produits/gestion-des-deliberations
 Author: Olivier Delaere
 Author-email: olivier.delaere@imio.be
 License: GPL
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
@@ -18,14 +18,25 @@
 
 Check 'docs/README.txt'
 Products.MeetingCPASLalouviere Changelog
 ====================================
 
 The Products.MeetingCommunes version must be the same as the Products.PloneMeeting version
 
+4.2.0a4 (2023-05-16)
+--------------------
+
+- Fix custom searches filters.
+  [odelaere]
+- Use legacy reviewers suffix.
+  [odelaere]
+- Added emergencyMotivation field.
+  [odelaere]
+
+
 4.2.0a3 (2023-05-15)
 --------------------
 
 - Fix proposed_to_budgetimpact_reviewer transition_mappings.
   [odelaere]
 - Added missing icon and translation.
   [odelaere]
```

### Comparing `Products.MeetingCPASLalouviere-4.2.0a3/src/Products.MeetingCPASLalouviere.egg-info/SOURCES.txt` & `Products.MeetingCPASLalouviere-4.2.0a4/src/Products.MeetingCPASLalouviere.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -134,15 +134,16 @@
 src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/proposeToN1.png
 src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/proposeToN2.png
 src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/proposeToPresident.png
 src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/proposeToSecretaire.png
 src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/validate.png
 src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_styles/imioapps_properties.props
 src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_styles/meetingcpaslalouviere.css
-src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_templates/isAReviewer.py
+src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_templates/meetingitem_edit.pt
+src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_templates/meetingitem_view.pt
 src/Products/MeetingCPASLalouviere/tests/MeetingCPASLalouviereTestCase.py
 src/Products/MeetingCPASLalouviere/tests/__init__.py
 src/Products/MeetingCPASLalouviere/tests/helpers.py
 src/Products/MeetingCPASLalouviere/tests/testAdvices.py
 src/Products/MeetingCPASLalouviere/tests/testAnnexes.py
 src/Products/MeetingCPASLalouviere/tests/testChangeItemOrderView.py
 src/Products/MeetingCPASLalouviere/tests/testColumns.py
```

