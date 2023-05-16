# Comparing `tmp/pynecone-0.1.30a0.tar.gz` & `tmp/pynecone-0.1.30a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynecone-0.1.30a0.tar", max compression
+gzip compressed data, was "pynecone-0.1.30a1.tar", max compression
```

## Comparing `pynecone-0.1.30a0.tar` & `pynecone-0.1.30a1.tar`

### file list

```diff
@@ -1,157 +1,157 @@
--rw-r--r--   0        0        0    11356 2023-01-24 01:31:44.826695 pynecone-0.1.30a0/LICENSE
--rw-r--r--   0        0        0     7876 2023-05-15 02:04:07.603507 pynecone-0.1.30a0/README.md
--rw-r--r--   0        0        0        0 2023-04-27 02:06:35.747147 pynecone-0.1.30a0/pynecone/.templates/apps/counter/__init__.py
--rw-r--r--   0        0        0     1340 2023-04-27 02:06:35.747526 pynecone-0.1.30a0/pynecone/.templates/apps/counter/counter.py
--rw-r--r--   0        0        0        0 2023-04-27 02:06:35.747631 pynecone-0.1.30a0/pynecone/.templates/apps/default/__init__.py
--rw-r--r--   0        0        0     1036 2023-04-27 02:06:35.747905 pynecone-0.1.30a0/pynecone/.templates/apps/default/default.py
--rw-r--r--   0        0        0    15406 2022-11-18 20:43:33.740339 pynecone-0.1.30a0/pynecone/.templates/assets/favicon.ico
--rw-r--r--   0        0        0      183 2023-05-15 02:04:07.604358 pynecone-0.1.30a0/pynecone/.templates/jinja/app/pcconfig.py.jinja2
--rw-r--r--   0        0        0      182 2023-05-15 02:04:07.604515 pynecone-0.1.30a0/pynecone/.templates/jinja/web/pages/_document.js.jinja2
--rw-r--r--   0        0        0      241 2023-05-15 02:04:07.604581 pynecone-0.1.30a0/pynecone/.templates/jinja/web/pages/base_page.js.jinja2
--rw-r--r--   0        0        0      252 2023-05-15 02:04:07.604642 pynecone-0.1.30a0/pynecone/.templates/jinja/web/pages/custom_component.js.jinja2
--rw-r--r--   0        0        0     2293 2023-05-15 02:04:07.604733 pynecone-0.1.30a0/pynecone/.templates/jinja/web/pages/index.js.jinja2
--rw-r--r--   0        0        0     2999 2023-05-15 02:04:07.604822 pynecone-0.1.30a0/pynecone/.templates/jinja/web/pages/utils.js.jinja2
--rw-r--r--   0        0        0       38 2023-05-15 02:04:07.604905 pynecone-0.1.30a0/pynecone/.templates/jinja/web/utils/theme.js.jinja2
--rw-r--r--   0        0        0      417 2022-12-27 07:35:12.085907 pynecone-0.1.30a0/pynecone/.templates/web/.gitignore
--rwxr-xr-x   0        0        0   254417 2023-05-15 02:04:07.606023 pynecone-0.1.30a0/pynecone/.templates/web/bun.lockb
--rw-r--r--   0        0        0       47 2022-12-20 23:31:29.590974 pynecone-0.1.30a0/pynecone/.templates/web/next.config.js
--rw-r--r--   0        0        0      927 2023-05-15 02:04:07.606305 pynecone-0.1.30a0/pynecone/.templates/web/package.json
--rw-r--r--   0        0        0      502 2022-11-18 20:43:33.740024 pynecone-0.1.30a0/pynecone/.templates/web/pages/404.js
--rw-r--r--   0        0        0      564 2023-01-12 05:38:04.342282 pynecone-0.1.30a0/pynecone/.templates/web/pages/_app.js
--rw-r--r--   0        0        0    29404 2022-12-20 23:31:29.592485 pynecone-0.1.30a0/pynecone/.templates/web/styles/code/prism.js
--rw-r--r--   0        0        0     7353 2023-05-15 17:32:17.390957 pynecone-0.1.30a0/pynecone/.templates/web/utils/state.js
--rw-r--r--   0        0        0     1363 2023-05-15 02:04:07.606665 pynecone-0.1.30a0/pynecone/__init__.py
--rw-r--r--   0        0        0    20075 2023-05-15 02:04:07.606864 pynecone-0.1.30a0/pynecone/app.py
--rw-r--r--   0        0        0     2510 2023-01-30 21:50:18.206745 pynecone-0.1.30a0/pynecone/base.py
--rw-r--r--   0        0        0       29 2022-11-18 20:43:33.740719 pynecone-0.1.30a0/pynecone/compiler/__init__.py
--rw-r--r--   0        0        0     6218 2023-05-15 02:04:07.607063 pynecone-0.1.30a0/pynecone/compiler/compiler.py
--rw-r--r--   0        0        0     2565 2023-05-15 02:04:07.607300 pynecone-0.1.30a0/pynecone/compiler/templates.py
--rw-r--r--   0        0        0     7384 2023-05-15 02:04:07.607425 pynecone-0.1.30a0/pynecone/compiler/utils.py
--rw-r--r--   0        0        0     6390 2023-05-15 17:32:17.391279 pynecone-0.1.30a0/pynecone/components/__init__.py
--rw-r--r--   0        0        0      226 2023-03-13 04:10:28.615930 pynecone-0.1.30a0/pynecone/components/base/__init__.py
--rw-r--r--   0        0        0      727 2023-05-15 02:04:07.607680 pynecone-0.1.30a0/pynecone/components/base/bare.py
--rw-r--r--   0        0        0      153 2023-03-13 04:10:28.760655 pynecone-0.1.30a0/pynecone/components/base/body.py
--rw-r--r--   0        0        0      725 2023-01-30 22:40:32.678074 pynecone-0.1.30a0/pynecone/components/base/document.py
--rw-r--r--   0        0        0      265 2023-05-15 02:04:07.607851 pynecone-0.1.30a0/pynecone/components/base/head.py
--rw-r--r--   0        0        0      930 2023-05-15 02:04:07.607989 pynecone-0.1.30a0/pynecone/components/base/link.py
--rw-r--r--   0        0        0     1340 2023-05-15 02:04:07.608303 pynecone-0.1.30a0/pynecone/components/base/meta.py
--rw-r--r--   0        0        0    22071 2023-05-15 17:32:17.391734 pynecone-0.1.30a0/pynecone/components/component.py
--rw-r--r--   0        0        0      422 2023-04-02 23:51:14.632016 pynecone-0.1.30a0/pynecone/components/datadisplay/__init__.py
--rw-r--r--   0        0        0      334 2023-05-15 02:04:07.608726 pynecone-0.1.30a0/pynecone/components/datadisplay/badge.py
--rw-r--r--   0        0        0     2513 2023-05-15 02:04:07.608840 pynecone-0.1.30a0/pynecone/components/datadisplay/code.py
--rw-r--r--   0        0        0     4033 2023-05-15 02:04:07.608953 pynecone-0.1.30a0/pynecone/components/datadisplay/datatable.py
--rw-r--r--   0        0        0      537 2023-05-15 02:04:07.609045 pynecone-0.1.30a0/pynecone/components/datadisplay/divider.py
--rw-r--r--   0        0        0      187 2023-04-02 23:51:14.632124 pynecone-0.1.30a0/pynecone/components/datadisplay/keyboard_key.py
--rw-r--r--   0        0        0     1430 2023-05-15 02:04:07.609140 pynecone-0.1.30a0/pynecone/components/datadisplay/list.py
--rw-r--r--   0        0        0     2157 2023-05-15 02:04:07.609232 pynecone-0.1.30a0/pynecone/components/datadisplay/stat.py
--rw-r--r--   0        0        0     5157 2023-05-15 02:04:07.609333 pynecone-0.1.30a0/pynecone/components/datadisplay/table.py
--rw-r--r--   0        0        0      316 2023-01-24 02:43:48.871608 pynecone-0.1.30a0/pynecone/components/disclosure/__init__.py
--rw-r--r--   0        0        0     2941 2023-05-15 02:04:07.609439 pynecone-0.1.30a0/pynecone/components/disclosure/accordion.py
--rw-r--r--   0        0        0     2777 2023-05-15 02:04:07.609534 pynecone-0.1.30a0/pynecone/components/disclosure/tabs.py
--rw-r--r--   0        0        0      285 2022-12-05 22:26:47.605453 pynecone-0.1.30a0/pynecone/components/disclosure/visuallyhidden.py
--rw-r--r--   0        0        0      313 2022-11-18 20:43:33.723246 pynecone-0.1.30a0/pynecone/components/feedback/__init__.py
--rw-r--r--   0        0        0     1571 2023-05-15 02:04:07.609649 pynecone-0.1.30a0/pynecone/components/feedback/alert.py
--rw-r--r--   0        0        0     1905 2023-05-15 02:04:07.609745 pynecone-0.1.30a0/pynecone/components/feedback/circularprogress.py
--rw-r--r--   0        0        0      879 2023-05-15 02:04:07.609838 pynecone-0.1.30a0/pynecone/components/feedback/progress.py
--rw-r--r--   0        0        0     1785 2023-05-15 02:04:07.609925 pynecone-0.1.30a0/pynecone/components/feedback/skeleton.py
--rw-r--r--   0        0        0      678 2023-05-15 02:04:07.610013 pynecone-0.1.30a0/pynecone/components/feedback/spinner.py
--rw-r--r--   0        0        0     1109 2023-05-15 17:32:17.392078 pynecone-0.1.30a0/pynecone/components/forms/__init__.py
--rw-r--r--   0        0        0     1765 2023-05-15 17:32:17.392510 pynecone-0.1.30a0/pynecone/components/forms/button.py
--rw-r--r--   0        0        0     2470 2023-05-15 02:04:07.610312 pynecone-0.1.30a0/pynecone/components/forms/checkbox.py
--rw-r--r--   0        0        0      594 2023-05-15 02:04:07.610405 pynecone-0.1.30a0/pynecone/components/forms/copytoclipboard.py
--rw-r--r--   0        0        0     1965 2023-05-15 02:04:07.610525 pynecone-0.1.30a0/pynecone/components/forms/editable.py
--rw-r--r--   0        0        0     2694 2023-05-15 17:32:17.392793 pynecone-0.1.30a0/pynecone/components/forms/formcontrol.py
--rw-r--r--   0        0        0      802 2023-05-15 02:04:07.610729 pynecone-0.1.30a0/pynecone/components/forms/iconbutton.py
--rw-r--r--   0        0        0     2896 2023-05-15 02:04:07.610887 pynecone-0.1.30a0/pynecone/components/forms/input.py
--rw-r--r--   0        0        0     3913 2023-05-15 02:04:07.610995 pynecone-0.1.30a0/pynecone/components/forms/numberinput.py
--rw-r--r--   0        0        0      253 2023-05-15 02:04:07.611101 pynecone-0.1.30a0/pynecone/components/forms/password.py
--rw-r--r--   0        0        0     2686 2023-05-15 02:04:07.611210 pynecone-0.1.30a0/pynecone/components/forms/pininput.py
--rw-r--r--   0        0        0     3059 2023-05-15 02:04:07.611316 pynecone-0.1.30a0/pynecone/components/forms/radio.py
--rw-r--r--   0        0        0     2869 2023-05-15 02:04:07.611635 pynecone-0.1.30a0/pynecone/components/forms/rangeslider.py
--rw-r--r--   0        0        0     3522 2023-05-15 02:04:07.612361 pynecone-0.1.30a0/pynecone/components/forms/select.py
--rw-r--r--   0        0        0     3140 2023-05-15 02:04:07.612880 pynecone-0.1.30a0/pynecone/components/forms/slider.py
--rw-r--r--   0        0        0     1568 2023-05-15 02:04:07.613206 pynecone-0.1.30a0/pynecone/components/forms/switch.py
--rw-r--r--   0        0        0     1547 2023-05-15 02:04:07.613331 pynecone-0.1.30a0/pynecone/components/forms/textarea.py
--rw-r--r--   0        0        0     2931 2023-05-15 02:04:07.613558 pynecone-0.1.30a0/pynecone/components/forms/upload.py
--rw-r--r--   0        0        0      351 2023-01-24 02:43:48.879007 pynecone-0.1.30a0/pynecone/components/graphing/__init__.py
--rw-r--r--   0        0        0     1357 2023-05-15 02:04:07.613685 pynecone-0.1.30a0/pynecone/components/graphing/plotly.py
--rw-r--r--   0        0        0    17360 2023-05-15 02:04:07.613960 pynecone-0.1.30a0/pynecone/components/graphing/victory.py
--rw-r--r--   0        0        0      815 2023-04-02 23:51:14.632791 pynecone-0.1.30a0/pynecone/components/layout/__init__.py
--rw-r--r--   0        0        0      324 2023-05-15 02:04:07.614167 pynecone-0.1.30a0/pynecone/components/layout/aspect_ratio.py
--rw-r--r--   0        0        0      769 2023-05-15 02:04:07.614311 pynecone-0.1.30a0/pynecone/components/layout/box.py
--rw-r--r--   0        0        0      396 2022-12-07 23:08:48.792563 pynecone-0.1.30a0/pynecone/components/layout/center.py
--rw-r--r--   0        0        0     3804 2023-05-15 02:04:07.614477 pynecone-0.1.30a0/pynecone/components/layout/cond.py
--rw-r--r--   0        0        0      363 2023-05-15 02:04:07.614634 pynecone-0.1.30a0/pynecone/components/layout/container.py
--rw-r--r--   0        0        0      656 2023-05-15 02:04:07.614740 pynecone-0.1.30a0/pynecone/components/layout/flex.py
--rw-r--r--   0        0        0     2768 2023-05-15 02:04:07.614860 pynecone-0.1.30a0/pynecone/components/layout/foreach.py
--rw-r--r--   0        0        0      314 2022-12-20 23:31:29.595612 pynecone-0.1.30a0/pynecone/components/layout/fragment.py
--rw-r--r--   0        0        0     2418 2023-05-15 02:04:07.614987 pynecone-0.1.30a0/pynecone/components/layout/grid.py
--rw-r--r--   0        0        0      979 2023-04-27 02:06:35.755389 pynecone-0.1.30a0/pynecone/components/layout/html.py
--rw-r--r--   0        0        0     1900 2023-03-10 00:25:42.702272 pynecone-0.1.30a0/pynecone/components/layout/responsive.py
--rw-r--r--   0        0        0      186 2022-12-07 23:08:48.793614 pynecone-0.1.30a0/pynecone/components/layout/spacer.py
--rw-r--r--   0        0        0      995 2023-05-15 02:04:07.615111 pynecone-0.1.30a0/pynecone/components/layout/stack.py
--rw-r--r--   0        0        0     1471 2023-05-15 02:04:07.615242 pynecone-0.1.30a0/pynecone/components/layout/wrap.py
--rw-r--r--   0        0        0       33 2022-11-18 20:43:33.727543 pynecone-0.1.30a0/pynecone/components/libs/__init__.py
--rw-r--r--   0        0        0      222 2022-11-18 20:43:33.727419 pynecone-0.1.30a0/pynecone/components/libs/chakra.py
--rw-r--r--   0        0        0      190 2022-11-18 20:43:33.736163 pynecone-0.1.30a0/pynecone/components/media/__init__.py
--rw-r--r--   0        0        0     1540 2023-05-15 02:04:07.615552 pynecone-0.1.30a0/pynecone/components/media/avatar.py
--rw-r--r--   0        0        0     2391 2023-03-16 23:52:12.745547 pynecone-0.1.30a0/pynecone/components/media/icon.py
--rw-r--r--   0        0        0     1416 2023-05-15 02:04:07.615745 pynecone-0.1.30a0/pynecone/components/media/image.py
--rw-r--r--   0        0        0      282 2023-01-24 02:43:48.884756 pynecone-0.1.30a0/pynecone/components/navigation/__init__.py
--rw-r--r--   0        0        0     2023 2023-05-15 02:04:07.615856 pynecone-0.1.30a0/pynecone/components/navigation/breadcrumb.py
--rw-r--r--   0        0        0     1083 2023-05-15 02:04:07.616009 pynecone-0.1.30a0/pynecone/components/navigation/link.py
--rw-r--r--   0        0        0      530 2023-05-15 02:04:07.616129 pynecone-0.1.30a0/pynecone/components/navigation/linkoverlay.py
--rw-r--r--   0        0        0      507 2023-05-15 02:04:07.616229 pynecone-0.1.30a0/pynecone/components/navigation/nextlink.py
--rw-r--r--   0        0        0      850 2023-01-24 02:43:48.892006 pynecone-0.1.30a0/pynecone/components/overlay/__init__.py
--rw-r--r--   0        0        0     5043 2023-05-15 02:04:07.616653 pynecone-0.1.30a0/pynecone/components/overlay/alertdialog.py
--rw-r--r--   0        0        0     4697 2023-05-15 02:04:07.616785 pynecone-0.1.30a0/pynecone/components/overlay/drawer.py
--rw-r--r--   0        0        0     5546 2023-05-15 02:04:07.617056 pynecone-0.1.30a0/pynecone/components/overlay/menu.py
--rw-r--r--   0        0        0     4933 2023-05-15 02:04:07.617172 pynecone-0.1.30a0/pynecone/components/overlay/modal.py
--rw-r--r--   0        0        0     5704 2023-05-15 02:04:07.617273 pynecone-0.1.30a0/pynecone/components/overlay/popover.py
--rw-r--r--   0        0        0     1965 2023-05-15 02:04:07.617360 pynecone-0.1.30a0/pynecone/components/overlay/tooltip.py
--rw-r--r--   0        0        0      120 2022-11-18 20:43:33.725191 pynecone-0.1.30a0/pynecone/components/tags/__init__.py
--rw-r--r--   0        0        0      451 2023-05-15 02:04:07.617454 pynecone-0.1.30a0/pynecone/components/tags/cond_tag.py
--rw-r--r--   0        0        0     2306 2023-05-15 02:04:07.617560 pynecone-0.1.30a0/pynecone/components/tags/iter_tag.py
--rw-r--r--   0        0        0     5156 2023-05-15 17:32:17.393054 pynecone-0.1.30a0/pynecone/components/tags/tag.py
--rw-r--r--   0        0        0      591 2023-03-16 23:52:12.746470 pynecone-0.1.30a0/pynecone/components/tags/tagless.py
--rw-r--r--   0        0        0      271 2022-12-07 23:08:48.795802 pynecone-0.1.30a0/pynecone/components/typography/__init__.py
--rw-r--r--   0        0        0      282 2023-05-15 02:04:07.617958 pynecone-0.1.30a0/pynecone/components/typography/heading.py
--rw-r--r--   0        0        0      358 2023-05-15 02:04:07.618079 pynecone-0.1.30a0/pynecone/components/typography/highlight.py
--rw-r--r--   0        0        0     3288 2023-05-15 02:04:07.618181 pynecone-0.1.30a0/pynecone/components/typography/markdown.py
--rw-r--r--   0        0        0      337 2023-05-15 02:04:07.618372 pynecone-0.1.30a0/pynecone/components/typography/span.py
--rw-r--r--   0        0        0      306 2023-05-15 02:04:07.618520 pynecone-0.1.30a0/pynecone/components/typography/text.py
--rw-r--r--   0        0        0     5296 2023-04-27 02:06:35.756502 pynecone-0.1.30a0/pynecone/config.py
--rw-r--r--   0        0        0     9090 2023-05-15 02:04:07.618709 pynecone-0.1.30a0/pynecone/constants.py
--rw-r--r--   0        0        0       73 2023-04-27 02:06:35.757531 pynecone-0.1.30a0/pynecone/el/__init__.py
--rw-r--r--   0        0        0      115 2023-04-27 02:06:35.757829 pynecone-0.1.30a0/pynecone/el/constants/__init__.py
--rw-r--r--   0        0        0     7175 2023-04-27 02:06:35.758045 pynecone-0.1.30a0/pynecone/el/constants/html.py
--rw-r--r--   0        0        0     1719 2023-04-27 02:06:35.758325 pynecone-0.1.30a0/pynecone/el/constants/pynecone.py
--rw-r--r--   0        0        0    15554 2023-04-27 02:06:35.758673 pynecone-0.1.30a0/pynecone/el/constants/react.py
--rw-r--r--   0        0        0     1283 2023-05-15 02:04:07.619213 pynecone-0.1.30a0/pynecone/el/element.py
--rw-r--r--   0        0        0   108518 2023-05-15 02:04:07.619552 pynecone-0.1.30a0/pynecone/el/elements/__init__.py
--rwxr-xr-x   0        0        0     2667 2023-05-15 02:04:07.619858 pynecone-0.1.30a0/pynecone/el/precompile.py
--rw-r--r--   0        0        0    10647 2023-05-15 17:32:17.393442 pynecone-0.1.30a0/pynecone/event.py
--rw-r--r--   0        0        0      113 2023-05-15 02:04:07.620772 pynecone-0.1.30a0/pynecone/middleware/__init__.py
--rw-r--r--   0        0        0     1738 2023-05-15 02:04:07.621034 pynecone-0.1.30a0/pynecone/middleware/hydrate_middleware.py
--rw-r--r--   0        0        0     1167 2023-05-15 02:04:07.621188 pynecone-0.1.30a0/pynecone/middleware/middleware.py
--rw-r--r--   0        0        0     2085 2023-04-27 23:08:51.380631 pynecone-0.1.30a0/pynecone/model.py
--rw-r--r--   0        0        0     7979 2023-05-15 17:32:17.393651 pynecone-0.1.30a0/pynecone/pc.py
--rw-r--r--   0        0        0        0 2023-03-10 00:25:42.707141 pynecone-0.1.30a0/pynecone/py.typed
--rw-r--r--   0        0        0     4108 2023-03-16 23:52:12.748303 pynecone-0.1.30a0/pynecone/route.py
--rw-r--r--   0        0        0    29790 2023-05-15 02:04:07.621653 pynecone-0.1.30a0/pynecone/state.py
--rw-r--r--   0        0        0     1060 2023-05-15 02:04:07.621889 pynecone-0.1.30a0/pynecone/style.py
--rw-r--r--   0        0        0       26 2023-05-15 02:04:07.622076 pynecone-0.1.30a0/pynecone/utils/__init__.py
--rw-r--r--   0        0        0     5318 2023-05-15 17:32:17.393927 pynecone-0.1.30a0/pynecone/utils/build.py
--rw-r--r--   0        0        0     1759 2023-05-15 02:04:07.622587 pynecone-0.1.30a0/pynecone/utils/console.py
--rw-r--r--   0        0        0     3517 2023-05-15 02:04:07.622776 pynecone-0.1.30a0/pynecone/utils/exec.py
--rw-r--r--   0        0        0    10594 2023-05-15 17:32:17.394250 pynecone-0.1.30a0/pynecone/utils/format.py
--rw-r--r--   0        0        0      587 2023-05-15 02:04:07.623144 pynecone-0.1.30a0/pynecone/utils/imports.py
--rw-r--r--   0        0        0     2451 2023-03-16 23:52:12.757162 pynecone-0.1.30a0/pynecone/utils/path_ops.py
--rw-r--r--   0        0        0    10095 2023-05-15 02:04:07.623381 pynecone-0.1.30a0/pynecone/utils/prerequisites.py
--rw-r--r--   0        0        0     3021 2023-03-16 23:52:12.757337 pynecone-0.1.30a0/pynecone/utils/processes.py
--rw-r--r--   0        0        0     2397 2023-05-15 02:04:07.623496 pynecone-0.1.30a0/pynecone/utils/telemetry.py
--rw-r--r--   0        0        0     4389 2023-05-15 02:04:07.623635 pynecone-0.1.30a0/pynecone/utils/types.py
--rw-r--r--   0        0        0     2634 2023-05-15 02:04:07.623722 pynecone-0.1.30a0/pynecone/utils/watch.py
--rw-r--r--   0        0        0    30835 2023-05-15 02:04:07.623926 pynecone-0.1.30a0/pynecone/vars.py
--rw-r--r--   0        0        0     1798 2023-05-15 17:32:46.599676 pynecone-0.1.30a0/pyproject.toml
--rw-r--r--   0        0        0     9407 1970-01-01 00:00:00.000000 pynecone-0.1.30a0/PKG-INFO
+-rw-r--r--   0        0        0    11356 2023-01-24 01:31:44.826695 pynecone-0.1.30a1/LICENSE
+-rw-r--r--   0        0        0     7876 2023-05-15 02:04:07.603507 pynecone-0.1.30a1/README.md
+-rw-r--r--   0        0        0        0 2023-04-27 02:06:35.747147 pynecone-0.1.30a1/pynecone/.templates/apps/counter/__init__.py
+-rw-r--r--   0        0        0     1340 2023-05-16 19:12:26.220987 pynecone-0.1.30a1/pynecone/.templates/apps/counter/counter.py
+-rw-r--r--   0        0        0        0 2023-04-27 02:06:35.747631 pynecone-0.1.30a1/pynecone/.templates/apps/default/__init__.py
+-rw-r--r--   0        0        0     1036 2023-04-27 02:06:35.747905 pynecone-0.1.30a1/pynecone/.templates/apps/default/default.py
+-rw-r--r--   0        0        0    15406 2022-11-18 20:43:33.740339 pynecone-0.1.30a1/pynecone/.templates/assets/favicon.ico
+-rw-r--r--   0        0        0      183 2023-05-15 02:04:07.604358 pynecone-0.1.30a1/pynecone/.templates/jinja/app/pcconfig.py.jinja2
+-rw-r--r--   0        0        0      182 2023-05-15 02:04:07.604515 pynecone-0.1.30a1/pynecone/.templates/jinja/web/pages/_document.js.jinja2
+-rw-r--r--   0        0        0      241 2023-05-15 02:04:07.604581 pynecone-0.1.30a1/pynecone/.templates/jinja/web/pages/base_page.js.jinja2
+-rw-r--r--   0        0        0      252 2023-05-15 02:04:07.604642 pynecone-0.1.30a1/pynecone/.templates/jinja/web/pages/custom_component.js.jinja2
+-rw-r--r--   0        0        0     2345 2023-05-16 19:33:51.153974 pynecone-0.1.30a1/pynecone/.templates/jinja/web/pages/index.js.jinja2
+-rw-r--r--   0        0        0     2999 2023-05-15 02:04:07.604822 pynecone-0.1.30a1/pynecone/.templates/jinja/web/pages/utils.js.jinja2
+-rw-r--r--   0        0        0       38 2023-05-15 02:04:07.604905 pynecone-0.1.30a1/pynecone/.templates/jinja/web/utils/theme.js.jinja2
+-rw-r--r--   0        0        0      417 2022-12-27 07:35:12.085907 pynecone-0.1.30a1/pynecone/.templates/web/.gitignore
+-rwxr-xr-x   0        0        0   254417 2023-05-15 02:04:07.606023 pynecone-0.1.30a1/pynecone/.templates/web/bun.lockb
+-rw-r--r--   0        0        0       47 2022-12-20 23:31:29.590974 pynecone-0.1.30a1/pynecone/.templates/web/next.config.js
+-rw-r--r--   0        0        0      927 2023-05-15 02:04:07.606305 pynecone-0.1.30a1/pynecone/.templates/web/package.json
+-rw-r--r--   0        0        0      502 2022-11-18 20:43:33.740024 pynecone-0.1.30a1/pynecone/.templates/web/pages/404.js
+-rw-r--r--   0        0        0      564 2023-01-12 05:38:04.342282 pynecone-0.1.30a1/pynecone/.templates/web/pages/_app.js
+-rw-r--r--   0        0        0    29404 2022-12-20 23:31:29.592485 pynecone-0.1.30a1/pynecone/.templates/web/styles/code/prism.js
+-rw-r--r--   0        0        0     7657 2023-05-16 19:33:51.154248 pynecone-0.1.30a1/pynecone/.templates/web/utils/state.js
+-rw-r--r--   0        0        0     1363 2023-05-15 02:04:07.606665 pynecone-0.1.30a1/pynecone/__init__.py
+-rw-r--r--   0        0        0    20075 2023-05-15 02:04:07.606864 pynecone-0.1.30a1/pynecone/app.py
+-rw-r--r--   0        0        0     2510 2023-01-30 21:50:18.206745 pynecone-0.1.30a1/pynecone/base.py
+-rw-r--r--   0        0        0       29 2022-11-18 20:43:33.740719 pynecone-0.1.30a1/pynecone/compiler/__init__.py
+-rw-r--r--   0        0        0     6290 2023-05-16 19:33:51.154440 pynecone-0.1.30a1/pynecone/compiler/compiler.py
+-rw-r--r--   0        0        0     2565 2023-05-15 02:04:07.607300 pynecone-0.1.30a1/pynecone/compiler/templates.py
+-rw-r--r--   0        0        0     7384 2023-05-15 02:04:07.607425 pynecone-0.1.30a1/pynecone/compiler/utils.py
+-rw-r--r--   0        0        0     6390 2023-05-15 17:32:17.391279 pynecone-0.1.30a1/pynecone/components/__init__.py
+-rw-r--r--   0        0        0      226 2023-03-13 04:10:28.615930 pynecone-0.1.30a1/pynecone/components/base/__init__.py
+-rw-r--r--   0        0        0      727 2023-05-15 02:04:07.607680 pynecone-0.1.30a1/pynecone/components/base/bare.py
+-rw-r--r--   0        0        0      153 2023-03-13 04:10:28.760655 pynecone-0.1.30a1/pynecone/components/base/body.py
+-rw-r--r--   0        0        0      725 2023-01-30 22:40:32.678074 pynecone-0.1.30a1/pynecone/components/base/document.py
+-rw-r--r--   0        0        0      265 2023-05-15 02:04:07.607851 pynecone-0.1.30a1/pynecone/components/base/head.py
+-rw-r--r--   0        0        0      930 2023-05-15 02:04:07.607989 pynecone-0.1.30a1/pynecone/components/base/link.py
+-rw-r--r--   0        0        0     1340 2023-05-15 02:04:07.608303 pynecone-0.1.30a1/pynecone/components/base/meta.py
+-rw-r--r--   0        0        0    22653 2023-05-16 19:11:41.005106 pynecone-0.1.30a1/pynecone/components/component.py
+-rw-r--r--   0        0        0      422 2023-04-02 23:51:14.632016 pynecone-0.1.30a1/pynecone/components/datadisplay/__init__.py
+-rw-r--r--   0        0        0      334 2023-05-15 02:04:07.608726 pynecone-0.1.30a1/pynecone/components/datadisplay/badge.py
+-rw-r--r--   0        0        0     2513 2023-05-15 02:04:07.608840 pynecone-0.1.30a1/pynecone/components/datadisplay/code.py
+-rw-r--r--   0        0        0     4033 2023-05-15 02:04:07.608953 pynecone-0.1.30a1/pynecone/components/datadisplay/datatable.py
+-rw-r--r--   0        0        0      537 2023-05-15 02:04:07.609045 pynecone-0.1.30a1/pynecone/components/datadisplay/divider.py
+-rw-r--r--   0        0        0      187 2023-04-02 23:51:14.632124 pynecone-0.1.30a1/pynecone/components/datadisplay/keyboard_key.py
+-rw-r--r--   0        0        0     1430 2023-05-15 02:04:07.609140 pynecone-0.1.30a1/pynecone/components/datadisplay/list.py
+-rw-r--r--   0        0        0     2157 2023-05-15 02:04:07.609232 pynecone-0.1.30a1/pynecone/components/datadisplay/stat.py
+-rw-r--r--   0        0        0     5157 2023-05-15 02:04:07.609333 pynecone-0.1.30a1/pynecone/components/datadisplay/table.py
+-rw-r--r--   0        0        0      316 2023-01-24 02:43:48.871608 pynecone-0.1.30a1/pynecone/components/disclosure/__init__.py
+-rw-r--r--   0        0        0     2941 2023-05-15 02:04:07.609439 pynecone-0.1.30a1/pynecone/components/disclosure/accordion.py
+-rw-r--r--   0        0        0     2777 2023-05-15 02:04:07.609534 pynecone-0.1.30a1/pynecone/components/disclosure/tabs.py
+-rw-r--r--   0        0        0      285 2022-12-05 22:26:47.605453 pynecone-0.1.30a1/pynecone/components/disclosure/visuallyhidden.py
+-rw-r--r--   0        0        0      313 2022-11-18 20:43:33.723246 pynecone-0.1.30a1/pynecone/components/feedback/__init__.py
+-rw-r--r--   0        0        0     1571 2023-05-15 02:04:07.609649 pynecone-0.1.30a1/pynecone/components/feedback/alert.py
+-rw-r--r--   0        0        0     1905 2023-05-15 02:04:07.609745 pynecone-0.1.30a1/pynecone/components/feedback/circularprogress.py
+-rw-r--r--   0        0        0      879 2023-05-15 02:04:07.609838 pynecone-0.1.30a1/pynecone/components/feedback/progress.py
+-rw-r--r--   0        0        0     1785 2023-05-15 02:04:07.609925 pynecone-0.1.30a1/pynecone/components/feedback/skeleton.py
+-rw-r--r--   0        0        0      678 2023-05-15 02:04:07.610013 pynecone-0.1.30a1/pynecone/components/feedback/spinner.py
+-rw-r--r--   0        0        0     1109 2023-05-16 05:05:39.515505 pynecone-0.1.30a1/pynecone/components/forms/__init__.py
+-rw-r--r--   0        0        0     1765 2023-05-15 17:32:17.392510 pynecone-0.1.30a1/pynecone/components/forms/button.py
+-rw-r--r--   0        0        0     2454 2023-05-16 19:11:41.005270 pynecone-0.1.30a1/pynecone/components/forms/checkbox.py
+-rw-r--r--   0        0        0      578 2023-05-16 19:11:41.005389 pynecone-0.1.30a1/pynecone/components/forms/copytoclipboard.py
+-rw-r--r--   0        0        0     1949 2023-05-16 19:11:41.005504 pynecone-0.1.30a1/pynecone/components/forms/editable.py
+-rw-r--r--   0        0        0     2965 2023-05-16 19:11:41.005634 pynecone-0.1.30a1/pynecone/components/forms/formcontrol.py
+-rw-r--r--   0        0        0      802 2023-05-15 02:04:07.610729 pynecone-0.1.30a1/pynecone/components/forms/iconbutton.py
+-rw-r--r--   0        0        0     2880 2023-05-16 19:11:41.005746 pynecone-0.1.30a1/pynecone/components/forms/input.py
+-rw-r--r--   0        0        0     3897 2023-05-16 19:11:41.005870 pynecone-0.1.30a1/pynecone/components/forms/numberinput.py
+-rw-r--r--   0        0        0      253 2023-05-15 02:04:07.611101 pynecone-0.1.30a1/pynecone/components/forms/password.py
+-rw-r--r--   0        0        0     2670 2023-05-16 19:11:41.006022 pynecone-0.1.30a1/pynecone/components/forms/pininput.py
+-rw-r--r--   0        0        0     3043 2023-05-16 19:11:41.006148 pynecone-0.1.30a1/pynecone/components/forms/radio.py
+-rw-r--r--   0        0        0     2853 2023-05-16 19:11:41.006264 pynecone-0.1.30a1/pynecone/components/forms/rangeslider.py
+-rw-r--r--   0        0        0     3506 2023-05-16 19:11:41.006377 pynecone-0.1.30a1/pynecone/components/forms/select.py
+-rw-r--r--   0        0        0     3124 2023-05-16 19:11:41.006525 pynecone-0.1.30a1/pynecone/components/forms/slider.py
+-rw-r--r--   0        0        0     1552 2023-05-16 19:11:41.006661 pynecone-0.1.30a1/pynecone/components/forms/switch.py
+-rw-r--r--   0        0        0     1531 2023-05-16 19:11:41.006795 pynecone-0.1.30a1/pynecone/components/forms/textarea.py
+-rw-r--r--   0        0        0     2915 2023-05-16 19:11:41.006932 pynecone-0.1.30a1/pynecone/components/forms/upload.py
+-rw-r--r--   0        0        0      351 2023-01-24 02:43:48.879007 pynecone-0.1.30a1/pynecone/components/graphing/__init__.py
+-rw-r--r--   0        0        0     1357 2023-05-15 02:04:07.613685 pynecone-0.1.30a1/pynecone/components/graphing/plotly.py
+-rw-r--r--   0        0        0    17360 2023-05-15 02:04:07.613960 pynecone-0.1.30a1/pynecone/components/graphing/victory.py
+-rw-r--r--   0        0        0      815 2023-04-02 23:51:14.632791 pynecone-0.1.30a1/pynecone/components/layout/__init__.py
+-rw-r--r--   0        0        0      324 2023-05-15 02:04:07.614167 pynecone-0.1.30a1/pynecone/components/layout/aspect_ratio.py
+-rw-r--r--   0        0        0      769 2023-05-15 02:04:07.614311 pynecone-0.1.30a1/pynecone/components/layout/box.py
+-rw-r--r--   0        0        0      396 2022-12-07 23:08:48.792563 pynecone-0.1.30a1/pynecone/components/layout/center.py
+-rw-r--r--   0        0        0     3844 2023-05-16 19:11:41.007084 pynecone-0.1.30a1/pynecone/components/layout/cond.py
+-rw-r--r--   0        0        0      363 2023-05-15 02:04:07.614634 pynecone-0.1.30a1/pynecone/components/layout/container.py
+-rw-r--r--   0        0        0      656 2023-05-15 02:04:07.614740 pynecone-0.1.30a1/pynecone/components/layout/flex.py
+-rw-r--r--   0        0        0     2843 2023-05-16 19:11:41.007298 pynecone-0.1.30a1/pynecone/components/layout/foreach.py
+-rw-r--r--   0        0        0      314 2022-12-20 23:31:29.595612 pynecone-0.1.30a1/pynecone/components/layout/fragment.py
+-rw-r--r--   0        0        0     2418 2023-05-15 02:04:07.614987 pynecone-0.1.30a1/pynecone/components/layout/grid.py
+-rw-r--r--   0        0        0      979 2023-04-27 02:06:35.755389 pynecone-0.1.30a1/pynecone/components/layout/html.py
+-rw-r--r--   0        0        0     1900 2023-03-10 00:25:42.702272 pynecone-0.1.30a1/pynecone/components/layout/responsive.py
+-rw-r--r--   0        0        0      186 2022-12-07 23:08:48.793614 pynecone-0.1.30a1/pynecone/components/layout/spacer.py
+-rw-r--r--   0        0        0      995 2023-05-15 02:04:07.615111 pynecone-0.1.30a1/pynecone/components/layout/stack.py
+-rw-r--r--   0        0        0     1471 2023-05-15 02:04:07.615242 pynecone-0.1.30a1/pynecone/components/layout/wrap.py
+-rw-r--r--   0        0        0       33 2022-11-18 20:43:33.727543 pynecone-0.1.30a1/pynecone/components/libs/__init__.py
+-rw-r--r--   0        0        0      222 2022-11-18 20:43:33.727419 pynecone-0.1.30a1/pynecone/components/libs/chakra.py
+-rw-r--r--   0        0        0      190 2022-11-18 20:43:33.736163 pynecone-0.1.30a1/pynecone/components/media/__init__.py
+-rw-r--r--   0        0        0     1524 2023-05-16 19:11:41.007509 pynecone-0.1.30a1/pynecone/components/media/avatar.py
+-rw-r--r--   0        0        0     2391 2023-03-16 23:52:12.745547 pynecone-0.1.30a1/pynecone/components/media/icon.py
+-rw-r--r--   0        0        0     1400 2023-05-16 19:11:41.007692 pynecone-0.1.30a1/pynecone/components/media/image.py
+-rw-r--r--   0        0        0      282 2023-01-24 02:43:48.884756 pynecone-0.1.30a1/pynecone/components/navigation/__init__.py
+-rw-r--r--   0        0        0     2023 2023-05-15 02:04:07.615856 pynecone-0.1.30a1/pynecone/components/navigation/breadcrumb.py
+-rw-r--r--   0        0        0     1083 2023-05-15 02:04:07.616009 pynecone-0.1.30a1/pynecone/components/navigation/link.py
+-rw-r--r--   0        0        0      530 2023-05-15 02:04:07.616129 pynecone-0.1.30a1/pynecone/components/navigation/linkoverlay.py
+-rw-r--r--   0        0        0      507 2023-05-15 02:04:07.616229 pynecone-0.1.30a1/pynecone/components/navigation/nextlink.py
+-rw-r--r--   0        0        0      850 2023-01-24 02:43:48.892006 pynecone-0.1.30a1/pynecone/components/overlay/__init__.py
+-rw-r--r--   0        0        0     5027 2023-05-16 19:11:41.008011 pynecone-0.1.30a1/pynecone/components/overlay/alertdialog.py
+-rw-r--r--   0        0        0     4681 2023-05-16 19:11:41.008241 pynecone-0.1.30a1/pynecone/components/overlay/drawer.py
+-rw-r--r--   0        0        0     5530 2023-05-16 19:11:41.008524 pynecone-0.1.30a1/pynecone/components/overlay/menu.py
+-rw-r--r--   0        0        0     4917 2023-05-16 19:11:41.008688 pynecone-0.1.30a1/pynecone/components/overlay/modal.py
+-rw-r--r--   0        0        0     5688 2023-05-16 19:11:41.008862 pynecone-0.1.30a1/pynecone/components/overlay/popover.py
+-rw-r--r--   0        0        0     1949 2023-05-16 19:11:41.009041 pynecone-0.1.30a1/pynecone/components/overlay/tooltip.py
+-rw-r--r--   0        0        0      120 2022-11-18 20:43:33.725191 pynecone-0.1.30a1/pynecone/components/tags/__init__.py
+-rw-r--r--   0        0        0      451 2023-05-15 02:04:07.617454 pynecone-0.1.30a1/pynecone/components/tags/cond_tag.py
+-rw-r--r--   0        0        0     2306 2023-05-15 02:04:07.617560 pynecone-0.1.30a1/pynecone/components/tags/iter_tag.py
+-rw-r--r--   0        0        0     5018 2023-05-16 19:11:41.009247 pynecone-0.1.30a1/pynecone/components/tags/tag.py
+-rw-r--r--   0        0        0      591 2023-03-16 23:52:12.746470 pynecone-0.1.30a1/pynecone/components/tags/tagless.py
+-rw-r--r--   0        0        0      271 2022-12-07 23:08:48.795802 pynecone-0.1.30a1/pynecone/components/typography/__init__.py
+-rw-r--r--   0        0        0      282 2023-05-15 02:04:07.617958 pynecone-0.1.30a1/pynecone/components/typography/heading.py
+-rw-r--r--   0        0        0      358 2023-05-15 02:04:07.618079 pynecone-0.1.30a1/pynecone/components/typography/highlight.py
+-rw-r--r--   0        0        0     3288 2023-05-15 02:04:07.618181 pynecone-0.1.30a1/pynecone/components/typography/markdown.py
+-rw-r--r--   0        0        0      337 2023-05-15 02:04:07.618372 pynecone-0.1.30a1/pynecone/components/typography/span.py
+-rw-r--r--   0        0        0      306 2023-05-15 02:04:07.618520 pynecone-0.1.30a1/pynecone/components/typography/text.py
+-rw-r--r--   0        0        0     5296 2023-04-27 02:06:35.756502 pynecone-0.1.30a1/pynecone/config.py
+-rw-r--r--   0        0        0     8974 2023-05-16 04:11:28.941645 pynecone-0.1.30a1/pynecone/constants.py
+-rw-r--r--   0        0        0       73 2023-04-27 02:06:35.757531 pynecone-0.1.30a1/pynecone/el/__init__.py
+-rw-r--r--   0        0        0      115 2023-04-27 02:06:35.757829 pynecone-0.1.30a1/pynecone/el/constants/__init__.py
+-rw-r--r--   0        0        0     7175 2023-04-27 02:06:35.758045 pynecone-0.1.30a1/pynecone/el/constants/html.py
+-rw-r--r--   0        0        0     1719 2023-04-27 02:06:35.758325 pynecone-0.1.30a1/pynecone/el/constants/pynecone.py
+-rw-r--r--   0        0        0    15554 2023-04-27 02:06:35.758673 pynecone-0.1.30a1/pynecone/el/constants/react.py
+-rw-r--r--   0        0        0     1283 2023-05-15 02:04:07.619213 pynecone-0.1.30a1/pynecone/el/element.py
+-rw-r--r--   0        0        0   108518 2023-05-15 02:04:07.619552 pynecone-0.1.30a1/pynecone/el/elements/__init__.py
+-rwxr-xr-x   0        0        0     2667 2023-05-15 02:04:07.619858 pynecone-0.1.30a1/pynecone/el/precompile.py
+-rw-r--r--   0        0        0    10647 2023-05-15 17:32:17.393442 pynecone-0.1.30a1/pynecone/event.py
+-rw-r--r--   0        0        0      113 2023-05-15 02:04:07.620772 pynecone-0.1.30a1/pynecone/middleware/__init__.py
+-rw-r--r--   0        0        0     1738 2023-05-15 02:04:07.621034 pynecone-0.1.30a1/pynecone/middleware/hydrate_middleware.py
+-rw-r--r--   0        0        0     1167 2023-05-15 02:04:07.621188 pynecone-0.1.30a1/pynecone/middleware/middleware.py
+-rw-r--r--   0        0        0     2085 2023-04-27 23:08:51.380631 pynecone-0.1.30a1/pynecone/model.py
+-rw-r--r--   0        0        0     7979 2023-05-15 17:32:17.393651 pynecone-0.1.30a1/pynecone/pc.py
+-rw-r--r--   0        0        0        0 2023-03-10 00:25:42.707141 pynecone-0.1.30a1/pynecone/py.typed
+-rw-r--r--   0        0        0     4108 2023-03-16 23:52:12.748303 pynecone-0.1.30a1/pynecone/route.py
+-rw-r--r--   0        0        0    29790 2023-05-15 02:04:07.621653 pynecone-0.1.30a1/pynecone/state.py
+-rw-r--r--   0        0        0     1060 2023-05-15 02:04:07.621889 pynecone-0.1.30a1/pynecone/style.py
+-rw-r--r--   0        0        0       26 2023-05-15 02:04:07.622076 pynecone-0.1.30a1/pynecone/utils/__init__.py
+-rw-r--r--   0        0        0     5318 2023-05-15 17:32:17.393927 pynecone-0.1.30a1/pynecone/utils/build.py
+-rw-r--r--   0        0        0     1759 2023-05-15 02:04:07.622587 pynecone-0.1.30a1/pynecone/utils/console.py
+-rw-r--r--   0        0        0     3517 2023-05-15 02:04:07.622776 pynecone-0.1.30a1/pynecone/utils/exec.py
+-rw-r--r--   0        0        0    11346 2023-05-16 19:11:41.009451 pynecone-0.1.30a1/pynecone/utils/format.py
+-rw-r--r--   0        0        0      587 2023-05-15 02:04:07.623144 pynecone-0.1.30a1/pynecone/utils/imports.py
+-rw-r--r--   0        0        0     2451 2023-03-16 23:52:12.757162 pynecone-0.1.30a1/pynecone/utils/path_ops.py
+-rw-r--r--   0        0        0    10033 2023-05-16 04:11:28.941837 pynecone-0.1.30a1/pynecone/utils/prerequisites.py
+-rw-r--r--   0        0        0     3021 2023-03-16 23:52:12.757337 pynecone-0.1.30a1/pynecone/utils/processes.py
+-rw-r--r--   0        0        0     2397 2023-05-15 02:04:07.623496 pynecone-0.1.30a1/pynecone/utils/telemetry.py
+-rw-r--r--   0        0        0     4389 2023-05-15 02:04:07.623635 pynecone-0.1.30a1/pynecone/utils/types.py
+-rw-r--r--   0        0        0     2634 2023-05-15 02:04:07.623722 pynecone-0.1.30a1/pynecone/utils/watch.py
+-rw-r--r--   0        0        0    30918 2023-05-16 19:11:41.009774 pynecone-0.1.30a1/pynecone/vars.py
+-rw-r--r--   0        0        0     1798 2023-05-16 19:34:33.336016 pynecone-0.1.30a1/pyproject.toml
+-rw-r--r--   0        0        0     9407 1970-01-01 00:00:00.000000 pynecone-0.1.30a1/PKG-INFO
```

### Comparing `pynecone-0.1.30a0/LICENSE` & `pynecone-0.1.30a1/LICENSE`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a0/README.md` & `pynecone-0.1.30a1/README.md`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a0/pynecone/.templates/apps/counter/counter.py` & `pynecone-0.1.30a1/pynecone/.templates/apps/counter/counter.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a0/pynecone/.templates/apps/default/default.py` & `pynecone-0.1.30a1/pynecone/.templates/apps/default/default.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a0/pynecone/.templates/assets/favicon.ico` & `pynecone-0.1.30a1/pynecone/.templates/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a0/pynecone/.templates/jinja/web/pages/index.js.jinja2` & `pynecone-0.1.30a1/pynecone/.templates/jinja/web/pages/index.js.jinja2`

 * *Files 2% similar despite different names*

```diff
@@ -15,18 +15,21 @@
   const [{{state_name}}, {{state_name|react_setter}}] = useState({{initial_state|json_dumps}})
   const [{{const.result}}, {{const.result|react_setter}}] = useState({{const.initial_result|json_dumps}})
   const {{const.router}} = useRouter()
   const {{const.socket}} = useRef(null)
   const { isReady } = {{const.router}}
   const { {{const.color_mode}}, {{const.toggle_color_mode}} } = {{const.use_color_mode}}()
 
