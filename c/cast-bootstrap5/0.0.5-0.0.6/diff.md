# Comparing `tmp/cast_bootstrap5-0.0.5.tar.gz` & `tmp/cast_bootstrap5-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cast_bootstrap5-0.0.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "cast_bootstrap5-0.0.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `cast_bootstrap5-0.0.5.tar` & `cast_bootstrap5-0.0.6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     3077 2023-05-14 19:45:16.622485 cast_bootstrap5-0.0.5/.gitignore
--rw-r--r--   0        0        0     1281 2023-05-14 19:46:05.392913 cast_bootstrap5-0.0.5/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1505 2023-05-14 05:53:16.406076 cast_bootstrap5-0.0.5/LICENSE
--rw-r--r--   0        0        0     1212 2023-05-14 19:45:16.622564 cast_bootstrap5-0.0.5/README.md
--rw-r--r--   0        0        0       63 2023-05-14 19:52:16.779078 cast_bootstrap5-0.0.5/cast_bootstrap5/__init__.py
--rw-r--r--   0        0        0      104 2023-05-14 06:02:59.592444 cast_bootstrap5-0.0.5/cast_bootstrap5/apps.py
--rw-r--r--   0        0        0   194902 2023-05-14 19:45:16.623441 cast_bootstrap5-0.0.5/cast_bootstrap5/static/cast_bootstrap5/css/bootstrap5/bootstrap.min.css
--rw-r--r--   0        0        0   522640 2023-05-14 19:45:16.626769 cast_bootstrap5-0.0.5/cast_bootstrap5/static/cast_bootstrap5/css/bootstrap5/bootstrap.min.css.map
--rw-r--r--   0        0        0     6287 2023-05-14 12:11:23.910525 cast_bootstrap5-0.0.5/cast_bootstrap5/static/cast_bootstrap5/css/bootstrap5/cast.css
--rw-r--r--   0        0        0    80421 2023-05-14 19:45:16.623332 cast_bootstrap5-0.0.5/cast_bootstrap5/static/cast_bootstrap5/js/bootstrap5/bootstrap.bundle.min.js
--rw-r--r--   0        0        0   333079 2023-05-14 19:45:16.623393 cast_bootstrap5-0.0.5/cast_bootstrap5/static/cast_bootstrap5/js/bootstrap5/bootstrap.bundle.min.js.map
--rw-r--r--   0        0        0    42820 2023-05-14 19:45:16.626371 cast_bootstrap5-0.0.5/cast_bootstrap5/static/cast_bootstrap5/js/htmx.min.js
--rw-r--r--   0        0        0    87462 1991-10-18 12:00:00.000000 cast_bootstrap5-0.0.5/cast_bootstrap5/static/cast_bootstrap5/js/jquery/jquery-3.7.0.min.js
--rw-r--r--   0        0        0      196 2023-05-14 05:59:16.067158 cast_bootstrap5-0.0.5/cast_bootstrap5/templates/cast/bootstrap5/400.html
--rw-r--r--   0        0        0      184 2023-05-14 05:59:16.067612 cast_bootstrap5-0.0.5/cast_bootstrap5/templates/cast/bootstrap5/403.html
--rw-r--r--   0        0        0      200 2023-05-14 05:59:16.068027 cast_bootstrap5-0.0.5/cast_bootstrap5/templates/cast/bootstrap5/403_csrf.html
--rw-r--r--   0        0        0      198 2023-05-14 05:59:16.068410 cast_bootstrap5-0.0.5/cast_bootstrap5/templates/cast/bootstrap5/404.html
--rw-r--r--   0        0        0      319 2023-05-14 05:59:16.068832 cast_bootstrap5-0.0.5/cast_bootstrap5/templates/cast/bootstrap5/500.html
--rw-r--r--   0        0        0      748 2023-05-14 05:59:16.069442 cast_bootstrap5-0.0.5/cast_bootstrap5/templates/cast/bootstrap5/_list_of_posts_and_paging_controls.html
--rw-r--r--   0        0        0     2859 2023-05-14 19:45:17.514619 cast_bootstrap5-0.0.5/cast_bootstrap5/templates/cast/bootstrap5/base.html
--rw-r--r--   0        0        0     2984 2023-05-14 06:54:16.139088 cast_bootstrap5-0.0.5/cast_bootstrap5/templates/cast/bootstrap5/blog_list_of_posts.html
--rw-r--r--   0        0        0      213 2023-05-14 05:59:16.070689 cast_bootstrap5-0.0.5/cast_bootstrap5/templates/cast/bootstrap5/episode.html
--rw-r--r--   0        0        0     2367 2023-05-14 05:59:16.071108 cast_bootstrap5-0.0.5/cast_bootstrap5/templates/cast/bootstrap5/pagination.html
--rw-r--r--   0        0        0     2092 2023-05-14 05:59:16.071518 cast_bootstrap5-0.0.5/cast_bootstrap5/templates/cast/bootstrap5/post.html
--rw-r--r--   0        0        0      573 2023-05-14 05:59:16.071911 cast_bootstrap5-0.0.5/cast_bootstrap5/templates/cast/bootstrap5/post_body.html
--rw-r--r--   0        0        0     1476 2023-05-14 19:45:17.519283 cast_bootstrap5-0.0.5/cast_bootstrap5/templates/cast/gallery.html
--rw-r--r--   0        0        0     2146 2023-05-14 07:08:10.337131 cast_bootstrap5-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1929 1970-01-01 00:00:00.000000 cast_bootstrap5-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     3077 2023-05-14 19:45:16.622485 cast_bootstrap5-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1281 2023-05-14 19:46:05.392913 cast_bootstrap5-0.0.6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1505 2023-05-14 05:53:16.406076 cast_bootstrap5-0.0.6/LICENSE
+-rw-r--r--   0        0        0     1212 2023-05-14 19:45:16.622564 cast_bootstrap5-0.0.6/README.md
+-rw-r--r--   0        0        0       63 2023-05-16 20:49:48.875929 cast_bootstrap5-0.0.6/cast_bootstrap5/__init__.py
+-rw-r--r--   0        0        0      104 2023-05-14 06:02:59.592444 cast_bootstrap5-0.0.6/cast_bootstrap5/apps.py
+-rw-r--r--   0        0        0   194902 2023-05-14 19:45:16.623441 cast_bootstrap5-0.0.6/cast_bootstrap5/static/cast_bootstrap5/css/bootstrap5/bootstrap.min.css
+-rw-r--r--   0        0        0   522640 2023-05-14 19:45:16.626769 cast_bootstrap5-0.0.6/cast_bootstrap5/static/cast_bootstrap5/css/bootstrap5/bootstrap.min.css.map
+-rw-r--r--   0        0        0     6287 2023-05-14 12:11:23.910525 cast_bootstrap5-0.0.6/cast_bootstrap5/static/cast_bootstrap5/css/bootstrap5/cast.css
+-rw-r--r--   0        0        0    80421 2023-05-14 19:45:16.623332 cast_bootstrap5-0.0.6/cast_bootstrap5/static/cast_bootstrap5/js/bootstrap5/bootstrap.bundle.min.js
+-rw-r--r--   0        0        0   333079 2023-05-14 19:45:16.623393 cast_bootstrap5-0.0.6/cast_bootstrap5/static/cast_bootstrap5/js/bootstrap5/bootstrap.bundle.min.js.map
+-rw-r--r--   0        0        0    42820 2023-05-14 19:45:16.626371 cast_bootstrap5-0.0.6/cast_bootstrap5/static/cast_bootstrap5/js/htmx.min.js
+-rw-r--r--   0        0        0    87462 1991-10-18 12:00:00.000000 cast_bootstrap5-0.0.6/cast_bootstrap5/static/cast_bootstrap5/js/jquery/jquery-3.7.0.min.js
+-rw-r--r--   0        0        0      196 2023-05-14 05:59:16.067158 cast_bootstrap5-0.0.6/cast_bootstrap5/templates/cast/bootstrap5/400.html
+-rw-r--r--   0        0        0      184 2023-05-14 05:59:16.067612 cast_bootstrap5-0.0.6/cast_bootstrap5/templates/cast/bootstrap5/403.html
+-rw-r--r--   0        0        0      200 2023-05-14 05:59:16.068027 cast_bootstrap5-0.0.6/cast_bootstrap5/templates/cast/bootstrap5/403_csrf.html
+-rw-r--r--   0        0        0      198 2023-05-14 05:59:16.068410 cast_bootstrap5-0.0.6/cast_bootstrap5/templates/cast/bootstrap5/404.html
+-rw-r--r--   0        0        0      319 2023-05-14 05:59:16.068832 cast_bootstrap5-0.0.6/cast_bootstrap5/templates/cast/bootstrap5/500.html
+-rw-r--r--   0        0        0      748 2023-05-14 05:59:16.069442 cast_bootstrap5-0.0.6/cast_bootstrap5/templates/cast/bootstrap5/_list_of_posts_and_paging_controls.html
+-rw-r--r--   0        0        0     2859 2023-05-14 19:45:17.514619 cast_bootstrap5-0.0.6/cast_bootstrap5/templates/cast/bootstrap5/base.html
+-rw-r--r--   0        0        0     2984 2023-05-14 06:54:16.139088 cast_bootstrap5-0.0.6/cast_bootstrap5/templates/cast/bootstrap5/blog_list_of_posts.html
+-rw-r--r--   0        0        0      213 2023-05-14 05:59:16.070689 cast_bootstrap5-0.0.6/cast_bootstrap5/templates/cast/bootstrap5/episode.html
+-rw-r--r--   0        0        0     2367 2023-05-14 05:59:16.071108 cast_bootstrap5-0.0.6/cast_bootstrap5/templates/cast/bootstrap5/pagination.html
+-rw-r--r--   0        0        0     2092 2023-05-14 05:59:16.071518 cast_bootstrap5-0.0.6/cast_bootstrap5/templates/cast/bootstrap5/post.html
+-rw-r--r--   0        0        0      573 2023-05-14 05:59:16.071911 cast_bootstrap5-0.0.6/cast_bootstrap5/templates/cast/bootstrap5/post_body.html
+-rw-r--r--   0        0        0     1431 2023-05-16 20:47:59.028895 cast_bootstrap5-0.0.6/cast_bootstrap5/templates/cast/gallery.html
+-rw-r--r--   0        0        0     2146 2023-05-14 07:08:10.337131 cast_bootstrap5-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1929 1970-01-01 00:00:00.000000 cast_bootstrap5-0.0.6/PKG-INFO
```

### Comparing `cast_bootstrap5-0.0.5/.gitignore` & `cast_bootstrap5-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `cast_bootstrap5-0.0.5/.pre-commit-config.yaml` & `cast_bootstrap5-0.0.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `cast_bootstrap5-0.0.5/LICENSE` & `cast_bootstrap5-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cast_bootstrap5-0.0.5/README.md` & `cast_bootstrap5-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `cast_bootstrap5-0.0.5/cast_bootstrap5/static/cast_bootstrap5/css/bootstrap5/bootstrap.min.css` & `cast_bootstrap5-0.0.6/cast_bootstrap5/static/cast_bootstrap5/css/bootstrap5/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `cast_bootstrap5-0.0.5/cast_bootstrap5/static/cast_bootstrap5/css/bootstrap5/bootstrap.min.css.map` & `cast_bootstrap5-0.0.6/cast_bootstrap5/static/cast_bootstrap5/css/bootstrap5/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `cast_bootstrap5-0.0.5/cast_bootstrap5/static/cast_bootstrap5/css/bootstrap5/cast.css` & `cast_bootstrap5-0.0.6/cast_bootstrap5/static/cast_bootstrap5/css/bootstrap5/cast.css`

 * *Files identical despite different names*

