# Comparing `tmp/tuack-0.1.5.tar.gz` & `tmp/tuack-0.1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tuack-0.1.5.tar", last modified: Sat May 13 04:22:15 2023, max compression
+gzip compressed data, was "tuack-0.1.5.1.tar", last modified: Tue May 16 13:21:22 2023, max compression
```

## Comparing `tuack-0.1.5.tar` & `tuack-0.1.5.1.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxrwxrwx   0        0        0        0 2023-05-13 04:22:15.336016 tuack-0.1.5/
--rw-rw-rw-   0        0        0    35055 2019-01-19 08:45:12.000000 tuack-0.1.5/LICENSE
--rw-rw-rw-   0        0        0       17 2018-03-03 08:40:20.000000 tuack-0.1.5/MANIFEST.in
--rw-rw-rw-   0        0        0      518 2023-05-13 04:22:15.336016 tuack-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     1717 2023-01-09 01:26:59.000000 tuack-0.1.5/README.md
--rw-rw-rw-   0        0        0       42 2023-05-13 04:22:15.336016 tuack-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1926 2023-05-13 04:18:17.000000 tuack-0.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-13 04:22:14.885832 tuack-0.1.5/tuack/
--rw-rw-rw-   0        0        0      116 2018-03-03 08:40:20.000000 tuack-0.1.5/tuack/__init__.py
--rw-rw-rw-   0        0        0    34145 2023-05-13 04:08:47.000000 tuack-0.1.5/tuack/base.py
--rw-rw-rw-   0        0        0    13348 2023-01-09 01:26:59.000000 tuack-0.1.5/tuack/doc.py
--rw-rw-rw-   0        0        0    27313 2023-05-13 04:13:10.000000 tuack-0.1.5/tuack/dump.py
--rw-rw-rw-   0        0        0    14486 2023-01-09 01:26:59.000000 tuack-0.1.5/tuack/gen.py
--rw-rw-rw-   0        0        0     2334 2023-01-09 01:26:59.000000 tuack-0.1.5/tuack/install.py
-drwxrwxrwx   0        0        0        0 2023-05-13 04:22:15.097790 tuack-0.1.5/tuack/lex/
--rw-rw-rw-   0        0        0        0 2018-09-07 13:38:42.000000 tuack-0.1.5/tuack/lex/compile.log
--rw-rw-rw-   0        0        0      971 2019-01-19 08:45:12.000000 tuack-0.1.5/tuack/lex/compile.pyinc
--rw-rw-rw-   0        0        0  2295192 2019-01-19 08:45:12.000000 tuack-0.1.5/tuack/lex/format-linux
--rw-rw-rw-   0        0        0    61896 2019-01-19 08:45:12.000000 tuack-0.1.5/tuack/lex/format-mac
--rwxrwxrwx   0        0        0  2178321 2019-01-19 08:45:12.000000 tuack-0.1.5/tuack/lex/format-win.exe
--rw-rw-rw-   0        0        0      320 2018-08-27 16:45:44.000000 tuack-0.1.5/tuack/lex/hehe.log
--rw-rw-rw-   0        0        0    11191 2019-01-19 08:45:12.000000 tuack-0.1.5/tuack/lex/lex.l
--rw-rw-rw-   0        0        0    94066 2018-09-07 13:38:44.000000 tuack-0.1.5/tuack/lex/lex.yy.c
--rw-rw-rw-   0        0        0    36942 2018-06-11 12:35:42.000000 tuack-0.1.5/tuack/lex/lex.yy.o
--rw-rw-rw-   0        0        0      185 2019-01-19 08:45:12.000000 tuack-0.1.5/tuack/lex/main.h
--rw-rw-rw-   0        0        0    42594 2018-09-07 13:38:44.000000 tuack-0.1.5/tuack/lex/yacc.tab.c
--rw-rw-rw-   0        0        0     1906 2018-09-07 13:38:44.000000 tuack-0.1.5/tuack/lex/yacc.tab.h
--rw-rw-rw-   0        0        0     9007 2018-06-11 12:35:42.000000 tuack-0.1.5/tuack/lex/yacc.tab.o
--rw-rw-rw-   0        0        0      388 2019-01-19 08:45:12.000000 tuack-0.1.5/tuack/lex/yacc.y
--rw-rw-rw-   0        0        0    12225 2023-01-09 01:26:59.000000 tuack-0.1.5/tuack/load.py
--rw-rw-rw-   0        0        0     3605 2019-01-19 08:45:12.000000 tuack-0.1.5/tuack/num2chinese.py
--rw-rw-rw-   0        0        0    12608 2018-03-03 08:40:20.000000 tuack-0.1.5/tuack/packer.py
--rw-rw-rw-   0        0        0    24468 2023-04-24 01:29:13.000000 tuack-0.1.5/tuack/ren.py
-drwxrwxrwx   0        0        0        0 2023-05-13 04:22:15.163722 tuack-0.1.5/tuack/sample/
--rw-rw-rw-   0        0        0     7909 2023-01-09 01:26:59.000000 tuack-0.1.5/tuack/sample/arbiter_e.noi_linux1.sample
--rw-rw-rw-   0        0        0    23576 2023-01-09 01:26:59.000000 tuack-0.1.5/tuack/sample/arbiter_e.sample
--rw-rw-rw-   0        0        0     5586 2023-01-09 01:26:59.000000 tuack-0.1.5/tuack/sample/chk.cpp
--rw-rw-rw-   0        0        0      195 2023-01-09 01:26:59.000000 tuack-0.1.5/tuack/sample/contest.gitignore
--rw-rw-rw-   0        0        0      266 2023-01-09 01:26:59.000000 tuack-0.1.5/tuack/sample/contest.json
--rw-rw-rw-   0        0        0      186 2023-01-09 01:26:59.000000 tuack-0.1.5/tuack/sample/day.gitignore
--rw-rw-rw-   0        0        0      207 2023-01-09 01:26:59.000000 tuack-0.1.5/tuack/sample/day.json
--rw-rw-rw-   0        0        0      351 2023-01-09 01:26:59.000000 tuack-0.1.5/tuack/sample/empty.gitattributes
--rw-rw-rw-   0        0        0      254 2023-01-09 01:26:59.000000 tuack-0.1.5/tuack/sample/empty.gitignore
--rw-rw-rw-   0        0        0      435 2023-01-09 01:26:59.000000 tuack-0.1.5/tuack/sample/empty.json
-drwxrwxrwx   0        0        0        0 2023-05-13 04:22:15.218786 tuack-0.1.5/tuack/sample/precautions/
--rw-rw-rw-   0        0        0       60 2022-08-12 11:20:32.000000 tuack-0.1.5/tuack/sample/precautions/zh-cn.md
--rw-rw-rw-   0        0        0      342 2018-03-03 08:40:20.000000 tuack-0.1.5/tuack/sample/problem.gitattributes
--rw-rw-rw-   0        0        0      254 2023-01-09 01:26:59.000000 tuack-0.1.5/tuack/sample/problem.gitignore
--rw-rw-rw-   0        0        0      466 2023-01-09 01:26:59.000000 tuack-0.1.5/tuack/sample/problem.json
--rw-rw-rw-   0        0        0       76 2018-03-03 08:40:20.000000 tuack-0.1.5/tuack/sample/uoj.json
-drwxrwxrwx   0        0        0        0 2023-05-13 04:22:14.835087 tuack-0.1.5/tuack/sample-empty/
-drwxrwxrwx   0        0        0        0 2023-05-13 04:22:15.164705 tuack-0.1.5/tuack/sample-empty/statement/
--rw-rw-rw-   0        0        0      411 2023-01-09 01:26:59.000000 tuack-0.1.5/tuack/sample-empty/statement/zh-cn.md
-drwxrwxrwx   0        0        0        0 2023-05-13 04:22:14.836609 tuack-0.1.5/tuack/sample-problem/
-drwxrwxrwx   0        0        0        0 2023-05-13 04:22:15.175668 tuack-0.1.5/tuack/sample-problem/data/
--rw-rw-rw-   0        0        0       44 2023-01-09 01:26:59.000000 tuack-0.1.5/tuack/sample-problem/data/1.ans
--rw-rw-rw-   0        0        0       43 2023-01-09 01:26:59.000000 tuack-0.1.5/tuack/sample-problem/data/1.in
-drwxrwxrwx   0        0        0        0 2023-05-13 04:22:15.184637 tuack-0.1.5/tuack/sample-problem/down/
--rw-rw-rw-   0        0        0       79 2023-01-09 01:26:59.000000 tuack-0.1.5/tuack/sample-problem/down/1.ans
--rw-rw-rw-   0        0        0       77 2023-01-09 01:26:59.000000 tuack-0.1.5/tuack/sample-problem/down/1.in
-drwxrwxrwx   0        0        0        0 2023-05-13 04:22:15.191624 tuack-0.1.5/tuack/sample-problem/pre/
--rw-rw-rw-   0        0        0       80 2023-01-09 01:26:59.000000 tuack-0.1.5/tuack/sample-problem/pre/1.ans
--rw-rw-rw-   0        0        0       78 2023-01-09 01:26:59.000000 tuack-0.1.5/tuack/sample-problem/pre/1.in
-drwxrwxrwx   0        0        0        0 2023-05-13 04:22:15.199809 tuack-0.1.5/tuack/sample-problem/resources/
--rw-rw-rw-   0        0        0  3293583 2023-01-09 01:26:59.000000 tuack-0.1.5/tuack/sample-problem/resources/sample.png
-drwxrwxrwx   0        0        0        0 2023-05-13 04:22:15.201798 tuack-0.1.5/tuack/sample-problem/solution/
--rw-rw-rw-   0        0        0     1968 2023-01-09 01:26:59.000000 tuack-0.1.5/tuack/sample-problem/solution/zh-cn.md
-drwxrwxrwx   0        0        0        0 2023-05-13 04:22:15.202785 tuack-0.1.5/tuack/sample-problem/statement/
--rw-rw-rw-   0        0        0     6819 2023-04-24 01:30:55.000000 tuack-0.1.5/tuack/sample-problem/statement/zh-cn.md
-drwxrwxrwx   0        0        0        0 2023-05-13 04:22:15.218786 tuack-0.1.5/tuack/sample-problem/tables/
--rw-rw-rw-   0        0        0     1062 2023-03-28 10:24:11.000000 tuack-0.1.5/tuack/sample-problem/tables/data.pyinc
--rw-rw-rw-   0        0        0     1227 2023-01-09 01:26:59.000000 tuack-0.1.5/tuack/sample-problem/tables/json_data.json
--rw-rw-rw-   0        0        0      205 2023-01-09 01:26:59.000000 tuack-0.1.5/tuack/sample-problem/tables/table.json
-drwxrwxrwx   0        0        0        0 2023-05-13 04:22:15.315086 tuack-0.1.5/tuack/templates/
--rw-rw-rw-   0        0        0      911 2023-01-09 01:26:59.000000 tuack-0.1.5/tuack/templates/ccc.tex.jinja
--rw-rw-rw-   0        0        0    71170 2018-03-03 08:40:20.000000 tuack-0.1.5/tuack/templates/ccpc.png
--rw-rw-rw-   0        0        0     1240 2023-01-09 01:26:59.000000 tuack-0.1.5/tuack/templates/ccpc.tex.jinja
-drwxrwxrwx   0        0        0        0 2023-05-13 04:22:14.836609 tuack-0.1.5/tuack/templates/en/
-drwxrwxrwx   0        0        0        0 2023-05-13 04:22:15.326051 tuack-0.1.5/tuack/templates/en/LC_MESSAGES/
--rw-rw-rw-   0        0        0     2978 2019-01-19 08:45:12.000000 tuack-0.1.5/tuack/templates/en/LC_MESSAGES/lang.mo
--rw-rw-rw-   0        0        0     3681 2019-01-19 08:45:12.000000 tuack-0.1.5/tuack/templates/en/LC_MESSAGES/lang.po
--rw-rw-rw-   0        0        0       77 2019-01-19 08:45:12.000000 tuack-0.1.5/tuack/templates/font.html.jinja
--rw-rw-rw-   0        0        0       70 2019-01-19 08:45:12.000000 tuack-0.1.5/tuack/templates/font.tex.jinja
--rw-rw-rw-   0        0        0      670 2023-01-09 01:26:59.000000 tuack-0.1.5/tuack/templates/hand.tex.jinja
--rw-rw-rw-   0        0        0      144 2023-01-09 01:26:59.000000 tuack-0.1.5/tuack/templates/image.html.jinja
--rw-rw-rw-   0        0        0      530 2023-01-09 01:26:59.000000 tuack-0.1.5/tuack/templates/image.tex.jinja
--rw-rw-rw-   0        0        0     5116 2023-04-24 08:07:57.000000 tuack-0.1.5/tuack/templates/problem_base.md.jinja
--rw-rw-rw-   0        0        0     1051 2019-01-19 08:45:12.000000 tuack-0.1.5/tuack/templates/table.html.jinja
--rw-rw-rw-   0        0        0      402 2023-01-09 01:26:59.000000 tuack-0.1.5/tuack/templates/table.md.jinja
--rw-rw-rw-   0        0        0     2295 2018-03-03 08:40:20.000000 tuack-0.1.5/tuack/templates/table.tex.jinja
--rw-rw-rw-   0        0        0     2125 2023-01-09 01:26:59.000000 tuack-0.1.5/tuack/templates/template_base.tex.jinja
--rw-rw-rw-   0        0        0      182 2019-01-19 08:45:12.000000 tuack-0.1.5/tuack/templates/template_base.tex.jinja.tex
--rw-rw-rw-   0        0        0     4756 2023-01-09 01:26:59.000000 tuack-0.1.5/tuack/templates/tuack.cls
--rw-rw-rw-   0        0        0     8743 2023-01-09 01:26:59.000000 tuack-0.1.5/tuack/templates/tuoi.tex.jinja
--rw-rw-rw-   0        0        0     1443 2023-01-09 01:26:59.000000 tuack-0.1.5/tuack/templates/tupc.tex.jinja
-drwxrwxrwx   0        0        0        0 2023-05-13 04:22:14.836609 tuack-0.1.5/tuack/templates/zh-cn/
-drwxrwxrwx   0        0        0        0 2023-05-13 04:22:15.335022 tuack-0.1.5/tuack/templates/zh-cn/LC_MESSAGES/
--rw-rw-rw-   0        0        0     3139 2023-01-09 01:26:59.000000 tuack-0.1.5/tuack/templates/zh-cn/LC_MESSAGES/lang.mo
--rw-rw-rw-   0        0        0     3543 2023-01-09 01:26:59.000000 tuack-0.1.5/tuack/templates/zh-cn/LC_MESSAGES/lang.po
--rw-rw-rw-   0        0        0    17692 2023-01-09 01:27:42.000000 tuack-0.1.5/tuack/test.py
--rw-rw-rw-   0        0        0     3777 2023-02-22 09:36:20.000000 tuack-0.1.5/tuack/tools.py
-drwxrwxrwx   0        0        0        0 2023-05-13 04:22:14.895797 tuack-0.1.5/tuack.egg-info/
--rw-rw-rw-   0        0        0      518 2023-05-13 04:22:14.000000 tuack-0.1.5/tuack.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2261 2023-05-13 04:22:14.000000 tuack-0.1.5/tuack.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-13 04:22:14.000000 tuack-0.1.5/tuack.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       77 2023-05-13 04:22:14.000000 tuack-0.1.5/tuack.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-13 04:22:14.000000 tuack-0.1.5/tuack.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-16 13:21:22.256579 tuack-0.1.5.1/
+-rw-rw-rw-   0        0        0    35055 2019-01-19 08:45:12.000000 tuack-0.1.5.1/LICENSE
+-rw-rw-rw-   0        0        0       17 2018-03-03 08:40:20.000000 tuack-0.1.5.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      520 2023-05-16 13:21:22.256579 tuack-0.1.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1717 2023-01-09 01:26:59.000000 tuack-0.1.5.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-16 13:21:22.257586 tuack-0.1.5.1/setup.cfg
+-rw-rw-rw-   0        0        0     1928 2023-05-16 13:21:02.000000 tuack-0.1.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 13:21:22.176746 tuack-0.1.5.1/tuack/
+-rw-rw-rw-   0        0        0      116 2018-03-03 08:40:20.000000 tuack-0.1.5.1/tuack/__init__.py
+-rw-rw-rw-   0        0        0    34497 2023-05-16 13:16:53.000000 tuack-0.1.5.1/tuack/base.py
+-rw-rw-rw-   0        0        0    13348 2023-01-09 01:26:59.000000 tuack-0.1.5.1/tuack/doc.py
+-rw-rw-rw-   0        0        0    27596 2023-05-13 08:34:57.000000 tuack-0.1.5.1/tuack/dump.py
+-rw-rw-rw-   0        0        0    14486 2023-01-09 01:26:59.000000 tuack-0.1.5.1/tuack/gen.py
+-rw-rw-rw-   0        0        0     2334 2023-01-09 01:26:59.000000 tuack-0.1.5.1/tuack/install.py
+drwxrwxrwx   0        0        0        0 2023-05-16 13:21:22.210316 tuack-0.1.5.1/tuack/lex/
+-rw-rw-rw-   0        0        0        0 2018-09-07 13:38:42.000000 tuack-0.1.5.1/tuack/lex/compile.log
+-rw-rw-rw-   0        0        0      971 2019-01-19 08:45:12.000000 tuack-0.1.5.1/tuack/lex/compile.pyinc
+-rw-rw-rw-   0        0        0  2295192 2019-01-19 08:45:12.000000 tuack-0.1.5.1/tuack/lex/format-linux
+-rw-rw-rw-   0        0        0    61896 2019-01-19 08:45:12.000000 tuack-0.1.5.1/tuack/lex/format-mac
+-rwxrwxrwx   0        0        0  2178321 2019-01-19 08:45:12.000000 tuack-0.1.5.1/tuack/lex/format-win.exe
+-rw-rw-rw-   0        0        0      320 2018-08-27 16:45:44.000000 tuack-0.1.5.1/tuack/lex/hehe.log
+-rw-rw-rw-   0        0        0    11191 2019-01-19 08:45:12.000000 tuack-0.1.5.1/tuack/lex/lex.l
+-rw-rw-rw-   0        0        0    94066 2018-09-07 13:38:44.000000 tuack-0.1.5.1/tuack/lex/lex.yy.c
+-rw-rw-rw-   0        0        0    36942 2018-06-11 12:35:42.000000 tuack-0.1.5.1/tuack/lex/lex.yy.o
+-rw-rw-rw-   0        0        0      185 2019-01-19 08:45:12.000000 tuack-0.1.5.1/tuack/lex/main.h
+-rw-rw-rw-   0        0        0    42594 2018-09-07 13:38:44.000000 tuack-0.1.5.1/tuack/lex/yacc.tab.c
+-rw-rw-rw-   0        0        0     1906 2018-09-07 13:38:44.000000 tuack-0.1.5.1/tuack/lex/yacc.tab.h
+-rw-rw-rw-   0        0        0     9007 2018-06-11 12:35:42.000000 tuack-0.1.5.1/tuack/lex/yacc.tab.o
+-rw-rw-rw-   0        0        0      388 2019-01-19 08:45:12.000000 tuack-0.1.5.1/tuack/lex/yacc.y
+-rw-rw-rw-   0        0        0    12225 2023-01-09 01:26:59.000000 tuack-0.1.5.1/tuack/load.py
+-rw-rw-rw-   0        0        0     3605 2019-01-19 08:45:12.000000 tuack-0.1.5.1/tuack/num2chinese.py
+-rw-rw-rw-   0        0        0    12659 2023-05-16 13:14:46.000000 tuack-0.1.5.1/tuack/packer.py
+-rw-rw-rw-   0        0        0    24468 2023-05-13 04:24:01.000000 tuack-0.1.5.1/tuack/ren.py
+drwxrwxrwx   0        0        0        0 2023-05-16 13:21:22.220544 tuack-0.1.5.1/tuack/sample/
+-rw-rw-rw-   0        0        0     7909 2023-01-09 01:26:59.000000 tuack-0.1.5.1/tuack/sample/arbiter_e.noi_linux1.sample
+-rw-rw-rw-   0        0        0    23576 2023-01-09 01:26:59.000000 tuack-0.1.5.1/tuack/sample/arbiter_e.sample
+-rw-rw-rw-   0        0        0     5586 2023-01-09 01:26:59.000000 tuack-0.1.5.1/tuack/sample/chk.cpp
+-rw-rw-rw-   0        0        0      195 2023-01-09 01:26:59.000000 tuack-0.1.5.1/tuack/sample/contest.gitignore
+-rw-rw-rw-   0        0        0      266 2023-01-09 01:26:59.000000 tuack-0.1.5.1/tuack/sample/contest.json
+-rw-rw-rw-   0        0        0      186 2023-01-09 01:26:59.000000 tuack-0.1.5.1/tuack/sample/day.gitignore
+-rw-rw-rw-   0        0        0      207 2023-01-09 01:26:59.000000 tuack-0.1.5.1/tuack/sample/day.json
+-rw-rw-rw-   0        0        0      351 2023-01-09 01:26:59.000000 tuack-0.1.5.1/tuack/sample/empty.gitattributes
+-rw-rw-rw-   0        0        0      254 2023-01-09 01:26:59.000000 tuack-0.1.5.1/tuack/sample/empty.gitignore
+-rw-rw-rw-   0        0        0      435 2023-01-09 01:26:59.000000 tuack-0.1.5.1/tuack/sample/empty.json
+drwxrwxrwx   0        0        0        0 2023-05-16 13:21:22.234636 tuack-0.1.5.1/tuack/sample/precautions/
+-rw-rw-rw-   0        0        0       60 2022-08-12 11:20:32.000000 tuack-0.1.5.1/tuack/sample/precautions/zh-cn.md
+-rw-rw-rw-   0        0        0      342 2018-03-03 08:40:20.000000 tuack-0.1.5.1/tuack/sample/problem.gitattributes
+-rw-rw-rw-   0        0        0      254 2023-01-09 01:26:59.000000 tuack-0.1.5.1/tuack/sample/problem.gitignore
+-rw-rw-rw-   0        0        0      466 2023-01-09 01:26:59.000000 tuack-0.1.5.1/tuack/sample/problem.json
+-rw-rw-rw-   0        0        0       76 2018-03-03 08:40:20.000000 tuack-0.1.5.1/tuack/sample/uoj.json
+drwxrwxrwx   0        0        0        0 2023-05-16 13:21:22.152628 tuack-0.1.5.1/tuack/sample-empty/
+drwxrwxrwx   0        0        0        0 2023-05-16 13:21:22.222273 tuack-0.1.5.1/tuack/sample-empty/statement/
+-rw-rw-rw-   0        0        0      411 2023-01-09 01:26:59.000000 tuack-0.1.5.1/tuack/sample-empty/statement/zh-cn.md
+drwxrwxrwx   0        0        0        0 2023-05-16 13:21:22.160667 tuack-0.1.5.1/tuack/sample-problem/
+drwxrwxrwx   0        0        0        0 2023-05-16 13:21:22.223275 tuack-0.1.5.1/tuack/sample-problem/data/
+-rw-rw-rw-   0        0        0       44 2023-01-09 01:26:59.000000 tuack-0.1.5.1/tuack/sample-problem/data/1.ans
+-rw-rw-rw-   0        0        0       43 2023-01-09 01:26:59.000000 tuack-0.1.5.1/tuack/sample-problem/data/1.in
+drwxrwxrwx   0        0        0        0 2023-05-16 13:21:22.224930 tuack-0.1.5.1/tuack/sample-problem/down/
+-rw-rw-rw-   0        0        0       79 2023-01-09 01:26:59.000000 tuack-0.1.5.1/tuack/sample-problem/down/1.ans
+-rw-rw-rw-   0        0        0       77 2023-01-09 01:26:59.000000 tuack-0.1.5.1/tuack/sample-problem/down/1.in
+drwxrwxrwx   0        0        0        0 2023-05-16 13:21:22.225943 tuack-0.1.5.1/tuack/sample-problem/pre/
+-rw-rw-rw-   0        0        0       80 2023-01-09 01:26:59.000000 tuack-0.1.5.1/tuack/sample-problem/pre/1.ans
+-rw-rw-rw-   0        0        0       78 2023-01-09 01:26:59.000000 tuack-0.1.5.1/tuack/sample-problem/pre/1.in
+drwxrwxrwx   0        0        0        0 2023-05-16 13:21:22.226955 tuack-0.1.5.1/tuack/sample-problem/resources/
+-rw-rw-rw-   0        0        0  3293583 2023-01-09 01:26:59.000000 tuack-0.1.5.1/tuack/sample-problem/resources/sample.png
+drwxrwxrwx   0        0        0        0 2023-05-16 13:21:22.229927 tuack-0.1.5.1/tuack/sample-problem/solution/
+-rw-rw-rw-   0        0        0     1968 2023-01-09 01:26:59.000000 tuack-0.1.5.1/tuack/sample-problem/solution/zh-cn.md
+drwxrwxrwx   0        0        0        0 2023-05-16 13:21:22.229927 tuack-0.1.5.1/tuack/sample-problem/statement/
+-rw-rw-rw-   0        0        0     6819 2023-05-13 04:24:01.000000 tuack-0.1.5.1/tuack/sample-problem/statement/zh-cn.md
+drwxrwxrwx   0        0        0        0 2023-05-16 13:21:22.233563 tuack-0.1.5.1/tuack/sample-problem/tables/
+-rw-rw-rw-   0        0        0     1062 2023-03-28 10:24:11.000000 tuack-0.1.5.1/tuack/sample-problem/tables/data.pyinc
+-rw-rw-rw-   0        0        0     1227 2023-01-09 01:26:59.000000 tuack-0.1.5.1/tuack/sample-problem/tables/json_data.json
+-rw-rw-rw-   0        0        0      205 2023-01-09 01:26:59.000000 tuack-0.1.5.1/tuack/sample-problem/tables/table.json
+drwxrwxrwx   0        0        0        0 2023-05-16 13:21:22.253127 tuack-0.1.5.1/tuack/templates/
+-rw-rw-rw-   0        0        0      911 2023-01-09 01:26:59.000000 tuack-0.1.5.1/tuack/templates/ccc.tex.jinja
+-rw-rw-rw-   0        0        0    71170 2018-03-03 08:40:20.000000 tuack-0.1.5.1/tuack/templates/ccpc.png
+-rw-rw-rw-   0        0        0     1240 2023-01-09 01:26:59.000000 tuack-0.1.5.1/tuack/templates/ccpc.tex.jinja
+drwxrwxrwx   0        0        0        0 2023-05-16 13:21:22.162049 tuack-0.1.5.1/tuack/templates/en/
+drwxrwxrwx   0        0        0        0 2023-05-16 13:21:22.254124 tuack-0.1.5.1/tuack/templates/en/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     2978 2019-01-19 08:45:12.000000 tuack-0.1.5.1/tuack/templates/en/LC_MESSAGES/lang.mo
+-rw-rw-rw-   0        0        0     3681 2019-01-19 08:45:12.000000 tuack-0.1.5.1/tuack/templates/en/LC_MESSAGES/lang.po
+-rw-rw-rw-   0        0        0       77 2019-01-19 08:45:12.000000 tuack-0.1.5.1/tuack/templates/font.html.jinja
+-rw-rw-rw-   0        0        0       70 2019-01-19 08:45:12.000000 tuack-0.1.5.1/tuack/templates/font.tex.jinja
+-rw-rw-rw-   0        0        0      670 2023-01-09 01:26:59.000000 tuack-0.1.5.1/tuack/templates/hand.tex.jinja
+-rw-rw-rw-   0        0        0      144 2023-01-09 01:26:59.000000 tuack-0.1.5.1/tuack/templates/image.html.jinja
+-rw-rw-rw-   0        0        0      530 2023-01-09 01:26:59.000000 tuack-0.1.5.1/tuack/templates/image.tex.jinja
+-rw-rw-rw-   0        0        0     5116 2023-05-13 04:24:01.000000 tuack-0.1.5.1/tuack/templates/problem_base.md.jinja
+-rw-rw-rw-   0        0        0     1051 2019-01-19 08:45:12.000000 tuack-0.1.5.1/tuack/templates/table.html.jinja
+-rw-rw-rw-   0        0        0      402 2023-01-09 01:26:59.000000 tuack-0.1.5.1/tuack/templates/table.md.jinja
+-rw-rw-rw-   0        0        0     2295 2018-03-03 08:40:20.000000 tuack-0.1.5.1/tuack/templates/table.tex.jinja
+-rw-rw-rw-   0        0        0     2125 2023-01-09 01:26:59.000000 tuack-0.1.5.1/tuack/templates/template_base.tex.jinja
+-rw-rw-rw-   0        0        0      182 2019-01-19 08:45:12.000000 tuack-0.1.5.1/tuack/templates/template_base.tex.jinja.tex
+-rw-rw-rw-   0        0        0     4756 2023-01-09 01:26:59.000000 tuack-0.1.5.1/tuack/templates/tuack.cls
+-rw-rw-rw-   0        0        0     8743 2023-01-09 01:26:59.000000 tuack-0.1.5.1/tuack/templates/tuoi.tex.jinja
+-rw-rw-rw-   0        0        0     1443 2023-01-09 01:26:59.000000 tuack-0.1.5.1/tuack/templates/tupc.tex.jinja
+drwxrwxrwx   0        0        0        0 2023-05-16 13:21:22.162312 tuack-0.1.5.1/tuack/templates/zh-cn/
+drwxrwxrwx   0        0        0        0 2023-05-16 13:21:22.255580 tuack-0.1.5.1/tuack/templates/zh-cn/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     3139 2023-01-09 01:26:59.000000 tuack-0.1.5.1/tuack/templates/zh-cn/LC_MESSAGES/lang.mo
+-rw-rw-rw-   0        0        0     3543 2023-01-09 01:26:59.000000 tuack-0.1.5.1/tuack/templates/zh-cn/LC_MESSAGES/lang.po
+-rw-rw-rw-   0        0        0    17692 2023-01-09 01:27:42.000000 tuack-0.1.5.1/tuack/test.py
+-rw-rw-rw-   0        0        0     3777 2023-02-22 09:36:20.000000 tuack-0.1.5.1/tuack/tools.py
+drwxrwxrwx   0        0        0        0 2023-05-16 13:21:22.192980 tuack-0.1.5.1/tuack.egg-info/
+-rw-rw-rw-   0        0        0      520 2023-05-16 13:21:21.000000 tuack-0.1.5.1/tuack.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2261 2023-05-16 13:21:22.000000 tuack-0.1.5.1/tuack.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 13:21:21.000000 tuack-0.1.5.1/tuack.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       77 2023-05-16 13:21:21.000000 tuack-0.1.5.1/tuack.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-16 13:21:21.000000 tuack-0.1.5.1/tuack.egg-info/top_level.txt
```

### Comparing `tuack-0.1.5/LICENSE` & `tuack-0.1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5/PKG-INFO` & `tuack-0.1.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tuack
-Version: 0.1.5
+Version: 0.1.5.1
 Summary: Tools for generating an Tsinghua/OI/ICPC-styled problem or contest for multiple judges.
 Home-page: 
 Author: Chenxu Min, Zhang Ruizhe, Liu Xiaoyi, Chen Junkun, Chen Shengqi, Luo Lingxiao, Cheng Yuxuan
 Author-email: chen.xm.mu@gmail.com, 657228726@qq.com, circuitcoder0@gmail.com, 1261954105@qq.com, i@harrychen.xyz, 0.0@pku.edu.cn
 License: https://git.thusaac.com/publish/tuack/blob/master/LICENSE
 Platform: UNKNOWN
 License-File: LICENSE
