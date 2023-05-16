# Comparing `tmp/stmaterial-0.0.6.tar.gz` & `tmp/stmaterial-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stmaterial-0.0.6.tar", last modified: Sun May 14 03:21:24 2023, max compression
+gzip compressed data, was "stmaterial-0.0.7.tar", last modified: Tue May 16 14:59:27 2023, max compression
```

## Comparing `stmaterial-0.0.6.tar` & `stmaterial-0.0.7.tar`

### file list

```diff
@@ -1,216 +1,208 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 03:21:24.695963 stmaterial-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-14 03:21:07.611593 stmaterial-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-14 03:21:07.611593 stmaterial-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-05-14 03:21:07.611593 stmaterial-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 03:21:07.615594 stmaterial-0.0.6/docs/_images/
--rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-05-14 03:21:07.611593 stmaterial-0.0.6/docs/_images/a.png
--rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-05-14 03:21:07.611593 stmaterial-0.0.6/docs/_images/b.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 03:21:07.611593 stmaterial-0.0.6/docs/_images/books/
--rw-r--r--   0 runner    (1001) docker     (123)    20978 2023-05-14 03:21:07.611593 stmaterial-0.0.6/docs/_images/books/benders分解.png
--rw-r--r--   0 runner    (1001) docker     (123)   394770 2023-05-14 03:21:07.615594 stmaterial-0.0.6/docs/_images/books/内点法.png
--rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-05-14 03:21:07.615594 stmaterial-0.0.6/docs/_images/c.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 03:21:07.615594 stmaterial-0.0.6/docs/_images/links/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 03:21:07.615594 stmaterial-0.0.6/docs/_images/links/gallery/
--rw-r--r--   0 runner    (1001) docker     (123)   164525 2023-05-14 03:21:07.615594 stmaterial-0.0.6/docs/_images/links/gallery/jupyter_book.png
--rw-r--r--   0 runner    (1001) docker     (123)    93132 2023-05-14 03:21:07.615594 stmaterial-0.0.6/docs/_images/links/gallery/matplotlib.png
--rw-r--r--   0 runner    (1001) docker     (123)   112977 2023-05-14 03:21:07.615594 stmaterial-0.0.6/docs/_images/links/gallery/pandas.png
--rw-r--r--   0 runner    (1001) docker     (123)   204727 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/_images/links/gallery/sphinx_design.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    21234 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/_static/favicon.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/_static/links/
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/_static/links/gallery.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/_static/logo-.png
--rw-r--r--   0 runner    (1001) docker     (123)    24875 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/_static/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/blog.md
--rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/develop.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/examples/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/examples/kitchen-sink/
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/examples/kitchen-sink/admonitions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/examples/kitchen-sink/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8119 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/examples/kitchen-sink/blocks.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8978 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/examples/kitchen-sink/generic.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/examples/kitchen-sink/images.rst
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/examples/kitchen-sink/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     6186 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/examples/kitchen-sink/lists.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12894 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/examples/kitchen-sink/really-long.md
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/examples/kitchen-sink/sphinx-design.md
--rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/examples/kitchen-sink/structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/examples/kitchen-sink/tables.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/examples/kitchen-sink/typography.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/examples/reference/
--rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/examples/reference/admonitions.md
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/examples/reference/api.md
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/examples/reference/code-blocks.md
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/examples/reference/hyperlinks.md
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/examples/reference/images.md
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/examples/reference/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/examples/reference/lists.md
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/examples/reference/tables.md
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/examples/reference/tabs.md
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/examples/reference/text-formatting.md
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/posts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/posts/plangs/
--rw-r--r--   0 runner    (1001) docker     (123)    11385 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/posts/plangs/2021-python-pathlib.md
--rw-r--r--   0 runner    (1001) docker     (123)    13248 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/posts/plangs/2022-pytest-tutorial.md
--rw-r--r--   0 runner    (1001) docker     (123)    20426 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/posts/plangs/2022-python-setup.md
--rw-r--r--   0 runner    (1001) docker     (123)    19012 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/posts/plangs/2022-python-typing.md
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/user_guide/
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/user_guide/header.md
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/user_guide/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/user_guide/sidenav.md
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/user_guide/source-buttons.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/user_guide_tmp/
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/user_guide_tmp/edit-button.md
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/user_guide_tmp/fonts.md
--rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/user_guide_tmp/header.md
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/user_guide_tmp/index1.md
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/user_guide_tmp/landing-page.md
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/user_guide_tmp/logo.md
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/user_guide_tmp/sidebar-title.md
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/user_guide_tmp/sidebar.md
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/user_guide_tmp/toc.md
--rw-r--r--   0 runner    (1001) docker     (123)     5422 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/web-components.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-05-14 03:21:07.619594 stmaterial-0.0.6/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (123)   220389 2023-05-14 03:21:07.619594 stmaterial-0.0.6/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-14 03:21:07.619594 stmaterial-0.0.6/package.json
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-14 03:21:07.619594 stmaterial-0.0.6/postcss.config.js
--rwxr-xr-x   0 runner    (1001) docker     (123)     1507 2023-05-14 03:21:07.619594 stmaterial-0.0.6/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 03:21:07.619594 stmaterial-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/
--rw-r--r--   0 runner    (1001) docker     (123)    12341 2023-05-14 03:21:07.619594 stmaterial-0.0.6/src/stmaterial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17633 2023-05-14 03:21:07.619594 stmaterial-0.0.6/src/stmaterial/_navigation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5390 2023-05-14 03:21:07.619594 stmaterial-0.0.6/src/stmaterial/_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/_translations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)    12991 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/scripts/gumshoe-patched.js
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/scripts/materialize.js
--rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/scripts/stmaterial.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/base/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/base/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/base/_theme.sass
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/base/_typography.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/components/
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/components/_article-metadata-info.scss
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/components/_back-to-top.scss
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/components/_brand-logo.scss
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/components/_breadcrumb.sass
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/components/_dropdown.scss
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/components/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/components/_prev-next.scss
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/components/_scrollbar.scss
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/components/_search-field.sass
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/components/_search.sass
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/components/_searchbox.scss
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/components/_sidenav-icons.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/components/_table-of-contents.sass
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/content/
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/content/_admonitions.sass
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/content/_api.sass
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/content/_blocks.sass
--rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/content/_code.sass
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/content/_footnotes.sass
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/content/_gui-labels.sass
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/content/_images.sass
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/content/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/content/_indexes.sass
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/content/_lists.sass
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/content/_math.sass
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/content/_misc.sass
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/content/_rubrics.sass
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/content/_sidebar.sass
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/content/_spans.scss
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/content/_tables.sass
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/content/_target.sass
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/extensions/_ablog.scss
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/extensions/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/extensions/_myst-nb.scss
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/extensions/_timeline.scss
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/extensions/_tippy.sass
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/extensions/_togglebutton.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/patch/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/patch/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/patch/_legacy.sass
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/patch/_patch.scss
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/patch/_test.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/sections/
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/sections/_article.sass
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/sections/_footer.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/sections/_headnav.scss
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/sections/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/sections/_sidebar-toggle.scss
--rw-r--r--   0 runner    (1001) docker     (123)     3715 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/sections/_stm-sidenav.scss
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/stmaterial.sass
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/variables/
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/variables/_admonitions.scss
--rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/variables/_colors.scss
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/variables/_fonts.scss
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/variables/_icons.scss
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/variables/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/variables/_layout.scss
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/variables/_spacing.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/translations/
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/translations/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/translations/jsons/
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/translations/jsons/Back to top.json
--rw-r--r--   0 runner    (1001) docker     (123)     5371 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/translations/jsons/Edit this page.json
--rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/translations/jsons/On this page.json
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/translations/jsons/stmaterial theme.json
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/translations/jsons/with.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/demo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/demo/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/demo/sphinxext.py
--rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/directives.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/theme/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/theme/stmaterial/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3418 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/theme/stmaterial/base.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/theme/stmaterial/components/
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/theme/stmaterial/components/back-to-top.html
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/theme/stmaterial/components/brand-logo.html
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/theme/stmaterial/components/breadcrumbs.html
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/theme/stmaterial/components/copyright.html
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/theme/stmaterial/components/edit-this-page.html
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/theme/stmaterial/components/headnav-items.html
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/theme/stmaterial/components/last-updated.html
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/theme/stmaterial/components/license.html
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/theme/stmaterial/components/postnav.html
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/theme/stmaterial/components/prev-next.html
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/theme/stmaterial/components/search-button.html
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/theme/stmaterial/components/search-field.html
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/theme/stmaterial/components/search-wrapper.html
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/theme/stmaterial/components/searchbox.html
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/theme/stmaterial/components/sidenav-nav.html
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/theme/stmaterial/components/sourcelink.html
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/theme/stmaterial/components/sphinx-version.html
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/theme/stmaterial/domainindex.html
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/theme/stmaterial/genindex.html
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/theme/stmaterial/globaltoc.html
--rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/theme/stmaterial/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/theme/stmaterial/localtoc.html
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/theme/stmaterial/page.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/theme/stmaterial/partials/
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/theme/stmaterial/partials/_head_css_variables.html
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/theme/stmaterial/partials/_icon_links_declaration.html
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/theme/stmaterial/search.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/theme/stmaterial/sections/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/theme/stmaterial/sections/footer.html
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/theme/stmaterial/sections/headnav.html
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/theme/stmaterial/sections/sidenav.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/theme/stmaterial/static/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/theme/stmaterial/static/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/theme/stmaterial/static/images/
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/theme/stmaterial/static/images/github.svg
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/theme/stmaterial/theme.conf
--rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 03:21:07.623594 stmaterial-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 03:21:07.623594 stmaterial-0.0.6/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-05-14 03:21:07.623594 stmaterial-0.0.6/webpack.config.js
--rw-r--r--   0        0        0     4163 1970-01-01 00:00:00.000000 stmaterial-0.0.6/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:59:27.742927 stmaterial-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-16 14:59:01.190998 stmaterial-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-16 14:59:01.190998 stmaterial-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-05-16 14:59:01.190998 stmaterial-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:59:01.194998 stmaterial-0.0.7/docs/_images/
+-rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-05-16 14:59:01.190998 stmaterial-0.0.7/docs/_images/a.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-05-16 14:59:01.190998 stmaterial-0.0.7/docs/_images/b.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:59:01.190998 stmaterial-0.0.7/docs/_images/books/
+-rw-r--r--   0 runner    (1001) docker     (123)    20978 2023-05-16 14:59:01.190998 stmaterial-0.0.7/docs/_images/books/benders分解.png
+-rw-r--r--   0 runner    (1001) docker     (123)   394770 2023-05-16 14:59:01.194998 stmaterial-0.0.7/docs/_images/books/内点法.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-05-16 14:59:01.194998 stmaterial-0.0.7/docs/_images/c.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:59:01.194998 stmaterial-0.0.7/docs/_images/links/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:59:01.194998 stmaterial-0.0.7/docs/_images/links/gallery/
+-rw-r--r--   0 runner    (1001) docker     (123)   164525 2023-05-16 14:59:01.194998 stmaterial-0.0.7/docs/_images/links/gallery/jupyter_book.png
+-rw-r--r--   0 runner    (1001) docker     (123)    93132 2023-05-16 14:59:01.194998 stmaterial-0.0.7/docs/_images/links/gallery/matplotlib.png
+-rw-r--r--   0 runner    (1001) docker     (123)   112977 2023-05-16 14:59:01.194998 stmaterial-0.0.7/docs/_images/links/gallery/pandas.png
+-rw-r--r--   0 runner    (1001) docker     (123)   204727 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/_images/links/gallery/sphinx_design.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    21234 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/_static/favicon.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/_static/links/
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/_static/links/gallery.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/_static/logo-.png
+-rw-r--r--   0 runner    (1001) docker     (123)    24875 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/_static/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/blog.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5249 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/develop.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/examples/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/examples/kitchen-sink/
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/examples/kitchen-sink/admonitions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/examples/kitchen-sink/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8119 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/examples/kitchen-sink/blocks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8978 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/examples/kitchen-sink/generic.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/examples/kitchen-sink/images.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/examples/kitchen-sink/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6186 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/examples/kitchen-sink/lists.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12894 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/examples/kitchen-sink/really-long.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/examples/kitchen-sink/sphinx-design.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/examples/kitchen-sink/structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/examples/kitchen-sink/tables.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/examples/kitchen-sink/typography.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/examples/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/examples/reference/admonitions.md
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/examples/reference/api.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/examples/reference/code-blocks.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/examples/reference/hyperlinks.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/examples/reference/images.md
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/examples/reference/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/examples/reference/lists.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/examples/reference/tables.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/examples/reference/tabs.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/examples/reference/text-formatting.md
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/posts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/posts/plangs/
+-rw-r--r--   0 runner    (1001) docker     (123)    11303 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/posts/plangs/2021-python-pathlib.md
+-rw-r--r--   0 runner    (1001) docker     (123)    20375 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/posts/plangs/2022-python-setup.md
+-rw-r--r--   0 runner    (1001) docker     (123)    18997 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/posts/plangs/2022-python-typing.md
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/user_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/user_guide/header.md
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/user_guide/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/user_guide/sidenav.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/user_guide/source-buttons.md
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/user_guide/variables.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/web-components.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-05-16 14:59:01.198998 stmaterial-0.0.7/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)   220389 2023-05-16 14:59:01.198998 stmaterial-0.0.7/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-16 14:59:01.198998 stmaterial-0.0.7/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-16 14:59:01.198998 stmaterial-0.0.7/postcss.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-05-16 14:59:01.198998 stmaterial-0.0.7/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:59:01.198998 stmaterial-0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/
+-rw-r--r--   0 runner    (1001) docker     (123)    12460 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17690 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/_navigation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5357 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/_translations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)    12991 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/scripts/gumshoe-patched.js
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/scripts/materialize.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9734 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/scripts/stmaterial.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/base/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/base/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/base/_theme.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/base/_typography.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/components/_article-bottom.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/components/_article-top.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/components/_back-to-top.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/components/_brand-logo.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/components/_breadcrumb.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/components/_dropdown.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/components/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/components/_prev-next.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/components/_scrollbar.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/components/_search-field.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/components/_search.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/components/_searchbox.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/components/_sidenav-icons.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/components/_table-of-contents.sass
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/content/
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/content/_admonitions.sass
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/content/_api.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/content/_blocks.sass
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/content/_code.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/content/_footnotes.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/content/_gui-labels.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/content/_images.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/content/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/content/_indexes.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/content/_lists.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/content/_math.sass
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/content/_misc.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/content/_rubrics.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/content/_sidebar.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/content/_spans.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/content/_tables.sass
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/content/_target.sass
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/extensions/_ablog.scss
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/extensions/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/extensions/_myst-nb.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/extensions/_timeline.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/extensions/_tippy.sass
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/extensions/_togglebutton.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/patch/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/patch/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/patch/_patch.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/patch/_test.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/sections/
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/sections/_article.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/sections/_footer.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/sections/_headnav.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/sections/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/sections/_sidebar-toggle.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     3801 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/sections/_stm-sidenav.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/stmaterial.sass
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/variables/_admonitions.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     5711 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/variables/_colors.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/variables/_fonts.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/variables/_icons.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/variables/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/variables/_layout.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/variables/_spacing.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/translations/
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/translations/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/translations/jsons/
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/translations/jsons/Back to top.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/translations/jsons/Edit this page.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/translations/jsons/On this page.json
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/translations/jsons/stmaterial theme.json
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/translations/jsons/with.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/demo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/demo/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/demo/sphinxext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/directives.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/theme/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/theme/stmaterial/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3567 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/theme/stmaterial/base.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/theme/stmaterial/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/theme/stmaterial/components/back-to-top.html
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/theme/stmaterial/components/brand-logo.html
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/theme/stmaterial/components/breadcrumbs.html
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/theme/stmaterial/components/copyright.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/theme/stmaterial/components/edit-this-page.html
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/theme/stmaterial/components/headnav-items.html
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/theme/stmaterial/components/last-updated.html
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/theme/stmaterial/components/license.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/theme/stmaterial/components/postnav.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/theme/stmaterial/components/prev-next.html
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/theme/stmaterial/components/search-button.html
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/theme/stmaterial/components/search-field.html
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/theme/stmaterial/components/search-wrapper.html
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/theme/stmaterial/components/searchbox.html
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/theme/stmaterial/components/sidenav-nav.html
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/theme/stmaterial/components/sourcelink.html
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/theme/stmaterial/components/sphinx-version.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/theme/stmaterial/domainindex.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/theme/stmaterial/genindex.html
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/theme/stmaterial/globaltoc.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/theme/stmaterial/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/theme/stmaterial/localtoc.html
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/theme/stmaterial/page.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/theme/stmaterial/partials/
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/theme/stmaterial/partials/_head_css_variables.html
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/theme/stmaterial/partials/_icon_links_declaration.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/theme/stmaterial/search.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/theme/stmaterial/sections/
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/theme/stmaterial/sections/article-bottom.html
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/theme/stmaterial/sections/article-top.html
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/theme/stmaterial/sections/footer.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/theme/stmaterial/sections/headnav.html
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/theme/stmaterial/sections/sidenav.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/theme/stmaterial/static/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/theme/stmaterial/static/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/theme/stmaterial/static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/theme/stmaterial/static/images/github.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/theme/stmaterial/theme.conf
+-rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:59:01.202998 stmaterial-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 14:59:01.202998 stmaterial-0.0.7/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-05-16 14:59:01.202998 stmaterial-0.0.7/webpack.config.js
+-rw-r--r--   0        0        0     4153 1970-01-01 00:00:00.000000 stmaterial-0.0.7/PKG-INFO
```

### Comparing `stmaterial-0.0.6/LICENSE` & `stmaterial-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.6/README.md` & `stmaterial-0.0.7/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 <h1 align="center">
   <img src="https://cdn.jsdelivr.net/gh/zclab/stmaterial/docs/_static/logo.png" width="400">
 </h1>
 
 <p align="center">
   <strong>