### Comparing `cast_bootstrap5-0.0.5/cast_bootstrap5/static/cast_bootstrap5/js/bootstrap5/bootstrap.bundle.min.js` & `cast_bootstrap5-0.0.6/cast_bootstrap5/static/cast_bootstrap5/js/bootstrap5/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `cast_bootstrap5-0.0.5/cast_bootstrap5/static/cast_bootstrap5/js/bootstrap5/bootstrap.bundle.min.js.map` & `cast_bootstrap5-0.0.6/cast_bootstrap5/static/cast_bootstrap5/js/bootstrap5/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `cast_bootstrap5-0.0.5/cast_bootstrap5/static/cast_bootstrap5/js/htmx.min.js` & `cast_bootstrap5-0.0.6/cast_bootstrap5/static/cast_bootstrap5/js/htmx.min.js`

 * *Files identical despite different names*

### Comparing `cast_bootstrap5-0.0.5/cast_bootstrap5/static/cast_bootstrap5/js/jquery/jquery-3.7.0.min.js` & `cast_bootstrap5-0.0.6/cast_bootstrap5/static/cast_bootstrap5/js/jquery/jquery-3.7.0.min.js`

 * *Files identical despite different names*

### Comparing `cast_bootstrap5-0.0.5/cast_bootstrap5/templates/cast/bootstrap5/_list_of_posts_and_paging_controls.html` & `cast_bootstrap5-0.0.6/cast_bootstrap5/templates/cast/bootstrap5/_list_of_posts_and_paging_controls.html`

 * *Files identical despite different names*

