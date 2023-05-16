# Comparing `tmp/labelme-5.2.1.tar.gz` & `tmp/labelme-5.3.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labelme-5.2.1.tar", last modified: Tue May 16 15:06:28 2023, max compression
+gzip compressed data, was "labelme-5.3.0a0.tar", last modified: Tue May 16 15:09:12 2023, max compression
```

## Comparing `labelme-5.2.1.tar` & `labelme-5.3.0a0.tar`

### file list

```diff
@@ -1,88 +1,93 @@
-drwxr-xr-x   0 wkentaro   (501) staff       (20)        0 2023-05-16 15:06:28.608505 labelme-5.2.1/
--rw-r--r--   0 wkentaro   (501) staff       (20)      692 2023-04-16 12:20:20.000000 labelme-5.2.1/LICENSE
--rw-r--r--   0 wkentaro   (501) staff       (20)       18 2023-04-16 12:20:20.000000 labelme-5.2.1/MANIFEST.in
--rw-r--r--   0 wkentaro   (501) staff       (20)    10956 2023-05-16 15:06:28.608314 labelme-5.2.1/PKG-INFO
--rw-r--r--   0 wkentaro   (501) staff       (20)     8746 2023-04-16 12:20:20.000000 labelme-5.2.1/README.md
-drwxr-xr-x   0 wkentaro   (501) staff       (20)        0 2023-05-16 15:06:28.592389 labelme-5.2.1/labelme/
--rw-r--r--   0 wkentaro   (501) staff       (20)      668 2023-05-16 15:06:16.000000 labelme-5.2.1/labelme/__init__.py
--rw-r--r--   0 wkentaro   (501) staff       (20)     5792 2023-04-16 13:33:53.000000 labelme-5.2.1/labelme/__main__.py
--rw-r--r--   0 wkentaro   (501) staff       (20)    73759 2023-05-16 15:05:56.000000 labelme-5.2.1/labelme/app.py
-drwxr-xr-x   0 wkentaro   (501) staff       (20)        0 2023-05-16 15:06:28.594494 labelme-5.2.1/labelme/cli/
--rw-r--r--   0 wkentaro   (501) staff       (20)      123 2023-04-16 12:20:20.000000 labelme-5.2.1/labelme/cli/__init__.py
--rw-r--r--   0 wkentaro   (501) staff       (20)     1345 2023-04-16 12:20:20.000000 labelme-5.2.1/labelme/cli/draw_json.py
--rw-r--r--   0 wkentaro   (501) staff       (20)      636 2023-04-16 12:20:20.000000 labelme-5.2.1/labelme/cli/draw_label_png.py
--rw-r--r--   0 wkentaro   (501) staff       (20)     2388 2023-04-16 12:20:20.000000 labelme-5.2.1/labelme/cli/json_to_dataset.py
--rw-r--r--   0 wkentaro   (501) staff       (20)     2749 2023-04-16 12:20:20.000000 labelme-5.2.1/labelme/cli/on_docker.py
-drwxr-xr-x   0 wkentaro   (501) staff       (20)        0 2023-05-16 15:06:28.594805 labelme-5.2.1/labelme/config/
--rw-r--r--   0 wkentaro   (501) staff       (20)     2698 2023-04-16 12:20:20.000000 labelme-5.2.1/labelme/config/__init__.py
--rw-r--r--   0 wkentaro   (501) staff       (20)     2203 2023-05-16 15:05:56.000000 labelme-5.2.1/labelme/config/default_config.yaml
-drwxr-xr-x   0 wkentaro   (501) staff       (20)        0 2023-05-16 15:06:28.605839 labelme-5.2.1/labelme/icons/
--rw-r--r--   0 wkentaro   (501) staff       (20)     2136 2023-04-16 12:20:20.000000 labelme-5.2.1/labelme/icons/cancel.png
--rw-r--r--   0 wkentaro   (501) staff       (20)     3111 2023-04-16 12:20:20.000000 labelme-5.2.1/labelme/icons/close.png
--rw-r--r--   0 wkentaro   (501) staff       (20)     2368 2023-04-16 12:20:20.000000 labelme-5.2.1/labelme/icons/color-line.png
--rw-r--r--   0 wkentaro   (501) staff       (20)     1461 2023-04-16 12:20:20.000000 labelme-5.2.1/labelme/icons/color.png
--rw-r--r--   0 wkentaro   (501) staff       (20)      646 2023-04-16 12:20:20.000000 labelme-5.2.1/labelme/icons/copy.png
--rw-r--r--   0 wkentaro   (501) staff       (20)     1486 2023-04-16 12:20:20.000000 labelme-5.2.1/labelme/icons/delete.png
--rw-r--r--   0 wkentaro   (501) staff       (20)     2198 2023-04-16 12:20:20.000000 labelme-5.2.1/labelme/icons/done.png
--rw-r--r--   0 wkentaro   (501) staff       (20)    22232 2023-04-16 12:20:20.000000 labelme-5.2.1/labelme/icons/done.svg
--rw-r--r--   0 wkentaro   (501) staff       (20)     1092 2023-04-16 12:20:20.000000 labelme-5.2.1/labelme/icons/edit.png
--rw-r--r--   0 wkentaro   (501) staff       (20)     7718 2023-04-16 12:20:20.000000 labelme-5.2.1/labelme/icons/expert.png
--rw-r--r--   0 wkentaro   (501) staff       (20)     1264 2023-04-16 12:20:20.000000 labelme-5.2.1/labelme/icons/eye.png
--rw-r--r--   0 wkentaro   (501) staff       (20)     8059 2023-04-16 12:20:20.000000 labelme-5.2.1/labelme/icons/feBlend-icon.png
--rw-r--r--   0 wkentaro   (501) staff       (20)      765 2023-04-16 12:20:20.000000 labelme-5.2.1/labelme/icons/file.png
--rw-r--r--   0 wkentaro   (501) staff       (20)     1365 2023-04-16 12:20:20.000000 labelme-5.2.1/labelme/icons/fit-width.png
--rw-r--r--   0 wkentaro   (501) staff       (20)     1102 2023-04-16 12:20:20.000000 labelme-5.2.1/labelme/icons/fit-window.png
--rw-r--r--   0 wkentaro   (501) staff       (20)     2262 2023-04-16 12:20:20.000000 labelme-5.2.1/labelme/icons/fit.png
--rw-r--r--   0 wkentaro   (501) staff       (20)     1587 2023-04-16 12:20:20.000000 labelme-5.2.1/labelme/icons/help.png
--rw-r--r--   0 wkentaro   (501) staff       (20)  1128131 2023-04-16 12:20:20.000000 labelme-5.2.1/labelme/icons/icon.icns
--rw-r--r--   0 wkentaro   (501) staff       (20)   183198 2023-04-16 12:20:20.000000 labelme-5.2.1/labelme/icons/icon.ico
--rw-r--r--   0 wkentaro   (501) staff       (20)    44771 2023-04-16 12:20:20.000000 labelme-5.2.1/labelme/icons/icon.png
--rw-r--r--   0 wkentaro   (501) staff       (20)     2381 2023-04-16 12:20:20.000000 labelme-5.2.1/labelme/icons/labels.png
--rw-r--r--   0 wkentaro   (501) staff       (20)    36694 2023-04-16 12:20:20.000000 labelme-5.2.1/labelme/icons/labels.svg
--rw-r--r--   0 wkentaro   (501) staff       (20)      977 2023-04-16 12:20:20.000000 labelme-5.2.1/labelme/icons/new.png
--rw-r--r--   0 wkentaro   (501) staff       (20)    30288 2023-04-16 12:20:20.000000 labelme-5.2.1/labelme/icons/next.png
--rw-r--r--   0 wkentaro   (501) staff       (20)     1103 2023-04-16 12:20:20.000000 labelme-5.2.1/labelme/icons/objects.png
--rw-r--r--   0 wkentaro   (501) staff       (20)     2073 2023-04-16 12:20:20.000000 labelme-5.2.1/labelme/icons/open.png
--rw-r--r--   0 wkentaro   (501) staff       (20)    18197 2023-04-16 12:20:20.000000 labelme-5.2.1/labelme/icons/open.svg
--rw-r--r--   0 wkentaro   (501) staff       (20)    30665 2023-04-16 12:20:20.000000 labelme-5.2.1/labelme/icons/prev.png
--rw-r--r--   0 wkentaro   (501) staff       (20)     1915 2023-04-16 12:20:20.000000 labelme-5.2.1/labelme/icons/quit.png
--rw-r--r--   0 wkentaro   (501) staff       (20)     2811 2023-04-16 12:20:20.000000 labelme-5.2.1/labelme/icons/save-as.png
--rw-r--r--   0 wkentaro   (501) staff       (20)    64005 2023-04-16 12:20:20.000000 labelme-5.2.1/labelme/icons/save-as.svg
--rw-r--r--   0 wkentaro   (501) staff       (20)     1187 2023-04-16 12:20:20.000000 labelme-5.2.1/labelme/icons/save.png
--rw-r--r--   0 wkentaro   (501) staff       (20)    30613 2023-04-16 12:20:20.000000 labelme-5.2.1/labelme/icons/save.svg
--rw-r--r--   0 wkentaro   (501) staff       (20)     2004 2023-04-16 12:20:20.000000 labelme-5.2.1/labelme/icons/undo-cross.png
--rw-r--r--   0 wkentaro   (501) staff       (20)     2018 2023-04-16 12:20:20.000000 labelme-5.2.1/labelme/icons/undo.png
--rw-r--r--   0 wkentaro   (501) staff       (20)     1099 2023-04-16 12:20:20.000000 labelme-5.2.1/labelme/icons/zoom-in.png
--rw-r--r--   0 wkentaro   (501) staff       (20)     1074 2023-04-16 12:20:20.000000 labelme-5.2.1/labelme/icons/zoom-out.png
--rw-r--r--   0 wkentaro   (501) staff       (20)     1139 2023-04-16 12:20:20.000000 labelme-5.2.1/labelme/icons/zoom.png
--rw-r--r--   0 wkentaro   (501) staff       (20)     6435 2023-05-16 15:05:56.000000 labelme-5.2.1/labelme/label_file.py
--rw-r--r--   0 wkentaro   (501) staff       (20)     1836 2023-05-16 15:05:56.000000 labelme-5.2.1/labelme/logger.py
--rw-r--r--   0 wkentaro   (501) staff       (20)    10149 2023-05-16 15:05:56.000000 labelme-5.2.1/labelme/shape.py
--rw-r--r--   0 wkentaro   (501) staff       (20)      849 2023-04-16 12:20:20.000000 labelme-5.2.1/labelme/testing.py
-drwxr-xr-x   0 wkentaro   (501) staff       (20)        0 2023-05-16 15:06:28.606446 labelme-5.2.1/labelme/utils/
--rw-r--r--   0 wkentaro   (501) staff       (20)      722 2023-05-16 15:05:56.000000 labelme-5.2.1/labelme/utils/__init__.py
--rw-r--r--   0 wkentaro   (501) staff       (20)      675 2023-04-16 12:20:20.000000 labelme-5.2.1/labelme/utils/_io.py
--rw-r--r--   0 wkentaro   (501) staff       (20)     2367 2023-05-16 15:05:56.000000 labelme-5.2.1/labelme/utils/image.py
--rw-r--r--   0 wkentaro   (501) staff       (20)     2392 2023-05-16 15:05:56.000000 labelme-5.2.1/labelme/utils/qt.py
--rw-r--r--   0 wkentaro   (501) staff       (20)     3650 2023-04-16 12:20:20.000000 labelme-5.2.1/labelme/utils/shape.py
-drwxr-xr-x   0 wkentaro   (501) staff       (20)        0 2023-05-16 15:06:28.608007 labelme-5.2.1/labelme/widgets/
--rw-r--r--   0 wkentaro   (501) staff       (20)      510 2023-04-16 12:20:20.000000 labelme-5.2.1/labelme/widgets/__init__.py
--rw-r--r--   0 wkentaro   (501) staff       (20)     1468 2023-04-16 12:20:20.000000 labelme-5.2.1/labelme/widgets/brightness_contrast_dialog.py
--rw-r--r--   0 wkentaro   (501) staff       (20)    33601 2023-05-16 15:05:56.000000 labelme-5.2.1/labelme/widgets/canvas.py
--rw-r--r--   0 wkentaro   (501) staff       (20)     1200 2023-04-16 12:20:20.000000 labelme-5.2.1/labelme/widgets/color_dialog.py
--rw-r--r--   0 wkentaro   (501) staff       (20)      281 2023-04-16 12:20:20.000000 labelme-5.2.1/labelme/widgets/escapable_qlist_widget.py
--rw-r--r--   0 wkentaro   (501) staff       (20)     2434 2023-04-16 12:20:20.000000 labelme-5.2.1/labelme/widgets/file_dialog_preview.py
--rw-r--r--   0 wkentaro   (501) staff       (20)     8780 2023-04-16 12:20:20.000000 labelme-5.2.1/labelme/widgets/label_dialog.py
--rw-r--r--   0 wkentaro   (501) staff       (20)     5792 2023-04-16 12:20:20.000000 labelme-5.2.1/labelme/widgets/label_list_widget.py
--rw-r--r--   0 wkentaro   (501) staff       (20)      970 2023-04-16 12:20:20.000000 labelme-5.2.1/labelme/widgets/tool_bar.py
--rw-r--r--   0 wkentaro   (501) staff       (20)     1374 2023-04-16 12:20:20.000000 labelme-5.2.1/labelme/widgets/unique_label_qlist_widget.py
--rw-r--r--   0 wkentaro   (501) staff       (20)      712 2023-05-10 12:16:05.000000 labelme-5.2.1/labelme/widgets/zoom_widget.py
-drwxr-xr-x   0 wkentaro   (501) staff       (20)        0 2023-05-16 15:06:28.593403 labelme-5.2.1/labelme.egg-info/
--rw-r--r--   0 wkentaro   (501) staff       (20)    10956 2023-05-16 15:06:28.000000 labelme-5.2.1/labelme.egg-info/PKG-INFO
--rw-r--r--   0 wkentaro   (501) staff       (20)     1984 2023-05-16 15:06:28.000000 labelme-5.2.1/labelme.egg-info/SOURCES.txt
--rw-r--r--   0 wkentaro   (501) staff       (20)        1 2023-05-16 15:06:28.000000 labelme-5.2.1/labelme.egg-info/dependency_links.txt
--rw-r--r--   0 wkentaro   (501) staff       (20)      260 2023-05-16 15:06:28.000000 labelme-5.2.1/labelme.egg-info/entry_points.txt
--rw-r--r--   0 wkentaro   (501) staff       (20)       87 2023-05-16 15:06:28.000000 labelme-5.2.1/labelme.egg-info/requires.txt
--rw-r--r--   0 wkentaro   (501) staff       (20)        8 2023-05-16 15:06:28.000000 labelme-5.2.1/labelme.egg-info/top_level.txt
--rw-r--r--   0 wkentaro   (501) staff       (20)       38 2023-05-16 15:06:28.608547 labelme-5.2.1/setup.cfg
--rw-r--r--   0 wkentaro   (501) staff       (20)     4533 2023-05-16 15:05:56.000000 labelme-5.2.1/setup.py
+drwxr-xr-x   0 wkentaro   (501) staff       (20)        0 2023-05-16 15:09:12.209357 labelme-5.3.0a0/
+-rw-r--r--   0 wkentaro   (501) staff       (20)      692 2023-04-16 12:20:20.000000 labelme-5.3.0a0/LICENSE
+-rw-r--r--   0 wkentaro   (501) staff       (20)       18 2023-04-16 12:20:20.000000 labelme-5.3.0a0/MANIFEST.in
+-rw-r--r--   0 wkentaro   (501) staff       (20)    10958 2023-05-16 15:09:12.209162 labelme-5.3.0a0/PKG-INFO
+-rw-r--r--   0 wkentaro   (501) staff       (20)     8746 2023-04-16 12:20:20.000000 labelme-5.3.0a0/README.md
+drwxr-xr-x   0 wkentaro   (501) staff       (20)        0 2023-05-16 15:09:12.200081 labelme-5.3.0a0/labelme/
+-rw-r--r--   0 wkentaro   (501) staff       (20)      670 2023-05-16 15:08:59.000000 labelme-5.3.0a0/labelme/__init__.py
+-rw-r--r--   0 wkentaro   (501) staff       (20)     5792 2023-04-16 13:33:53.000000 labelme-5.3.0a0/labelme/__main__.py
+drwxr-xr-x   0 wkentaro   (501) staff       (20)        0 2023-05-16 15:09:12.200959 labelme-5.3.0a0/labelme/ai/
+-rw-r--r--   0 wkentaro   (501) staff       (20)     1804 2023-05-16 15:08:51.000000 labelme-5.3.0a0/labelme/ai/__init__.py
+drwxr-xr-x   0 wkentaro   (501) staff       (20)        0 2023-05-16 15:09:12.201178 labelme-5.3.0a0/labelme/ai/models/
+-rw-r--r--   0 wkentaro   (501) staff       (20)        0 2023-05-16 15:08:51.000000 labelme-5.3.0a0/labelme/ai/models/__init__.py
+-rw-r--r--   0 wkentaro   (501) staff       (20)     6007 2023-05-16 15:08:51.000000 labelme-5.3.0a0/labelme/ai/models/segment_anything.py
+-rw-r--r--   0 wkentaro   (501) staff       (20)    77318 2023-05-16 15:08:51.000000 labelme-5.3.0a0/labelme/app.py
+drwxr-xr-x   0 wkentaro   (501) staff       (20)        0 2023-05-16 15:09:12.201743 labelme-5.3.0a0/labelme/cli/
+-rw-r--r--   0 wkentaro   (501) staff       (20)      123 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/cli/__init__.py
+-rw-r--r--   0 wkentaro   (501) staff       (20)     1345 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/cli/draw_json.py
+-rw-r--r--   0 wkentaro   (501) staff       (20)      636 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/cli/draw_label_png.py
+-rw-r--r--   0 wkentaro   (501) staff       (20)     2388 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/cli/json_to_dataset.py
+-rw-r--r--   0 wkentaro   (501) staff       (20)     2749 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/cli/on_docker.py
+drwxr-xr-x   0 wkentaro   (501) staff       (20)        0 2023-05-16 15:09:12.202037 labelme-5.3.0a0/labelme/config/
+-rw-r--r--   0 wkentaro   (501) staff       (20)     2698 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/config/__init__.py
+-rw-r--r--   0 wkentaro   (501) staff       (20)     2230 2023-05-16 15:08:51.000000 labelme-5.3.0a0/labelme/config/default_config.yaml
+drwxr-xr-x   0 wkentaro   (501) staff       (20)        0 2023-05-16 15:09:12.207135 labelme-5.3.0a0/labelme/icons/
+-rw-r--r--   0 wkentaro   (501) staff       (20)     2136 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/icons/cancel.png
+-rw-r--r--   0 wkentaro   (501) staff       (20)     3111 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/icons/close.png
+-rw-r--r--   0 wkentaro   (501) staff       (20)     2368 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/icons/color-line.png
+-rw-r--r--   0 wkentaro   (501) staff       (20)     1461 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/icons/color.png
+-rw-r--r--   0 wkentaro   (501) staff       (20)      646 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/icons/copy.png
+-rw-r--r--   0 wkentaro   (501) staff       (20)     1486 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/icons/delete.png
+-rw-r--r--   0 wkentaro   (501) staff       (20)     2198 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/icons/done.png
+-rw-r--r--   0 wkentaro   (501) staff       (20)    22232 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/icons/done.svg
+-rw-r--r--   0 wkentaro   (501) staff       (20)     1092 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/icons/edit.png
+-rw-r--r--   0 wkentaro   (501) staff       (20)     7718 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/icons/expert.png
+-rw-r--r--   0 wkentaro   (501) staff       (20)     1264 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/icons/eye.png
+-rw-r--r--   0 wkentaro   (501) staff       (20)     8059 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/icons/feBlend-icon.png
+-rw-r--r--   0 wkentaro   (501) staff       (20)      765 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/icons/file.png
+-rw-r--r--   0 wkentaro   (501) staff       (20)     1365 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/icons/fit-width.png
+-rw-r--r--   0 wkentaro   (501) staff       (20)     1102 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/icons/fit-window.png
+-rw-r--r--   0 wkentaro   (501) staff       (20)     2262 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/icons/fit.png
+-rw-r--r--   0 wkentaro   (501) staff       (20)     1587 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/icons/help.png
+-rw-r--r--   0 wkentaro   (501) staff       (20)  1128131 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/icons/icon.icns
+-rw-r--r--   0 wkentaro   (501) staff       (20)   183198 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/icons/icon.ico
+-rw-r--r--   0 wkentaro   (501) staff       (20)    44771 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/icons/icon.png
+-rw-r--r--   0 wkentaro   (501) staff       (20)     2381 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/icons/labels.png
+-rw-r--r--   0 wkentaro   (501) staff       (20)    36694 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/icons/labels.svg
+-rw-r--r--   0 wkentaro   (501) staff       (20)      977 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/icons/new.png
+-rw-r--r--   0 wkentaro   (501) staff       (20)    30288 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/icons/next.png
+-rw-r--r--   0 wkentaro   (501) staff       (20)     1103 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/icons/objects.png
+-rw-r--r--   0 wkentaro   (501) staff       (20)     2073 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/icons/open.png
+-rw-r--r--   0 wkentaro   (501) staff       (20)    18197 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/icons/open.svg
+-rw-r--r--   0 wkentaro   (501) staff       (20)    30665 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/icons/prev.png
+-rw-r--r--   0 wkentaro   (501) staff       (20)     1915 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/icons/quit.png
+-rw-r--r--   0 wkentaro   (501) staff       (20)     2811 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/icons/save-as.png
+-rw-r--r--   0 wkentaro   (501) staff       (20)    64005 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/icons/save-as.svg
+-rw-r--r--   0 wkentaro   (501) staff       (20)     1187 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/icons/save.png
+-rw-r--r--   0 wkentaro   (501) staff       (20)    30613 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/icons/save.svg
+-rw-r--r--   0 wkentaro   (501) staff       (20)     2004 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/icons/undo-cross.png
+-rw-r--r--   0 wkentaro   (501) staff       (20)     2018 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/icons/undo.png
+-rw-r--r--   0 wkentaro   (501) staff       (20)     1099 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/icons/zoom-in.png
+-rw-r--r--   0 wkentaro   (501) staff       (20)     1074 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/icons/zoom-out.png
+-rw-r--r--   0 wkentaro   (501) staff       (20)     1139 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/icons/zoom.png
+-rw-r--r--   0 wkentaro   (501) staff       (20)     5809 2023-05-16 15:08:51.000000 labelme-5.3.0a0/labelme/label_file.py
+-rw-r--r--   0 wkentaro   (501) staff       (20)     1633 2023-05-16 15:08:51.000000 labelme-5.3.0a0/labelme/logger.py
+-rw-r--r--   0 wkentaro   (501) staff       (20)    11626 2023-05-16 15:08:51.000000 labelme-5.3.0a0/labelme/shape.py
+-rw-r--r--   0 wkentaro   (501) staff       (20)      849 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/testing.py
+drwxr-xr-x   0 wkentaro   (501) staff       (20)        0 2023-05-16 15:09:12.207700 labelme-5.3.0a0/labelme/utils/
+-rw-r--r--   0 wkentaro   (501) staff       (20)      755 2023-05-16 15:08:51.000000 labelme-5.3.0a0/labelme/utils/__init__.py
+-rw-r--r--   0 wkentaro   (501) staff       (20)      675 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/utils/_io.py
+-rw-r--r--   0 wkentaro   (501) staff       (20)     2619 2023-05-16 15:08:51.000000 labelme-5.3.0a0/labelme/utils/image.py
+-rw-r--r--   0 wkentaro   (501) staff       (20)     2414 2023-05-16 15:08:51.000000 labelme-5.3.0a0/labelme/utils/qt.py
+-rw-r--r--   0 wkentaro   (501) staff       (20)     3650 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/utils/shape.py
+drwxr-xr-x   0 wkentaro   (501) staff       (20)        0 2023-05-16 15:09:12.208980 labelme-5.3.0a0/labelme/widgets/
+-rw-r--r--   0 wkentaro   (501) staff       (20)      510 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/widgets/__init__.py
+-rw-r--r--   0 wkentaro   (501) staff       (20)     1468 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/widgets/brightness_contrast_dialog.py
+-rw-r--r--   0 wkentaro   (501) staff       (20)    38987 2023-05-16 15:08:51.000000 labelme-5.3.0a0/labelme/widgets/canvas.py
+-rw-r--r--   0 wkentaro   (501) staff       (20)     1200 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/widgets/color_dialog.py
+-rw-r--r--   0 wkentaro   (501) staff       (20)      281 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/widgets/escapable_qlist_widget.py
+-rw-r--r--   0 wkentaro   (501) staff       (20)     2434 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/widgets/file_dialog_preview.py
+-rw-r--r--   0 wkentaro   (501) staff       (20)     8780 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/widgets/label_dialog.py
+-rw-r--r--   0 wkentaro   (501) staff       (20)     5792 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/widgets/label_list_widget.py
+-rw-r--r--   0 wkentaro   (501) staff       (20)      970 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/widgets/tool_bar.py
+-rw-r--r--   0 wkentaro   (501) staff       (20)     1374 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/widgets/unique_label_qlist_widget.py
+-rw-r--r--   0 wkentaro   (501) staff       (20)      712 2023-05-10 12:16:05.000000 labelme-5.3.0a0/labelme/widgets/zoom_widget.py
+drwxr-xr-x   0 wkentaro   (501) staff       (20)        0 2023-05-16 15:09:12.200841 labelme-5.3.0a0/labelme.egg-info/
+-rw-r--r--   0 wkentaro   (501) staff       (20)    10958 2023-05-16 15:09:12.000000 labelme-5.3.0a0/labelme.egg-info/PKG-INFO
+-rw-r--r--   0 wkentaro   (501) staff       (20)     2075 2023-05-16 15:09:12.000000 labelme-5.3.0a0/labelme.egg-info/SOURCES.txt
+-rw-r--r--   0 wkentaro   (501) staff       (20)        1 2023-05-16 15:09:12.000000 labelme-5.3.0a0/labelme.egg-info/dependency_links.txt
+-rw-r--r--   0 wkentaro   (501) staff       (20)      260 2023-05-16 15:09:12.000000 labelme-5.3.0a0/labelme.egg-info/entry_points.txt
+-rw-r--r--   0 wkentaro   (501) staff       (20)      126 2023-05-16 15:09:12.000000 labelme-5.3.0a0/labelme.egg-info/requires.txt
+-rw-r--r--   0 wkentaro   (501) staff       (20)        8 2023-05-16 15:09:12.000000 labelme-5.3.0a0/labelme.egg-info/top_level.txt
+-rw-r--r--   0 wkentaro   (501) staff       (20)       38 2023-05-16 15:09:12.209433 labelme-5.3.0a0/setup.cfg
+-rw-r--r--   0 wkentaro   (501) staff       (20)     4605 2023-05-16 15:08:51.000000 labelme-5.3.0a0/setup.py
```

### Comparing `labelme-5.2.1/LICENSE` & `labelme-5.3.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `labelme-5.2.1/PKG-INFO` & `labelme-5.3.0a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labelme
-Version: 5.2.1
+Version: 5.3.0a0
 Summary: Image Polygonal Annotation with Python
 Home-page: https://github.com/wkentaro/labelme
 Author: Kentaro Wada
 Author-email: www.kentaro.wada@gmail.com
 License: GPLv3
 Keywords: Image Annotation,Machine Learning
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: labelme Version: 5.2.1 Summary: Image Polygonal
+Metadata-Version: 2.1 Name: labelme Version: 5.3.0a0 Summary: Image Polygonal
 Annotation with Python Home-page: https://github.com/wkentaro/labelme Author:
 Kentaro Wada Author-email: www.kentaro.wada@gmail.com License: GPLv3 Keywords:
 Image Annotation,Machine Learning Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Science/Research Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python Classifier: Programming Language :: Python :: 3.5 Classifier:
```

