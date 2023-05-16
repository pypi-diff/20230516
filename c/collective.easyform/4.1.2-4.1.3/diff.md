# Comparing `tmp/collective.easyform-4.1.2.tar.gz` & `tmp/collective.easyform-4.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "collective.easyform-4.1.2.tar", last modified: Mon Jan  2 16:45:44 2023, max compression
+gzip compressed data, was "collective.easyform-4.1.3.tar", last modified: Tue May 16 07:21:17 2023, max compression
```

## Comparing `collective.easyform-4.1.2.tar` & `collective.easyform-4.1.3.tar`

### file list

```diff
@@ -1,266 +1,271 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-01-02 16:45:44.668622 collective.easyform-4.1.2/
--rw-r--r--   0 maurits    (501) staff       (20)    16411 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)      781 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/CONTRIBUTORS.rst
--rw-r--r--   0 maurits    (501) staff       (20)      197 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)    26567 2023-01-02 16:45:44.668836 collective.easyform-4.1.2/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     9067 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/README.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-01-02 16:45:44.613240 collective.easyform-4.1.2/docs/
--rw-r--r--   0 maurits    (501) staff       (20)      433 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/docs/INSTALL.txt
--rw-r--r--   0 maurits    (501) staff       (20)    18032 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/docs/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)      736 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/docs/LICENSE.txt
--rw-r--r--   0 maurits    (501) staff       (20)     2755 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/docs/actions.rst
--rw-r--r--   0 maurits    (501) staff       (20)      677 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/docs/adding.rst
--rw-r--r--   0 maurits    (501) staff       (20)      851 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/docs/collective.easyform.browser.rst
--rw-r--r--   0 maurits    (501) staff       (20)     1784 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/docs/collective.easyform.rst
--rw-r--r--   0 maurits    (501) staff       (20)     8426 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/docs/conf.py
--rw-r--r--   0 maurits    (501) staff       (20)     1855 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/docs/fields.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-01-02 16:45:44.622659 collective.easyform-4.1.2/docs/images/
--rw-r--r--   0 maurits    (501) staff       (20)    41696 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/docs/images/add-new-action-overlay.png
--rw-r--r--   0 maurits    (501) staff       (20)    41507 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/docs/images/add-new-field-overlay.png
--rw-r--r--   0 maurits    (501) staff       (20)    20434 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/docs/images/add-new-fieldset-overlay.png
--rw-r--r--   0 maurits    (501) staff       (20)    20189 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/docs/images/add-new-menu.png
--rw-r--r--   0 maurits    (501) staff       (20)     5577 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/docs/images/added-new-action.png
--rw-r--r--   0 maurits    (501) staff       (20)     4427 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/docs/images/added-new-field.png
--rw-r--r--   0 maurits    (501) staff       (20)     2220 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/docs/images/added-new-fieldset.png
--rw-r--r--   0 maurits    (501) staff       (20)     8436 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/docs/images/click-actions-contentview.png
--rw-r--r--   0 maurits    (501) staff       (20)     6638 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/docs/images/click-add-new-action.png
--rw-r--r--   0 maurits    (501) staff       (20)     6571 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/docs/images/click-add-new-field.png
--rw-r--r--   0 maurits    (501) staff       (20)     7140 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/docs/images/click-add-new-fieldset.png
--rw-r--r--   0 maurits    (501) staff       (20)     8513 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/docs/images/click-fields-contentview.png
--rw-r--r--   0 maurits    (501) staff       (20)   212025 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/docs/images/conditional_fields_and_field_css.png
--rw-r--r--   0 maurits    (501) staff       (20)    13050 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/docs/images/created-easyform-actions.png
--rw-r--r--   0 maurits    (501) staff       (20)    22083 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/docs/images/created-easyform-fields.png
--rw-r--r--   0 maurits    (501) staff       (20)    14271 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/docs/images/created-easyform.png
--rw-r--r--   0 maurits    (501) staff       (20)    85234 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/docs/images/default-actions-mailer.png
--rw-r--r--   0 maurits    (501) staff       (20)   139577 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/docs/images/define-actions-menu-choice.png
--rw-r--r--   0 maurits    (501) staff       (20)    78436 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/docs/images/easyform-youtube.png
--rw-r--r--   0 maurits    (501) staff       (20)     9762 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/docs/images/edit-xml-actions-model-button.png
--rw-r--r--   0 maurits    (501) staff       (20)    38328 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/docs/images/edit-xml-actions-model-page.png
--rw-r--r--   0 maurits    (501) staff       (20)     9283 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/docs/images/edit-xml-fields-model-button.png
--rw-r--r--   0 maurits    (501) staff       (20)    50439 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/docs/images/edit-xml-fields-model-page.png
--rw-r--r--   0 maurits    (501) staff       (20)   143076 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/docs/images/form_multicolumns.png
--rw-r--r--   0 maurits    (501) staff       (20)   124476 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/docs/images/mailer-adapter-message-settings.png
--rw-r--r--   0 maurits    (501) staff       (20)    75303 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/docs/images/new-easyform-default-contributor.png
--rw-r--r--   0 maurits    (501) staff       (20)    82997 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/docs/images/new-easyform-default.png
--rw-r--r--   0 maurits    (501) staff       (20)   100335 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/docs/images/new-easyform-overrides.png
--rw-r--r--   0 maurits    (501) staff       (20)    62231 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/docs/images/new-easyform-thankspage-contributor.png
--rw-r--r--   0 maurits    (501) staff       (20)    59760 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/docs/images/new-easyform-thankspage.png
--rw-r--r--   0 maurits    (501) staff       (20)     2298 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/docs/index.rst
--rw-r--r--   0 maurits    (501) staff       (20)     6453 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/docs/rtd-requirements.txt
--rw-r--r--   0 maurits    (501) staff       (20)      405 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/docs/tests.rst
--rw-r--r--   0 maurits    (501) staff       (20)      278 2023-01-02 16:45:44.669327 collective.easyform-4.1.2/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     2623 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/setup.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-01-02 16:45:44.601279 collective.easyform-4.1.2/src/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-01-02 16:45:44.623074 collective.easyform-4.1.2/src/collective/
--rw-r--r--   0 maurits    (501) staff       (20)       80 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-01-02 16:45:44.630734 collective.easyform-4.1.2/src/collective/easyform/
--rw-r--r--   0 maurits    (501) staff       (20)      104 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/Form.gif
--rw-r--r--   0 maurits    (501) staff       (20)      135 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)    32069 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/actions.py
--rw-r--r--   0 maurits    (501) staff       (20)      748 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/actions.zcml
--rw-r--r--   0 maurits    (501) staff       (20)    10365 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/api.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-01-02 16:45:44.639177 collective.easyform-4.1.2/src/collective/easyform/browser/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/browser/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     3084 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/browser/action_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)    12722 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/browser/actions.py
--rw-r--r--   0 maurits    (501) staff       (20)     3053 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/browser/actions.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     4360 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/browser/actions_listing.pt
--rw-r--r--   0 maurits    (501) staff       (20)     3037 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/browser/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     1549 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/browser/controlpanel.py
--rw-r--r--   0 maurits    (501) staff       (20)      972 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/browser/easyform.css
--rw-r--r--   0 maurits    (501) staff       (20)      851 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/browser/easyform_form.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1032 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/browser/easyform_form_embedded.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1060 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/browser/easyform_layout.pt
--rw-r--r--   0 maurits    (501) staff       (20)      128 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/browser/empty.pt
--rw-r--r--   0 maurits    (501) staff       (20)     2331 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/browser/exportimport.py
--rw-r--r--   0 maurits    (501) staff       (20)     7766 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/browser/fields.py
--rw-r--r--   0 maurits    (501) staff       (20)     3398 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/browser/fields.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     5233 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/browser/fields_listing.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1243 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/browser/label.pt
--rw-r--r--   0 maurits    (501) staff       (20)     2212 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/browser/likert.py
--rw-r--r--   0 maurits    (501) staff       (20)      958 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/browser/likert.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      973 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/browser/likert_display.pt
--rw-r--r--   0 maurits    (501) staff       (20)      492 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/browser/likert_hidden.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1558 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/browser/likert_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)      777 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/browser/model_listing.pt
--rw-r--r--   0 maurits    (501) staff       (20)     2149 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/browser/modeleditor.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1251 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/browser/rich_label.pt
--rw-r--r--   0 maurits    (501) staff       (20)      956 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/browser/saveddata.pt
--rw-r--r--   0 maurits    (501) staff       (20)     2211 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/browser/saveddata_form.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1456 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/browser/thank_you.pt
--rw-r--r--   0 maurits    (501) staff       (20)    19678 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/browser/view.py
--rw-r--r--   0 maurits    (501) staff       (20)     2059 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/browser/widget.pt
--rw-r--r--   0 maurits    (501) staff       (20)     3233 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/browser/widgets.py
--rw-r--r--   0 maurits    (501) staff       (20)     4886 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/browser/widgets.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     2142 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/config.py
--rw-r--r--   0 maurits    (501) staff       (20)     2181 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      241 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/content.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-01-02 16:45:44.640155 collective.easyform-4.1.2/src/collective/easyform/default_schemata/
--rw-r--r--   0 maurits    (501) staff       (20)      494 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/default_schemata/actions_default.xml
--rw-r--r--   0 maurits    (501) staff       (20)      903 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/default_schemata/fields_default.xml
--rw-r--r--   0 maurits    (501) staff       (20)      528 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/default_schemata/mail_body_default.pt
--rw-r--r--   0 maurits    (501) staff       (20)       94 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/default_schemata/model_default.xml
--rw-r--r--   0 maurits    (501) staff       (20)     5668 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/exportimport.py
--rw-r--r--   0 maurits    (501) staff       (20)      980 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/exportimport.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     9505 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/fields.py
--rw-r--r--   0 maurits    (501) staff       (20)     2309 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/fields.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-01-02 16:45:44.642306 collective.easyform-4.1.2/src/collective/easyform/interfaces/
--rw-r--r--   0 maurits    (501) staff       (20)     1694 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/interfaces/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     3762 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/interfaces/actions.py
--rw-r--r--   0 maurits    (501) staff       (20)     1244 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/interfaces/customscript.py
--rw-r--r--   0 maurits    (501) staff       (20)    17139 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/interfaces/easyform.py
--rw-r--r--   0 maurits    (501) staff       (20)     8953 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/interfaces/fields.py
--rw-r--r--   0 maurits    (501) staff       (20)      177 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/interfaces/layer.py
--rw-r--r--   0 maurits    (501) staff       (20)    19973 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/interfaces/mailer.py
--rw-r--r--   0 maurits    (501) staff       (20)     2910 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/interfaces/savedata.py
--rw-r--r--   0 maurits    (501) staff       (20)      889 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/interfaces/validators.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-01-02 16:45:44.642770 collective.easyform-4.1.2/src/collective/easyform/locales/
--rw-r--r--   0 maurits    (501) staff       (20)    32629 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/locales/collective.easyform.pot
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-01-02 16:45:44.602651 collective.easyform-4.1.2/src/collective/easyform/locales/de/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-01-02 16:45:44.643298 collective.easyform-4.1.2/src/collective/easyform/locales/de/LC_MESSAGES/
--rw-r--r--   0 maurits    (501) staff       (20)    37093 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/locales/de/LC_MESSAGES/collective.easyform.po
--rw-r--r--   0 maurits    (501) staff       (20)      679 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/locales/de/LC_MESSAGES/plone.po
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-01-02 16:45:44.602990 collective.easyform-4.1.2/src/collective/easyform/locales/en/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-01-02 16:45:44.643776 collective.easyform-4.1.2/src/collective/easyform/locales/en/LC_MESSAGES/
--rw-r--r--   0 maurits    (501) staff       (20)    32468 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/locales/en/LC_MESSAGES/collective.easyform.po
--rw-r--r--   0 maurits    (501) staff       (20)      654 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/locales/en/LC_MESSAGES/plone.po
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-01-02 16:45:44.603216 collective.easyform-4.1.2/src/collective/easyform/locales/es/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-01-02 16:45:44.644335 collective.easyform-4.1.2/src/collective/easyform/locales/es/LC_MESSAGES/
--rw-r--r--   0 maurits    (501) staff       (20)    44240 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/locales/es/LC_MESSAGES/collective.easyform.po
--rw-r--r--   0 maurits    (501) staff       (20)      718 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/locales/es/LC_MESSAGES/plone.po
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-01-02 16:45:44.603603 collective.easyform-4.1.2/src/collective/easyform/locales/eu/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-01-02 16:45:44.644823 collective.easyform-4.1.2/src/collective/easyform/locales/eu/LC_MESSAGES/
--rw-r--r--   0 maurits    (501) staff       (20)    43331 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/locales/eu/LC_MESSAGES/collective.easyform.po
--rw-r--r--   0 maurits    (501) staff       (20)      656 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/locales/eu/LC_MESSAGES/plone.po
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-01-02 16:45:44.603887 collective.easyform-4.1.2/src/collective/easyform/locales/fr/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-01-02 16:45:44.645315 collective.easyform-4.1.2/src/collective/easyform/locales/fr/LC_MESSAGES/
--rw-r--r--   0 maurits    (501) staff       (20)    47080 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/locales/fr/LC_MESSAGES/collective.easyform.po
--rw-r--r--   0 maurits    (501) staff       (20)      667 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/locales/fr/LC_MESSAGES/plone.po
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-01-02 16:45:44.604230 collective.easyform-4.1.2/src/collective/easyform/locales/it/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-01-02 16:45:44.645833 collective.easyform-4.1.2/src/collective/easyform/locales/it/LC_MESSAGES/
--rw-r--r--   0 maurits    (501) staff       (20)    37804 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/locales/it/LC_MESSAGES/collective.easyform.po
--rw-r--r--   0 maurits    (501) staff       (20)      654 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/locales/it/LC_MESSAGES/plone.po
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-01-02 16:45:44.604504 collective.easyform-4.1.2/src/collective/easyform/locales/ja/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-01-02 16:45:44.646355 collective.easyform-4.1.2/src/collective/easyform/locales/ja/LC_MESSAGES/
--rw-r--r--   0 maurits    (501) staff       (20)    63446 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/locales/ja/LC_MESSAGES/collective.easyform.po
--rw-r--r--   0 maurits    (501) staff       (20)      647 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/locales/ja/LC_MESSAGES/plone.po
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-01-02 16:45:44.604769 collective.easyform-4.1.2/src/collective/easyform/locales/nl/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-01-02 16:45:44.646932 collective.easyform-4.1.2/src/collective/easyform/locales/nl/LC_MESSAGES/
--rw-r--r--   0 maurits    (501) staff       (20)    44857 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/locales/nl/LC_MESSAGES/collective.easyform.po
--rw-r--r--   0 maurits    (501) staff       (20)      689 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/locales/nl/LC_MESSAGES/plone.po
--rw-r--r--   0 maurits    (501) staff       (20)      653 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/locales/plone.pot
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-01-02 16:45:44.605073 collective.easyform-4.1.2/src/collective/easyform/locales/pt_BR/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-01-02 16:45:44.647436 collective.easyform-4.1.2/src/collective/easyform/locales/pt_BR/LC_MESSAGES/
--rw-r--r--   0 maurits    (501) staff       (20)    44331 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/locales/pt_BR/LC_MESSAGES/collective.easyform.po
--rw-r--r--   0 maurits    (501) staff       (20)      653 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/locales/pt_BR/LC_MESSAGES/plone.po
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-01-02 16:45:44.605292 collective.easyform-4.1.2/src/collective/easyform/locales/uk/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-01-02 16:45:44.648034 collective.easyform-4.1.2/src/collective/easyform/locales/uk/LC_MESSAGES/
--rw-r--r--   0 maurits    (501) staff       (20)    52193 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/locales/uk/LC_MESSAGES/collective.easyform.po
--rw-r--r--   0 maurits    (501) staff       (20)      682 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/locales/uk/LC_MESSAGES/plone.po
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-01-02 16:45:44.649421 collective.easyform-4.1.2/src/collective/easyform/migration/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/migration/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     5058 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/migration/actions.py
--rw-r--r--   0 maurits    (501) staff       (20)      393 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/migration/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     2278 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/migration/data.py
--rw-r--r--   0 maurits    (501) staff       (20)    10128 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/migration/fields.py
--rw-r--r--   0 maurits    (501) staff       (20)     4012 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/migration/pfg.py
--rw-r--r--   0 maurits    (501) staff       (20)     1429 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/permissions.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-01-02 16:45:44.606185 collective.easyform-4.1.2/src/collective/easyform/profiles/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-01-02 16:45:44.651216 collective.easyform-4.1.2/src/collective/easyform/profiles/default/
--rw-r--r--   0 maurits    (501) staff       (20)     4551 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/profiles/default/actions.xml
--rw-r--r--   0 maurits    (501) staff       (20)      127 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/profiles/default/browserlayer.xml
--rw-r--r--   0 maurits    (501) staff       (20)      427 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/profiles/default/controlpanel.xml
--rw-r--r--   0 maurits    (501) staff       (20)       71 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/profiles/default/metadata.xml
--rw-r--r--   0 maurits    (501) staff       (20)     3345 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/profiles/default/registry.xml
--rw-r--r--   0 maurits    (501) staff       (20)     2186 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/profiles/default/rolemap.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-01-02 16:45:44.651425 collective.easyform-4.1.2/src/collective/easyform/profiles/default/types/
--rw-r--r--   0 maurits    (501) staff       (20)     2408 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/profiles/default/types/EasyForm.xml
--rw-r--r--   0 maurits    (501) staff       (20)      166 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/profiles/default/types.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-01-02 16:45:44.652887 collective.easyform-4.1.2/src/collective/easyform/profiles/uninstall/
--rw-r--r--   0 maurits    (501) staff       (20)      732 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/profiles/uninstall/actions.xml
--rw-r--r--   0 maurits    (501) staff       (20)      122 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/profiles/uninstall/browserlayer.xml
--rw-r--r--   0 maurits    (501) staff       (20)      272 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/profiles/uninstall/controlpanel.xml
--rw-r--r--   0 maurits    (501) staff       (20)      190 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/profiles/uninstall/registry.xml
--rw-r--r--   0 maurits    (501) staff       (20)      190 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/profiles/uninstall/types.xml
--rw-r--r--   0 maurits    (501) staff       (20)     5236 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/serializer.py
--rw-r--r--   0 maurits    (501) staff       (20)      348 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/setuphandlers.py
--rw-r--r--   0 maurits    (501) staff       (20)      269 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/subscribers.py
--rw-r--r--   0 maurits    (501) staff       (20)      453 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/subscribers.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-01-02 16:45:44.658630 collective.easyform-4.1.2/src/collective/easyform/tests/
--rw-r--r--   0 maurits    (501) staff       (20)     4339 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/tests/PloneLogo.png
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     4813 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/tests/action_errors.rst
--rw-r--r--   0 maurits    (501) staff       (20)    10119 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/tests/attachment.rst
--rw-r--r--   0 maurits    (501) staff       (20)     4498 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/tests/base.py
--rw-r--r--   0 maurits    (501) staff       (20)     2924 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/tests/basic.rst
--rw-r--r--   0 maurits    (501) staff       (20)     7732 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/tests/browser.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-01-02 16:45:44.661607 collective.easyform-4.1.2/src/collective/easyform/tests/fixtures/
--rw-r--r--   0 maurits    (501) staff       (20)     1077 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/tests/fixtures/fieldset_file.xml
--rw-r--r--   0 maurits    (501) staff       (20)     1492 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/tests/fixtures/fieldset_form.xml
--rw-r--r--   0 maurits    (501) staff       (20)     1288 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/tests/fixtures/fieldset_multiple_choice.xml
--rw-r--r--   0 maurits    (501) staff       (20)      921 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/tests/fixtures/fieldset_recaptcha.xml
--rw-r--r--   0 maurits    (501) staff       (20)     1019 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/tests/fixtures/fieldset_with_single_field.xml
--rw-r--r--   0 maurits    (501) staff       (20)      826 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/tests/fixtures/hcaptcha.xml
--rw-r--r--   0 maurits    (501) staff       (20)      799 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/tests/fixtures/hidden_form.xml
--rw-r--r--   0 maurits    (501) staff       (20)      879 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/tests/fixtures/radio_form.xml
--rw-r--r--   0 maurits    (501) staff       (20)      827 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/tests/fixtures/recaptcha.xml
--rw-r--r--   0 maurits    (501) staff       (20)      921 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/tests/fixtures/single_field.xml
--rw-r--r--   0 maurits    (501) staff       (20)      263 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/tests/fixtures/tests.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      883 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/tests/fixtures/wrapper_template.pt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-01-02 16:45:44.663569 collective.easyform-4.1.2/src/collective/easyform/tests/robot/
--rw-r--r--   0 maurits    (501) staff       (20)     2005 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/tests/robot/keywords.robot
--rw-r--r--   0 maurits    (501) staff       (20)     3099 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/tests/robot/test_addform.robot
--rw-r--r--   0 maurits    (501) staff       (20)     1517 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/tests/robot/test_editxmlmodel.robot
--rw-r--r--   0 maurits    (501) staff       (20)      619 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/tests/robot/test_headerinjection.robot
--rw-r--r--   0 maurits    (501) staff       (20)     2201 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/tests/robot/todo_test_addaction.robot
--rw-r--r--   0 maurits    (501) staff       (20)     2564 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/tests/robot/todo_test_addfield.robot
--rw-r--r--   0 maurits    (501) staff       (20)     1447 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/tests/robot/todo_test_addfieldset.robot
--rw-r--r--   0 maurits    (501) staff       (20)      542 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/tests/robot/todo_test_submit.robot
--rw-r--r--   0 maurits    (501) staff       (20)     3431 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/tests/serverside_field.rst
--rw-r--r--   0 maurits    (501) staff       (20)     1966 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/tests/ssl.rst
--rw-r--r--   0 maurits    (501) staff       (20)     8436 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/tests/testApi.py
--rw-r--r--   0 maurits    (501) staff       (20)     4656 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/tests/testControlpanel.py
--rw-r--r--   0 maurits    (501) staff       (20)    10802 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/tests/testCustomScript.py
--rw-r--r--   0 maurits    (501) staff       (20)     2061 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/tests/testDocTests.py
--rw-r--r--   0 maurits    (501) staff       (20)     5394 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/tests/testEmbedding.py
--rw-r--r--   0 maurits    (501) staff       (20)     1113 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/tests/testEvents.py
--rw-r--r--   0 maurits    (501) staff       (20)     5957 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/tests/testLikert.py
--rw-r--r--   0 maurits    (501) staff       (20)    29357 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/tests/testMailer.py
--rw-r--r--   0 maurits    (501) staff       (20)     3830 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/tests/testMisc.py
--rw-r--r--   0 maurits    (501) staff       (20)     8312 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/tests/testSavedDataSerializer.py
--rw-r--r--   0 maurits    (501) staff       (20)    27302 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/tests/testSaver.py
--rw-r--r--   0 maurits    (501) staff       (20)     4039 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/tests/testSetup.py
--rw-r--r--   0 maurits    (501) staff       (20)     6799 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/tests/testThanksPage.py
--rw-r--r--   0 maurits    (501) staff       (20)    18564 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/tests/testValidators.py
--rw-r--r--   0 maurits    (501) staff       (20)      780 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/tests/test_robot.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-01-02 16:45:44.668271 collective.easyform-4.1.2/src/collective/easyform/upgrades/
--rw-r--r--   0 maurits    (501) staff       (20)      508 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/upgrades/1001.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      582 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/upgrades/1002.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      449 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/upgrades/1003.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      466 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/upgrades/1004.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      495 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/upgrades/1005.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      442 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/upgrades/1006.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      518 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/upgrades/1007.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      397 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/upgrades/1008.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      397 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/upgrades/1009.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      400 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/upgrades/1010.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      398 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/upgrades/1011.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      410 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/upgrades/1012.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      414 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/upgrades/1013.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      400 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/upgrades/1014.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      395 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/upgrades/1015.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     3231 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/upgrades/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      531 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/upgrades/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     2532 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/validators.py
--rw-r--r--   0 maurits    (501) staff       (20)      749 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/validators.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     4317 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/vocabularies.py
--rw-r--r--   0 maurits    (501) staff       (20)     1347 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective/easyform/vocabularies.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-01-02 16:45:44.625317 collective.easyform-4.1.2/src/collective.easyform.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    26567 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective.easyform.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)    10191 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective.easyform.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective.easyform.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)       40 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective.easyform.egg-info/entry_points.txt
--rw-r--r--   0 maurits    (501) staff       (20)       11 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective.easyform.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective.easyform.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      622 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective.easyform.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)       11 2023-01-02 16:45:44.000000 collective.easyform-4.1.2/src/collective.easyform.egg-info/top_level.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-16 07:21:17.609701 collective.easyform-4.1.3/
+-rw-r--r--   0 maurits    (501) staff       (20)    16725 2023-05-16 07:21:16.000000 collective.easyform-4.1.3/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      781 2023-05-16 07:21:16.000000 collective.easyform-4.1.3/CONTRIBUTORS.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      197 2023-05-16 07:21:16.000000 collective.easyform-4.1.3/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    26881 2023-05-16 07:21:17.609854 collective.easyform-4.1.3/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     9067 2023-05-16 07:21:16.000000 collective.easyform-4.1.3/README.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-16 07:21:17.542689 collective.easyform-4.1.3/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)      433 2023-05-16 07:21:16.000000 collective.easyform-4.1.3/docs/INSTALL.txt
+-rw-r--r--   0 maurits    (501) staff       (20)    18032 2023-05-16 07:21:16.000000 collective.easyform-4.1.3/docs/LICENSE.GPL
+-rw-r--r--   0 maurits    (501) staff       (20)      736 2023-05-16 07:21:16.000000 collective.easyform-4.1.3/docs/LICENSE.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     2755 2023-05-16 07:21:16.000000 collective.easyform-4.1.3/docs/actions.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      677 2023-05-16 07:21:16.000000 collective.easyform-4.1.3/docs/adding.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      851 2023-05-16 07:21:16.000000 collective.easyform-4.1.3/docs/collective.easyform.browser.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     1784 2023-05-16 07:21:16.000000 collective.easyform-4.1.3/docs/collective.easyform.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     8426 2023-05-16 07:21:16.000000 collective.easyform-4.1.3/docs/conf.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1855 2023-05-16 07:21:16.000000 collective.easyform-4.1.3/docs/fields.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-16 07:21:17.554359 collective.easyform-4.1.3/docs/images/
+-rw-r--r--   0 maurits    (501) staff       (20)    41696 2023-05-16 07:21:16.000000 collective.easyform-4.1.3/docs/images/add-new-action-overlay.png
+-rw-r--r--   0 maurits    (501) staff       (20)    41507 2023-05-16 07:21:16.000000 collective.easyform-4.1.3/docs/images/add-new-field-overlay.png
+-rw-r--r--   0 maurits    (501) staff       (20)    20434 2023-05-16 07:21:16.000000 collective.easyform-4.1.3/docs/images/add-new-fieldset-overlay.png
+-rw-r--r--   0 maurits    (501) staff       (20)    20189 2023-05-16 07:21:16.000000 collective.easyform-4.1.3/docs/images/add-new-menu.png
+-rw-r--r--   0 maurits    (501) staff       (20)     5577 2023-05-16 07:21:16.000000 collective.easyform-4.1.3/docs/images/added-new-action.png
+-rw-r--r--   0 maurits    (501) staff       (20)     4427 2023-05-16 07:21:16.000000 collective.easyform-4.1.3/docs/images/added-new-field.png
+-rw-r--r--   0 maurits    (501) staff       (20)     2220 2023-05-16 07:21:16.000000 collective.easyform-4.1.3/docs/images/added-new-fieldset.png
+-rw-r--r--   0 maurits    (501) staff       (20)     8436 2023-05-16 07:21:16.000000 collective.easyform-4.1.3/docs/images/click-actions-contentview.png
+-rw-r--r--   0 maurits    (501) staff       (20)     6638 2023-05-16 07:21:16.000000 collective.easyform-4.1.3/docs/images/click-add-new-action.png
+-rw-r--r--   0 maurits    (501) staff       (20)     6571 2023-05-16 07:21:16.000000 collective.easyform-4.1.3/docs/images/click-add-new-field.png
+-rw-r--r--   0 maurits    (501) staff       (20)     7140 2023-05-16 07:21:16.000000 collective.easyform-4.1.3/docs/images/click-add-new-fieldset.png
+-rw-r--r--   0 maurits    (501) staff       (20)     8513 2023-05-16 07:21:16.000000 collective.easyform-4.1.3/docs/images/click-fields-contentview.png
+-rw-r--r--   0 maurits    (501) staff       (20)   212025 2023-05-16 07:21:16.000000 collective.easyform-4.1.3/docs/images/conditional_fields_and_field_css.png
+-rw-r--r--   0 maurits    (501) staff       (20)    13050 2023-05-16 07:21:16.000000 collective.easyform-4.1.3/docs/images/created-easyform-actions.png
+-rw-r--r--   0 maurits    (501) staff       (20)    22083 2023-05-16 07:21:16.000000 collective.easyform-4.1.3/docs/images/created-easyform-fields.png
+-rw-r--r--   0 maurits    (501) staff       (20)    14271 2023-05-16 07:21:16.000000 collective.easyform-4.1.3/docs/images/created-easyform.png
+-rw-r--r--   0 maurits    (501) staff       (20)    85234 2023-05-16 07:21:16.000000 collective.easyform-4.1.3/docs/images/default-actions-mailer.png
+-rw-r--r--   0 maurits    (501) staff       (20)   139577 2023-05-16 07:21:16.000000 collective.easyform-4.1.3/docs/images/define-actions-menu-choice.png
+-rw-r--r--   0 maurits    (501) staff       (20)    78436 2023-05-16 07:21:16.000000 collective.easyform-4.1.3/docs/images/easyform-youtube.png
+-rw-r--r--   0 maurits    (501) staff       (20)     9762 2023-05-16 07:21:16.000000 collective.easyform-4.1.3/docs/images/edit-xml-actions-model-button.png
+-rw-r--r--   0 maurits    (501) staff       (20)    38328 2023-05-16 07:21:16.000000 collective.easyform-4.1.3/docs/images/edit-xml-actions-model-page.png
+-rw-r--r--   0 maurits    (501) staff       (20)     9283 2023-05-16 07:21:16.000000 collective.easyform-4.1.3/docs/images/edit-xml-fields-model-button.png
+-rw-r--r--   0 maurits    (501) staff       (20)    50439 2023-05-16 07:21:16.000000 collective.easyform-4.1.3/docs/images/edit-xml-fields-model-page.png
+-rw-r--r--   0 maurits    (501) staff       (20)   143076 2023-05-16 07:21:16.000000 collective.easyform-4.1.3/docs/images/form_multicolumns.png
+-rw-r--r--   0 maurits    (501) staff       (20)   124476 2023-05-16 07:21:16.000000 collective.easyform-4.1.3/docs/images/mailer-adapter-message-settings.png
+-rw-r--r--   0 maurits    (501) staff       (20)    75303 2023-05-16 07:21:16.000000 collective.easyform-4.1.3/docs/images/new-easyform-default-contributor.png
+-rw-r--r--   0 maurits    (501) staff       (20)    82997 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/docs/images/new-easyform-default.png
+-rw-r--r--   0 maurits    (501) staff       (20)   100335 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/docs/images/new-easyform-overrides.png
+-rw-r--r--   0 maurits    (501) staff       (20)    62231 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/docs/images/new-easyform-thankspage-contributor.png
+-rw-r--r--   0 maurits    (501) staff       (20)    59760 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/docs/images/new-easyform-thankspage.png
+-rw-r--r--   0 maurits    (501) staff       (20)     2298 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/docs/index.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     6453 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/docs/rtd-requirements.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      405 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/docs/tests.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      278 2023-05-16 07:21:17.610330 collective.easyform-4.1.3/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     2648 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-16 07:21:17.528786 collective.easyform-4.1.3/src/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-16 07:21:17.554748 collective.easyform-4.1.3/src/collective/
+-rw-r--r--   0 maurits    (501) staff       (20)       80 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-16 07:21:17.563642 collective.easyform-4.1.3/src/collective/easyform/
+-rw-r--r--   0 maurits    (501) staff       (20)      104 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/Form.gif
+-rw-r--r--   0 maurits    (501) staff       (20)      135 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)    32069 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/actions.py
+-rw-r--r--   0 maurits    (501) staff       (20)      748 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/actions.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)    10365 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/api.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-16 07:21:17.573463 collective.easyform-4.1.3/src/collective/easyform/browser/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/browser/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3084 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/browser/action_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)    12722 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/browser/actions.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3053 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/browser/actions.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     4360 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/browser/actions_listing.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     3037 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/browser/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     1549 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/browser/controlpanel.py
+-rw-r--r--   0 maurits    (501) staff       (20)      972 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/browser/easyform.css
+-rw-r--r--   0 maurits    (501) staff       (20)      851 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/browser/easyform_form.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1032 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/browser/easyform_form_embedded.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1060 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/browser/easyform_layout.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      128 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/browser/empty.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     2331 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/browser/exportimport.py
+-rw-r--r--   0 maurits    (501) staff       (20)     7766 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/browser/fields.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3398 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/browser/fields.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     5233 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/browser/fields_listing.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1243 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/browser/label.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     2212 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/browser/likert.py
+-rw-r--r--   0 maurits    (501) staff       (20)      958 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/browser/likert.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      973 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/browser/likert_display.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      492 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/browser/likert_hidden.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1558 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/browser/likert_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      777 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/browser/model_listing.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     2149 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/browser/modeleditor.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1251 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/browser/rich_label.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      956 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/browser/saveddata.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     2211 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/browser/saveddata_form.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1456 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/browser/thank_you.pt
+-rw-r--r--   0 maurits    (501) staff       (20)    19775 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/browser/view.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2059 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/browser/widget.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     3233 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/browser/widgets.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4886 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/browser/widgets.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     2142 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/config.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2181 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      241 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/content.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-16 07:21:17.574707 collective.easyform-4.1.3/src/collective/easyform/default_schemata/
+-rw-r--r--   0 maurits    (501) staff       (20)      494 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/default_schemata/actions_default.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      903 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/default_schemata/fields_default.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      528 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/default_schemata/mail_body_default.pt
+-rw-r--r--   0 maurits    (501) staff       (20)       94 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/default_schemata/model_default.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     5668 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/exportimport.py
+-rw-r--r--   0 maurits    (501) staff       (20)      980 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/exportimport.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     9505 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/fields.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2309 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/fields.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-16 07:21:17.577499 collective.easyform-4.1.3/src/collective/easyform/interfaces/
+-rw-r--r--   0 maurits    (501) staff       (20)     1694 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/interfaces/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3762 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/interfaces/actions.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1244 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/interfaces/customscript.py
+-rw-r--r--   0 maurits    (501) staff       (20)    17139 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/interfaces/easyform.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8953 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/interfaces/fields.py
+-rw-r--r--   0 maurits    (501) staff       (20)      177 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/interfaces/layer.py
+-rw-r--r--   0 maurits    (501) staff       (20)    19973 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/interfaces/mailer.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2910 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/interfaces/savedata.py
+-rw-r--r--   0 maurits    (501) staff       (20)      889 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/interfaces/validators.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-16 07:21:17.578169 collective.easyform-4.1.3/src/collective/easyform/locales/
+-rw-r--r--   0 maurits    (501) staff       (20)    32629 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/locales/collective.easyform.pot
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-16 07:21:17.530400 collective.easyform-4.1.3/src/collective/easyform/locales/de/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-16 07:21:17.578837 collective.easyform-4.1.3/src/collective/easyform/locales/de/LC_MESSAGES/
+-rw-r--r--   0 maurits    (501) staff       (20)    37093 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/locales/de/LC_MESSAGES/collective.easyform.po
+-rw-r--r--   0 maurits    (501) staff       (20)      679 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/locales/de/LC_MESSAGES/plone.po
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-16 07:21:17.530801 collective.easyform-4.1.3/src/collective/easyform/locales/en/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-16 07:21:17.579498 collective.easyform-4.1.3/src/collective/easyform/locales/en/LC_MESSAGES/
+-rw-r--r--   0 maurits    (501) staff       (20)    32468 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/locales/en/LC_MESSAGES/collective.easyform.po
+-rw-r--r--   0 maurits    (501) staff       (20)      654 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/locales/en/LC_MESSAGES/plone.po
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-16 07:21:17.531195 collective.easyform-4.1.3/src/collective/easyform/locales/es/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-16 07:21:17.580165 collective.easyform-4.1.3/src/collective/easyform/locales/es/LC_MESSAGES/
+-rw-r--r--   0 maurits    (501) staff       (20)    46845 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/locales/es/LC_MESSAGES/collective.easyform.po
+-rw-r--r--   0 maurits    (501) staff       (20)      718 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/locales/es/LC_MESSAGES/plone.po
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-16 07:21:17.531603 collective.easyform-4.1.3/src/collective/easyform/locales/eu/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-16 07:21:17.580816 collective.easyform-4.1.3/src/collective/easyform/locales/eu/LC_MESSAGES/
+-rw-r--r--   0 maurits    (501) staff       (20)    43331 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/locales/eu/LC_MESSAGES/collective.easyform.po
+-rw-r--r--   0 maurits    (501) staff       (20)      656 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/locales/eu/LC_MESSAGES/plone.po
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-16 07:21:17.532009 collective.easyform-4.1.3/src/collective/easyform/locales/fr/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-16 07:21:17.581452 collective.easyform-4.1.3/src/collective/easyform/locales/fr/LC_MESSAGES/
+-rw-r--r--   0 maurits    (501) staff       (20)    47080 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/locales/fr/LC_MESSAGES/collective.easyform.po
+-rw-r--r--   0 maurits    (501) staff       (20)      667 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/locales/fr/LC_MESSAGES/plone.po
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-16 07:21:17.532455 collective.easyform-4.1.3/src/collective/easyform/locales/it/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-16 07:21:17.582084 collective.easyform-4.1.3/src/collective/easyform/locales/it/LC_MESSAGES/
+-rw-r--r--   0 maurits    (501) staff       (20)    37804 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/locales/it/LC_MESSAGES/collective.easyform.po
+-rw-r--r--   0 maurits    (501) staff       (20)      654 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/locales/it/LC_MESSAGES/plone.po
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-16 07:21:17.532872 collective.easyform-4.1.3/src/collective/easyform/locales/ja/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-16 07:21:17.582707 collective.easyform-4.1.3/src/collective/easyform/locales/ja/LC_MESSAGES/
+-rw-r--r--   0 maurits    (501) staff       (20)    63446 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/locales/ja/LC_MESSAGES/collective.easyform.po
+-rw-r--r--   0 maurits    (501) staff       (20)      647 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/locales/ja/LC_MESSAGES/plone.po
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-16 07:21:17.533278 collective.easyform-4.1.3/src/collective/easyform/locales/nl/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-16 07:21:17.583325 collective.easyform-4.1.3/src/collective/easyform/locales/nl/LC_MESSAGES/
+-rw-r--r--   0 maurits    (501) staff       (20)    44857 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/locales/nl/LC_MESSAGES/collective.easyform.po
+-rw-r--r--   0 maurits    (501) staff       (20)      689 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/locales/nl/LC_MESSAGES/plone.po
+-rw-r--r--   0 maurits    (501) staff       (20)      653 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/locales/plone.pot
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-16 07:21:17.533681 collective.easyform-4.1.3/src/collective/easyform/locales/pt_BR/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-16 07:21:17.583963 collective.easyform-4.1.3/src/collective/easyform/locales/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 maurits    (501) staff       (20)    44331 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/locales/pt_BR/LC_MESSAGES/collective.easyform.po
+-rw-r--r--   0 maurits    (501) staff       (20)      653 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/locales/pt_BR/LC_MESSAGES/plone.po
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-16 07:21:17.534081 collective.easyform-4.1.3/src/collective/easyform/locales/uk/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-16 07:21:17.584575 collective.easyform-4.1.3/src/collective/easyform/locales/uk/LC_MESSAGES/
+-rw-r--r--   0 maurits    (501) staff       (20)    52193 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/locales/uk/LC_MESSAGES/collective.easyform.po
+-rw-r--r--   0 maurits    (501) staff       (20)      682 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/locales/uk/LC_MESSAGES/plone.po
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-16 07:21:17.586083 collective.easyform-4.1.3/src/collective/easyform/migration/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/migration/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5058 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/migration/actions.py
+-rw-r--r--   0 maurits    (501) staff       (20)      393 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/migration/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     2278 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/migration/data.py
+-rw-r--r--   0 maurits    (501) staff       (20)    10128 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/migration/fields.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4012 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/migration/pfg.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1429 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/permissions.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-16 07:21:17.535118 collective.easyform-4.1.3/src/collective/easyform/profiles/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-16 07:21:17.587972 collective.easyform-4.1.3/src/collective/easyform/profiles/default/
+-rw-r--r--   0 maurits    (501) staff       (20)     4710 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/profiles/default/actions.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      127 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/profiles/default/browserlayer.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      427 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/profiles/default/controlpanel.xml
+-rw-r--r--   0 maurits    (501) staff       (20)       71 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/profiles/default/metadata.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     3345 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/profiles/default/registry.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     2186 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/profiles/default/rolemap.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-16 07:21:17.588254 collective.easyform-4.1.3/src/collective/easyform/profiles/default/types/
+-rw-r--r--   0 maurits    (501) staff       (20)     2408 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/profiles/default/types/EasyForm.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      166 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/profiles/default/types.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-16 07:21:17.589787 collective.easyform-4.1.3/src/collective/easyform/profiles/uninstall/
+-rw-r--r--   0 maurits    (501) staff       (20)      732 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/profiles/uninstall/actions.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      122 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/profiles/uninstall/browserlayer.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      272 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/profiles/uninstall/controlpanel.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      190 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/profiles/uninstall/registry.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      190 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/profiles/uninstall/types.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     5236 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/serializer.py
+-rw-r--r--   0 maurits    (501) staff       (20)      805 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/setuphandlers.py
+-rw-r--r--   0 maurits    (501) staff       (20)      269 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/subscribers.py
+-rw-r--r--   0 maurits    (501) staff       (20)      453 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/subscribers.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-16 07:21:17.596881 collective.easyform-4.1.3/src/collective/easyform/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)     4339 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/tests/PloneLogo.png
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4813 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/tests/action_errors.rst
+-rw-r--r--   0 maurits    (501) staff       (20)    10119 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/tests/attachment.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     4498 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/tests/base.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2924 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/tests/basic.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     7732 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/tests/browser.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-16 07:21:17.601199 collective.easyform-4.1.3/src/collective/easyform/tests/fixtures/
+-rw-r--r--   0 maurits    (501) staff       (20)     1077 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/tests/fixtures/fieldset_file.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     1492 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/tests/fixtures/fieldset_form.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     1288 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/tests/fixtures/fieldset_multiple_choice.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      921 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/tests/fixtures/fieldset_recaptcha.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     1019 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/tests/fixtures/fieldset_with_single_field.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      826 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/tests/fixtures/hcaptcha.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      799 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/tests/fixtures/hidden_form.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      879 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/tests/fixtures/radio_form.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      827 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/tests/fixtures/recaptcha.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      921 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/tests/fixtures/single_field.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      263 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/tests/fixtures/tests.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      883 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/tests/fixtures/wrapper_template.pt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-16 07:21:17.603948 collective.easyform-4.1.3/src/collective/easyform/tests/robot/
+-rw-r--r--   0 maurits    (501) staff       (20)     2005 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/tests/robot/keywords.robot
+-rw-r--r--   0 maurits    (501) staff       (20)     3099 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/tests/robot/test_addform.robot
+-rw-r--r--   0 maurits    (501) staff       (20)     1517 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/tests/robot/test_editxmlmodel.robot
+-rw-r--r--   0 maurits    (501) staff       (20)      619 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/tests/robot/test_headerinjection.robot
+-rw-r--r--   0 maurits    (501) staff       (20)     2201 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/tests/robot/todo_test_addaction.robot
+-rw-r--r--   0 maurits    (501) staff       (20)     2564 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/tests/robot/todo_test_addfield.robot
+-rw-r--r--   0 maurits    (501) staff       (20)     1447 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/tests/robot/todo_test_addfieldset.robot
+-rw-r--r--   0 maurits    (501) staff       (20)      542 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/tests/robot/todo_test_submit.robot
+-rw-r--r--   0 maurits    (501) staff       (20)     3431 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/tests/serverside_field.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     1966 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/tests/ssl.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     8436 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/tests/testApi.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4656 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/tests/testControlpanel.py
+-rw-r--r--   0 maurits    (501) staff       (20)    10802 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/tests/testCustomScript.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2061 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/tests/testDocTests.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5394 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/tests/testEmbedding.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1113 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/tests/testEvents.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5957 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/tests/testLikert.py
+-rw-r--r--   0 maurits    (501) staff       (20)    29357 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/tests/testMailer.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3830 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/tests/testMisc.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8312 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/tests/testSavedDataSerializer.py
+-rw-r--r--   0 maurits    (501) staff       (20)    27302 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/tests/testSaver.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4039 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/tests/testSetup.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6799 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/tests/testThanksPage.py
+-rw-r--r--   0 maurits    (501) staff       (20)    18564 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/tests/testValidators.py
+-rw-r--r--   0 maurits    (501) staff       (20)      780 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/tests/test_robot.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-16 07:21:17.608931 collective.easyform-4.1.3/src/collective/easyform/upgrades/
+-rw-r--r--   0 maurits    (501) staff       (20)      508 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/upgrades/1001.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      582 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/upgrades/1002.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      449 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/upgrades/1003.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      466 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/upgrades/1004.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      495 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/upgrades/1005.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      442 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/upgrades/1006.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      518 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/upgrades/1007.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      397 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/upgrades/1008.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      397 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/upgrades/1009.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      400 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/upgrades/1010.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      398 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/upgrades/1011.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      410 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/upgrades/1012.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      414 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/upgrades/1013.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      400 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/upgrades/1014.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      395 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/upgrades/1015.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      654 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/upgrades/1016.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     3231 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/upgrades/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      562 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/upgrades/configure.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-16 07:21:17.536378 collective.easyform-4.1.3/src/collective/easyform/upgrades/profiles/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-16 07:21:17.609458 collective.easyform-4.1.3/src/collective/easyform/upgrades/profiles/1016/
+-rw-r--r--   0 maurits    (501) staff       (20)     1480 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/upgrades/profiles/1016/actions.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      274 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/upgrades/profiles/1016/registry.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     2532 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/validators.py
+-rw-r--r--   0 maurits    (501) staff       (20)      749 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/validators.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     4317 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/vocabularies.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1347 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/vocabularies.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-16 07:21:17.557205 collective.easyform-4.1.3/src/collective.easyform.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    26881 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective.easyform.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)    10353 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective.easyform.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective.easyform.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       40 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective.easyform.egg-info/entry_points.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       11 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective.easyform.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective.easyform.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      636 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective.easyform.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       11 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective.easyform.egg-info/top_level.txt
```

### Comparing `collective.easyform-4.1.2/CHANGES.rst` & `collective.easyform-4.1.3/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,27 @@
 Changelog
 =========
 
 