-  const Event = events => {{state_name|react_setter}}({
-    ...{{state_name}},
-    events: [...{{state_name}}.events, ...events],
-  })
+  const Event = (events, _e) => {
+      preventDefault(_e);
+      {{state_name|react_setter}}({
+        ...{{state_name}},
+        events: [...{{state_name}}.events, ...events],
+      })
+  }
 
   const File = files => {{state_name|react_setter}}({
     ...{{state_name}},
     files,
   })
 
   useEffect(()=>{
@@ -47,16 +50,16 @@
           {{const.state}}: null,
           {{const.events}}: [],
           {{const.processing}}: false,
         })
       }
 
       await updateState({{state_name}}, {{state_name|react_setter}}, {{const.result}}, {{const.result|react_setter}}, {{const.router}}, {{const.socket}}.current)
-      }
-      update()
+    }
+    update()
   })
   useEffect(() => {
     const change_complete = () => Event([E('{{state_name}}.{{const.hydrate}}', {})])
     {{const.router}}.events.on('routeChangeComplete', change_complete)
     return () => {
       {{const.router}}.events.off('routeChangeComplete', change_complete)
     }
```

### Comparing `pynecone-0.1.30a0/pynecone/.templates/jinja/web/pages/utils.js.jinja2` & `pynecone-0.1.30a1/pynecone/.templates/jinja/web/pages/utils.js.jinja2`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a0/pynecone/.templates/web/bun.lockb` & `pynecone-0.1.30a1/pynecone/.templates/web/bun.lockb`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a0/pynecone/.templates/web/package.json` & `pynecone-0.1.30a1/pynecone/.templates/web/package.json`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a0/pynecone/.templates/web/pages/_app.js` & `pynecone-0.1.30a1/pynecone/.templates/web/pages/_app.js`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a0/pynecone/.templates/web/styles/code/prism.js` & `pynecone-0.1.30a1/pynecone/.templates/web/styles/code/prism.js`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a0/pynecone/.templates/web/utils/state.js` & `pynecone-0.1.30a1/pynecone/.templates/web/utils/state.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,20 +1,23 @@
 // State management for Pynecone web apps.
 import axios from "axios";
 import io from "socket.io-client";
 import JSON5 from "json5";
-import config from "../pynecone.json"
+import config from "../pynecone.json";
 
 const UPLOAD = config.uploadUrl;
 // Global variable to hold the token.
 let token;
 
 // Key for the token in the session storage.
 const TOKEN_KEY = "token";
 
+// Dictionary holding component references.
+export const refs = {};
+
 /**
  * Generate a UUID (Used for session tokens).
  * Taken from: https://stackoverflow.com/questions/105034/how-do-i-create-a-guid-uuid
  * @returns A UUID.
  */
 const generateUUID = () => {
     let d = new Date().getTime(),
@@ -89,16 +92,17 @@
 
     if (event.name == "_alert") {
         alert(event.payload.message);
         return false;
     }
 
     if (event.name == "_set_value") {
-        event.payload.ref.current.blur();
-        event.payload.ref.current.value = event.payload.value;
+        const ref =
+            event.payload.ref in refs ? refs[event.payload.ref] : event.payload.ref;
+        ref.current.value = event.payload.value;
         return false;
     }
 
     // Send the event to the server.
     event.token = getToken();
     event.router_data = (({
         pathname,
@@ -117,25 +121,19 @@
 
 /**
  * Process an event off the event queue.
  * @param queue_event The current event
  * @param state The state with the event queue.
  * @param setResult The function to set the result.
  */
-export const applyRestEvent = async (
-    queue_event,
-    state,
-    setResult,
-) => {
+export const applyRestEvent = async (queue_event, state, setResult) => {
     if (queue_event.handler == "uploadFiles") {
-        await uploadFiles(state, setResult, queue_event.name, UPLOAD)
+        await uploadFiles(state, setResult, queue_event.name, UPLOAD);
     }
-
-}
-
+};
 
 /**
  * Process an event off the event queue.
  * @param state The state with the event queue.
  * @param setState The function to set the state.
  * @param result The current result.
  * @param setResult The function to set the result.
@@ -167,33 +165,27 @@
     setState({
         ...state,
         events: state.events
     });
 
     // Process events with handlers via REST and all others via websockets.
     if (queue_event.handler) {
-
-        await applyRestEvent(queue_event, state, setResult)
-
-
+        await applyRestEvent(queue_event, state, setResult);
     } else {
         const eventSent = await applyEvent(queue_event, router, socket);
         if (!eventSent) {
             // If no event was sent, set processing to false and return.
             setResult({
                 ...state,
                 processing: false
             });
         }
     }
-
-
 };
 
-
 /**
  * Connect to a websocket and set the handlers.
  * @param socket The socket object to connect.
  * @param state The state object to apply the deltas to.
  * @param setState The function to set the state.
  * @param result The current result.
  * @param setResult The function to set the result.
@@ -240,35 +232,34 @@
  * Upload files to the server.
  *
  * @param state The state to apply the delta to.
  * @param setResult The function to set the result.
  * @param handler The handler to use.
  * @param endpoint The endpoint to upload to.
  */
-export const uploadFiles = async (
-    state,
-    setResult,
-    handler,
-    endpoint
-) => {
-    const files = state.files
+export const uploadFiles = async (state, setResult, handler, endpoint) => {
+    const files = state.files;
 
     // return if there's no file to upload
     if (files.length == 0) {
-        return
+        return;
     }
 
     const headers = {
         "Content-Type": files[0].type,
     };
     const formdata = new FormData();
 
     // Add the token and handler to the file name.
     for (let i = 0; i < files.length; i++) {
-        formdata.append("files", files[i], getToken() + ":" + handler + ":" + files[i].name);
+        formdata.append(
+            "files",
+            files[i],
+            getToken() + ":" + handler + ":" + files[i].name
+        );
     }
 
     // Send the file to the server.
     await axios.post(endpoint, formdata, headers).then((response) => {
         // Apply the delta and set the result.
         const update = response.data;
         applyDelta(state, update.delta);
@@ -294,16 +285,25 @@
     return {
         name,
         payload,
         handler
     };
 };
 
-
 /***
  * Check if a value is truthy in python.
  * @param val The value to check.
  * @returns True if the value is truthy, false otherwise.
  */
 export const isTrue = (val) => {
-    return Array.isArray(val) ? val.length > 0 : !!val
-}
+    return Array.isArray(val) ? val.length > 0 : !!val;
+};
+
+/**
+ * Prevent the default event.
+ * @param event
+ */
+export const preventDefault = (event) => {
+    if (event && event.hasOwnProperty("preventDefault")) {
+        event.preventDefault();
+    }
+};
```

### Comparing `pynecone-0.1.30a0/pynecone/__init__.py` & `pynecone-0.1.30a1/pynecone/__init__.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a0/pynecone/app.py` & `pynecone-0.1.30a1/pynecone/app.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a0/pynecone/base.py` & `pynecone-0.1.30a1/pynecone/base.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a0/pynecone/compiler/compiler.py` & `pynecone-0.1.30a1/pynecone/compiler/compiler.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,16 @@
     "next/router": {ImportVar(tag="useRouter")},
     f"/{constants.STATE_PATH}": {
         ImportVar(tag="connect"),
         ImportVar(tag="updateState"),
         ImportVar(tag="uploadFiles"),
         ImportVar(tag="E"),
         ImportVar(tag="isTrue"),
+        ImportVar(tag="preventDefault"),
+        ImportVar(tag="refs"),
     },
     "": {ImportVar(tag="focus-visible/dist/focus-visible")},
     "@chakra-ui/react": {ImportVar(tag=constants.USE_COLOR_MODE)},
 }
 
 
 def _compile_document_root(root: Component) -> str:
```

### Comparing `pynecone-0.1.30a0/pynecone/compiler/templates.py` & `pynecone-0.1.30a1/pynecone/compiler/templates.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a0/pynecone/compiler/utils.py` & `pynecone-0.1.30a1/pynecone/compiler/utils.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a0/pynecone/components/__init__.py` & `pynecone-0.1.30a1/pynecone/components/__init__.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a0/pynecone/components/base/bare.py` & `pynecone-0.1.30a1/pynecone/components/base/bare.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a0/pynecone/components/base/document.py` & `pynecone-0.1.30a1/pynecone/components/base/document.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a0/pynecone/components/base/link.py` & `pynecone-0.1.30a1/pynecone/components/base/link.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a0/pynecone/components/base/meta.py` & `pynecone-0.1.30a1/pynecone/components/base/meta.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a0/pynecone/components/component.py` & `pynecone-0.1.30a1/pynecone/components/component.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,14 +90,21 @@
         Args:
             *args: Args to initialize the component.
             **kwargs: Kwargs to initialize the component.
 
         Raises:
             TypeError: If an invalid prop is passed.
         """
+        # Set the id and children initially.
+        initial_kwargs = {
+            "id": kwargs.get("id"),
+            "children": kwargs.get("children", []),
+        }
+        super().__init__(**initial_kwargs)
+
         # Get the component fields, triggers, and props.
         fields = self.get_fields()
         triggers = self.get_triggers()
         props = self.get_props()
 
         # Add any events triggers.
         if "event_triggers" not in kwargs:
@@ -260,25 +267,23 @@
         state_name = state_name if full_control else ""
 
         # Return the event chain.
         return EventChain(
             events=events, state_name=state_name, full_control=full_control
         )
 
-    @classmethod
-    def get_triggers(cls) -> Set[str]:
+    def get_triggers(self) -> Set[str]:
         """Get the event triggers for the component.
 
         Returns:
             The event triggers.
         """
-        return EVENT_TRIGGERS | set(cls.get_controlled_triggers())
+        return EVENT_TRIGGERS | set(self.get_controlled_triggers())
 
-    @classmethod
-    def get_controlled_triggers(cls) -> Dict[str, Var]:
+    def get_controlled_triggers(self) -> Dict[str, Var]:
         """Get the event triggers that pass the component's value to the handler.
 
         Returns:
             A dict mapping the event trigger to the var that is passed to the handler.
         """
         return {}
 
@@ -465,15 +470,15 @@
         """Get the React hooks for this component.
 
         Returns:
             The hooks for just this component.
         """
         ref = self.get_ref()
         if ref is not None:
-            return f"const {ref} = useRef(null);"
+            return f"const {ref} = useRef(null); refs['{ref}'] = {ref};"
         return None
 
     def get_hooks(self) -> Set[str]:
         """Get the React hooks for this component and its children.
 
         Returns:
             The code that should appear just before returning the rendered component.
@@ -484,28 +489,42 @@
         # Add the hook code for this component.
         hooks = self._get_hooks()
         if hooks is not None:
             code.add(hooks)
 
         # Add the hook code for the children.
         for child in self.children:
-            code.update(child.get_hooks())
+            code |= child.get_hooks()
 
         return code
 
     def get_ref(self) -> Optional[str]:
         """Get the name of the ref for the component.
 
         Returns:
             The ref name.
         """
         if self.id is None:
             return None
         return format.format_ref(self.id)
 
+    def get_refs(self) -> Set[str]:
+        """Get the refs for the children of the component.
+
+        Returns:
+            The refs for the children.
+        """
+        refs = set()
+        ref = self.get_ref()
+        if ref is not None:
+            refs.add(ref)
+        for child in self.children:
+            refs |= child.get_refs()
+        return refs
+
     def get_custom_components(
         self, seen: Optional[Set[str]] = None
     ) -> Set[CustomComponent]:
         """Get all the custom components used by the component.
 
         Args:
             seen: The tags of the components that have already been seen.
@@ -561,15 +580,15 @@
 class CustomComponent(Component):
     """A custom user-defined component."""
 
     # Use the components library.
     library = f"/{constants.COMPONENTS_PATH}"
 
     # The function that creates the component.
-    component_fn: Callable[..., Component]
+    component_fn: Callable[..., Component] = Component.create
 
     # The props of the component.
     props: Dict[str, Any] = {}
 
     def __init__(self, *args, **kwargs):
         """Initialize the custom component.
```

### Comparing `pynecone-0.1.30a0/pynecone/components/datadisplay/code.py` & `pynecone-0.1.30a1/pynecone/components/datadisplay/code.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a0/pynecone/components/datadisplay/datatable.py` & `pynecone-0.1.30a1/pynecone/components/datadisplay/datatable.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a0/pynecone/components/datadisplay/divider.py` & `pynecone-0.1.30a1/pynecone/components/datadisplay/divider.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a0/pynecone/components/datadisplay/list.py` & `pynecone-0.1.30a1/pynecone/components/datadisplay/list.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a0/pynecone/components/datadisplay/stat.py` & `pynecone-0.1.30a1/pynecone/components/datadisplay/stat.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a0/pynecone/components/datadisplay/table.py` & `pynecone-0.1.30a1/pynecone/components/datadisplay/table.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a0/pynecone/components/disclosure/accordion.py` & `pynecone-0.1.30a1/pynecone/components/disclosure/accordion.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a0/pynecone/components/disclosure/tabs.py` & `pynecone-0.1.30a1/pynecone/components/disclosure/tabs.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a0/pynecone/components/feedback/alert.py` & `pynecone-0.1.30a1/pynecone/components/feedback/alert.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a0/pynecone/components/feedback/circularprogress.py` & `pynecone-0.1.30a1/pynecone/components/feedback/circularprogress.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a0/pynecone/components/feedback/progress.py` & `pynecone-0.1.30a1/pynecone/components/feedback/progress.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a0/pynecone/components/feedback/skeleton.py` & `pynecone-0.1.30a1/pynecone/components/feedback/skeleton.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a0/pynecone/components/feedback/spinner.py` & `pynecone-0.1.30a1/pynecone/components/feedback/spinner.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a0/pynecone/components/forms/__init__.py` & `pynecone-0.1.30a1/pynecone/components/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a0/pynecone/components/forms/button.py` & `pynecone-0.1.30a1/pynecone/components/forms/button.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a0/pynecone/components/forms/checkbox.py` & `pynecone-0.1.30a1/pynecone/components/forms/checkbox.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,16 +44,15 @@
 
     # The name of the input field in a checkbox (Useful for form submission).
     name: Var[str]
 
     # The spacing between the checkbox and its label text (0.5rem)
     spacing: Var[str]
 
-    @classmethod
-    def get_controlled_triggers(cls) -> Dict[str, Var]:
+    def get_controlled_triggers(self) -> Dict[str, Var]:
         """Get the event triggers that pass the component's value to the handler.
 
         Returns:
             A dict mapping the event trigger to the var that is passed to the handler.
         """
         return {
             "on_change": EVENT_ARG.target.checked,
```

### Comparing `pynecone-0.1.30a0/pynecone/components/forms/copytoclipboard.py` & `pynecone-0.1.30a1/pynecone/components/forms/copytoclipboard.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,14 @@
     library = "react-copy-to-clipboard"
 
     tag = "CopyToClipboard"
 
     # The text to copy when clicked.
     text: Var[str]
 
-    @classmethod
-    def get_controlled_triggers(cls) -> Set[str]:
+    def get_controlled_triggers(self) -> Set[str]:
         """Get the event triggers that pass the component's value to the handler.
 
         Returns:
             The controlled event triggers.
         """
         return {"on_copy"}
```

### Comparing `pynecone-0.1.30a0/pynecone/components/forms/editable.py` & `pynecone-0.1.30a1/pynecone/components/forms/editable.py`

 * *Files 11% similar despite different names*

```diff
@@ -32,16 +32,15 @@
 
     # The value of the Editable in both edit & preview mode
     value: Var[str]
 
     # The initial value of the Editable in both edit and preview mode.
     default_value: Var[str]
 
-    @classmethod
-    def get_controlled_triggers(cls) -> Dict[str, Var]:
+    def get_controlled_triggers(self) -> Dict[str, Var]:
         """Get the event triggers that pass the component's value to the handler.
 
         Returns:
             A dict mapping the event trigger to the var that is passed to the handler.
         """
         return {
             "on_change": EVENT_ARG,
```

### Comparing `pynecone-0.1.30a0/pynecone/components/forms/formcontrol.py` & `pynecone-0.1.30a1/pynecone/components/forms/formcontrol.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 """Form components."""
 
-from typing import Set
+from typing import Dict
 
 from pynecone.components.component import Component
 from pynecone.components.libs.chakra import ChakraComponent
 from pynecone.vars import Var
 
 
 class Form(ChakraComponent):
     """A form component."""
 
     tag = "Box"
 
     as_: Var[str] = "form"  # type: ignore
 
-    @classmethod
-    def get_triggers(cls) -> Set[str]:
-        """Get the event triggers for the component.
+    def get_controlled_triggers(self) -> Dict[str, Dict]:
+        """Get the event triggers that pass the component's value to the handler.
 
         Returns:
-            The event triggers.
+            A dict mapping the event trigger to the var that is passed to the handler.
         """
-        return super().get_triggers() | {"on_submit"}
+        # Send all the input refs to the handler.
+        return {
+            "on_submit": {
+                ref[4:]: Var.create(f"{ref}.current.value", is_local=False)
+                for ref in self.get_refs()
+            }
+        }
 
 
 class FormControl(ChakraComponent):
     """Provide context to form components."""
 
     tag = "FormControl"
 
@@ -48,15 +53,15 @@
     def create(
         cls,
         *children,
         label=None,
         input=None,
         help_text=None,
         error_message=None,
-        **props
+        **props,
     ) -> Component:
         """Create a form control component.
 
         Args:
             children: The children of the form control.
             label: The label of the form control.
             input: The input of the form control.
```

### Comparing `pynecone-0.1.30a0/pynecone/components/forms/iconbutton.py` & `pynecone-0.1.30a1/pynecone/components/forms/iconbutton.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a0/pynecone/components/forms/input.py` & `pynecone-0.1.30a1/pynecone/components/forms/input.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,16 +51,15 @@
 
     def _get_imports(self) -> imports.ImportDict:
         return imports.merge_imports(
             super()._get_imports(),
             {"/utils/state": {ImportVar(tag="set_val")}},
         )
 
-    @classmethod
-    def get_controlled_triggers(cls) -> Dict[str, Var]:
+    def get_controlled_triggers(self) -> Dict[str, Var]:
         """Get the event triggers that pass the component's value to the handler.
 
         Returns:
             A dict mapping the event trigger to the var that is passed to the handler.
         """
         return {
             "on_change": EVENT_ARG.target.value,
```

### Comparing `pynecone-0.1.30a0/pynecone/components/forms/numberinput.py` & `pynecone-0.1.30a1/pynecone/components/forms/numberinput.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,16 +60,15 @@
 
     # The minimum value of the counter
     min_: Var[int]
 
     # "outline" | "filled" | "flushed" | "unstyled"
     variant: Var[str]
 
-    @classmethod
-    def get_controlled_triggers(cls) -> Dict[str, Var]:
+    def get_controlled_triggers(self) -> Dict[str, Var]:
         """Get the event triggers that pass the component's value to the handler.
 
         Returns:
             A dict mapping the event trigger to the var that is passed to the handler.
         """
         return {
             "on_change": EVENT_ARG,
```

### Comparing `pynecone-0.1.30a0/pynecone/components/forms/pininput.py` & `pynecone-0.1.30a1/pynecone/components/forms/pininput.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,16 +51,15 @@
 
     # The type of values the pin-input should allow ("number" | "alphanumeric").
     type_: Var[str]
 
     # "outline" | "flushed" | "filled" | "unstyled"
     variant: Var[str]
 
-    @classmethod
-    def get_controlled_triggers(cls) -> Dict[str, Var]:
+    def get_controlled_triggers(self) -> Dict[str, Var]:
         """Get the event triggers that pass the component's value to the handler.
 
         Returns:
             A dict mapping the event trigger to the var that is passed to the handler.
         """
         return {
             "on_change": EVENT_ARG,
```

### Comparing `pynecone-0.1.30a0/pynecone/components/forms/radio.py` & `pynecone-0.1.30a1/pynecone/components/forms/radio.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,16 +19,15 @@
 
     # State var to bind the the input.
     value: Var[Any]
 
     # The default value.
     default_value: Var[Any]
 
-    @classmethod
-    def get_controlled_triggers(cls) -> Dict[str, Var]:
+    def get_controlled_triggers(self) -> Dict[str, Var]:
         """Get the event triggers that pass the component's value to the handler.
 
         Returns:
             A dict mapping the event trigger to the var that is passed to the handler.
         """
         return {
             "on_change": EVENT_ARG,
```

### Comparing `pynecone-0.1.30a0/pynecone/components/forms/rangeslider.py` & `pynecone-0.1.30a1/pynecone/components/forms/rangeslider.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,16 +39,15 @@
 
     # The maximum value of the slider.
     max_: Var[int]
 
     # The minimum distance between slider thumbs. Useful for preventing the thumbs from being too close together.
     min_steps_between_thumbs: Var[int]
 
-    @classmethod
-    def get_controlled_triggers(cls) -> Dict[str, Var]:
+    def get_controlled_triggers(self) -> Dict[str, Var]:
         """Get the event triggers that pass the component's value to the handler.
 
         Returns:
             A dict mapping the event trigger to the var that is passed to the handler.
         """
         return {
             "on_change": EVENT_ARG,
```

### Comparing `pynecone-0.1.30a0/pynecone/components/forms/select.py` & `pynecone-0.1.30a1/pynecone/components/forms/select.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,16 +44,15 @@
 
     # "outline" | "filled" | "flushed" | "unstyled"
     variant: Var[str]
 
     # The size of the select.
     size: Var[str]
 
-    @classmethod
-    def get_controlled_triggers(cls) -> Dict[str, Var]:
+    def get_controlled_triggers(self) -> Dict[str, Var]:
         """Get the event triggers that pass the component's value to the handler.
 
         Returns:
             A dict mapping the event trigger to the var that is passed to the handler.
         """
         return {
             "on_change": EVENT_ARG.target.value,
```

### Comparing `pynecone-0.1.30a0/pynecone/components/forms/slider.py` & `pynecone-0.1.30a1/pynecone/components/forms/slider.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,16 +57,15 @@
 
     # Maximum height of the slider.
     max_h: Var[str]
 
     # Maximum width of the slider.
     max_w: Var[str]
 
-    @classmethod
-    def get_controlled_triggers(cls) -> Dict[str, Var]:
+    def get_controlled_triggers(self) -> Dict[str, Var]:
         """Get the event triggers that pass the component's value to the handler.
 
         Returns:
             A dict mapping the event trigger to the var that is passed to the handler.
         """
         return {
             "on_change": EVENT_ARG,
```

### Comparing `pynecone-0.1.30a0/pynecone/components/forms/switch.py` & `pynecone-0.1.30a1/pynecone/components/forms/switch.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,16 +37,15 @@
 
     # The placeholder text.
     placeholder: Var[str]
 
     # The color scheme of the switch (e.g. "blue", "green", "red", etc.)
     color_scheme: Var[str]
 
-    @classmethod
-    def get_controlled_triggers(cls) -> Dict[str, Var]:
+    def get_controlled_triggers(self) -> Dict[str, Var]:
         """Get the event triggers that pass the component's value to the handler.
 
         Returns:
             A dict mapping the event trigger to the var that is passed to the handler.
         """
         return {
             "on_change": EVENT_ARG.target.checked,
```

### Comparing `pynecone-0.1.30a0/pynecone/components/forms/textarea.py` & `pynecone-0.1.30a1/pynecone/components/forms/textarea.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,16 +38,15 @@
 
     # If true, the form control will be required.
     is_required: Var[bool]
 
     # "outline" | "filled" | "flushed" | "unstyled"
     variant: Var[str]
 
-    @classmethod
-    def get_controlled_triggers(cls) -> Dict[str, Var]:
+    def get_controlled_triggers(self) -> Dict[str, Var]:
         """Get the event triggers that pass the component's value to the handler.
 
         Returns:
             A dict mapping the event trigger to the var that is passed to the handler.
         """
         return {
             "on_change": EVENT_ARG.target.value,
```

### Comparing `pynecone-0.1.30a0/pynecone/components/forms/upload.py` & `pynecone-0.1.30a1/pynecone/components/forms/upload.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,16 +76,15 @@
             **{k: v for k, v in props.items() if k not in supported_props}
         )
         zone.special_props = {BaseVar(name="{...getRootProps()}", type_=None)}
 
         # Create the component.
         return super().create(zone, on_drop=upload_file, **upload_props)
 
-    @classmethod
-    def get_controlled_triggers(cls) -> Dict[str, Var]:
+    def get_controlled_triggers(self) -> Dict[str, Var]:
         """Get the event triggers that pass the component's value to the handler.
 
         Returns:
             A dict mapping the event trigger to the var that is passed to the handler.
         """
         return {
             "on_drop": EVENT_ARG,
```

### Comparing `pynecone-0.1.30a0/pynecone/components/graphing/plotly.py` & `pynecone-0.1.30a1/pynecone/components/graphing/plotly.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a0/pynecone/components/graphing/victory.py` & `pynecone-0.1.30a1/pynecone/components/graphing/victory.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a0/pynecone/components/layout/__init__.py` & `pynecone-0.1.30a1/pynecone/components/layout/__init__.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a0/pynecone/components/layout/box.py` & `pynecone-0.1.30a1/pynecone/components/layout/box.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a0/pynecone/components/layout/cond.py` & `pynecone-0.1.30a1/pynecone/components/layout/cond.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 class Cond(Component):
     """Render one of two components based on a condition."""
 
     # The cond to determine which component to render.
     cond: Var[Any]
 
     # The component to render if the cond is true.
-    comp1: Component
+    comp1: Component = Fragment.create()
 
     # The component to render if the cond is false.
-    comp2: Component
+    comp2: Component = Fragment.create()
 
     @classmethod
     def create(
         cls, cond: Var, comp1: Component, comp2: Optional[Component]
     ) -> Component:
         """Create a conditional component.
```

### Comparing `pynecone-0.1.30a0/pynecone/components/layout/flex.py` & `pynecone-0.1.30a1/pynecone/components/layout/flex.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a0/pynecone/components/layout/foreach.py` & `pynecone-0.1.30a1/pynecone/components/layout/foreach.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 """Create a list of components from an iterable."""
 from __future__ import annotations
 
 from typing import Any, Callable, List
 
 from pynecone.components.component import Component
+from pynecone.components.layout.fragment import Fragment
 from pynecone.components.tags import IterTag
 from pynecone.vars import BaseVar, Var, get_unique_variable_name
 
 
 class Foreach(Component):
     """A component that takes in an iterable and a render function and renders a list of components."""
 
     # The iterable to create components from.
     iterable: Var[List]
 
     # A function from the render args to the component.
-    render_fn: Callable
+    render_fn: Callable = Fragment.create
 
     @classmethod
     def create(cls, iterable: Var[List], render_fn: Callable, **props) -> Foreach:
         """Create a foreach component.
 
         Args:
             iterable: The iterable to create components from.
```

### Comparing `pynecone-0.1.30a0/pynecone/components/layout/grid.py` & `pynecone-0.1.30a1/pynecone/components/layout/grid.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a0/pynecone/components/layout/html.py` & `pynecone-0.1.30a1/pynecone/components/layout/html.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a0/pynecone/components/layout/responsive.py` & `pynecone-0.1.30a1/pynecone/components/layout/responsive.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a0/pynecone/components/layout/stack.py` & `pynecone-0.1.30a1/pynecone/components/layout/stack.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a0/pynecone/components/layout/wrap.py` & `pynecone-0.1.30a1/pynecone/components/layout/wrap.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a0/pynecone/components/media/avatar.py` & `pynecone-0.1.30a1/pynecone/components/media/avatar.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,16 +31,15 @@
 
     # List of sources to use for different screen resolutions.
     src_set: Var[str]
 
     # "2xs" | "xs" | "sm" | "md" | "lg" | "xl" | "2xl" | "full"
     size: Var[str]
 
-    @classmethod
-    def get_triggers(cls) -> Set[str]:
+    def get_triggers(self) -> Set[str]:
         """Get the event triggers for the component.
 
         Returns:
             The event triggers.
         """
         return super().get_triggers() | {"on_error"}
```

### Comparing `pynecone-0.1.30a0/pynecone/components/media/icon.py` & `pynecone-0.1.30a1/pynecone/components/media/icon.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a0/pynecone/components/media/image.py` & `pynecone-0.1.30a1/pynecone/components/media/image.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,14 @@
 
     # The image src attribute.
     src: Var[str]
 
     # The image srcset attribute.
     src_set: Var[str]
 
-    @classmethod
-    def get_triggers(cls) -> Set[str]:
+    def get_triggers(self) -> Set[str]:
         """Get the event triggers for the component.
 
         Returns:
             The event triggers.
         """
         return super().get_triggers() | {"on_error", "on_load"}
```

### Comparing `pynecone-0.1.30a0/pynecone/components/navigation/breadcrumb.py` & `pynecone-0.1.30a1/pynecone/components/navigation/breadcrumb.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a0/pynecone/components/navigation/link.py` & `pynecone-0.1.30a1/pynecone/components/navigation/link.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a0/pynecone/components/navigation/linkoverlay.py` & `pynecone-0.1.30a1/pynecone/components/navigation/linkoverlay.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a0/pynecone/components/overlay/__init__.py` & `pynecone-0.1.30a1/pynecone/components/overlay/__init__.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a0/pynecone/components/overlay/alertdialog.py` & `pynecone-0.1.30a1/pynecone/components/overlay/alertdialog.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,16 +48,15 @@
 
     # "xs" | "sm" | "md" | "lg" | "xl" | "2xl" | "3xl" | "4xl" | "5xl" | "6xl" | "full"
     size: Var[str]
 
     # If true, the siblings of the modal will have `aria-hidden` set to true so that screen readers can only see the modal. This is commonly known as making the other elements **inert**
     use_inert: Var[bool]
 
-    @classmethod
-    def get_triggers(cls) -> Set[str]:
+    def get_triggers(self) -> Set[str]:
         """Get the event triggers for the component.
 
         Returns:
             The event triggers.
         """
         return super().get_triggers() | {
             "on_close",
```

### Comparing `pynecone-0.1.30a0/pynecone/components/overlay/drawer.py` & `pynecone-0.1.30a1/pynecone/components/overlay/drawer.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,16 +54,15 @@
 
     # A11y: If true, the siblings of the modal will have `aria-hidden` set to true so that screen readers can only see the modal. This is commonly known as making the other elements **inert**
     use_inert: Var[bool]
 
     # Variant of drawer
     variant: Var[str]
 
-    @classmethod
-    def get_triggers(cls) -> Set[str]:
+    def get_triggers(self) -> Set[str]:
         """Get the event triggers for the component.
 
         Returns:
             The event triggers.
         """
         return super().get_triggers() | {
             "on_close",
```

### Comparing `pynecone-0.1.30a0/pynecone/components/overlay/menu.py` & `pynecone-0.1.30a1/pynecone/components/overlay/menu.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,16 +56,15 @@
 
     # If true, will prevent the popper from being cut off and ensure it's visible within the boundary area.
     prevent_overflow: Var[bool]
 
     # The CSS positioning strategy to use. ("fixed" | "absolute")
     strategy: Var[str]
 
-    @classmethod
-    def get_triggers(cls) -> Set[str]:
+    def get_triggers(self) -> Set[str]:
         """Get the event triggers for the component.
 
         Returns:
             The event triggers.
         """
         return super().get_triggers() | {"on_close", "on_open"}
```

### Comparing `pynecone-0.1.30a0/pynecone/components/overlay/modal.py` & `pynecone-0.1.30a1/pynecone/components/overlay/modal.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,16 +48,15 @@
 
     # "xs" | "sm" | "md" | "lg" | "xl" | "2xl" | "3xl" | "4xl" | "5xl" | "6xl" | "full"
     size: Var[str]
 
     # A11y: If true, the siblings of the modal will have `aria-hidden` set to true so that screen readers can only see the modal. This is commonly known as making the other elements **inert**
     use_inert: Var[bool]
 
-    @classmethod
-    def get_triggers(cls) -> Set[str]:
+    def get_triggers(self) -> Set[str]:
         """Get the event triggers for the component.
 
         Returns:
             The event triggers.
         """
         return super().get_triggers() | {
             "on_close",
```

### Comparing `pynecone-0.1.30a0/pynecone/components/overlay/popover.py` & `pynecone-0.1.30a1/pynecone/components/overlay/popover.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,16 +71,15 @@
 
     # The CSS positioning strategy to use. ("fixed" | "absolute")
     strategy: Var[str]
 
     # The interaction that triggers the popover. hover - means the popover will open when you hover with mouse or focus with keyboard on the popover trigger click - means the popover will open on click or press Enter to Space on keyboard ("click" | "hover")
     trigger: Var[str]
 
-    @classmethod
-    def get_triggers(cls) -> Set[str]:
+    def get_triggers(self) -> Set[str]:
         """Get the event triggers for the component.
 
         Returns:
             The event triggers.
         """
         return super().get_triggers() | {"on_close", "on_open"}
```

### Comparing `pynecone-0.1.30a0/pynecone/components/overlay/tooltip.py` & `pynecone-0.1.30a1/pynecone/components/overlay/tooltip.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,15 +58,14 @@
 
     # The placement of the popper relative to its reference.
     placement: Var[str]
 
     # If true, the tooltip will wrap its children in a `<span/>` with `tabIndex=0`
     should_wrap_children: Var[bool]
 
-    @classmethod
-    def get_triggers(cls) -> Set[str]:
+    def get_triggers(self) -> Set[str]:
         """Get the event triggers for the component.
 
         Returns:
             The event triggers.
         """
         return super().get_triggers() | {"on_close", "on_open"}
```

### Comparing `pynecone-0.1.30a0/pynecone/components/tags/iter_tag.py` & `pynecone-0.1.30a1/pynecone/components/tags/iter_tag.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a0/pynecone/components/tags/tag.py` & `pynecone-0.1.30a1/pynecone/components/tags/tag.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """A React tag."""
 
 from __future__ import annotations
 
 import json
-import re
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Set, Tuple, Union
 
 from plotly.graph_objects import Figure
 from plotly.io import to_json
 
 from pynecone.base import Base
 from pynecone.event import EVENT_ARG, EventChain
@@ -60,14 +59,17 @@
         """Format a prop.
 
         Args:
             prop: The prop to format.
 
         Returns:
             The formatted prop to display within a tag.
+
+        Raises:
+            TypeError: If the prop is not a valid type.
         """
         # Handle var props.
         if isinstance(prop, Var):
             if not prop.is_local or prop.is_string:
                 return str(prop)
             if types._issubclass(prop.type_, str):
                 return format.json_dumps(prop.full_name)
@@ -77,42 +79,38 @@
         elif isinstance(prop, EventChain):
             if prop.full_control:
                 # Full control component events.
                 event = format.format_full_control_event(prop)
             else:
                 # All other events.
                 chain = ",".join([format.format_event(event) for event in prop.events])
-                event = f"{{{EVENT_ARG}.preventDefault(); Event([{chain}])}}"
-            prop = f"({EVENT_ARG}) => {event}"
+                event = f"Event([{chain}], {EVENT_ARG})"
+            prop = f"{EVENT_ARG} => {event}"
 
         # Handle other types.
         elif isinstance(prop, str):
             if format.is_wrapped(prop, "{"):
                 return prop
             return format.json_dumps(prop)
 
         elif isinstance(prop, Figure):
             prop = json.loads(to_json(prop))["data"]  # type: ignore
 
         # For dictionaries, convert any properties to strings.
-        else:
-            if isinstance(prop, dict):
-                # Convert any var keys to strings.
-                prop = {
-                    key: str(val) if isinstance(val, Var) else val
-                    for key, val in prop.items()
-                }
+        elif isinstance(prop, dict):
+            prop = format.format_dict(prop)
 
+        else:
             # Dump the prop as JSON.
-            prop = format.json_dumps(prop)
-
-            # This substitution is necessary to unwrap var values.
-            prop = re.sub('"{', "", prop)
-            prop = re.sub('}"', "", prop)
-            prop = re.sub('\\\\"', '"', prop)
+            try:
+                prop = format.json_dumps(prop)
+            except TypeError as e:
+                raise TypeError(
+                    f"Could not format prop: {prop} of type {type(prop)}"
+                ) from e
 
         # Wrap the variable in braces.
         assert isinstance(prop, str), "The prop must be a string."
         return format.wrap(prop, "{", check_first=False)
 
     def format_props(self) -> List:
         """Format the tag's props.
```

### Comparing `pynecone-0.1.30a0/pynecone/components/tags/tagless.py` & `pynecone-0.1.30a1/pynecone/components/tags/tagless.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a0/pynecone/components/typography/markdown.py` & `pynecone-0.1.30a1/pynecone/components/typography/markdown.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a0/pynecone/config.py` & `pynecone-0.1.30a1/pynecone/config.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a0/pynecone/constants.py` & `pynecone-0.1.30a1/pynecone/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,27 +4,24 @@
 import re
 from enum import Enum
 from types import SimpleNamespace
 
 import pkg_resources
 
 # App names and versions.
-# The name of the Pynecone module.
+# The name of the Pynecone package.
 MODULE_NAME = "pynecone"
-# The name of the pip install package.
-PACKAGE_NAME = "pynecone"
 # The current version of Pynecone.
-VERSION = pkg_resources.get_distribution(PACKAGE_NAME).version
+VERSION = pkg_resources.get_distribution(MODULE_NAME).version
 # Minimum version of Node.js required to run Pynecone.
 MIN_NODE_VERSION = "16.6.0"
 
 # Valid bun versions.
 MIN_BUN_VERSION = "0.5.9"
 MAX_BUN_VERSION = "0.5.9"
-INVALID_BUN_VERSIONS = ["0.5.5", "0.5.6", "0.5.7"]
 
 # Files and directories used to init a new project.
 # The root directory of the pynecone library.
 ROOT_DIR = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
 # The name of the assets directory.
 APP_ASSETS_DIR = "assets"
 # The template directory used during pc init.
```

### Comparing `pynecone-0.1.30a0/pynecone/el/constants/html.py` & `pynecone-0.1.30a1/pynecone/el/constants/html.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a0/pynecone/el/constants/pynecone.py` & `pynecone-0.1.30a1/pynecone/el/constants/pynecone.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a0/pynecone/el/constants/react.py` & `pynecone-0.1.30a1/pynecone/el/constants/react.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a0/pynecone/el/element.py` & `pynecone-0.1.30a1/pynecone/el/element.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a0/pynecone/el/elements/__init__.py` & `pynecone-0.1.30a1/pynecone/el/elements/__init__.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a0/pynecone/el/precompile.py` & `pynecone-0.1.30a1/pynecone/el/precompile.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a0/pynecone/event.py` & `pynecone-0.1.30a1/pynecone/event.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a0/pynecone/middleware/hydrate_middleware.py` & `pynecone-0.1.30a1/pynecone/middleware/hydrate_middleware.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a0/pynecone/middleware/middleware.py` & `pynecone-0.1.30a1/pynecone/middleware/middleware.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a0/pynecone/model.py` & `pynecone-0.1.30a1/pynecone/model.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a0/pynecone/pc.py` & `pynecone-0.1.30a1/pynecone/pc.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a0/pynecone/route.py` & `pynecone-0.1.30a1/pynecone/route.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a0/pynecone/state.py` & `pynecone-0.1.30a1/pynecone/state.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a0/pynecone/style.py` & `pynecone-0.1.30a1/pynecone/style.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a0/pynecone/utils/build.py` & `pynecone-0.1.30a1/pynecone/utils/build.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a0/pynecone/utils/console.py` & `pynecone-0.1.30a1/pynecone/utils/console.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a0/pynecone/utils/exec.py` & `pynecone-0.1.30a1/pynecone/utils/exec.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a0/pynecone/utils/format.py` & `pynecone-0.1.30a1/pynecone/utils/format.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import plotly.graph_objects as go
 from plotly.io import to_json
 
 from pynecone import constants
 from pynecone.utils import types
 
 if TYPE_CHECKING:
+    from pynecone.components.component import ComponentStyle
     from pynecone.event import EventChain, EventHandler, EventSpec
 
 WRAP_MAP = {
     "{": "}",
     "(": ")",
     "[": "]",
     "<": ">",
@@ -407,14 +408,41 @@
         The formatted ref.
     """
     # Replace all non-word characters with underscores.
     clean_ref = re.sub(r"[^\w]+", "_", ref)
     return f"ref_{clean_ref}"
 
 
+def format_dict(prop: ComponentStyle) -> str:
+    """Format a dict with vars potentially as values.
+
+    Args:
+        prop: The dict to format.
+
+    Returns:
+        The formatted dict.
+    """
+    # Import here to avoid circular imports.
+    from pynecone.vars import Var
+
+    # Convert any var keys to strings.
+    prop = {key: str(val) if isinstance(val, Var) else val for key, val in prop.items()}
+
+    # Dump the dict to a string.
+    fprop = json_dumps(prop)
+
+    # This substitution is necessary to unwrap var values.
+    fprop = re.sub('"{', "", fprop)
+    fprop = re.sub('}"', "", fprop)
+    fprop = re.sub('\\\\"', '"', fprop)
+
+    # Return the formatted dict.
+    return fprop
+
+
 def json_dumps(obj: Any) -> str:
     """Takes an object and returns a jsonified string.
 
     Args:
         obj: The object to be serialized.
 
     Returns:
```

### Comparing `pynecone-0.1.30a0/pynecone/utils/imports.py` & `pynecone-0.1.30a1/pynecone/utils/imports.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a0/pynecone/utils/path_ops.py` & `pynecone-0.1.30a1/pynecone/utils/path_ops.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a0/pynecone/utils/prerequisites.py` & `pynecone-0.1.30a1/pynecone/utils/prerequisites.py`

 * *Files 2% similar despite different names*

```diff
@@ -226,15 +226,14 @@
         Exit: If the bun version is not supported.
 
     """
     bun_version = get_bun_version()
     if bun_version is not None and (
         bun_version < version.parse(constants.MIN_BUN_VERSION)
         or bun_version > version.parse(constants.MAX_BUN_VERSION)
-        or str(bun_version) in constants.INVALID_BUN_VERSIONS
     ):
         console.print(
             f"""[red]Bun version {bun_version} is not supported by Pynecone. Please change your to bun version to be between {constants.MIN_BUN_VERSION} and {constants.MAX_BUN_VERSION}."""
         )
         action = console.ask(
             "Enter 'yes' to install the latest supported bun version or 'no' to exit.",
             choices=["yes", "no"],
```

### Comparing `pynecone-0.1.30a0/pynecone/utils/processes.py` & `pynecone-0.1.30a1/pynecone/utils/processes.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a0/pynecone/utils/telemetry.py` & `pynecone-0.1.30a1/pynecone/utils/telemetry.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a0/pynecone/utils/types.py` & `pynecone-0.1.30a1/pynecone/utils/types.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a0/pynecone/utils/watch.py` & `pynecone-0.1.30a1/pynecone/utils/watch.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a0/pynecone/vars.py` & `pynecone-0.1.30a1/pynecone/vars.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,14 +97,17 @@
         type_ = type(value)
 
         # Special case for plotly figures.
         if isinstance(value, Figure):
             value = json.loads(to_json(value))["data"]  # type: ignore
             type_ = Figure
 
+        if isinstance(value, dict):
+            value = format.format_dict(value)
+
         try:
             name = value if isinstance(value, str) else json.dumps(value)
         except TypeError as e:
             raise TypeError(
                 f"To create a Var must be Var or JSON-serializable. Got {value} of type {type(value)}."
             ) from e
```

### Comparing `pynecone-0.1.30a0/pyproject.toml` & `pynecone-0.1.30a1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pynecone"
-version = "0.1.30a0"
+version = "0.1.30a1"
 description = "Web apps in pure Python."
 license = "Apache-2.0"
 authors = [
     "Nikhil Rao <nikhil@pynecone.io>",
     "Alek Petuskey <alek@pynecone.io>",
 ]
 readme = "README.md"
```

### Comparing `pynecone-0.1.30a0/PKG-INFO` & `pynecone-0.1.30a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynecone
-Version: 0.1.30a0
+Version: 0.1.30a1
 Summary: Web apps in pure Python.
 Home-page: https://pynecone.io
 License: Apache-2.0
 Keywords: web,framework
 Author: Nikhil Rao
 Author-email: nikhil@pynecone.io
 Requires-Python: >=3.7,<4.0
```