### Comparing `labelme-5.2.1/README.md` & `labelme-5.3.0a0/README.md`

 * *Files identical despite different names*

### Comparing `labelme-5.2.1/labelme/__init__.py` & `labelme-5.3.0a0/labelme/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 __appname__ = "labelme"
 
 # Semantic Versioning 2.0.0: https://semver.org/
 # 1. MAJOR version when you make incompatible API changes;
 # 2. MINOR version when you add functionality in a backwards-compatible manner;
 # 3. PATCH version when you make backwards-compatible bug fixes.
 # e.g., 1.0.0a0, 1.0.0a1, 1.0.0b0, 1.0.0rc0, 1.0.0, 1.0.0.post0
-__version__ = "5.2.1"
+__version__ = "5.3.0a0"
 
 QT4 = QT_VERSION[0] == "4"
 QT5 = QT_VERSION[0] == "5"
 del QT_VERSION
 
 PY2 = sys.version[0] == "2"
 PY3 = sys.version[0] == "3"
```

### Comparing `labelme-5.2.1/labelme/__main__.py` & `labelme-5.3.0a0/labelme/__main__.py`

 * *Files identical despite different names*

### Comparing `labelme-5.2.1/labelme/app.py` & `labelme-5.3.0a0/labelme/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from qtpy import QtGui
 from qtpy import QtWidgets
 
 from labelme import __appname__
 from labelme import PY2
 
 from . import utils
