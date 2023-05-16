# Comparing `tmp/django-entries-0.1.8.tar.gz` & `tmp/django-entries-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-entries-0.1.8.tar", max compression
+gzip compressed data, was "django-entries-0.1.9.tar", max compression
```

## Comparing `django-entries-0.1.8.tar` & `django-entries-0.1.9.tar`

### file list

```diff
@@ -1,41 +1,44 @@
--rw-r--r--   0        0        0     1189 2021-12-04 16:31:52.348327 django-entries-0.1.8/README.md
--rw-r--r--   0        0        0        0 2021-12-04 15:10:47.921810 django-entries-0.1.8/entries/__init__.py
--rw-r--r--   0        0        0      194 2021-12-04 15:10:47.922771 django-entries-0.1.8/entries/admin.py
--rw-r--r--   0        0        0      146 2021-12-04 15:10:47.924556 django-entries-0.1.8/entries/apps.py
--rw-r--r--   0        0        0      946 2021-12-04 15:10:47.926071 django-entries-0.1.8/entries/forms.py
--rw-r--r--   0        0        0     2999 2021-12-04 15:10:47.927441 django-entries-0.1.8/entries/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2021-12-04 15:10:47.927685 django-entries-0.1.8/entries/migrations/__init__.py
--rw-r--r--   0        0        0     2551 2021-12-07 11:08:12.675079 django-entries-0.1.8/entries/models.py
--rw-r--r--   0        0        0     1082 2021-12-04 15:10:47.930598 django-entries-0.1.8/entries/static/css/starter.css
--rw-r--r--   0        0        0     6311 2021-12-04 15:10:47.932998 django-entries-0.1.8/entries/static/img/favicons/android-chrome-192x192.png
--rw-r--r--   0        0        0    18345 2021-12-04 15:10:47.934911 django-entries-0.1.8/entries/static/img/favicons/android-chrome-512x512.png
--rw-r--r--   0        0        0     5734 2021-12-04 15:10:47.936200 django-entries-0.1.8/entries/static/img/favicons/apple-touch-icon.png
--rw-r--r--   0        0        0      570 2021-12-04 15:10:47.937326 django-entries-0.1.8/entries/static/img/favicons/favicon-16x16.png
--rw-r--r--   0        0        0     1110 2021-12-04 15:10:47.938437 django-entries-0.1.8/entries/static/img/favicons/favicon-32x32.png
--rw-r--r--   0        0        0    15406 2021-12-04 15:10:47.939346 django-entries-0.1.8/entries/static/img/favicons/favicon.ico
--rw-r--r--   0        0        0      264 2021-12-04 15:10:47.940024 django-entries-0.1.8/entries/static/img/favicons/site.webmanifest
--rw-r--r--   0        0        0      407 2021-12-04 15:10:47.940878 django-entries-0.1.8/entries/templates/_favicons.html
--rw-r--r--   0        0        0       47 2021-12-04 15:10:47.941564 django-entries-0.1.8/entries/templates/_form.html
--rw-r--r--   0        0        0      187 2021-12-04 15:10:47.942340 django-entries-0.1.8/entries/templates/_messages.html
--rw-r--r--   0        0        0      361 2021-12-04 15:10:47.943063 django-entries-0.1.8/entries/templates/_meta.html
--rw-r--r--   0        0        0      387 2021-12-04 15:10:47.943813 django-entries-0.1.8/entries/templates/_nav.html
--rw-r--r--   0        0        0      582 2021-12-04 15:10:47.944629 django-entries-0.1.8/entries/templates/about.html
--rw-r--r--   0        0        0     1337 2021-12-04 15:10:47.945402 django-entries-0.1.8/entries/templates/base.html
--rw-r--r--   0        0        0      947 2021-12-07 11:08:12.677045 django-entries-0.1.8/entries/templates/entry_detail.html
--rw-r--r--   0        0        0      353 2021-12-04 15:10:47.948144 django-entries-0.1.8/entries/templates/entry_edit.html
--rw-r--r--   0        0        0     1058 2021-12-04 15:10:47.949606 django-entries-0.1.8/entries/templates/entry_list.html
--rw-r--r--   0        0        0      165 2021-12-04 15:10:47.950729 django-entries-0.1.8/entries/templates/home.html
--rw-r--r--   0        0        0     2040 2021-12-04 15:10:47.951486 django-entries-0.1.8/entries/tests/conftest.py
--rw-r--r--   0        0        0     1264 2021-12-04 15:10:47.952237 django-entries-0.1.8/entries/tests/test_entry_create.py
--rw-r--r--   0        0        0     1318 2021-12-04 15:10:47.952953 django-entries-0.1.8/entries/tests/test_entry_delete.py
--rw-r--r--   0        0        0     1843 2021-12-06 10:05:21.507973 django-entries-0.1.8/entries/tests/test_entry_edit.py
--rw-r--r--   0        0        0      859 2021-12-04 15:10:47.954518 django-entries-0.1.8/entries/tests/test_entry_read.py
--rw-r--r--   0        0        0     1096 2021-12-04 15:10:47.955311 django-entries-0.1.8/entries/tests/test_forms.py
--rw-r--r--   0        0        0     1085 2021-12-04 15:10:47.956097 django-entries-0.1.8/entries/tests/test_utils.py
--rw-r--r--   0        0        0      546 2021-12-07 11:08:12.678895 django-entries-0.1.8/entries/urls.py
--rw-r--r--   0        0        0      607 2021-12-04 15:10:47.957758 django-entries-0.1.8/entries/utils.py
--rw-r--r--   0        0        0      497 2021-12-04 15:10:47.958617 django-entries-0.1.8/entries/validators.py
--rw-r--r--   0        0        0     2363 2021-12-07 08:47:51.451744 django-entries-0.1.8/entries/views.py
--rw-r--r--   0        0        0     1431 2021-12-07 11:16:08.851928 django-entries-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     2264 2021-12-07 11:16:35.572976 django-entries-0.1.8/setup.py
--rw-r--r--   0        0        0     2195 2021-12-07 11:16:35.573355 django-entries-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1846 2021-12-08 15:46:18.117439 django-entries-0.1.9/README.md
+-rw-r--r--   0        0        0        0 2021-12-04 15:10:47.921810 django-entries-0.1.9/entries/__init__.py
+-rw-r--r--   0        0        0      194 2021-12-07 12:47:48.656115 django-entries-0.1.9/entries/admin.py
+-rw-r--r--   0        0        0      146 2021-12-04 15:10:47.924556 django-entries-0.1.9/entries/apps.py
+-rw-r--r--   0        0        0     3754 2021-12-08 15:55:01.955983 django-entries-0.1.9/entries/docs/infinity_scroll.md
+-rw-r--r--   0        0        0      946 2021-12-07 15:15:57.534998 django-entries-0.1.9/entries/forms.py
+-rw-r--r--   0        0        0     2985 2021-12-08 15:48:01.529716 django-entries-0.1.9/entries/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2021-12-04 15:10:47.927685 django-entries-0.1.9/entries/migrations/__init__.py
+-rw-r--r--   0        0        0     2583 2021-12-08 14:44:00.445763 django-entries-0.1.9/entries/models.py
+-rw-r--r--   0        0        0     1082 2021-12-04 15:10:47.930598 django-entries-0.1.9/entries/static/css/starter.css
+-rw-r--r--   0        0        0     6311 2021-12-04 15:10:47.932998 django-entries-0.1.9/entries/static/img/favicons/android-chrome-192x192.png
+-rw-r--r--   0        0        0    18345 2021-12-04 15:10:47.934911 django-entries-0.1.9/entries/static/img/favicons/android-chrome-512x512.png
+-rw-r--r--   0        0        0     5734 2021-12-04 15:10:47.936200 django-entries-0.1.9/entries/static/img/favicons/apple-touch-icon.png
+-rw-r--r--   0        0        0      570 2021-12-04 15:10:47.937326 django-entries-0.1.9/entries/static/img/favicons/favicon-16x16.png
+-rw-r--r--   0        0        0     1110 2021-12-04 15:10:47.938437 django-entries-0.1.9/entries/static/img/favicons/favicon-32x32.png
+-rw-r--r--   0        0        0    15406 2021-12-04 15:10:47.939346 django-entries-0.1.9/entries/static/img/favicons/favicon.ico
+-rw-r--r--   0        0        0      264 2021-12-04 15:10:47.940024 django-entries-0.1.9/entries/static/img/favicons/site.webmanifest
+-rw-r--r--   0        0        0      582 2021-12-04 15:10:47.944629 django-entries-0.1.9/entries/templates/about.html
+-rw-r--r--   0        0        0     1393 2021-12-08 12:15:52.825166 django-entries-0.1.9/entries/templates/base.html
+-rw-r--r--   0        0        0      407 2021-12-08 12:15:52.825693 django-entries-0.1.9/entries/templates/base_template/_favicons.html
+-rw-r--r--   0        0        0      187 2021-12-08 12:15:52.825977 django-entries-0.1.9/entries/templates/base_template/_messages.html
+-rw-r--r--   0        0        0      357 2021-12-08 12:15:52.826460 django-entries-0.1.9/entries/templates/base_template/_meta.html
+-rw-r--r--   0        0        0      387 2021-12-08 12:15:52.826884 django-entries-0.1.9/entries/templates/base_template/_nav.html
+-rw-r--r--   0        0        0       47 2021-12-08 12:15:52.827504 django-entries-0.1.9/entries/templates/entries/_form.html
+-rw-r--r--   0        0        0     1055 2021-12-08 13:00:08.165147 django-entries-0.1.9/entries/templates/entries/entry_detail.html
+-rw-r--r--   0        0        0      361 2021-12-08 12:15:52.829110 django-entries-0.1.9/entries/templates/entries/entry_edit.html
+-rw-r--r--   0        0        0      192 2021-12-08 15:47:59.661183 django-entries-0.1.9/entries/templates/entries/entry_item.html
+-rw-r--r--   0        0        0      648 2021-12-08 15:52:40.911814 django-entries-0.1.9/entries/templates/entries/entry_list.html
+-rw-r--r--   0        0        0      250 2021-12-08 15:48:37.321794 django-entries-0.1.9/entries/templates/entries/entry_next.html
+-rw-r--r--   0        0        0      165 2021-12-04 15:10:47.950729 django-entries-0.1.9/entries/templates/home.html
+-rw-r--r--   0        0        0     2040 2021-12-04 15:10:47.951486 django-entries-0.1.9/entries/tests/conftest.py
+-rw-r--r--   0        0        0     1287 2021-12-08 12:15:52.836503 django-entries-0.1.9/entries/tests/test_entry_create.py
+-rw-r--r--   0        0        0     1318 2021-12-07 12:47:48.665088 django-entries-0.1.9/entries/tests/test_entry_delete.py
+-rw-r--r--   0        0        0     1866 2021-12-08 12:15:52.838816 django-entries-0.1.9/entries/tests/test_entry_edit.py
+-rw-r--r--   0        0        0      859 2021-12-07 12:47:48.669693 django-entries-0.1.9/entries/tests/test_entry_read.py
+-rw-r--r--   0        0        0     1096 2021-12-04 15:10:47.955311 django-entries-0.1.9/entries/tests/test_forms.py
+-rw-r--r--   0        0        0     1093 2021-12-08 12:15:52.841252 django-entries-0.1.9/entries/tests/test_utils.py
+-rw-r--r--   0        0        0      633 2021-12-08 12:15:52.843458 django-entries-0.1.9/entries/urls.py
+-rw-r--r--   0        0        0      607 2021-12-04 15:10:47.957758 django-entries-0.1.9/entries/utils.py
+-rw-r--r--   0        0        0      497 2021-12-04 15:10:47.958617 django-entries-0.1.9/entries/validators.py
+-rw-r--r--   0        0        0     3320 2021-12-08 15:17:00.628131 django-entries-0.1.9/entries/views.py
+-rw-r--r--   0        0        0     1431 2021-12-08 15:46:56.135381 django-entries-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     3074 2021-12-08 15:58:07.056460 django-entries-0.1.9/setup.py
+-rw-r--r--   0        0        0     2852 2021-12-08 15:58:07.056918 django-entries-0.1.9/PKG-INFO
```

### Comparing `django-entries-0.1.8/README.md` & `django-entries-0.1.9/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,20 @@
-# Entries
+# django-entries
 
 ## Overview
 