-    A 
+    A
     <a href="https://materializeweb.com/">Materialize</a> based <a href="https://www.sphinx-doc.org/en/master/">sphinx</a> theme.
   </strong>
 </p>
 
 <!-- [![deploy](https://github.com/zclab/stmaterial/actions/workflows/deploy-docs.yml/badge.svg)](https://zclab.github.io/stmaterial/) -->
+
 [![deploy](https://img.shields.io/readthedocs/stmaterial?style=flat-square&logo=readthedocs&logoColor=white)](https://stmaterial.readthedocs.io/en/latest/)
 [![Downloads](https://img.shields.io/pypi/dm/stmaterial.svg?style=flat-square)](https://pypistats.org/packages/stmaterial)
 [![python](https://img.shields.io/pypi/pyversions/stmaterial.svg?style=flat-square)](https://pypi.org/project/stmaterial/)
 [![PyPI](https://img.shields.io/pypi/v/stmaterial?style=flat-square&logo=python&logoColor=white&color=orange)](https://pypi.org/project/stmaterial/)
 [![status](https://img.shields.io/pypi/status/stmaterial.svg?style=flat-square)](https://pypi.org/project/stmaterial/)
 [![license](https://img.shields.io/pypi/l/stmaterial.svg?style=flat-square&logo=opensourceinitiative&logoColor=white)](https://github.com/zclab/stmaterial/blob/main/LICENSE)
 
-
 ## Installation and usage
 
 <!-- start quickstart -->
 
 To use this theme in the repository, follow these steps:
 
 1. Install the `stmaterial` in your doc build environment:
-   
-    ```
-    pip install stmaterial
-    ```
+
+   ```
+   pip install stmaterial
+   ```
 
 2. Configure the Sphinx docs to use the theme by editing `conf.py`
 
-    ```python
-    html_theme = "stmaterial"
-    ```
+   ```python
+   html_theme = "stmaterial"
+   ```
 
 3. Your Sphinx documentation's HTML pages will now be generated with this theme! 🎉
 
 <!-- end quickstart -->
```

### Comparing `stmaterial-0.0.6/docs/_images/a.png` & `stmaterial-0.0.7/docs/_images/a.png`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.6/docs/_images/b.png` & `stmaterial-0.0.7/docs/_images/b.png`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.6/docs/_images/books/benders分解.png` & `stmaterial-0.0.7/docs/_images/books/benders分解.png`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.6/docs/_images/books/内点法.png` & `stmaterial-0.0.7/docs/_images/books/内点法.png`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.6/docs/_images/c.png` & `stmaterial-0.0.7/docs/_images/c.png`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.6/docs/_images/links/gallery/jupyter_book.png` & `stmaterial-0.0.7/docs/_images/links/gallery/jupyter_book.png`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.6/docs/_images/links/gallery/matplotlib.png` & `stmaterial-0.0.7/docs/_images/links/gallery/matplotlib.png`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.6/docs/_images/links/gallery/pandas.png` & `stmaterial-0.0.7/docs/_images/links/gallery/pandas.png`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.6/docs/_images/links/gallery/sphinx_design.png` & `stmaterial-0.0.7/docs/_images/links/gallery/sphinx_design.png`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.6/docs/_static/favicon.png` & `stmaterial-0.0.7/docs/_static/favicon.png`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.6/docs/_static/links/gallery.yaml` & `stmaterial-0.0.7/docs/_static/links/gallery.yaml`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 - title: Sphinx Design
   website: https://sphinx-design.readthedocs.io/
   img-bottom: /_images/links/gallery/sphinx_design.png
   link: https://sphinx-design.readthedocs.io/
 - title: Jupyter Book
   website: https://jupyterbook.org/en/stable/intro.html
   img-bottom: /_images/links/gallery/jupyter_book.png
-  link: https://jupyterbook.org/en/stable/intro.html
+  link: https://jupyterbook.org/en/stable/intro.html
```

### Comparing `stmaterial-0.0.6/docs/_static/logo-.png` & `stmaterial-0.0.7/docs/_static/logo-.png`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.6/docs/_static/logo.png` & `stmaterial-0.0.7/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.6/docs/conf.py` & `stmaterial-0.0.7/docs/conf.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import sys
 from os.path import abspath, join, dirname
-sys.path.insert(0, abspath(join(dirname(__file__), "../src")))
 import stmaterial
 
+sys.path.insert(0, abspath(join(dirname(__file__), "../src")))
 
 project = "sphinx theme of material"
 copyright = "2023"
 author = "zclab"
 master_doc = "index"
 version = stmaterial.__version__
-language = 'en' #'zh_CN'
+language = "en"  #'zh_CN'
 
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.extlinks",
     "sphinx.ext.intersphinx",
     "sphinx.ext.todo",
     "sphinx.ext.viewcode",
@@ -26,19 +26,19 @@
     "sphinx_togglebutton",
     "sphinx_subfigure",
 ]
 
 
 myst_enable_extensions = ["colon_fence", "deflist"]
 exclude_patterns = [
-    "_build", 
-    "Thumbs.db", 
+    "_build",
+    "Thumbs.db",
     ".DS_Store",
     "contributing",
-    "user_guide_tmp/*"
+    "user_guide_tmp/*",
 ]
 
 intersphinx_mapping = {
     "python": ("https://docs.python.org/3.9", None),
     "sphinx": ("https://www.sphinx-doc.org/en/master", None),
     "markdown_it": ("https://markdown-it-py.readthedocs.io/en/latest", None),
 }
@@ -57,76 +57,127 @@
 
 html_theme_options = {
     "header_links_before_dropdown": 4,
     "source_repository": "https://github.com/zclab/stmaterial",
     "source_branch": "main",
     "source_directory": "docs/",
     "show_back_to_top": True,
-    "fix_header_nav": False,
-    "logo":{
-        "text": "Stmaterial",
-        "logo": "_static/logo.png"
-    },
+    "fix_header_nav": True,
+    "logo": {"text": "Stmaterial", "logo": "_static/logo.png"},
     "external_links": [
         {"name": "Furo", "url": "https://pradyunsg.me/furo/quickstart/"},
-        {"name": "Sphinx book theme", "url": "https://sphinx-book-theme.readthedocs.io/en/latest/"},
-        {"name": "Pydata sphinx theme", "url": "https://pydata-sphinx-theme.readthedocs.io/"},
+        {
+            "name": "Sphinx book theme",
+            "url": "https://sphinx-book-theme.readthedocs.io/en/latest/",
+        },
+        {
+            "name": "Pydata sphinx theme",
+            "url": "https://pydata-sphinx-theme.readthedocs.io/",
+        },
     ],
     "show_toc_level": 1,
     "header_icons": [
-        {"name":"Github", "url": "http://github.com/zclab/stmaterial", "fontawesome":"fa-brands fa-github"},
+        {
+            "name": "Github",
+            "url": "http://github.com/zclab/stmaterial",
+            "fontawesome": "fa-brands fa-github",
+        },
     ],
     "sidenav_icons": [
-        {"name":"pypistats", "url": "https://pypistats.org/packages/stmaterial", "image":"https://img.shields.io/pypi/dm/stmaterial.svg?style=flat-square"},
-        {"name":"Github Stars", "url": "https://github.com/zclab/stmaterial", "image":"https://img.shields.io/github/stars/zclab/stmaterial?style=flat-square&logo=github"},
+        {
+            "name": "pypistats",
+            "url": "https://pypistats.org/packages/stmaterial",
+            "image": "https://img.shields.io/pypi/dm/stmaterial.svg?style=flat-square",
+        },
+        {
+            "name": "Github Stars",
+            "url": "https://github.com/zclab/stmaterial",
+            "image": "https://img.shields.io/github/stars/zclab/stmaterial?style=flat-square&logo=github",
+        },
     ],
     "footer_icons": [
-        {"name":"Licence", "url": "https://github.com/zclab/stmaterial/blob/main/LICENSE", "fontawesome":"fa-solid fa-file"},
-        {"name":"Github", "url": "http://github.com/zclab/stmaterial", "fontawesome":"fa-brands fa-github"},
+        {
+            "name": "Licence",
+            "url": "https://github.com/zclab/stmaterial/blob/main/LICENSE",
+            "fontawesome": "fa-solid fa-file",
+        },
+        {
+            "name": "Github",
+            "url": "http://github.com/zclab/stmaterial",
+            "fontawesome": "fa-brands fa-github",
+        },
     ],
     "use_edit_page_button": True,
     "toc_title": "On this page",
     "custom_fonts": {
-        "name": 'LXGWWenKaiLite',
-        "type": 'truetype',
+        "name": "LXGWWenKaiLite",
+        "type": "truetype",
         "src": [
-            {"weight": 200, "url":"https://cdn.jsdelivr.net/gh/zclab/static/fonts/LxgwWenKai-Lite/LXGWWenKaiLite-Light.ttf"},
-            {"weight": 300, "url":"https://cdn.jsdelivr.net/gh/zclab/static/fonts/LxgwWenKai-Lite/LXGWWenKaiLite-Light.ttf"},
-            {"weight": 400, "url":"https://cdn.jsdelivr.net/gh/zclab/static/fonts/LxgwWenKai-Lite/LXGWWenKaiLite-Regular.ttf"},
-            {"weight": 500, "url":"https://cdn.jsdelivr.net/gh/zclab/static/fonts/LxgwWenKai-Lite/LXGWWenKaiLite-Bold.ttf"},
-            {"weight": 600, "url":"https://cdn.jsdelivr.net/gh/zclab/static/fonts/LxgwWenKai-Lite/LXGWWenKaiLite-Bold.ttf"},
+            {
+                "weight": 200,
+                "url": "https://cdn.jsdelivr.net/gh/zclab/static/fonts/LxgwWenKai-Lite/LXGWWenKaiLite-Light.ttf",
+            },
+            {
+                "weight": 300,
+                "url": "https://cdn.jsdelivr.net/gh/zclab/static/fonts/LxgwWenKai-Lite/LXGWWenKaiLite-Light.ttf",
+            },
+            {
+                "weight": 400,
+                "url": "https://cdn.jsdelivr.net/gh/zclab/static/fonts/LxgwWenKai-Lite/LXGWWenKaiLite-Regular.ttf",
+            },
+            {
+                "weight": 500,
+                "url": "https://cdn.jsdelivr.net/gh/zclab/static/fonts/LxgwWenKai-Lite/LXGWWenKaiLite-Bold.ttf",
+            },
+            {
+                "weight": 600,
+                "url": "https://cdn.jsdelivr.net/gh/zclab/static/fonts/LxgwWenKai-Lite/LXGWWenKaiLite-Bold.ttf",
+            },
         ],
     },
-    "light_css_variables": {
-        "primary-color": "#5c6bc0",
+    "css_variables": {
+        "primary-color": "#3949ab",
         "primary-color-dark": "#283593",
-        "primary-color-raised-hover-solid": "#7986cb",
-        "primary-color-raised-focus-solid":"#7986cb",
+        "primary-color-raised-hover-solid": "#5c6bc0",
+        "primary-color-raised-focus-solid": "#5c6bc0",
     },
     "navigation_with_keys": True,
+    "article_top_right": "searchbox.html",
 }
-    
+
 
 blog_path = "blog"
 blog_post_pattern = "posts/*/*"
 blog_authors = {
     "zclab": ("子川", "https://github.com/zclab"),
 }
 
 html_sidebars = {
-    "index":[],
+    "index": [],
     "posts/**": [
-        "search-field.html", "ablog/postcard.html","ablog/categories.html","ablog/tagcloud.html", "ablog/recentposts.html",
+        "search-field.html",
+        "ablog/postcard.html",
+        "ablog/categories.html",
+        "ablog/tagcloud.html",
+        "ablog/recentposts.html",
     ],
     "blog": [
-        "search-field.html", "ablog/categories.html","ablog/tagcloud.html","ablog/archives.html","ablog/recentposts.html",
+        "search-field.html",
+        "ablog/categories.html",
+        "ablog/tagcloud.html",
+        "ablog/archives.html",
+        "ablog/recentposts.html",
     ],
     "blog/**": [
-        "search-field.html", "ablog/categories.html","ablog/tagcloud.html","ablog/archives.html","ablog/recentposts.html",
+        "search-field.html",
+        "ablog/categories.html",
+        "ablog/tagcloud.html",
+        "ablog/archives.html",
+        "ablog/recentposts.html",
     ],
 }
 
 # https://github.com/hung1001/font-awesome-pro-v6
 html_css_files = [
-      "https://cdn.jsdelivr.net/gh/duyplus/fontawesome-pro/css/all.min.css",
+    "https://cdn.jsdelivr.net/gh/duyplus/fontawesome-pro/css/all.min.css",
 ]
 fontawesome_included = True
```

### Comparing `stmaterial-0.0.6/docs/develop.md` & `stmaterial-0.0.7/docs/develop.md`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -5,34 +5,34 @@
 This theme uses the [`sphinx-theme-builder` tool](https://github.com/pradyunsg/sphinx-theme-builder), which is a helper tool for automatically compiling Sphinx theme assets.
 This will download a local copy of NodeJS and build the theme's assets with the environment specified in `package.json`.
 
 ## Theme structure
 
 This theme follows the [`sphinx-theme-builder` filesystem layout](https://sphinx-theme-builder.readthedocs.io/en/latest/reference/filesystem-layout/).
 
-
 ## Build the theme locally
 
 You can build the documentation for this theme to preview it.
 The easiest way to build the documentation in this repository is to use [the `nox` automation tool](https://nox.thea.codes/), a tool for quickly building environments and running commands within them.
 This ensures that your environment has all the dependencies needed to build the documentation.
 
 To do so, follow these steps:
 
 1. Install `nox`
 
    ```console
    $ pip install nox
    ```
+
 2. Build the documentation:
 
    ```console
    $ nox -s docs
    ```
 
 This should create a local environment in a `.nox` folder, build the documentation (as specified in the `noxfile.py` configuration), and the output will be in `docs/_build/html`.
 
 To build live documentation that updates when you update local files, run the following command:
 
 ```console
 $ nox -s docs-live
-```
+```
```

### Comparing `stmaterial-0.0.6/docs/examples/kitchen-sink/admonitions.rst` & `stmaterial-0.0.7/docs/examples/kitchen-sink/admonitions.rst`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.6/docs/examples/kitchen-sink/api.rst` & `stmaterial-0.0.7/docs/examples/kitchen-sink/api.rst`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.6/docs/examples/kitchen-sink/blocks.rst` & `stmaterial-0.0.7/docs/examples/kitchen-sink/blocks.rst`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.6/docs/examples/kitchen-sink/generic.rst` & `stmaterial-0.0.7/docs/examples/kitchen-sink/generic.rst`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.6/docs/examples/kitchen-sink/images.rst` & `stmaterial-0.0.7/docs/examples/kitchen-sink/images.rst`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.6/docs/examples/kitchen-sink/index.md` & `stmaterial-0.0.7/docs/examples/kitchen-sink/index.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.6/docs/examples/kitchen-sink/lists.rst` & `stmaterial-0.0.7/docs/examples/kitchen-sink/lists.rst`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.6/docs/examples/kitchen-sink/really-long.md` & `stmaterial-0.0.7/docs/examples/kitchen-sink/really-long.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.6/docs/examples/kitchen-sink/sphinx-design.md` & `stmaterial-0.0.7/docs/examples/kitchen-sink/sphinx-design.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.6/docs/examples/kitchen-sink/structure.rst` & `stmaterial-0.0.7/docs/examples/kitchen-sink/structure.rst`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.6/docs/examples/kitchen-sink/tables.rst` & `stmaterial-0.0.7/docs/examples/kitchen-sink/tables.rst`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.6/docs/examples/kitchen-sink/typography.rst` & `stmaterial-0.0.7/docs/examples/kitchen-sink/typography.rst`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.6/docs/examples/reference/admonitions.md` & `stmaterial-0.0.7/docs/examples/reference/admonitions.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.6/docs/examples/reference/api.md` & `stmaterial-0.0.7/docs/examples/reference/api.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.6/docs/examples/reference/code-blocks.md` & `stmaterial-0.0.7/docs/examples/reference/code-blocks.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.6/docs/examples/reference/hyperlinks.md` & `stmaterial-0.0.7/docs/examples/reference/hyperlinks.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.6/docs/examples/reference/images.md` & `stmaterial-0.0.7/docs/examples/reference/images.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.6/docs/examples/reference/index.md` & `stmaterial-0.0.7/docs/examples/reference/index.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.6/docs/examples/reference/lists.md` & `stmaterial-0.0.7/docs/examples/reference/lists.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.6/docs/examples/reference/tables.md` & `stmaterial-0.0.7/docs/examples/reference/tables.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.6/docs/examples/reference/tabs.md` & `stmaterial-0.0.7/docs/examples/reference/tabs.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.6/docs/examples/reference/text-formatting.md` & `stmaterial-0.0.7/docs/examples/reference/text-formatting.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.6/docs/posts/plangs/2021-python-pathlib.md` & `stmaterial-0.0.7/docs/posts/plangs/2021-python-pathlib.md`

 * *Files 4% similar despite different names*

```diff
@@ -6,133 +6,129 @@
 tags: python, pathlib
 ---
 
 # Python 中 `pathlib` 模块的使用
 
 `pathlib` 是 python 3.4 才引进的一个较新的模块，`pathlib` 把每一个 `path` 封装成一个对象，通过操作对象来操作路径，非常体现类和对象的封装思想，而且通过对象操作，可以使用链式编程，非常方便。
 
-
 ## 实例化一个 `Path` 对象
 
 使用方法：`Path([path字符串])` -> `Path` 对象
 
 ```python
 >>> from pathlib import Path
- 
+
 #默认是当前目录‘.’
 >>> Path()
- 
+
 #将path路径实例化对象
 >>> Path('/etc/fstab')
- 
+
 #将path路径实例化对象
 >>> Path('a/b')
 ```
 
 ## `Path` 路径查看
 
 使用方法：`str(Path对象)` -> `Path` 路径字符
 
 ```python
 >>> str(Path('/etc/fs'))
 '/etc/fs'
- 
+
 >>> str(Path())
 '.'
- 
+
 >>> str(Path('a/b'))
 'a/b'
 ```
 
 ## 路径拼接操作符 `/`
 
- Path实例化后的路径对象可以通过操作符 `/` 进行路径拼接
+Path实例化后的路径对象可以通过操作符 `/` 进行路径拼接
 
- * `Path对象 / Path对象` -> `Path对象`
- * `Paht对象 / 路径字符串` 或者 `路径字符串 / Paht对象`  -> `Path对象`
+- `Path对象 / Path对象` -> `Path对象`
+- `Paht对象 / 路径字符串` 或者 `路径字符串 / Paht对象` -> `Path对象`
 
 ```python
 >>> P1 = Path('/root')
 >>> P2 = Path('/data')
 >>> P3 = Path('data')
- 
+
 >>> str(P1 / P2)
 '/data'
- 
+
 >>> str(P1 / P3)
 '/root/data'
- 
+
 >>> P1 / '/data'
 PosixPath('/data')
- 
+
 >>> P1 / 'data'
 PosixPath('/root/data')
- 
+
 >>> '/home' / P3
 PosixPath('/home/data')
 ```
 
-
 ## 路径拼接方法
 
 使用方法：`Path对象.joinpath(Path对象|path字符串)` -> `Path` 对象
 
 实现的功能跟操作符 `/` 一样，也可以进行Path对象和字符串的拼接
 
 ```python
 >>> P1 = Path('/root')
 >>> P2 = Path('/data')
 >>> P3 = Path('data')
- 
+
 >>> str(P1.joinpath(P2))
 '/data'
- 
+
 >>> str(P1.joinpath(P3))
 '/root/data'
- 
+
 >>> str(P1.joinpath('data'))
 '/root/data'
- 
+
 >>> str(P1.joinpath('/data'))
 '/data'
 ```
 
-
 ## 路径分解
 
 使用方法：`Path对象.parts` -> `Tuple`
 
 说明：
 
 1. `parts` 是属性，不是方法
 2. 将 `Path` 对象的路径分解成各个部分，然后封装成一个元组
 
 ```python
 >>> P1 = Path('/root/dir1/test1.py')
- 
+
 >>> P1.parts
 ('/', 'root', 'dir1', 'test1.py')
 ```
 
-
 ## 一级父目录
 
 使用方法：`Path对象.parent` -> `Path对象`
 
 说明：
 
 1. `parent` 是属性，不是方法
 2. 返回的是一个 `Path` 对象，所以又可以进行对象操作
 
 ```python
 >>> P1 = Path('/root/dir1/test1.py')
- 
+
 >>> P1.parent
 PosixPath('/root/dir1')
- 
+
 >>> str(P1.parent.parent)
 '/root'
 ```
 
 ## 多级父目录
 
 使用方法：`Path对象.parents` -> `sequence`
@@ -141,24 +137,24 @@
 
 1. 返回的是一个有序序列，可以通过 `list` 查看，或者 `for` 循环迭代
 2. 序列的每一个元素都是 `Path` 对象
 3. 既然是有序的，就可以用 `index`，`index` 为 0 的是父目录，`index` 为 1 的是祖父目录，以此类推到根目录
 
 ```python
 >>> P1 = Path('/root/dir1/test1.py')
- 
+
 >>> P1.parents
 <PosixPath.parents>
- 
+
 >>> list(P1.parents)
 [PosixPath('/root/dir1'), PosixPath('/root'), PosixPath('/')]
- 
+
 >>> for i in P1.parents:
 >>>     print(i)
- 
+
 /root/dir1
 /root
 /
 ```
 
 ## 查看Path对象的文件名称
 
@@ -166,148 +162,141 @@
 
 说明：查看路径最后一部分的文件名称
 
 ```python
 >>> P1 = Path('/root/dir1/test1.py')
 >>> P1.name
 'test1.py'
- 
+
 >>> P2 = Path('/root/dir1/test1.py/')
 >>> P2.name
 'test1.py'
- 
+
 >>> P3 = Path('/')
 >>> P3.name
 ''
 ```
 
-
 ## 查看Path对象的文件名称
 
 使用方法：`Path对象.stem` -> 不带后缀的文件名称
 
 说明：
 
 1.  查看路径最后一部分的不带后缀的文件名称
 2.  不带后缀就是文件名称去掉 `.xxx` 的内容，只会去掉最后一个后缀名称
 
 ```python
 >>> P1 = Path('/root/dir1/test1.py')
 >>> P1.stem
 'test1'
- 
+
 #如果有多个后缀，只会去掉最后一个后缀
 >>> P2 = Path('/root/dir1/test1.tar.gz')
 >>> P2.stem
 'test1.tar'
- 
+
 >>> P3 = Path('/')
 >>> P3.stem
 ''
 ```
 
-
 ## 查看Path对象的文件名称后缀
 
 使用方法：`Path对象.suffix` -> 后缀名称
 
 说明：
 
 1. 如果一个文件有多个后缀，只会查看最后一个后缀的名称
 
 ```python
 >>> P1 = Path('/root/dir1/test1.py')
 >>> P1.suffix
 '.py'
- 
+
 #如果有多个后缀，只会返回最后一个后缀名称
 >>> P2 = Path('/root/dir1/test1.tar.gz')
 >>> P2.suffix
 '.gz'
 ```
 
-
 ## 查看Path对象的文件名称后缀
 
 使用方法：`Path对象.suffixes` -> 后缀名称组成的列表
 
 说明：
+
 1. 将文件名的一个或多个后缀放到列表中
 2. 适合有多个后缀名称的文件
 
-
 ```python
 >>> P1 = Path('/root/dir1/test1.py')
 >>> P1.suffixes
 ['.py']
- 
+
 >>> P2 = Path('/root/dir1/test1.tar.gz')
 >>> P2.suffixes
 ['.tar', '.gz']
 ```
 
-
 ## 添加后缀名到路径尾部
 
 使用方法：`Path对象.with_suffix(suffix)` -> `Path` 对象
 
 ① 给文件名添加指定后缀
 
 ② 如果文件名已经存在后缀，则替换
 
 ```python
 #如果后缀已经存在，则替换
 >>> P1 = Path('/root/dir1/test1.py')
 >>> P1.with_suffix('.gz')
 PosixPath('/root/dir1/test1.gz')
- 
+
 >>> P2 = Path('/root/dir1/test1')
 >>> P2.with_suffix('.gz')
 PosixPath('/root/dir1/test1.gz')
- 
+
 >>> P3 = Path('/root/dir1/test1/')
 >>> P3.with_suffix('.gz')
 PosixPath('/root/dir1/test1.gz')
 ```
 
 ## 替换路径的文件名
 
 使用方法：`Path对象.with_name(name)` -> `Path` 对象
 
 ```python
 >>> P1 = Path('/root/dir1/test1.py')
 >>> P1.with_name('.gz')
 PosixPath('/root/dir1/.gz')
- 
+
 >>> P2 = Path('/root/dir1/test1/')
 >>> P2.with_name('good')
 PosixPath('/root/dir1/good')
 ```
 
-
 ## 返回当前工作目录
 
 使用方法：`Path.cwd()` -> `Path` 对象
 
 ```python
 >>> P1.cwd()
 PosixPath('/home/python/jupyter')
 ```
 
-
 ## 返回当前家目录
 
 使用方法：`Path.home()` -> `Path` 对象
 
 ```python
 >>> P1.home()
 PosixPath('/home/python')
 ```
 
-
 ## `is` 系列的判断
 
 ① `exists()`：判断Path对象路径是否存在
 
 ② `is_dir()`：判断Path对象是否是目录
 
 ③ `is_file()`：判断Path对象是否是文件
@@ -324,27 +313,26 @@
 
 说明：判断的时候，要有查看的权限，不然会抛出异常
 
 ```python
 >>> P1 = Path('/root/dir1/test1/')
 >>> P1.is_file()
 PermissionError: [Errno 13] Permission denied: '/root/dir1/test1'
- 
+
 >>> P2 = Path('/tmp/dirt/test1')
 >>> P2.is_dir()
 False
- 
+
 >>> P3 = Path('/etc/rc.local')
 >>> P3.is_file()
 True
 >>> P3.is_symlink()
 True
 ```
 
-
 ## 解析一个路径
 
 使用方法：`Path对象.resolve()` -> `Path` 对象
 
 说明：
 
 ① 如果Path对象是一个普通文件，则返回自身
@@ -352,127 +340,121 @@
 ② 如果Path对象是一个链接文件，则返回源文件
 
 ```python
 #链接文件，返回源文件
 >>> P1 = Path('/etc/rc.local')
 >>> P1.resolve()
 PosixPath('/etc/rc.d/rc.local')
- 
+
 #普通文件，返回自身
 >>> P2 = Path('/etc/rc.d/rc.local')
 >>> P2.resolve()
 PosixPath('/etc/rc.d/rc.local')
 ```
 
-
 ## 删除一层空目录
 
 使用方法：`Path对象.rmdir()`
 
 说明：
 
 ① Path对象必须是一个空目录
 
 ```python
 >>> P1 = Path('/tmp/test1.py')
- 
+
 #Path对象必须是一个空目录
 >>> P1.rmdir()
 NotADirectoryError: [Errno 20] Not a directory: '/tmp/test1.py'
- 
+
 #Path对象必须是一个空目录
 >>> P2 = Path('/tmp/test_go')
 >>> P2.rmdir()
 OSError: [Errno 39] Directory not empty: '/tmp/test_go'
- 
+
 #成功删除
 >>> P3 = Path('/tmp/test_go/dir2')
 P3.rmdir()
 ```
 
-
 ## 创建一个文件
 
 使用方法：`Paht对象.touch(mode=0oxxx)`
 
 说明：
 
 ① 如果文件已经存在，则不会重新创建
 
 ② 指定文件权限使用八进制格式
 
 ```python
 >>> P1 = Path('/tmp/test1.py')
 >>> P1.touch()
- 
+
 >>> P2 = Path('/tmp/test3.py')
 >>> P2.touch(0o777)
 ```
 
-
 ## 创建目录
 
 使用方法：`Paht对象.mkdir(mode=0oxxx, parents=False,exist_ok=Fasle)`
 
 说明：
 
 ① `mode`：指定目录权限，使用八进制格式
 
 ② `parents`：如果父目录不存在，是否创建，True 等同于 linux 的 `mkdir -p` 命令
 
 ③ `exist_ok`：Fasle表示，如果目录已经存在，则抛出异常，True 表示，如果目录存在不抛出异常
 
-
 ```python
 >>> P1 = Path('/tmp/test_do')
 >>> P1.mkdir(mode=0o744)
- 
+
 #默认只能创建一层空目录
 >>> P2 = Path('/tmp/test_do/a/b/c')
 >>> P2.mkdir()
 FileNotFoundError: [Errno 2] No such file or directory: '/tmp/test_do/a/b/c'
- 
+
 #使用parents=True，可以递归创建目录
 >>> P2.mkdir(parents=True)
- 
+
 #目录已经存在，再创建抛出异常
 >>> P2.mkdir(parents=True)
 FileExistsError: [Errno 17] File exists: '/tmp/test_do/a/b/c'
- 
+
 #目录已经存在，指定了exitst_ok=True，所以不抛出异常
 >>> P2.mkdir(parents=True,exist_ok=True)
 ```
 
-
 ## 迭代当前目录
 
 使用方法：`Path对象.iterdir()` -> `Generator`
 
 说明：
 
 ① 只对当前目录进行迭代，不会渗透入到每个子目录
 
 ② 返回一个生成器，可以使用for循环进行迭代
 
-
 ```shell
 [root@jimmy tmp]# tree test_go/
 test_go/
 |-- dir1
 |   `-- dir1.py
 |-- dir3
 |-- test.p3
 |-- test.py1
 `-- test.py2
- 
+
 #对当前目录的所有文件（文件和目录）进行迭代
 >>> P1 = Path('/tmp/test_go')
 >>> for i in P1.iterdir():
 >>>     print(i)
-     
+
 /tmp/test_go/dir1
 /tmp/test_go/test.py2
 /tmp/test_go/dir3
 /tmp/test_go/test.py1
 /tmp/test_go/test.p3
 ```
 
@@ -484,80 +466,73 @@
 
 ① 只会查询指定目录的文件，不会递归
 
 ② 返回的是一个生成器，可以使用for循环，或者用list
 
 ③ 生成器的每一个元素都是一个 `Path` 对象
 
-
 ```shell
 [root@jimmy tmp]# tree test_go/
 test_go/
 |-- dir1
 |   |-- dir1.py
 |   `-- test.py
 |-- dir3
 |-- test.p3
 |-- test.py1
 `-- test.py2
- 
+
 >>> P1 = Path('/tmp/test_go')
- 
+
 >>> list(P1.glob("py*"))
 []
- 
+
 #当前目录只有两个以test.py开头的文件，不会递归子目录
 >>> list(P1.glob("test.py*"))
 [PosixPath('/tmp/test_go/test.py2'), PosixPath('/tmp/test_go/test.py1')]
 ```
 
-
 ## 通过通配符查询指定路径下的文件
 
 使用方法：`Path对象.rglob(pattern)` -> `Generator`
 
 说明：
 
 ① 只会查询指定目录的文件，会递归每一个子目录
 
 ② 返回的是一个生成器，可以使用for循环，或者用list
 
 ③ 生成器的每一个元素都是一个 `Path` 对象
 
-
 ```shell
 #当前所有目录有三个以test.py开头的文件，递归了子目录
 >>> list(P1.rglob("test.py*"))
 [PosixPath('/tmp/test_go/test.py2'),
  PosixPath('/tmp/test_go/test.py1'),
  PosixPath('/tmp/test_go/dir1/test.py')]
- ```
-
+```
 
 ## 查看文件详细信息
- 
+
 使用方法：`Path对象.stat()`
 
 说明：
 
 ① 等同于 linux 的 `stat` 命令，返回一个 `stat` 对象
 
 ② 如果是链接文件，会跟踪到源文件，使用 `lstat()` 查看的是文件本身
 
 ```python
 >>> P1 = Path('/tmp/test_go')
 >>> P1.stat()
 os.stat_result(st_mode=16893, st_ino=256377, st_dev=64769, st_nlink=4, st_uid=1000, st_gid=1000, st_size=4096, st_atime=1554106724, st_mtime=1554186613, st_ctime=1554186613)
- 
+
 #返回一个stat对象，通过属性相关数值
 >>> P1.stat().st_uid
 100
 ```
 
-
-
 ## `Path` 使用总结
 
 ① 核心就是把一个路径封装成一个对象，通过对象的属性或者方法来操作路径
 
 ② 很多方法返回的仍然是一个 `Path` 对象，通过 `Path` 对象又可以访问属性或者调用访问，实现链式编程
-
```

### Comparing `stmaterial-0.0.6/docs/posts/plangs/2022-python-setup.md` & `stmaterial-0.0.7/docs/posts/plangs/2022-python-setup.md`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,14 @@
 - Wheel 使用和 PEP376 兼容的 `.dist-info` 目录，而 Egg 使用 `.egg-info` 目录
 - Wheel 有着更丰富的命名规则。
 - Wheel 是有版本的。每个 Wheel 文件都包含 wheel 规范的版本和打包的实现
 - Wheel 在内部被 sysconfig path type 管理，因此转向其他格式也更容易
 
 详细描述可见：[Wheel vs Egg](https://packaging.python.org/discussions/wheel-vs-egg/)
 
-
 ## `setup.py` 文件
 
 Python 库打包分发的关键在于编写 `setup.py` 文件。`setup.py` 文件编写的规则是从 setuptools 或者 distuils 模块导入 setup 函数，并传入各类参数进行调用。
 
 ```python
 # coding:utf-8
 
@@ -120,35 +119,35 @@
 
 默认默认情况下 `setup.py` 文件只在其所在的目录下搜索包。如果不用 `find_packages`，想要找到其他目录下的包，也可以设置 package_dir 参数，其指定哪些目录下的文件被映射到哪个源码包，如: `package_dir={'': 'src'}` 表示 “root package” 中的模块都在 src 目录中。
 
 ### 包含数据文件
 
 - **`package_data`:**
 
-    该参数是一个从包名称到 glob 模式列表的字典。如果数据文件包含在包的子目录中，则 `glob` 可以包括子目录名称。其格式一般为 `{'package_name': ['files']}`，比如：`package_data={'mypkg': ['data/*.dat'],}`。
+  该参数是一个从包名称到 glob 模式列表的字典。如果数据文件包含在包的子目录中，则 `glob` 可以包括子目录名称。其格式一般为 `{'package_name': ['files']}`，比如：`package_data={'mypkg': ['data/*.dat'],}`。
 
 - **`include_package_data`:**
 
-    该参数被设置为 True 时自动添加包中受版本控制的数据文件，可替代 `package_data`，同时，`exclude_package_data` 可以排除某些文件。注意当需要加入没有被版本控制的文件时，还是仍然需要使用 `package_data` 参数才行。
+  该参数被设置为 True 时自动添加包中受版本控制的数据文件，可替代 `package_data`，同时，`exclude_package_data` 可以排除某些文件。注意当需要加入没有被版本控制的文件时，还是仍然需要使用 `package_data` 参数才行。
 
 - **`data_files`:**
 
-    该参数通常用于包含不在包内的数据文件，即包的外部文件，如：配置文件，消息目录，数据文件。其指定了一系列二元组，即`(目的安装目录，源文件)` ，表示哪些文件被安装到哪些目录中。如果目录名是相对路径，则相对于安装前缀进行解释。
+  该参数通常用于包含不在包内的数据文件，即包的外部文件，如：配置文件，消息目录，数据文件。其指定了一系列二元组，即`(目的安装目录，源文件)` ，表示哪些文件被安装到哪些目录中。如果目录名是相对路径，则相对于安装前缀进行解释。
 
 - **`manifest template`:**
 
-    `manifest template` 即编写 `MANIFEST.in` 文件，文件内容就是需要包含在分发包中的文件。一个 MANIFEST.in 文件如下：
+  `manifest template` 即编写 `MANIFEST.in` 文件，文件内容就是需要包含在分发包中的文件。一个 MANIFEST.in 文件如下：
 
-    ```
-    include *.txt
-    recursive-include examples *.txt *.py
-    prune examples/sample?/build
-    ```
+  ```
+  include *.txt
+  recursive-include examples *.txt *.py
+  prune examples/sample?/build
+  ```
 
-    **`MANIFEST.in`** 文件的编写规则可参考：[Creating a Source Distribution](https://docs.python.org/3.6/distutils/sourcedist.html)
+  **`MANIFEST.in`** 文件的编写规则可参考：[Creating a Source Distribution](https://docs.python.org/3.6/distutils/sourcedist.html)
 
 ### 生成脚本
 
 有两个参数 `scripts` 参数或 `console_scripts` 可用于生成脚本。
 
 `entry_points ` 参数用来支持自动生成脚本，其值应该为是一个字典，从 `entry_point` 组名映射到一个表示 `entry_point` 的字符串或字符串列表，如：
 
@@ -213,15 +212,14 @@
                   include_dirs=[numpy.get_include()])
     ]
 )
 ```
 
 详细了解可参考：[preprocessor options](https://docs.python.org/3.6/distutils/setupscript.html#preprocessor-options)
 
-
 ### `zip_safe`
 
 `zip_safe` 参数决定包是否作为一个 zip 压缩后的 egg 文件安装，还是作为一个以 .egg 结尾的目录安装。因为有些工具不支持 zip 压缩文件，而且压缩后的包也不方便调试，所以建议将其设为 False，即 `zip_safe=False`。
 
 ### 自定义命令
 
 `Setup.py` 文件有很多内置的的命令，可以使用 `python setup.py --help-commands` 查看。如果想要定制自己需要的命令，可以添加 cmdclass 参数，其值为一个 dict。实现自定义命名需要继承 `setuptools.Command` 或者 `distutils.core.Command` 并重写 **run** 方法。
@@ -330,68 +328,67 @@
     'Programming Language :: Python :: 3',
     'Programming Language :: Python :: 3.3',
     'Programming Language :: Python :: 3.4',
     'Programming Language :: Python :: 3.5',
 ]
 ```
 
-
 ## `setup.py` 命令
 
 `setup.py` 文件有很多内置命令可供使用，查看所有支持的命令：
 
 > python setup.py --help-commands
 
 此处列举一些常用命令：
 
 - **`build`:**
 
-    构建安装时所需的所有内容
+  构建安装时所需的所有内容
 
 - **`build_ext`:**
 
-    构建扩展，如用 C/C++, Cython 等编写的扩展，在调试时通常加 `--inplace` 参数，表示原地编译，即生成的扩展与源文件在同样的位置。
+  构建扩展，如用 C/C++, Cython 等编写的扩展，在调试时通常加 `--inplace` 参数，表示原地编译，即生成的扩展与源文件在同样的位置。
 
 - **`sdist`:**
 
-    构建源码分发包，在 Windows 下为 zip 格式，Linux 下为 tag.gz 格式 。执行 sdist 命令时，默认会被打包的文件：
+  构建源码分发包，在 Windows 下为 zip 格式，Linux 下为 tag.gz 格式 。执行 sdist 命令时，默认会被打包的文件：
 
-    ```
-    所有 py_modules 或 packages 指定的源码文件
-    所有 ext_modules 指定的文件
-    所有 package_data 或 data_files 指定的文件
-    所有 scripts 指定的脚本文件
-    README、README.txt、setup.py 和 setup.cfg文件
-    ```
+  ```
+  所有 py_modules 或 packages 指定的源码文件
+  所有 ext_modules 指定的文件
+  所有 package_data 或 data_files 指定的文件
+  所有 scripts 指定的脚本文件
+  README、README.txt、setup.py 和 setup.cfg文件
+  ```
 
-    该命令构建的包主要用于发布，例如上传到 [pypi](https://pypi.org/) 上。
+  该命令构建的包主要用于发布，例如上传到 [pypi](https://pypi.org/) 上。
 
 - **`bdist`:**
 
-    构建一个二进制的分发包。
+  构建一个二进制的分发包。
 
 - **`bdist_egg`:**
 
-    构建一个 egg 分发包，经常用来替代基于 bdist 生成的模式
+  构建一个 egg 分发包，经常用来替代基于 bdist 生成的模式
 
 - **`bdist_wheel`:**
 
-    构建一个 wheel 分发包，egg 包是过时的，whl 包是新的标准
+  构建一个 wheel 分发包，egg 包是过时的，whl 包是新的标准
 
 - **`install`:**
 
-    安装包到系统环境中。
+  安装包到系统环境中。
 
 - **`develop`:**
 
-    以开发方式安装包，该命名不会真正的安装包，而是在系统环境中创建一个软链接指向包实际所在目录。这边在修改包之后不用再安装就能生效，便于调试。
+  以开发方式安装包，该命名不会真正的安装包，而是在系统环境中创建一个软链接指向包实际所在目录。这边在修改包之后不用再安装就能生效，便于调试。
 
 - **`register`、`upload`:**
 
-    用于包的上传发布，后文详述。
+  用于包的上传发布，后文详述。
 
 ## `setup.cfg` 文件
 
 `setup.cfg` 文件用于提供 `setup.py` 的默认参数，详细的书写规则可参考：[configfile](https://docs.python.org/3/distutils/configfile.html)
 
 ## 版本命名
 
@@ -409,15 +406,15 @@
 - `N[.N]`: 阶段版本号，如果提供，则至少有一位主版本号，后面可以加无限多位的副版本号
 - `.postN`: 发行后更新版本号，可选
 - `.devN`: 开发期间的发行版本号，可选
 
 ## `easy_install` 与 `pip`
 
 `easy_insall` 是 setuptool 包提供的第三方包安装工具，而 `pip` 是 Python
- 中一个功能完备的包管理工具，是 `easy_install` 的改进版，提供更好的提示信息，删除包等功能。
+中一个功能完备的包管理工具，是 `easy_install` 的改进版，提供更好的提示信息，删除包等功能。
 
 `pip` 相对于 `easy_install` 进行了以下几个方面的改进:
 
 - 所有的包是在安装之前就下载了，所以不可能出现只安装了一部分的情况
 - 在终端上的输出更加友好
 - 对于动作的原因进行持续的跟踪。例如，如果一个包正在安装，那么 `pip` 就会跟踪为什么这个包会被安装
 - 错误信息会非常有用
@@ -472,15 +469,15 @@
 ```
 python setup.py sdist bdist_wheel && twine upload dist/*
 ```
 
 ## 参考资料
 
 - [Building and Distributing Packages with Setuptools
-](https://setuptools.readthedocs.io/en/latest/setuptools.html)
+  ](https://setuptools.readthedocs.io/en/latest/setuptools.html)
 - [Python 包管理工具解惑](https://blog.zengrong.net/post/2169.html)
 - [Differences between distribute, distutils, setuptools and distutils2?
-](https://stackoverflow.com/questions/6344076/differences-between-distribute-distutils-setuptools-and-distutils2)
+  ](https://stackoverflow.com/questions/6344076/differences-between-distribute-distutils-setuptools-and-distutils2)
 - [如何打包你的Python代码](http://python-packaging-zh.readthedocs.io/zh_CN/latest/index.html)
 - [How to extend distutils with a simple post install script?
-](https://stackoverflow.com/questions/1321270/how-to-extend-distutils-with-a-simple-post-install-script/1321345)
-- [Why use pip over easy_install?](https://stackoverflow.com/questions/3220404/why-use-pip-over-easy-install)
+  ](https://stackoverflow.com/questions/1321270/how-to-extend-distutils-with-a-simple-post-install-script/1321345)
+- [Why use pip over easy_install?](https://stackoverflow.com/questions/3220404/why-use-pip-over-easy-install)
```

### Comparing `stmaterial-0.0.6/docs/posts/plangs/2022-python-typing.md` & `stmaterial-0.0.7/docs/posts/plangs/2022-python-typing.md`

 * *Files 1% similar despite different names*

```diff
@@ -49,36 +49,35 @@
 
 ```python
 add(2)
 ```
 
 则可以正常输出结果 3。但如果我们传入的参数并不是我们期望的类型，比如传入一个字符类型，那么就会同样报刚才类似的错误。 但又由于 Python 的特性，很多情况下我们并不用去声明它的类型，因此从方法定义上面来看，我们实际上是不知道一个方法的参数到底应该传入什么类型的。 这样其实就造成了很多不方便的地方，在某些情况下一些复杂的方法，如果不借助于一些额外的说明，我们是不知道参数到底是什么类型的。 因此，Python 中的类型注解就显得比较重要了。
 
-
 ## 类型注解
 
 在 Python 3.5 中，Python PEP 484 引入了类型注解（type hints），在 Python 3.6 中，PEP 526 又进一步引入了变量注解（Variable Annotations），所以上面的代码我们改写成如下写法：
 
 ```python
 a: int = 2
 print('5 + a =', 5 + a)
 
 def add(a: int) -> int:
     return a + 1
 ```
 
 具体的语法是可以归纳为两点：
-* 在声明变量时，变量的后面可以加一个冒号，后面再写上变量的类型，如 int、list 等等。
-* 在声明方法返回值的时候，可以在方法的后面加一个箭头，后面加上返回值的类型，如 int、list 等等。
 
+- 在声明变量时，变量的后面可以加一个冒号，后面再写上变量的类型，如 int、list 等等。
+- 在声明方法返回值的时候，可以在方法的后面加一个箭头，后面加上返回值的类型，如 int、list 等等。
 
 在 PEP 8 中，具体的格式是这样规定的：
-* 在声明变量类型时，变量后方紧跟一个冒号，冒号后面跟一个空格，再跟上变量的类型。
-* 在声明方法返回值的时候，箭头左边是方法定义，箭头右边是返回值的类型，箭头左右两边都要留有空格。
 
+- 在声明变量类型时，变量后方紧跟一个冒号，冒号后面跟一个空格，再跟上变量的类型。
+- 在声明方法返回值的时候，箭头左边是方法定义，箭头右边是返回值的类型，箭头左右两边都要留有空格。
 
 有了这样的声明，以后我们如果看到这个方法的定义，我们就知道传入的参数类型了，如调用 add 方法的时候，我们就知道传入的需要是一个数值类型的变量，而不是字符串类型，非常直观。 但值得注意的是，这种类型和变量注解实际上只是一种类型提示，对运行实际上是没有影响的，比如调用 add 方法的时候，我们传入的不是 int 类型，而是一个 float 类型，它也不会报错，也不会对参数进行类型转换，如：
 
 ```python
 add(1.5)
 ```
 
@@ -111,24 +110,22 @@
 names: List[str] = ['Germey', 'Guido']
 version: Tuple[int, int, int] = (3, 7, 4)
 operations: Dict[str, bool] = {'show': False, 'sort': True}
 ```
 
 这样一来，变量的类型便可以非常直观地体现出来了。 目前 `typing` 模块也已经被加入到 Python 标准库中，不需要安装第三方模块，我们就可以直接使用了。
 
-
 ## `typing`
 
 下面我们再来详细看下`typing` 模块的具体用法，这里主要会介绍一些常用的注解类型，如 `List`、`Tuple`、`Dict`、`Sequence` 等等，了解了每个类型的具体使用方法，我们可以得心应手的对任何变量进行声明了。 在引入的时候就直接通过 `typing` 模块引入就好了，例如：
 
 ```python
 from typing import List, Tuple
 ```
 
-
 ### `List`
 
 `List`、列表，是 list 的泛型，基本等同于 list，其后紧跟一个方括号，里面代表了构成这个列表的元素类型，如由数字构成的列表可以声明为：
 
 ```python
 var: List[int or float] = [2, 3.5]
 ```
@@ -145,39 +142,36 @@
 
 ```python
 person: Tuple[str, int, float] = ('Mike', 22, 1.75)
 ```
 
 同样地也可以使用类型嵌套。 `NamedTuple`，是 `collections.namedtuple` 的泛型，实际上就和 `namedtuple` 用法完全一致，但个人其实并不推荐使用 `NamedTuple`，推荐使用 attrs 这个库来声明一些具有表征意义的类。
 
-
 ### `Dict`、`Mapping`、`MutableMapping`
 
 `Dict`、字典，是 dict 的泛型；`Mapping`，映射，是 `collections.abc.Mapping` 的泛型。根据官方文档，`Dict` 推荐用于注解返回类型，`Mapping` 推荐用于注解参数。它们的使用方法都是一样的，其后跟一个中括号，中括号内分别声明键名、键值的类型，如：
 
 ```python
 def size(rect: Mapping[str, int]) -> Dict[str, int]:
     return {'width': rect['width'] + 100, 'height': rect['width'] + 100}
 ```
 
 这里将 Dict 用作了返回值类型注解，将 Mapping 用作了参数类型注解。 MutableMapping 则是 Mapping 对象的子类，在很多库中也经常用 MutableMapping 来代替 Mapping。
 
-
 ### `Set`、`AbstractSet`
 
 `Set`、集合，是 `set` 的泛型；`AbstractSet`、是 `collections.abc.Set` 的泛型。根据官方文档，Set 推荐用于注解返回类型，`AbstractSet` 用于注解参数。它们的使用方法都是一样的，其后跟一个中括号，里面声明集合中元素的类型，如：
 
 ```python
 def describe(s: AbstractSet[int]) -> Set[int]:
     return set(s)
 ```
 
 这里将 Set 用作了返回值类型注解，将 `AbstractSet` 用作了参数类型注解。
 
-
 ### `Sequence`
 
 `Sequence`，是 `collections.abc.Sequence` 的泛型，在某些情况下，我们可能并不需要严格区分一个变量或参数到底是列表 list 类型还是元组 `tuple` 类型，我们可以使用一个更为泛化的类型，叫做 `Sequence`，其用法类似于 `List`，如：
 
 ```python
 def square(elements: Sequence[float]) -> List[float]:
     return [x ** 2 for x in elements]
@@ -188,57 +182,52 @@
 `NoReturn`，当一个方法没有返回结果时，为了注解它的返回类型，我们可以将其注解为 `NoReturn`，例如：
 
 ```python
 def hello() -> NoReturn:
     print('hello')
 ```
 
-
 ### `Any`
 
 Any，是一种特殊的类型，它可以代表所有类型，静态类型检查器的所有类型都与 Any 类型兼容，所有的无参数类型注解和返回类型注解的都会默认使用 Any 类型，也就是说，下面两个方法的声明是完全等价的：
 
 ```python
 def add(a):
     return a + 1
 
 def add(a: Any) -> Any:
     return a + 1
 ```
 
-
 原理类似于 object，所有的类型都是 object 的子类。但如果我们将参数声明为 object 类型，静态参数类型检查便会抛出错误，而 Any 则不会，具体可以参考官方文档的说明：[Any 类型](https://docs.python.org/zh-cn/3/library/typing.html?highlight=typing#the-any-type)。
 
-
 ### `TypeVar`
 
 `TypeVar`，我们可以借助它来自定义兼容特定类型的变量，比如有的变量声明为 `int`、`float`、`None` 都是符合要求的，实际就是代表任意的数字或者空内容都可以，其他的类型则不可以，比如列表 `list`、字典 `dict` 等等，像这样的情况，我们可以使用 `TypeVar` 来表示。 例如一个人的身高，便可以使用 `int` 或 `float` 或 `None` 来表示，但不能用 `dict` 来表示，所以可以这么声明：
 
 ```python
 height = 1.75
 Height = TypeVar('Height', int, float, None)
 def get_height() -> Height:
     return height
 ```
 
 这里我们使用 `TypeVar` 声明了一个 Height 类型，然后将其用于注解方法的返回结果。
 
-
 ### `NewType`
 
 `NewType`，我们可以借助于它来声明一些具有特殊含义的类型，例如像 `Tuple` 的例子一样，我们需要将它表示为 `Person`，即一个人的含义，但但从表面上声明为 `Tuple` 并不直观，所以我们可以使用 `NewType` 为其声明一个类型，如：
 
 ```python
 Person = NewType('Person', Tuple[str, int, float])
 person = Person(('Mike', 22, 1.75))
 ```
 
 这里实际上 person 就是一个 tuple 类型，我们可以对其像 tuple 一样正常操作。
 
-
 ### `Callable`
 
 `Callable`，可调用类型，它通常用来注解一个方法，比如我们刚才声明了一个 `add` 方法，它就是一个 `Callable` 类型：
 
 ```python
 print(Callable, type(add), isinstance(add, Callable))
 ```
@@ -257,15 +246,14 @@
 
 def get_date_fn() -> Callable[[int, int, int], str]:
     return date
 ```
 
 这里首先声明了一个方法 date，接收三个 int 参数，返回一个 str 结果，`get_date_fn` 方法返回了这个方法本身，它的返回值类型就可以标记为 `Callable`，中括号内分别标记了返回的方法的参数类型和返回值类型。
 
-
 ### `Union`
 
 `Union`，联合类型，`Union[X, Y]` 代表要么是 `X` 类型，要么是 `Y` 类型。 联合类型的联合类型等价于展平后的类型：
 
 ```python
 Union[Union[int, str], float] == Union[int, str, float]
 ```
@@ -297,25 +285,23 @@
         pass
     elif isinstance(fn, Callable):
         fn()
 ```
 
 这样的声明在一些类库方法定义的时候十分常见。
 
-
 ### `Optional`
 
 `Optional`，意思是说这个参数可以为空或已经声明的类型，即 `Optional[X]` 等价于 `Union[X, None]`。 但值得注意的是，这个并不等价于可选参数，当它作为参数类型注解的时候，不代表这个参数可以不传递了，而是说这个参数可以传为 `None`。 如当一个方法执行结果，如果执行完毕就不返回错误信息， 如果发生问题就返回错误信息，则可以这么声明：
 
 ```python
 def judge(result: bool) -> Optional[str]:
     if result: return 'Error Occurred'
 ```
 
-
 ### `Generator`
 
 如果想代表一个生成器类型，可以使用 `Generator`，它的声明比较特殊，其后的中括号紧跟着三个参数，分别代表 `YieldType`、`SendType`、`ReturnType`，如：
 
 ```python
 def echo_round() -> Generator[int, float, str]:
     sent = yield 0
@@ -329,16 +315,14 @@
 ```python
 def infinite_stream(start: int) -> Generator[int, None, None]:
     while True:
         yield start
         start += 1
 ```
 
-
-
 ## 案例实战
 
 接下来让我们看一个实际的项目，看看经常用到的类型一般是怎么使用的。 这里我们看的库是 requests-html，是由 Kenneth Reitz 所开发的，其 GitHub 地址为：[https://github.com/psf/requests-html](https://github.com/psf/requests-html)，下面我们主要看看它的源代码中一些类型是如何声明的。 这个库的源代码其实就一个文件，那就是 [requests_html.py](https://github.com/psf/requests-html/blob/master/requests_html.py)，我们看一下它里面的一些 `typing` 的定义和方法定义。 首先 Typing 的定义部分如下：
 
 ```python
 from typing import Set, Union, List, MutableMapping, Optional
 
@@ -400,8 +384,8 @@
             for attr in ['class', 'rel']:
                 if attr in self._attrs:
                     self._attrs[attr] = tuple(self._attrs[attr].split())
 
         return self._attrs
 ```
 
-这里 `__init__` 方法接收非常多的参数，同时使用 `_URL` 、`_DefaultEncoding` 进行了参数类型注解，另外 `attrs` 方法使用了 `_Attrs` 进行了返回结果类型注解。 整体看下来，每个参数的类型、返回值都进行了清晰地注解，代码可读性大大提高。 以上便是类型注解和 `typing` 模块的详细介绍。
+这里 `__init__` 方法接收非常多的参数，同时使用 `_URL` 、`_DefaultEncoding` 进行了参数类型注解，另外 `attrs` 方法使用了 `_Attrs` 进行了返回结果类型注解。 整体看下来，每个参数的类型、返回值都进行了清晰地注解，代码可读性大大提高。 以上便是类型注解和 `typing` 模块的详细介绍。
```

### Comparing `stmaterial-0.0.6/docs/user_guide/header.md` & `stmaterial-0.0.7/docs/user_guide/header.md`

 * *Files 8% similar despite different names*

```diff
@@ -6,29 +6,27 @@
 
 ```python
 html_theme_options = {
     "fix_header_nav": True,
 }
 ```
 
-
 ## Changing header icons
 
-Stmaterial allows customising the icons that are presented in the header. These icons can be used to link to relevant resources for your project and documentation. To add custom header icons, you need to provide the `header_icons` configuration value to Stmaterial. 
+Stmaterial allows customising the icons that are presented in the header. These icons can be used to link to relevant resources for your project and documentation. To add custom header icons, you need to provide the `header_icons` configuration value to Stmaterial.
 
 ```python
 html_theme_options = {
     "header_icons": [
         {"name":"Github", "url": "http://github.com/zclab/stmaterial", "svg":"github.svg"},
         {"name":"Gitlab", "url": "http://gitlabcom/zclab/stmaterial", "fontawesome":"fa-brands fa-gitlab"},
     ],
 }
 ```
 
-
 ````{note}
 If you wish to use Font Awesome icons in the header, Using `html_css_files` to add the CSS file(s) for Font Awesome.
 ```python
 html_css_files = [
     "https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/fontawesome.min.css",
     "https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/solid.min.css",
     "https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/brands.min.css",
```

### Comparing `stmaterial-0.0.6/docs/user_guide/sidenav.md` & `stmaterial-0.0.7/docs/user_guide/sidenav.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 # Changing sidenav elements
 
-Stmaterial supports customising the elements that show up in the sidenav (left). 
-
+Stmaterial supports customising the elements that show up in the sidenav (left).
 
 ## Default design
 
 The following code snippet lists the fragments (HTML files from Stmaterial's theme folder) that are used for the default sidenav design.
 
 ```{literalinclude} ../../src/stmaterial/theme/stmaterial/theme.conf
 ---
 language: ini
 start-after: "# sidebar-start"
 end-before: "# sidebar-end"
 ---
 ```
 
-
 ## Hiding sidenav
 
 Stmaterial supports hiding the sidenav. To explicitly hide it on a specific page, `hide-sidenav` can be set in the [File-Wide metadata][sphinx-file-wide-metadata] for that page..
 
-
 ````{tab} reStructuredText
 ```rst
 :hide-sidenav:
 
 [page contents]
 ```
 ````
@@ -35,18 +32,17 @@
 hide-sidenav: true
 ---
 
 [page contents]
 ```
 ````
 
-
 ## Set up sidenav icons
 
-Stmaterial allows set up the icons that are presented in the sidenav, there is no sidenav icons by default. To add custom sidenav icons, you need to provide the `sidenav_icons` configuration value to Stmaterial. 
+Stmaterial allows set up the icons that are presented in the sidenav, there is no sidenav icons by default. To add custom sidenav icons, you need to provide the `sidenav_icons` configuration value to Stmaterial.
 
 ```python
 html_theme_options = {
     "sidenav_icons": [
         {"name":"Gitlab", "url": "http://gitlabcom/zclab/stmaterial", "fontawesome":"fa-brands fa-gitlab"},
     ],
 }
```

### Comparing `stmaterial-0.0.6/docs/user_guide/source-buttons.md` & `stmaterial-0.0.7/docs/user_guide/source-buttons.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,61 @@
 # Source Buttons
 
 Source buttons are links to the source of your page’s content (either on your site, or on hosting sites like GitHub).
 
 ## Add an edit button
-You can add a button to each page that will allow users to edit the page text directly and submit a pull request to update the documentation. 
+
+You can add a button to each page that will allow users to edit the page text directly and submit a pull request to update the documentation. To add an edit button, use the following configuration:
+
+```py
+html_theme_options = {
+    "use_edit_page_button": True
+}
+```
+
+By default, an edit buttion is added at the bottom of a page. You can also place the edit button at the top of a page using the following configuration:
+
+```py
+html_theme_options = {
+    "article_top_right": "edit-this-page.html"
+}
+```
 
 ### With popular VCS hosts
+
 Provide the relevant VCS variables, by setting the following keys in [html_theme_options](https://www.sphinx-doc.org/en/master/usage/configuration.html#confval-html_theme_options):
 
 ```py
 html_theme_options = {
-    "source_repository": "https://github.com/pradyunsg/furo/",
+    "source_repository": "https://github.com/zclab/stmaterial/",
     "source_branch": "main",
     "source_directory": "docs/",
 }
 ```
 
 ### With arbitrary URLs
+
 Use arbitrary URLs for the edit button, by setting the following key in [html_theme_options](https://www.sphinx-doc.org/en/master/usage/configuration.html#confval-html_theme_options):
 
 ```py
 html_theme_options = {
     "source_edit_link": "https://my.awesome.host.example.com/awesome/project/edit/{filename}",
 }
 ```
 
 The `{filename}` component will be replaced with the full path to the file, as known from the base of the documentation directory.
 
-
 ## View Source link
-By default, this theme adds a button link to view the source of a page. To disable it, use the following configuration:
+
+By default, this theme adds a button link to view the source of a page at the top of the page. To disable it, use the following configuration:
 
 ```py
 html_show_sourcelink = False
 ```
+
+You can also place the source link button at the bottom of a page using the following configuration:
+
+```py
+html_theme_options = {
+    "article_bottom_right": "sourcelink.html"
+}
+```
```

### Comparing `stmaterial-0.0.6/docs/web-components.rst` & `stmaterial-0.0.7/docs/web-components.rst`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -228,8 +228,8 @@
 .. admonition:: Click me to toggle!
    :class: dropdown
 
    This will be hidden until a click!
 
 .. toggle::
 
-    A standalone toggle button!
+    A standalone toggle button!
```

### Comparing `stmaterial-0.0.6/noxfile.py` & `stmaterial-0.0.7/noxfile.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,40 +5,40 @@
 
 import nox
 
 PACKAGE_NAME = "stmaterial"
 nox.options.sessions = ["lint", "test"]
 KWARGS = dict(level1=None, level2=9, level3=5)
 
+
 #
 # Helpers
 #
 def _versions_bump_helper(version_number, max_version=None):
-    
-    if not(max_version) or int(version_number) <= max_version:
+    if not (max_version) or int(version_number) <= max_version:
         return 0, int(version_number)
     else:
         return 1, 0
 
 
 def _determine_versions(current_version, **kwargs):
     """Returns (version_in_release, version_after_release)"""
     version_in_release = current_version.rsplit(".dev", 1)[0]
-    version_split = version_in_release.split('.')
+    version_split = version_in_release.split(".")
 
     plus, version_after_release = 1, []
     for idx, vs in enumerate(version_split[::-1]):
         vs = int(vs) + plus
-        max_version = kwargs[f'level{len(version_split)-idx}']
+        max_version = kwargs[f"level{len(version_split)-idx}"]
         plus, version_number = _versions_bump_helper(vs, max_version)
         version_after_release.insert(0, str(version_number))
 
     return (
         version_in_release,
-        '.'.join(version_after_release) + ".dev",
+        ".".join(version_after_release) + ".dev",
     )
 
 
 # fmt: off
 assert (
     _determine_versions("0.9.1.dev", **KWARGS)
     == ("0.9.1", "0.9.2.dev")
@@ -133,17 +133,15 @@
     args = session.posargs or ["-n", "auto", "--cov", PACKAGE_NAME]
     session.run("pytest", *args)
 
 
 @nox.session
 def release(session):
     version_file = f"src/{PACKAGE_NAME}/__init__.py"
-    allowed_upstreams = [
-        f"git@github.com:zclab/{PACKAGE_NAME.replace('_', '-')}.git"
-    ]
+    allowed_upstreams = [f"git@github.com:zclab/{PACKAGE_NAME.replace('_', '-')}.git"]
 
     release_version, next_version = get_release_versions(version_file)
 
     session.install(
         "keyring",
         "release-helper",
         "sphinx-theme-builder[cli]",
```

### Comparing `stmaterial-0.0.6/package-lock.json` & `stmaterial-0.0.7/package-lock.json`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.6/package.json` & `stmaterial-0.0.7/package.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -35,8 +35,8 @@
 00000220: 7322 3a20 225e 382e 342e 3231 220a 2020  s": "^8.4.21".  
 00000230: 7d2c 0a20 2022 6465 7065 6e64 656e 6369  },.  "dependenci
 00000240: 6573 223a 207b 0a20 2020 2022 406d 6174  es": {.    "@mat
 00000250: 6572 6961 6c69 7a65 6373 732f 6d61 7465  erializecss/mate
 00000260: 7269 616c 697a 6522 3a20 225e 312e 322e  rialize": "^1.2.
 00000270: 3222 2c0a 2020 2020 226d 6174 6572 6961  2",.    "materia
 00000280: 6c2d 6963 6f6e 7322 3a20 225e 312e 3133  l-icons": "^1.13
-00000290: 2e33 220a 2020 7d0a 7d                   .3".  }.}
+00000290: 2e33 220a 2020 7d0a 7d0a                 .3".  }.}.
```

### Comparing `stmaterial-0.0.6/pyproject.toml` & `stmaterial-0.0.7/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 description = "A sphinx theme of materializecss."
 dynamic = ["version"]
 readme = "README.md"
 
 requires-python = ">=3.8"
 dependencies = [
   "beautifulsoup4",
-  "sphinx >= 5.0,<7.0",
+  "sphinx >= 5.0,< 8.0",
   "sphinx-basic-ng",
   "pygments >= 2.7",
 ]
 
 license = { file = "LICENSE" }
 authors = [{ name = "zclab", email = "syfhub@hotmail.com" }]
 classifiers = [
@@ -50,7 +50,24 @@
 
 [project.entry-points]
 "sphinx.html_themes" = { stmaterial = "stmaterial" }
 
 [project.urls]
 Repository = "https://github.com/zclab/stmaterial"
 Documentation = "https://stmaterial.readthedocs.io/en/latest/"
+
+[tool.ruff]
+ignore-init-module-imports = true
+fix = true
+ignore = [
+  "E501", # line too long | Black take care of it
+]
+
+[tool.djlint]
+profile = "jinja"
+extension = "html"
+indent = 2
+max_line_length = 120
+use_gitignore = true
+format_js = true
+format_css = true
+ignore = "H006,J018,T003,H025"
```

### Comparing `stmaterial-0.0.6/src/stmaterial/__init__.py` & `stmaterial-0.0.7/src/stmaterial/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from sphinx.locale import get_translation
 from ._navigation import add_toctree_functions
 from ._transforms import ShortenLinkTransform, WrapTableAndMathInAContainerTransform
 from .utils import get_theme_options, config_provided_by_user
 from .directives import GalleryDirective
 
 
-__version__ = "0.0.6"
+__version__ = "0.0.7"
 logger = logging.getLogger(__name__)
 
 MESSAGE_CATALOG_NAME = "stmaterial"
 _KNOWN_STYLES_IN_USE: Dict[str, Optional[Style]] = {
     "light": None,
     "dark": None,
 }
@@ -38,15 +38,14 @@
 
 
 def _get_light_style(app: sphinx.application.Sphinx) -> Style:
     return app.builder.highlighter.formatter_args["style"]
 
 
 def _get_dark_style(app: sphinx.application.Sphinx) -> Style:
-    
     # HACK: begins here
     dark_style = None
     try:
         if (
             hasattr(app.config, "_raw_config")
             and isinstance(app.config._raw_config, dict)
             and "pygments_dark_style" in app.config._raw_config
@@ -117,15 +116,15 @@
     light_formatter = HtmlFormatter(style=_KNOWN_STYLES_IN_USE["light"])
     dark_formatter = HtmlFormatter(style=_KNOWN_STYLES_IN_USE["dark"])
 
     lines: List[str] = []
 
     lines.extend(_get_styles(light_formatter, prefix=".highlight"))
 
-    dark_prefix = ':root[theme=dark] .highlight'
+    dark_prefix = ":root[theme=dark] .highlight"
     lines.extend(_get_styles(dark_formatter, prefix=dark_prefix))
 
     return "\n".join(lines)
 
 
 def _overwrite_pygments_css(
     app: sphinx.application.Sphinx,
@@ -175,49 +174,49 @@
     file_meta = context.get("meta", None) or {}
     if "hide-toc" in file_meta:
         return True
     elif "toc" not in context:
         return True
     elif not context["toc"]:
         return True
-    
+
     return False
 
 
 def _compute_hide_sidenav(
     context: Dict[str, Any],
     *,
     builder: StandaloneHTMLBuilder,
     docname: str,
 ) -> bool:
     # Should the sidenav be hidden?
     file_meta = context.get("meta", None) or {}
     if "hide-sidenav" in file_meta:
         return True
-    
+
     if "full-width" in file_meta:
         return True
-    
+
     return False
 
 
 def _compute_hide_tocnav(
     context: Dict[str, Any],
     *,
     builder: StandaloneHTMLBuilder,
     docname: str,
 ) -> bool:
     # Should the sidenav be hidden?
     file_meta = context.get("meta", None) or {}
     if "hide-tocnav" in file_meta:
         return True
-    
+
     if "full-width" in file_meta:
         return True
-    
+
     return False
 
 
 def _html_page_context(
     app: sphinx.application.Sphinx,
     pagename: str,
     templatename: str,
@@ -293,52 +292,52 @@
         )
 
     if not isinstance(app.builder, StandaloneHTMLBuilder):
         raise Exception(
             "stmaterial is being used as an extension in a non-HTML build. "
             "This should not happen."
         )
-    
 
     builder = app.builder
     assert builder, "what?"
     assert (
         builder.highlighter is not None
     ), "there should be a default style known to Sphinx"
     assert (
         builder.dark_highlighter is None
     ), "this shouldn't be a dark style known to Sphinx"
 
     update_known_styles_state(app)
 
     if "ablog" in app.config.extensions:
-        if not config_provided_by_user(
-            app, "post_show_prev_next"
-        ) or app.config.post_show_prev_next == True:
+        if (
+            not config_provided_by_user(app, "post_show_prev_next")
+            or app.config.post_show_prev_next
+        ):
             app.config.post_show_prev_next = False
 
         else:
-            app.config.post_show_prev_next = ''
+            app.config.post_show_prev_next = ""
 
     def _update_default(key: str, *, new_default: Any) -> None:
         app.config.values[key] = (new_default, *app.config.values[key][1:])
 
     # Change the default permalinks icon
     _update_default("html_permalinks_icon", new_default="#")
 
 
 def _update_config(app: sphinx.application.Sphinx) -> None:
     theme_options = get_theme_options(app)
 
     header_icons = theme_options.get("header_icons", [])
     source_repo = theme_options.get("source_repository", None)
-    if not(header_icons) and source_repo:
+    if not (header_icons) and source_repo:
         header_icons.append(
-            {"name":"Github", "url": source_repo, "class":"fa-brands fa-github"}
-            )
+            {"name": "Github", "url": source_repo, "class": "fa-brands fa-github"}
+        )
         theme_options["header_icons"] = header_icons
 
     else:
         for icon in header_icons:
             svg = icon.get("svg")
             if svg:
                 svg = f"_static/{svg}"
@@ -347,14 +346,18 @@
 
 def update_and_remove_templates(
     app: sphinx.application.Sphinx, pagename: str, templatename: str, context, doctree
 ) -> None:
     template_sections = [
         "theme_footer",
         "theme_footer_content",
+        "theme_article_top_left",
+        "theme_article_top_right",
+        "theme_article_bottom_left",
+        "theme_article_bottom_right",
         "sidebars",
     ]
 
     for section in template_sections:
         if context.get(section):
             # Break apart `,` separated strings so we can use , in the defaults
             if isinstance(context.get(section), str):
```

### Comparing `stmaterial-0.0.6/src/stmaterial/_navigation.py` & `stmaterial-0.0.7/src/stmaterial/_navigation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Generate the navigation tree from Sphinx's toctree function's output."""
 
 import functools
-from urllib.parse import urlparse, urlunparse
+from urllib.parse import urlparse
 from docutils import nodes
 from sphinx.environment.adapters.toctree import TocTree
 from sphinx.addnodes import toctree as toctree_node
 from sphinx import addnodes
-from bs4 import BeautifulSoup, Tag
+from bs4 import BeautifulSoup
 
 
 def add_inline_math(node):
     """Render a node with HTML tags that activate MathJax processing.
     This is meant for use with rendering section titles with math in them, because
     math outputs are ignored by pydata-sphinx-theme's header.
     related to the behaviour of a normal math node from:
@@ -89,15 +89,15 @@
         if soup.new_tag is None:
             continue
 
         label = soup.new_tag(
             "label", attrs={"for": checkbox_name, "class": "toctree-toggle"}
         )
         toggle_icon = soup.new_tag("i", attrs={"class": "material-icons"})
-        toggle_icon.string="keyboard_arrow_down"
+        toggle_icon.string = "keyboard_arrow_down"
         label.append(toggle_icon)
         if "toctree-l0" in classes:
             # making label cover the whole caption text with css
             label["class"] = "label-parts"
         element.insert(1, label)
 
         # Add the checkbox that's used to store expanded/collapsed state.
@@ -113,15 +113,15 @@
 
         # if this has a "current" class, be expanded by default
         # (by checking the checkbox)
         if "current" in classes:
             checkbox.attrs["checked"] = ""
 
         element.insert(1, checkbox)
-        
+
 
 def index_toctree(app, pagename: str, startdepth: int, collapse: bool = True, **kwargs):
     """
     Returns the "local" (starting at `startdepth`) TOC tree containing the
     current page, rendered as HTML bullet lists.
     This is the equivalent of `context["toctree"](**kwargs)` in sphinx
     templating, but using the startdepth-local instead of global TOC tree.
@@ -152,15 +152,14 @@
     toctree_element = _get_local_toctree_for(
         toctree, indexname, pagename, app.builder, collapse, **kwargs
     )
     return app.builder.render_partial(toctree_element)["fragment"]
 
 
 def add_toctree_functions(app, pagename, templatename, context, doctree):
-
     @functools.lru_cache(maxsize=None)
     def generate_header_nav_html(n_links_before_dropdown=5):
         """
         Generate top-level links that are meant for the header navigation.
         We use this function instead of the TocTree-based one used for the
         sidebar because this one is much faster for generating the links and
         we don't need the complexity of the full Sphinx TocTree.
@@ -201,15 +200,17 @@
         meth = "findall" if hasattr(root, "findall") else "traverse"
         for toc in getattr(root, meth)(toctree_node):
             for title, page in toc.attributes["entries"]:
                 # if the page is using "self" use the correct link
                 page = toc.attributes["parent"] if page == "self" else page
 
                 # If this is the active ancestor page, add a class so we highlight it
-                current = "active md-tabs__item--active" if page == active_header_page else ""
+                current = (
+                    "active md-tabs__item--active" if page == active_header_page else ""
+                )
 
                 # sanitize page title for use in the html output if needed
                 if title is None:
                     title = ""
                     for node in app.env.titles[page].children:
                         if isinstance(node, nodes.math):
                             title += add_inline_math(node)
@@ -238,15 +239,15 @@
 
         # Add external links defined in configuration as sibling list items
         for external_link in context["theme_external_links"]:
             links_html.append(
                 f"""
                 <li class="md-tabs__item">
                   <a class="md-tabs__link nav-external" href="{ external_link["url"] }">
-                    { external_link["name"] } 
+                    { external_link["name"] }
                   </a>
                 </li>
                 """
             )
 
         # The first links will always be visible
         links_solo = links_html[:n_links_before_dropdown]
@@ -337,15 +338,17 @@
 
             # Add collapse boxes for parts/captions.
             # Wraps the TOC part in an extra <ul> to behave like chapters with toggles
             # show_nav_level: 0 means make parts collapsible.
             if show_nav_level == 0:
                 partcaptions = soup.find_all("p", attrs={"class": "caption"})
                 if len(partcaptions):
-                    new_soup = BeautifulSoup("<ul class='list-caption'></ul>", "html.parser")
+                    new_soup = BeautifulSoup(
+                        "<ul class='list-caption'></ul>", "html.parser"
+                    )
                     for caption in partcaptions:
                         # Assume that the next <ul> element is the TOC list
                         # for this part
                         for sibling in caption.next_siblings:
                             if sibling.name == "ul":
                                 toclist = sibling
                                 break
@@ -411,11 +414,11 @@
             out = soup
 
         # Return the toctree object
         if kind == "html":
             return out
         else:
             return soup
-    
+
     context["generate_header_nav_html"] = generate_header_nav_html
     context["generate_toctree_html"] = generate_toctree_html
     context["generate_toc_html"] = generate_toc_html
```

### Comparing `stmaterial-0.0.6/src/stmaterial/_transforms.py` & `stmaterial-0.0.7/src/stmaterial/_transforms.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-from typing import Any, Dict, Iterator, List, Optional
+from typing import Any
 from urllib.parse import urlparse, urlunparse
 from docutils import nodes
 from sphinx.transforms.post_transforms import SphinxPostTransform
 from sphinx.util.nodes import NodeMatcher
 from .utils import traverse_or_findall
 
 
-
 class ShortenLinkTransform(SphinxPostTransform):
     """
     Shorten link when they are coming from github or gitlab and add an extra class to the tag
     for further styling.
     Before::
         <a class="reference external" href="https://github.com/2i2c-org/infrastructure/issues/1329">
             https://github.com/2i2c-org/infrastructure/issues/1329
```

### Comparing `stmaterial-0.0.6/src/stmaterial/_translations.py` & `stmaterial-0.0.7/src/stmaterial/_translations.py`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.6/src/stmaterial/assets/scripts/gumshoe-patched.js` & `stmaterial-0.0.7/src/stmaterial/assets/scripts/gumshoe-patched.js`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.6/src/stmaterial/assets/scripts/stmaterial.js` & `stmaterial-0.0.7/src/stmaterial/assets/scripts/stmaterial.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -84,22 +84,24 @@
             ticking = true;
         }
     });
     window.scroll();
 }
 
 function addTOCInteractivity() {
-    document.addEventListener('gumshoeActivate', function(event) {
+    document.addEventListener("gumshoeActivate", function(event) {
         const navLinks = document.querySelectorAll(".table-of-contents li>a");
 
         navLinks.forEach((navLink) => {
             navLink.parentElement.classList.remove("active");
         });
 
-        const activeNavLinks = document.querySelectorAll(".table-of-contents li.scroll-current>a");
+        const activeNavLinks = document.querySelectorAll(
+            ".table-of-contents li.scroll-current>a",
+        );
         activeNavLinks.forEach((navLink) => {
             navLink.parentElement.classList.add("active");
         });
     });
 }
 
 function setupScrollSpy() {
@@ -109,15 +111,15 @@
 
     // Scrollspy -- highlight table on contents, based on scroll
     new Gumshoe(".table-of-contents a", {
         reflow: true,
         recursive: true,
         navClass: "scroll-current",
         nested: true,
-        nestedClass: 'scroll-current', // 
+        nestedClass: "scroll-current", //
         events: true,
         offset: () => {
             let rem = parseFloat(getComputedStyle(document.documentElement).fontSize);
             return header.getBoundingClientRect().height + 0.5 * rem + 1;
         },
     });
 }
@@ -128,90 +130,88 @@
     setupScrollSpy();
 }
 
 function init_materialize() {
     // Detect touch screen and enable scrollbar if necessary
     function is_touch_device() {
         try {
-            document.createEvent('TouchEvent');
+            document.createEvent("TouchEvent");
             return true;
         } catch (e) {
             return false;
         }
     }
 
     // Mobile Overflow
     // if (is_touch_device()) {
     //   document.querySelector('#nav-mobile').style.overflow = 'auto';
     // }
 
     // Theme
-    const theme = localStorage.getItem('theme');
-    const themeSwitch = document.querySelector('#theme-switch');
-    const themeSwitch__mobile = document.querySelector('#theme-switch--mobile');
+    const theme = localStorage.getItem("theme");
+    const themeSwitch = document.querySelector("#theme-switch");
+    const themeSwitch__mobile = document.querySelector("#theme-switch--mobile");
     const setTheme = (isDark) => {
         if (isDark) {
-            themeSwitch.classList.add('is-dark');
-            themeSwitch.querySelector('i').innerText = 'light_mode';
-            themeSwitch.title = 'Switch to light mode';
-
-            themeSwitch__mobile.classList.add('is-dark');
-            themeSwitch__mobile.querySelector('i').innerText = 'light_mode';
-            themeSwitch__mobile.title = 'Switch to light mode';
+            themeSwitch.classList.add("is-dark");
+            themeSwitch.querySelector("i").innerText = "light_mode";
+            themeSwitch.title = "Switch to light mode";
+
+            themeSwitch__mobile.classList.add("is-dark");
+            themeSwitch__mobile.querySelector("i").innerText = "light_mode";
+            themeSwitch__mobile.title = "Switch to light mode";
         } else {
-            themeSwitch.classList.remove('is-dark');
-            themeSwitch.querySelector('i').innerText = 'dark_mode';
-            themeSwitch.title = 'Switch to dark mode';
-
-            themeSwitch__mobile.classList.remove('is-dark');
-            themeSwitch__mobile.querySelector('i').innerText = 'dark_mode';
-            themeSwitch__mobile.title = 'Switch to dark mode';
+            themeSwitch.classList.remove("is-dark");
+            themeSwitch.querySelector("i").innerText = "dark_mode";
+            themeSwitch.title = "Switch to dark mode";
+
+            themeSwitch__mobile.classList.remove("is-dark");
+            themeSwitch__mobile.querySelector("i").innerText = "dark_mode";
+            themeSwitch__mobile.title = "Switch to dark mode";
         }
-    }
+    };
     if (themeSwitch || themeSwitch__mobile) {
         // Load
         if (theme) setTheme(true);
         // Change
-        themeSwitch.addEventListener('click', e => {
+        themeSwitch.addEventListener("click", (e) => {
             e.preventDefault();
-            if (!themeSwitch.classList.contains('is-dark')) {
+            if (!themeSwitch.classList.contains("is-dark")) {
                 // Dark Theme
-                document.documentElement.setAttribute('theme', 'dark');
-                localStorage.setItem('theme', 'dark');
+                document.documentElement.setAttribute("theme", "dark");
+                localStorage.setItem("theme", "dark");
                 setTheme(true);
             } else {
                 // Light Theme
-                document.documentElement.removeAttribute('theme');
-                localStorage.removeItem('theme');
+                document.documentElement.removeAttribute("theme");
+                localStorage.removeItem("theme");
                 setTheme(false);
             }
         });
 
-        themeSwitch__mobile.addEventListener('click', e => {
+        themeSwitch__mobile.addEventListener("click", (e) => {
             e.preventDefault();
-            if (!themeSwitch__mobile.classList.contains('is-dark')) {
+            if (!themeSwitch__mobile.classList.contains("is-dark")) {
                 // Dark Theme
-                document.documentElement.setAttribute('theme', 'dark');
-                localStorage.setItem('theme', 'dark');
+                document.documentElement.setAttribute("theme", "dark");
+                localStorage.setItem("theme", "dark");
                 setTheme(true);
             } else {
                 // Light Theme
-                document.documentElement.removeAttribute('theme');
-                localStorage.removeItem('theme');
+                document.documentElement.removeAttribute("theme");
+                localStorage.removeItem("theme");
                 setTheme(false);
             }
         });
     }
 
-
     // M.Sidenav.init(document.querySelectorAll('.stm-sidenav'), {});
-    M.Dropdown.init(document.querySelectorAll('.dropdown-trigger'), {
+    M.Dropdown.init(document.querySelectorAll(".dropdown-trigger"), {
         constrainWidth: false,
     });
-
 }
 
 /*******************************************************************************
  * Search
  */
 
 /**
@@ -226,15 +226,15 @@
         var form;
         if (forms.length == 1) {
             // there is exactly one search form (persistent or hidden)
             form = forms[0];
         } else {
             // must be at least one persistent form, use the first persistent one
             form = document.querySelector(
-                "div:not(.search-button__search-container) > form.search-wrapper"
+                "div:not(.search-button__search-container) > form.search-wrapper",
             );
         }
         return form.querySelector("input");
     }
 };
 
 /**
@@ -279,27 +279,27 @@
                 toggleSearchField();
             }
             // also allow Escape key to hide (but not show) the dynamic search field
             else if (document.activeElement === input && event.code == "Escape") {
                 toggleSearchField();
             }
         },
-        true
+        true,
     );
 };
 
 /**
  * Change the search hint to `meta key` if we are a Mac
  */
 var changeSearchShortcutKey = () => {
     let forms = document.querySelectorAll("form.search-wrapper");
     var isMac = window.navigator.platform.toUpperCase().indexOf("MAC") >= 0;
     if (isMac) {
         forms.forEach(
-            (f) => (f.querySelector("kbd.kbd-shortcut__modifier").innerText = "⌘")
+            (f) => (f.querySelector("kbd.kbd-shortcut__modifier").innerText = "⌘"),
         );
     }
 };
 
 /**
  * Activate callbacks for search button popup
  */
@@ -315,15 +315,14 @@
     // Add the search button overlay event callback
     let overlay = document.querySelector(".search-button__overlay");
     if (overlay) {
         overlay.onclick = toggleSearchField;
     }
 };
 
-
 ////////////////////////////////////////////////////////////////////////////////
 // Main entrypoint
 ////////////////////////////////////////////////////////////////////////////////
 function main() {
     document.body.parentNode.classList.remove("no-js");
     init_materialize();
     setupSearchButtons();
```

### Comparing `stmaterial-0.0.6/src/stmaterial/assets/styles/base/_typography.scss` & `stmaterial-0.0.7/src/stmaterial/assets/styles/base/_typography.scss`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 body {
   display: flex;
   min-height: 100vh;
   flex-direction: column;
 }
 
-
 main {
   display: flex;
   flex-grow: 1;
-  width: calc(100% - $sidenav-width);
+  width: calc(100% - var(--sidenav-width));
   flex-direction: column;
 }
 
 .stm-main {
   display: flex;
   flex: 1 0 auto;
   flex-direction: column;
@@ -41,15 +40,14 @@
 
 .stm-article-footer {
   margin-top: auto;
   margin-bottom: 20px;
 }
 
 a {
-
   &.github,
   &.gitlab {
     &::before {
       color: var(--color-link);
       font: var(--fa-font-brands);
       margin-right: 0.25rem;
     }
@@ -67,8 +65,8 @@
 b,
 strong {
   font-weight: 900;
 }
 
 .centered {
   text-align: center;
-}
+}
```

### Comparing `stmaterial-0.0.6/src/stmaterial/assets/styles/components/_back-to-top.scss` & `stmaterial-0.0.7/src/stmaterial/assets/styles/components/_back-to-top.scss`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
   display: none;
   position: fixed;
   left: 0;
   // top: 1rem;
   padding: 0.5rem;
   padding-right: 0.75rem;
   border-radius: 1.2rem;
-  font-size: 1.0rem;
+  font-size: 1rem;
 
   background: var(--background-color);
   box-shadow: 0 0.2rem 0.5rem rgba(0, 0, 0, 0.05), #6b728080 0px 0px 1px 0px;
 
   z-index: 10;
 
   margin-left: 50%;
@@ -40,8 +40,8 @@
   color: var(--font-color-main);
 
   &:hover {
     text-decoration: none;
     background: var(--primary-color);
     color: white;
   }
-}
+}
```

### Comparing `stmaterial-0.0.6/src/stmaterial/assets/styles/components/_brand-logo.scss` & `stmaterial-0.0.7/src/stmaterial/assets/styles/components/_brand-logo.scss`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 .stm-brand-logo {
   display: flex;
   align-items: center;
   gap: 0.5rem;
   padding-left: 15px;
   height: $navbar-height;
-  width: $sidenav-width;
+  width: var(--sidenav-width);
 
   @media (max-width: $medium-screen-up) {
     height: $navbar-height-mobile;
   }
 
   img {
-    max-width: calc($sidenav-width - var(--header-horizontal-spacing)*2); // $sidenav-width - 30px; 
+    max-width: calc(
+      var(--sidenav-width) - var(--header-horizontal-spacing) * 2
+    ); // $sidenav-width - 30px;
     max-height: $navbar-height;
 
     @media (max-width: $medium-screen-up) {
       max-height: $navbar-height-mobile;
     }
   }
 }
```

### Comparing `stmaterial-0.0.6/src/stmaterial/assets/styles/components/_prev-next.scss` & `stmaterial-0.0.7/src/stmaterial/assets/styles/components/_prev-next.scss`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -51,8 +51,8 @@
   width: 45%;
 }
 
 .stm-prev {
   display: flex;
   margin-right: auto;
   width: 45%;
-}
+}
```

### Comparing `stmaterial-0.0.6/src/stmaterial/assets/styles/components/_search-field.sass` & `stmaterial-0.0.7/src/stmaterial/assets/styles/components/_search-field.sass`

 * *Files 12% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     display: flex
     position: absolute
     right: 5px
 
 
 input:not([type]):not(.browser-default)
   border-top: $input-border
-  margin: 0.68rem 0 
+  margin: 0.68rem 0
   padding-left: calc(var(--header-horizontal-spacing) + 10px)
   background-color: var(--background-color-sidenav)
   color: var(--font-color-main)
 
   &:focus:not([readonly])
     border-top: 1px solid var(--input-focus-color)
     border-bottom: 1px solid var(--input-focus-color)
```

### Comparing `stmaterial-0.0.6/src/stmaterial/assets/styles/components/_searchbox.scss` & `stmaterial-0.0.7/src/stmaterial/assets/styles/components/_searchbox.scss`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 div#searchbox p.highlight-link {
-  box-shadow: 0 .2rem .5rem var(--surface-color), 0 0 .0625rem var(--surface-color) !important;
-  margin: 1rem 0;
+  box-shadow: 0 0.2rem 0.5rem var(--surface-color),
+    0 0 0.0625rem var(--surface-color) !important;
+  margin: 0;
   width: fit-content;
-
 }
 
 div#searchbox p.highlight-link a {
   display: flex;
   background-color: var(--primary-color);
-  border-radius: .25rem;
+  border-radius: 0.25rem;
   color: #fff;
   font-size: 1.25rem;
-  padding: .75rem;
-  transition: box-shadow .25s ease-out
+  padding: 0.05rem 0.45rem;
+  transition: box-shadow 0.25s ease-out;
 }
 
 div#searchbox p.highlight-link a:hover {
-  box-shadow: inset 0 0 50px 50px rgba(0, 0, 0, .25);
-  text-decoration: none
+  box-shadow: inset 0 0 50px 50px rgba(0, 0, 0, 0.25);
+  text-decoration: none;
 }
 
 div#searchbox p.highlight-link a:before {
   color: unset;
   content: "\e900";
   font-family: Material Icons;
-  margin-right: .5rem;
+  margin-right: 0.5rem;
 }
```

### Comparing `stmaterial-0.0.6/src/stmaterial/assets/styles/components/_table-of-contents.sass` & `stmaterial-0.0.7/src/stmaterial/assets/styles/components/_table-of-contents.sass`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 .stm-toc
   height: 100%
 
 .toc-wrapper
   position: sticky
-  top: calc($navbar-height + 2.8rem)
+  top: calc($navbar-height + 2.8rem + 15px)
   overflow: auto
-  max-height: calc(100vh - $navbar-height - 2.8rem)
+  max-height: calc(100vh - $navbar-height - 2.8rem - 15px)
 
 .toc-scroll
   .nav
     display: none
 
     &.visible
       display: block
 
-    >.active>ul 
+    >.active>ul
       display: block
 
 .toc-title
   display: flex
   gap: 0.25em
   padding-left: 16px
   border-left: 1px solid var(--separator-color)
```

### Comparing `stmaterial-0.0.6/src/stmaterial/assets/styles/content/_admonitions.sass` & `stmaterial-0.0.7/src/stmaterial/assets/styles/content/_admonitions.sass`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.6/src/stmaterial/assets/styles/content/_api.sass` & `stmaterial-0.0.7/src/stmaterial/assets/styles/content/_api.sass`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.6/src/stmaterial/assets/styles/content/_code.sass` & `stmaterial-0.0.7/src/stmaterial/assets/styles/content/_code.sass`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.6/src/stmaterial/assets/styles/content/_footnotes.sass` & `stmaterial-0.0.7/src/stmaterial/assets/styles/content/_footnotes.sass`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.6/src/stmaterial/assets/styles/content/_images.sass` & `stmaterial-0.0.7/src/stmaterial/assets/styles/content/_images.sass`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.6/src/stmaterial/assets/styles/content/_lists.sass` & `stmaterial-0.0.7/src/stmaterial/assets/styles/content/_lists.sass`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.6/src/stmaterial/assets/styles/content/_misc.sass` & `stmaterial-0.0.7/src/stmaterial/assets/styles/content/_misc.sass`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.6/src/stmaterial/assets/styles/content/_sidebar.sass` & `stmaterial-0.0.7/src/stmaterial/assets/styles/content/_sidebar.sass`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.6/src/stmaterial/assets/styles/content/_tables.sass` & `stmaterial-0.0.7/src/stmaterial/assets/styles/content/_tables.sass`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.6/src/stmaterial/assets/styles/content/_target.sass` & `stmaterial-0.0.7/src/stmaterial/assets/styles/content/_target.sass`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.6/src/stmaterial/assets/styles/extensions/_ablog.scss` & `stmaterial-0.0.7/src/stmaterial/assets/styles/extensions/_ablog.scss`

 * *Files 9% similar despite different names*

```diff
@@ -2,16 +2,18 @@
   margin-top: var(--sidenav-ablog-space-above);
   margin-bottom: var(--sidenav-ablog-space-below);
   font-size: var(--sidebar-item-font-size);
 
   h2,
   h3 {
     padding: 0;
-    font-size: 1.30em;
-    margin: 0 var(--sidenav-item-horizontal-spacing) calc(var(--sidenav-ablog-space-below) * 0.5) var(--sidenav-item-horizontal-spacing);
+    font-size: 1.3em;
+    margin: 0 var(--sidenav-item-horizontal-spacing)
+      calc(var(--sidenav-ablog-space-below) * 0.5)
+      var(--sidenav-item-horizontal-spacing);
 
     a {
       color: var(--font-color-main);
       text-decoration: none;
     }
 
     i {
@@ -50,21 +52,20 @@
         display: flex;
         align-items: center;
       }
     }
   }
 }
 
-
 .ablog__prev-next {
   font-size: 0.9em;
   display: flex;
   padding: 1rem 0;
 
-  >span {
+  > span {
     display: flex;
     max-width: 45%;
 
     a {
       display: flex;
       align-items: center;
       margin-left: auto;
@@ -81,20 +82,19 @@
     &.ablog__next {
       margin-left: auto;
       text-align: right;
     }
   }
 }
 
-
 .ablog__collection {
   padding-left: 0;
 
   .ablog-post {
-    ul>li {
+    ul > li {
       list-style: none;
     }
 
     .ablog-archive {
       display: flex;
       flex-direction: row;
       flex-wrap: wrap;
@@ -116,14 +116,13 @@
 
     .ablog-post-expand {
       margin-bottom: 0.5rem;
     }
   }
 }
 
-
 .ablog__catalog_header {
   .section {
     padding-bottom: 0;
     padding-top: 0;
   }
-}
+}
```

### Comparing `stmaterial-0.0.6/src/stmaterial/assets/styles/extensions/_timeline.scss` & `stmaterial-0.0.7/src/stmaterial/assets/styles/extensions/_timeline.scss`

 * *Files 13% similar despite different names*

```diff
@@ -48,15 +48,15 @@
       display: block;
       position: absolute;
       border: 1px black solid;
       z-index: 999;
     }
 
     &.left::after {
-      right: -.6em;
+      right: -0.6em;
     }
 
     &.right::after {
-      left: -.6em;
+      left: -0.6em;
     }
   }
-}
+}
```

### Comparing `stmaterial-0.0.6/src/stmaterial/assets/styles/patch/_test.scss` & `stmaterial-0.0.7/src/stmaterial/assets/styles/patch/_test.scss`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 .section {
-  padding-top: 0
+  padding-top: 0;
 }
 
 /*************************
  * Search button
  */
 // Search link icon should be a bit bigger since it is separate from icon links
 
-
 // __search-container will only show up when we use the search pop-up bar
 .search-button__search-container,
 .search-button__overlay {
   display: none;
 }
 
 .search-button__wrapper.show {
```

### Comparing `stmaterial-0.0.6/src/stmaterial/assets/styles/sections/_footer.scss` & `stmaterial-0.0.7/src/stmaterial/assets/styles/sections/_footer.scss`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.6/src/stmaterial/assets/styles/sections/_headnav.scss` & `stmaterial-0.0.7/src/stmaterial/assets/styles/sections/_headnav.scss`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     z-index: 1099;
   }
 
   .nav-wrapper {
     display: flex;
 
     @media (max-width: $medium-screen-up) {
-      padding-left: 0
+      padding-left: 0;
     }
   }
 
   ul {
     a {
       display: flex;
       padding: 0 var(--header-horizontal-spacing);
@@ -88,15 +88,14 @@
           gap: 0.25rem;
         }
       }
     }
   }
 }
 
-
 a {
   &.nav-external:after {
     color: unset;
     content: "\e89e";
     font-family: Material Icons;
   }
 }
```

### Comparing `stmaterial-0.0.6/src/stmaterial/assets/styles/sections/_sidebar-toggle.scss` & `stmaterial-0.0.7/src/stmaterial/assets/styles/sections/_sidebar-toggle.scss`

 * *Files 9% similar despite different names*

```diff
@@ -23,28 +23,26 @@
   top: 0;
   left: 0;
   transition: opacity 0.3s ease-out;
   z-index: 1299;
 }
 
 input {
-
   // Show the correct overlay when its input is checked
-  &#__primary:checked+label.overlay.overlay-primary,
-  &#__secondary:checked+label.overlay.overlay-secondary {
+  &#__primary:checked + label.overlay.overlay-primary,
+  &#__secondary:checked + label.overlay.overlay-secondary {
     height: 100vh;
     width: 100vw;
   }
 
   // Primary sidebar slides in from the left
-  &#__primary:checked~.stm-main .stm-sidenav {
+  &#__primary:checked ~ .stm-main .stm-sidenav {
     visibility: visible;
     margin-left: 0;
   }
-
 }
 
 /*******************************************************************************
 * Sidebar drawer behavior
 */
 
 /**
@@ -59,37 +57,34 @@
   top: 0;
   z-index: 1299;
   height: 100vh;
   max-height: 100vh;
   width: 75%;
   flex-grow: 0.75;
   max-width: 350px;
-  transition: visibility 0.3s ease-out,
-    margin 0.3s ease-out;
+  transition: visibility 0.3s ease-out, margin 0.3s ease-out;
   visibility: hidden;
 
-  @if $side =="right" {
+  @if $side == "right" {
     margin-right: -75%;
     right: 0;
-  }
-
-  @else {
+  } @else {
     margin-left: -75%;
     left: 0;
   }
 }
 
 // Primary sidebar hides/shows at earlier widths
 @media (min-width: $medium-screen-up) {
   label.sidebar-toggle.primary-toggle {
     display: none;
   }
 
   input#__primary {
-    &:checked+label.overlay.overlay-primary {
+    &:checked + label.overlay.overlay-primary {
       height: 0;
       width: 0;
     }
   }
 
   .stm-sidenav {
     margin-left: 0;
@@ -99,15 +94,14 @@
 
 .stm-sidenav {
   @media (max-width: $medium-screen-up) {
     @include sliding-drawer("left");
   }
 }
 
-
 nav label.sidebar-toggle {
   align-items: center;
   color: var(--pst-color-muted);
   cursor: pointer;
   display: flex;
   font-size: var(--pst-font-size-icon);
   margin-bottom: 0;
```

### Comparing `stmaterial-0.0.6/src/stmaterial/assets/styles/sections/_stm-sidenav.scss` & `stmaterial-0.0.7/src/stmaterial/assets/styles/sections/_stm-sidenav.scss`

 * *Files 3% similar despite different names*

```diff
@@ -3,18 +3,24 @@
 }
 
 aside.stm-sidenav {
   border-right: 1px solid var(--separator-color);
   clip-path: inset(0);
   display: block;
   background-color: var(--background-color-sidenav);
-  width: $sidenav-width;
+  width: var(--sidenav-width);
+
+  @media (max-width: $medium-screen-up) {
+    width: 300px;
+  }
 
   @media (min-width: $medium-screen-up) {
-    margin-top: calc($navbar-height *-1 - 2px); // 2px because of box shadow is 2px height offset of nav, see z-depth-1
+    margin-top: calc(
+      $navbar-height * -1 - 2px
+    ); // 2px because of box shadow is 2px height offset of nav, see z-depth-1
   }
 
   .sidenav-viewport {
     height: 100%;
     max-height: 100vh;
     position: sticky;
     top: 0;
@@ -25,15 +31,15 @@
       height: 100%;
       // width: $sidenav-width;
 
       .sidenav-menu {
         flex-grow: 1;
         padding: 0 0 0 var(--header-horizontal-spacing);
         overflow: auto;
-        margin-top: 1.0rem;
+        margin-top: 1rem;
 
         .sidenav-menulist {
           list-style: none;
           margin: 0;
           padding-left: 0;
 
           p {
@@ -61,25 +67,24 @@
 
             &.active {
               background-color: var(--focus-color);
 
               &:not(.has-children) {
                 border-top: 1px solid var(--separator-color);
                 border-bottom: 1px solid var(--separator-color);
-                border-left: .2rem solid var(--primary-color-dark);
+                border-left: 0.2rem solid var(--primary-color-dark);
               }
             }
           }
         }
       }
     }
   }
 }
 
-
 aside.stm-sidenav {
   label.toctree-toggle {
     position: absolute;
     top: 0;
     margin-top: 4px;
     right: 0;
     height: 30px;
@@ -115,51 +120,49 @@
     }
   }
 
   li {
     position: relative;
 
     &.has-children {
-      >.reference {
+      > .reference {
         padding-right: 30px;
       }
 
-      >ul {
+      > ul {
         background-color: var(--background-color-sidenav);
         padding: 0 0 0 1rem;
       }
     }
   }
 
   .toctree-checkbox {
     position: absolute;
     display: none;
 
-    ~ul {
+    ~ ul {
       display: none;
     }
 
-    ~label i {
+    ~ label i {
       transform: rotate(0deg);
     }
   }
 
   .toctree-checkbox:checked {
-    ~ul {
+    ~ ul {
       display: block;
     }
 
-    ~label i {
+    ~ label i {
       transform: rotate(180deg);
     }
   }
 }
 
-
-
 .sidenav-header-items {
   display: flex;
   flex-direction: column;
   padding: 0 0 0 var(--header-horizontal-spacing);
 }
 
 .sidenav-header-items__center {
```

### Comparing `stmaterial-0.0.6/src/stmaterial/assets/styles/variables/_admonitions.scss` & `stmaterial-0.0.7/src/stmaterial/assets/styles/variables/_admonitions.scss`

 * *Files 7% similar despite different names*

```diff
@@ -34,19 +34,15 @@
   --color-topic-title: #{$color};
   --color-topic-title-background: #{rgba($color, 0.2)};
 
   --icon-topic-default: var(--icon-#{$icon-name});
 }
 
 @mixin admonitions {
-
-  @each $name,
-  $values in $admonitions {
+  @each $name, $values in $admonitions {
     --color-admonition-title--#{$name}: #{nth($values, 1)};
     --color-admonition-title-background--#{$name}: #{rgba(
- nth($values, 1),
-    0.2)
+        nth($values, 1),
+        0.2
+      )};
   }
-
-  ;
 }
-}
```

### Comparing `stmaterial-0.0.6/src/stmaterial/assets/styles/variables/_colors.scss` & `stmaterial-0.0.7/src/stmaterial/assets/styles/variables/_colors.scss`

 * *Files 2% similar despite different names*

```diff
@@ -7,32 +7,32 @@
 // `colors-dark` depends on `colors` being included at a lower specificity.
 
 @mixin colors {
   // primary and secondary color
   --primary-color: #26a69a;
   --primary-color-dark: #009688;
   --primary-color-numeric: 38, 166, 154;
-  --primary-color-raised-hover-solid: #30B0A4;
-  --primary-color-raised-focus-solid: #44C4B8;
+  --primary-color-raised-hover-solid: #30b0a4;
+  --primary-color-raised-focus-solid: #44c4b8;
   --primary-color-font-medium-color: rgba(var(--primary-color-numeric), 0.7);
   --primary-color-font-disabled-color: rgba(var(--primary-color-numeric), 0.4);
   --primary-color-hover-opaque: rgba(var(--primary-color-numeric), 0.06);
   --primary-color-focus-opaque: rgba(var(--primary-color-numeric), 0.18);
-  --secondary-color: #EF5350;
-  --secondary-color-hover-solid: #FE625F;
-  --secondary-color-focus-solid: #FF7B78;
+  --secondary-color: #ef5350;
+  --secondary-color-hover-solid: #fe625f;
+  --secondary-color-focus-solid: #ff7b78;
 
   // font related color
   --font-color-main: rgba(0, 0, 0, 0.87);
   --font-color-medium: rgba(0, 0, 0, 0.56);
   --font-color-disabled: rgba(0, 0, 0, 0.38);
   --font-on-primary-color-main: rgba(255, 255, 255, 0.87);
   --font-on-primary-color-dark-main: rgba(255, 255, 255, 0.87);
-  --font-on-primary-color-dark-medium: rgba(255, 255, 255, 0.60);
-  --font-on-primary-color-medium: rgba(255, 255, 255, 0.60);
+  --font-on-primary-color-dark-medium: rgba(255, 255, 255, 0.6);
+  --font-on-primary-color-medium: rgba(255, 255, 255, 0.6);
   --font-on-primary-color-disabled: rgba(255, 255, 255, 0.38);
   --font-on-secondary-color-main: rgba(0, 0, 0, 0.87);
 
   // background color
   --surface-color: #eeeeee;
   --background-color: #ffffff;
   --background-color-sidenav: aliceblue;
@@ -41,23 +41,23 @@
   --background-color-level-16dp-solid: var(--surface-color);
   --background-color-slight-emphasis: rgba(0, 0, 0, 0.025);
   --background-color-card: var(--surface-color);
 
   // others color
   --hover-color: rgba(0, 0, 0, 0.04);
   --focus-color: rgba(0, 0, 0, 0.12);
-  --focus-color-solid: #E0E0E0;
+  --focus-color-solid: #e0e0e0;
   --tooltip-background-color: #313033;
   --tooltip-font-color: rgba(255, 255, 255, 0.77);
-  --separator-color: #DDDDDD;
-  --error-color: #F44336;
+  --separator-color: #dddddd;
+  --error-color: #f44336;
   --slider-track-color: rgba(0, 0, 0, 0.26);
   --switch-thumb-off-color: #ffffff;
   --carousel-indicator-color: rgba(255, 255, 255, 0.45);
-  --carousel-indicator-active-color: #FFF;
+  --carousel-indicator-active-color: #fff;
   --md_sys_color_on-surface: 28, 27, 31;
 
   //dependent variables
   --color-highlighted-background: var(--focus-color);
   --color-highlighted-text: var(--secondary-color-focus-solid);
   --button-raised-background-hover: var(--primary-color-raised-hover-solid);
 
@@ -85,29 +85,29 @@
   --dropdown-color: var(--primary-color);
 
   --input-focus-color: var(--secondary-color-focus-solid);
 }
 
 @mixin colors-dark {
   // primary and secondary color
-  --primary-color: #B39DDB;
-  --primary-color-dark: #9575CD;
+  --primary-color: #b39ddb;
+  --primary-color-dark: #9575cd;
   --primary-color-numeric: 179, 157, 219;
-  --primary-color-raised-hover-solid: #C2ACEA;
-  --primary-color-raised-focus-solid: #DBC5FF;
-  --secondary-color: #CDDC39;
-  --secondary-color-hover-solid: #DCEB48;
-  --secondary-color-focus-solid: #F5FF61;
+  --primary-color-raised-hover-solid: #c2acea;
+  --primary-color-raised-focus-solid: #dbc5ff;
+  --secondary-color: #cddc39;
+  --secondary-color-hover-solid: #dceb48;
+  --secondary-color-focus-solid: #f5ff61;
   // font related color
   --font-color-main: rgba(255, 255, 255, 0.87);
-  --font-color-medium: rgba(255, 255, 255, 0.60);
+  --font-color-medium: rgba(255, 255, 255, 0.6);
   --font-color-disabled: rgba(255, 255, 255, 0.38);
   --font-on-primary-color-main: rgba(0, 0, 0, 0.87);
   --font-on-primary-color-dark-main: rgba(255, 255, 255, 0.87);
-  --font-on-primary-color-dark-medium: rgba(255, 255, 255, 0.60);
+  --font-on-primary-color-dark-medium: rgba(255, 255, 255, 0.6);
   --font-on-primary-color-medium: rgba(0, 0, 0, 0.56);
   --font-on-primary-color-disabled: rgba(0, 0, 0, 0.38);
 
   // background color
   --surface-color: #242424;
   --background-color: #121212;
   --background-color-sidenav: #121212;
@@ -118,20 +118,19 @@
   --background-color-slight-emphasis: rgba(255, 255, 255, 0.05);
 
   // others color
   --hover-color: rgba(255, 255, 255, 0.04);
   --focus-color: rgba(255, 255, 255, 0.12);
   --focus-color-solid: #424242;
   --separator-color: #424242;
-  --error-color: #CF6679;
+  --error-color: #cf6679;
   --slider-track-color: rgba(255, 255, 255, 0.26);
   --switch-thumb-off-color: #bababa;
   --md_sys_color_on-surface: 230, 225, 229;
 
-
   //tmp definition
   --color-highlighted-background: var(--focus-color);
   --color-highlighted-text: var(--secondary-color-focus-solid);
 
   // colors from furo
   --color-background-hover: #1e2124ff;
   --color-problematic: #ee5151;
```

### Comparing `stmaterial-0.0.6/src/stmaterial/assets/styles/variables/_icons.scss` & `stmaterial-0.0.7/src/stmaterial/assets/styles/variables/_icons.scss`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,32 @@
 // Expose theme icons as CSS variables.
 
 $icons: (
   // Adapted from tabler-icons
   //    url: https://tablericons.com/
-  "search": url('data:image/svg+xml;charset=utf-8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" fill="none" stroke-linecap="round" stroke-linejoin="round"><path stroke="none" d="M0 0h24v24H0z"/><circle cx="10" cy="10" r="7" /><line x1="21" y1="21" x2="15" y2="15" /></svg>'),
+  "search":
+    url('data:image/svg+xml;charset=utf-8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" fill="none" stroke-linecap="round" stroke-linejoin="round"><path stroke="none" d="M0 0h24v24H0z"/><circle cx="10" cy="10" r="7" /><line x1="21" y1="21" x2="15" y2="15" /></svg>'),
   // Factored out from mkdocs-material on 24-Aug-2020.
   //    url: https://squidfunk.github.io/mkdocs-material/reference/admonitions/
-  "pencil": url('data:image/svg+xml;charset=utf-8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M20.71 7.04c.39-.39.39-1.04 0-1.41l-2.34-2.34c-.37-.39-1.02-.39-1.41 0l-1.84 1.83 3.75 3.75M3 17.25V21h3.75L17.81 9.93l-3.75-3.75L3 17.25z"/></svg>'),
-  "abstract": url('data:image/svg+xml;charset=utf-8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M4 5h16v2H4V5m0 4h16v2H4V9m0 4h16v2H4v-2m0 4h10v2H4v-2z"/></svg>'),
-  "info": url('data:image/svg+xml;charset=utf-8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M13 9h-2V7h2m0 10h-2v-6h2m-1-9A10 10 0 002 12a10 10 0 0010 10 10 10 0 0010-10A10 10 0 0012 2z"/></svg>'),
-  "flame": url('data:image/svg+xml;charset=utf-8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M17.55 11.2c-.23-.3-.5-.56-.76-.82-.65-.6-1.4-1.03-2.03-1.66C13.3 7.26 13 4.85 13.91 3c-.91.23-1.75.75-2.45 1.32-2.54 2.08-3.54 5.75-2.34 8.9.04.1.08.2.08.33 0 .22-.15.42-.35.5-.22.1-.46.04-.64-.12a.83.83 0 01-.15-.17c-1.1-1.43-1.28-3.48-.53-5.12C5.89 10 5 12.3 5.14 14.47c.04.5.1 1 .27 1.5.14.6.4 1.2.72 1.73 1.04 1.73 2.87 2.97 4.84 3.22 2.1.27 4.35-.12 5.96-1.6 1.8-1.66 2.45-4.32 1.5-6.6l-.13-.26c-.2-.46-.47-.87-.8-1.25l.05-.01m-3.1 6.3c-.28.24-.73.5-1.08.6-1.1.4-2.2-.16-2.87-.82 1.19-.28 1.89-1.16 2.09-2.05.17-.8-.14-1.46-.27-2.23-.12-.74-.1-1.37.18-2.06.17.38.37.76.6 1.06.76 1 1.95 1.44 2.2 2.8.04.14.06.28.06.43.03.82-.32 1.72-.92 2.27h.01z"/></svg>'),
-  "question": url('data:image/svg+xml;charset=utf-8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M15.07 11.25l-.9.92C13.45 12.89 13 13.5 13 15h-2v-.5c0-1.11.45-2.11 1.17-2.83l1.24-1.26c.37-.36.59-.86.59-1.41a2 2 0 00-2-2 2 2 0 00-2 2H8a4 4 0 014-4 4 4 0 014 4 3.2 3.2 0 01-.93 2.25M13 19h-2v-2h2M12 2A10 10 0 002 12a10 10 0 0010 10 10 10 0 0010-10c0-5.53-4.5-10-10-10z"/></svg>'),
-  "warning": url('data:image/svg+xml;charset=utf-8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M13 14h-2v-4h2m0 8h-2v-2h2M1 21h22L12 2 1 21z"/></svg>'),
-  "failure": url('data:image/svg+xml;charset=utf-8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M12 2c5.53 0 10 4.47 10 10s-4.47 10-10 10S2 17.53 2 12 6.47 2 12 2m3.59 5L12 10.59 8.41 7 7 8.41 10.59 12 7 15.59 8.41 17 12 13.41 15.59 17 17 15.59 13.41 12 17 8.41 15.59 7z"/></svg>'),
-  "spark": url('data:image/svg+xml;charset=utf-8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M11.5 20l4.86-9.73H13V4l-5 9.73h3.5V20M12 2c2.75 0 5.1 1 7.05 2.95C21 6.9 22 9.25 22 12s-1 5.1-2.95 7.05C17.1 21 14.75 22 12 22s-5.1-1-7.05-2.95C3 17.1 2 14.75 2 12s1-5.1 2.95-7.05C6.9 3 9.25 2 12 2z"/></svg>')
+  "pencil":
+    url('data:image/svg+xml;charset=utf-8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M20.71 7.04c.39-.39.39-1.04 0-1.41l-2.34-2.34c-.37-.39-1.02-.39-1.41 0l-1.84 1.83 3.75 3.75M3 17.25V21h3.75L17.81 9.93l-3.75-3.75L3 17.25z"/></svg>'),
+  "abstract":
+    url('data:image/svg+xml;charset=utf-8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M4 5h16v2H4V5m0 4h16v2H4V9m0 4h16v2H4v-2m0 4h10v2H4v-2z"/></svg>'),
+  "info":
+    url('data:image/svg+xml;charset=utf-8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M13 9h-2V7h2m0 10h-2v-6h2m-1-9A10 10 0 002 12a10 10 0 0010 10 10 10 0 0010-10A10 10 0 0012 2z"/></svg>'),
+  "flame":
+    url('data:image/svg+xml;charset=utf-8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M17.55 11.2c-.23-.3-.5-.56-.76-.82-.65-.6-1.4-1.03-2.03-1.66C13.3 7.26 13 4.85 13.91 3c-.91.23-1.75.75-2.45 1.32-2.54 2.08-3.54 5.75-2.34 8.9.04.1.08.2.08.33 0 .22-.15.42-.35.5-.22.1-.46.04-.64-.12a.83.83 0 01-.15-.17c-1.1-1.43-1.28-3.48-.53-5.12C5.89 10 5 12.3 5.14 14.47c.04.5.1 1 .27 1.5.14.6.4 1.2.72 1.73 1.04 1.73 2.87 2.97 4.84 3.22 2.1.27 4.35-.12 5.96-1.6 1.8-1.66 2.45-4.32 1.5-6.6l-.13-.26c-.2-.46-.47-.87-.8-1.25l.05-.01m-3.1 6.3c-.28.24-.73.5-1.08.6-1.1.4-2.2-.16-2.87-.82 1.19-.28 1.89-1.16 2.09-2.05.17-.8-.14-1.46-.27-2.23-.12-.74-.1-1.37.18-2.06.17.38.37.76.6 1.06.76 1 1.95 1.44 2.2 2.8.04.14.06.28.06.43.03.82-.32 1.72-.92 2.27h.01z"/></svg>'),
+  "question":
+    url('data:image/svg+xml;charset=utf-8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M15.07 11.25l-.9.92C13.45 12.89 13 13.5 13 15h-2v-.5c0-1.11.45-2.11 1.17-2.83l1.24-1.26c.37-.36.59-.86.59-1.41a2 2 0 00-2-2 2 2 0 00-2 2H8a4 4 0 014-4 4 4 0 014 4 3.2 3.2 0 01-.93 2.25M13 19h-2v-2h2M12 2A10 10 0 002 12a10 10 0 0010 10 10 10 0 0010-10c0-5.53-4.5-10-10-10z"/></svg>'),
+  "warning":
+    url('data:image/svg+xml;charset=utf-8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M13 14h-2v-4h2m0 8h-2v-2h2M1 21h22L12 2 1 21z"/></svg>'),
+  "failure":
+    url('data:image/svg+xml;charset=utf-8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M12 2c5.53 0 10 4.47 10 10s-4.47 10-10 10S2 17.53 2 12 6.47 2 12 2m3.59 5L12 10.59 8.41 7 7 8.41 10.59 12 7 15.59 8.41 17 12 13.41 15.59 17 17 15.59 13.41 12 17 8.41 15.59 7z"/></svg>'),
+  "spark":
+    url('data:image/svg+xml;charset=utf-8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M11.5 20l4.86-9.73H13V4l-5 9.73h3.5V20M12 2c2.75 0 5.1 1 7.05 2.95C21 6.9 22 9.25 22 12s-1 5.1-2.95 7.05C17.1 21 14.75 22 12 22s-5.1-1-7.05-2.95C3 17.1 2 14.75 2 12s1-5.1 2.95-7.05C6.9 3 9.25 2 12 2z"/></svg>')
 );
 
 @mixin icons {
-
-  @each $name,
-  $glyph in $icons {
+  @each $name, $glyph in $icons {
     --icon-#{$name}: #{$glyph};
   }
-}
+}
```

### Comparing `stmaterial-0.0.6/src/stmaterial/assets/translations/README.md` & `stmaterial-0.0.7/src/stmaterial/assets/translations/README.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.6/src/stmaterial/assets/translations/jsons/Edit this page.json` & `stmaterial-0.0.7/src/stmaterial/assets/translations/jsons/Edit this page.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 22% similar despite different names*

```diff
@@ -1,336 +1,290 @@
-00000000: 5b0a 2020 2020 7b0a 2020 2020 2020 2020  [.    {.        
-00000010: 226c 616e 6775 6167 6522 3a20 2245 6e67  "language": "Eng
-00000020: 6c69 7368 222c 0a20 2020 2020 2020 2022  lish",.        "
-00000030: 7379 6d62 6f6c 223a 2022 656e 222c 0a20  symbol": "en",. 
-00000040: 2020 2020 2020 2022 7465 7874 223a 2022         "text": "
-00000050: 4564 6974 2074 6869 7320 7061 6765 220a  Edit this page".
-00000060: 2020 2020 7d2c 0a20 2020 207b 0a20 2020      },.    {.   
-00000070: 2020 2020 2022 6c61 6e67 7561 6765 223a       "language":
-00000080: 2022 4172 6162 6963 222c 0a20 2020 2020   "Arabic",.     
-00000090: 2020 2022 7379 6d62 6f6c 223a 2022 6172     "symbol": "ar
-000000a0: 222c 0a20 2020 2020 2020 2022 7465 7874  ",.        "text
-000000b0: 223a 2022 d982 d985 20d8 a8d8 aad8 add8  ": ".... .......
-000000c0: b1d9 8ad8 b120 d987 d8b0 d987 20d8 a7d9  ..... ...... ...
-000000d0: 84d8 b5d9 81d8 add8 a922 0a20 2020 207d  .........".    }
-000000e0: 2c0a 2020 2020 7b0a 2020 2020 2020 2020  ,.    {.        
-000000f0: 226c 616e 6775 6167 6522 3a20 2242 756c  "language": "Bul
-00000100: 6761 7269 616e 222c 0a20 2020 2020 2020  garian",.       
-00000110: 2022 7379 6d62 6f6c 223a 2022 6267 222c   "symbol": "bg",
-00000120: 0a20 2020 2020 2020 2022 7465 7874 223a  .        "text":
-00000130: 2022 d0a0 d0b5 d0b4 d0b0 d0ba d182 d0b8   "..............
-00000140: d180 d0b0 d0b9 d182 d0b5 20d1 82d0 b0d0  .......... .....
-00000150: b7d0 b820 d181 d182 d180 d0b0 d0bd d0b8  ... ............
-00000160: d186 d0b0 220a 2020 2020 7d2c 0a20 2020  ....".    },.   
-00000170: 207b 0a20 2020 2020 2020 2022 6c61 6e67   {.        "lang
-00000180: 7561 6765 223a 2022 4368 696e 6573 6520  uage": "Chinese 
-00000190: 5369 6d70 6c69 6669 6564 222c 0a20 2020  Simplified",.   
-000001a0: 2020 2020 2022 7379 6d62 6f6c 223a 2022       "symbol": "
-000001b0: 7a68 5f43 4e22 2c0a 2020 2020 2020 2020  zh_CN",.        
-000001c0: 2274 6578 7422 3a20 22e7 bc96 e8be 91e6  "text": ".......
-000001d0: ada4 e9a1 b5e9 9da2 220a 2020 2020 7d2c  ........".    },
-000001e0: 0a20 2020 207b 0a20 2020 2020 2020 2022  .    {.        "
-000001f0: 6c61 6e67 7561 6765 223a 2022 4368 696e  language": "Chin
-00000200: 6573 6520 5472 6164 6974 696f 6e61 6c22  ese Traditional"
-00000210: 2c0a 2020 2020 2020 2020 2273 796d 626f  ,.        "symbo
-00000220: 6c22 3a20 227a 682d 7477 222c 0a20 2020  l": "zh-tw",.   
-00000230: 2020 2020 2022 7465 7874 223a 2022 e7b7       "text": "..
-00000240: a8e8 bcaf e6ad a4e9 a081 e99d a222 0a20  .............". 
-00000250: 2020 207d 2c0a 2020 2020 7b0a 2020 2020     },.    {.    
-00000260: 2020 2020 226c 616e 6775 6167 6522 3a20      "language": 
-00000270: 2243 726f 6174 6961 6e22 2c0a 2020 2020  "Croatian",.    
-00000280: 2020 2020 2273 796d 626f 6c22 3a20 2268      "symbol": "h
-00000290: 7222 2c0a 2020 2020 2020 2020 2274 6578  r",.        "tex
-000002a0: 7422 3a20 2255 7265 6469 7465 206f 7675  t": "Uredite ovu
-000002b0: 2073 7472 616e 6963 7522 0a20 2020 207d   stranicu".    }
-000002c0: 2c0a 2020 2020 7b0a 2020 2020 2020 2020  ,.    {.        
-000002d0: 226c 616e 6775 6167 6522 3a20 2243 7a65  "language": "Cze
-000002e0: 6368 222c 0a20 2020 2020 2020 2022 7379  ch",.        "sy
-000002f0: 6d62 6f6c 223a 2022 6373 222c 0a20 2020  mbol": "cs",.   
-00000300: 2020 2020 2022 7465 7874 223a 2022 5570       "text": "Up
-00000310: 7261 7669 7420 7475 746f 2073 7472 c3a1  ravit tuto str..
-00000320: 6e6b 7522 0a20 2020 207d 2c0a 2020 2020  nku".    },.    
-00000330: 7b0a 2020 2020 2020 2020 226c 616e 6775  {.        "langu
-00000340: 6167 6522 3a20 2244 616e 6973 6822 2c0a  age": "Danish",.
-00000350: 2020 2020 2020 2020 2273 796d 626f 6c22          "symbol"
-00000360: 3a20 2264 6122 2c0a 2020 2020 2020 2020  : "da",.        
-00000370: 2274 6578 7422 3a20 2252 6564 6967 6572  "text": "Rediger
-00000380: 2064 656e 6e65 2073 6964 6522 0a20 2020   denne side".   
-00000390: 207d 2c0a 2020 2020 7b0a 2020 2020 2020   },.    {.      
-000003a0: 2020 226c 616e 6775 6167 6522 3a20 2244    "language": "D
-000003b0: 7574 6368 222c 0a20 2020 2020 2020 2022  utch",.        "
-000003c0: 7379 6d62 6f6c 223a 2022 6e6c 222c 0a20  symbol": "nl",. 
-000003d0: 2020 2020 2020 2022 7465 7874 223a 2022         "text": "
-000003e0: 6265 7765 726b 2064 657a 6520 7061 6769  bewerk deze pagi
-000003f0: 6e61 220a 2020 2020 7d2c 0a20 2020 207b  na".    },.    {
-00000400: 0a20 2020 2020 2020 2022 6c61 6e67 7561  .        "langua
-00000410: 6765 223a 2022 4573 7065 7261 6e74 6f22  ge": "Esperanto"
-00000420: 2c0a 2020 2020 2020 2020 2273 796d 626f  ,.        "symbo
-00000430: 6c22 3a20 2265 6f22 2c0a 2020 2020 2020  l": "eo",.      
-00000440: 2020 2274 6578 7422 3a20 2252 6564 616b    "text": "Redak
-00000450: 7475 20c4 8969 2074 6975 6e20 7061 c49d  tu ..i tiun pa..
-00000460: 6f6e 220a 2020 2020 7d2c 0a20 2020 207b  on".    },.    {
-00000470: 0a20 2020 2020 2020 2022 6c61 6e67 7561  .        "langua
-00000480: 6765 223a 2022 4573 746f 6e69 616e 222c  ge": "Estonian",
-00000490: 0a20 2020 2020 2020 2022 7379 6d62 6f6c  .        "symbol
-000004a0: 223a 2022 6574 222c 0a20 2020 2020 2020  ": "et",.       
-000004b0: 2022 7465 7874 223a 2022 4d75 7574 6b65   "text": "Muutke
-000004c0: 2073 6564 6120 6c65 6874 6522 0a20 2020   seda lehte".   
-000004d0: 207d 2c0a 2020 2020 7b0a 2020 2020 2020   },.    {.      
-000004e0: 2020 226c 616e 6775 6167 6522 3a20 2246    "language": "F
-000004f0: 696e 6e69 7368 222c 0a20 2020 2020 2020  innish",.       
-00000500: 2022 7379 6d62 6f6c 223a 2022 6669 222c   "symbol": "fi",
-00000510: 0a20 2020 2020 2020 2022 7465 7874 223a  .        "text":
-00000520: 2022 4d75 6f6b 6b61 6120 74c3 a474 c3a4   "Muokkaa t..t..
-00000530: 2073 6976 7561 220a 2020 2020 7d2c 0a20   sivua".    },. 
-00000540: 2020 207b 0a20 2020 2020 2020 2022 6c61     {.        "la
-00000550: 6e67 7561 6765 223a 2022 4672 656e 6368  nguage": "French
-00000560: 222c 0a20 2020 2020 2020 2022 7379 6d62  ",.        "symb
-00000570: 6f6c 223a 2022 6672 222c 0a20 2020 2020  ol": "fr",.     
-00000580: 2020 2022 7465 7874 223a 2022 4d6f 6469     "text": "Modi
-00000590: 6669 6572 2063 6574 7465 2070 6167 6522  fier cette page"
-000005a0: 0a20 2020 207d 2c0a 2020 2020 7b0a 2020  .    },.    {.  
-000005b0: 2020 2020 2020 226c 616e 6775 6167 6522        "language"
-000005c0: 3a20 2247 6572 6d61 6e22 2c0a 2020 2020  : "German",.    
-000005d0: 2020 2020 2273 796d 626f 6c22 3a20 2264      "symbol": "d
-000005e0: 6522 2c0a 2020 2020 2020 2020 2274 6578  e",.        "tex
-000005f0: 7422 3a20 2242 6561 7262 6569 7465 2064  t": "Bearbeite d
-00000600: 6965 7365 2053 6569 7465 220a 2020 2020  iese Seite".    
-00000610: 7d2c 0a20 2020 207b 0a20 2020 2020 2020  },.    {.       
-00000620: 2022 6c61 6e67 7561 6765 223a 2022 4772   "language": "Gr
-00000630: 6565 6b22 2c0a 2020 2020 2020 2020 2273  eek",.        "s
-00000640: 796d 626f 6c22 3a20 2265 6c22 2c0a 2020  ymbol": "el",.  
-00000650: 2020 2020 2020 2274 6578 7422 3a20 22ce        "text": ".
-00000660: 95cf 80ce b5ce bece b5cf 81ce b3ce b1cf  ................
-00000670: 83cf 84ce b5ce afcf 84ce b520 ceb1 cf85  ........... ....
-00000680: cf84 ceae cebd 20cf 84ce b720 cf83 ceb5  ...... .... ....
-00000690: cebb ceaf ceb4 ceb1 220a 2020 2020 7d2c  ........".    },
-000006a0: 0a20 2020 207b 0a20 2020 2020 2020 2022  .    {.        "
-000006b0: 6c61 6e67 7561 6765 223a 2022 4865 6272  language": "Hebr
-000006c0: 6577 222c 0a20 2020 2020 2020 2022 7379  ew",.        "sy
-000006d0: 6d62 6f6c 223a 2022 6977 222c 0a20 2020  mbol": "iw",.   
-000006e0: 2020 2020 2022 7465 7874 223a 2022 d7a2       "text": "..
-000006f0: d7a8 d795 d79a 20d7 93d7 a320 d796 d794  ...... .... ....
-00000700: 220a 2020 2020 7d2c 0a20 2020 207b 0a20  ".    },.    {. 
-00000710: 2020 2020 2020 2022 6c61 6e67 7561 6765         "language
-00000720: 223a 2022 496e 646f 6e65 7369 616e 222c  ": "Indonesian",
-00000730: 0a20 2020 2020 2020 2022 7379 6d62 6f6c  .        "symbol
-00000740: 223a 2022 6964 222c 0a20 2020 2020 2020  ": "id",.       
-00000750: 2022 7465 7874 223a 2022 4564 6974 2068   "text": "Edit h
-00000760: 616c 616d 616e 2069 6e69 220a 2020 2020  alaman ini".    
-00000770: 7d2c 0a20 2020 207b 0a20 2020 2020 2020  },.    {.       
-00000780: 2022 6c61 6e67 7561 6765 223a 2022 4974   "language": "It
-00000790: 616c 6961 6e22 2c0a 2020 2020 2020 2020  alian",.        
-000007a0: 2273 796d 626f 6c22 3a20 2269 7422 2c0a  "symbol": "it",.
-000007b0: 2020 2020 2020 2020 2274 6578 7422 3a20          "text": 
-000007c0: 224d 6f64 6966 6963 6120 7175 6573 7461  "Modifica questa
-000007d0: 2070 6167 696e 6122 0a20 2020 207d 2c0a   pagina".    },.
-000007e0: 2020 2020 7b0a 2020 2020 2020 2020 226c      {.        "l
-000007f0: 616e 6775 6167 6522 3a20 224a 6170 616e  anguage": "Japan
-00000800: 6573 6522 2c0a 2020 2020 2020 2020 2273  ese",.        "s
-00000810: 796d 626f 6c22 3a20 226a 6122 2c0a 2020  ymbol": "ja",.  
-00000820: 2020 2020 2020 2274 6578 7422 3a20 22e3        "text": ".
-00000830: 8193 e381 aee3 839a e383 bce3 82b8 e382  ................
-00000840: 92e7 b7a8 e99b 8622 0a20 2020 207d 2c0a  .......".    },.
-00000850: 2020 2020 7b0a 2020 2020 2020 2020 226c      {.        "l
-00000860: 616e 6775 6167 6522 3a20 224b 6f72 6561  anguage": "Korea
-00000870: 6e22 2c0a 2020 2020 2020 2020 2273 796d  n",.        "sym
-00000880: 626f 6c22 3a20 226b 6f22 2c0a 2020 2020  bol": "ko",.    
-00000890: 2020 2020 2274 6578 7422 3a20 22ec 9db4      "text": "...
-000008a0: 20ed 8e98 ec9d b4ec a780 20ed 8eb8 eca7   ......... .....
-000008b0: 9122 0a20 2020 207d 2c0a 2020 2020 7b0a  .".    },.    {.
-000008c0: 2020 2020 2020 2020 226c 616e 6775 6167          "languag
-000008d0: 6522 3a20 224c 6174 7669 616e 222c 0a20  e": "Latvian",. 
-000008e0: 2020 2020 2020 2022 7379 6d62 6f6c 223a         "symbol":
-000008f0: 2022 6c76 222c 0a20 2020 2020 2020 2022   "lv",.        "
-00000900: 7465 7874 223a 2022 5265 6469 c4a3 c493  text": "Redi....
-00000910: 7420 c5a1 6f20 6c61 7075 220a 2020 2020  t ..o lapu".    
-00000920: 7d2c 0a20 2020 207b 0a20 2020 2020 2020  },.    {.       
-00000930: 2022 6c61 6e67 7561 6765 223a 2022 4c69   "language": "Li
-00000940: 7468 7561 6e69 616e 222c 0a20 2020 2020  thuanian",.     
-00000950: 2020 2022 7379 6d62 6f6c 223a 2022 6c74     "symbol": "lt
-00000960: 222c 0a20 2020 2020 2020 2022 7465 7874  ",.        "text
-00000970: 223a 2022 5265 6461 6775 6f74 6920 c5a1  ": "Redaguoti ..
-00000980: c4af 2070 7573 6c61 70c4 af22 0a20 2020  .. puslap..".   
-00000990: 207d 2c0a 2020 2020 7b0a 2020 2020 2020   },.    {.      
-000009a0: 2020 226c 616e 6775 6167 6522 3a20 224e    "language": "N
-000009b0: 6f72 7765 6769 616e 222c 0a20 2020 2020  orwegian",.     
-000009c0: 2020 2022 7379 6d62 6f6c 223a 2022 6e6f     "symbol": "no
-000009d0: 222c 0a20 2020 2020 2020 2022 7465 7874  ",.        "text
-000009e0: 223a 2022 5265 6469 6765 7220 6465 6e6e  ": "Rediger denn
-000009f0: 6520 7369 6465 6e22 0a20 2020 207d 2c0a  e siden".    },.
-00000a00: 2020 2020 7b0a 2020 2020 2020 2020 226c      {.        "l
-00000a10: 616e 6775 6167 6522 3a20 2250 6f6c 6973  anguage": "Polis
-00000a20: 6822 2c0a 2020 2020 2020 2020 2273 796d  h",.        "sym
-00000a30: 626f 6c22 3a20 2270 6c22 2c0a 2020 2020  bol": "pl",.    
-00000a40: 2020 2020 2274 6578 7422 3a20 2245 6479      "text": "Edy
-00000a50: 7475 6a20 74c4 9920 7374 726f 6e65 220a  tuj t.. strone".
-00000a60: 2020 2020 7d2c 0a20 2020 207b 0a20 2020      },.    {.   
-00000a70: 2020 2020 2022 6c61 6e67 7561 6765 223a       "language":
-00000a80: 2022 506f 7274 7567 7565 7365 222c 0a20   "Portuguese",. 
-00000a90: 2020 2020 2020 2022 7379 6d62 6f6c 223a         "symbol":
-00000aa0: 2022 7074 222c 0a20 2020 2020 2020 2022   "pt",.        "
-00000ab0: 7465 7874 223a 2022 4564 6974 6520 6573  text": "Edite es
-00000ac0: 7361 2070 c3a1 6769 6e61 220a 2020 2020  sa p..gina".    
-00000ad0: 7d2c 0a20 2020 207b 0a20 2020 2020 2020  },.    {.       
-00000ae0: 2022 6c61 6e67 7561 6765 223a 2022 526f   "language": "Ro
-00000af0: 6d61 6e69 616e 222c 0a20 2020 2020 2020  manian",.       
-00000b00: 2022 7379 6d62 6f6c 223a 2022 726f 222c   "symbol": "ro",
-00000b10: 0a20 2020 2020 2020 2022 7465 7874 223a  .        "text":
-00000b20: 2022 4564 6974 61c8 9b69 2061 6365 6173   "Edita..i aceas
-00000b30: 74c4 8320 7061 6769 6ec4 8322 0a20 2020  t.. pagin..".   
-00000b40: 207d 2c0a 2020 2020 7b0a 2020 2020 2020   },.    {.      
-00000b50: 2020 226c 616e 6775 6167 6522 3a20 2252    "language": "R
-00000b60: 7573 7369 616e 222c 0a20 2020 2020 2020  ussian",.       
-00000b70: 2022 7379 6d62 6f6c 223a 2022 7275 222c   "symbol": "ru",
-00000b80: 0a20 2020 2020 2020 2022 7465 7874 223a  .        "text":
-00000b90: 2022 d0a0 d0b5 d0b4 d0b0 d0ba d182 d0b8   "..............
-00000ba0: d180 d0be d0b2 d0b0 d182 d18c 20d1 8dd1  ............ ...
-00000bb0: 82d1 8320 d181 d182 d180 d0b0 d0bd d0b8  ... ............
-00000bc0: d186 d183 220a 2020 2020 7d2c 0a20 2020  ....".    },.   
-00000bd0: 207b 0a20 2020 2020 2020 2022 6c61 6e67   {.        "lang
-00000be0: 7561 6765 223a 2022 5365 7262 6961 6e22  uage": "Serbian"
-00000bf0: 2c0a 2020 2020 2020 2020 2273 796d 626f  ,.        "symbo
-00000c00: 6c22 3a20 2273 7222 2c0a 2020 2020 2020  l": "sr",.      
-00000c10: 2020 2274 6578 7422 3a20 22d0 a3d1 80d0    "text": ".....
-00000c20: b5d0 b4d0 b8d1 82d0 b520 d0be d0b2 d183  ......... ......
-00000c30: 20d1 81d1 82d1 80d0 b0d0 bdd0 b8d1 86d1   ...............
-00000c40: 8322 0a20 2020 207d 2c0a 2020 2020 7b0a  .".    },.    {.
-00000c50: 2020 2020 2020 2020 226c 616e 6775 6167          "languag
-00000c60: 6522 3a20 2253 6c6f 7661 6b22 2c0a 2020  e": "Slovak",.  
-00000c70: 2020 2020 2020 2273 796d 626f 6c22 3a20        "symbol": 
-00000c80: 2273 6b22 2c0a 2020 2020 2020 2020 2274  "sk",.        "t
-00000c90: 6578 7422 3a20 2255 7072 6176 69c5 a520  ext": "Upravi.. 
-00000ca0: 74c3 ba74 6f20 7374 72c3 a16e 6b75 220a  t..to str..nku".
-00000cb0: 2020 2020 7d2c 0a20 2020 207b 0a20 2020      },.    {.   
-00000cc0: 2020 2020 2022 6c61 6e67 7561 6765 223a       "language":
-00000cd0: 2022 536c 6f76 656e 6961 6e22 2c0a 2020   "Slovenian",.  
-00000ce0: 2020 2020 2020 2273 796d 626f 6c22 3a20        "symbol": 
-00000cf0: 2273 6c22 2c0a 2020 2020 2020 2020 2274  "sl",.        "t
-00000d00: 6578 7422 3a20 2255 7265 6469 7465 2074  ext": "Uredite t
-00000d10: 6f20 7374 7261 6e22 0a20 2020 207d 2c0a  o stran".    },.
-00000d20: 2020 2020 7b0a 2020 2020 2020 2020 226c      {.        "l
-00000d30: 616e 6775 6167 6522 3a20 2253 7061 6e69  anguage": "Spani
-00000d40: 7368 222c 0a20 2020 2020 2020 2022 7379  sh",.        "sy
-00000d50: 6d62 6f6c 223a 2022 6573 222c 0a20 2020  mbol": "es",.   
-00000d60: 2020 2020 2022 7465 7874 223a 2022 4564       "text": "Ed
-00000d70: 6974 6120 6573 7461 2070 c3a1 6769 6e61  ita esta p..gina
-00000d80: 220a 2020 2020 7d2c 0a20 2020 207b 0a20  ".    },.    {. 
-00000d90: 2020 2020 2020 2022 6c61 6e67 7561 6765         "language
-00000da0: 223a 2022 5377 6564 6973 6822 2c0a 2020  ": "Swedish",.  
-00000db0: 2020 2020 2020 2273 796d 626f 6c22 3a20        "symbol": 
-00000dc0: 2273 7622 2c0a 2020 2020 2020 2020 2274  "sv",.        "t
-00000dd0: 6578 7422 3a20 2252 6564 6967 6572 6120  ext": "Redigera 
-00000de0: 6465 6e20 68c3 a472 2073 6964 616e 220a  den h..r sidan".
-00000df0: 2020 2020 7d2c 0a20 2020 207b 0a20 2020      },.    {.   
-00000e00: 2020 2020 2022 6c61 6e67 7561 6765 223a       "language":
-00000e10: 2022 5461 6a69 6b22 2c0a 2020 2020 2020   "Tajik",.      
-00000e20: 2020 2273 796d 626f 6c22 3a20 2274 6722    "symbol": "tg"
-00000e30: 2c0a 2020 2020 2020 2020 2274 6578 7422  ,.        "text"
-00000e40: 3a20 22d0 98d0 bd20 d181 d0b0 d2b3 d0b8  : ".... ........
-00000e50: d184 d0b0 d180 d0be 20d1 82d0 b0d2 b3d1  ........ .......
-00000e60: 80d0 b8d1 8020 d0ba d183 d0bd d0b5 d0b4  ..... ..........
-00000e70: 220a 2020 2020 7d2c 0a20 2020 207b 0a20  ".    },.    {. 
-00000e80: 2020 2020 2020 2022 6c61 6e67 7561 6765         "language
-00000e90: 223a 2022 5468 6169 222c 0a20 2020 2020  ": "Thai",.     
-00000ea0: 2020 2022 7379 6d62 6f6c 223a 2022 7468     "symbol": "th
-00000eb0: 222c 0a20 2020 2020 2020 2022 7465 7874  ",.        "text
-00000ec0: 223a 2022 e0b9 81e0 b881 e0b9 89e0 b984  ": "............
-00000ed0: e0b8 82e0 b8ab e0b8 99e0 b989 e0b8 b2e0  ................
-00000ee0: b899 e0b8 b5e0 b989 220a 2020 2020 7d2c  ........".    },
-00000ef0: 0a20 2020 207b 0a20 2020 2020 2020 2022  .    {.        "
-00000f00: 6c61 6e67 7561 6765 223a 2022 5475 726b  language": "Turk
-00000f10: 6973 6822 2c0a 2020 2020 2020 2020 2273  ish",.        "s
-00000f20: 796d 626f 6c22 3a20 2274 7222 2c0a 2020  ymbol": "tr",.  
-00000f30: 2020 2020 2020 2274 6578 7422 3a20 2242        "text": "B
-00000f40: 7520 7361 7966 6179 c4b1 2064 c3bc 7a65  u sayfay.. d..ze
-00000f50: 6e6c 6522 0a20 2020 207d 2c0a 2020 2020  nle".    },.    
-00000f60: 7b0a 2020 2020 2020 2020 226c 616e 6775  {.        "langu
-00000f70: 6167 6522 3a20 2255 6b72 6169 6e69 616e  age": "Ukrainian
-00000f80: 222c 0a20 2020 2020 2020 2022 7379 6d62  ",.        "symb
-00000f90: 6f6c 223a 2022 756b 222c 0a20 2020 2020  ol": "uk",.     
-00000fa0: 2020 2022 7465 7874 223a 2022 d0a0 d0b5     "text": "....
-00000fb0: d0b4 d0b0 d0b3 d183 d0b2 d0b0 d182 d0b8  ................
-00000fc0: 20d1 86d1 8e20 d181 d182 d0be d180 d196   .... ..........
-00000fd0: d0bd d0ba d183 220a 2020 2020 7d2c 0a20  ......".    },. 
-00000fe0: 2020 207b 0a20 2020 2020 2020 2022 6c61     {.        "la
-00000ff0: 6e67 7561 6765 223a 2022 5669 6574 6e61  nguage": "Vietna
-00001000: 6d65 7365 222c 0a20 2020 2020 2020 2022  mese",.        "
-00001010: 7379 6d62 6f6c 223a 2022 7669 222c 0a20  symbol": "vi",. 
-00001020: 2020 2020 2020 2022 7465 7874 223a 2022         "text": "
-00001030: 6368 e1bb 896e 6820 73e1 bbad 6120 7472  ch...nh s...a tr
-00001040: 616e 6720 6ec3 a079 220a 2020 2020 7d2c  ang n..y".    },
-00001050: 0a20 2020 207b 0a20 2020 2020 2020 2022  .    {.        "
-00001060: 6c61 6e67 7561 6765 223a 2022 4265 6e67  language": "Beng
-00001070: 616c 6922 2c0a 2020 2020 2020 2020 2273  ali",.        "s
-00001080: 796d 626f 6c22 3a20 2262 6e22 2c0a 2020  ymbol": "bn",.  
-00001090: 2020 2020 2020 2274 6578 7422 3a20 22e0        "text": ".
-000010a0: a68f e0a6 8720 e0a6 aae0 a783 e0a6 b7e0  ..... ..........
-000010b0: a78d e0a6 a0e0 a6be e0a6 9fe0 a6bf 20e0  .............. .
-000010c0: a6b8 e0a6 aee0 a78d e0a6 aae0 a6be e0a6  ................
-000010d0: a6e0 a6a8 e0a6 be20 e0a6 95e0 a6b0 e0a7  ....... ........
-000010e0: 81e0 a6a8 220a 2020 2020 7d2c 0a20 2020  ....".    },.   
-000010f0: 207b 0a20 2020 2020 2020 2022 6c61 6e67   {.        "lang
-00001100: 7561 6765 223a 2022 4669 6c69 7069 6e6f  uage": "Filipino
-00001110: 222c 0a20 2020 2020 2020 2022 7379 6d62  ",.        "symb
-00001120: 6f6c 223a 2022 746c 222c 0a20 2020 2020  ol": "tl",.     
-00001130: 2020 2022 7465 7874 223a 2022 492d 6564     "text": "I-ed
-00001140: 6974 2061 6e67 2070 6168 696e 616e 6720  it ang pahinang 
-00001150: 6974 6f22 0a20 2020 207d 2c0a 2020 2020  ito".    },.    
-00001160: 7b0a 2020 2020 2020 2020 226c 616e 6775  {.        "langu
-00001170: 6167 6522 3a20 224d 6172 6174 6869 222c  age": "Marathi",
-00001180: 0a20 2020 2020 2020 2022 7379 6d62 6f6c  .        "symbol
-00001190: 223a 2022 6d72 222c 0a20 2020 2020 2020  ": "mr",.       
-000011a0: 2022 7465 7874 223a 2022 e0a4 b9e0 a587   "text": "......
-000011b0: 20e0 a4aa e0a5 83e0 a4b7 e0a5 8de0 a4a0   ...............
-000011c0: 20e0 a4b8 e0a4 82e0 a4aa e0a4 bee0 a4a6   ...............
-000011d0: e0a4 bfe0 a4a4 20e0 a495 e0a4 b0e0 a4be  ...... .........
-000011e0: 220a 2020 2020 7d2c 0a20 2020 207b 0a20  ".    },.    {. 
-000011f0: 2020 2020 2020 2022 6c61 6e67 7561 6765         "language
-00001200: 223a 2022 4d61 6c61 7922 2c0a 2020 2020  ": "Malay",.    
-00001210: 2020 2020 2273 796d 626f 6c22 3a20 226d      "symbol": "m
-00001220: 7322 2c0a 2020 2020 2020 2020 2274 6578  s",.        "tex
-00001230: 7422 3a20 2245 6469 7420 6861 6c61 6d61  t": "Edit halama
-00001240: 6e20 696e 6922 0a20 2020 207d 2c0a 2020  n ini".    },.  
-00001250: 2020 7b0a 2020 2020 2020 2020 226c 616e    {.        "lan
-00001260: 6775 6167 6522 3a20 224d 616c 6179 616c  guage": "Malayal
-00001270: 616d 222c 0a20 2020 2020 2020 2022 7379  am",.        "sy
-00001280: 6d62 6f6c 223a 2022 6d6c 222c 0a20 2020  mbol": "ml",.   
-00001290: 2020 2020 2022 7465 7874 223a 2022 e0b4       "text": "..
-000012a0: 8820 e0b4 aae0 b587 e0b4 9ce0 b58d 20e0  . ............ .
-000012b0: b48e e0b4 a1e0 b4bf e0b4 b1e0 b58d e0b4  ................
-000012c0: b1e0 b581 e0b4 9ae0 b586 e0b4 afe0 b58d  ................
-000012d0: e0b4 afe0 b581 e0b4 9522 0a20 2020 207d  .........".    }
-000012e0: 2c0a 2020 2020 7b0a 2020 2020 2020 2020  ,.    {.        
-000012f0: 226c 616e 6775 6167 6522 3a20 2255 7264  "language": "Urd
-00001300: 7522 2c0a 2020 2020 2020 2020 2273 796d  u",.        "sym
-00001310: 626f 6c22 3a20 2275 7222 2c0a 2020 2020  bol": "ur",.    
-00001320: 2020 2020 2274 6578 7422 3a20 22d8 a7d8      "text": "...
-00001330: b320 d8b5 d981 d8ad db92 20d9 85db 8cda  . ........ .....
-00001340: ba20 d8aa d8b1 d985 db8c d985 20da a9d8  . .......... ...
-00001350: b1db 8cda ba22 0a20 2020 207d 2c0a 2020  .....".    },.  
-00001360: 2020 7b0a 2020 2020 2020 2020 226c 616e    {.        "lan
-00001370: 6775 6167 6522 3a20 2254 656c 7567 7522  guage": "Telugu"
-00001380: 2c0a 2020 2020 2020 2020 2273 796d 626f  ,.        "symbo
-00001390: 6c22 3a20 2274 6522 2c0a 2020 2020 2020  l": "te",.      
-000013a0: 2020 2274 6578 7422 3a20 22e0 b088 20e0    "text": "... .
-000013b0: b0aa e0b1 87e0 b09c e0b1 80e0 b0a8 e0b0  ................
-000013c0: bf20 e0b0 b8e0 b0b5 e0b0 b0e0 b0bf e0b0  . ..............
-000013d0: 82e0 b09a e0b0 82e0 b0a1 e0b0 bf22 0a20  .............". 
-000013e0: 2020 207d 2c0a 2020 2020 7b0a 2020 2020     },.    {.    
-000013f0: 2020 2020 226c 616e 6775 6167 6522 3a20      "language": 
-00001400: 2254 616d 696c 222c 0a20 2020 2020 2020  "Tamil",.       
-00001410: 2022 7379 6d62 6f6c 223a 2022 7461 222c   "symbol": "ta",
-00001420: 0a20 2020 2020 2020 2022 7465 7874 223a  .        "text":
-00001430: 2022 e0ae 87e0 aea8 e0af 8de0 aea4 e0ae   "..............
-00001440: aae0 af8d 20e0 aeaa e0ae 95e0 af8d e0ae  .... ...........
-00001450: 95e0 aea4 e0af 8de0 aea4 e0af 88e0 aea4  ................
-00001460: e0af 8d20 e0ae a4e0 aebf e0ae b0e0 af81  ... ............
-00001470: e0ae a4e0 af8d e0ae a4e0 aeb5 e0af 81e0  ................
-00001480: aeae e0af 8d22 0a20 2020 207d 2c0a 2020  .....".    },.  
-00001490: 2020 7b0a 2020 2020 2020 2020 226c 616e    {.        "lan
-000014a0: 6775 6167 6522 3a20 2243 6174 616c 616e  guage": "Catalan
-000014b0: 222c 0a20 2020 2020 2020 2022 7379 6d62  ",.        "symb
-000014c0: 6f6c 223a 2022 6361 222c 0a20 2020 2020  ol": "ca",.     
-000014d0: 2020 2022 7465 7874 223a 2022 4564 6974     "text": "Edit
-000014e0: 6575 2061 7175 6573 7461 2070 c3a0 6769  eu aquesta p..gi
-000014f0: 6e61 220a 2020 2020 7d0a 5d              na".    }.]
+00000000: 5b0a 2020 7b0a 2020 2020 226c 616e 6775  [.  {.    "langu
+00000010: 6167 6522 3a20 2245 6e67 6c69 7368 222c  age": "English",
+00000020: 0a20 2020 2022 7379 6d62 6f6c 223a 2022  .    "symbol": "
+00000030: 656e 222c 0a20 2020 2022 7465 7874 223a  en",.    "text":
+00000040: 2022 4564 6974 2074 6869 7320 7061 6765   "Edit this page
+00000050: 220a 2020 7d2c 0a20 207b 0a20 2020 2022  ".  },.  {.    "
+00000060: 6c61 6e67 7561 6765 223a 2022 4172 6162  language": "Arab
+00000070: 6963 222c 0a20 2020 2022 7379 6d62 6f6c  ic",.    "symbol
+00000080: 223a 2022 6172 222c 0a20 2020 2022 7465  ": "ar",.    "te
+00000090: 7874 223a 2022 d982 d985 20d8 a8d8 aad8  xt": ".... .....
+000000a0: add8 b1d9 8ad8 b120 d987 d8b0 d987 20d8  ....... ...... .
+000000b0: a7d9 84d8 b5d9 81d8 add8 a922 0a20 207d  ...........".  }
+000000c0: 2c0a 2020 7b0a 2020 2020 226c 616e 6775  ,.  {.    "langu
+000000d0: 6167 6522 3a20 2242 756c 6761 7269 616e  age": "Bulgarian
+000000e0: 222c 0a20 2020 2022 7379 6d62 6f6c 223a  ",.    "symbol":
+000000f0: 2022 6267 222c 0a20 2020 2022 7465 7874   "bg",.    "text
+00000100: 223a 2022 d0a0 d0b5 d0b4 d0b0 d0ba d182  ": "............
+00000110: d0b8 d180 d0b0 d0b9 d182 d0b5 20d1 82d0  ............ ...
+00000120: b0d0 b7d0 b820 d181 d182 d180 d0b0 d0bd  ..... ..........
+00000130: d0b8 d186 d0b0 220a 2020 7d2c 0a20 207b  ......".  },.  {
+00000140: 0a20 2020 2022 6c61 6e67 7561 6765 223a  .    "language":
+00000150: 2022 4368 696e 6573 6520 5369 6d70 6c69   "Chinese Simpli
+00000160: 6669 6564 222c 0a20 2020 2022 7379 6d62  fied",.    "symb
+00000170: 6f6c 223a 2022 7a68 5f43 4e22 2c0a 2020  ol": "zh_CN",.  
+00000180: 2020 2274 6578 7422 3a20 22e7 bc96 e8be    "text": ".....
+00000190: 91e6 ada4 e9a1 b5e9 9da2 220a 2020 7d2c  ..........".  },
+000001a0: 0a20 207b 0a20 2020 2022 6c61 6e67 7561  .  {.    "langua
+000001b0: 6765 223a 2022 4368 696e 6573 6520 5472  ge": "Chinese Tr
+000001c0: 6164 6974 696f 6e61 6c22 2c0a 2020 2020  aditional",.    
+000001d0: 2273 796d 626f 6c22 3a20 227a 682d 7477  "symbol": "zh-tw
+000001e0: 222c 0a20 2020 2022 7465 7874 223a 2022  ",.    "text": "
+000001f0: e7b7 a8e8 bcaf e6ad a4e9 a081 e99d a222  ..............."
+00000200: 0a20 207d 2c0a 2020 7b0a 2020 2020 226c  .  },.  {.    "l
+00000210: 616e 6775 6167 6522 3a20 2243 726f 6174  anguage": "Croat
+00000220: 6961 6e22 2c0a 2020 2020 2273 796d 626f  ian",.    "symbo
+00000230: 6c22 3a20 2268 7222 2c0a 2020 2020 2274  l": "hr",.    "t
+00000240: 6578 7422 3a20 2255 7265 6469 7465 206f  ext": "Uredite o
+00000250: 7675 2073 7472 616e 6963 7522 0a20 207d  vu stranicu".  }
+00000260: 2c0a 2020 7b0a 2020 2020 226c 616e 6775  ,.  {.    "langu
+00000270: 6167 6522 3a20 2243 7a65 6368 222c 0a20  age": "Czech",. 
+00000280: 2020 2022 7379 6d62 6f6c 223a 2022 6373     "symbol": "cs
+00000290: 222c 0a20 2020 2022 7465 7874 223a 2022  ",.    "text": "
+000002a0: 5570 7261 7669 7420 7475 746f 2073 7472  Upravit tuto str
+000002b0: c3a1 6e6b 7522 0a20 207d 2c0a 2020 7b0a  ..nku".  },.  {.
+000002c0: 2020 2020 226c 616e 6775 6167 6522 3a20      "language": 
+000002d0: 2244 616e 6973 6822 2c0a 2020 2020 2273  "Danish",.    "s
+000002e0: 796d 626f 6c22 3a20 2264 6122 2c0a 2020  ymbol": "da",.  
+000002f0: 2020 2274 6578 7422 3a20 2252 6564 6967    "text": "Redig
+00000300: 6572 2064 656e 6e65 2073 6964 6522 0a20  er denne side". 
+00000310: 207d 2c0a 2020 7b0a 2020 2020 226c 616e   },.  {.    "lan
+00000320: 6775 6167 6522 3a20 2244 7574 6368 222c  guage": "Dutch",
+00000330: 0a20 2020 2022 7379 6d62 6f6c 223a 2022  .    "symbol": "
+00000340: 6e6c 222c 0a20 2020 2022 7465 7874 223a  nl",.    "text":
+00000350: 2022 6265 7765 726b 2064 657a 6520 7061   "bewerk deze pa
+00000360: 6769 6e61 220a 2020 7d2c 0a20 207b 0a20  gina".  },.  {. 
+00000370: 2020 2022 6c61 6e67 7561 6765 223a 2022     "language": "
+00000380: 4573 7065 7261 6e74 6f22 2c0a 2020 2020  Esperanto",.    
+00000390: 2273 796d 626f 6c22 3a20 2265 6f22 2c0a  "symbol": "eo",.
+000003a0: 2020 2020 2274 6578 7422 3a20 2252 6564      "text": "Red
+000003b0: 616b 7475 20c4 8969 2074 6975 6e20 7061  aktu ..i tiun pa
+000003c0: c49d 6f6e 220a 2020 7d2c 0a20 207b 0a20  ..on".  },.  {. 
+000003d0: 2020 2022 6c61 6e67 7561 6765 223a 2022     "language": "
+000003e0: 4573 746f 6e69 616e 222c 0a20 2020 2022  Estonian",.    "
+000003f0: 7379 6d62 6f6c 223a 2022 6574 222c 0a20  symbol": "et",. 
+00000400: 2020 2022 7465 7874 223a 2022 4d75 7574     "text": "Muut
+00000410: 6b65 2073 6564 6120 6c65 6874 6522 0a20  ke seda lehte". 
+00000420: 207d 2c0a 2020 7b0a 2020 2020 226c 616e   },.  {.    "lan
+00000430: 6775 6167 6522 3a20 2246 696e 6e69 7368  guage": "Finnish
+00000440: 222c 0a20 2020 2022 7379 6d62 6f6c 223a  ",.    "symbol":
+00000450: 2022 6669 222c 0a20 2020 2022 7465 7874   "fi",.    "text
+00000460: 223a 2022 4d75 6f6b 6b61 6120 74c3 a474  ": "Muokkaa t..t
+00000470: c3a4 2073 6976 7561 220a 2020 7d2c 0a20  .. sivua".  },. 
+00000480: 207b 0a20 2020 2022 6c61 6e67 7561 6765   {.    "language
+00000490: 223a 2022 4672 656e 6368 222c 0a20 2020  ": "French",.   
+000004a0: 2022 7379 6d62 6f6c 223a 2022 6672 222c   "symbol": "fr",
+000004b0: 0a20 2020 2022 7465 7874 223a 2022 4d6f  .    "text": "Mo
+000004c0: 6469 6669 6572 2063 6574 7465 2070 6167  difier cette pag
+000004d0: 6522 0a20 207d 2c0a 2020 7b0a 2020 2020  e".  },.  {.    
+000004e0: 226c 616e 6775 6167 6522 3a20 2247 6572  "language": "Ger
+000004f0: 6d61 6e22 2c0a 2020 2020 2273 796d 626f  man",.    "symbo
+00000500: 6c22 3a20 2264 6522 2c0a 2020 2020 2274  l": "de",.    "t
+00000510: 6578 7422 3a20 2242 6561 7262 6569 7465  ext": "Bearbeite
+00000520: 2064 6965 7365 2053 6569 7465 220a 2020   diese Seite".  
+00000530: 7d2c 0a20 207b 0a20 2020 2022 6c61 6e67  },.  {.    "lang
+00000540: 7561 6765 223a 2022 4772 6565 6b22 2c0a  uage": "Greek",.
+00000550: 2020 2020 2273 796d 626f 6c22 3a20 2265      "symbol": "e
+00000560: 6c22 2c0a 2020 2020 2274 6578 7422 3a20  l",.    "text": 
+00000570: 22ce 95cf 80ce b5ce bece b5cf 81ce b3ce  "...............
+00000580: b1cf 83cf 84ce b5ce afcf 84ce b520 ceb1  ............. ..
+00000590: cf85 cf84 ceae cebd 20cf 84ce b720 cf83  ........ .... ..
+000005a0: ceb5 cebb ceaf ceb4 ceb1 220a 2020 7d2c  ..........".  },
+000005b0: 0a20 207b 0a20 2020 2022 6c61 6e67 7561  .  {.    "langua
+000005c0: 6765 223a 2022 4865 6272 6577 222c 0a20  ge": "Hebrew",. 
+000005d0: 2020 2022 7379 6d62 6f6c 223a 2022 6977     "symbol": "iw
+000005e0: 222c 0a20 2020 2022 7465 7874 223a 2022  ",.    "text": "
+000005f0: d7a2 d7a8 d795 d79a 20d7 93d7 a320 d796  ........ .... ..
+00000600: d794 220a 2020 7d2c 0a20 207b 0a20 2020  ..".  },.  {.   
+00000610: 2022 6c61 6e67 7561 6765 223a 2022 496e   "language": "In
+00000620: 646f 6e65 7369 616e 222c 0a20 2020 2022  donesian",.    "
+00000630: 7379 6d62 6f6c 223a 2022 6964 222c 0a20  symbol": "id",. 
+00000640: 2020 2022 7465 7874 223a 2022 4564 6974     "text": "Edit
+00000650: 2068 616c 616d 616e 2069 6e69 220a 2020   halaman ini".  
+00000660: 7d2c 0a20 207b 0a20 2020 2022 6c61 6e67  },.  {.    "lang
+00000670: 7561 6765 223a 2022 4974 616c 6961 6e22  uage": "Italian"
+00000680: 2c0a 2020 2020 2273 796d 626f 6c22 3a20  ,.    "symbol": 
+00000690: 2269 7422 2c0a 2020 2020 2274 6578 7422  "it",.    "text"
+000006a0: 3a20 224d 6f64 6966 6963 6120 7175 6573  : "Modifica ques
+000006b0: 7461 2070 6167 696e 6122 0a20 207d 2c0a  ta pagina".  },.
+000006c0: 2020 7b0a 2020 2020 226c 616e 6775 6167    {.    "languag
+000006d0: 6522 3a20 224a 6170 616e 6573 6522 2c0a  e": "Japanese",.
+000006e0: 2020 2020 2273 796d 626f 6c22 3a20 226a      "symbol": "j
+000006f0: 6122 2c0a 2020 2020 2274 6578 7422 3a20  a",.    "text": 
+00000700: 22e3 8193 e381 aee3 839a e383 bce3 82b8  "...............
+00000710: e382 92e7 b7a8 e99b 8622 0a20 207d 2c0a  .........".  },.
+00000720: 2020 7b0a 2020 2020 226c 616e 6775 6167    {.    "languag
+00000730: 6522 3a20 224b 6f72 6561 6e22 2c0a 2020  e": "Korean",.  
+00000740: 2020 2273 796d 626f 6c22 3a20 226b 6f22    "symbol": "ko"
+00000750: 2c0a 2020 2020 2274 6578 7422 3a20 22ec  ,.    "text": ".
+00000760: 9db4 20ed 8e98 ec9d b4ec a780 20ed 8eb8  .. ......... ...
+00000770: eca7 9122 0a20 207d 2c0a 2020 7b0a 2020  ...".  },.  {.  
+00000780: 2020 226c 616e 6775 6167 6522 3a20 224c    "language": "L
+00000790: 6174 7669 616e 222c 0a20 2020 2022 7379  atvian",.    "sy
+000007a0: 6d62 6f6c 223a 2022 6c76 222c 0a20 2020  mbol": "lv",.   
+000007b0: 2022 7465 7874 223a 2022 5265 6469 c4a3   "text": "Redi..
+000007c0: c493 7420 c5a1 6f20 6c61 7075 220a 2020  ..t ..o lapu".  
+000007d0: 7d2c 0a20 207b 0a20 2020 2022 6c61 6e67  },.  {.    "lang
+000007e0: 7561 6765 223a 2022 4c69 7468 7561 6e69  uage": "Lithuani
+000007f0: 616e 222c 0a20 2020 2022 7379 6d62 6f6c  an",.    "symbol
+00000800: 223a 2022 6c74 222c 0a20 2020 2022 7465  ": "lt",.    "te
+00000810: 7874 223a 2022 5265 6461 6775 6f74 6920  xt": "Redaguoti 
+00000820: c5a1 c4af 2070 7573 6c61 70c4 af22 0a20  .... puslap..". 
+00000830: 207d 2c0a 2020 7b0a 2020 2020 226c 616e   },.  {.    "lan
+00000840: 6775 6167 6522 3a20 224e 6f72 7765 6769  guage": "Norwegi
+00000850: 616e 222c 0a20 2020 2022 7379 6d62 6f6c  an",.    "symbol
+00000860: 223a 2022 6e6f 222c 0a20 2020 2022 7465  ": "no",.    "te
+00000870: 7874 223a 2022 5265 6469 6765 7220 6465  xt": "Rediger de
+00000880: 6e6e 6520 7369 6465 6e22 0a20 207d 2c0a  nne siden".  },.
+00000890: 2020 7b0a 2020 2020 226c 616e 6775 6167    {.    "languag
+000008a0: 6522 3a20 2250 6f6c 6973 6822 2c0a 2020  e": "Polish",.  
+000008b0: 2020 2273 796d 626f 6c22 3a20 2270 6c22    "symbol": "pl"
+000008c0: 2c0a 2020 2020 2274 6578 7422 3a20 2245  ,.    "text": "E
+000008d0: 6479 7475 6a20 74c4 9920 7374 726f 6e65  dytuj t.. strone
+000008e0: 220a 2020 7d2c 0a20 207b 0a20 2020 2022  ".  },.  {.    "
+000008f0: 6c61 6e67 7561 6765 223a 2022 506f 7274  language": "Port
+00000900: 7567 7565 7365 222c 0a20 2020 2022 7379  uguese",.    "sy
+00000910: 6d62 6f6c 223a 2022 7074 222c 0a20 2020  mbol": "pt",.   
+00000920: 2022 7465 7874 223a 2022 4564 6974 6520   "text": "Edite 
+00000930: 6573 7361 2070 c3a1 6769 6e61 220a 2020  essa p..gina".  
+00000940: 7d2c 0a20 207b 0a20 2020 2022 6c61 6e67  },.  {.    "lang
+00000950: 7561 6765 223a 2022 526f 6d61 6e69 616e  uage": "Romanian
+00000960: 222c 0a20 2020 2022 7379 6d62 6f6c 223a  ",.    "symbol":
+00000970: 2022 726f 222c 0a20 2020 2022 7465 7874   "ro",.    "text
+00000980: 223a 2022 4564 6974 61c8 9b69 2061 6365  ": "Edita..i ace
+00000990: 6173 74c4 8320 7061 6769 6ec4 8322 0a20  ast.. pagin..". 
+000009a0: 207d 2c0a 2020 7b0a 2020 2020 226c 616e   },.  {.    "lan
+000009b0: 6775 6167 6522 3a20 2252 7573 7369 616e  guage": "Russian
+000009c0: 222c 0a20 2020 2022 7379 6d62 6f6c 223a  ",.    "symbol":
+000009d0: 2022 7275 222c 0a20 2020 2022 7465 7874   "ru",.    "text
+000009e0: 223a 2022 d0a0 d0b5 d0b4 d0b0 d0ba d182  ": "............
+000009f0: d0b8 d180 d0be d0b2 d0b0 d182 d18c 20d1  .............. .
+00000a00: 8dd1 82d1 8320 d181 d182 d180 d0b0 d0bd  ..... ..........
+00000a10: d0b8 d186 d183 220a 2020 7d2c 0a20 207b  ......".  },.  {
+00000a20: 0a20 2020 2022 6c61 6e67 7561 6765 223a  .    "language":
+00000a30: 2022 5365 7262 6961 6e22 2c0a 2020 2020   "Serbian",.    
+00000a40: 2273 796d 626f 6c22 3a20 2273 7222 2c0a  "symbol": "sr",.
+00000a50: 2020 2020 2274 6578 7422 3a20 22d0 a3d1      "text": "...
+00000a60: 80d0 b5d0 b4d0 b8d1 82d0 b520 d0be d0b2  ........... ....
+00000a70: d183 20d1 81d1 82d1 80d0 b0d0 bdd0 b8d1  .. .............
+00000a80: 86d1 8322 0a20 207d 2c0a 2020 7b0a 2020  ...".  },.  {.  
+00000a90: 2020 226c 616e 6775 6167 6522 3a20 2253    "language": "S
+00000aa0: 6c6f 7661 6b22 2c0a 2020 2020 2273 796d  lovak",.    "sym
+00000ab0: 626f 6c22 3a20 2273 6b22 2c0a 2020 2020  bol": "sk",.    
+00000ac0: 2274 6578 7422 3a20 2255 7072 6176 69c5  "text": "Upravi.
+00000ad0: a520 74c3 ba74 6f20 7374 72c3 a16e 6b75  . t..to str..nku
+00000ae0: 220a 2020 7d2c 0a20 207b 0a20 2020 2022  ".  },.  {.    "
+00000af0: 6c61 6e67 7561 6765 223a 2022 536c 6f76  language": "Slov
+00000b00: 656e 6961 6e22 2c0a 2020 2020 2273 796d  enian",.    "sym
+00000b10: 626f 6c22 3a20 2273 6c22 2c0a 2020 2020  bol": "sl",.    
+00000b20: 2274 6578 7422 3a20 2255 7265 6469 7465  "text": "Uredite
+00000b30: 2074 6f20 7374 7261 6e22 0a20 207d 2c0a   to stran".  },.
+00000b40: 2020 7b0a 2020 2020 226c 616e 6775 6167    {.    "languag
+00000b50: 6522 3a20 2253 7061 6e69 7368 222c 0a20  e": "Spanish",. 
+00000b60: 2020 2022 7379 6d62 6f6c 223a 2022 6573     "symbol": "es
+00000b70: 222c 0a20 2020 2022 7465 7874 223a 2022  ",.    "text": "
+00000b80: 4564 6974 6120 6573 7461 2070 c3a1 6769  Edita esta p..gi
+00000b90: 6e61 220a 2020 7d2c 0a20 207b 0a20 2020  na".  },.  {.   
+00000ba0: 2022 6c61 6e67 7561 6765 223a 2022 5377   "language": "Sw
+00000bb0: 6564 6973 6822 2c0a 2020 2020 2273 796d  edish",.    "sym
+00000bc0: 626f 6c22 3a20 2273 7622 2c0a 2020 2020  bol": "sv",.    
+00000bd0: 2274 6578 7422 3a20 2252 6564 6967 6572  "text": "Rediger
+00000be0: 6120 6465 6e20 68c3 a472 2073 6964 616e  a den h..r sidan
+00000bf0: 220a 2020 7d2c 0a20 207b 0a20 2020 2022  ".  },.  {.    "
+00000c00: 6c61 6e67 7561 6765 223a 2022 5461 6a69  language": "Taji
+00000c10: 6b22 2c0a 2020 2020 2273 796d 626f 6c22  k",.    "symbol"
+00000c20: 3a20 2274 6722 2c0a 2020 2020 2274 6578  : "tg",.    "tex
+00000c30: 7422 3a20 22d0 98d0 bd20 d181 d0b0 d2b3  t": ".... ......
+00000c40: d0b8 d184 d0b0 d180 d0be 20d1 82d0 b0d2  .......... .....
+00000c50: b3d1 80d0 b8d1 8020 d0ba d183 d0bd d0b5  ....... ........
+00000c60: d0b4 220a 2020 7d2c 0a20 207b 0a20 2020  ..".  },.  {.   
+00000c70: 2022 6c61 6e67 7561 6765 223a 2022 5468   "language": "Th
+00000c80: 6169 222c 0a20 2020 2022 7379 6d62 6f6c  ai",.    "symbol
+00000c90: 223a 2022 7468 222c 0a20 2020 2022 7465  ": "th",.    "te
+00000ca0: 7874 223a 2022 e0b9 81e0 b881 e0b9 89e0  xt": "..........
+00000cb0: b984 e0b8 82e0 b8ab e0b8 99e0 b989 e0b8  ................
+00000cc0: b2e0 b899 e0b8 b5e0 b989 220a 2020 7d2c  ..........".  },
+00000cd0: 0a20 207b 0a20 2020 2022 6c61 6e67 7561  .  {.    "langua
+00000ce0: 6765 223a 2022 5475 726b 6973 6822 2c0a  ge": "Turkish",.
+00000cf0: 2020 2020 2273 796d 626f 6c22 3a20 2274      "symbol": "t
+00000d00: 7222 2c0a 2020 2020 2274 6578 7422 3a20  r",.    "text": 
+00000d10: 2242 7520 7361 7966 6179 c4b1 2064 c3bc  "Bu sayfay.. d..
+00000d20: 7a65 6e6c 6522 0a20 207d 2c0a 2020 7b0a  zenle".  },.  {.
+00000d30: 2020 2020 226c 616e 6775 6167 6522 3a20      "language": 
+00000d40: 2255 6b72 6169 6e69 616e 222c 0a20 2020  "Ukrainian",.   
+00000d50: 2022 7379 6d62 6f6c 223a 2022 756b 222c   "symbol": "uk",
+00000d60: 0a20 2020 2022 7465 7874 223a 2022 d0a0  .    "text": "..
+00000d70: d0b5 d0b4 d0b0 d0b3 d183 d0b2 d0b0 d182  ................
+00000d80: d0b8 20d1 86d1 8e20 d181 d182 d0be d180  .. .... ........
+00000d90: d196 d0bd d0ba d183 220a 2020 7d2c 0a20  ........".  },. 
+00000da0: 207b 0a20 2020 2022 6c61 6e67 7561 6765   {.    "language
+00000db0: 223a 2022 5669 6574 6e61 6d65 7365 222c  ": "Vietnamese",
+00000dc0: 0a20 2020 2022 7379 6d62 6f6c 223a 2022  .    "symbol": "
+00000dd0: 7669 222c 0a20 2020 2022 7465 7874 223a  vi",.    "text":
+00000de0: 2022 6368 e1bb 896e 6820 73e1 bbad 6120   "ch...nh s...a 
+00000df0: 7472 616e 6720 6ec3 a079 220a 2020 7d2c  trang n..y".  },
+00000e00: 0a20 207b 0a20 2020 2022 6c61 6e67 7561  .  {.    "langua
+00000e10: 6765 223a 2022 4265 6e67 616c 6922 2c0a  ge": "Bengali",.
+00000e20: 2020 2020 2273 796d 626f 6c22 3a20 2262      "symbol": "b
+00000e30: 6e22 2c0a 2020 2020 2274 6578 7422 3a20  n",.    "text": 
+00000e40: 22e0 a68f e0a6 8720 e0a6 aae0 a783 e0a6  "...... ........
+00000e50: b7e0 a78d e0a6 a0e0 a6be e0a6 9fe0 a6bf  ................
+00000e60: 20e0 a6b8 e0a6 aee0 a78d e0a6 aae0 a6be   ...............
+00000e70: e0a6 a6e0 a6a8 e0a6 be20 e0a6 95e0 a6b0  ......... ......
+00000e80: e0a7 81e0 a6a8 220a 2020 7d2c 0a20 207b  ......".  },.  {
+00000e90: 0a20 2020 2022 6c61 6e67 7561 6765 223a  .    "language":
+00000ea0: 2022 4669 6c69 7069 6e6f 222c 0a20 2020   "Filipino",.   
+00000eb0: 2022 7379 6d62 6f6c 223a 2022 746c 222c   "symbol": "tl",
+00000ec0: 0a20 2020 2022 7465 7874 223a 2022 492d  .    "text": "I-
+00000ed0: 6564 6974 2061 6e67 2070 6168 696e 616e  edit ang pahinan
+00000ee0: 6720 6974 6f22 0a20 207d 2c0a 2020 7b0a  g ito".  },.  {.
+00000ef0: 2020 2020 226c 616e 6775 6167 6522 3a20      "language": 
+00000f00: 224d 6172 6174 6869 222c 0a20 2020 2022  "Marathi",.    "
+00000f10: 7379 6d62 6f6c 223a 2022 6d72 222c 0a20  symbol": "mr",. 
+00000f20: 2020 2022 7465 7874 223a 2022 e0a4 b9e0     "text": "....
+00000f30: a587 20e0 a4aa e0a5 83e0 a4b7 e0a5 8de0  .. .............
+00000f40: a4a0 20e0 a4b8 e0a4 82e0 a4aa e0a4 bee0  .. .............
+00000f50: a4a6 e0a4 bfe0 a4a4 20e0 a495 e0a4 b0e0  ........ .......
+00000f60: a4be 220a 2020 7d2c 0a20 207b 0a20 2020  ..".  },.  {.   
+00000f70: 2022 6c61 6e67 7561 6765 223a 2022 4d61   "language": "Ma
+00000f80: 6c61 7922 2c0a 2020 2020 2273 796d 626f  lay",.    "symbo
+00000f90: 6c22 3a20 226d 7322 2c0a 2020 2020 2274  l": "ms",.    "t
+00000fa0: 6578 7422 3a20 2245 6469 7420 6861 6c61  ext": "Edit hala
+00000fb0: 6d61 6e20 696e 6922 0a20 207d 2c0a 2020  man ini".  },.  
+00000fc0: 7b0a 2020 2020 226c 616e 6775 6167 6522  {.    "language"
+00000fd0: 3a20 224d 616c 6179 616c 616d 222c 0a20  : "Malayalam",. 
+00000fe0: 2020 2022 7379 6d62 6f6c 223a 2022 6d6c     "symbol": "ml
+00000ff0: 222c 0a20 2020 2022 7465 7874 223a 2022  ",.    "text": "
+00001000: e0b4 8820 e0b4 aae0 b587 e0b4 9ce0 b58d  ... ............
+00001010: 20e0 b48e e0b4 a1e0 b4bf e0b4 b1e0 b58d   ...............
+00001020: e0b4 b1e0 b581 e0b4 9ae0 b586 e0b4 afe0  ................
+00001030: b58d e0b4 afe0 b581 e0b4 9522 0a20 207d  ...........".  }
+00001040: 2c0a 2020 7b0a 2020 2020 226c 616e 6775  ,.  {.    "langu
+00001050: 6167 6522 3a20 2255 7264 7522 2c0a 2020  age": "Urdu",.  
+00001060: 2020 2273 796d 626f 6c22 3a20 2275 7222    "symbol": "ur"
+00001070: 2c0a 2020 2020 2274 6578 7422 3a20 22d8  ,.    "text": ".
+00001080: a7d8 b320 d8b5 d981 d8ad db92 20d9 85db  ... ........ ...
+00001090: 8cda ba20 d8aa d8b1 d985 db8c d985 20da  ... .......... .
+000010a0: a9d8 b1db 8cda ba22 0a20 207d 2c0a 2020  .......".  },.  
+000010b0: 7b0a 2020 2020 226c 616e 6775 6167 6522  {.    "language"
+000010c0: 3a20 2254 656c 7567 7522 2c0a 2020 2020  : "Telugu",.    
+000010d0: 2273 796d 626f 6c22 3a20 2274 6522 2c0a  "symbol": "te",.
+000010e0: 2020 2020 2274 6578 7422 3a20 22e0 b088      "text": "...
+000010f0: 20e0 b0aa e0b1 87e0 b09c e0b1 80e0 b0a8   ...............
+00001100: e0b0 bf20 e0b0 b8e0 b0b5 e0b0 b0e0 b0bf  ... ............
+00001110: e0b0 82e0 b09a e0b0 82e0 b0a1 e0b0 bf22  ..............."
+00001120: 0a20 207d 2c0a 2020 7b0a 2020 2020 226c  .  },.  {.    "l
+00001130: 616e 6775 6167 6522 3a20 2254 616d 696c  anguage": "Tamil
+00001140: 222c 0a20 2020 2022 7379 6d62 6f6c 223a  ",.    "symbol":
+00001150: 2022 7461 222c 0a20 2020 2022 7465 7874   "ta",.    "text
+00001160: 223a 2022 e0ae 87e0 aea8 e0af 8de0 aea4  ": "............
+00001170: e0ae aae0 af8d 20e0 aeaa e0ae 95e0 af8d  ...... .........
+00001180: e0ae 95e0 aea4 e0af 8de0 aea4 e0af 88e0  ................
+00001190: aea4 e0af 8d20 e0ae a4e0 aebf e0ae b0e0  ..... ..........
+000011a0: af81 e0ae a4e0 af8d e0ae a4e0 aeb5 e0af  ................
+000011b0: 81e0 aeae e0af 8d22 0a20 207d 2c0a 2020  .......".  },.  
+000011c0: 7b0a 2020 2020 226c 616e 6775 6167 6522  {.    "language"
+000011d0: 3a20 2243 6174 616c 616e 222c 0a20 2020  : "Catalan",.   
+000011e0: 2022 7379 6d62 6f6c 223a 2022 6361 222c   "symbol": "ca",
+000011f0: 0a20 2020 2022 7465 7874 223a 2022 4564  .    "text": "Ed
+00001200: 6974 6575 2061 7175 6573 7461 2070 c3a0  iteu aquesta p..
+00001210: 6769 6e61 220a 2020 7d0a 5d0a            gina".  }.].
```

### Comparing `stmaterial-0.0.6/src/stmaterial/assets/translations/jsons/On this page.json` & `stmaterial-0.0.7/src/stmaterial/assets/translations/jsons/On this page.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -182,8 +182,8 @@
 00000b50: 756b 222c 0a20 2020 2022 7465 7874 223a  uk",.    "text":
 00000b60: 2022 d097 d0bc d196 d181 d182 220a 2020   "..........".  
 00000b70: 7d2c 0a20 207b 0a20 2020 2022 6c61 6e67  },.  {.    "lang
 00000b80: 7561 6765 223a 2022 5669 6574 6e61 6d65  uage": "Vietname
 00000b90: 7365 222c 0a20 2020 2022 7379 6d62 6f6c  se",.    "symbol
 00000ba0: 223a 2022 7669 222c 0a20 2020 2022 7465  ": "vi",.    "te
 00000bb0: 7874 223a 2022 4ee1 bb99 6920 6475 6e67  xt": "N...i dung
-00000bc0: 220a 2020 7d0a 5d                        ".  }.]
+00000bc0: 220a 2020 7d0a 5d0a                      ".  }.].
```

### Comparing `stmaterial-0.0.6/src/stmaterial/demo/module.py` & `stmaterial-0.0.7/src/stmaterial/demo/module.py`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.6/src/stmaterial/demo/sphinxext.py` & `stmaterial-0.0.7/src/stmaterial/demo/sphinxext.py`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.6/src/stmaterial/directives.py` & `stmaterial-0.0.7/src/stmaterial/directives.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import List
 from yaml import safe_load
 from pathlib import Path
 from docutils import nodes
 from docutils.parsers.rst import directives
 from sphinx.util.docutils import SphinxDirective
 from sphinx.util import logging
+
 SPHINX_LOGGER = logging.getLogger(__name__)
 
 TEMPLATE_GRID = """
 `````{{grid}} {grid_columns}
 {container_options}
 
 {content}
@@ -20,14 +21,15 @@
 ````{{grid-item-card}} {title}
 {card_options}
 
 {content}
 ````
 """
 
+
 class GalleryDirective(SphinxDirective):
     """A directive to show a gallery of images and links in a grid."""
 
     name = "gallery-grid"
     has_content = True
     required_arguments = 0
     optional_arguments = 1
@@ -47,15 +49,15 @@
             path_doc, _ = self.get_source_info()
             path_doc = Path(path_doc).parent
             path_data = (path_doc / path_data_rel).resolve()
             if not path_data.exists():
                 SPHINX_LOGGER.warn(f"Could not find grid data at {path_data}.")
                 nodes.text("No grid data found at {path_data}.")
                 return
-            yaml_string = path_data.read_text(encoding='utf-8')
+            yaml_string = path_data.read_text(encoding="utf-8")
         else:
             yaml_string = "\n".join(self.content)
 
         # Read in YAML so we can generate the gallery
         grid_data = safe_load(yaml_string)
 
         grid_items = []
```

### Comparing `stmaterial-0.0.6/src/stmaterial/theme/stmaterial/base.html` & `stmaterial-0.0.7/src/stmaterial/theme/stmaterial/base.html`

 * *Files 13% similar despite different names*

```diff
@@ -2,18 +2,19 @@
 <html class="no-js" {% if language is not none %} lang="{{ language }}" {% endif %}>
 {%- import "static/webpack-macros.html" as _webpack with context %}
 {%- import "partials/_icon_links_declaration.html" as _icon_declare with context %}
 
 <head>
     {%- block site_meta -%}
     <meta charset="utf-8" />
+    <meta name="keywords" content="python, sphinx, sphinx-theme, documentation" />
+    <meta name="description" content="A Materialize based sphinx theme" />
     <meta name="viewport" content="width=device-width,initial-scale=1" />
-    <meta http-equiv="X-UA-Compatible" content="IE=edge">
-    <meta name="msapplication-tap-highlight" content="no">
-    <meta http-equiv="Permissions-Policy" content="interest-cohort=()">
+    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
+    <meta name="msapplication-tap-highlight" content="no" />
 
     {%- if metatags %}{{ metatags }}{% endif -%}
 
     {%- block linktags %}
     {%- if hasdoc('about') %}
     <link rel="author" title="{{ _('About these documents') }}" href="{{ pathto('about') }}" />
     {%- endif %}
@@ -69,45 +70,45 @@
     {%- endif %}
     {% endfor -%}
     {%- endblock regular_styles -%}
 
     {#- Theme-related stylesheets -#}
     {%- block theme_styles %}
     {% include "partials/_head_css_variables.html" with context %}
-    {%- endblock -%}
+    {%- endblock theme_styles -%}
 
     {%- block extra_styles %}
-    {%- endblock -%}
+    {%- endblock extra_styles -%}
 
     {{ _webpack.head_js_preload() }}
     {%- endblock styles -%}
 
     {#- Custom front matter #}
-    {%- block extrahead -%}{%- endblock -%}
+    {%- block extrahead -%}{%- endblock extrahead -%}
     <script>
         const theme = localStorage.getItem('theme');
         if (theme) document.documentElement.setAttribute('theme', theme);
     </script>
 </head>
 
 <body>
     {% block htmlbody %}
-    {% endblock %}
+    {% endblock htmlbody %}
 
     {%- block scripts -%}
 
     {# Custom JS #}
     {%- block regular_scripts -%}
     {% for path in script_files -%}
     {{ js_tag(path) }}
     {% endfor -%}
     {%- endblock regular_scripts -%}
 
     {# Theme-related JavaScript code #}
     {%- block theme_scripts -%}
     {{ _webpack.body_post() }}
-    {%- endblock -%}
+    {%- endblock theme_scripts -%}
 
     {%- endblock scripts -%}
 </body>
 
 </html>
```

#### html2text {}

```diff
@@ -3,14 +3,15 @@
 "static/webpack-macros.html" as _webpack with context %} {%- import "partials/
 _icon_links_declaration.html" as _icon_declare with context %}
 {%- block site_meta -%}
 
 
 
 
+
  {%- if metatags %}{{ metatags }}{% endif -%} {%- block linktags %} {%- if
 hasdoc('about') %}
  {%- endif %} {%- if hasdoc('genindex') %}
  {%- endif %} {%- if hasdoc('search') %}
  {%- endif %} {%- if hasdoc('copyright') %}
  {%- endif %} {%- if next %}
  {%- endif %} {%- if prev %}
@@ -21,15 +22,16 @@
 {% elif pagename == master_doc %}
 {% else %}
 {% endif %} {%- endblock -%} {%- block styles -%} {{ _webpack.head_pre_icons()
 }} {# Custom stylesheets #} {%- block regular_styles -%} {%- for css in
 css_files -%} {% if css|attr("filename") -%} {{ css_tag(css) }} {%- else -%}
  {%- endif %} {% endfor -%} {%- endblock regular_styles -%} {#- Theme-related
 stylesheets -#} {%- block theme_styles %} {% include "partials/
-_head_css_variables.html" with context %} {%- endblock -%} {%- block
-extra_styles %} {%- endblock -%} {{ _webpack.head_js_preload() }} {%- endblock
-styles -%} {#- Custom front matter #} {%- block extrahead -%}{%- endblock -%}
-{% block htmlbody %} {% endblock %} {%- block scripts -%} {# Custom JS #} {%-
-block regular_scripts -%} {% for path in script_files -%} {{ js_tag(path) }} {%
-endfor -%} {%- endblock regular_scripts -%} {# Theme-related JavaScript code #}
-{%- block theme_scripts -%} {{ _webpack.body_post() }} {%- endblock -%} {%-
-endblock scripts -%}
+_head_css_variables.html" with context %} {%- endblock theme_styles -%} {%-
+block extra_styles %} {%- endblock extra_styles -%} {{ _webpack.head_js_preload
+() }} {%- endblock styles -%} {#- Custom front matter #} {%- block extrahead -
+%}{%- endblock extrahead -%}
+{% block htmlbody %} {% endblock htmlbody %} {%- block scripts -%} {# Custom JS
+#} {%- block regular_scripts -%} {% for path in script_files -%} {{ js_tag
+(path) }} {% endfor -%} {%- endblock regular_scripts -%} {# Theme-related
+JavaScript code #} {%- block theme_scripts -%} {{ _webpack.body_post() }} {%-
+endblock theme_scripts -%} {%- endblock scripts -%}
```

### Comparing `stmaterial-0.0.6/src/stmaterial/theme/stmaterial/components/breadcrumbs.html` & `stmaterial-0.0.7/src/stmaterial/theme/stmaterial/components/breadcrumbs.html`

 * *Files 8% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 #}
 {% if parents|length>2 %}
 {% set parents=[parents[0], {"title": '<i class="fa-solid fa-ellipsis"></i>'}, parents[-1]] %}
 {% endif %}
 
 
 {#- Hide breadcrumbs on the home page #}
-
-<div class="nav-breadcrumbs">
+{% if title and pagename != root_doc %}
+<div class="stm-article-breadcrumbs">
     <a href="{{ pathto(root_doc) }}" class="breadcrumb breadcrumb-home"><i class="material-icons">home</i></a>
     {%- for doc in parents %}
     {% if doc.link %}
     <a href="{{ doc.link|e }}" class="breadcrumb">{{ doc.title }}</a>
     {% else %}
     <a class="breadcrumb">{{ doc.title }}</a>
     {% endif %}
     {%- endfor %}
     <a class="breadcrumb" aria-current="page">{{ title }}</a>
 </div>
-
-{%- endblock %}
+{% endif %}
+{%- endblock %}
```

#### html2text {}

```diff
@@ -1,9 +1,10 @@
 {%- block breadcrumbs %} {# If we have more than 3 parents (excluding the home
 page) then we remove The ones in the middle and add an ellipsis. This code is
 from https://github.com/pydata/pydata-sphinx-theme/blob/main/src/
 pydata_sphinx_theme/theme/pydata_sphinx_theme/components/breadcrumbs.html #} {%
 if parents|length>2 %} {% set parents=[parents[0], {"title": ''}, parents[-1]]
-%} {% endif %} {#- Hide breadcrumbs on the home page #}
+%} {% endif %} {#- Hide breadcrumbs on the home page #} {% if title and
+pagename != root_doc %}
 home {%- for doc in parents %} {% if doc.link %} {{_doc.title_}} {% else %} {
 { doc.title }} {% endif %} {%- endfor %} {{ title }}
-{%- endblock %}
+{% endif %} {%- endblock %}
```

### Comparing `stmaterial-0.0.6/src/stmaterial/theme/stmaterial/components/edit-this-page.html` & `stmaterial-0.0.7/src/stmaterial/theme/stmaterial/components/edit-this-page.html`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 {% extends "basic-ng/components/edit-this-page.html" %}
 {% from "basic-ng/components/edit-this-page.html" import determine_page_edit_link with context %}
 
 {%- macro page_edit_button(url) -%}
+{% if theme_use_edit_page_button %}
 <a class="edit-this-page" href="{{ url }}" title="{{ translate('Edit this page') }}">
     <i class="material-icons">mode_edit</i> {% if not show_source %} {{ translate('Edit this page') }} {% endif %}
 </a>
+{% endif %}
 {%- endmacro -%}
 
 {% block link_available -%}
 {{ page_edit_button(determine_page_edit_link()) }}
-{%- endblock %}
+{%- endblock link_available %}
 
 {% block link_not_available %}
 {# Make nice things happen, on Read the Docs #}
 {%- if READTHEDOCS and conf_py_path and page_source_suffix and github_user != "None" and github_repo != "None" and
 github_version and pagename and page_source_suffix %}
 {% set url = "https://github.com/" + github_user + "/" + github_repo + "/edit/" + github_version + conf_py_path +
 pagename + page_source_suffix %}
 {{ page_edit_button(url) }}
 {%- endif -%}
-{% endblock %}
+{% endblock link_not_available %}
```

### Comparing `stmaterial-0.0.6/src/stmaterial/theme/stmaterial/components/postnav.html` & `stmaterial-0.0.7/src/stmaterial/theme/stmaterial/components/postnav.html`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -24,8 +24,8 @@
                 <p class="prev-next-title">{{ post.next.title }}</p>
             </div>
             <i class="material-icons">chevron_right</i>
         </div>
     </a>
     {%- endif %}
 </div>
-{% endif %}
+{% endif %}
```

### Comparing `stmaterial-0.0.6/src/stmaterial/theme/stmaterial/components/prev-next.html` & `stmaterial-0.0.7/src/stmaterial/theme/stmaterial/components/prev-next.html`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -21,8 +21,8 @@
                 <p class="prev-next-title">{{ next_title or next.title }}</p>
             </div>
             <i class="material-icons">chevron_right</i>
         </div>
     </a>
     {%- endif %}
 </div>
-{%- endif %}
+{%- endif %}
```

### Comparing `stmaterial-0.0.6/src/stmaterial/theme/stmaterial/components/search-field.html` & `stmaterial-0.0.7/src/stmaterial/theme/stmaterial/components/search-field.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <form class="search-wrapper" method="get" action="{{ pathto('search') }}" role="search">
     <span class="material-icons">search</span>
     <input class="search-docs" placeholder="{{ theme_search_bar_text }}" name="q"
         aria-label="{{ theme_search_bar_text }}" autocomplete="off" autocorrect="off" autocapitalize="off"
-        spellcheck="false">
-    <input type="hidden" name="check_keywords" value="yes">
-    <input type="hidden" name="area" value="default">
+        spellcheck="false" />
+    <input type="hidden" name="check_keywords" value="yes" />
+    <input type="hidden" name="area" value="default" />
     <span class="search-button__kbd-shortcut"><kbd class="kbd-shortcut__modifier">Ctrl</kbd>+<kbd>K</kbd></span>
 </form>
```

### Comparing `stmaterial-0.0.6/src/stmaterial/theme/stmaterial/domainindex.html` & `stmaterial-0.0.7/src/stmaterial/theme/stmaterial/domainindex.html`

 * *Files 6% similar despite different names*

```diff
@@ -23,36 +23,36 @@
 </section>
 
 {%- set groupid = idgen() %}
 <table class="domainindex-table">
     {%- for letter, entries in content %}
     <tr class="pcap">
         <td></td>
-        <td>&#160;</td>
+        <td>{# djlint:off #}&#160;{# djlint:on #}</td>
         <td></td>
     </tr>
     <tr class="cap" id="cap-{{ letter }}">
         <td></td>
         <td><strong>{{ letter }}</strong></td>
         <td></td>
     </tr>
     {%- for (name, grouptype, page, anchor, extra, qualifier, description) in entries %}
     <tr{% if grouptype==2 %} class="cg-{{ groupid.current() }}" {% endif %}>
         <td>{% if grouptype == 1 -%}
-            <img src="{{ pathto('_static/minus.png', 1) }}" class="toggler" id="toggle-{{ groupid.next() }}"
-                style="display: none" alt="-" />
+            {# djlint:off #}<img src="{{ pathto('_static/minus.png', 1) }}" class="toggler"
+                id="toggle-{{ groupid.next() }}" style="display: none" alt="-" />{# djlint:on #}
             {%- endif %}
         </td>
-        <td>{% if grouptype == 2 %}&#160;&#160;&#160;{% endif %}
+        <td>{% if grouptype == 2 %}{# djlint:off #}&#160;&#160;&#160;{# djlint:on #}{% endif %}
             {% if page %}<a href="{{ pathto(page)|e }}#{{ anchor }}">{% endif -%}
                 <code class="xref">{{ name|e }}</code>
                 {%- if page %}</a>{% endif %}
             {%- if extra %} <em>({{ extra|e }})</em>{% endif -%}
         </td>
         <td>{% if qualifier %}<strong>{{ qualifier|e }}:</strong>{% endif %}
             <em>{{ description|e }}</em>
         </td>
         </tr>
         {%- endfor %}
         {%- endfor %}
 </table>
-{% endblock body %}
+{% endblock body %}
```

#### html2text {}

```diff
@@ -2,10 +2,10 @@
 {% endblock htmltitle -%} {% block scripts -%} {{ super() }} {%- if not
 embedded and collapse_index %}
  {%- endif -%} {%- endblock scripts %} {% block body %}
 ****** {{ indextitle }} ******
 {%- for (letter, entries) in content -%} {{_letter_}} {%- if not loop.last %} |
 {% endif -%} {%- endfor -%}
  {%- set groupid = idgen() %}
-  
+ {# djlint:off #} {# djlint:on #}
  {{ letter }}
 {% endblock body %}
```

### Comparing `stmaterial-0.0.6/src/stmaterial/theme/stmaterial/genindex.html` & `stmaterial-0.0.7/src/stmaterial/theme/stmaterial/genindex.html`

 * *Files 18% similar despite different names*

```diff
@@ -33,18 +33,18 @@
         {%- endfor -%}
     </div>
 </section>
 
 {%- for key, entries in genindexentries %}
 <section id="{{ key }}" class="genindex-section">
     <h2>{{ key }}</h2>
-    <table style="width: 100%" class="indextable genindextable">
+    <table class="indextable genindextable">
         <tr>
             {%- for column in entries|slice_index(2) if column %}
-            <td style="width: 33%; vertical-align: top;">
+            <td>
                 <ul>
                     {%- for entryname, (links, subitems, _) in column %}
                     <li>{{ indexentries(entryname, links) }}
                         {%- if subitems %}
                         <ul>
                             {%- for subentryname, subentrylinks in subitems %}
                             <li>{{ indexentries(subentryname, subentrylinks) }}</li>
@@ -56,8 +56,8 @@
                 </ul>
             </td>
             {%- endfor %}
         </tr>
     </table>
 </section>
 {% endfor %}
-{% endblock %}
+{% endblock body %}
```

#### html2text {}

```diff
@@ -12,8 +12,8 @@
     * {%- for entryname, (links, subitems, _) in column %}
     * {{ indexentries(entryname, links) }} {%- if subitems %}
           o {%- for subentryname, subentrylinks in subitems %}
           o {{ indexentries(subentryname, subentrylinks) }}
           o {%- endfor %}
       {%- endif -%}
     * {%- endfor %}
- {% endfor %} {% endblock %}
+ {% endfor %} {% endblock body %}
```

### Comparing `stmaterial-0.0.6/src/stmaterial/theme/stmaterial/layout.html` & `stmaterial-0.0.7/src/stmaterial/theme/stmaterial/layout.html`

 * *Files 10% similar despite different names*

```diff
@@ -5,19 +5,17 @@
 show_nav_level=theme_show_nav_level|int,
 maxdepth=theme_navigation_depth|int,
 collapse=theme_collapse_navigation|tobool,
 includehidden=True,
 titles_only=True)
 -%}
 
-
 {%- set head_nav_html = generate_header_nav_html(n_links_before_dropdown=theme_header_links_before_dropdown)
 -%}
 
-
 {% block htmlbody -%}
 {# checkbox to toggle primary sidebar #}
 <input type="checkbox" class="sidebar-toggle" name="__primary" id="__primary" />
 <label class="overlay overlay-primary" for="__primary"></label>
 
 {% block docs_headnav %}
 <header>
@@ -45,32 +43,22 @@
                 {% endblock left_sidebar %}
             </div>
         </aside>
         <main class="stm-content">
             <div class="container">
                 <div class="row">
                     <div class="stm-article section col s12 {% if not hide_tocnav %} m10 xl9 {% endif %}">
+                        {% include "sections/article-top.html" %}
                         {% include "components/searchbox.html" %}
+
                         <article role="main" class="section">
-                            {% block body %}{{ body }}{% endblock %}
+                            {% block body %}{{ body }}{% endblock body %}
                         </article>
 
-                        <div class="stm-article-metadata-info">
-                            <div class="metadata-info-area">
-                                <div class="metadata-left">
-                                    {% include "components/last-updated.html" %}
-                                </div>
-                                <div class="metadata-right">
-                                    {% include "components/sourcelink.html" %}
-                                    {% if theme_use_edit_page_button %}
-                                    {% include "components/edit-this-page.html" %}
-                                    {% endif %}
-                                </div>
-                            </div>
-                        </div>
+                        {% include "sections/article-bottom.html" %}
 
                         <div class="stm-article-footer">
                             <div class="prev-next-area">
                                 {% if theme_show_prev_next %}
                                 {% include "components/prev-next.html" %}
                                 {% endif %}
                                 {% include "components/postnav.html" %}
@@ -119,11 +107,11 @@
     </div>
 </div>
 
 {% block footer %}
 {% if theme_footer %}
 {% include "sections/footer.html" %}
 {% endif %}
-{% endblock %}
+{% endblock footer %}
 
-{%- endblock %}
-{%- endblock %}
+{%- endblock mainbody %}
+{%- endblock htmlbody %}
```

### Comparing `stmaterial-0.0.6/src/stmaterial/theme/stmaterial/partials/_head_css_variables.html` & `stmaterial-0.0.7/src/stmaterial/theme/stmaterial/partials/_head_css_variables.html`

 * *Files 8% similar despite different names*

```diff
@@ -7,46 +7,45 @@
 {% if user_customisations -%}
 {% for name, value in user_customisations.items() -%}
 --{{ name }}: {{ value }};
 {% endfor %}
 {%- endif %}
 {%- endmacro %}
 
-
 {% macro declare_font_variables(user_customisations) -%}
 {% if user_customisations -%}
 {% for src in user_customisations.src -%}
 @font-face {
 font-family: {{ user_customisations.name }};
 font-weight: {{ src.weight }};
 font-style: normal;
 font-display: swap;
 src: url({{ src.url }}) format({{ user_customisations.type }});
 }
 {% endfor %}
 {% if user_customisations.font_stack -%}
 :root {
---font-stack: {{ user_customisations.font_stack}}, -apple-system, BlinkMacSystemFont, Segoe UI, Helvetica, Arial, sans-serif, Apple Color Emoji, Segoe UI Emoji;
+--font-stack: {{ user_customisations.font_stack }}, -apple-system, BlinkMacSystemFont, Segoe UI, Helvetica, Arial, sans-serif, Apple Color Emoji, Segoe UI Emoji;
 }
 {% else %}
 :root {
---font-stack: Georgia, {{ user_customisations.name}}, STXihei, -apple-system, BlinkMacSystemFont, Segoe UI, Helvetica, Arial, sans-serif, Apple Color Emoji, Segoe UI Emoji;
+--font-stack: Georgia, {{ user_customisations.name }}, STXihei, -apple-system, BlinkMacSystemFont, Segoe UI, Helvetica, Arial, sans-serif, Apple Color Emoji, Segoe UI Emoji;
 }
 {%- endif %}
 {%- endif %}
 {%- endmacro %}
 
 
 <style>
     {{ declare_font_variables(theme_custom_fonts) }}
 
     html {
         font-family: var(--font-stack);
     }
 
     :root {
-        {{ declare_css_variables(theme_light_css_variables, stmaterial_pygments.light) }}
+        {{ declare_css_variables(theme_css_variables, stmaterial_pygments.light) }}
     }
     :root[theme="dark"] {
         {{ declare_css_variables(theme_dark_css_variables, stmaterial_pygments.dark) }}
     }
 </style>
```

#### html2text {}

```diff
@@ -6,13 +6,13 @@
 {% endfor %} {%- endif %} {%- endmacro %} {% macro declare_font_variables
 (user_customisations) -%} {% if user_customisations -%} {% for src in
 user_customisations.src -%} @font-face { font-family: {
 { user_customisations.name }}; font-weight: {{ src.weight }}; font-style:
 normal; font-display: swap; src: url({{ src.url }}) format({
 { user_customisations.type }}); } {% endfor %} {% if
 user_customisations.font_stack -%} :root { --font-stack: {
-{ user_customisations.font_stack}}, -apple-system, BlinkMacSystemFont, Segoe
+{ user_customisations.font_stack }}, -apple-system, BlinkMacSystemFont, Segoe
 UI, Helvetica, Arial, sans-serif, Apple Color Emoji, Segoe UI Emoji; } {% else
-%} :root { --font-stack: Georgia, {{ user_customisations.name}}, STXihei, -
+%} :root { --font-stack: Georgia, {{ user_customisations.name }}, STXihei, -
 apple-system, BlinkMacSystemFont, Segoe UI, Helvetica, Arial, sans-serif, Apple
 Color Emoji, Segoe UI Emoji; } {%- endif %} {%- endif %} {%- endmacro %}
```

### Comparing `stmaterial-0.0.6/src/stmaterial/theme/stmaterial/partials/_icon_links_declaration.html` & `stmaterial-0.0.7/src/stmaterial/theme/stmaterial/partials/_icon_links_declaration.html`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,14 @@
         {% if icon_dict.class %}
         <i class="{{ icon_dict.class }}"></i>
         {% elif icon_dict.material_icons %}
         <i class="material-icons">{{ icon_dict.material_icons }}</i>
         {% elif icon_dict.fontawesome %}
         <i class="{{ icon_dict.fontawesome }}"></i>
         {% elif icon_dict.image %}
-        <img src="{{ icon_dict.image }}" class="stm-icon-image" alt="{{ icon_dict.name }}">
+        <img src="{{ icon_dict.image }}" class="stm-icon-image" alt="{{ icon_dict.name }}" />
         {% endif %}
     </a>
 </li>
 {% endfor %}
 {%- endif %}
 {%- endmacro %}
```

### Comparing `stmaterial-0.0.6/src/stmaterial/theme/stmaterial/search.html` & `stmaterial-0.0.7/src/stmaterial/theme/stmaterial/search.html`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 {% extends "page.html" %}
 
 {%- block regular_scripts -%}
 {{ super() }}
 <script src="{{ pathto('_static/searchtools.js', 1) }}"></script>
 <script src="{{ pathto('_static/language_data.js', 1) }}"></script>
-{%- endblock regular_scripts-%}
+{%- endblock regular_scripts -%}
 
 {%- block htmltitle -%}
 <title>{{ _("Search") }} - {{ docstitle }}</title>
 {%- endblock htmltitle -%}
 
 {% block body %}
 <noscript>
@@ -27,13 +27,13 @@
     let searchInput = document.querySelector("form.search-wrapper input");
     if (searchInput) {
         searchInput.focus();
         searchInput.select();
         console.log("[PST]: Set focus on search field.");
     }
 </script>
-{% endblock %}
+{% endblock body %}
 
 {% block scripts -%}
 {{ super() }}
 <script src="{{ pathto('searchindex.js', 1) }}"></script>
 {%- endblock scripts %}
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
 {% extends "page.html" %} {%- block regular_scripts -%} {{ super() }}
- {%- endblock regular_scripts-%} {%- block htmltitle -%}
+ {%- endblock regular_scripts -%} {%- block htmltitle -%}
 {%- endblock htmltitle -%} {% block body %}
 {% trans %}Error{% endtrans %}
 {% trans %}Please activate JavaScript to enable the search functionality.{%
 endtrans %}
- {% endblock %} {% block scripts -%} {{ super() }}
+ {% endblock body %} {% block scripts -%} {{ super() }}
  {%- endblock scripts %}
```

### Comparing `stmaterial-0.0.6/src/stmaterial/theme/stmaterial/sections/headnav.html` & `stmaterial-0.0.7/src/stmaterial/theme/stmaterial/sections/headnav.html`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.6/src/stmaterial/theme/stmaterial/sections/sidenav.html` & `stmaterial-0.0.7/src/stmaterial/theme/stmaterial/sections/sidenav.html`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.6/src/stmaterial/theme/stmaterial/static/images/github.svg` & `stmaterial-0.0.7/src/stmaterial/theme/stmaterial/static/images/github.svg`

 * *Files 0% similar despite different names*

```diff
@@ -54,7 +54,8 @@
 00000350: 342e 3839 2032 2e38 3533 2033 2e33 3136  4.89 2.853 3.316
 00000360: 2032 2e33 3634 2031 392e 3431 322d 362e   2.364 19.412-6.
 00000370: 3532 2033 332e 3430 352d 3234 2e39 3335  52 33.405-24.935
 00000380: 2033 332e 3430 352d 3436 2e36 3931 4339   33.405-46.691C9
 00000390: 372e 3730 3720 3232 2037 352e 3738 3820  7.707 22 75.788 
 000003a0: 3020 3438 2e38 3534 2030 7a22 2066 696c  0 48.854 0z" fil
 000003b0: 6c3d 2223 6666 6622 2f3e 3c2f 7376 673e  l="#fff"/></svg>
+000003c0: 0a                                       .
```

### Comparing `stmaterial-0.0.6/src/stmaterial/theme/stmaterial/theme.conf` & `stmaterial-0.0.7/src/stmaterial/theme/stmaterial/theme.conf`

 * *Files 12% similar despite different names*

```diff
@@ -6,30 +6,34 @@
 sidebars = search-field.html, sidenav-nav.html
 # sidebar-end
 
 [options]
 navigation_depth = 4
 show_nav_level = 1
 show_toc_level = 1
-logo = 
+logo =
 header_links_before_dropdown = 4
-external_links = 
+external_links =
 header_icons =
-footer_icons = 
+footer_icons =
 sidenav_icons =
 use_edit_page_button=
 source_repository=
 source_branch =
 source_directory =
 source_edit_link =
 custom_fonts =
 show_prev_next = True
 show_back_to_top = True
-fix_header_nav = 
-light_css_variables =
+fix_header_nav =
+css_variables =
 dark_css_variables =
-footer = 
-footer_content = components/sphinx-version.html, components/copyright.html
-toc_title = 
+footer =
+footer_content = sphinx-version.html, copyright.html
+toc_title =
 search_bar_text = Search the docs ...
 dropdown_label_name = More
 navigation_with_keys = True
+article_top_left = breadcrumbs.html
+article_top_right = sourcelink.html
+article_bottom_left = last-updated.html
+article_bottom_right = edit-this-page.html
```

### Comparing `stmaterial-0.0.6/src/stmaterial/utils.py` & `stmaterial-0.0.7/src/stmaterial/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from sphinx.application import Sphinx
-from typing import Any, Dict, Iterator
+from typing import Iterator
 from docutils.nodes import Node
 
 
-
-def config_provided_by_user(app: Sphinx, key:str) -> bool:
+def config_provided_by_user(app: Sphinx, key: str) -> bool:
     """Check if the user has manually provided the config.
     REMOVE when pydata v0.14 is released and import from there.
     """
     return any(key in ii for ii in [app.config.overrides, app.config._raw_config])
 
 
 def get_theme_options(app: Sphinx):
@@ -24,24 +23,24 @@
     else:
         # Empty dictionary as a fail-safe.
         return {}
 
 
 def activate_extensions(app: Sphinx, extensions):
     """Activate extensions bundled with this theme.
-    
+
     This also manually triggers the `config-inited` build step to account for
     added extensions that hook into this event.
     """
 
     # Remove all of the `config-inited` event listeners because they've already triggered
     # We'll then re-trigger this event after adding extensions so that *only* their event hooks trigger
     old_listeners = app.events.listeners["config-inited"]
     app.events.listeners["config-inited"] = []
-    
+
     for extension in extensions:
         # If it's already been activated just skip it
         if extension in app.config.extensions:
             continue
         app.setup_extension(extension)
 
     # Emit the config-inited event so that the new extensions run their hooks
@@ -57,8 +56,8 @@
     TODO: This check can be removed when the minimum supported docutils version
     for numpydoc is docutils>=0.18.1.
     """
     return (
         node.findall(condition, **kwargs)
         if hasattr(node, "findall")
         else node.traverse(condition, **kwargs)
-    )
+    )
```

### Comparing `stmaterial-0.0.6/webpack.config.js` & `stmaterial-0.0.7/webpack.config.js`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.6/PKG-INFO` & `stmaterial-0.0.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stmaterial
-Version: 0.0.6
+Version: 0.0.7
 Summary: A sphinx theme of materializecss.
 Author-Email: zclab <syfhub@hotmail.com>
 License: MIT License
         
         Copyright (c) 2023 zc
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -38,55 +38,55 @@
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Documentation
 Classifier: Topic :: Software Development :: Documentation
 Project-URL: Repository, https://github.com/zclab/stmaterial
 Project-URL: Documentation, https://stmaterial.readthedocs.io/en/latest/
 Requires-Python: >=3.8
 Requires-Dist: beautifulsoup4
-Requires-Dist: sphinx<7.0,>=5.0
+Requires-Dist: sphinx<8.0,>=5.0
 Requires-Dist: sphinx-basic-ng
 Requires-Dist: pygments>=2.7
 Requires-Dist: sphinx-theme-builder[cli]>=0.2.0b2; extra == "dev"
 Provides-Extra: dev
 Description-Content-Type: text/markdown
 
 <h1 align="center">
   <img src="https://cdn.jsdelivr.net/gh/zclab/stmaterial/docs/_static/logo.png" width="400">
 </h1>
 
 <p align="center">
   <strong>
-    A 
+    A
     <a href="https://materializeweb.com/">Materialize</a> based <a href="https://www.sphinx-doc.org/en/master/">sphinx</a> theme.
   </strong>
 </p>
 
 <!-- [![deploy](https://github.com/zclab/stmaterial/actions/workflows/deploy-docs.yml/badge.svg)](https://zclab.github.io/stmaterial/) -->
+
 [![deploy](https://img.shields.io/readthedocs/stmaterial?style=flat-square&logo=readthedocs&logoColor=white)](https://stmaterial.readthedocs.io/en/latest/)
 [![Downloads](https://img.shields.io/pypi/dm/stmaterial.svg?style=flat-square)](https://pypistats.org/packages/stmaterial)
 [![python](https://img.shields.io/pypi/pyversions/stmaterial.svg?style=flat-square)](https://pypi.org/project/stmaterial/)
 [![PyPI](https://img.shields.io/pypi/v/stmaterial?style=flat-square&logo=python&logoColor=white&color=orange)](https://pypi.org/project/stmaterial/)
 [![status](https://img.shields.io/pypi/status/stmaterial.svg?style=flat-square)](https://pypi.org/project/stmaterial/)
 [![license](https://img.shields.io/pypi/l/stmaterial.svg?style=flat-square&logo=opensourceinitiative&logoColor=white)](https://github.com/zclab/stmaterial/blob/main/LICENSE)
 
-
 ## Installation and usage
 
 <!-- start quickstart -->
 
 To use this theme in the repository, follow these steps:
 
 1. Install the `stmaterial` in your doc build environment:
-   
-    ```
-    pip install stmaterial
-    ```
+
+   ```
+   pip install stmaterial
+   ```
 
 2. Configure the Sphinx docs to use the theme by editing `conf.py`
 
-    ```python
-    html_theme = "stmaterial"
-    ```
+   ```python
+   html_theme = "stmaterial"
+   ```
 
 3. Your Sphinx documentation's HTML pages will now be generated with this theme! 🎉
 
 <!-- end quickstart -->
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: stmaterial Version: 0.0.6 Summary: A sphinx theme
+Metadata-Version: 2.1 Name: stmaterial Version: 0.0.7 Summary: A sphinx theme
 of materializecss. Author-Email: zclab
 hotmail.com> License: MIT License Copyright (c) 2023 zc Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
@@ -21,15 +21,15 @@
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Operating System :: OS Independent Classifier: Topic
 :: Documentation Classifier: Topic :: Software Development :: Documentation
 Project-URL: Repository, https://github.com/zclab/stmaterial Project-URL:
 Documentation, https://stmaterial.readthedocs.io/en/latest/ Requires-Python:
->=3.8 Requires-Dist: beautifulsoup4 Requires-Dist: sphinx<7.0,>=5.0 Requires-
+>=3.8 Requires-Dist: beautifulsoup4 Requires-Dist: sphinx<8.0,>=5.0 Requires-
 Dist: sphinx-basic-ng Requires-Dist: pygments>=2.7 Requires-Dist: sphinx-theme-
 builder[cli]>=0.2.0b2; extra == "dev" Provides-Extra: dev Description-Content-
 Type: text/markdown
   ****** [https://cdn.jsdelivr.net/gh/zclab/stmaterial/docs/_static/logo.png]
                                     ******
                        A Materialize based sphinx theme.
  [![deploy](https://img.shields.io/readthedocs/stmaterial?style=flat-
```