+from labelme.ai import MODELS
 from labelme.config import get_config
 from labelme.label_file import LabelFile
 from labelme.label_file import LabelFileError
 from labelme.logger import logger
 from labelme.shape import Shape
 from labelme.widgets import BrightnessContrastDialog
 from labelme.widgets import Canvas
@@ -363,14 +364,22 @@
             self.tr("Create LineStrip"),
             lambda: self.toggleDrawMode(False, createMode="linestrip"),
             shortcuts["create_linestrip"],
             "objects",
             self.tr("Start drawing linestrip. Ctrl+LeftClick ends creation."),
             enabled=False,
         )
+        createAiPolygonMode = action(
+            self.tr("Create AI-Polygon"),
+            lambda: self.toggleDrawMode(False, createMode="ai_polygon"),
+            None,
+            "objects",
+            self.tr("Start drawing ai_polygon. Ctrl+LeftClick ends creation."),
+            enabled=False,
+        )
         editMode = action(
             self.tr("Edit Polygons"),
             self.setEditMode,
             shortcuts["edit_polygon"],
             "edit",
             self.tr("Move and edit the selected polygons"),
             enabled=False,
@@ -453,15 +462,22 @@
             self.tr("&Tutorial"),
             self.tutorial,
             icon="help",
             tip=self.tr("Show tutorial page"),
         )
 
         zoom = QtWidgets.QWidgetAction(self)