-Entries is a Django app that has basic create-read-update-delete (CRUD) functionality for an `Entry` model with `title`, `excerpt`,`content` and `author` fields. The base [template](./entries/templates/base.html) makes use of light css and javascript.
+Basic create-read-update-delete (CRUD) functionality for an `Entry` model.
 
-## CSS
+The base [template](./entries/templates/base.html) makes use of light css and javascript:
 
 1. `starter.css` [stylesheet](./entries/static/css/starter.css)
 2. `pylon` 0.1.1 for `<hstack>` and `<vstack>` layouts
-
-## JS
-
-1. `htmx` 1.6.1 for html-over-the-wire functionality
-2. `hyperscript` 0.9 for client-side reactivity
-3. `simplemde` a simple markdown editor
+3. `htmx` 1.6.1 for html-over-the-wire functionality, e.g. [infinite scrolling](./entries/docs/infinity_scroll.md)
+4. `hyperscript` 0.9 for client-side reactivity
+5. `simplemde` a simple markdown editor
 
 ## Quickstart
 
 Install in your virtual environment:
 
 ```zsh
 .venv> pip3 install django-entries # poetry add django-entries
@@ -30,19 +27,39 @@
 INSTALLED_APPS = [
     ...,
     'crispy_forms',  # add crispy_forms at least > v1.13, if not yet added
     'entries' # this is the new django-entries folder
 ]
 
 # in project_folder/urls.py
+from django.views.generic import TemplateView
 from django.urls import path, include # new
 urlpatterns = [
     ...,
     path('entry/', include('entries.urls')) # new
+    path("", TemplateView.as_view(template_name="home.html")), # (optional: if fresh project install)
 ]
 ```
 
 Add to database:
 
 ```zsh
 .venv> python manage.py migrate # adds the `Entry` model to the database.
+.venv> python manage.py createsuperuser # (optional: if fresh project install)
+```
+
+Login to add:
+
+```zsh
+.venv> `python manage.py runserver`
+# Visit http://127.0.0.1:8000/entry/entries/list
+# Assumes _entry_ as folder in config/urls.py
+# The `Add entry` button is only visible to logged in users.
+# Can login via admin using the superuser account http://127.0.0.1:8000/admin/
+# Visit the list page again at http://127.0.0.1:8000/entry/entries/list to see the `Add entry` button.
+```
+
+## Test
+
+```zsh
+.venv> pytest --ds=config.settings --cov
 ```