```

### Comparing `tuack-0.1.5/README.md` & `tuack-0.1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5/setup.py` & `tuack-0.1.5.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 	'pyyaml >= 5.1',
 	'rarfile >= 3.0',
 	'requests_toolbelt >= 0.9.1'
 ]
 
 setup(
 	name = 'tuack',
-	version = '0.1.5',
+	version = '0.1.5.1',
 	packages = find_packages(),
 	author = 'Chenxu Min, Zhang Ruizhe, Liu Xiaoyi, Chen Junkun, Chen Shengqi, Luo Lingxiao, Cheng Yuxuan',
 	author_email = 'chen.xm.mu@gmail.com, 657228726@qq.com, circuitcoder0@gmail.com, 1261954105@qq.com, i@harrychen.xyz, 0.0@pku.edu.cn',
 	url = '',
 	license = 'https://git.thusaac.com/publish/tuack/blob/master/LICENSE',
 	description = 'Tools for generating an Tsinghua/OI/ICPC-styled problem or contest for multiple judges.',
 	cmdclass={
```

### Comparing `tuack-0.1.5/tuack/base.py` & `tuack-0.1.5.1/tuack/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -807,157 +807,165 @@
 		tool_conf = {}
 	sys_env = get_sys_env()
 	if sys_env not in tool_conf:
 		tool_conf[sys_env] = {}
 	env_conf = tool_conf[sys_env]
 	return tool_conf
 
+class NoInstalledException(Exception):
+	def __init__(self, value):
+		self.value = value
+	def __str__(self):
+		return repr(self.value)
+
 def check_install(pack):
 	def check_import(pack, extra_info = '', pack_name = None, level = logging.ERROR):
 		try:
 			__import__(pack)
 		except Exception as e:
 			log.log(level, u'python包%s没有安装，使用 pip install %s 安装。%s' % (pack, pack_name if pack_name else pack, extra_info))
 			if system == 'Windows':
 				log.info(u'如果pip没有安装，Windows下推荐用Anaconda等集成环境。')
 			if system == 'Linux':
 				log.info(u'如果pip没有安装，Ubuntu下用 sudo apt install python-pip 安装。')
-			raise e
+			raise NoInstalledException(str(e))
 	check_pyside = lambda : check_import('PySide', u'注意这个包只能在 python2 下使用。', 'pyside')
 	check_natsort = lambda : check_import('natsort', level = logging.WARNING)
 	def check_pandoc():
 		ret = os.system('pandoc -v')
 		if ret != 0:
 			log.error(u'格式转换工具pandoc没有安装。')
 			if system == 'Windows':
 				log.info(u'Windows用户去官方网站下载安装，安装好后把pandoc.exe所在路径添加到环境变量PATH中。')
 			if system == 'Linux':
 				log.info(u'Ubuntu下用 sudo apt install pandoc 安装。')
-			raise Exception('pandoc not found')
+			raise NoInstalledException('pandoc not found')
 	def check_xelatex():
 		ret = os.system('xelatex --version')
 		if ret != 0:
 			log.error(u'TeX渲染工具XeLaTeX没有安装。')
 			if system == 'Windows':
 				log.info(u'Windows下可以先安装MiKTeX，在首次运行的时候会再提示安装后续文件。')
 			if system == 'Linux':
 				log.info(u'Ubuntu下先用 sudo apt install texlive-xetex texlive-fonts-recommended texlive-latex-extra 安装工具；')
 				log.info(u'然后一般会因为缺少有些字体而报错（Windows有使用权，但Ubuntu没有，所以没有预装这些字体）。')
 				log.info(u'可以使用下列页面上的方法安装缺少的字体或是把win下的字体复制过来。')
 				log.info(u'http://linux-wiki.cn/wiki/zh-hans/LaTeX%E4%B8%AD%E6%96%87%E6%8E%92%E7%89%88%EF%BC%88%E4%BD%BF%E7%94%A8XeTeX%EF%BC%89')
-			raise Exception('xelatex not found')
+			raise NoInstalledException('xelatex not found')
 	def check_git():
 		ret = os.system('git --version')
 		if ret != 0:
 			log.warning(u'版本管理工具git没有安装，如果工程用git维护则你的修改可能无法成功提交。')
 			log.info(u'一个可能的安装教程见这里：')
 			log.info(u'https://git-scm.com/book/zh/v2/%E8%B5%B7%E6%AD%A5-%E5%AE%89%E8%A3%85-Git')
 			if system == 'Windows':
 				log.info(u'Windows下有多种不同的git版本，大家可以多交流好用的版本。')
 			log.info(u'git入门可以参看这里：')
 			log.info(u'http://rogerdudler.github.io/git-guide/index.zh.html')
 			log.info(u'一般推荐用ssh方式克隆仓库，并用公私钥保证安全，添加密钥的方式一般仓库的git网页上能找到。')
-			raise Exception('git not found')
+			raise NoInstalledException('git not found')
 	def check_git_lfs():
 		ret = os.system('git lfs')
 		if ret != 0:
 			log.warning(u'git大文件系统lfs没有安装，如果工程使用了它你可能无法同步。')
 			log.info(u'因为有些评测数据比较大，所以一般要求用git lfs大文件系统（Large File System）管理评测数据（in/ans）')
 			log.info(u'一个可能的安装教程见这里：')
 			log.info(u'https://git-lfs.github.com/')
 			log.info(u'如果你用本工具的generator生成题目工程，那么你装好lfs以后一般可以不用再手工指定in和ans文件用lfs管理。')
 			log.info(u'如果你的多人合作工程用到了lfs，请务必不要在没有安装lfs前把数据添加到工程中！')
-			raise Exception('git lfs not found')
+			raise NoInstalledException('git lfs not found')
 
 	def check_gpp():
 		ret = os.system('g++ -v')
 		if ret != 0:
 			log.warning(u'g++未安装，将可能无法测试C++代码。')
-			raise Exception('g++ not found')
+			raise NoInstalledException('g++ not found')
 	
 	def check_gcc():
 		ret = os.system('gcc -v')
 		if ret != 0:
 			log.warning(u'gcc未安装，将可能无法测试C代码。')
-			raise Exception('gcc not found')
+			raise NoInstalledException('gcc not found')
 			
 	def check_java():
 		ret = os.system('javac -version')
 		if ret != 0:
 			log.warning(u'javac未安装，将可能无法测试Java代码。')
-			raise Exception('javac not found')
+			raise NoInstalledException('javac not found')
 		ret = os.system('java -version')
 		if ret != 0:
 			log.warning(u'java未安装，将可能无法测试Java代码。')
-			raise Exception('java not found')
+			raise NoInstalledException('java not found')
 
 	def check_py2():
 		ret = os.system('python2 --version')
 		if ret != 0:
 			log.warning(u'python2未安装，将可能无法测试Python2代码。')
-			raise Exception('python2 not found')
+			raise NoInstalledException('python2 not found')
 
 	def check_py3():
 		ret = os.system('python3 --version')
 		if ret != 0:
 			log.warning(u'python3未安装，将可能无法测试Python3代码。')
-			raise Exception('python3 not found')
+			raise NoInstalledException('python3 not found')
 
 	def check_py():
 		ret = os.system('python --version')
 		if ret != 0:
 			log.warning(u'python未安装，将可能无法测试Python代码。')
-			raise Exception('python not found')
+			raise NoInstalledException('python not found')
 			
 	def check_flex():
 		ret = os.system('flex --version')
 		if ret != 0:
 			log.warning(u'flex未安装，将可能无法检查题面格式。')
-			raise Exception('flex not found')
+			raise NoInstalledException('flex not found')
 
 	def check_bison():
 		ret = os.system('bison --version')
 		if ret != 0:
 			log.warning(u'bison未安装，将可能无法检查题面格式。')
-			raise Exception('bison not found')
+			raise NoInstalledException('bison not found')
 			
 	def check_format():
 		ret = os.system('"%s" -v' % pjoin(tool_path, format_checker_name))
 		if ret != 0:
 			log.warning(u'format checker未安装，使用`python -m tuack.install format`安装。')
-			raise Exception('format not found')
+			raise NoInstalledException('format not found')
 			
 	def check_unrar():
 		ret = os.system('unrar --version')
 		if ret != 0:
 			log.warning(u'unrar未安装，将无法解压rar文件，请安装unrar。')
 			log.warning(u'对于Windows用户，你可以将WinRar的安装目录添加到PATH。')
-			raise Exception('unrar not found')
+			raise NoInstalledException('unrar not found')
 
 	def check_time():
 		ret = os.system('time ls')
 		if ret != 0:
 			log.warning(u'time未安装，将无法测试运行时间。')
 			log.warning(u'类Ubuntu用户可以用apt install time安装。')
-			raise Exception('time not found')
+			raise NoInstalledException('time not found')
 
 	if pack in {'g++', 'cpp'}:
 		pack = 'gpp'
 	if pack == 'c':
 		pack = 'gcc'
 	global tool_conf
 	tool_conf = get_tool_conf()
 	if 'installed' not in env_conf:
 		env_conf['installed'] = {}
 	if pack in env_conf['installed'] and env_conf['installed'][pack]:
 		return True
-	if isfunction('check_' + pack):
-		eval('check_' + pack)()
-	else:
+	try:
+		eval('check_' + pack)
+	except:
 		check_import(pack)
+	else:
+		eval('check_' + pack)()
 	env_conf['installed'][pack] = True
 
 	open(pjoin(tool_path, 'conf.json'), 'wb').write(json.dumps(tool_conf, indent = 2, sort_keys = True).encode('utf-8'))
 	return True
 
 def change_eol(path, eol, show_path = None):
 	import uuid
```

### Comparing `tuack-0.1.5/tuack/doc.py` & `tuack-0.1.5.1/tuack/doc.py`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5/tuack/dump.py` & `tuack-0.1.5.1/tuack/dump.py`

 * *Files 4% similar despite different names*

```diff
@@ -153,55 +153,63 @@
 							base.pjoin(prob['name'], str(c) + '.in')
 						],
 						"outputFiles": [
 							base.pjoin(prob['name'], str(c) + '.ans')
 						]
 					} for c in prob.test_cases
 				]
-			tasks.append({
+			task = {
 				'answerFileExtension' : 'out',
-				"comparisonMode": 1,	#TODO: What if there is spj (code = 4)
+				"comparisonMode": 1,
 				"diffArguments": "--ignore-space-change --text --brief",
 				"inputFileName": prob['name'] + '.in',
 				"outputFileName": prob['name'] + '.out',
 				"problemTitle": base.tr(prob['title']),
 				"realPrecision": 3,		#float number error bound
 				"sourceFileName": prob['name'],
-				"specialJudge": "",		#TODO: What if there is spj
+				"specialJudge": "",
 				"standardInputCheck": False,
 				"standardOutputCheck": False,
 				"subFolderCheck": False,
 				"taskType": 1 if prob['type'] == 'output' else 0,
 				"compilerConfiguration": {
 					{
 						'cpp' : 'g++',
 						'c' : 'gcc',
 						'pas' : 'fpc',
 						'py' : 'python',
 						'java' : 'javac'
 					}[i] : 'default' for i in prob.get('compile', {}) if i in {'cpp', 'c', 'pas', 'py', 'java'}
 				},
 				"testCases" : cases
-			})
+			}
 			sp = list(prob.route.split('/'))
 			target = ['lemon'] + sp[:-1] + ['data', sp[-1]]
 			shutil.copytree(base.pjoin(prob.path, 'data'), base.pjoin(*target))
+			if os.path.isdir(base.pjoin(prob.path, 'data', 'chk')) and os.path.isfile(base.pjoin(prob.path, 'data', 'chk', 'chk.cpp')):
+				log.info('发现chk，尝试编译。')
+				os.system("g++ %s -o %s -O2 -std=c++17" % (
+					base.pjoin(prob.path, 'data', 'chk', 'chk.cpp'),
+					base.pjoin(*(target + ['chk.exe']))
+				))
+				task['comparisonMode'] = 4
+				task['specialJudge'] = base.pjoin(prob['name'], 'chk.exe')
+			tasks.append(task)
 		open(base.pjoin('lemon', conf.route, conf['name'] + '.cdf'), 'wb').write(json.dumps({
 			"contestTitle" : conf['name'],
 			"contestants" : [],
 			"tasks" : tasks
 		}).encode('utf-8'))
 	
 	base.run_r(base.unix2dos, base.pjoin('lemon', conf.route, 'data'))
 	
 	if base.do_zip:
 		import zipfile
 		with zipfile.ZipFile(base.pjoin('lemon', conf.route) + '.zip', 'w') as z:
 			base.run_r(lambda path : z.write(path), base.pjoin('lemon', conf.route))
-	log.warning(u'目前SPJ的支持暂时还没有实现，有需要请手工配置。')
 	log.warning(u'目前lemon的编译选项是写在注册表里的，暂时没有实现该功能，请手工配置。')
 
 def arbiter_main(conf = None,daynum = 0):
 	def arbiter_info(info, filename):
 		with open(filename,'wb') as ofile:
 			for key, val in info.items():
 				ofile.write(('%s%s\n' % (key, val)).encode('utf-8'))
```

### Comparing `tuack-0.1.5/tuack/gen.py` & `tuack-0.1.5.1/tuack/gen.py`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5/tuack/install.py` & `tuack-0.1.5.1/tuack/install.py`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5/tuack/lex/compile.pyinc` & `tuack-0.1.5.1/tuack/lex/compile.pyinc`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5/tuack/lex/format-linux` & `tuack-0.1.5.1/tuack/lex/format-linux`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5/tuack/lex/format-mac` & `tuack-0.1.5.1/tuack/lex/format-mac`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5/tuack/lex/format-win.exe` & `tuack-0.1.5.1/tuack/lex/format-win.exe`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5/tuack/lex/lex.l` & `tuack-0.1.5.1/tuack/lex/lex.l`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5/tuack/lex/lex.yy.c` & `tuack-0.1.5.1/tuack/lex/lex.yy.c`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5/tuack/lex/lex.yy.o` & `tuack-0.1.5.1/tuack/lex/lex.yy.o`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5/tuack/lex/yacc.tab.c` & `tuack-0.1.5.1/tuack/lex/yacc.tab.c`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5/tuack/lex/yacc.tab.h` & `tuack-0.1.5.1/tuack/lex/yacc.tab.h`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5/tuack/lex/yacc.tab.o` & `tuack-0.1.5.1/tuack/lex/yacc.tab.o`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5/tuack/load.py` & `tuack-0.1.5.1/tuack/load.py`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5/tuack/num2chinese.py` & `tuack-0.1.5.1/tuack/num2chinese.py`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5/tuack/packer.py` & `tuack-0.1.5.1/tuack/packer.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,16 @@
 	return None
 
 def test_copy_problem_files(prob):
 	data_path = os.path.join(prob.path, 'data')
 	try:
 		copy(data_path, 'chk', base.pjoin(output_folder, prob.route))
 		prob.chk = True
+	except base.NoInstalledException as e:
+		raise(e)
 	except Exception as e:
 		prob.chk = False
 	
 def copy_one_day_files(probs, day_name):
 	remkdir(os.path.join(output_folder, day_name, 'data'))
 	print('copy data files')
 	for prob in probs:
```

### Comparing `tuack-0.1.5/tuack/ren.py` & `tuack-0.1.5.1/tuack/ren.py`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5/tuack/sample/arbiter_e.noi_linux1.sample` & `tuack-0.1.5.1/tuack/sample/arbiter_e.noi_linux1.sample`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5/tuack/sample/arbiter_e.sample` & `tuack-0.1.5.1/tuack/sample/arbiter_e.sample`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5/tuack/sample/chk.cpp` & `tuack-0.1.5.1/tuack/sample/chk.cpp`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5/tuack/sample-problem/resources/sample.png` & `tuack-0.1.5.1/tuack/sample-problem/resources/sample.png`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5/tuack/sample-problem/solution/zh-cn.md` & `tuack-0.1.5.1/tuack/sample-problem/solution/zh-cn.md`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5/tuack/sample-problem/statement/zh-cn.md` & `tuack-0.1.5.1/tuack/sample-problem/statement/zh-cn.md`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5/tuack/sample-problem/tables/data.pyinc` & `tuack-0.1.5.1/tuack/sample-problem/tables/data.pyinc`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5/tuack/sample-problem/tables/json_data.json` & `tuack-0.1.5.1/tuack/sample-problem/tables/json_data.json`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5/tuack/templates/ccc.tex.jinja` & `tuack-0.1.5.1/tuack/templates/ccc.tex.jinja`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5/tuack/templates/ccpc.png` & `tuack-0.1.5.1/tuack/templates/ccpc.png`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5/tuack/templates/ccpc.tex.jinja` & `tuack-0.1.5.1/tuack/templates/ccpc.tex.jinja`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5/tuack/templates/en/LC_MESSAGES/lang.mo` & `tuack-0.1.5.1/tuack/templates/en/LC_MESSAGES/lang.mo`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5/tuack/templates/en/LC_MESSAGES/lang.po` & `tuack-0.1.5.1/tuack/templates/en/LC_MESSAGES/lang.po`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5/tuack/templates/hand.tex.jinja` & `tuack-0.1.5.1/tuack/templates/hand.tex.jinja`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5/tuack/templates/image.tex.jinja` & `tuack-0.1.5.1/tuack/templates/image.tex.jinja`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5/tuack/templates/problem_base.md.jinja` & `tuack-0.1.5.1/tuack/templates/problem_base.md.jinja`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5/tuack/templates/table.html.jinja` & `tuack-0.1.5.1/tuack/templates/table.html.jinja`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5/tuack/templates/table.tex.jinja` & `tuack-0.1.5.1/tuack/templates/table.tex.jinja`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5/tuack/templates/template_base.tex.jinja` & `tuack-0.1.5.1/tuack/templates/template_base.tex.jinja`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5/tuack/templates/tuack.cls` & `tuack-0.1.5.1/tuack/templates/tuack.cls`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5/tuack/templates/tuoi.tex.jinja` & `tuack-0.1.5.1/tuack/templates/tuoi.tex.jinja`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5/tuack/templates/tupc.tex.jinja` & `tuack-0.1.5.1/tuack/templates/tupc.tex.jinja`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5/tuack/templates/zh-cn/LC_MESSAGES/lang.mo` & `tuack-0.1.5.1/tuack/templates/zh-cn/LC_MESSAGES/lang.mo`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5/tuack/templates/zh-cn/LC_MESSAGES/lang.po` & `tuack-0.1.5.1/tuack/templates/zh-cn/LC_MESSAGES/lang.po`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5/tuack/test.py` & `tuack-0.1.5.1/tuack/test.py`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5/tuack/tools.py` & `tuack-0.1.5.1/tuack/tools.py`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5/tuack.egg-info/PKG-INFO` & `tuack-0.1.5.1/tuack.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tuack
-Version: 0.1.5
+Version: 0.1.5.1
 Summary: Tools for generating an Tsinghua/OI/ICPC-styled problem or contest for multiple judges.
 Home-page: 
 Author: Chenxu Min, Zhang Ruizhe, Liu Xiaoyi, Chen Junkun, Chen Shengqi, Luo Lingxiao, Cheng Yuxuan
 Author-email: chen.xm.mu@gmail.com, 657228726@qq.com, circuitcoder0@gmail.com, 1261954105@qq.com, i@harrychen.xyz, 0.0@pku.edu.cn
 License: https://git.thusaac.com/publish/tuack/blob/master/LICENSE
 Platform: UNKNOWN
 License-File: LICENSE
```

### Comparing `tuack-0.1.5/tuack.egg-info/SOURCES.txt` & `tuack-0.1.5.1/tuack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