-        zoom.setDefaultWidget(self.zoomWidget)
+        zoomBoxLayout = QtWidgets.QVBoxLayout()
+        zoomBoxLayout.addWidget(self.zoomWidget)
+        zoomLabel = QtWidgets.QLabel("Zoom")
+        zoomLabel.setAlignment(Qt.AlignCenter)
+        zoomLabel.setFont(QtGui.QFont(None, 10))
+        zoomBoxLayout.addWidget(zoomLabel)
+        zoom.setDefaultWidget(QtWidgets.QWidget())
+        zoom.defaultWidget().setLayout(zoomBoxLayout)
         self.zoomWidget.setWhatsThis(
             str(
                 self.tr(
                     "Zoom in or out of the image. Also accessible with "
                     "{} and {} from the canvas."
                 )
             ).format(
@@ -563,15 +579,16 @@
             self.canvas.setFillDrawing,
             None,
             "color",
             self.tr("Fill polygon while drawing"),
             checkable=True,
             enabled=True,
         )
-        fill_drawing.trigger()
+        if self._config["canvas"]["fill_drawing"]:
+            fill_drawing.trigger()
 
         # Lavel list context menu.
         labelMenu = QtWidgets.QMenu()
         utils.addActions(labelMenu, (edit, delete))
         self.labelList.setContextMenuPolicy(Qt.CustomContextMenu)
         self.labelList.customContextMenuRequested.connect(
             self.popLabelListMenu
@@ -599,14 +616,15 @@
             createMode=createMode,
             editMode=editMode,
             createRectangleMode=createRectangleMode,
             createCircleMode=createCircleMode,
             createLineMode=createLineMode,
             createPointMode=createPointMode,
             createLineStripMode=createLineStripMode,
+            createAiPolygonMode=createAiPolygonMode,
             zoom=zoom,
             zoomIn=zoomIn,
             zoomOut=zoomOut,
             zoomOrg=zoomOrg,
             keepPrevScale=keepPrevScale,
             fitWindow=fitWindow,
             fitWidth=fitWidth,
@@ -633,14 +651,15 @@
             menu=(
                 createMode,
                 createRectangleMode,
                 createCircleMode,
                 createLineMode,
                 createPointMode,
                 createLineStripMode,
+                createAiPolygonMode,
                 editMode,
                 edit,
                 duplicate,
                 copy,
                 paste,
                 delete,
                 undo,
@@ -651,14 +670,15 @@
                 close,
                 createMode,
                 createRectangleMode,
                 createCircleMode,
                 createLineMode,
                 createPointMode,
                 createLineStripMode,
+                createAiPolygonMode,
                 editMode,
                 brightnessContrast,
             ),
             onShapesPresent=(saveAs, hideAll, showAll),
         )
 
         self.canvas.vertexSelected.connect(self.actions.removePoint.setEnabled)
@@ -725,16 +745,35 @@
             self.canvas.menus[1],
             (
                 action("&Copy here", self.copyShape),
                 action("&Move here", self.moveShape),
             ),
         )
 
+        selectAiModel = QtWidgets.QWidgetAction(self)
+        selectAiModel.setDefaultWidget(QtWidgets.QWidget())
+        selectAiModel.defaultWidget().setLayout(QtWidgets.QVBoxLayout())
+        self._selectAiModelComboBox = QtWidgets.QComboBox()
+        selectAiModel.defaultWidget().layout().addWidget(
+            self._selectAiModelComboBox
+        )
+        self._selectAiModelComboBox.addItems([model.name for model in MODELS])
+        self._selectAiModelComboBox.setCurrentIndex(1)
+        self._selectAiModelComboBox.setEnabled(False)
+        self._selectAiModelComboBox.currentIndexChanged.connect(
+            lambda: self.canvas.initializeAiModel(
+                name=self._selectAiModelComboBox.currentText()
+            )
+        )
+        selectAiModelLabel = QtWidgets.QLabel(self.tr("AI Model"))
+        selectAiModelLabel.setAlignment(QtCore.Qt.AlignCenter)
+        selectAiModelLabel.setFont(QtGui.QFont(None, 10))
+        selectAiModel.defaultWidget().layout().addWidget(selectAiModelLabel)
+
         self.tools = self.toolbar("Tools")