```

### Comparing `django-entries-0.1.8/entries/forms.py` & `django-entries-0.1.9/entries/forms.py`

 * *Files identical despite different names*

### Comparing `django-entries-0.1.8/entries/migrations/0001_initial.py` & `django-entries-0.1.9/entries/migrations/0001_initial.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,24 @@
-# Generated by Django 3.2.9 on 2021-12-04 08:37
+# Generated by Django 4.0 on 2021-12-08 15:46
 
 import uuid
 
 import django.db.models.deletion
 import django_extensions.db.fields
-from django.conf import settings
 from django.db import migrations, models
 
 import entries.validators
 
 
 class Migration(migrations.Migration):
 
     initial = True
 
     dependencies = [
-        migrations.swappable_dependency(settings.AUTH_USER_MODEL),
+        ("auth", "0012_alter_user_first_name_max_length"),
     ]
 
     operations = [
         migrations.CreateModel(
             name="Entry",
             fields=[
                 (
@@ -77,17 +76,18 @@
                     ),
                 ),
                 (
                     "author",
                     models.ForeignKey(
                         on_delete=django.db.models.deletion.CASCADE,
                         related_name="entries",
-                        to=settings.AUTH_USER_MODEL,
+                        to="auth.user",
                     ),
                 ),
             ],
             options={
                 "verbose_name": "Entry",
                 "verbose_name_plural": "Entries",
+                "ordering": ["-created"],
             },
         ),
     ]