+4.1.3 (2023-05-16)
+------------------
+
+
+Bug fixes:
+
+- Add upgrade step and profile to update contenttype icon in registry.
+  [maurits]
+
+- Add icon expressions for actions.
+  [maurits]
+
+- Update Spanish translations.
+  [macagua]
+
+
 4.1.2 (2023-01-02)
 ------------------
 
 - Define 'Edit' and 'View' icons for the form. (#390)
   [frapell]
 
 - Require at least Python 3.8.  Test with 3.8-3.11.  [maurits]
@@ -22,14 +38,17 @@
 
 - Prevent RichLabel fields from breaking the form
   [MrTango]
 
 - Schemaeditor UI: close modals and reload fields(sets) when saving.
   [petschki]
 
+- Fix bug which did not render correctly GroupForm widgets (see #370)
+  [petschki]
+
 
 4.1.0 (2022-08-10)
 ------------------
 
 New features:
 
 - Add support for field level CSS classes.
```

### Comparing `collective.easyform-4.1.2/CONTRIBUTORS.rst` & `collective.easyform-4.1.3/CONTRIBUTORS.rst`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/PKG-INFO` & `collective.easyform-4.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.easyform
-Version: 4.1.2
+Version: 4.1.3
 Summary: Forms for Plone
 Home-page: https://github.com/collective/collective.easyform
 Author: Roman Kozlovskyi
 Author-email: krzroman@gmail.com
 Maintainer: Plone Release Team
 Maintainer-email: releaseteam@plone.org
 License: GPLv2
@@ -342,14 +342,30 @@
 - 3.x targets Plone 5.2
 - 4.x targets Plone 6, on Python 3
 
 Changelog
 =========
 
 
+4.1.3 (2023-05-16)
+------------------
+
+
+Bug fixes:
+
+- Add upgrade step and profile to update contenttype icon in registry.
+  [maurits]
+
+- Add icon expressions for actions.
+  [maurits]
+
+- Update Spanish translations.
+  [macagua]
+
+
 4.1.2 (2023-01-02)
 ------------------
 
 - Define 'Edit' and 'View' icons for the form. (#390)
   [frapell]
 
 - Require at least Python 3.8.  Test with 3.8-3.11.  [maurits]
@@ -366,14 +382,17 @@
 
 - Prevent RichLabel fields from breaking the form
   [MrTango]
 
 - Schemaeditor UI: close modals and reload fields(sets) when saving.
   [petschki]
 
+- Fix bug which did not render correctly GroupForm widgets (see #370)
+  [petschki]
+
 
 4.1.0 (2022-08-10)
 ------------------
 
 New features:
 
 - Add support for field level CSS classes.
```

### Comparing `collective.easyform-4.1.2/README.rst` & `collective.easyform-4.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/docs/LICENSE.GPL` & `collective.easyform-4.1.3/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/docs/LICENSE.txt` & `collective.easyform-4.1.3/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/docs/actions.rst` & `collective.easyform-4.1.3/docs/actions.rst`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/docs/adding.rst` & `collective.easyform-4.1.3/docs/adding.rst`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/docs/collective.easyform.browser.rst` & `collective.easyform-4.1.3/docs/collective.easyform.browser.rst`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/docs/collective.easyform.rst` & `collective.easyform-4.1.3/docs/collective.easyform.rst`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/docs/conf.py` & `collective.easyform-4.1.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/docs/fields.rst` & `collective.easyform-4.1.3/docs/fields.rst`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/docs/images/add-new-action-overlay.png` & `collective.easyform-4.1.3/docs/images/add-new-action-overlay.png`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/docs/images/add-new-field-overlay.png` & `collective.easyform-4.1.3/docs/images/add-new-field-overlay.png`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/docs/images/add-new-fieldset-overlay.png` & `collective.easyform-4.1.3/docs/images/add-new-fieldset-overlay.png`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/docs/images/add-new-menu.png` & `collective.easyform-4.1.3/docs/images/add-new-menu.png`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/docs/images/added-new-action.png` & `collective.easyform-4.1.3/docs/images/added-new-action.png`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/docs/images/added-new-field.png` & `collective.easyform-4.1.3/docs/images/added-new-field.png`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/docs/images/added-new-fieldset.png` & `collective.easyform-4.1.3/docs/images/added-new-fieldset.png`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/docs/images/click-actions-contentview.png` & `collective.easyform-4.1.3/docs/images/click-actions-contentview.png`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/docs/images/click-add-new-action.png` & `collective.easyform-4.1.3/docs/images/click-add-new-action.png`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/docs/images/click-add-new-field.png` & `collective.easyform-4.1.3/docs/images/click-add-new-field.png`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/docs/images/click-add-new-fieldset.png` & `collective.easyform-4.1.3/docs/images/click-add-new-fieldset.png`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/docs/images/click-fields-contentview.png` & `collective.easyform-4.1.3/docs/images/click-fields-contentview.png`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/docs/images/conditional_fields_and_field_css.png` & `collective.easyform-4.1.3/docs/images/conditional_fields_and_field_css.png`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/docs/images/created-easyform-actions.png` & `collective.easyform-4.1.3/docs/images/created-easyform-actions.png`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/docs/images/created-easyform-fields.png` & `collective.easyform-4.1.3/docs/images/created-easyform-fields.png`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/docs/images/created-easyform.png` & `collective.easyform-4.1.3/docs/images/created-easyform.png`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/docs/images/default-actions-mailer.png` & `collective.easyform-4.1.3/docs/images/default-actions-mailer.png`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/docs/images/define-actions-menu-choice.png` & `collective.easyform-4.1.3/docs/images/define-actions-menu-choice.png`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/docs/images/easyform-youtube.png` & `collective.easyform-4.1.3/docs/images/easyform-youtube.png`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/docs/images/edit-xml-actions-model-button.png` & `collective.easyform-4.1.3/docs/images/edit-xml-actions-model-button.png`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/docs/images/edit-xml-actions-model-page.png` & `collective.easyform-4.1.3/docs/images/edit-xml-actions-model-page.png`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/docs/images/edit-xml-fields-model-button.png` & `collective.easyform-4.1.3/docs/images/edit-xml-fields-model-button.png`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/docs/images/edit-xml-fields-model-page.png` & `collective.easyform-4.1.3/docs/images/edit-xml-fields-model-page.png`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/docs/images/form_multicolumns.png` & `collective.easyform-4.1.3/docs/images/form_multicolumns.png`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/docs/images/mailer-adapter-message-settings.png` & `collective.easyform-4.1.3/docs/images/mailer-adapter-message-settings.png`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/docs/images/new-easyform-default-contributor.png` & `collective.easyform-4.1.3/docs/images/new-easyform-default-contributor.png`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/docs/images/new-easyform-default.png` & `collective.easyform-4.1.3/docs/images/new-easyform-default.png`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/docs/images/new-easyform-overrides.png` & `collective.easyform-4.1.3/docs/images/new-easyform-overrides.png`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/docs/images/new-easyform-thankspage-contributor.png` & `collective.easyform-4.1.3/docs/images/new-easyform-thankspage-contributor.png`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/docs/images/new-easyform-thankspage.png` & `collective.easyform-4.1.3/docs/images/new-easyform-thankspage.png`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/docs/index.rst` & `collective.easyform-4.1.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/docs/rtd-requirements.txt` & `collective.easyform-4.1.3/docs/rtd-requirements.txt`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/setup.py` & `collective.easyform-4.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = "4.1.2"
+version = "4.1.3"
 
 setup(
     name="collective.easyform",
     version=version,
     description="Forms for Plone",
     long_description=open("README.rst").read() + "\n" + open("CHANGES.rst").read(),
     # Get more strings from https://pypi.org/classifiers/
@@ -44,14 +44,15 @@
         "plone.app.textfield >= 1.2.8",
         "plone.autoform",
         "plone.dexterity",
         "plone.namedfile",
         "plone.schema",
         "plone.schemaeditor>=4.0.0b1",
         "plone.supermodel",
+        "plone.restapi",
         "Products.CMFPlone>=6.0.0b1",
         "Products.validation",
         "setuptools",
         "six",
         # -*- Extra requirements: -*-
     ],
     extras_require={
```

### Comparing `collective.easyform-4.1.2/src/collective/easyform/actions.py` & `collective.easyform-4.1.3/src/collective/easyform/actions.py`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/actions.zcml` & `collective.easyform-4.1.3/src/collective/easyform/actions.zcml`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/api.py` & `collective.easyform-4.1.3/src/collective/easyform/api.py`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/browser/action_input.pt` & `collective.easyform-4.1.3/src/collective/easyform/browser/action_input.pt`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/browser/actions.py` & `collective.easyform-4.1.3/src/collective/easyform/browser/actions.py`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/browser/actions.zcml` & `collective.easyform-4.1.3/src/collective/easyform/browser/actions.zcml`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/browser/actions_listing.pt` & `collective.easyform-4.1.3/src/collective/easyform/browser/actions_listing.pt`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/browser/configure.zcml` & `collective.easyform-4.1.3/src/collective/easyform/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/browser/controlpanel.py` & `collective.easyform-4.1.3/src/collective/easyform/browser/controlpanel.py`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/browser/easyform.css` & `collective.easyform-4.1.3/src/collective/easyform/browser/easyform.css`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/browser/easyform_form.pt` & `collective.easyform-4.1.3/src/collective/easyform/browser/easyform_form.pt`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/browser/easyform_form_embedded.pt` & `collective.easyform-4.1.3/src/collective/easyform/browser/easyform_form_embedded.pt`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/browser/easyform_layout.pt` & `collective.easyform-4.1.3/src/collective/easyform/browser/easyform_layout.pt`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/browser/exportimport.py` & `collective.easyform-4.1.3/src/collective/easyform/browser/exportimport.py`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/browser/fields.py` & `collective.easyform-4.1.3/src/collective/easyform/browser/fields.py`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/browser/fields.zcml` & `collective.easyform-4.1.3/src/collective/easyform/browser/fields.zcml`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/browser/fields_listing.pt` & `collective.easyform-4.1.3/src/collective/easyform/browser/fields_listing.pt`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/browser/label.pt` & `collective.easyform-4.1.3/src/collective/easyform/browser/label.pt`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/browser/likert.py` & `collective.easyform-4.1.3/src/collective/easyform/browser/likert.py`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/browser/likert.zcml` & `collective.easyform-4.1.3/src/collective/easyform/browser/likert.zcml`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/browser/likert_display.pt` & `collective.easyform-4.1.3/src/collective/easyform/browser/likert_display.pt`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/browser/likert_input.pt` & `collective.easyform-4.1.3/src/collective/easyform/browser/likert_input.pt`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/browser/model_listing.pt` & `collective.easyform-4.1.3/src/collective/easyform/browser/model_listing.pt`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/browser/modeleditor.pt` & `collective.easyform-4.1.3/src/collective/easyform/browser/modeleditor.pt`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/browser/rich_label.pt` & `collective.easyform-4.1.3/src/collective/easyform/browser/rich_label.pt`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/browser/saveddata.pt` & `collective.easyform-4.1.3/src/collective/easyform/browser/saveddata.pt`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/browser/saveddata_form.pt` & `collective.easyform-4.1.3/src/collective/easyform/browser/saveddata_form.pt`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/browser/thank_you.pt` & `collective.easyform-4.1.3/src/collective/easyform/browser/thank_you.pt`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/browser/view.py` & `collective.easyform-4.1.3/src/collective/easyform/browser/view.py`

 * *Files 1% similar despite different names*

```diff
@@ -296,20 +296,22 @@
                     self.context, self.context.submitLabelOverride
                 )
             else:
                 self.actions["submit"].title = self.context.submitLabel
         if "reset" in self.actions:
             self.actions["reset"].title = self.context.resetLabel
 
-    def updateWidgets(self):
-        super(EasyFormForm, self).updateWidgets()
+    def markWidgets(self):
         for w in self.widgets.values():
             if not IEasyFormWidget.providedBy(w):
-                # add marker for custom widget renderer
                 alsoProvides(w, IEasyFormWidget)
+        for g in self.groups:
+            for w in g.widgets.values():
+                if not IEasyFormWidget.providedBy(w):
+                    alsoProvides(w, IEasyFormWidget)
 
     def formMaybeForceSSL(self):
         """Redirect to an https:// URL if the 'force SSL' option is on.
 
         However, don't do so for those with rights to edit the form,
         to avoid making the form uneditable if SSL isn't configured
         properly.  These users will still get an SSL-ified form
@@ -324,14 +326,15 @@
                 secure_url = self.request["URL"].replace("http://", "https://")
                 self.request.response.redirect(secure_url, status="movedtemporarily")
 
     def update(self):
         """Update form - see interfaces.IForm"""
         self.formMaybeForceSSL()
         super(EasyFormForm, self).update()
+        self.markWidgets()
         self.template = self.form_template
         if self.request.method != "POST" or self.context.thanksPageOverride:
             # go with all but default thank you page rendering
             return
         # If an adapter has already set errors, don't re-run extraction and
         # validation, just bail out:
         # (we copy the logic from plone.app.z3cform at templates/macros.pt)
```

### Comparing `collective.easyform-4.1.2/src/collective/easyform/browser/widget.pt` & `collective.easyform-4.1.3/src/collective/easyform/browser/widget.pt`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/browser/widgets.py` & `collective.easyform-4.1.3/src/collective/easyform/browser/widgets.py`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/browser/widgets.zcml` & `collective.easyform-4.1.3/src/collective/easyform/browser/widgets.zcml`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/config.py` & `collective.easyform-4.1.3/src/collective/easyform/config.py`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/configure.zcml` & `collective.easyform-4.1.3/src/collective/easyform/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/default_schemata/fields_default.xml` & `collective.easyform-4.1.3/src/collective/easyform/default_schemata/fields_default.xml`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/default_schemata/mail_body_default.pt` & `collective.easyform-4.1.3/src/collective/easyform/default_schemata/mail_body_default.pt`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/exportimport.py` & `collective.easyform-4.1.3/src/collective/easyform/exportimport.py`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/exportimport.zcml` & `collective.easyform-4.1.3/src/collective/easyform/exportimport.zcml`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/fields.py` & `collective.easyform-4.1.3/src/collective/easyform/fields.py`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/fields.zcml` & `collective.easyform-4.1.3/src/collective/easyform/fields.zcml`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/interfaces/__init__.py` & `collective.easyform-4.1.3/src/collective/easyform/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/interfaces/actions.py` & `collective.easyform-4.1.3/src/collective/easyform/interfaces/actions.py`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/interfaces/customscript.py` & `collective.easyform-4.1.3/src/collective/easyform/interfaces/customscript.py`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/interfaces/easyform.py` & `collective.easyform-4.1.3/src/collective/easyform/interfaces/easyform.py`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/interfaces/fields.py` & `collective.easyform-4.1.3/src/collective/easyform/interfaces/fields.py`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/interfaces/mailer.py` & `collective.easyform-4.1.3/src/collective/easyform/interfaces/mailer.py`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/interfaces/savedata.py` & `collective.easyform-4.1.3/src/collective/easyform/interfaces/savedata.py`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/interfaces/validators.py` & `collective.easyform-4.1.3/src/collective/easyform/interfaces/validators.py`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/locales/collective.easyform.pot` & `collective.easyform-4.1.3/src/collective/easyform/locales/collective.easyform.pot`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/locales/de/LC_MESSAGES/collective.easyform.po` & `collective.easyform-4.1.3/src/collective/easyform/locales/de/LC_MESSAGES/collective.easyform.po`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/locales/de/LC_MESSAGES/plone.po` & `collective.easyform-4.1.3/src/collective/easyform/locales/de/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/locales/en/LC_MESSAGES/collective.easyform.po` & `collective.easyform-4.1.3/src/collective/easyform/locales/en/LC_MESSAGES/collective.easyform.po`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/locales/en/LC_MESSAGES/plone.po` & `collective.easyform-4.1.3/src/collective/easyform/locales/en/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/locales/es/LC_MESSAGES/collective.easyform.po` & `collective.easyform-4.1.3/src/collective/easyform/locales/es/LC_MESSAGES/collective.easyform.po`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 # --- PLEASE EDIT THE LINES BELOW CORRECTLY ---
 # SOME DESCRIPTIVE TITLE.
-# FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
+# Mikel Larreategi <mlarreategi@codesyntax.com>, 2018 - 2022.
+# Leonardo J. Caballero G. <leonardocaballero@gmail.com>, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: \n"
 "POT-Creation-Date: 2022-06-13 19:03+0000\n"
-"PO-Revision-Date: 2018-11-09 09:59+0100\n"
-"Last-Translator: Mikel Larreategi <mlarreategi@codesyntax.com>\n"
-"Language-Team: \n"
+"PO-Revision-Date: 2023-02-13 03:30-0400\n"
+"Last-Translator: Leonardo J. Caballero G. <leonardocaballero@gmail.com>\n"
+"Language-Team: ES <LL@li.org>\n"
+"Language: es\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"X-Generator: Virtaal 0.7.1\n"
 "Language-Code: en\n"
 "Language-Name: English\n"
 "Preferred-Encodings: utf-8 latin1\n"
 "Domain: collective.easyform\n"
-"Language: es\n"
-"X-Generator: Poedit 2.0.6\n"
 
 #: collective/easyform/browser/actions.py:137
 msgid "${items} input(s) saved"
-msgstr ""
+msgstr "${items} entrada(s) guardada(s)"
 
 #: collective/easyform/profiles/default/types/EasyForm.xml
 msgid "A web-form builder"
-msgstr ""
+msgstr "Un constructor de formularios web"
 
 #: collective/easyform/interfaces/actions.py:51
 msgid "Action type"
 msgstr "Tipo de Acción"
 
 #: collective/easyform/interfaces/easyform.py:93
 msgid "Actions Model"
@@ -42,53 +43,53 @@
 #: collective/easyform/interfaces/mailer.py:85
 msgid "Addressing"
 msgstr "Direcciónes"
 
 #: collective/easyform/interfaces/easyform.py:197
 #: collective/easyform/interfaces/fields.py:62
 msgid "Advanced"
-msgstr ""
+msgstr "Avanzado"
 
 #: collective/easyform/browser/controlpanel.py:28
 #: collective/easyform/profiles/default/registry.xml
 msgid "Allowed Fields"
 msgstr "Campos permitidos"
 
 #: collective/easyform/browser/controlpanel.py:38
 #: collective/easyform/browser/saveddata_form.pt:39
 msgid "CSV delimiter"
-msgstr ""
+msgstr "delimitador CSV"
 
 #: collective/easyform/browser/saveddata_form.pt:42
 msgid "CSV delimiter is required."
-msgstr ""
+msgstr "El delimitador CSV es obligatorio."
 
 #: collective/easyform/browser/saveddata.pt:7
 msgid "Choose an adapter."
-msgstr ""
+msgstr "Elige un adaptador."
 
 #: collective/easyform/browser/actions.py:175
 msgid "Clear all"
 msgstr "Limpiar"
 
 #: collective/easyform/default_schemata/fields_default.xml
 msgid "Comments"
-msgstr ""
+msgstr "Comentarios"
 
 #: collective/easyform/profiles/default/actions.xml
 msgid "Define form actions"
 msgstr "Configurar acciones"
 
 #: collective/easyform/profiles/default/actions.xml
 msgid "Define form fields"
 msgstr "Configurar campos"
 
 #: collective/easyform/default_schemata/actions_default.xml
 msgid "E-Mails Form Input"
-msgstr ""
+msgstr "Entrada de formulario de correos electrónicos"
 
 #: collective/easyform/profiles/default/types/EasyForm.xml
 msgid "EasyForm"
 msgstr "EasyForm"
 
 #: collective/easyform/browser/actions.py:355
 msgid "Edit Action '${fieldname}'"
@@ -100,35 +101,35 @@
 
 #: collective/easyform/browser/fields.py:98
 msgid "Edit XML Fields Model"
 msgstr "Editar XML de Modelo de Campos"
 
 #: collective/easyform/interfaces/fields.py:203
 msgid "Enter allowed choices one per line."
-msgstr ""
+msgstr "Ingrese las opciones permitidas una por línea."
 
 #: collective/easyform/browser/fields.py:187
 msgid "Error: all model elements must be 'schema'"
-msgstr ""
+msgstr "Error: todos los elementos del modelo deben ser 'schema'"
 
 #: collective/easyform/browser/fields.py:179
 msgid "Error: root tag must be 'model'"
-msgstr ""
+msgstr "Error: la etiqueta raíz debe ser 'model'"
 
 #: collective/easyform/profiles/default/actions.xml
 msgid "Export"
 msgstr "Exportar"
 
 #: collective/easyform/interfaces/easyform.py:90
 msgid "Fields Model"
 msgstr "Modelo de campos"
 
 #: collective/easyform/interfaces/mailer.py:32
 msgid "Form Submission"
-msgstr ""
+msgstr "Envío de formulario"
 
 #: collective/easyform/browser/exportimport.py:56
 msgid "Form imported."
 msgstr "Formulario importado."
 
 #: collective/easyform/interfaces/mailer.py:366
 msgid "Headers"
@@ -140,49 +141,51 @@
 
 #: collective/easyform/validators.py:58
 msgid "Links are not allowed."
 msgstr "No se permiten enlaces."
 
 #: collective/easyform/browser/saveddata.pt:6
 msgid "List of Save Data Adapters"
-msgstr ""
+msgstr "Lista de adaptadores de Guardar datos"
 
 #: collective/easyform/default_schemata/actions_default.xml
 msgid "Mailer"
-msgstr ""
+msgstr "Remitente"
 
 #: collective/easyform/validators.py:33
 msgid "Must be a valid list of email addresses (separated by commas)."
-msgstr "Tiene que ser una lista de dirección de correo electrónico válidas (separada por comas)."
+msgstr ""
+"Tiene que ser una lista de dirección de correo electrónico válidas (separada "
+"por comas)."
 
 #: collective/easyform/validators.py:43
 msgid "Must be checked."
 msgstr "Tiene que estar seleccionado."
 
 #: collective/easyform/validators.py:48
 msgid "Must be unchecked."
 msgstr "No tiene que estar seleccionado."
 
 #: collective/easyform/browser/saveddata.pt:25
 msgid "No adapters available."
-msgstr ""
+msgstr "No hay adaptadores disponibles."
 
 #: collective/easyform/interfaces/actions.py:77
 #: collective/easyform/interfaces/easyform.py:304
 #: collective/easyform/interfaces/fields.py:92
 msgid "Overrides"
 msgstr "Personalización"
 
 #: collective/easyform/interfaces/fields.py:210
 msgid "Possible answers"
-msgstr ""
+msgstr "Respuestas posibles"
 
 #: collective/easyform/interfaces/fields.py:202
 msgid "Possible questions"
-msgstr ""
+msgstr "Posibles preguntas"
 
 #: collective/easyform/interfaces/savedata.py:19
 msgid "Posting Date/Time"
 msgstr "Día y hora del envío"
 
 #: collective/easyform/vocabularies.py:30
 msgid "Redirect to"
@@ -194,56 +197,58 @@
 
 #: collective/easyform/interfaces/fields.py:176
 msgid "Rich Label"
 msgstr "Etiqueta de texto enriquecido"
 
 #: collective/easyform/browser/saveddata_form.pt:9
 msgid "Saved Data"
-msgstr ""
+msgstr "Datos guardados"
 
 #: collective/easyform/profiles/default/actions.xml
 msgid "Saved data"
 msgstr "Datos almacenados"
 
 #: collective/easyform/browser/controlpanel.py:40
 msgid "Set the default delimiter for CSV download."
-msgstr ""
+msgstr "Establezca el delimitador predeterminado para la descarga de CSV."
 
 #: collective/easyform/default_schemata/fields_default.xml
 msgid "Subject"
-msgstr ""
+msgstr "Asunto"
 
 #: collective/easyform/interfaces/easyform.py:117
 msgid "Thanks Page"
 msgstr "Página de agradecimiento"
 
 #: collective/easyform/browser/controlpanel.py:29
 #: collective/easyform/profiles/default/registry.xml
 msgid "These Fields are available for your forms."
-msgstr "Estos campos están disponibles para tus formularios"
+msgstr "Estos campos están disponibles para tus formularios."
 
 #: collective/easyform/browser/controlpanel.py:21
 msgid "This will migrate all the forms already present in the site from archetype to dexterity"
 msgstr ""
+"Esto migrará todas las formas ya presentes en el sitio del archetype a "
+"dexterity"
 
 #: collective/easyform/vocabularies.py:30
 msgid "Traverse to"
 msgstr "Ir a"
 
 #: collective/easyform/interfaces/fields.py:74
 msgid "Validators"
 msgstr "Validadores"
 
 #: collective/easyform/profiles/default/actions.xml
 msgid "View"
-msgstr ""
+msgstr "Vista"
 
 #: collective/easyform/default_schemata/fields_default.xml
 msgid "Your E-Mail Address"
-msgstr ""
+msgstr "Su dirección de correo electrónico"
 
 #. Default: "Reset"
 #: collective/easyform/interfaces/easyform.py:34
 msgid "default_resetLabel"
 msgstr "Limpiar"
 
 #. Default: "Submit"
@@ -260,118 +265,169 @@
 #: collective/easyform/interfaces/easyform.py:42
 msgid "default_thankstitle"
 msgstr "Gracias"
 
 #. Default: "Mark this field as a value to be injected into the request form for use by action adapters and is not modifiable by or exposed to the client."
 #: collective/easyform/interfaces/fields.py:149
 msgid "description_server_side_text"
-msgstr "Activar este campo para que su valor se inyecte automáticamente en la petición, se pueda utilizar por alguna acción, no sea expuesto al cliente y éste no lo pueda modificar."
+msgstr ""
+"Activar este campo para que su valor se inyecte automáticamente en la "
+"petición, se pueda utilizar por alguna acción, no sea expuesto al cliente y "
+"éste no lo pueda modificar."
 
 #: collective/easyform/browser/controlpanel.py:49
 msgid "easyform Settings"
-msgstr ""
+msgstr "Ajustes de easyform"
 
 #. Default: "${name} Header"
 #: collective/easyform/interfaces/mailer.py:397
 #: collective/easyform/interfaces/savedata.py:22
 msgid "extra_header"
 msgstr "Cabecera ${name}"
 
 #. Default: "A TALES expression that will be called after the form issuccessfully validated, but before calling an action adapter (if any) or displaying a thanks page.Form input will be in the request.form dictionary.Leave empty if unneeded. The most common use of this field is to call a python scriptto clean up form input or to script an alternative action. Any value returned by the expression is ignored.PLEASE NOTE: errors in the evaluation of this expression willcause an error on form display."
 #: collective/easyform/interfaces/easyform.py:398
 msgid "help_AfterValidationOverride_text"
-msgstr "Una expresión TALES que será llamada después que el formulario se valide, pero antes de llamar un adaptador de acción (si hay alguno) o mostrar la página de agradecimiento. Los datos introducidos en el formulario estará en el diccionario \\\"request.form\\\". Déjela vacía si no la necesita. El uso más común de este campo es para llamar un script python para limpiar la entrada del formulario o para ejecutar una acción alternativa. Cualquier valor devuelto por la expresión se ignorará. NOTA: errores en la evaluación de esta expresión causarán un error al mostrar el formulario."
+msgstr ""
+"Una expresión TALES que será llamada después que el formulario se valide, "
+"pero antes de llamar un adaptador de acción (si hay alguno) o mostrar la "
+"página de agradecimiento. Los datos introducidos en el formulario estará en "
+"el diccionario \\\"request.form\\\". Déjela vacía si no la necesita. El uso "
+"más común de este campo es para llamar un script python para limpiar la "
+"entrada del formulario o para ejecutar una acción alternativa. Cualquier "
+"valor devuelto por la expresión se ignorará. NOTA: errores en la evaluación "
+"de esta expresión causarán un error al mostrar el formulario."
 
 #. Default: "A TALES expression that will be called when the form is displayed. Leave empty if unneeded. The most common use of this field is to call a python script that sets defaults for multiple fields by pre-populating request.form. Any value returned by the expression is ignored. PLEASE NOTE: errors in the evaluation of this expression will cause an error on form display."
 #: collective/easyform/interfaces/easyform.py:378
 msgid "help_OnDisplayOverride_text"
-msgstr "Una expresión TALES que será llamada cuando el formulario se muestra. Déjela vacía si no la necesita. El uso más común de este campo es para llamar un script python que asigna valores por defecto para múltiples campos pre-populando el request.form. Cualquier valor devuelto por la expresión se ignorará. NOTA: errores en la evaluación de esta expresión causarán un error al mostrar el formulario."
+msgstr ""
+"Una expresión TALES que será llamada cuando el formulario se muestra. Déjela "
+"vacía si no la necesita. El uso más común de este campo es para llamar un "
+"script python que asigna valores por defecto para múltiples campos pre-"
+"populando el request.form. Cualquier valor devuelto por la expresión se "
+"ignorará. NOTA: errores en la evaluación de esta expresión causarán un error "
+"al mostrar el formulario."
 
 #. Default: "A TALES expression that will be evaluated to override any value otherwise entered for the BCC list. You are strongly cautioned against using unvalidated data from the request for this purpose. Leave empty if unneeded. Your expression should evaluate as a sequence of strings. PLEASE NOTE: errors in the evaluation of this expression will cause an error on form display."
 #: collective/easyform/interfaces/mailer.py:497
 msgid "help_bcc_override_text"
-msgstr "Una expresión TALES que devolverá el listado de correos electrónicos que sobreescribirán el valor del campo BCC. Ten cuidado al utilizar datos del request sin validar para esto. Déjela vacía si no la necesita. La expresión deberá devolver una lista de cadenas de texto. NOTA: errores en la evaluación de esta expresión causarán un error al mostrar el formulario."
+msgstr ""
+"Una expresión TALES que devolverá el listado de correos electrónicos que "
+"sobreescribirán el valor del campo BCC. Ten cuidado al utilizar datos del "
+"request sin validar para esto. Déjela vacía si no la necesita. La expresión "
+"deberá devolver una lista de cadenas de texto. NOTA: errores en la "
+"evaluación de esta expresión causarán un error al mostrar el formulario."
 
 #. Default: "A TALES expression that will be evaluated to override any value otherwise entered for the CC list. You are strongly cautioned against using unvalidated data from the request for this purpose. Leave empty if unneeded. Your expression should evaluate as a sequence of strings. PLEASE NOTE: errors in the evaluation of this expression will cause an error on form display."
 #: collective/easyform/interfaces/mailer.py:477
 msgid "help_cc_override_text"
-msgstr "Una expresión TALES que devolverá el listado de correos electrónicos que sobreescribirán el valor del campo CC. Ten cuidado al utilizar datos del request sin validar para esto. Déjela vacía si no la necesita. La expresión deberá devolver una lista de cadenas de texto. NOTA: errores en la evaluación de esta expresión causarán un error al mostrar el formulario."
+msgstr ""
+"Una expresión TALES que devolverá el listado de correos electrónicos que "
+"sobreescribirán el valor del campo CC. Ten cuidado al utilizar datos del "
+"request sin validar para esto. Déjela vacía si no la necesita. La expresión "
+"deberá devolver una lista de cadenas de texto. NOTA: errores en la "
+"evaluación de esta expresión causarán un error al mostrar el formulario."
 
 #. Default: "Check this to employ Cross-Site Request Forgery protection. Note that only HTTP Post actions will be allowed."
 #: collective/easyform/interfaces/easyform.py:276
 msgid "help_csrf"
-msgstr "Activar para utilizar la protección Cross-Site Request Forgery. Solo se permitirán peticiones HTTP POST."
+msgstr ""
+"Activar para utilizar la protección Cross-Site Request Forgery. Solo se "
+"permitirán peticiones HTTP POST."
 
 #. Default: "This field allows you to change default fieldset label."
 #: collective/easyform/interfaces/easyform.py:251
 msgid "help_default_fieldset_label_text"
-msgstr "Con este campo puedes modificar la etiqueta del conjunto de campos por defecto."
+msgstr ""
+"Con este campo puedes modificar la etiqueta del conjunto de campos por "
+"defecto."
 
 #. Default: "The text will be displayed after the form fields."
 #: collective/easyform/interfaces/easyform.py:107
 msgid "help_epilogue_text"
 msgstr "Este texto se mostrará después de los campos del formulario."
 
 #. Default: "A TALES expression that will be evaluated to determine whether or not to execute this action. Leave empty if unneeded, and the action will be executed. Your expression should evaluate as a boolean; return True if you wish the action to execute. PLEASE NOTE: errors in the evaluation of this expression will  cause an error on form display."
 #: collective/easyform/interfaces/actions.py:82
 msgid "help_execcondition_text"
-msgstr "Una expresión TALES que será evaluada para decidir si se ejecutará esta acción o no. Déjela vacía si no la necesita. La expresión deberá devolver un valor booleano; return True para que la acción se ejecute. NOTA: errores en la evaluación de esta expresión causarán un error al mostrar el formulario."
+msgstr ""
+"Una expresión TALES que será evaluada para decidir si se ejecutará esta "
+"acción o no. Déjela vacía si no la necesita. La expresión deberá devolver un "
+"valor booleano; return True para que la acción se ejecute. NOTA: errores en "
+"la evaluación de esta expresión causarán un error al mostrar el formulario."
 
 #: collective/easyform/interfaces/fields.py:68
 msgid "help_field_widget"
 msgstr ""
 
 #. Default: "Check this to make the form redirect to an SSL-enabled version of itself (https://) if accessed via a non-SSL URL (http://).  In order to function properly, this requires a web server that has been configured to handle the HTTPS protocol on port 443 and forward it to Zope."
 #: collective/easyform/interfaces/easyform.py:288
 msgid "help_force_ssl"
-msgstr "Activar para que el formulario se muestre en la versión con SSL activado (https://) si se accede a él desde una versión no-SSL (http://). Para que esta redirección funcione adecuadamente, el servidor web tiene que estar configurado para servir peticiones con el protocolo HTTPS en el puerto 443 y redirigir las peticiones a Zope."
+msgstr ""
+"Activar para que el formulario se muestre en la versión con SSL activado "
+"(https://) si se accede a él desde una versión no-SSL (http://). Para que "
+"esta redirección funcione adecuadamente, el servidor web tiene que estar "
+"configurado para servir peticiones con el protocolo HTTPS en el puerto 443 y "
+"redirigir las peticiones a Zope."
 
 #: collective/easyform/interfaces/easyform.py:241
 msgid "help_form_tabbing"
 msgstr ""
 
 #. Default: "Use this field to override the form action attribute. Specify a URL to which the form will post. This will bypass form validation, success action adapter and thanks page."
 #: collective/easyform/interfaces/easyform.py:364
 msgid "help_formactionoverride_text"
-msgstr "Utiliza este campo para sobreescribir el valor del atributo \"action\" del formulario. Especifica la URL a la que se enviarán los datos. Esta configuración hará que no se ejecute la validación, las acciones configuradas y la página de agradecimiento."
+msgstr ""
+"Utiliza este campo para sobreescribir el valor del atributo \"action\" del "
+"formulario. Especifica la URL a la que se enviarán los datos. Esta "
+"configuración hará que no se ejecute la validación, las acciones "
+"configuradas y la página de agradecimiento."
 
 #. Default: "Additional e-mail-header lines. Only use RFC822-compliant headers."
 #: collective/easyform/interfaces/mailer.py:389
 msgid "help_formmailer_additional_headers"
-msgstr "Cabeceras adicionales del correo electrónico enviado. Utilizar solo cabeceras RFC822."
+msgstr ""
+"Cabeceras adicionales del correo electrónico enviado. Utilizar solo "
+"cabeceras RFC822."
 
 #. Default: "E-mail addresses which receive a blind carbon copy."
 #: collective/easyform/interfaces/mailer.py:121
 msgid "help_formmailer_bcc_recipients"
 msgstr "Correos electrónicos que recibirán una copia oculta (BCC, CCO)"
 
 #. Default: "Text used as the footer at bottom, delimited from the body by a dashed line."
 #: collective/easyform/interfaces/mailer.py:225
 msgid "help_formmailer_body_footer"
 msgstr "Texto que se añade en el pie de página."
 
 #. Default: "Text appended to fields listed in mail-body"
 #: collective/easyform/interfaces/mailer.py:210
 msgid "help_formmailer_body_post"
-msgstr "Texto que se añade después los campos del cuerpo de texto."
+msgstr "Texto que se añade después los campos del cuerpo de texto"
 
 #. Default: "Text prepended to fields listed in mail-body"
 #: collective/easyform/interfaces/mailer.py:195
 msgid "help_formmailer_body_pre"
-msgstr "Texto que se añade antes de los campos del cuerpo de texto."
+msgstr "Texto que se añade antes de los campos del cuerpo de texto"
 
 #. Default: "This is a Zope Page Template used for rendering of the mail-body. You don't need to modify it, but if you know TAL (Zope's Template Attribute Language) have the full power to customize your outgoing mails."
 #: collective/easyform/interfaces/mailer.py:341
 msgid "help_formmailer_body_pt"
-msgstr "Esta es una plantilla Zope Page Templates que se utiliza para crear el texto del correo electrónico. No necesitas modificarla, pero si sabes TAL puedes personalizar los mensajes."
+msgstr ""
+"Esta es una plantilla Zope Page Templates que se utiliza para crear el texto "
+"del correo electrónico. No necesitas modificarla, pero si sabes TAL puedes "
+"personalizar los mensajes."
 
 #. Default: "Set the mime-type of the mail-body. Change this setting only if you know exactly what you are doing. Leave it blank for default behaviour."
 #: collective/easyform/interfaces/mailer.py:356
 msgid "help_formmailer_body_type"
-msgstr "Establece el tipo MIME del cuerpo del mensaje. Cambiar solo si se sabe que está haciendo. Déjalo vacío para el comportamiento habitual."
+msgstr ""
+"Establece el tipo MIME del cuerpo del mensaje. Cambiar solo si se sabe que "
+"está haciendo. Déjalo vacío para el comportamiento habitual."
 
 #. Default: "E-mail addresses which receive a carbon copy."
 #: collective/easyform/interfaces/mailer.py:108
 msgid "help_formmailer_cc_recipients"
 msgstr "Correos electrónicos que recibirán una copia del mensaje (CC)."
 
 #. Default: "The recipients e-mail address."
@@ -383,94 +439,131 @@
 #: collective/easyform/interfaces/mailer.py:62
 msgid "help_formmailer_recipient_fullname"
 msgstr "Nombre del receptor"
 
 #. Default: "Choose a form field from which you wish to extract input for the Reply-To header. NOTE: You should activate e-mail address verification for the designated field."
 #: collective/easyform/interfaces/mailer.py:134
 msgid "help_formmailer_replyto_extract"
-msgstr "Elige un campo del formulario del que se extraerá el valor de la cabecera \"Reply-To\". NOTA: Deberías activar la validación para verificar que el campo contenga una dirección de correo electrónico."
+msgstr ""
+"Elige un campo del formulario del que se extraerá el valor de la cabecera \""
+"Reply-To\". NOTA: Deberías activar la validación para verificar que el campo "
+"contenga una dirección de correo electrónico."
 
 #. Default: "Subject line of message. This is used if you do not specify a subject field or if the field is empty."
 #: collective/easyform/interfaces/mailer.py:165
 msgid "help_formmailer_subject"
-msgstr "Asunto del mensaje. Se utiliza si no eliges un campo para extraer el asunto o si el valor de dicho campo es vacío."
+msgstr ""
+"Asunto del mensaje. Se utiliza si no eliges un campo para extraer el asunto "
+"o si el valor de dicho campo es vacío."
 
 #. Default: "Choose a form field from which you wish to extract input for the mail subject line."
 #: collective/easyform/interfaces/mailer.py:181
 msgid "help_formmailer_subject_extract"
-msgstr "Elige un campo del formulario del que se extraerá el valor del asunto del mensaje."
+msgstr ""
+"Elige un campo del formulario del que se extraerá el valor del asunto del "
+"mensaje."
 
 #. Default: "Choose a form field from which you wish to extract input for the To header. If you choose anything other than \"None\", this will override the \"Recipient's \" e-mail address setting above. Be very cautious about allowing unguarded user input for this purpose."
 #: collective/easyform/interfaces/mailer.py:92
 msgid "help_formmailer_to_extract"
-msgstr "Elige un campo del formulario del que se extraerá el valor de la cabecera \"To\", es decir, a quién se enviará el formulario. Si seleccionas algo que no sea \"None\", esto sobreescribirá el valor del \"Correo electrónico del receptor. Cuidado al utilizar valores introducidos por el usuario que no se hayan validado o limpiado."
+msgstr ""
+"Elige un campo del formulario del que se extraerá el valor de la cabecera \\"
+"\"To\\\", es decir, a quién se enviará el formulario. Si seleccionas algo "
+"que no sea \\\"None\\\", esto sobreescribirá el valor del correo electrónico "
+"del \\\"Receptor\\\". Cuidado al utilizar valores introducidos por el "
+"usuario que no se hayan validado o limpiado."
 
 #. Default: "This override field allows you to insert content into the xhtml head. The typical use is to add custom CSS or JavaScript. Specify a TALES expression returning a string. The string will be inserted with no interpretation. PLEASE NOTE: errors in the evaluation of this expression will cause an error on form display."
 #: collective/easyform/interfaces/easyform.py:418
 msgid "help_headerInjection_text"
-msgstr "Este campo permite introducir código en la cabecera HTML. El uso más habitual es para introducir CSS o JavaScript. Especificar una expresión TALES que devuelva una cadena de caracteres. La cadena se incorporará tal cual al HTML. NOTA: errores en la evaluación de esta expresión causarán un error al mostrar el formulario."
+msgstr ""
+"Este campo permite introducir código en la cabecera HTML. El uso más "
+"habitual es para introducir CSS o JavaScript. Especificar una expresión "
+"TALES que devuelva una cadena de caracteres. La cadena se incorporará tal "
+"cual al HTML. TENGA EN CUENTA: errores en la evaluación de esta expresión "
+"causarán un error al mostrar el formulario."
 
 #. Default: "Field is hidden"
 #: collective/easyform/interfaces/fields.py:86
 msgid "help_hidden"
-msgstr ""
+msgstr "El campo está oculto"
 
 #. Default: "Check this to display field titles for fields that received no input. Uncheck to leave fields with no input off the list."
 #: collective/easyform/interfaces/easyform.py:167
 msgid "help_includeEmpties_text"
-msgstr "Seleccionar para mostrar los títulos de los campos que se han dejado vacíos. Si no está seleccionado, los campos vacíos no se mostrarán en el listado."
+msgstr ""
+"Seleccionar para mostrar los títulos de los campos que se han dejado vacíos. "
+"Si no está seleccionado, los campos vacíos no se mostrarán en el listado."
 
 #. Default: "Check this to include titles for fields that received no input. Uncheck to leave fields with no input out of the e-mail."
 #: collective/easyform/interfaces/mailer.py:269
 msgid "help_mailEmpties_text"
-msgstr "Seleccionar para mostrar los títulos de los campos que se han dejado vacíos en el mensaje. Si no está seleccionado, los campos vacíos no se mostrarán en el mensaje."
+msgstr ""
+"Seleccionar para mostrar los títulos de los campos que se han dejado vacíos "
+"en el mensaje. Si no está seleccionado, los campos vacíos no se mostrarán en "
+"el mensaje."
 
 #. Default: "Check this to include input for all fields (except label and file fields). If you check this, the choices in the pick box below will be ignored."
 #: collective/easyform/interfaces/mailer.py:241
 msgid "help_mailallfields_text"
-msgstr "Seleccionar para incluir todos los campos (excepto los campos de etiqueta y los de archivo). Si está seleccionado, la selección del campo siguiente se ignorará."
+msgstr ""
+"Seleccionar para incluir todos los campos (excepto los campos de etiqueta y "
+"los de archivo). Si está seleccionado, la selección del campo siguiente se "
+"ignorará."
 
 #. Default: "Pick the fields whose inputs you'd like to include in the e-mail."
 #: collective/easyform/interfaces/mailer.py:256
 msgid "help_mailfields_text"
-msgstr "Seleccionar los campos que se incluirán en el mensaje."
+msgstr ""
+"Elija los campos cuyas entradas le gustaría incluir en el correo electrónico."
 
 #: collective/easyform/interfaces/easyform.py:261
 msgid "help_method"
 msgstr ""
 
 #. Default: "optional, sets the name attribute on the form container. can be used for form analytics"
 #: collective/easyform/interfaces/easyform.py:232
 msgid "help_name_attribute"
 msgstr ""
+"opcional, establece el atributo de nombre en el contenedor del formulario. "
+"se puede usar para análisis de formularios"
 
 #. Default: "This text will be displayed above the form fields."
 #: collective/easyform/interfaces/easyform.py:99
 msgid "help_prologue_text"
 msgstr "Este texto se mostrará antes que los campos del formulario"
 
 #. Default: "A TALES expression that will be evaluated to override any value otherwise entered for the recipient e-mail address. You are strongly cautioned against usingunvalidated data from the request for this purpose. Leave empty if unneeded. Your expression should evaluate as a string. PLEASE NOTE: errors in the evaluation of this expression will cause an error on form display."
 #: collective/easyform/interfaces/mailer.py:456
-#, fuzzy
 msgid "help_recipient_override_text"
-msgstr "Una expresión TALES que se evaluará para sobreescribir cualquier valor del campo del correo electrónico del receptor del mensaje. Cuidado al utilizar datos no validados del formulario. Déjela vacía si no la necesita. La expresión debería devolver una cadena de caracteres. NOTA: errores en la evaluación de esta expresión causarán un error al mostrar el formulario."
+msgstr ""
+"Una expresión TALES que se evaluará para sobreescribir cualquier valor del "
+"campo del correo electrónico del receptor del mensaje. Cuidado al utilizar "
+"datos no validados del formulario. Déjela vacía si no la necesita. La "
+"expresión debería devolver una cadena de caracteres. TENGA EN CUENTA: "
+"errores en la evaluación de esta expresión causarán un error al mostrar el "
+"formulario."
 
 #: collective/easyform/interfaces/easyform.py:226
 msgid "help_reset_button"
 msgstr ""
 
 #. Default: "Pick any extra data you'd like saved with the form input."
 #: collective/easyform/interfaces/savedata.py:72
 msgid "help_savedataextra_text"
-msgstr "Seleccionar los datos adicionales a guardar junto con los datos del formulario."
+msgstr ""
+"Seleccionar los datos adicionales a guardar junto con los datos del "
+"formulario."
 
 #. Default: "Pick the fields whose inputs you'd like to include in the saved data. If empty, all fields will be saved."
 #: collective/easyform/interfaces/savedata.py:60
 msgid "help_savefields_text"
-msgstr "Seleccionar los campos a guardar. Si está vacío se guardarán todos."
+msgstr ""
+"Elija los campos cuyas entradas le gustaría incluir en los datos guardados. "
+"Si está vacío, se guardarán todos los campos."
 
 #. Default: "Write your script here."
 #: collective/easyform/interfaces/customscript.py:32
 msgid "help_script_body"
 msgstr "Escribir el script aquí."
 
 #. Default: "Role under which to run the script."
@@ -478,121 +571,171 @@
 msgid "help_script_proxy"
 msgstr "Rol con el que se ejecutará el script."
 
 #. Default: "Check this to send a CSV file attachment containing the values filled out in the form."
 #: collective/easyform/interfaces/mailer.py:283
 msgid "help_sendCSV_text"
 msgstr ""
+"Marque esto para enviar un archivo CSV adjunto que contenga los valores "
+"completados en el formulario."
 
 #. Default: "Check this to include the CSV/XLSX header in file attachments."
 #: collective/easyform/interfaces/mailer.py:297
 msgid "help_sendWithHeader_text"
 msgstr ""
+"Marque esto para incluir el encabezado CSV/XLSX en los archivos adjuntos."
 
 #. Default: "Check this to send a XLSX file attachment containing the values filled out in the form."
 #: collective/easyform/interfaces/mailer.py:310
 msgid "help_sendXLSX_text"
 msgstr ""
+"Marque esto para enviar un archivo XLSX adjunto que contenga los valores "
+"completados en el formulario."
 
 #. Default: "Check this to send an XML file attachment containing the values filled out in the form."
 #: collective/easyform/interfaces/mailer.py:325
 msgid "help_sendXML_text"
 msgstr ""
+"Marque esto para enviar un archivo XML adjunto que contenga los valores "
+"completados en el formulario."
 
 #. Default: "A TALES expression that will be evaluated to override the \"From\" header. Leave empty if unneeded. Your expression should evaluate as a string. PLEASE NOTE: errors in the evaluation of this expression will cause an error on form display."
 #: collective/easyform/interfaces/mailer.py:438
 msgid "help_sender_override_text"
-msgstr "Seleccionar los datos adicionales a guardar junto con los datos del formulario."
+msgstr ""
+"Una expresión TALES que se evaluará para anular el encabezado \\\"From\\\". "
+"Dejar vacío si no es necesario. Su expresión debe evaluarse como una cadena. "
+"TENGA EN CUENTA: los errores en la evaluación de esta expresión provocarán "
+"un error en la visualización del formulario."
 
 #. Default: "Check this to display input for all fields (except label and file fields). If you check this, the choices in the pick box below will be ignored."
 #: collective/easyform/interfaces/easyform.py:143
 msgid "help_showallfields_text"
-msgstr "Seleccionar para mostrar los datos de todos los campos (salvo los campos de etiqueta y de archivo). Si está seleccionado, la selección del campo siguiente se ignorará."
+msgstr ""
+"Seleccionar para mostrar los datos de todos los campos (salvo los campos de "
+"etiqueta y de archivo). Si está seleccionado, la selección del campo "
+"siguiente se ignorará."
 
 #: collective/easyform/interfaces/easyform.py:220
 msgid "help_showcancel_text"
 msgstr ""
 
 #. Default: "Pick the fields whose inputs you'd like to display on the success page."
 #: collective/easyform/interfaces/easyform.py:156
 msgid "help_showfields_text"
 msgstr "Seleccionar los campos que se mostrarán en la página de agradecimiento."
 
 #. Default: "A TALES expression that will be evaluated to override any value otherwise entered for the e-mail subject header. Leave empty if unneeded. Your expression should evaluate as a string. PLEASE NOTE: errors in the evaluation of this expression will cause an error on form display."
 #: collective/easyform/interfaces/mailer.py:419
 msgid "help_subject_override_text"
-msgstr "Una expresión TALES que se evaluará para sobreescribir cualquier valor del campo asunto. Déjela vacía si no la necesita. La expresión debería devolver una cadena de caracteres. NOTA: errores en la evaluación de esta expresión causarán un error al mostrar el formulario."
+msgstr ""
+"Una expresión TALES que se evaluará para sobreescribir cualquier valor del "
+"campo asunto. Déjela vacía si no la necesita. La expresión debería devolver "
+"una cadena de caracteres. NOTA: errores en la evaluación de esta expresión "
+"causarán un error al mostrar el formulario."
 
 #: collective/easyform/interfaces/easyform.py:214
 msgid "help_submitlabel_text"
 msgstr ""
 
 #. Default: "This override field allows you to change submit button label. The typical use is to set label with request parameters. Specify a TALES expression returning a string. PLEASE NOTE: errors in the evaluation of this expression will cause an error on form display."
 #: collective/easyform/interfaces/easyform.py:436
 msgid "help_submitlabeloverride_text"
-msgstr "Este campo permite sobreescribir el texto del botón de envío del formulario. El uso más habitual es cambiar la etiqueta según algún parámetro de la petición. NOTA: errores en la evaluación de esta expresión causarán un error al mostrar el formulario."
+msgstr ""
+"Este campo permite sobreescribir el texto del botón de envío del formulario. "
+"El uso más habitual es cambiar la etiqueta según algún parámetro de la "
+"petición. NOTA: errores en la evaluación de esta expresión causarán un error "
+"al mostrar el formulario."
 
 #. Default: "A TALES expression that will be evaluated when the formis displayed to get the field default value. Leave empty if unneeded. Your expression should evaluate as a string. PLEASE NOTE: errors in the evaluation of this expression will cause an error on form display."
 #: collective/easyform/interfaces/fields.py:98
 msgid "help_tdefault_text"
-msgstr "Una expresión TALES que se evaluará cuando se muestre el formulario para obtener el valor por defecto del campo. Déjela vacía si no la necesita. La expresión debería devolver una cadena de caracteres. NOTA: errores en la evaluación de esta expresión causarán un error al mostrar el formulario."
+msgstr ""
+"Una expresión TALES que se evaluará cuando se muestre el formulario para "
+"obtener el valor por defecto del campo. Déjela vacía si no la necesita. La "
+"expresión debería devolver una cadena de caracteres. NOTA: errores en la "
+"evaluación de esta expresión causarán un error al mostrar el formulario."
 
 #. Default: "A TALES expression that will be evaluated when the form is displayed to determine whether or not the field is enabled. Your expression should evaluate as True if the field should be included in the form, False if it should be omitted. Leave this expression field empty if unneeded: the field will be included. PLEASE NOTE: errors in the evaluation of this expression will cause an error on form display."
 #: collective/easyform/interfaces/fields.py:113
 msgid "help_tenabled_text"
 msgstr "Una expresión TALES que se evaluará para decidir si el campo está activo o no. La expresión deberá evaluarse como True si el campo se tiene que incluir en el formulario y False si no debe ser incluido. Déjela vacía si no la necesita y en ese caso el campo se incluirá. La expresión debería devolver una cadena de caracteres. NOTA: errores en la evaluación de esta expresión causarán un error al mostrar el formulario."
 
 #. Default: "Used in thanks page."
 #: collective/easyform/interfaces/easyform.py:136
 msgid "help_thanksdescription"
-msgstr "Se utiliza en la página de agradecimiento"
+msgstr "Usado en la página de agradecimiento."
 
 #. Default: "The text will be displayed after the field inputs."
 #: collective/easyform/interfaces/easyform.py:187
 msgid "help_thanksepilogue_text"
 msgstr "El texto se mostrará tras los datos del formulario."
 
 #. Default: "Use this field in place of a thanks-page designation to determine final action after calling your action adapter (if you have one). You would usually use this for a custom success template or script. Leave empty if unneeded. Otherwise, specify as you would a CMFFormController action type and argument, complete with type of action to execute (e.g., \"redirect_to\" or \"traverse_to\") and a TALES expression. For example, \"Redirect to\" and \"string:thanks-page\" would redirect to \"thanks-page\"."
 #: collective/easyform/interfaces/easyform.py:343
 msgid "help_thankspageoverride_text"
-msgstr "Este campo se utiliza en lugar de la página de agradecimiento para determinar a dónde redirigir al usuario después de la acción (si hay alguna). Normalmente se utilizará para una plantilla o script personalizado. Déjela vacía si no la necesita. El valor debe ser una acción de CMFFormController y el argumento (por ejemplo: \"redirect_to\" ó \"traverse_to\" y la expresión TALES correspondiente. Por ejemplo: redirect_to: string:thanks-page."
+msgstr ""
+"Este campo se utiliza en lugar de la página de agradecimiento para "
+"determinar a dónde redirigir al usuario después de la acción (si hay alguna)"
+". Normalmente se utilizará para una plantilla o script personalizado. Déjela "
+"vacía si no la necesita. El valor debe ser una acción de CMFFormController y "
+"el argumento (por ejemplo: \\\"redirect_to\\\" ó \\\"traverse_to\\\" y la "
+"expresión TALES correspondiente. Por ejemplo, \\\"Redirect to\\\" y \\\""
+"string:thanks-page\\\" podria redirigiría a \\\"thanks-page\\\"."
 
 #. Default: "Use this field in place of a thanks-page designation to determine final action after calling your action adapter (if you have one). You would usually use this for a custom success template or script. Leave empty if unneeded. Otherwise, specify as you would a CMFFormController action type and argument, complete with type of action to execute (e.g., \"redirect_to\" or \"traverse_to\") and a TALES expression. For example, \"Redirect to\" and \"string:thanks-page\" would redirect to \"thanks-page\"."
 #: collective/easyform/interfaces/easyform.py:322
 msgid "help_thankspageoverrideaction_text"
-msgstr "Este campo se utiliza en lugar de la página de agradecimiento para determinar a dónde redirigir al usuario después de la acción (si hay alguna). Normalmente se utilizará para una plantilla o script personalizado. Déjela vacía si no la necesita. El valor debe ser una acción de CMFFormController y el argumento (por ejemplo: \"redirect_to\" ó \"traverse_to\" y la expresión TALES correspondiente. Por ejemplo: redirect_to: string:thanks-page."
+msgstr ""
+"Este campo se utiliza en lugar de la página de agradecimiento para "
+"determinar a dónde redirigir al usuario después de la acción (si hay alguna)"
+". Normalmente se utilizará para una plantilla o script personalizado. Déjela "
+"vacía si no la necesita. El valor debe ser una acción de CMFFormController y "
+"el argumento, completo con el tipo de acción a ejecutar (por ejemplo, \\\""
+"redirect_to\\\" o \\\"traverse_to\\\") y una expresión TALES. Por ejemplo, \\"
+"\"Redirigir a\\\" y \\\"string:thanks-page\\\" redirigirían a \\\"thanks-"
+"page\\\"."
 
 #. Default: "This text will be displayed above the selected field inputs."
 #: collective/easyform/interfaces/easyform.py:179
 msgid "help_thanksprologue_text"
 msgstr "Este texto se mostrará antes de los datos del formulario."
 
 #. Default: "A TALES expression that will be evaluated when the form is validated. Validate against 'value', which will contain the field input. Return False if valid; if not valid return a string error message. E.G., \"python: test(value=='eggs', False, 'input must be eggs')\" will require \"eggs\" for input. PLEASE NOTE: errors in the evaluation of this expression will cause an error on form display."
 #: collective/easyform/interfaces/fields.py:131
 msgid "help_tvalidator_text"
-msgstr "Una expresión TALES que se evaluará al validar el formulario. Utilizar 'value' para realizar la validación, que contendrá el dato introducir. Devolver False si es válido; si no devolver el mensaje de error. Por ejemplo: python:test(value=='casa', False, 'tiene que introducir casa') requerirá que el valor introducio sea 'casa'. NOTA: errores en la evaluación de esta expresión causarán un error al mostrar el formulario."
+msgstr ""
+"Una expresión TALES que se evaluará al validar el formulario. Utilizar "
+"'value' para realizar la validación, que contendrá el dato introducir. "
+"Devolver False si es válido; si no devolver el mensaje de error. Por ejemplo:"
+" \\\"python:test(value=='casa', False, 'tiene que introducir casa')\\\" "
+"requerirá que el valor introducio sea \\\"casa\\\". NOTA: errores en la "
+"evaluación de esta expresión causarán un error al mostrar el formulario."
 
 #: collective/easyform/interfaces/easyform.py:269
 msgid "help_unload_protection"
 msgstr ""
 
 #. Default: "Do you wish to have column names on the first line of downloaded input?"
 #: collective/easyform/interfaces/savedata.py:86
 msgid "help_usecolumnnames_text"
-msgstr "¿Añadir los nombres de los campos como primera línea del archivo descargado?"
+msgstr ""
+"¿Añadir los nombres de los campos como primera línea del archivo descargado?"
 
 #. Default: "Select the validators to use on this field"
 #: collective/easyform/interfaces/fields.py:75
 msgid "help_userfield_validators"
 msgstr "Seleccionar los validadores de este campo"
 
 #. Default: "Pick any items from the HTTP headers that you'd like to insert as X- headers in the message."
 #: collective/easyform/interfaces/mailer.py:373
 msgid "help_xinfo_headers_text"
-msgstr "Seleccionar cualquier elemento de las cabeceras HTTP que se quiera introducir como cabecera X-header del mensaje."
+msgstr ""
+"Seleccionar cualquier elemento de las cabeceras HTTP que se quiera "
+"introducir como cabecera X-header del mensaje."
 
 #: collective/easyform/browser/exportimport.py:46
 msgid "import"
 msgstr "Importar"
 
 #. Default: "After Validation Script"
 #: collective/easyform/interfaces/easyform.py:395
@@ -618,15 +761,15 @@
 #: collective/easyform/interfaces/easyform.py:275
 msgid "label_csrf"
 msgstr "Protección CSRF"
 
 #. Default: "Custom Script"
 #: collective/easyform/actions.py:905
 msgid "label_customscript_action"
-msgstr ""
+msgstr "Script personalizado"
 
 #. Default: "Custom Default Fieldset Label"
 #: collective/easyform/interfaces/easyform.py:247
 msgid "label_default_fieldset_label_text"
 msgstr "Etiqueta personalizada del conjunto de campos por defecto"
 
 #. Default: "Download Format"
@@ -733,75 +876,75 @@
 #: collective/easyform/interfaces/mailer.py:91
 msgid "label_formmailer_to_extract"
 msgstr "Extraer Receptor"
 
 #. Default: "HCaptcha"
 #: collective/easyform/fields.py:234
 msgid "label_hcaptcha_field"
-msgstr ""
+msgstr "HCaptcha"
 
 #. Default: "Header Injection"
 #: collective/easyform/interfaces/easyform.py:417
 msgid "label_headerInjection_text"
 msgstr "Inyección de cabeceras"
 
 #. Default: "Hidden"
 #: collective/easyform/interfaces/fields.py:85
 msgid "label_hidden"
-msgstr ""
+msgstr "Oculto"
 
 #. Default: "Include Empties"
 #: collective/easyform/interfaces/easyform.py:166
 msgid "label_includeEmpties_text"
 msgstr "Incluir valores vacíos"
 
 #. Default: "Label"
 #: collective/easyform/fields.py:209
 msgid "label_label_field"
 msgstr "Etiqueta"
 
 #. Default: "Likert"
 #: collective/easyform/fields.py:285
 msgid "label_likert_field"
-msgstr ""
+msgstr "Me gusta"
 
 #. Default: "Include Empties"
 #: collective/easyform/interfaces/mailer.py:268
 msgid "label_mailEmpties_text"
 msgstr "Incluir vacíos"
 
 #. Default: "Include All Fields"
 #: collective/easyform/interfaces/mailer.py:240
 msgid "label_mailallfields_text"
 msgstr "Incluir todos los campos"
 
 #. Default: "Mailer"
 #: collective/easyform/actions.py:900
 msgid "label_mailer_action"
-msgstr ""
+msgstr "Remitente"
 
 #. Default: "Show Responses"
 #: collective/easyform/interfaces/mailer.py:255
 msgid "label_mailfields_text"
 msgstr "Mostrar respuestas"
 
 #. Default: "Form method"
 #: collective/easyform/interfaces/easyform.py:260
 msgid "label_method"
 msgstr "Método del formulario"
 
 #. Default: "Name attribute"
 #: collective/easyform/interfaces/easyform.py:231
 msgid "label_name_attribute"
-msgstr ""
+msgstr "Atributo de nombre"
 
 #. Default: "NorobotCaptcha"
 #: collective/easyform/fields.py:245
 msgid "label_norobot_field"
-msgstr ""
+msgstr "NorobotCaptcha"
 
 #. Default: "Form Prologue"
 #: collective/easyform/interfaces/easyform.py:98
 msgid "label_prologue_text"
 msgstr "Prólogo del formulario"
 
 #. Default: "ReCaptcha"
@@ -823,15 +966,15 @@
 #: collective/easyform/fields.py:211
 msgid "label_richlabel_field"
 msgstr "Etiqueta de texto enriquecido"
 
 #. Default: "Save Data"
 #: collective/easyform/actions.py:910
 msgid "label_savedata_action"
-msgstr ""
+msgstr "Guardar datos"
 
 #. Default: "Extra Data"
 #: collective/easyform/interfaces/savedata.py:71
 msgid "label_savedataextra_text"
 msgstr "Datos adicionales"
 
 #. Default: "Saved Fields"
@@ -848,30 +991,30 @@
 #: collective/easyform/interfaces/customscript.py:20
 msgid "label_script_proxy"
 msgstr "Proxy rol"
 
 #. Default: "Send CSV data attachment"
 #: collective/easyform/interfaces/mailer.py:282
 msgid "label_sendCSV_text"
-msgstr ""
+msgstr "Enviar archivo adjunto de datos CSV"
 
 #. Default: "Include header in attached CSV/XLSX data"
 #: collective/easyform/interfaces/mailer.py:296
 msgid "label_sendWithHeader_text"
-msgstr ""
+msgstr "Incluir encabezado en los datos CSV/XLSX adjuntos"
 
 #. Default: "Send XLSX data attachment"
 #: collective/easyform/interfaces/mailer.py:309
 msgid "label_sendXLSX_text"
-msgstr ""
+msgstr "Enviar archivo adjunto de datos XLSX"
 
 #. Default: "Send XML data attachment"
 #: collective/easyform/interfaces/mailer.py:324
 msgid "label_sendXML_text"
-msgstr ""
+msgstr "Enviar archivo adjunto de datos XML"
 
 #. Default: "Sender Expression"
 #: collective/easyform/interfaces/mailer.py:437
 msgid "label_sender_override_text"
 msgstr "Expresión del remitente"
 
 #. Default: "Server-Side Variable"
@@ -967,28 +1110,29 @@
 #. Default: "HTTP Headers"
 #: collective/easyform/interfaces/mailer.py:372
 msgid "label_xinfo_headers_text"
 msgstr "Cabeceras HTTP"
 
 #: collective/easyform/browser/controlpanel.py:20
 msgid "migrate all the forms to dexterity"
-msgstr ""
+msgstr "migrar todas las formas a dexterity"
 
 #: collective/easyform/browser/view.py:417
 msgid "msg_file_not_allowed"
 msgstr "Archivo no permitido"
 
 #: collective/easyform/browser/view.py:408
 msgid "msg_file_too_big"
 msgstr "Archivo demasiado grande"
 
 #. Default: "The saved data of ${formname} stored in the adapter ${adapter}"
 #: collective/easyform/browser/saveddata_form.pt:14
 msgid "saveddata_form_description"
 msgstr ""
+"Los datos guardados de ${formname} almacenados en el adaptador ${adapter}"
 
 #. Default: "Comma-Separated Values"
 #: collective/easyform/vocabularies.py:79
 msgid "vocabulary_csv_text"
 msgstr "Archivo CSV (separado por comas)"
 
 #. Default: "Posting Date/Time"
@@ -1000,8 +1144,8 @@
 #: collective/easyform/vocabularies.py:78
 msgid "vocabulary_tsv_text"
 msgstr "Archivo TSV (separado por tabulaciones)"
 
 #. Default: "XLSX"
 #: collective/easyform/vocabularies.py:84
 msgid "vocabulary_xlsx_text"
-msgstr ""
+msgstr "XLSX"
```

### Comparing `collective.easyform-4.1.2/src/collective/easyform/locales/es/LC_MESSAGES/plone.po` & `collective.easyform-4.1.3/src/collective/easyform/locales/es/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/locales/eu/LC_MESSAGES/collective.easyform.po` & `collective.easyform-4.1.3/src/collective/easyform/locales/eu/LC_MESSAGES/collective.easyform.po`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/locales/eu/LC_MESSAGES/plone.po` & `collective.easyform-4.1.3/src/collective/easyform/locales/eu/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/locales/fr/LC_MESSAGES/collective.easyform.po` & `collective.easyform-4.1.3/src/collective/easyform/locales/fr/LC_MESSAGES/collective.easyform.po`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/locales/fr/LC_MESSAGES/plone.po` & `collective.easyform-4.1.3/src/collective/easyform/locales/fr/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/locales/it/LC_MESSAGES/collective.easyform.po` & `collective.easyform-4.1.3/src/collective/easyform/locales/it/LC_MESSAGES/collective.easyform.po`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/locales/it/LC_MESSAGES/plone.po` & `collective.easyform-4.1.3/src/collective/easyform/locales/it/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/locales/ja/LC_MESSAGES/collective.easyform.po` & `collective.easyform-4.1.3/src/collective/easyform/locales/ja/LC_MESSAGES/collective.easyform.po`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/locales/ja/LC_MESSAGES/plone.po` & `collective.easyform-4.1.3/src/collective/easyform/locales/ja/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/locales/nl/LC_MESSAGES/collective.easyform.po` & `collective.easyform-4.1.3/src/collective/easyform/locales/nl/LC_MESSAGES/collective.easyform.po`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/locales/nl/LC_MESSAGES/plone.po` & `collective.easyform-4.1.3/src/collective/easyform/locales/nl/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/locales/plone.pot` & `collective.easyform-4.1.3/src/collective/easyform/locales/plone.pot`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/locales/pt_BR/LC_MESSAGES/collective.easyform.po` & `collective.easyform-4.1.3/src/collective/easyform/locales/pt_BR/LC_MESSAGES/collective.easyform.po`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/locales/pt_BR/LC_MESSAGES/plone.po` & `collective.easyform-4.1.3/src/collective/easyform/locales/pt_BR/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/locales/uk/LC_MESSAGES/collective.easyform.po` & `collective.easyform-4.1.3/src/collective/easyform/locales/uk/LC_MESSAGES/collective.easyform.po`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/locales/uk/LC_MESSAGES/plone.po` & `collective.easyform-4.1.3/src/collective/easyform/locales/uk/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/migration/actions.py` & `collective.easyform-4.1.3/src/collective/easyform/migration/actions.py`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/migration/data.py` & `collective.easyform-4.1.3/src/collective/easyform/migration/data.py`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/migration/fields.py` & `collective.easyform-4.1.3/src/collective/easyform/migration/fields.py`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/migration/pfg.py` & `collective.easyform-4.1.3/src/collective/easyform/migration/pfg.py`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/permissions.zcml` & `collective.easyform-4.1.3/src/collective/easyform/permissions.zcml`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/profiles/default/actions.xml` & `collective.easyform-4.1.3/src/collective/easyform/profiles/default/actions.xml`

 * *Files 10% similar despite different names*

#### Comparing `collective.easyform-4.1.2/src/collective/easyform/profiles/default/actions.xml` & `collective.easyform-4.1.3/src/collective/easyform/profiles/default/actions.xml`

```diff
@@ -1,72 +1,72 @@
 <?xml version="1.0" encoding="utf-8"?>
 <object xmlns:i18n="http://xml.zope.org/namespaces/i18n" meta_type="Plone Actions Tool" name="portal_actions">
   <object meta_type="CMF Action Category" name="object">
     <object meta_type="CMF Action" name="easyform-view" insert-after="folderContents" i18n:domain="collective.easyform">
       <property name="title" i18n:translate="">View</property>
       <property name="description" i18n:translate=""/>
       <property name="url_expr">python:context.restrictedTraverse('@@get-easyform-url')('')</property>
-      <property name="icon_expr"/>
+      <property name="icon_expr">string:ui-checks</property>
       <property name="available_expr">python:object.portal_type == 'EasyForm' and object.restrictedTraverse('@@is-sub-easyform')()</property>
       <property name="permissions">
         <element value="Manage portal"/>
       </property>
       <property name="visible">True</property>
     </object>
   </object>
   <object meta_type="CMF Action Category" name="object_buttons">
     <object meta_type="CMF Action" name="export" i18n:domain="collective.easyform">
       <property name="title" i18n:translate="">Export</property>
       <property name="description" i18n:translate=""/>
       <property name="url_expr">python:context.restrictedTraverse('@@get-easyform-url')('@@export-easyform')</property>
-      <property name="icon_expr"/>
+      <property name="icon_expr">string:box-arrow-right</property>
       <property name="available_expr">python:object.portal_type == 'EasyForm'</property>
       <property name="permissions">
         <element value="Manage portal"/>
       </property>
       <property name="visible">True</property>
     </object>
     <object meta_type="CMF Action" name="import" i18n:domain="collective.easyform">
       <property name="title" i18n:translate="">Import</property>
       <property name="description" i18n:translate=""/>
       <property name="url_expr">python:context.restrictedTraverse('@@get-easyform-url')('@@import-easyform')</property>
-      <property name="icon_expr"/>
+      <property name="icon_expr">string:box-arrow-in-left</property>
       <property name="available_expr">python:object.portal_type == 'EasyForm'</property>
       <property name="permissions">
         <element value="Manage portal"/>
       </property>
       <property name="visible">True</property>
     </object>
     <object meta_type="CMF Action" name="saveddata" i18n:domain="collective.easyform">
       <property name="title" i18n:translate="">Saved data</property>
       <property name="description" i18n:translate=""/>
       <property name="url_expr">python:context.restrictedTraverse('@@get-easyform-url')('@@saveddata')</property>
-      <property name="icon_expr"/>
+      <property name="icon_expr">string:database</property>
       <property name="available_expr">python:object.portal_type == 'EasyForm'</property>
       <property name="permissions">
         <element value="collective.easyform: Download Saved Input"/>
       </property>
       <property name="visible">True</property>
     </object>
     <object meta_type="CMF Action" name="Fields" i18n:domain="collective.easyform">
       <property name="title" i18n:translate="">Define form fields</property>
       <property name="description" i18n:translate=""/>
       <property name="url_expr">python:context.restrictedTraverse('@@get-easyform-url')('fields')</property>
-      <property name="icon_expr"/>
+      <property name="icon_expr">string:list</property>
       <property name="available_expr">python:object.portal_type == 'EasyForm'</property>
       <property name="permissions">
         <element value="Modify portal content"/>
       </property>
       <property name="visible">True</property>
     </object>
     <object meta_type="CMF Action" name="Actions" i18n:domain="collective.easyform">
       <property name="title" i18n:translate="">Define form actions</property>
       <property name="description" i18n:translate=""/>
       <property name="url_expr">python:context.restrictedTraverse('@@get-easyform-url')('actions')</property>
-      <property name="icon_expr"/>
+      <property name="icon_expr">string:list-check</property>
       <property name="available_expr">python:object.portal_type == 'EasyForm'</property>
       <property name="permissions">
         <element value="Modify portal content"/>
       </property>
       <property name="visible">True</property>
     </object>
   </object>
```

### Comparing `collective.easyform-4.1.2/src/collective/easyform/profiles/default/registry.xml` & `collective.easyform-4.1.3/src/collective/easyform/profiles/default/registry.xml`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/profiles/default/rolemap.xml` & `collective.easyform-4.1.3/src/collective/easyform/profiles/default/rolemap.xml`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/profiles/default/types/EasyForm.xml` & `collective.easyform-4.1.3/src/collective/easyform/profiles/default/types/EasyForm.xml`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/profiles/uninstall/actions.xml` & `collective.easyform-4.1.3/src/collective/easyform/profiles/uninstall/actions.xml`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/serializer.py` & `collective.easyform-4.1.3/src/collective/easyform/serializer.py`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/tests/PloneLogo.png` & `collective.easyform-4.1.3/src/collective/easyform/tests/PloneLogo.png`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/tests/action_errors.rst` & `collective.easyform-4.1.3/src/collective/easyform/tests/action_errors.rst`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/tests/attachment.rst` & `collective.easyform-4.1.3/src/collective/easyform/tests/attachment.rst`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/tests/base.py` & `collective.easyform-4.1.3/src/collective/easyform/tests/base.py`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/tests/basic.rst` & `collective.easyform-4.1.3/src/collective/easyform/tests/basic.rst`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/tests/browser.rst` & `collective.easyform-4.1.3/src/collective/easyform/tests/browser.rst`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/tests/fixtures/fieldset_file.xml` & `collective.easyform-4.1.3/src/collective/easyform/tests/fixtures/fieldset_file.xml`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/tests/fixtures/fieldset_form.xml` & `collective.easyform-4.1.3/src/collective/easyform/tests/fixtures/fieldset_form.xml`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/tests/fixtures/fieldset_multiple_choice.xml` & `collective.easyform-4.1.3/src/collective/easyform/tests/fixtures/fieldset_multiple_choice.xml`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/tests/fixtures/fieldset_recaptcha.xml` & `collective.easyform-4.1.3/src/collective/easyform/tests/fixtures/fieldset_recaptcha.xml`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/tests/fixtures/fieldset_with_single_field.xml` & `collective.easyform-4.1.3/src/collective/easyform/tests/fixtures/fieldset_with_single_field.xml`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/tests/fixtures/hcaptcha.xml` & `collective.easyform-4.1.3/src/collective/easyform/tests/fixtures/hcaptcha.xml`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/tests/fixtures/hidden_form.xml` & `collective.easyform-4.1.3/src/collective/easyform/tests/fixtures/hidden_form.xml`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/tests/fixtures/radio_form.xml` & `collective.easyform-4.1.3/src/collective/easyform/tests/fixtures/radio_form.xml`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/tests/fixtures/recaptcha.xml` & `collective.easyform-4.1.3/src/collective/easyform/tests/fixtures/recaptcha.xml`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/tests/fixtures/single_field.xml` & `collective.easyform-4.1.3/src/collective/easyform/tests/fixtures/single_field.xml`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/tests/fixtures/wrapper_template.pt` & `collective.easyform-4.1.3/src/collective/easyform/tests/fixtures/wrapper_template.pt`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/tests/robot/keywords.robot` & `collective.easyform-4.1.3/src/collective/easyform/tests/robot/keywords.robot`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/tests/robot/test_addform.robot` & `collective.easyform-4.1.3/src/collective/easyform/tests/robot/test_addform.robot`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/tests/robot/test_editxmlmodel.robot` & `collective.easyform-4.1.3/src/collective/easyform/tests/robot/test_editxmlmodel.robot`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/tests/robot/test_headerinjection.robot` & `collective.easyform-4.1.3/src/collective/easyform/tests/robot/test_headerinjection.robot`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/tests/robot/todo_test_addaction.robot` & `collective.easyform-4.1.3/src/collective/easyform/tests/robot/todo_test_addaction.robot`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/tests/robot/todo_test_addfield.robot` & `collective.easyform-4.1.3/src/collective/easyform/tests/robot/todo_test_addfield.robot`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/tests/robot/todo_test_addfieldset.robot` & `collective.easyform-4.1.3/src/collective/easyform/tests/robot/todo_test_addfieldset.robot`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/tests/robot/todo_test_submit.robot` & `collective.easyform-4.1.3/src/collective/easyform/tests/robot/todo_test_submit.robot`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/tests/serverside_field.rst` & `collective.easyform-4.1.3/src/collective/easyform/tests/serverside_field.rst`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/tests/ssl.rst` & `collective.easyform-4.1.3/src/collective/easyform/tests/ssl.rst`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/tests/testApi.py` & `collective.easyform-4.1.3/src/collective/easyform/tests/testApi.py`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/tests/testControlpanel.py` & `collective.easyform-4.1.3/src/collective/easyform/tests/testControlpanel.py`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/tests/testCustomScript.py` & `collective.easyform-4.1.3/src/collective/easyform/tests/testCustomScript.py`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/tests/testDocTests.py` & `collective.easyform-4.1.3/src/collective/easyform/tests/testDocTests.py`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/tests/testEmbedding.py` & `collective.easyform-4.1.3/src/collective/easyform/tests/testEmbedding.py`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/tests/testEvents.py` & `collective.easyform-4.1.3/src/collective/easyform/tests/testEvents.py`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/tests/testLikert.py` & `collective.easyform-4.1.3/src/collective/easyform/tests/testLikert.py`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/tests/testMailer.py` & `collective.easyform-4.1.3/src/collective/easyform/tests/testMailer.py`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/tests/testMisc.py` & `collective.easyform-4.1.3/src/collective/easyform/tests/testMisc.py`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/tests/testSavedDataSerializer.py` & `collective.easyform-4.1.3/src/collective/easyform/tests/testSavedDataSerializer.py`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/tests/testSaver.py` & `collective.easyform-4.1.3/src/collective/easyform/tests/testSaver.py`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/tests/testSetup.py` & `collective.easyform-4.1.3/src/collective/easyform/tests/testSetup.py`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/tests/testThanksPage.py` & `collective.easyform-4.1.3/src/collective/easyform/tests/testThanksPage.py`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/tests/testValidators.py` & `collective.easyform-4.1.3/src/collective/easyform/tests/testValidators.py`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/tests/test_robot.py` & `collective.easyform-4.1.3/src/collective/easyform/tests/test_robot.py`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/upgrades/1002.zcml` & `collective.easyform-4.1.3/src/collective/easyform/upgrades/1002.zcml`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/upgrades/1007.zcml` & `collective.easyform-4.1.3/src/collective/easyform/upgrades/1007.zcml`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/upgrades/__init__.py` & `collective.easyform-4.1.3/src/collective/easyform/upgrades/__init__.py`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/upgrades/configure.zcml` & `collective.easyform-4.1.3/src/collective/easyform/upgrades/configure.zcml`

 * *Files 11% similar despite different names*

```diff
@@ -10,9 +10,10 @@
   <include file="1009.zcml" />
   <include file="1010.zcml" />
   <include file="1011.zcml" />
   <include file="1012.zcml" />
   <include file="1013.zcml" />
   <include file="1014.zcml" />
   <include file="1015.zcml" />
+  <include file="1016.zcml" />
 
 </configure>
```

### Comparing `collective.easyform-4.1.2/src/collective/easyform/validators.py` & `collective.easyform-4.1.3/src/collective/easyform/validators.py`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/validators.zcml` & `collective.easyform-4.1.3/src/collective/easyform/validators.zcml`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/vocabularies.py` & `collective.easyform-4.1.3/src/collective/easyform/vocabularies.py`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective/easyform/vocabularies.zcml` & `collective.easyform-4.1.3/src/collective/easyform/vocabularies.zcml`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.2/src/collective.easyform.egg-info/PKG-INFO` & `collective.easyform-4.1.3/src/collective.easyform.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.easyform
-Version: 4.1.2
+Version: 4.1.3
 Summary: Forms for Plone
 Home-page: https://github.com/collective/collective.easyform
 Author: Roman Kozlovskyi
 Author-email: krzroman@gmail.com
 Maintainer: Plone Release Team
 Maintainer-email: releaseteam@plone.org
 License: GPLv2
@@ -342,14 +342,30 @@
 - 3.x targets Plone 5.2
 - 4.x targets Plone 6, on Python 3
 
 Changelog
 =========
 
 
+4.1.3 (2023-05-16)
+------------------
+
+
+Bug fixes:
+
+- Add upgrade step and profile to update contenttype icon in registry.
+  [maurits]
+
+- Add icon expressions for actions.
+  [maurits]
+
+- Update Spanish translations.
+  [macagua]
+
+
 4.1.2 (2023-01-02)
 ------------------
 
 - Define 'Edit' and 'View' icons for the form. (#390)
   [frapell]
 
 - Require at least Python 3.8.  Test with 3.8-3.11.  [maurits]
@@ -366,14 +382,17 @@
 
 - Prevent RichLabel fields from breaking the form
   [MrTango]
 
 - Schemaeditor UI: close modals and reload fields(sets) when saving.
   [petschki]
 
+- Fix bug which did not render correctly GroupForm widgets (see #370)
+  [petschki]
+
 
 4.1.0 (2022-08-10)
 ------------------
 
 New features:
 
 - Add support for field level CSS classes.
```

### Comparing `collective.easyform-4.1.2/src/collective.easyform.egg-info/SOURCES.txt` & `collective.easyform-4.1.3/src/collective.easyform.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -217,9 +217,12 @@
 src/collective/easyform/upgrades/1009.zcml
 src/collective/easyform/upgrades/1010.zcml
 src/collective/easyform/upgrades/1011.zcml
 src/collective/easyform/upgrades/1012.zcml
 src/collective/easyform/upgrades/1013.zcml
 src/collective/easyform/upgrades/1014.zcml
 src/collective/easyform/upgrades/1015.zcml
+src/collective/easyform/upgrades/1016.zcml
 src/collective/easyform/upgrades/__init__.py
-src/collective/easyform/upgrades/configure.zcml
+src/collective/easyform/upgrades/configure.zcml
+src/collective/easyform/upgrades/profiles/1016/actions.xml
+src/collective/easyform/upgrades/profiles/1016/registry.xml
```

### Comparing `collective.easyform-4.1.2/src/collective.easyform.egg-info/requires.txt` & `collective.easyform-4.1.3/src/collective.easyform.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 plone.app.textfield>=1.2.8
 plone.autoform
 plone.dexterity
 plone.namedfile
 plone.schema
 plone.schemaeditor>=4.0.0b1
 plone.supermodel
+plone.restapi
 Products.CMFPlone>=6.0.0b1
 Products.validation
 setuptools
 six
 
 [downloadxlsx]
 openpyxl
```