-        # Menu buttons on Left
         self.actions.tool = (
             open_,
             opendir,
             openNextImg,
             openPrevImg,
             save,
             deleteFile,
@@ -746,14 +785,16 @@
             paste,
             delete,
             undo,
             brightnessContrast,
             None,
             zoom,
             fitWidth,
+            None,
+            selectAiModel,
         )
 
         self.statusBar().showMessage(str(self.tr("%s started.")) % __appname__)
         self.statusBar().show()
 
         if output_file is not None and self._config["auto_save"]:
             logger.warn(
@@ -826,15 +867,15 @@
     def toolbar(self, title, actions=None):
         toolbar = ToolBar(title)
         toolbar.setObjectName("%sToolBar" % title)
         # toolbar.setOrientation(Qt.Vertical)
         toolbar.setToolButtonStyle(Qt.ToolButtonTextUnderIcon)
         if actions:
             utils.addActions(toolbar, actions)
-        self.addToolBar(Qt.LeftToolBarArea, toolbar)
+        self.addToolBar(Qt.TopToolBarArea, toolbar)
         return toolbar
 
     # Support Functions
 
     def noShapes(self):
         return not len(self.labelList)
 
@@ -848,14 +889,15 @@
         actions = (
             self.actions.createMode,
             self.actions.createRectangleMode,
             self.actions.createCircleMode,
             self.actions.createLineMode,
             self.actions.createPointMode,
             self.actions.createLineStripMode,
+            self.actions.createAiPolygonMode,
             self.actions.editMode,
         )
         utils.addActions(self.menus.edit, actions + self.actions.editMenu)
 
     def setDirty(self):
         # Even if we autosave the file, we keep the ability to undo
         self.actions.undo.setEnabled(self.canvas.isShapeRestorable)
@@ -879,14 +921,15 @@
         self.actions.save.setEnabled(False)
         self.actions.createMode.setEnabled(True)
         self.actions.createRectangleMode.setEnabled(True)
         self.actions.createCircleMode.setEnabled(True)
         self.actions.createLineMode.setEnabled(True)
         self.actions.createPointMode.setEnabled(True)
         self.actions.createLineStripMode.setEnabled(True)
+        self.actions.createAiPolygonMode.setEnabled(True)
         title = __appname__
         if self.filename is not None:
             title = "{} - {}".format(title, self.filename)
         self.setWindowTitle(title)
 
         if self.hasLabelFile():
             self.actions.deleteFile.setEnabled(True)
@@ -956,57 +999,83 @@
         if edit:
             self.actions.createMode.setEnabled(True)
             self.actions.createRectangleMode.setEnabled(True)
             self.actions.createCircleMode.setEnabled(True)
             self.actions.createLineMode.setEnabled(True)
             self.actions.createPointMode.setEnabled(True)
             self.actions.createLineStripMode.setEnabled(True)
+            self.actions.createAiPolygonMode.setEnabled(True)
+            self._selectAiModelComboBox.setEnabled(False)
         else:
             if createMode == "polygon":
                 self.actions.createMode.setEnabled(False)
                 self.actions.createRectangleMode.setEnabled(True)
                 self.actions.createCircleMode.setEnabled(True)
                 self.actions.createLineMode.setEnabled(True)
                 self.actions.createPointMode.setEnabled(True)
                 self.actions.createLineStripMode.setEnabled(True)
+                self.actions.createAiPolygonMode.setEnabled(True)
+                self._selectAiModelComboBox.setEnabled(False)
             elif createMode == "rectangle":
                 self.actions.createMode.setEnabled(True)
                 self.actions.createRectangleMode.setEnabled(False)
                 self.actions.createCircleMode.setEnabled(True)
                 self.actions.createLineMode.setEnabled(True)
                 self.actions.createPointMode.setEnabled(True)
                 self.actions.createLineStripMode.setEnabled(True)
+                self.actions.createAiPolygonMode.setEnabled(True)
+                self._selectAiModelComboBox.setEnabled(False)
             elif createMode == "line":
                 self.actions.createMode.setEnabled(True)
                 self.actions.createRectangleMode.setEnabled(True)
                 self.actions.createCircleMode.setEnabled(True)
                 self.actions.createLineMode.setEnabled(False)
                 self.actions.createPointMode.setEnabled(True)
                 self.actions.createLineStripMode.setEnabled(True)
+                self.actions.createAiPolygonMode.setEnabled(True)
+                self._selectAiModelComboBox.setEnabled(False)
             elif createMode == "point":
                 self.actions.createMode.setEnabled(True)
                 self.actions.createRectangleMode.setEnabled(True)
                 self.actions.createCircleMode.setEnabled(True)
                 self.actions.createLineMode.setEnabled(True)
                 self.actions.createPointMode.setEnabled(False)
                 self.actions.createLineStripMode.setEnabled(True)
+                self.actions.createAiPolygonMode.setEnabled(True)
+                self._selectAiModelComboBox.setEnabled(False)
             elif createMode == "circle":
                 self.actions.createMode.setEnabled(True)
                 self.actions.createRectangleMode.setEnabled(True)
                 self.actions.createCircleMode.setEnabled(False)
                 self.actions.createLineMode.setEnabled(True)
                 self.actions.createPointMode.setEnabled(True)
                 self.actions.createLineStripMode.setEnabled(True)
+                self.actions.createAiPolygonMode.setEnabled(True)
+                self._selectAiModelComboBox.setEnabled(False)
             elif createMode == "linestrip":
                 self.actions.createMode.setEnabled(True)
                 self.actions.createRectangleMode.setEnabled(True)
                 self.actions.createCircleMode.setEnabled(True)
                 self.actions.createLineMode.setEnabled(True)
                 self.actions.createPointMode.setEnabled(True)
                 self.actions.createLineStripMode.setEnabled(False)
+                self.actions.createAiPolygonMode.setEnabled(True)
+                self._selectAiModelComboBox.setEnabled(False)
+            elif createMode == "ai_polygon":
+                self.actions.createMode.setEnabled(True)
+                self.actions.createRectangleMode.setEnabled(True)
+                self.actions.createCircleMode.setEnabled(True)
+                self.actions.createLineMode.setEnabled(True)
+                self.actions.createPointMode.setEnabled(True)
+                self.actions.createLineStripMode.setEnabled(True)
+                self.actions.createAiPolygonMode.setEnabled(False)
+                self.canvas.initializeAiModel(
+                    name=self._selectAiModelComboBox.currentText()
+                )
+                self._selectAiModelComboBox.setEnabled(True)
             else:
                 raise ValueError("Unsupported createMode: %s" % createMode)
         self.actions.editMode.setEnabled(not edit)
 
     def setEditMode(self):
         self.toggleDrawMode(True)
```

### Comparing `labelme-5.2.1/labelme/cli/draw_json.py` & `labelme-5.3.0a0/labelme/cli/draw_json.py`

 * *Files identical despite different names*

### Comparing `labelme-5.2.1/labelme/cli/draw_label_png.py` & `labelme-5.3.0a0/labelme/cli/draw_label_png.py`

 * *Files identical despite different names*

### Comparing `labelme-5.2.1/labelme/cli/json_to_dataset.py` & `labelme-5.3.0a0/labelme/cli/json_to_dataset.py`

 * *Files identical despite different names*

### Comparing `labelme-5.2.1/labelme/cli/on_docker.py` & `labelme-5.3.0a0/labelme/cli/on_docker.py`

 * *Files identical despite different names*

### Comparing `labelme-5.2.1/labelme/config/__init__.py` & `labelme-5.3.0a0/labelme/config/__init__.py`

 * *Files identical despite different names*

### Comparing `labelme-5.2.1/labelme/config/default_config.yaml` & `labelme-5.3.0a0/labelme/config/default_config.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 shape_color: auto  # null, 'auto', 'manual'
 shift_auto_shape_color: 0
 label_colors: null
 
 shape:
   # drawing
   line_color: [0, 255, 0, 128]
-  fill_color: [0, 255, 0, 0]  # transparent
+  fill_color: [0, 0, 0, 64]
   vertex_fill_color: [0, 255, 0, 255]
   # selecting / hovering
   select_line_color: [255, 255, 255, 255]
   select_fill_color: [0, 255, 0, 155]
   hvertex_fill_color: [255, 255, 255, 255]
   point_size: 8
 
@@ -58,27 +58,29 @@
 fit_to_content:
   column: true
   row: false
 
 # canvas
 epsilon: 10.0
 canvas:
+  fill_drawing: true
   # None: do nothing
   # close: close polygon
   double_click: close
   # The max number of edits we can undo
   num_backups: 10
   # show crosshair
   crosshair:
     polygon: false
     rectangle: true
     circle: false
     line: false
     point: false
     linestrip: false
+    ai_polygon: false
 
 shortcuts:
   close: Ctrl+W
   open: Ctrl+O
   open_dir: Ctrl+U
   quit: Ctrl+Q
   save: Ctrl+S
```

### Comparing `labelme-5.2.1/labelme/icons/cancel.png` & `labelme-5.3.0a0/labelme/icons/cancel.png`

 * *Files identical despite different names*

### Comparing `labelme-5.2.1/labelme/icons/close.png` & `labelme-5.3.0a0/labelme/icons/close.png`

 * *Files identical despite different names*

### Comparing `labelme-5.2.1/labelme/icons/color-line.png` & `labelme-5.3.0a0/labelme/icons/color-line.png`

 * *Files identical despite different names*

### Comparing `labelme-5.2.1/labelme/icons/color.png` & `labelme-5.3.0a0/labelme/icons/color.png`

 * *Files identical despite different names*

### Comparing `labelme-5.2.1/labelme/icons/copy.png` & `labelme-5.3.0a0/labelme/icons/copy.png`

 * *Files identical despite different names*

### Comparing `labelme-5.2.1/labelme/icons/delete.png` & `labelme-5.3.0a0/labelme/icons/delete.png`

 * *Files identical despite different names*

### Comparing `labelme-5.2.1/labelme/icons/done.png` & `labelme-5.3.0a0/labelme/icons/done.png`

 * *Files identical despite different names*

### Comparing `labelme-5.2.1/labelme/icons/done.svg` & `labelme-5.3.0a0/labelme/icons/done.svg`

 * *Files identical despite different names*

### Comparing `labelme-5.2.1/labelme/icons/edit.png` & `labelme-5.3.0a0/labelme/icons/edit.png`

 * *Files identical despite different names*

### Comparing `labelme-5.2.1/labelme/icons/expert.png` & `labelme-5.3.0a0/labelme/icons/expert.png`

 * *Files identical despite different names*

### Comparing `labelme-5.2.1/labelme/icons/eye.png` & `labelme-5.3.0a0/labelme/icons/eye.png`

 * *Files identical despite different names*

### Comparing `labelme-5.2.1/labelme/icons/feBlend-icon.png` & `labelme-5.3.0a0/labelme/icons/feBlend-icon.png`

 * *Files identical despite different names*

### Comparing `labelme-5.2.1/labelme/icons/file.png` & `labelme-5.3.0a0/labelme/icons/file.png`

 * *Files identical despite different names*

### Comparing `labelme-5.2.1/labelme/icons/fit-width.png` & `labelme-5.3.0a0/labelme/icons/fit-width.png`

 * *Files identical despite different names*

### Comparing `labelme-5.2.1/labelme/icons/fit-window.png` & `labelme-5.3.0a0/labelme/icons/fit-window.png`

 * *Files identical despite different names*

### Comparing `labelme-5.2.1/labelme/icons/fit.png` & `labelme-5.3.0a0/labelme/icons/fit.png`

 * *Files identical despite different names*

### Comparing `labelme-5.2.1/labelme/icons/help.png` & `labelme-5.3.0a0/labelme/icons/help.png`

 * *Files identical despite different names*

### Comparing `labelme-5.2.1/labelme/icons/icon.icns` & `labelme-5.3.0a0/labelme/icons/icon.icns`

 * *Files identical despite different names*

### Comparing `labelme-5.2.1/labelme/icons/icon.ico` & `labelme-5.3.0a0/labelme/icons/icon.ico`

 * *Files identical despite different names*

### Comparing `labelme-5.2.1/labelme/icons/icon.png` & `labelme-5.3.0a0/labelme/icons/icon.png`

 * *Files identical despite different names*

### Comparing `labelme-5.2.1/labelme/icons/labels.png` & `labelme-5.3.0a0/labelme/icons/labels.png`

 * *Files identical despite different names*

### Comparing `labelme-5.2.1/labelme/icons/labels.svg` & `labelme-5.3.0a0/labelme/icons/labels.svg`

 * *Files identical despite different names*

### Comparing `labelme-5.2.1/labelme/icons/new.png` & `labelme-5.3.0a0/labelme/icons/new.png`

 * *Files identical despite different names*

### Comparing `labelme-5.2.1/labelme/icons/next.png` & `labelme-5.3.0a0/labelme/icons/next.png`

 * *Files identical despite different names*

### Comparing `labelme-5.2.1/labelme/icons/objects.png` & `labelme-5.3.0a0/labelme/icons/objects.png`

 * *Files identical despite different names*

### Comparing `labelme-5.2.1/labelme/icons/open.png` & `labelme-5.3.0a0/labelme/icons/open.png`

 * *Files identical despite different names*

### Comparing `labelme-5.2.1/labelme/icons/open.svg` & `labelme-5.3.0a0/labelme/icons/open.svg`

 * *Files identical despite different names*

### Comparing `labelme-5.2.1/labelme/icons/prev.png` & `labelme-5.3.0a0/labelme/icons/prev.png`

 * *Files identical despite different names*

### Comparing `labelme-5.2.1/labelme/icons/quit.png` & `labelme-5.3.0a0/labelme/icons/quit.png`

 * *Files identical despite different names*

### Comparing `labelme-5.2.1/labelme/icons/save-as.png` & `labelme-5.3.0a0/labelme/icons/save-as.png`

 * *Files identical despite different names*

### Comparing `labelme-5.2.1/labelme/icons/save-as.svg` & `labelme-5.3.0a0/labelme/icons/save-as.svg`

 * *Files identical despite different names*

### Comparing `labelme-5.2.1/labelme/icons/save.png` & `labelme-5.3.0a0/labelme/icons/save.png`

 * *Files identical despite different names*

### Comparing `labelme-5.2.1/labelme/icons/save.svg` & `labelme-5.3.0a0/labelme/icons/save.svg`

 * *Files identical despite different names*

### Comparing `labelme-5.2.1/labelme/icons/undo-cross.png` & `labelme-5.3.0a0/labelme/icons/undo-cross.png`

 * *Files identical despite different names*

### Comparing `labelme-5.2.1/labelme/icons/undo.png` & `labelme-5.3.0a0/labelme/icons/undo.png`

 * *Files identical despite different names*

### Comparing `labelme-5.2.1/labelme/icons/zoom-in.png` & `labelme-5.3.0a0/labelme/icons/zoom-in.png`

 * *Files identical despite different names*

### Comparing `labelme-5.2.1/labelme/icons/zoom-out.png` & `labelme-5.3.0a0/labelme/icons/zoom-out.png`

 * *Files identical despite different names*

### Comparing `labelme-5.2.1/labelme/icons/zoom.png` & `labelme-5.3.0a0/labelme/icons/zoom.png`

 * *Files identical despite different names*

### Comparing `labelme-5.2.1/labelme/label_file.py` & `labelme-5.3.0a0/labelme/label_file.py`

 * *Files 6% similar despite different names*

```diff
@@ -84,29 +84,14 @@
             "shape_type",
             "flags",
             "description",
         ]
         try:
             with open(filename, "r") as f:
                 data = json.load(f)