```

### Comparing `django-entries-0.1.8/entries/models.py` & `django-entries-0.1.9/entries/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
         help_text="Markdown text formatting, e.g. ##, *, 1., -, etc."
     )
     author = models.ForeignKey(
         get_user_model(), on_delete=models.CASCADE, related_name="entries"
     )
 
     class Meta:
+        ordering = ["-created"]
         verbose_name = "Entry"
         verbose_name_plural = "Entries"
 
     def __str__(self):
         return f"{self.title} by {self.author}"
 
     def get_absolute_url(self):
```

### Comparing `django-entries-0.1.8/entries/static/css/starter.css` & `django-entries-0.1.9/entries/static/css/starter.css`

 * *Files identical despite different names*

### Comparing `django-entries-0.1.8/entries/static/img/favicons/android-chrome-192x192.png` & `django-entries-0.1.9/entries/static/img/favicons/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `django-entries-0.1.8/entries/static/img/favicons/android-chrome-512x512.png` & `django-entries-0.1.9/entries/static/img/favicons/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `django-entries-0.1.8/entries/static/img/favicons/apple-touch-icon.png` & `django-entries-0.1.9/entries/static/img/favicons/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `django-entries-0.1.8/entries/static/img/favicons/favicon-16x16.png` & `django-entries-0.1.9/entries/static/img/favicons/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `django-entries-0.1.8/entries/static/img/favicons/favicon-32x32.png` & `django-entries-0.1.9/entries/static/img/favicons/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `django-entries-0.1.8/entries/static/img/favicons/favicon.ico` & `django-entries-0.1.9/entries/static/img/favicons/favicon.ico`

 * *Files identical despite different names*