### Comparing `cast_bootstrap5-0.0.5/cast_bootstrap5/templates/cast/bootstrap5/base.html` & `cast_bootstrap5-0.0.6/cast_bootstrap5/templates/cast/bootstrap5/base.html`

 * *Files identical despite different names*

### Comparing `cast_bootstrap5-0.0.5/cast_bootstrap5/templates/cast/bootstrap5/blog_list_of_posts.html` & `cast_bootstrap5-0.0.6/cast_bootstrap5/templates/cast/bootstrap5/blog_list_of_posts.html`

 * *Files identical despite different names*

### Comparing `cast_bootstrap5-0.0.5/cast_bootstrap5/templates/cast/bootstrap5/pagination.html` & `cast_bootstrap5-0.0.6/cast_bootstrap5/templates/cast/bootstrap5/pagination.html`

 * *Files identical despite different names*

### Comparing `cast_bootstrap5-0.0.5/cast_bootstrap5/templates/cast/bootstrap5/post.html` & `cast_bootstrap5-0.0.6/cast_bootstrap5/templates/cast/bootstrap5/post.html`

 * *Files identical despite different names*

### Comparing `cast_bootstrap5-0.0.5/cast_bootstrap5/templates/cast/bootstrap5/post_body.html` & `cast_bootstrap5-0.0.6/cast_bootstrap5/templates/cast/bootstrap5/post_body.html`

 * *Files identical despite different names*