-            version = data.get("version")
-            if version is None:
-                logger.warning(
-                    "Loading JSON file ({}) of unknown version".format(
-                        filename
-                    )
-                )
-            elif version.split(".")[0] != __version__.split(".")[0]:
-                logger.warning(
-                    "This JSON file ({}) may be incompatible with "
-                    "current labelme. version in file: {}, "
-                    "current version: {}".format(
-                        filename, version, __version__
-                    )
-                )
 
             if data["imageData"] is not None:
                 imageData = base64.b64decode(data["imageData"])
                 if PY2 and QT4:
                     imageData = utils.img_data_to_png_data(imageData)
             else:
                 # relative path from label file to relative path from cwd
```

### Comparing `labelme-5.2.1/labelme/shape.py` & `labelme-5.3.0a0/labelme/shape.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,14 +53,19 @@
         flags=None,
         group_id=None,
         description=None,
     ):
         self.label = label
         self.group_id = group_id
         self.points = []
+        self.point_labels = []
+        self.shape_type = shape_type
+        self._shape_raw = None
+        self._points_raw = []
+        self._shape_type_raw = None
         self.fill = False
         self.selected = False
         self.shape_type = shape_type
         self.flags = flags
         self.description = description
         self.other_data = {}
 
@@ -75,16 +80,26 @@
 
         if line_color is not None:
             # Override the class line_color attribute
             # with an object attribute. Currently this
             # is used for drawing the pending line a different color.
             self.line_color = line_color
 
+    def setShapeRefined(self, points, point_labels, shape_type):
+        self._shape_raw = (self.points, self.point_labels, self.shape_type)
+        self.points = points
+        self.point_labels = point_labels
         self.shape_type = shape_type
 
+    def restoreShapeRaw(self):
+        if self._shape_raw is None:
+            return
+        self.points, self.point_labels, self.shape_type = self._shape_raw
+        self._shape_raw = None
+
     @property
     def shape_type(self):
         return self._shape_type
 
     @shape_type.setter
     def shape_type(self, value):
         if value is None:
@@ -92,37 +107,42 @@
         if value not in [
             "polygon",
             "rectangle",
             "point",
             "line",
             "circle",
             "linestrip",
+            "points",
         ]:
             raise ValueError("Unexpected shape_type: {}".format(value))
         self._shape_type = value
 
     def close(self):
         self._closed = True
 
-    def addPoint(self, point):
+    def addPoint(self, point, label=1):
         if self.points and point == self.points[0]:
             self.close()
         else:
             self.points.append(point)
+            self.point_labels.append(label)
 
     def canAddPoint(self):
         return self.shape_type in ["polygon", "linestrip"]
 
     def popPoint(self):
         if self.points:
+            if self.point_labels:
+                self.point_labels.pop()
             return self.points.pop()
         return None
 
-    def insertPoint(self, i, point):
+    def insertPoint(self, i, point, label=1):
         self.points.insert(i, point)
+        self.point_labels.insert(i, label)
 
     def removePoint(self, i):
         if not self.canAddPoint():
             logger.warning(
                 "Cannot remove point from: shape_type=%r",
                 self.shape_type,
             )
@@ -141,14 +161,15 @@
                 "Cannot remove point from: shape_type=%r, len(points)=%d",
                 self.shape_type,
                 len(self.points),
             )
             return
 
         self.points.pop(i)
+        self.point_labels.pop(i)
 
     def isClosed(self):
         return self._closed
 
     def setOpen(self):
         self._closed = False
 
@@ -165,14 +186,15 @@
             pen = QtGui.QPen(color)
             # Try using integer sizes for smoother drawing(?)
             pen.setWidth(max(1, int(round(2.0 / self.scale))))
             painter.setPen(pen)
 
             line_path = QtGui.QPainterPath()
             vrtx_path = QtGui.QPainterPath()
+            negative_vrtx_path = QtGui.QPainterPath()
 
             if self.shape_type == "rectangle":
                 assert len(self.points) in [1, 2]
                 if len(self.points) == 2:
                     rectangle = self.getRectFromLine(*self.points)
                     line_path.addRect(rectangle)
                 for i in range(len(self.points)):
@@ -185,14 +207,23 @@
                 for i in range(len(self.points)):
                     self.drawVertex(vrtx_path, i)
             elif self.shape_type == "linestrip":
                 line_path.moveTo(self.points[0])
                 for i, p in enumerate(self.points):
                     line_path.lineTo(p)
                     self.drawVertex(vrtx_path, i)
+            elif self.shape_type == "points":
+                assert len(self.points) == len(self.point_labels)
+                for i, (p, l) in enumerate(
+                    zip(self.points, self.point_labels)
+                ):
+                    if l == 1:
+                        self.drawVertex(vrtx_path, i)
+                    else:
+                        self.drawVertex(negative_vrtx_path, i)
             else:
                 line_path.moveTo(self.points[0])
                 # Uncommenting the following line will draw 2 paths
                 # for the 1st vertex, and make it non-filled, which
                 # may be desirable.
                 # self.drawVertex(vrtx_path, 0)
 
@@ -209,14 +240,19 @@
                 color = (
                     self.select_fill_color
                     if self.selected
                     else self.fill_color
                 )
                 painter.fillPath(line_path, color)
 
+            pen.setColor(QtGui.QColor(255, 0, 0, 255))
+            painter.setPen(pen)
+            painter.drawPath(negative_vrtx_path)
+            painter.fillPath(negative_vrtx_path, QtGui.QColor(255, 0, 0, 255))
+
     def drawVertex(self, path, i):
         d = self.point_size / self.scale
         shape = self.point_type
         point = self.points[i]
         if i == self._highlightIndex:
             size, shape = self._highlightSettings[self._highlightMode]
             d *= size
```

### Comparing `labelme-5.2.1/labelme/testing.py` & `labelme-5.3.0a0/labelme/testing.py`

 * *Files identical despite different names*

### Comparing `labelme-5.2.1/labelme/utils/__init__.py` & `labelme-5.3.0a0/labelme/utils/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from .image import apply_exif_orientation
 from .image import img_arr_to_b64
 from .image import img_b64_to_arr
 from .image import img_data_to_arr
 from .image import img_data_to_pil
 from .image import img_data_to_png_data
 from .image import img_pil_to_data