### Comparing `django-entries-0.1.8/entries/templates/about.html` & `django-entries-0.1.9/entries/templates/about.html`

 * *Files identical despite different names*

### Comparing `django-entries-0.1.8/entries/templates/entry_detail.html` & `django-entries-0.1.9/entries/templates/entries/entry_detail.html`

 * *Files 15% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 {% block title %} {{entry.title}} | BrandX {% endblock title %}
 
 {% block content %}
     <hstack spacing=s>
         <h1>{{entry.title}}</h1>
         {% if user.is_authenticated and user == entry.author %}
             <spacer></spacer>
+            <button hx-get="{% url 'entries:add_entry' %}" hx-target="body" hx-boost="true">create</button>
             <button hx-get="{% url 'entries:edit_entry' entry.slug %}" hx-target="body" hx-boost="true">edit</button>
             <button hx-delete="{% url 'entries:delete_entry' entry.slug %}" hx-confirm="Are you sure you want to delete?" hx-boost="true">delete</button>
         {% endif %}
     </hstack>
     <hstack>
         <small>By: {{entry.author}}</small>
         <small>, {{ entry.created|date }}</small>
```

### Comparing `django-entries-0.1.8/entries/tests/conftest.py` & `django-entries-0.1.9/entries/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `django-entries-0.1.8/entries/tests/test_entry_create.py` & `django-entries-0.1.9/entries/tests/test_entry_create.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from http import HTTPStatus
 
 import pytest
 from django.http.response import HttpResponseRedirect
 from django.template.response import TemplateResponse
 from django.urls import reverse
 
+from entries.views import EDITOR
+
 ENDPOINT = "/entry/create/add"
 ROUTE = reverse("entries:add_entry")
 
 
 @pytest.mark.parametrize("url", [ENDPOINT, ROUTE])
 def test_add_entry_anonymous_redirected(client, url):
     response = client.get(url)
@@ -18,15 +20,15 @@
 
 @pytest.mark.parametrize("url", [ENDPOINT, ROUTE])
 def test_add_entry_get_authenticated(client, sample_user, url):
     client.force_login(sample_user)
     response = client.get(url)
     assert isinstance(response, TemplateResponse)
     assert HTTPStatus.OK == response.status_code
-    assert "entry_edit.html" == response.template_name
+    assert EDITOR == response.template_name
 
 
 @pytest.mark.django_db
 @pytest.mark.parametrize("url", [ENDPOINT, ROUTE])
 def test_add_entry_post_authenticated(
     client, sample_data, sample_user, sample_slug, url
 ):
```