### Comparing `cast_bootstrap5-0.0.5/cast_bootstrap5/templates/cast/gallery.html` & `cast_bootstrap5-0.0.6/cast_bootstrap5/templates/cast/gallery.html`

 * *Files 6% similar despite different names*

```diff
@@ -25,16 +25,15 @@
   {% endfor %}
   <!-- Modal -->
   <div class="modal fade" id="galleryModal-{{ block.id }}" tabindex="-1" role="dialog"
        aria-labelledby="galleryModalLabel" aria-hidden="true">
     <div class="modal-dialog modal-lg cast-gallery-lg" role="document">
       <div class="modal-content cast-gallery-content">
         <div class="modal-header cast-gallery-header">
-          <button type="button" class="close" data-dismiss="modal" aria-label="Close">
-            <span aria-hidden="true">&times;</span>
+          <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close">
           </button>
         </div>
         <div class="modal-body cast-gallery-body">
           <a><img class="modal-image cast-image" src="" srcset="" sizes="100vw"></img></a>
         </div>
         <div class="modal-footer cast-gallery-footer">
         </div>
```

### Comparing `cast_bootstrap5-0.0.5/pyproject.toml` & `cast_bootstrap5-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cast_bootstrap5-0.0.5/PKG-INFO` & `cast_bootstrap5-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cast-bootstrap5
-Version: 0.0.5
+Version: 0.0.6
 Summary: Bootstrap5 theme for django-cast
 Keywords: blog,podcast,video,audio
 Author-email: Jochen Wersdörfer <jochen-castbootstrap5@wersdoerfer.de>
 Requires-Python: >=3.9
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.0
```