+from .image import img_qt_to_arr
 
 from .shape import labelme_shapes_to_label
 from .shape import masks_to_bboxes
 from .shape import polygons_to_mask
 from .shape import shape_to_mask
 from .shape import shapes_to_label
```

### Comparing `labelme-5.2.1/labelme/utils/_io.py` & `labelme-5.3.0a0/labelme/utils/_io.py`

 * *Files identical despite different names*

### Comparing `labelme-5.2.1/labelme/utils/image.py` & `labelme-5.3.0a0/labelme/utils/image.py`

 * *Files 8% similar despite different names*

```diff
@@ -52,14 +52,21 @@
 
         with io.BytesIO() as f:
             img.save(f, "PNG")
             f.seek(0)
             return f.read()
 
 
+def img_qt_to_arr(img_qt):
+    w, h, d = img_qt.size().width(), img_qt.size().height(), img_qt.depth()
+    bytes_ = img_qt.bits().asstring(w * h * d // 8)
+    img_arr = np.frombuffer(bytes_, dtype=np.uint8).reshape((h, w, d // 8))
+    return img_arr
+
+
 def apply_exif_orientation(image):
     try:
         exif = image._getexif()
     except AttributeError:
         exif = None
 
     if exif is None:
```

### Comparing `labelme-5.2.1/labelme/utils/qt.py` & `labelme-5.3.0a0/labelme/utils/qt.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,14 +87,14 @@
     p2 = np.array([p2.x(), p2.y()])
     p3 = np.array([point.x(), point.y()])
     if np.dot((p3 - p1), (p2 - p1)) < 0:
         return np.linalg.norm(p3 - p1)
     if np.dot((p3 - p2), (p1 - p2)) < 0:
         return np.linalg.norm(p3 - p2)
     if np.linalg.norm(p2 - p1) == 0:
-        return 0
+        return np.linalg.norm(p3 - p1)
     return np.linalg.norm(np.cross(p2 - p1, p1 - p3)) / np.linalg.norm(p2 - p1)
 
 
 def fmtShortcut(text):
     mod, key = text.split("+", 1)
     return "<b>%s</b>+<b>%s</b>" % (mod, key)
```

### Comparing `labelme-5.2.1/labelme/utils/shape.py` & `labelme-5.3.0a0/labelme/utils/shape.py`

 * *Files identical despite different names*

### Comparing `labelme-5.2.1/labelme/widgets/brightness_contrast_dialog.py` & `labelme-5.3.0a0/labelme/widgets/brightness_contrast_dialog.py`

 * *Files identical despite different names*

### Comparing `labelme-5.2.1/labelme/widgets/canvas.py` & `labelme-5.3.0a0/labelme/widgets/canvas.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,14 @@
+import gdown
 from qtpy import QtCore
 from qtpy import QtGui
 from qtpy import QtWidgets
 
+import labelme.ai
+from labelme.logger import logger
 from labelme import QT5
 from labelme.shape import Shape
 import labelme.utils
 
 
 # TODO(unknown):
 # - [maybe] Find optimal epsilon value.
@@ -52,14 +55,15 @@
             {
                 "polygon": False,
                 "rectangle": True,
                 "circle": False,
                 "line": False,
                 "point": False,
                 "linestrip": False,
+                "ai_polygon": False,
             },
         )
         super(Canvas, self).__init__(*args, **kwargs)
         # Initialise local state.
         self.mode = self.EDIT
         self.shapes = []
         self.shapesBackups = []
@@ -95,14 +99,16 @@
         # 0: right-click without selection and dragging of shapes
         # 1: right-click with selection and dragging of shapes
         self.menus = (QtWidgets.QMenu(), QtWidgets.QMenu())
         # Set widget options.
         self.setMouseTracking(True)
         self.setFocusPolicy(QtCore.Qt.WheelFocus)
 
+        self._ai_model = None
+
     def fillDrawing(self):
         return self._fill_drawing
 
     def setFillDrawing(self, value):
         self._fill_drawing = value
 
     @property
@@ -114,18 +120,44 @@
         if value not in [
             "polygon",
             "rectangle",
             "circle",
             "line",
             "point",
             "linestrip",
+            "ai_polygon",
         ]:
             raise ValueError("Unsupported createMode: %s" % value)
         self._createMode = value
 
+    def initializeAiModel(self, name):
+        if name not in [model.name for model in labelme.ai.MODELS]:
+            raise ValueError("Unsupported ai model: %s" % name)
+        model = [model for model in labelme.ai.MODELS if model.name == name][0]
+
+        if self._ai_model is not None and self._ai_model.name == model.name:
+            logger.debug("AI model is already initialized: %r" % model.name)
+        else:
+            logger.debug("Initializing AI model: %r" % model.name)
+            self._ai_model = labelme.ai.SegmentAnythingModel(
+                name=model.name,
+                encoder_path=gdown.cached_download(
+                    url=model.encoder_weight.url,
+                    md5=model.encoder_weight.md5,
+                ),
+                decoder_path=gdown.cached_download(
+                    url=model.decoder_weight.url,
+                    md5=model.decoder_weight.md5,
+                ),
+            )
+
+        self._ai_model.set_image(
+            image=labelme.utils.img_qt_to_arr(self.pixmap.toImage())
+        )
+
     def storeShapes(self):
         shapesBackup = []
         for shape in self.shapes:
             shapesBackup.append(shape.copy())
         if len(self.shapesBackups) > self.num_backups:
             self.shapesBackups = self.shapesBackups[-self.num_backups - 1 :]
         self.shapesBackups.append(shapesBackup)
@@ -209,17 +241,22 @@
                 pos = self.transformPos(ev.posF())
         except AttributeError:
             return
 
         self.prevMovePoint = pos
         self.restoreCursor()
 
+        is_shift_pressed = ev.modifiers() & QtCore.Qt.ShiftModifier
+
         # Polygon drawing.
         if self.drawing():
-            self.line.shape_type = self.createMode
+            if self.createMode == "ai_polygon":
+                self.line.shape_type = "points"
+            else:
+                self.line.shape_type = self.createMode
 
             self.overrideCursor(CURSOR_DRAW)
             if not self.current:
                 self.repaint()  # draw crosshair
                 return
 
             if self.outOfPixmap(pos):
@@ -234,28 +271,39 @@
             ):
                 # Attract line to starting point and
                 # colorise to alert the user.
                 pos = self.current[0]
                 self.overrideCursor(CURSOR_POINT)
                 self.current.highlightVertex(0, Shape.NEAR_VERTEX)
             if self.createMode in ["polygon", "linestrip"]:
-                self.line[0] = self.current[-1]
-                self.line[1] = pos
+                self.line.points = [self.current[-1], pos]
+                self.line.point_labels = [1, 1]
+            elif self.createMode == "ai_polygon":
+                self.line.points = [self.current.points[-1], pos]
+                self.line.point_labels = [
+                    self.current.point_labels[-1],
+                    0 if is_shift_pressed else 1,
+                ]
             elif self.createMode == "rectangle":
                 self.line.points = [self.current[0], pos]
+                self.line.point_labels = [1, 1]
                 self.line.close()
             elif self.createMode == "circle":
                 self.line.points = [self.current[0], pos]
+                self.line.point_labels = [1, 1]
                 self.line.shape_type = "circle"
             elif self.createMode == "line":
                 self.line.points = [self.current[0], pos]
+                self.line.point_labels = [1, 1]
                 self.line.close()
             elif self.createMode == "point":
                 self.line.points = [self.current[0]]
+                self.line.point_labels = [1]
                 self.line.close()
+            assert len(self.line.points) == len(self.line.point_labels)
             self.repaint()
             self.current.highlightClear()
             return
 
         # Polygon copy moving.
         if QtCore.Qt.RightButton & ev.buttons():
             if self.selectedShapesCopy and self.prevPoint:
@@ -361,14 +409,17 @@
         self.movingShape = True  # Save changes
 
     def mousePressEvent(self, ev):
         if QT5:
             pos = self.transformPos(ev.localPos())
         else:
             pos = self.transformPos(ev.posF())
+
+        is_shift_pressed = ev.modifiers() & QtCore.Qt.ShiftModifier
+
         if ev.button() == QtCore.Qt.LeftButton:
             if self.drawing():
                 if self.current:
                     # Add point to existing shape.
                     if self.createMode == "polygon":
                         self.current.addPoint(self.line[1])
                         self.line[0] = self.current[-1]
@@ -379,24 +430,53 @@
                         self.current.points = self.line.points
                         self.finalise()
                     elif self.createMode == "linestrip":
                         self.current.addPoint(self.line[1])
                         self.line[0] = self.current[-1]
                         if int(ev.modifiers()) == QtCore.Qt.ControlModifier:
                             self.finalise()
+                    elif self.createMode == "ai_polygon":
+                        self.current.addPoint(
+                            self.line.points[1],
+                            label=self.line.point_labels[1],
+                        )
+                        self.line.points[0] = self.current.points[-1]
+                        self.line.point_labels[0] = self.current.point_labels[
+                            -1
+                        ]
+                        if ev.modifiers() & QtCore.Qt.ControlModifier:
+                            self.finalise()
                 elif not self.outOfPixmap(pos):
                     # Create new shape.
-                    self.current = Shape(shape_type=self.createMode)
-                    self.current.addPoint(pos)
+                    self.current = Shape(
+                        shape_type="points"
+                        if self.createMode == "ai_polygon"
+                        else self.createMode
+                    )
+                    self.current.addPoint(
+                        pos, label=0 if is_shift_pressed else 1
+                    )
                     if self.createMode == "point":
                         self.finalise()
+                    elif (
+                        self.createMode == "ai_polygon"
+                        and ev.modifiers() & QtCore.Qt.ControlModifier
+                    ):
+                        self.finalise()
                     else:
                         if self.createMode == "circle":
                             self.current.shape_type = "circle"
                         self.line.points = [pos, pos]
+                        if (
+                            self.createMode == "ai_polygon"
+                            and is_shift_pressed
+                        ):
+                            self.line.point_labels = [0, 0]
+                        else:
+                            self.line.point_labels = [1, 1]
                         self.setHiding()
                         self.drawingPolygon.emit(True)
                         self.update()
             elif self.editing():
                 if self.selectedEdge():
                     self.addPointToEdge()
                 elif (
@@ -480,22 +560,20 @@
     def setHiding(self, enable=True):
         self._hideBackround = self.hideBackround if enable else False
 
     def canCloseShape(self):
         return self.drawing() and self.current and len(self.current) > 2
 
     def mouseDoubleClickEvent(self, ev):
-        # We need at least 4 points here, since the mousePress handler
-        # adds an extra one before this handler is called.
+        if self.double_click != "close":
+            return
+
         if (
-            self.double_click == "close"
-            and self.canCloseShape()
-            and len(self.current) > 3
-        ):
-            self.current.popPoint()
+            self.createMode == "polygon" and self.canCloseShape()
+        ) or self.createMode == "ai_polygon":
             self.finalise()
 
     def selectShapes(self, shapes):
         self.setHiding()
         self.selectionChanged.emit(shapes)
         self.update()
 
@@ -660,29 +738,58 @@
             if (shape.selected or not self._hideBackround) and self.isVisible(
                 shape
             ):
                 shape.fill = shape.selected or shape == self.hShape
                 shape.paint(p)
         if self.current:
             self.current.paint(p)
+            assert len(self.line.points) == len(self.line.point_labels)
             self.line.paint(p)
         if self.selectedShapesCopy:
             for s in self.selectedShapesCopy:
                 s.paint(p)
 
         if (
             self.fillDrawing()
             and self.createMode == "polygon"
             and self.current is not None
             and len(self.current.points) >= 2
         ):
             drawing_shape = self.current.copy()
+            if drawing_shape.fill_color.getRgb()[3] == 0:
+                logger.warning(
+                    "fill_drawing=true, but fill_color is transparent,"
+                    " so forcing to be opaque."
+                )
+                drawing_shape.fill_color.setAlpha(64)
             drawing_shape.addPoint(self.line[1])
             drawing_shape.fill = True
             drawing_shape.paint(p)
+        elif self.createMode == "ai_polygon" and self.current is not None:
+            drawing_shape = self.current.copy()
+            drawing_shape.addPoint(
+                point=self.line.points[1],
+                label=self.line.point_labels[1],
+            )
+            points = self._ai_model.predict_polygon_from_points(
+                points=[
+                    [point.x(), point.y()] for point in drawing_shape.points
+                ],
+                point_labels=drawing_shape.point_labels,
+            )
+            if len(points) > 2:
+                drawing_shape.setShapeRefined(
+                    points=[
+                        QtCore.QPointF(point[0], point[1]) for point in points
+                    ],
+                    point_labels=[1] * len(points),
+                    shape_type="polygon",
+                )
+                drawing_shape.fill = self.fillDrawing()
+                drawing_shape.paint(p)
 
         p.end()
 
     def transformPos(self, point):
         """Convert from widget-logical coordinates to painter-logical ones."""
         return point / self.scale - self.offsetToCenter()
 
@@ -697,15 +804,32 @@
 
     def outOfPixmap(self, p):
         w, h = self.pixmap.width(), self.pixmap.height()
         return not (0 <= p.x() <= w - 1 and 0 <= p.y() <= h - 1)
 
     def finalise(self):
         assert self.current
+        if self.createMode == "ai_polygon":
+            # convert points to polygon by an AI model
+            assert self.current.shape_type == "points"
+            points = self._ai_model.predict_polygon_from_points(
+                points=[
+                    [point.x(), point.y()] for point in self.current.points
+                ],
+                point_labels=self.current.point_labels,
+            )
+            self.current.setShapeRefined(
+                points=[
+                    QtCore.QPointF(point[0], point[1]) for point in points
+                ],
+                point_labels=[1] * len(points),
+                shape_type="polygon",
+            )
         self.current.close()
+
         self.shapes.append(self.current)
         self.storeShapes()
         self.current = None
         self.setHiding(False)
         self.newShape.emit()
         self.update()
 
@@ -865,14 +989,15 @@
         self.storeShapes()
         return self.shapes[-1]
 
     def undoLastLine(self):
         assert self.shapes
         self.current = self.shapes.pop()
         self.current.setOpen()
+        self.current.restoreShapeRaw()
         if self.createMode in ["polygon", "linestrip"]:
             self.line.points = [self.current[-1], self.current[0]]
         elif self.createMode in ["rectangle", "line", "circle"]:
             self.current.points = self.current.points[0:1]
         elif self.createMode == "point":
             self.current = None
         self.drawingPolygon.emit(True)
@@ -886,14 +1011,18 @@
         else:
             self.current = None
             self.drawingPolygon.emit(False)
         self.update()
 
     def loadPixmap(self, pixmap, clear_shapes=True):
         self.pixmap = pixmap
+        if self._ai_model:
+            self._ai_model.set_image(
+                image=labelme.utils.img_qt_to_arr(self.pixmap.toImage())
+            )
         if clear_shapes:
             self.shapes = []
         self.update()
 
     def loadShapes(self, shapes, replace=True):
         if replace:
             self.shapes = list(shapes)
```

### Comparing `labelme-5.2.1/labelme/widgets/color_dialog.py` & `labelme-5.3.0a0/labelme/widgets/color_dialog.py`

 * *Files identical despite different names*

### Comparing `labelme-5.2.1/labelme/widgets/file_dialog_preview.py` & `labelme-5.3.0a0/labelme/widgets/file_dialog_preview.py`

 * *Files identical despite different names*

### Comparing `labelme-5.2.1/labelme/widgets/label_dialog.py` & `labelme-5.3.0a0/labelme/widgets/label_dialog.py`

 * *Files identical despite different names*

### Comparing `labelme-5.2.1/labelme/widgets/label_list_widget.py` & `labelme-5.3.0a0/labelme/widgets/label_list_widget.py`

 * *Files identical despite different names*

### Comparing `labelme-5.2.1/labelme/widgets/tool_bar.py` & `labelme-5.3.0a0/labelme/widgets/tool_bar.py`

 * *Files identical despite different names*

### Comparing `labelme-5.2.1/labelme/widgets/unique_label_qlist_widget.py` & `labelme-5.3.0a0/labelme/widgets/unique_label_qlist_widget.py`

 * *Files identical despite different names*

### Comparing `labelme-5.2.1/labelme/widgets/zoom_widget.py` & `labelme-5.3.0a0/labelme/widgets/zoom_widget.py`

 * *Files identical despite different names*

### Comparing `labelme-5.2.1/labelme.egg-info/PKG-INFO` & `labelme-5.3.0a0/labelme.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labelme
-Version: 5.2.1
+Version: 5.3.0a0
 Summary: Image Polygonal Annotation with Python
 Home-page: https://github.com/wkentaro/labelme
 Author: Kentaro Wada
 Author-email: www.kentaro.wada@gmail.com
 License: GPLv3
 Keywords: Image Annotation,Machine Learning
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: labelme Version: 5.2.1 Summary: Image Polygonal
+Metadata-Version: 2.1 Name: labelme Version: 5.3.0a0 Summary: Image Polygonal
 Annotation with Python Home-page: https://github.com/wkentaro/labelme Author:
 Kentaro Wada Author-email: www.kentaro.wada@gmail.com License: GPLv3 Keywords:
 Image Annotation,Machine Learning Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Science/Research Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python Classifier: Programming Language :: Python :: 3.5 Classifier:
```

### Comparing `labelme-5.2.1/labelme.egg-info/SOURCES.txt` & `labelme-5.3.0a0/labelme.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -11,14 +11,17 @@
 labelme/testing.py
 labelme.egg-info/PKG-INFO
 labelme.egg-info/SOURCES.txt
 labelme.egg-info/dependency_links.txt
 labelme.egg-info/entry_points.txt
 labelme.egg-info/requires.txt
 labelme.egg-info/top_level.txt
+labelme/ai/__init__.py
+labelme/ai/models/__init__.py
+labelme/ai/models/segment_anything.py
 labelme/cli/__init__.py
 labelme/cli/draw_json.py
 labelme/cli/draw_label_png.py
 labelme/cli/json_to_dataset.py
 labelme/cli/on_docker.py
 labelme/config/__init__.py
 labelme/config/default_config.yaml
```

### Comparing `labelme-5.2.1/setup.py` & `labelme-5.3.0a0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,21 +19,24 @@
         raise RuntimeError("{} doesn't contain __version__".format(filename))
     version = match.groups()[0]
     return version
 
 
 def get_install_requires():
     install_requires = [
+        "gdown",
         "imgviz>=0.11",
         "matplotlib",
         "natsort>=7.1.0",
         "numpy",
+        "onnxruntime>=1.14.1",
         "Pillow>=2.8",
         "PyYAML",
         "qtpy!=1.11.2",
+        "scikit-image",
         "termcolor",
     ]
 
     # Find python binding for qt with priority:
     # PyQt5 -> PySide2
     # and PyQt5 is automatically installed on Python3.
     QT_BINDING = None
```