### Comparing `django-entries-0.1.8/entries/tests/test_entry_delete.py` & `django-entries-0.1.9/entries/tests/test_entry_delete.py`

 * *Files identical despite different names*

### Comparing `django-entries-0.1.8/entries/tests/test_entry_edit.py` & `django-entries-0.1.9/entries/tests/test_entry_edit.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 import pytest
 from django.core.exceptions import PermissionDenied
 from django.http.response import HttpResponseRedirect
 from django.template.response import TemplateResponse
 from django.urls import reverse
 
+from entries.views import EDITOR
+
 ENDPOINT = lambda x: f"/entry/edit/{x}"
 ROUTE = lambda x: reverse("entries:edit_entry", kwargs={"slug": x})
 
 
 @pytest.mark.parametrize("formatter", [ENDPOINT, ROUTE])
 def test_edit_entry_anonymous_redirected(client, sample_slug, formatter):
     url = formatter(sample_slug)
@@ -34,15 +36,15 @@
     client, sample_user, test_entry, formatter
 ):
     client.force_login(sample_user)
     url = formatter(test_entry.slug)
     response = client.get(url)
     assert isinstance(response, TemplateResponse)
     assert HTTPStatus.OK == response.status_code
-    assert "entry_edit.html" == response.template_name
+    assert EDITOR == response.template_name
 
 
 @pytest.mark.parametrize("formatter", [ENDPOINT, ROUTE])
 def test_edit_entry_post_authenticated(
     client, modified_data, sample_user, test_entry, formatter
 ):
     url = formatter(test_entry.slug)
```

### Comparing `django-entries-0.1.8/entries/tests/test_entry_read.py` & `django-entries-0.1.9/entries/tests/test_entry_read.py`

 * *Files identical despite different names*

### Comparing `django-entries-0.1.8/entries/tests/test_forms.py` & `django-entries-0.1.9/entries/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `django-entries-0.1.8/entries/tests/test_utils.py` & `django-entries-0.1.9/entries/tests/test_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 
 @pytest.mark.django_db
 @pytest.mark.parametrize(
     "named_route, template_name",
     [
         ("entries:view_about", "about.html"),
-        ("entries:list_entries", "entry_list.html"),
+        ("entries:list_entries", "entries/entry_list.html"),
     ],
 )
 def test_ok_entry_views(client, named_route, template_name):
     url = reverse(named_route)
     response = client.get(url)
     assert HTTPStatus.OK == response.status_code
     assert template_name == response.template_name
```

### Comparing `django-entries-0.1.8/entries/urls.py` & `django-entries-0.1.9/entries/urls.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from django.urls import path
 
 from .views import (
     add_entry,
     delete_entry,
     edit_entry,
     list_entries,
+    scroll_entries,
     view_about,
     view_entry,
 )
 
 app_name = "entries"
 urlpatterns = [
+    path("entries/scroll", scroll_entries, name="scroll_entries"),
     path("entries/list", list_entries, name="list_entries"),
     path("create/add", add_entry, name="add_entry"),
     path("edit/<slug:slug>", edit_entry, name="edit_entry"),
     path("delete/<slug:slug>", delete_entry, name="delete_entry"),
     path("view/<slug:slug>", view_entry, name="view_entry"),
     path("about/", view_about, name="view_about"),
 ]
```

### Comparing `django-entries-0.1.8/entries/utils.py` & `django-entries-0.1.9/entries/utils.py`

 * *Files identical despite different names*

### Comparing `django-entries-0.1.8/entries/views.py` & `django-entries-0.1.9/entries/views.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,76 +1,91 @@
 from django.contrib.auth.decorators import login_required
+from django.core.paginator import EmptyPage, Paginator
 from django.http.request import HttpRequest
 from django.http.response import HttpResponse
 from django.shortcuts import get_object_or_404, redirect
 from django.template.response import TemplateResponse
 from django.urls import reverse
 from django.views.decorators.http import require_http_methods
 
 from .forms import EntryForm
 from .models import Entry
 
+EDITOR = "entries/entry_edit.html"
+DETAIL = "entries/entry_detail.html"
+FIRST_PAGE = "entries/entry_list.html"
+NEXT_PAGE = "entries/entry_next.html"
+ITEM_IN_PAGE = "entries/entry_item.html"
+MAX_ITEMS_PER_PAGE = 2
+
 
 @login_required
 def edit_entry(request: HttpRequest, slug: str) -> TemplateResponse:
     entry = Entry.get_for_user(slug, request.user)
     url = reverse("entries:edit_entry", kwargs={"slug": slug})
     form = EntryForm(request.POST or None, instance=entry, submit_url=url)
-    if request.method == "POST" and form.is_valid():
-        if form.has_changed():
-            form.save()
+    if request.method == "POST":
+        if form.is_valid():
+            if form.has_changed():
+                form.save()
         return redirect(entry.get_absolute_url())
-    return TemplateResponse(
-        request,
-        "entry_edit.html",
-        {
-            "form": form,
-            "edit_header": f"Update {entry.title}",
-        },
-    )
+    context = {"form": form, "edit_header": f"Update {entry.title}"}
+    return TemplateResponse(request, EDITOR, context)
 
 
 @login_required
 def add_entry(request: HttpRequest) -> TemplateResponse:
     url = reverse("entries:add_entry")
     form = EntryForm(request.POST or None, submit_url=url)
     if request.method == "POST" and form.is_valid():
         entry = form.save(commit=False)
         entry.author = request.user
         entry.save()
         return redirect(entry.get_absolute_url())
-    return TemplateResponse(
-        request,
-        "entry_edit.html",
-        {
-            "form": form,
-            "edit_header": "Write An Entry",
-        },
-    )
+    context = {"form": form, "edit_header": "Write An Entry"}
+    return TemplateResponse(request, EDITOR, context)
 
 
 @login_required
 @require_http_methods(["DELETE"])
 def delete_entry(request: HttpRequest, slug: str) -> HttpResponse:
     url = reverse("entries:list_entries")
     entry = Entry.get_for_user(slug, request.user)
     response = HttpResponse(headers={"HX-Redirect": url})
     entry.delete()
     return response
 
 
 def view_entry(request: HttpRequest, slug: str) -> TemplateResponse:
-    return TemplateResponse(
-        request,
-        "entry_detail.html",
-        {"entry": get_object_or_404(Entry, slug=slug)},
-    )
+    context = {"entry": get_object_or_404(Entry, slug=slug)}
+    return TemplateResponse(request, DETAIL, context)
+
+
+def set_context(request: HttpRequest, loader: str) -> TemplateResponse:
+    qs = Entry.objects.all()
+    paginator = Paginator(qs, MAX_ITEMS_PER_PAGE)
+    page_number = request.GET.get("next", 1)  # get next from url, else page 1
+    page_obj = paginator.get_page(page_number)
+    context = {"page_obj": page_obj, "template_for_item": ITEM_IN_PAGE}
+
+    next_num = None
+    if page_obj.has_next:
+        try:
+            next_num = page_obj.next_page_number()
+        except EmptyPage:
+            next_num = None
+    if next_num:  # adds next page to url for infinity scrolling
+        base_route = reverse("entries:scroll_entries")
+        context["next_page_url"] = f"{base_route}?next={next_num}"
+    return TemplateResponse(request, loader, context)
 
 
 def list_entries(request: HttpRequest) -> TemplateResponse:
-    return TemplateResponse(
-        request, "entry_list.html", {"entries": Entry.objects.all()}
-    )
+    return set_context(request, FIRST_PAGE)
+
+
+def scroll_entries(request: HttpRequest) -> TemplateResponse:
+    return set_context(request, NEXT_PAGE)
 
 
 def view_about(request: HttpRequest) -> TemplateResponse:
     return TemplateResponse(request, "about.html", {})
```

### Comparing `django-entries-0.1.8/pyproject.toml` & `django-entries-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-entries"
-version = "0.1.8"
+version = "0.1.9"
 description = "Entries is a helper Django app with CRUD functions based on htmx."
 authors = ["Marcelino G. Veloso III <mars@veloso.one>"]
 readme = "README.md"
 repository = "https://github.com/justmars/django-entries"
 license = "MIT"
 packages = [
     { include = "entries" }, # because django-entries differs from entries
```

