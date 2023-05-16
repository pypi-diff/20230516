# Comparing `tmp/featureform-1.8.0.tar.gz` & `tmp/featureform-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "featureform-1.8.0.tar", last modified: Mon May  1 21:15:27 2023, max compression
+gzip compressed data, was "featureform-1.8.1.tar", last modified: Tue May 16 19:41:24 2023, max compression
```

## Comparing `featureform-1.8.0.tar` & `featureform-1.8.1.tar`

### file list

```diff
@@ -1,368 +1,371 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:15:27.333976 featureform-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)    16724 2023-05-01 21:13:34.000000 featureform-1.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-01 21:13:34.000000 featureform-1.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-05-01 21:15:27.333976 featureform-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-05-01 21:13:34.000000 featureform-1.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-01 21:13:34.000000 featureform-1.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-05-01 21:15:27.333976 featureform-1.8.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:15:27.249973 featureform-1.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:15:27.257973 featureform-1.8.0/src/featureform/
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-01 21:13:34.000000 featureform-1.8.0/src/featureform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-01 21:13:34.000000 featureform-1.8.0/src/featureform/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7509 2023-05-01 21:13:34.000000 featureform-1.8.0/src/featureform/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-05-01 21:13:34.000000 featureform-1.8.0/src/featureform/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-01 21:13:34.000000 featureform-1.8.0/src/featureform/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:15:27.249973 featureform-1.8.0/src/featureform/dashboard/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:15:27.261973 featureform-1.8.0/src/featureform/dashboard/out/
--rw-r--r--   0 runner    (1001) docker     (123)    17164 2023-05-01 21:15:20.000000 featureform-1.8.0/src/featureform/dashboard/out/404.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:15:27.261973 featureform-1.8.0/src/featureform/dashboard/out/[type]/
--rw-r--r--   0 runner    (1001) docker     (123)    17956 2023-05-01 21:15:20.000000 featureform-1.8.0/src/featureform/dashboard/out/[type]/[entity].html
--rw-r--r--   0 runner    (1001) docker     (123)    17188 2023-05-01 21:15:20.000000 featureform-1.8.0/src/featureform/dashboard/out/[type].html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:15:27.249973 featureform-1.8.0/src/featureform/dashboard/out/_next/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:15:27.249973 featureform-1.8.0/src/featureform/dashboard/out/_next/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:15:27.261973 featureform-1.8.0/src/featureform/dashboard/out/_next/static/Jopdpwd8wB7tMgkcaVnsn/
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-01 21:13:34.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/Jopdpwd8wB7tMgkcaVnsn/_buildManifest.js
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-01 21:13:34.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/Jopdpwd8wB7tMgkcaVnsn/_ssgManifest.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:15:27.261973 featureform-1.8.0/src/featureform/dashboard/out/_next/static/XLqQwuMDcHNwRKV5unb2J/
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/XLqQwuMDcHNwRKV5unb2J/_buildManifest.js
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/XLqQwuMDcHNwRKV5unb2J/_ssgManifest.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:15:27.313975 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/
--rw-r--r--   0 runner    (1001) docker     (123)    83561 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/72a30a16.5298cad0ba46633d.js
--rw-r--r--   0 runner    (1001) docker     (123)    74481 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/7679.34cabcdac6ff42f5.js
--rw-r--r--   0 runner    (1001) docker     (123)    21739 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/7856.43cc2293f00befb0.js
--rw-r--r--   0 runner    (1001) docker     (123)   201393 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/ad7f724d.b238476ad0e6f6d2.js
--rw-r--r--   0 runner    (1001) docker     (123)   130270 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/framework-3412d1150754b2fb.js
--rw-r--r--   0 runner    (1001) docker     (123)   104027 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/main-2715d0c23f47c019.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:15:27.321975 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/pages/
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/pages/404-baaca4b2f4acc755.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:15:27.321975 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/pages/[type]/
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/pages/[type]/[entity]-b07f3c4463890639.js
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/pages/[type]-751a928da9d524e9.js
--rw-r--r--   0 runner    (1001) docker     (123)  3583019 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/pages/_app-a764893ff9420ec0.js
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/pages/_error-3f70f2d61eb8c6dd.js
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/pages/connections-1d67ba61869dece6.js
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/pages/index-c2ee5b1681e97e4b.js
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/pages/search-175858e61ba25631.js
--rw-r--r--   0 runner    (1001) docker     (123)    91460 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:15:27.321975 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter/
--rw-r--r--   0 runner    (1001) docker     (123)    35679 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter/refractor-core-import.d200df4f5651fe3c.js
--rw-r--r--   0 runner    (1001) docker     (123)     8068 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_abap.cff854fd7e5b1247.js
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_abnf.a1ff159f2ef1711f.js
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_actionscript.efd417c28a28b388.js
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ada.156060425d9edae1.js
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_agda.7c059beeef27c79a.js
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_al.f8ab011377e6cffa.js
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_antlr4.2c3a6fa926d2a251.js
--rw-r--r--   0 runner    (1001) docker     (123)     8341 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_apacheconf.a8e9c6e2469ebb48.js
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_apl.17fe889a8c792ca2.js
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_applescript.ec5486ed51b5bf2a.js
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_aql.efb695712e3f3aa3.js
--rw-r--r--   0 runner    (1001) docker     (123)     8763 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_arduino.681aaa7ec91aa809.js
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_arff.ab502da8667e6dc6.js
--rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_asciidoc.d34ffa4ca9efdc4d.js
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_asm6502.3eb992d6df117427.js
--rw-r--r--   0 runner    (1001) docker     (123)     7829 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_aspnet.0ba8de8f97453373.js
--rw-r--r--   0 runner    (1001) docker     (123)     9289 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_autohotkey.8bd8b23c56f29881.js
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_autoit.f687b627eb6354c6.js
--rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bash.fa5423ba02f0452a.js
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_basic.18dbad942d626219.js
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_batch.8ca1ac5c2d037485.js
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bbcode.4b540b8d0f463220.js
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bison.3be4b74c3d3e0770.js
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bnf.d1d39a9bd6ac45b9.js
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_brainfuck.42d8625dbbdd27ed.js
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_brightscript.5219a23e15549d0f.js
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bro.6a3db5175eef5a7c.js
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_c.fba60a9486edee8d.js
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cil.494c2357f1d5de1e.js
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_clike.065b788c95ab7f0a.js
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_clojure.144f4fa5cb5b7c94.js
--rw-r--r--   0 runner    (1001) docker     (123)    10794 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cmake.63bd8fd3867951a6.js
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_coffeescript.f3407609f464e5a7.js
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_concurnas.807a36085ae57a51.js
--rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cpp.9073ce25850a9aee.js
--rw-r--r--   0 runner    (1001) docker     (123)     5129 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_crystal.500857f6d38420ca.js
--rw-r--r--   0 runner    (1001) docker     (123)     6662 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_csharp.1ab46bae80c6b0ba.js
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_csp.dbb73c45172741db.js
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_css.c6ce776800cc984e.js
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cssExtras.9588a637662140d4.js
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cypher.899ff7f5c7459114.js
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_d.3e486cddc20d2ff9.js
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dart.9db40f270a0b6cb0.js
--rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dax.f58ad34d65866793.js
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dhall.0ca1a915d1865fb5.js
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_diff.e343fa532144b7a2.js
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_django.6ee6c39cb914f163.js
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dnsZoneFile.2a9886e744590498.js
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_docker.fde534872e6578fd.js
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ebnf.35e28e1f6e8a00e4.js
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_editorconfig.17a13e6bcda1e1f3.js
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_eiffel.64ef4de4060b9a23.js
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ejs.4c4ccb70f90dea01.js
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_elixir.a1e48f12166c723b.js
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_elm.6765aa0f50cbaf91.js
--rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_erb.e48ed285a1945936.js
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_erlang.2a114ebcf8dd2d26.js
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_etlua.afcb29f06feae539.js
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_excelFormula.62d0fdeee42f5d64.js
--rw-r--r--   0 runner    (1001) docker     (123)    10203 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_factor.ce84f1b770942d68.js
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_firestoreSecurityRules.209ede8c07b9e60b.js
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_flow.88a9cbf968cf47ec.js
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_fortran.ca33766cb3d9d13c.js
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_fsharp.1aa244fc87692af1.js
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ftl.0457d46374506e78.js
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gcode.ac01f4f7ac16a003.js
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gdscript.afa83bf48d38ded2.js
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gedcom.eae35079f43f4e91.js
--rw-r--r--   0 runner    (1001) docker     (123)     9971 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gherkin.1226aeae8764f3d7.js
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_git.0e0594706d30fbd8.js
--rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_glsl.aaa801f4d5c6da96.js
--rw-r--r--   0 runner    (1001) docker     (123)     8313 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gml.18f92cdfb2a6d10f.js
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_go.e302653e25089bba.js
--rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_graphql.8d0455822c35e9af.js
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_groovy.67837d37705d722b.js
--rw-r--r--   0 runner    (1001) docker     (123)     6051 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haml.9095964d871cb9e5.js
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_handlebars.3a1658c72e98aa85.js
--rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haskell.c37122cc55c1e696.js
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haxe.4e1677441d389a66.js
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hcl.f5277940e647aca6.js
--rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hlsl.f778194f7f56c677.js
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hpkp.2b3348708365f9ef.js
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hsts.5e3fe34e0eab5fdb.js
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_http.80f0633c0c6cabe9.js
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ichigojam.154c28afdb7a6cb3.js
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_icon.ee1eca6d9d8a1a78.js
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_iecst.ae937df11bf15aa5.js
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ignore.e7db33c594b328a4.js
--rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_inform7.25b80e018be9b4b0.js
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ini.1305ea3d405b7b77.js
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_io.57902ad550c5a076.js
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_j.d8b9ad361d46c928.js
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_java.375f3f7b940d3ea2.js
--rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javadoc.9022ca32626ca861.js
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javadoclike.a5b69d2a868cd5a6.js
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javascript.795b07cdb9c3aad5.js
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javastacktrace.8ef9f62617bbdae9.js
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jolie.fe8eb7d347ec2ee8.js
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jq.995d87dae4a1fc6c.js
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsExtras.a681c21d98be5d88.js
--rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsTemplates.e15b503a789336d0.js
--rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsdoc.863383140825aabf.js
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_json5.b916560a73dec284.js
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsonp.5d313969242bf8d5.js
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsstacktrace.237affac11d29a8e.js
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsx.66ae31b67824e2b1.js
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_julia.aebde82cc8e430a4.js
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_keyman.20a6fec54a9e6dc8.js
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_kotlin.204d94980c876688.js
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_latex.3ea6b205c4740fcf.js
--rw-r--r--   0 runner    (1001) docker     (123)     8821 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_latte.6c65a65bc30d6d65.js
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_less.571cfcc5f39892cf.js
--rw-r--r--   0 runner    (1001) docker     (123)     5499 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lilypond.b68fc0ec4de9b335.js
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_liquid.93e3d518888cf132.js
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lisp.eb4c988e1cb1b488.js
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_livescript.e154b07a04e47729.js
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_llvm.3edc24655432e967.js
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lolcode.920a08022d1f3fb3.js
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lua.b83366b41cb96d93.js
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_makefile.cac7a41c308ba41f.js
--rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markdown.06f7de54663dea9e.js
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markup.0001ba0d552266f8.js
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markupTemplating.1463fee82d988102.js
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_matlab.29f5102b58bb0786.js
--rw-r--r--   0 runner    (1001) docker     (123)    16942 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_mel.18e5992de05c1caa.js
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_mizar.2c0399b5c03c3450.js
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_monkey.bb2faba45e3cee8a.js
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_moonscript.e9dce6a537d684a9.js
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_n1ql.9924ec6c046bda5b.js
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_n4js.68b6d0a9d2b4e3b9.js
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nand2tetrisHdl.bd5b619f107eee8f.js
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nasm.08df2ec010d92ce1.js
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_neon.b4d21d37e14ff2e4.js
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nginx.a7f671ec4fed709c.js
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nim.b9b3330a8cc76ae6.js
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nix.ec8c698fe8cf158f.js
--rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nsis.17532a14606f8ba0.js
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_objectivec.a9a054b060f7e9c4.js
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ocaml.0ce7e66b58933eec.js
--rw-r--r--   0 runner    (1001) docker     (123)    12021 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_opencl.343386871671e433.js
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_oz.3dd791c14d6789e9.js
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_parigp.01c2a6558ead9c1d.js
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_parser.4080f0c5df8c5411.js
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pascal.714d7fd616dffa60.js
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pascaligo.3d9efa4ff03d798d.js
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pcaxis.dc2dc17ec584a4e1.js
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_peoplecode.00b98a730fe91b5e.js
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_perl.a4fecd65a9c2ecd2.js
--rw-r--r--   0 runner    (1001) docker     (123)     7638 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_php.1da6a39f37370ec1.js
--rw-r--r--   0 runner    (1001) docker     (123)     8084 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_phpExtras.8468f770a82630ef.js
--rw-r--r--   0 runner    (1001) docker     (123)     9335 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_phpdoc.59ba40872e3d9cfe.js
--rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_plsql.6fc1cf5b4b2439a3.js
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_powerquery.c87eb035121d7831.js
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_powershell.56966af030c91702.js
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_processing.ec8607c7392a938f.js
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_prolog.22a1c7ff76f01643.js
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_properties.c3ce1ad33d9983e2.js
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_protobuf.d96df12b0f0a2409.js
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pug.6b509aa2c3a57467.js
--rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_puppet.ce519d4962965362.js
--rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pure.e3fd8806900462cf.js
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_purebasic.70942e3d774ada85.js
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_q.1df151a687a188a7.js
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_qml.e36896b667a01ae9.js
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_qore.1137d54889243367.js
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_r.7ca305d9455cc86f.js
--rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_racket.bee31c56faa733b2.js
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_reason.af902fad4bd674df.js
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_regex.074352f8c0201b38.js
--rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_renpy.5938c171f23d6f29.js
--rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rest.fcefb9b5cfa112e0.js
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rip.5f599ff53f5c1e9a.js
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_roboconf.49d8eaad661bcd43.js
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_robotframework.883fa1f592ad87e7.js
--rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ruby.f76b4f68b3137a6f.js
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rust.ca92b5ca27e7312d.js
--rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sas.33e0e78e18cf156f.js
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sass.8436ff53b0701941.js
--rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scala.7db11a73d01e23d4.js
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scheme.a224b3505cc86f4d.js
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scss.fbd015582067d022.js
--rw-r--r--   0 runner    (1001) docker     (123)     7202 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_shellSession.54615d020c9c44d5.js
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smali.e44f80bb9100f728.js
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smalltalk.e89fea8686ec9f90.js
--rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smarty.404a8e12834103cf.js
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_solidity.537cb7600d04dae8.js
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_solutionFile.53d3dde6d83fdea2.js
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_soy.51e9adabd56f467a.js
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sparql.2aa3288ef8ae3374.js
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_splunkSpl.095636b50fe9a368.js
--rw-r--r--   0 runner    (1001) docker     (123)    33525 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sqf.11b0bee7a2de8e94.js
--rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_stylus.213bb148fbffff7f.js
--rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_swift.27d0fee1e44e54b6.js
--rw-r--r--   0 runner    (1001) docker     (123)     7602 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Cs.cd31c8bc90add20f.js
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Templating.c87834ec2ea19f73.js
--rw-r--r--   0 runner    (1001) docker     (123)     4746 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Vb.2cf235d46995926d.js
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tap.a22e7b01443f999b.js
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tcl.72a4244b8fb7ec0d.js
--rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_textile.e52c4e181b801ddd.js
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_toml.9bf8ce9e1f31a008.js
--rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tsx.f039389d397f2bb4.js
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tt2.645259383cf82689.js
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_turtle.69d8330a2e17bb57.js
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_twig.d5bfca25e9d2543d.js
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_typescript.d8f51be2a38383c6.js
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_unrealscript.9179623df9a8b80c.js
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vala.2e16603251de6f51.js
--rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vbnet.ac96de8240011055.js
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_velocity.bc75ee95252e2b47.js
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_verilog.4e42ac1a89cb8605.js
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vhdl.5ab0f6bc359d7c74.js
--rw-r--r--   0 runner    (1001) docker     (123)    14361 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vim.6c4d4c01dc147971.js
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_visualBasic.c3e43390c4a3ee45.js
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_warpscript.ccc821a2177dfac0.js
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_wasm.3ffc1a78867a6148.js
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_wiki.b5dc9ed00ff4ea53.js
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xeora.b31606451a6f896b.js
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xmlDoc.3eb6beae8084d868.js
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xojo.81cb4d9104c6ac5b.js
--rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xquery.4382c54a41b1309a.js
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_yaml.178577f1d765f16b.js
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_yang.28bbfbd268843c68.js
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_zig.a535909b59fc6987.js
--rw-r--r--   0 runner    (1001) docker     (123)    23694 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/webpack-6ed703bc0f4dd2fe.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:15:27.321975 featureform-1.8.0/src/featureform/dashboard/out/_next/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/css/85a2addfd2efc882.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:15:27.321975 featureform-1.8.0/src/featureform/dashboard/out/_next/static/media/
--rw-r--r--   0 runner    (1001) docker     (123)    81048 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/media/Matter-Regular.f1ae4ce5.ttf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:15:27.321975 featureform-1.8.0/src/featureform/dashboard/out/_next/static/u8jMEl73MAEGHR4r4U4Dw/
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-01 21:13:34.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/u8jMEl73MAEGHR4r4U4Dw/_buildManifest.js
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-01 21:13:34.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/u8jMEl73MAEGHR4r4U4Dw/_ssgManifest.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:15:27.321975 featureform-1.8.0/src/featureform/dashboard/out/_next/static/xB9Lh8aE_cExc1t6WFtEI/
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-01 21:13:34.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/xB9Lh8aE_cExc1t6WFtEI/_buildManifest.js
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-01 21:13:34.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/xB9Lh8aE_cExc1t6WFtEI/_ssgManifest.js
--rw-r--r--   0 runner    (1001) docker     (123)    27046 2023-05-01 21:15:20.000000 featureform-1.8.0/src/featureform/dashboard/out/connections.html
--rw-r--r--   0 runner    (1001) docker     (123)    35824 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/index.html
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/robots.txt
--rw-r--r--   0 runner    (1001) docker     (123)    17992 2023-05-01 21:15:20.000000 featureform-1.8.0/src/featureform/dashboard/out/search.html
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/site.webmanifest
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:15:27.329976 featureform-1.8.0/src/featureform/dashboard/out/static/
--rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/static/Apache_Spark_logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5390 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/static/Capital_One_logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/static/FeatureForm_Logo_Full_Black.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/static/Featureform_logo_pink.svg
--rw-r--r--   0 runner    (1001) docker     (123)    11281 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/static/Kubernetes_logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4440 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/static/Postgresql_elephant.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/static/Redis_Logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)    61862 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/static/Snowflake_Logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6384 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/static/amazon-dynamoDB.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4629 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/static/amazon_redshift.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/static/amazon_s3.svg
--rw-r--r--   0 runner    (1001) docker     (123)    26573 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/static/apache_cassandra.svg
--rw-r--r--   0 runner    (1001) docker     (123)    60161 2023-05-01 21:15:20.000000 featureform-1.8.0/src/featureform/dashboard/out/static/apache_hadoop.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-05-01 21:15:20.000000 featureform-1.8.0/src/featureform/dashboard/out/static/apple-touch-icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-01 21:15:20.000000 featureform-1.8.0/src/featureform/dashboard/out/static/azure_storage_accounts.svg
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-01 21:15:20.000000 featureform-1.8.0/src/featureform/dashboard/out/static/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-01 21:15:20.000000 featureform-1.8.0/src/featureform/dashboard/out/static/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-05-01 21:15:20.000000 featureform-1.8.0/src/featureform/dashboard/out/static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-01 21:15:20.000000 featureform-1.8.0/src/featureform/dashboard/out/static/google_bigquery.svg
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-01 21:15:20.000000 featureform-1.8.0/src/featureform/dashboard/out/static/google_cloud_storage.svg
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-01 21:15:20.000000 featureform-1.8.0/src/featureform/dashboard/out/static/google_firestore.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-05-01 21:15:20.000000 featureform-1.8.0/src/featureform/dashboard/out/static/logo192.png
--rw-r--r--   0 runner    (1001) docker     (123)     8459 2023-05-01 21:15:20.000000 featureform-1.8.0/src/featureform/dashboard/out/static/logo512.png
--rw-r--r--   0 runner    (1001) docker     (123)     7755 2023-05-01 21:15:20.000000 featureform-1.8.0/src/featureform/dashboard/out/static/mongoDB.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-05-01 21:15:20.000000 featureform-1.8.0/src/featureform/dashboard/out/static/safari-pinned-tab.svg
--rw-r--r--   0 runner    (1001) docker     (123)    17938 2023-05-01 21:13:34.000000 featureform-1.8.0/src/featureform/dashboard_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-05-01 21:13:34.000000 featureform-1.8.0/src/featureform/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-01 21:13:34.000000 featureform-1.8.0/src/featureform/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-05-01 21:13:34.000000 featureform-1.8.0/src/featureform/format.py
--rw-r--r--   0 runner    (1001) docker     (123)    10666 2023-05-01 21:13:34.000000 featureform-1.8.0/src/featureform/get.py
--rw-r--r--   0 runner    (1001) docker     (123)    17354 2023-05-01 21:13:34.000000 featureform-1.8.0/src/featureform/get_local.py
--rw-r--r--   0 runner    (1001) docker     (123)    20239 2023-05-01 21:13:34.000000 featureform-1.8.0/src/featureform/get_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-05-01 21:13:34.000000 featureform-1.8.0/src/featureform/list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-05-01 21:13:34.000000 featureform-1.8.0/src/featureform/list_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     8100 2023-05-01 21:13:34.000000 featureform-1.8.0/src/featureform/list_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-01 21:13:34.000000 featureform-1.8.0/src/featureform/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     7520 2023-05-01 21:13:34.000000 featureform-1.8.0/src/featureform/local_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    89279 2023-05-01 21:13:34.000000 featureform-1.8.0/src/featureform/local_dash_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-05-01 21:13:34.000000 featureform-1.8.0/src/featureform/local_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:15:27.329976 featureform-1.8.0/src/featureform/proto/
--rw-r--r--   0 runner    (1001) docker     (123)     9975 2023-05-01 21:14:32.000000 featureform-1.8.0/src/featureform/proto/metadata.proto
--rw-r--r--   0 runner    (1001) docker     (123)    23763 2023-05-01 21:14:33.000000 featureform-1.8.0/src/featureform/proto/metadata_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)   102266 2023-05-01 21:14:33.000000 featureform-1.8.0/src/featureform/proto/metadata_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-05-01 21:14:32.000000 featureform-1.8.0/src/featureform/proto/serving.proto
--rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-05-01 21:14:33.000000 featureform-1.8.0/src/featureform/proto/serving_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7808 2023-05-01 21:14:33.000000 featureform-1.8.0/src/featureform/proto/serving_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)   159624 2023-05-01 21:13:34.000000 featureform-1.8.0/src/featureform/register.py
--rw-r--r--   0 runner    (1001) docker     (123)    17986 2023-05-01 21:13:34.000000 featureform-1.8.0/src/featureform/register_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    58803 2023-05-01 21:13:34.000000 featureform-1.8.0/src/featureform/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-01 21:13:34.000000 featureform-1.8.0/src/featureform/search.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-01 21:13:34.000000 featureform-1.8.0/src/featureform/search_local.py
--rw-r--r--   0 runner    (1001) docker     (123)    34805 2023-05-01 21:13:34.000000 featureform-1.8.0/src/featureform/serving.py
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-01 21:13:34.000000 featureform-1.8.0/src/featureform/serving_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    29384 2023-05-01 21:13:34.000000 featureform-1.8.0/src/featureform/sqlite_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-01 21:13:34.000000 featureform-1.8.0/src/featureform/tls.py
--rw-r--r--   0 runner    (1001) docker     (123)     8991 2023-05-01 21:13:34.000000 featureform-1.8.0/src/featureform/type_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-01 21:13:34.000000 featureform-1.8.0/src/featureform/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:15:27.261973 featureform-1.8.0/src/featureform.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-05-01 21:15:27.000000 featureform-1.8.0/src/featureform.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    33006 2023-05-01 21:15:27.000000 featureform-1.8.0/src/featureform.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 21:15:27.000000 featureform-1.8.0/src/featureform.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-01 21:15:27.000000 featureform-1.8.0/src/featureform.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-01 21:15:27.000000 featureform-1.8.0/src/featureform.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-01 21:15:27.000000 featureform-1.8.0/src/featureform.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:15:27.333976 featureform-1.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    10754 2023-05-01 21:13:34.000000 featureform-1.8.0/tests/test_class_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-05-01 21:13:34.000000 featureform-1.8.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-05-01 21:13:34.000000 featureform-1.8.0/tests/test_executor_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-05-01 21:13:34.000000 featureform-1.8.0/tests/test_getting_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8225 2023-05-01 21:13:34.000000 featureform-1.8.0/tests/test_localmode_caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-05-01 21:13:34.000000 featureform-1.8.0/tests/test_localmode_include_label_ts.py
--rw-r--r--   0 runner    (1001) docker     (123)    11029 2023-05-01 21:13:34.000000 featureform-1.8.0/tests/test_localmode_lag_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-05-01 21:13:34.000000 featureform-1.8.0/tests/test_ondemand_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-05-01 21:13:34.000000 featureform-1.8.0/tests/test_resource_registration.py
--rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-05-01 21:13:34.000000 featureform-1.8.0/tests/test_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    15831 2023-05-01 21:13:34.000000 featureform-1.8.0/tests/test_serving_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4772 2023-05-01 21:13:34.000000 featureform-1.8.0/tests/test_source_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-05-01 21:13:34.000000 featureform-1.8.0/tests/test_spark_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    30091 2023-05-01 21:13:34.000000 featureform-1.8.0/tests/test_tags_and_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     7259 2023-05-01 21:13:34.000000 featureform-1.8.0/tests/test_updating_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:41:24.855564 featureform-1.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    16724 2023-05-16 19:39:40.000000 featureform-1.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-16 19:39:40.000000 featureform-1.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-05-16 19:41:24.855564 featureform-1.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-05-16 19:39:40.000000 featureform-1.8.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-16 19:39:40.000000 featureform-1.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-05-16 19:41:24.855564 featureform-1.8.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:41:24.795560 featureform-1.8.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:41:24.803560 featureform-1.8.1/src/featureform/
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-16 19:39:40.000000 featureform-1.8.1/src/featureform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-16 19:39:40.000000 featureform-1.8.1/src/featureform/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7509 2023-05-16 19:39:40.000000 featureform-1.8.1/src/featureform/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-05-16 19:39:40.000000 featureform-1.8.1/src/featureform/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-16 19:39:40.000000 featureform-1.8.1/src/featureform/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:41:24.795560 featureform-1.8.1/src/featureform/dashboard/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:41:24.803560 featureform-1.8.1/src/featureform/dashboard/out/
+-rw-r--r--   0 runner    (1001) docker     (123)    17392 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/404.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:41:24.803560 featureform-1.8.1/src/featureform/dashboard/out/[type]/
+-rw-r--r--   0 runner    (1001) docker     (123)    18184 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/[type]/[entity].html
+-rw-r--r--   0 runner    (1001) docker     (123)    17416 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/[type].html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:41:24.795560 featureform-1.8.1/src/featureform/dashboard/out/_next/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:41:24.795560 featureform-1.8.1/src/featureform/dashboard/out/_next/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:41:24.803560 featureform-1.8.1/src/featureform/dashboard/out/_next/static/Jopdpwd8wB7tMgkcaVnsn/
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-16 19:39:40.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/Jopdpwd8wB7tMgkcaVnsn/_buildManifest.js
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-16 19:39:40.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/Jopdpwd8wB7tMgkcaVnsn/_ssgManifest.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:41:24.803560 featureform-1.8.1/src/featureform/dashboard/out/_next/static/aZJnz9nRD9kOWLAxrQep6/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/aZJnz9nRD9kOWLAxrQep6/_buildManifest.js
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/aZJnz9nRD9kOWLAxrQep6/_ssgManifest.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:41:24.839563 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/
+-rw-r--r--   0 runner    (1001) docker     (123)    83561 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/72a30a16.5298cad0ba46633d.js
+-rw-r--r--   0 runner    (1001) docker     (123)    74481 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/7679.34cabcdac6ff42f5.js
+-rw-r--r--   0 runner    (1001) docker     (123)    21739 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/7856.43cc2293f00befb0.js
+-rw-r--r--   0 runner    (1001) docker     (123)   201393 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/ad7f724d.b238476ad0e6f6d2.js
+-rw-r--r--   0 runner    (1001) docker     (123)   130270 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/framework-3412d1150754b2fb.js
+-rw-r--r--   0 runner    (1001) docker     (123)   104027 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/main-2715d0c23f47c019.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:41:24.847564 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/pages/404-baaca4b2f4acc755.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:41:24.847564 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/pages/[type]/
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/pages/[type]/[entity]-92ac9566fcd3bf59.js
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/pages/[type]-1354c91ed8b0be2c.js
+-rw-r--r--   0 runner    (1001) docker     (123)  3582701 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/pages/_app-535a9349f87f23c6.js
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/pages/_error-3f70f2d61eb8c6dd.js
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/pages/connections-1d67ba61869dece6.js
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/pages/index-942ec646d90d2132.js
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/pages/query-9193959c04ff1e72.js
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/pages/search-175858e61ba25631.js
+-rw-r--r--   0 runner    (1001) docker     (123)    91460 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:41:24.847564 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter/
+-rw-r--r--   0 runner    (1001) docker     (123)    35679 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter/refractor-core-import.d200df4f5651fe3c.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8068 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_abap.cff854fd7e5b1247.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_abnf.a1ff159f2ef1711f.js
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_actionscript.efd417c28a28b388.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ada.156060425d9edae1.js
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_agda.7c059beeef27c79a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_al.f8ab011377e6cffa.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_antlr4.2c3a6fa926d2a251.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8341 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_apacheconf.a8e9c6e2469ebb48.js
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_apl.17fe889a8c792ca2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_applescript.ec5486ed51b5bf2a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_aql.efb695712e3f3aa3.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8763 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_arduino.681aaa7ec91aa809.js
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_arff.ab502da8667e6dc6.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_asciidoc.d34ffa4ca9efdc4d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_asm6502.3eb992d6df117427.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7829 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_aspnet.0ba8de8f97453373.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9289 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_autohotkey.8bd8b23c56f29881.js
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_autoit.f687b627eb6354c6.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bash.fa5423ba02f0452a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_basic.18dbad942d626219.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_batch.8ca1ac5c2d037485.js
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bbcode.4b540b8d0f463220.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bison.3be4b74c3d3e0770.js
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bnf.d1d39a9bd6ac45b9.js
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_brainfuck.42d8625dbbdd27ed.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_brightscript.5219a23e15549d0f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bro.6a3db5175eef5a7c.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_c.fba60a9486edee8d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cil.494c2357f1d5de1e.js
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_clike.065b788c95ab7f0a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_clojure.144f4fa5cb5b7c94.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10794 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cmake.63bd8fd3867951a6.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_coffeescript.f3407609f464e5a7.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_concurnas.807a36085ae57a51.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cpp.9073ce25850a9aee.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5129 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_crystal.500857f6d38420ca.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6662 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_csharp.1ab46bae80c6b0ba.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_csp.dbb73c45172741db.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_css.c6ce776800cc984e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cssExtras.9588a637662140d4.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cypher.899ff7f5c7459114.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_d.3e486cddc20d2ff9.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dart.9db40f270a0b6cb0.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dax.f58ad34d65866793.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dhall.0ca1a915d1865fb5.js
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_diff.e343fa532144b7a2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_django.6ee6c39cb914f163.js
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dnsZoneFile.2a9886e744590498.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_docker.fde534872e6578fd.js
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ebnf.35e28e1f6e8a00e4.js
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_editorconfig.17a13e6bcda1e1f3.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_eiffel.64ef4de4060b9a23.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ejs.4c4ccb70f90dea01.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_elixir.a1e48f12166c723b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_elm.6765aa0f50cbaf91.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_erb.e48ed285a1945936.js
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_erlang.2a114ebcf8dd2d26.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_etlua.afcb29f06feae539.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_excelFormula.62d0fdeee42f5d64.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10203 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_factor.ce84f1b770942d68.js
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_firestoreSecurityRules.209ede8c07b9e60b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_flow.88a9cbf968cf47ec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_fortran.ca33766cb3d9d13c.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_fsharp.1aa244fc87692af1.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ftl.0457d46374506e78.js
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gcode.ac01f4f7ac16a003.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gdscript.afa83bf48d38ded2.js
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gedcom.eae35079f43f4e91.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9971 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gherkin.1226aeae8764f3d7.js
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_git.0e0594706d30fbd8.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_glsl.aaa801f4d5c6da96.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8313 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gml.18f92cdfb2a6d10f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_go.e302653e25089bba.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_graphql.8d0455822c35e9af.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_groovy.67837d37705d722b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6051 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haml.9095964d871cb9e5.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_handlebars.3a1658c72e98aa85.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haskell.c37122cc55c1e696.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haxe.4e1677441d389a66.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hcl.f5277940e647aca6.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hlsl.f778194f7f56c677.js
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hpkp.2b3348708365f9ef.js
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hsts.5e3fe34e0eab5fdb.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_http.80f0633c0c6cabe9.js
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ichigojam.154c28afdb7a6cb3.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_icon.ee1eca6d9d8a1a78.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_iecst.ae937df11bf15aa5.js
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ignore.e7db33c594b328a4.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_inform7.25b80e018be9b4b0.js
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ini.1305ea3d405b7b77.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_io.57902ad550c5a076.js
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_j.d8b9ad361d46c928.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_java.375f3f7b940d3ea2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javadoc.9022ca32626ca861.js
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javadoclike.a5b69d2a868cd5a6.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javascript.795b07cdb9c3aad5.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javastacktrace.8ef9f62617bbdae9.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jolie.fe8eb7d347ec2ee8.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jq.995d87dae4a1fc6c.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsExtras.a681c21d98be5d88.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsTemplates.e15b503a789336d0.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsdoc.863383140825aabf.js
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_json5.b916560a73dec284.js
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsonp.5d313969242bf8d5.js
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsstacktrace.237affac11d29a8e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsx.66ae31b67824e2b1.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_julia.aebde82cc8e430a4.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_keyman.20a6fec54a9e6dc8.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_kotlin.204d94980c876688.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_latex.3ea6b205c4740fcf.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8821 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_latte.6c65a65bc30d6d65.js
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_less.571cfcc5f39892cf.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5499 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lilypond.b68fc0ec4de9b335.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_liquid.93e3d518888cf132.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lisp.eb4c988e1cb1b488.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_livescript.e154b07a04e47729.js
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_llvm.3edc24655432e967.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lolcode.920a08022d1f3fb3.js
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lua.b83366b41cb96d93.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_makefile.cac7a41c308ba41f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markdown.06f7de54663dea9e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markup.0001ba0d552266f8.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markupTemplating.1463fee82d988102.js
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_matlab.29f5102b58bb0786.js
+-rw-r--r--   0 runner    (1001) docker     (123)    16942 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_mel.18e5992de05c1caa.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_mizar.2c0399b5c03c3450.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_monkey.bb2faba45e3cee8a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_moonscript.e9dce6a537d684a9.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_n1ql.9924ec6c046bda5b.js
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_n4js.68b6d0a9d2b4e3b9.js
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nand2tetrisHdl.bd5b619f107eee8f.js
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nasm.08df2ec010d92ce1.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_neon.b4d21d37e14ff2e4.js
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nginx.a7f671ec4fed709c.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nim.b9b3330a8cc76ae6.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nix.ec8c698fe8cf158f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nsis.17532a14606f8ba0.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_objectivec.a9a054b060f7e9c4.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ocaml.0ce7e66b58933eec.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12021 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_opencl.343386871671e433.js
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_oz.3dd791c14d6789e9.js
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_parigp.01c2a6558ead9c1d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_parser.4080f0c5df8c5411.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pascal.714d7fd616dffa60.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pascaligo.3d9efa4ff03d798d.js
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pcaxis.dc2dc17ec584a4e1.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_peoplecode.00b98a730fe91b5e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_perl.a4fecd65a9c2ecd2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7638 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_php.1da6a39f37370ec1.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8084 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_phpExtras.8468f770a82630ef.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9335 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_phpdoc.59ba40872e3d9cfe.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_plsql.6fc1cf5b4b2439a3.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_powerquery.c87eb035121d7831.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_powershell.56966af030c91702.js
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_processing.ec8607c7392a938f.js
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_prolog.22a1c7ff76f01643.js
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_properties.c3ce1ad33d9983e2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_protobuf.d96df12b0f0a2409.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pug.6b509aa2c3a57467.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_puppet.ce519d4962965362.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pure.e3fd8806900462cf.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_purebasic.70942e3d774ada85.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_q.1df151a687a188a7.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_qml.e36896b667a01ae9.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_qore.1137d54889243367.js
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_r.7ca305d9455cc86f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_racket.bee31c56faa733b2.js
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_reason.af902fad4bd674df.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_regex.074352f8c0201b38.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_renpy.5938c171f23d6f29.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rest.fcefb9b5cfa112e0.js
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rip.5f599ff53f5c1e9a.js
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_roboconf.49d8eaad661bcd43.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_robotframework.883fa1f592ad87e7.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ruby.f76b4f68b3137a6f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rust.ca92b5ca27e7312d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sas.33e0e78e18cf156f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sass.8436ff53b0701941.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scala.7db11a73d01e23d4.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scheme.a224b3505cc86f4d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scss.fbd015582067d022.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7202 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_shellSession.54615d020c9c44d5.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smali.e44f80bb9100f728.js
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smalltalk.e89fea8686ec9f90.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smarty.404a8e12834103cf.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_solidity.537cb7600d04dae8.js
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_solutionFile.53d3dde6d83fdea2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_soy.51e9adabd56f467a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sparql.2aa3288ef8ae3374.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_splunkSpl.095636b50fe9a368.js
+-rw-r--r--   0 runner    (1001) docker     (123)    33525 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sqf.11b0bee7a2de8e94.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_stylus.213bb148fbffff7f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_swift.27d0fee1e44e54b6.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7602 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Cs.cd31c8bc90add20f.js
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Templating.c87834ec2ea19f73.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4746 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Vb.2cf235d46995926d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tap.a22e7b01443f999b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tcl.72a4244b8fb7ec0d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_textile.e52c4e181b801ddd.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_toml.9bf8ce9e1f31a008.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tsx.f039389d397f2bb4.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tt2.645259383cf82689.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_turtle.69d8330a2e17bb57.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_twig.d5bfca25e9d2543d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_typescript.d8f51be2a38383c6.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_unrealscript.9179623df9a8b80c.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vala.2e16603251de6f51.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vbnet.ac96de8240011055.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_velocity.bc75ee95252e2b47.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_verilog.4e42ac1a89cb8605.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vhdl.5ab0f6bc359d7c74.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14361 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vim.6c4d4c01dc147971.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_visualBasic.c3e43390c4a3ee45.js
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_warpscript.ccc821a2177dfac0.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_wasm.3ffc1a78867a6148.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_wiki.b5dc9ed00ff4ea53.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xeora.b31606451a6f896b.js
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xmlDoc.3eb6beae8084d868.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xojo.81cb4d9104c6ac5b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xquery.4382c54a41b1309a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_yaml.178577f1d765f16b.js
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_yang.28bbfbd268843c68.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_zig.a535909b59fc6987.js
+-rw-r--r--   0 runner    (1001) docker     (123)    23694 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/webpack-6ed703bc0f4dd2fe.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:41:24.847564 featureform-1.8.1/src/featureform/dashboard/out/_next/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/css/85a2addfd2efc882.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:41:24.847564 featureform-1.8.1/src/featureform/dashboard/out/_next/static/media/
+-rw-r--r--   0 runner    (1001) docker     (123)    81048 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/media/Matter-Regular.f1ae4ce5.ttf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:41:24.847564 featureform-1.8.1/src/featureform/dashboard/out/_next/static/u8jMEl73MAEGHR4r4U4Dw/
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-16 19:39:40.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/u8jMEl73MAEGHR4r4U4Dw/_buildManifest.js
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-16 19:39:40.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/u8jMEl73MAEGHR4r4U4Dw/_ssgManifest.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:41:24.847564 featureform-1.8.1/src/featureform/dashboard/out/_next/static/xB9Lh8aE_cExc1t6WFtEI/
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-16 19:39:40.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/xB9Lh8aE_cExc1t6WFtEI/_buildManifest.js
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-16 19:39:40.000000 featureform-1.8.1/src/featureform/dashboard/out/_next/static/xB9Lh8aE_cExc1t6WFtEI/_ssgManifest.js
+-rw-r--r--   0 runner    (1001) docker     (123)    27274 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/connections.html
+-rw-r--r--   0 runner    (1001) docker     (123)    36052 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)    18217 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/query.html
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/robots.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    18220 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/search.html
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/site.webmanifest
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:41:24.851564 featureform-1.8.1/src/featureform/dashboard/out/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/static/Apache_Spark_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5390 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/static/Capital_One_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/static/FeatureForm_Logo_Full_Black.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/static/Featureform_logo_pink.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    11281 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/static/Kubernetes_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4440 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/static/Postgresql_elephant.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/static/Redis_Logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    61862 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/static/Snowflake_Logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6384 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/static/amazon-dynamoDB.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4629 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/static/amazon_redshift.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/static/amazon_s3.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    26573 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/static/apache_cassandra.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    60161 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/static/apache_hadoop.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/static/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/static/azure_storage_accounts.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/static/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/static/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/static/google_bigquery.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/static/google_cloud_storage.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/static/google_firestore.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/static/logo192.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8459 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/static/logo512.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7755 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/static/mongoDB.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-05-16 19:41:17.000000 featureform-1.8.1/src/featureform/dashboard/out/static/safari-pinned-tab.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    18039 2023-05-16 19:39:40.000000 featureform-1.8.1/src/featureform/dashboard_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-05-16 19:39:40.000000 featureform-1.8.1/src/featureform/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-16 19:39:40.000000 featureform-1.8.1/src/featureform/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-05-16 19:39:40.000000 featureform-1.8.1/src/featureform/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10666 2023-05-16 19:39:40.000000 featureform-1.8.1/src/featureform/get.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17354 2023-05-16 19:39:40.000000 featureform-1.8.1/src/featureform/get_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20239 2023-05-16 19:39:40.000000 featureform-1.8.1/src/featureform/get_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-05-16 19:39:40.000000 featureform-1.8.1/src/featureform/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-05-16 19:39:40.000000 featureform-1.8.1/src/featureform/list_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8100 2023-05-16 19:39:40.000000 featureform-1.8.1/src/featureform/list_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-16 19:39:40.000000 featureform-1.8.1/src/featureform/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7520 2023-05-16 19:39:40.000000 featureform-1.8.1/src/featureform/local_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89279 2023-05-16 19:39:40.000000 featureform-1.8.1/src/featureform/local_dash_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-05-16 19:39:40.000000 featureform-1.8.1/src/featureform/local_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:41:24.851564 featureform-1.8.1/src/featureform/proto/
+-rw-r--r--   0 runner    (1001) docker     (123)     9975 2023-05-16 19:40:30.000000 featureform-1.8.1/src/featureform/proto/metadata.proto
+-rw-r--r--   0 runner    (1001) docker     (123)    23763 2023-05-16 19:40:31.000000 featureform-1.8.1/src/featureform/proto/metadata_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)   102266 2023-05-16 19:40:31.000000 featureform-1.8.1/src/featureform/proto/metadata_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-05-16 19:40:30.000000 featureform-1.8.1/src/featureform/proto/serving.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-05-16 19:40:31.000000 featureform-1.8.1/src/featureform/proto/serving_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7808 2023-05-16 19:40:31.000000 featureform-1.8.1/src/featureform/proto/serving_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)   161001 2023-05-16 19:39:40.000000 featureform-1.8.1/src/featureform/register.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17986 2023-05-16 19:39:40.000000 featureform-1.8.1/src/featureform/register_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58803 2023-05-16 19:39:40.000000 featureform-1.8.1/src/featureform/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-16 19:39:40.000000 featureform-1.8.1/src/featureform/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-16 19:39:40.000000 featureform-1.8.1/src/featureform/search_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35277 2023-05-16 19:39:40.000000 featureform-1.8.1/src/featureform/serving.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-16 19:39:40.000000 featureform-1.8.1/src/featureform/serving_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29384 2023-05-16 19:39:40.000000 featureform-1.8.1/src/featureform/sqlite_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-05-16 19:39:40.000000 featureform-1.8.1/src/featureform/status_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-16 19:39:40.000000 featureform-1.8.1/src/featureform/tls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8991 2023-05-16 19:39:40.000000 featureform-1.8.1/src/featureform/type_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-16 19:39:40.000000 featureform-1.8.1/src/featureform/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:41:24.803560 featureform-1.8.1/src/featureform.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-05-16 19:41:24.000000 featureform-1.8.1/src/featureform.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    33163 2023-05-16 19:41:24.000000 featureform-1.8.1/src/featureform.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 19:41:24.000000 featureform-1.8.1/src/featureform.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-16 19:41:24.000000 featureform-1.8.1/src/featureform.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-16 19:41:24.000000 featureform-1.8.1/src/featureform.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-16 19:41:24.000000 featureform-1.8.1/src/featureform.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:41:24.855564 featureform-1.8.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    10754 2023-05-16 19:39:40.000000 featureform-1.8.1/tests/test_class_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-05-16 19:39:40.000000 featureform-1.8.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-05-16 19:39:40.000000 featureform-1.8.1/tests/test_executor_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-05-16 19:39:40.000000 featureform-1.8.1/tests/test_getting_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8225 2023-05-16 19:39:40.000000 featureform-1.8.1/tests/test_localmode_caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-05-16 19:39:40.000000 featureform-1.8.1/tests/test_localmode_include_label_ts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11029 2023-05-16 19:39:40.000000 featureform-1.8.1/tests/test_localmode_lag_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-05-16 19:39:40.000000 featureform-1.8.1/tests/test_ondemand_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-05-16 19:39:40.000000 featureform-1.8.1/tests/test_resource_registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-05-16 19:39:40.000000 featureform-1.8.1/tests/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15831 2023-05-16 19:39:40.000000 featureform-1.8.1/tests/test_serving_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4772 2023-05-16 19:39:40.000000 featureform-1.8.1/tests/test_source_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-05-16 19:39:40.000000 featureform-1.8.1/tests/test_spark_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30091 2023-05-16 19:39:40.000000 featureform-1.8.1/tests/test_tags_and_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7259 2023-05-16 19:39:40.000000 featureform-1.8.1/tests/test_updating_provider.py
```

### Comparing `featureform-1.8.0/LICENSE` & `featureform-1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/PKG-INFO` & `featureform-1.8.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featureform
-Version: 1.8.0
+Version: 1.8.1
 Summary: Package for the Featureform Feature Store
 Home-page: https://featureform.com
 Author: FeatureForm, Inc.
 Author-email: hello@featureform.com
 Project-URL: Bug Tracker, https://github.com/featureform/embeddinghub/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

### Comparing `featureform-1.8.0/README.md` & `featureform-1.8.1/README.md`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/setup.cfg` & `featureform-1.8.1/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = featureform
-version = 1.8.0
+version = 1.8.1
 author = FeatureForm, Inc.
 author_email = hello@featureform.com
 description = Package for the Featureform Feature Store
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://featureform.com
 project_urls =
```

### Comparing `featureform-1.8.0/src/featureform/__init__.py` & `featureform-1.8.1/src/featureform/__init__.py`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/cli.py` & `featureform-1.8.1/src/featureform/cli.py`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/client.py` & `featureform-1.8.1/src/featureform/client.py`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/404.html` & `featureform-1.8.1/src/featureform/dashboard/out/404.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,136 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-6ed703bc0f4dd2fe.js" defer=""></script><script src="/_next/static/chunks/framework-3412d1150754b2fb.js" defer=""></script><script src="/_next/static/chunks/main-2715d0c23f47c019.js" defer=""></script><script src="/_next/static/chunks/pages/_app-a764893ff9420ec0.js" defer=""></script><script src="/_next/static/chunks/pages/404-baaca4b2f4acc755.js" defer=""></script><script src="/_next/static/XLqQwuMDcHNwRKV5unb2J/_buildManifest.js" defer=""></script><script src="/_next/static/XLqQwuMDcHNwRKV5unb2J/_ssgManifest.js" defer=""></script><style id="jss-server-side">.MuiTypography-root {
-  margin: 0;
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-6ed703bc0f4dd2fe.js" defer=""></script><script src="/_next/static/chunks/framework-3412d1150754b2fb.js" defer=""></script><script src="/_next/static/chunks/main-2715d0c23f47c019.js" defer=""></script><script src="/_next/static/chunks/pages/_app-535a9349f87f23c6.js" defer=""></script><script src="/_next/static/chunks/pages/404-baaca4b2f4acc755.js" defer=""></script><script src="/_next/static/aZJnz9nRD9kOWLAxrQep6/_buildManifest.js" defer=""></script><script src="/_next/static/aZJnz9nRD9kOWLAxrQep6/_ssgManifest.js" defer=""></script><style id="jss-server-side">.MuiContainer-root {
+  width: 100%;
+  display: block;
+  box-sizing: border-box;
+  margin-left: auto;
+  margin-right: auto;
+  padding-left: 16px;
+  padding-right: 16px;
 }
-.MuiTypography-body2 {
-  font-size: 0.875rem;
-  font-family: "Matter", "Lato", "Helvetica", sans-serif;
-  font-weight: 550;
-  line-height: 1.43;
-}
-.MuiTypography-body1 {
-  font-size: 1rem;
-  font-family: "Matter", "Lato", "Helvetica", sans-serif;
-  font-weight: 550;
-  line-height: 1.5;
-}
-.MuiTypography-caption {
-  font-size: 0.75rem;
-  font-family: "Matter", "Lato", "Helvetica", sans-serif;
-  font-weight: 550;
-  line-height: 1.66;
-}
-.MuiTypography-button {
-  font-size: 0.875rem;
-  font-family: "Matter", "Lato", "Helvetica", sans-serif;
-  font-weight: 650;
-  line-height: 1.75;
-  text-transform: uppercase;
-}
-.MuiTypography-h1 {
-  font-size: 3.5rem;
-  font-family: "Matter", "Lato", "Helvetica", sans-serif;
-  font-weight: 450;
-  line-height: 1.167;
+@media (min-width:600px) {
+  .MuiContainer-root {
+    padding-left: 24px;
+    padding-right: 24px;
+  }
+}
+  .MuiContainer-disableGutters {
+    padding-left: 0;
+    padding-right: 0;
+  }
+@media (min-width:600px) {
+  .MuiContainer-fixed {
+    max-width: 600px;
+  }
+}
+@media (min-width:960px) {
+  .MuiContainer-fixed {
+    max-width: 960px;
+  }
+}
+@media (min-width:1280px) {
+  .MuiContainer-fixed {
+    max-width: 1280px;
+  }
+}
+@media (min-width:1920px) {
+  .MuiContainer-fixed {
+    max-width: 1920px;
+  }
+}
+@media (min-width:0px) {
+  .MuiContainer-maxWidthXs {
+    max-width: 444px;
+  }
+}
+@media (min-width:600px) {
+  .MuiContainer-maxWidthSm {
+    max-width: 600px;
+  }
+}
+@media (min-width:960px) {
+  .MuiContainer-maxWidthMd {
+    max-width: 960px;
+  }
+}
+@media (min-width:1280px) {
+  .MuiContainer-maxWidthLg {
+    max-width: 1280px;
+  }
+}
+@media (min-width:1920px) {
+  .MuiContainer-maxWidthXl {
+    max-width: 1920px;
+  }
+}
+  html {
+    box-sizing: border-box;
+    -webkit-font-smoothing: antialiased;
+    -moz-osx-font-smoothing: grayscale;
+  }
+  *, *::before, *::after {
+    box-sizing: inherit;
+  }
+  strong, b {
+    font-weight: 700;
+  }
+  body {
+    color: #263238;
+    margin: 0;
+    font-size: 0.875rem;
+    background: radial-gradient(circle farthest-side, #E4D0FA 0%, rgba(255, 0, 0, 0) 40%) top left/200% 100%, radial-gradient(circle farthest-side, #FCA3BE 0%, rgba(255, 0, 0, 0) 40%) top right/180% 150%;;
+    font-family: "Matter", "Lato", "Helvetica", sans-serif;
+    font-weight: 550;
+    line-height: 1.43;
+    background-color: #FFFFFF;
+    background-repeat: no-repeat;
+    background-attachment: fixed;
+  }
+@media print {
+  body {
+    background-color: #fff;
+  }
 }
+  body::backdrop {
+    background-color: #FFFFFF;
+  }
+  .MuiTypography-root {
+    margin: 0;
+  }
+  .MuiTypography-body2 {
+    font-size: 0.875rem;
+    font-family: "Matter", "Lato", "Helvetica", sans-serif;
+    font-weight: 550;
+    line-height: 1.43;
+  }
+  .MuiTypography-body1 {
+    font-size: 1rem;
+    font-family: "Matter", "Lato", "Helvetica", sans-serif;
+    font-weight: 550;
+    line-height: 1.5;
+  }
+  .MuiTypography-caption {
+    font-size: 0.75rem;
+    font-family: "Matter", "Lato", "Helvetica", sans-serif;
+    font-weight: 550;
+    line-height: 1.66;
+  }
+  .MuiTypography-button {
+    font-size: 0.875rem;
+    font-family: "Matter", "Lato", "Helvetica", sans-serif;
+    font-weight: 650;
+    line-height: 1.75;
+    text-transform: uppercase;
+  }
+  .MuiTypography-h1 {
+    font-size: 3.5rem;
+    font-family: "Matter", "Lato", "Helvetica", sans-serif;
+    font-weight: 450;
+    line-height: 1.167;
+  }
 @media (min-width:600px) {
   .MuiTypography-h1 {
     font-size: 4.7129rem;
   }
 }
 @media (min-width:960px) {
   .MuiTypography-h1 {
@@ -220,14 +315,42 @@
   }
   .MuiTypography-displayInline {
     display: inline;
   }
   .MuiTypography-displayBlock {
     display: block;
   }
+  .MuiBreadcrumbs-ol {
+    margin: 0;
+    display: flex;
+    padding: 0;
+    flex-wrap: wrap;
+    list-style: none;
+    align-items: center;
+  }
+  .MuiBreadcrumbs-separator {
+    display: flex;
+    margin-left: 8px;
+    user-select: none;
+    margin-right: 8px;
+  }
+  .jss12 {
+    margin: 5px;
+  }
+  .jss13 {
+    align-items: inherit;
+  }
+  .jss14 {
+    font-size: 18px;
+  }
+  .jss15 {
+    align-items: auto;
+    margin-left: 0.2em;
+    margin-right: 0.2em;
+  }
   .MuiPaper-root {
     color: #263238;
     transition: box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;
     background-color: #fff;
   }
   .MuiPaper-rounded {
     border-radius: 4px;
@@ -306,45 +429,14 @@
   }
   .MuiPaper-elevation23 {
     box-shadow: 0px 11px 14px -7px rgba(0,0,0,0.2),0px 23px 36px 3px rgba(0,0,0,0.14),0px 9px 44px 8px rgba(0,0,0,0.12);
   }
   .MuiPaper-elevation24 {
     box-shadow: 0px 11px 15px -7px rgba(0,0,0,0.2),0px 24px 38px 3px rgba(0,0,0,0.14),0px 9px 46px 8px rgba(0,0,0,0.12);
   }
-  .MuiToolbar-root {
-    display: flex;
-    position: relative;
-    align-items: center;
-  }
-  .MuiToolbar-gutters {
-    padding-left: 16px;
-    padding-right: 16px;
-  }
-@media (min-width:600px) {
-  .MuiToolbar-gutters {
-    padding-left: 24px;
-    padding-right: 24px;
-  }
-}
-  .MuiToolbar-regular {
-    min-height: 56px;
-  }
-@media (min-width:0px) and (orientation: landscape) {
-  .MuiToolbar-regular {
-    min-height: 48px;
-  }
-}
-@media (min-width:600px) {
-  .MuiToolbar-regular {
-    min-height: 64px;
-  }
-}
-  .MuiToolbar-dense {
-    min-height: 48px;
-  }
   .MuiAppBar-root {
     width: 100%;
     display: flex;
     z-index: 1100;
     box-sizing: border-box;
     flex-shrink: 0;
     flex-direction: column;
@@ -393,136 +485,60 @@
   .MuiAppBar-colorInherit {
     color: inherit;
   }
   .MuiAppBar-colorTransparent {
     color: inherit;
     background-color: transparent;
   }
-  .MuiBreadcrumbs-ol {
-    margin: 0;
-    display: flex;
-    padding: 0;
-    flex-wrap: wrap;
-    list-style: none;
-    align-items: center;
+
+  .jss11 {
+    height: 30px;
+    display: [object Object];
+    flex-grow: 1;
   }
-  .MuiBreadcrumbs-separator {
-    display: flex;
-    margin-left: 8px;
-    user-select: none;
-    margin-right: 8px;
+@media (min-width:0px) {
+  .jss11 {
+    display: none;
   }
-  .MuiContainer-root {
-    width: 100%;
+}
+@media (min-width:600px) {
+  .jss11 {
     display: block;
-    box-sizing: border-box;
-    margin-left: auto;
-    margin-right: auto;
+  }
+}
+  .MuiToolbar-root {
+    display: flex;
+    position: relative;
+    align-items: center;
+  }
+  .MuiToolbar-gutters {
     padding-left: 16px;
     padding-right: 16px;
   }
 @media (min-width:600px) {
-  .MuiContainer-root {
+  .MuiToolbar-gutters {
     padding-left: 24px;
     padding-right: 24px;
   }
 }
-  .MuiContainer-disableGutters {
-    padding-left: 0;
-    padding-right: 0;
-  }
-@media (min-width:600px) {
-  .MuiContainer-fixed {
-    max-width: 600px;
-  }
-}
-@media (min-width:960px) {
-  .MuiContainer-fixed {
-    max-width: 960px;
-  }
-}
-@media (min-width:1280px) {
-  .MuiContainer-fixed {
-    max-width: 1280px;
-  }
-}
-@media (min-width:1920px) {
-  .MuiContainer-fixed {
-    max-width: 1920px;
+  .MuiToolbar-regular {
+    min-height: 56px;
   }
-}
-@media (min-width:0px) {
-  .MuiContainer-maxWidthXs {
-    max-width: 444px;
+@media (min-width:0px) and (orientation: landscape) {
+  .MuiToolbar-regular {
+    min-height: 48px;
   }
 }
 @media (min-width:600px) {
-  .MuiContainer-maxWidthSm {
-    max-width: 600px;
-  }
-}
-@media (min-width:960px) {
-  .MuiContainer-maxWidthMd {
-    max-width: 960px;
-  }
-}
-@media (min-width:1280px) {
-  .MuiContainer-maxWidthLg {
-    max-width: 1280px;
-  }
-}
-@media (min-width:1920px) {
-  .MuiContainer-maxWidthXl {
-    max-width: 1920px;
-  }
-}
-  html {
-    box-sizing: border-box;
-    -webkit-font-smoothing: antialiased;
-    -moz-osx-font-smoothing: grayscale;
-  }
-  *, *::before, *::after {
-    box-sizing: inherit;
-  }
-  strong, b {
-    font-weight: 700;
-  }
-  body {
-    color: #263238;
-    margin: 0;
-    font-size: 0.875rem;
-    background: radial-gradient(circle farthest-side, #E4D0FA 0%, rgba(255, 0, 0, 0) 40%) top left/200% 100%, radial-gradient(circle farthest-side, #FCA3BE 0%, rgba(255, 0, 0, 0) 40%) top right/180% 150%;;
-    font-family: "Matter", "Lato", "Helvetica", sans-serif;
-    font-weight: 550;
-    line-height: 1.43;
-    background-color: #FFFFFF;
-    background-repeat: no-repeat;
-    background-attachment: fixed;
-  }
-@media print {
-  body {
-    background-color: #fff;
+  .MuiToolbar-regular {
+    min-height: 64px;
   }
 }
-  body::backdrop {
-    background-color: #FFFFFF;
-  }
-  .jss11 {
-    margin: 5px;
-  }
-  .jss12 {
-    align-items: inherit;
-  }
-  .jss13 {
-    font-size: 18px;
-  }
-  .jss14 {
-    align-items: auto;
-    margin-left: 0.2em;
-    margin-right: 0.2em;
+  .MuiToolbar-dense {
+    min-height: 48px;
   }
   .jss2 {
     width: 100%;
     diplay: flex;
   }
   .jss3 {
     color: black;
@@ -560,8 +576,8 @@
     position: relative;
     font-size: 3em;
     justify-self: flex-end;
   }
   .jss1 {
     padding-left: 64px;
     padding-right: 64px;
-  }</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><div class="jss2"><header class="MuiPaper-root MuiAppBar-root MuiAppBar-positionStatic MuiAppBar-colorPrimary jss3 MuiPaper-elevation4"><div class="MuiToolbar-root MuiToolbar-regular jss6 MuiToolbar-gutters"><div class="jss7"><img src="/static/FeatureForm_Logo_Full_Black.svg" height="30" alt="Featureform" component="div" nowrap="true" style="cursor:pointer" sx="[object Object]"/></div><div class="jss9"></div></div></header></div><div class="MuiContainer-root MuiContainer-maxWidthXl jss1"><div class="jss11"><nav class="MuiTypography-root MuiBreadcrumbs-root jss13 MuiTypography-body1 MuiTypography-colorTextSecondary" style="margin:0.25em" aria-label="breadcrumb"><ol class="MuiBreadcrumbs-ol jss12"><li class="MuiBreadcrumbs-li"><a href="/">Home</a></li><li aria-hidden="true" class="MuiBreadcrumbs-separator jss14"><style data-emotion="css vubbuv">.css-vubbuv{-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;width:1em;height:1em;display:inline-block;fill:currentColor;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;-webkit-transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;font-size:1.5rem;}</style><svg class="MuiSvgIcon-root MuiSvgIcon-fontSizeMedium css-vubbuv" focusable="false" aria-hidden="true" viewBox="0 0 24 24" data-testid="NavigateNextIcon"><path d="M10 6 8.59 7.41 13.17 12l-4.58 4.59L10 18l6-6z"></path></svg></li><li class="MuiBreadcrumbs-li"><b>404</b></li></ol></nav></div><div data-testid="notFoundId"><h1>404 Not Found :(</h1></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/404","query":{},"buildId":"XLqQwuMDcHNwRKV5unb2J","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+  }</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><div class="jss2"><header class="MuiPaper-root MuiAppBar-root MuiAppBar-positionStatic MuiAppBar-colorPrimary jss3 MuiPaper-elevation4"><div class="MuiToolbar-root MuiToolbar-regular jss6 MuiToolbar-gutters"><div class="jss7"><img class="MuiBox-root jss11" src="/static/FeatureForm_Logo_Full_Black.svg" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss9"></div></div></header></div><div class="MuiContainer-root MuiContainer-maxWidthXl jss1"><div class="jss12"><nav class="MuiTypography-root MuiBreadcrumbs-root jss14 MuiTypography-body1 MuiTypography-colorTextSecondary" style="margin:0.25em" aria-label="breadcrumb"><ol class="MuiBreadcrumbs-ol jss13"><li class="MuiBreadcrumbs-li"><a href="/">Home</a></li><li aria-hidden="true" class="MuiBreadcrumbs-separator jss15"><style data-emotion="css vubbuv">.css-vubbuv{-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;width:1em;height:1em;display:inline-block;fill:currentColor;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;-webkit-transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;font-size:1.5rem;}</style><svg class="MuiSvgIcon-root MuiSvgIcon-fontSizeMedium css-vubbuv" focusable="false" aria-hidden="true" viewBox="0 0 24 24" data-testid="NavigateNextIcon"><path d="M10 6 8.59 7.41 13.17 12l-4.58 4.59L10 18l6-6z"></path></svg></li><li class="MuiBreadcrumbs-li"><b>404</b></li></ol></nav></div><div data-testid="notFoundId"><h1>404 Not Found :(</h1></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/404","query":{},"buildId":"aZJnz9nRD9kOWLAxrQep6","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/[type]/[entity].html` & `featureform-1.8.1/src/featureform/dashboard/out/[type]/[entity].html`

 * *Files 1% similar despite different names*

```diff
@@ -1,41 +1,136 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-6ed703bc0f4dd2fe.js" defer=""></script><script src="/_next/static/chunks/framework-3412d1150754b2fb.js" defer=""></script><script src="/_next/static/chunks/main-2715d0c23f47c019.js" defer=""></script><script src="/_next/static/chunks/pages/_app-a764893ff9420ec0.js" defer=""></script><script src="/_next/static/chunks/pages/%5Btype%5D/%5Bentity%5D-b07f3c4463890639.js" defer=""></script><script src="/_next/static/XLqQwuMDcHNwRKV5unb2J/_buildManifest.js" defer=""></script><script src="/_next/static/XLqQwuMDcHNwRKV5unb2J/_ssgManifest.js" defer=""></script><style id="jss-server-side">.MuiTypography-root {
-  margin: 0;
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-6ed703bc0f4dd2fe.js" defer=""></script><script src="/_next/static/chunks/framework-3412d1150754b2fb.js" defer=""></script><script src="/_next/static/chunks/main-2715d0c23f47c019.js" defer=""></script><script src="/_next/static/chunks/pages/_app-535a9349f87f23c6.js" defer=""></script><script src="/_next/static/chunks/pages/%5Btype%5D/%5Bentity%5D-92ac9566fcd3bf59.js" defer=""></script><script src="/_next/static/aZJnz9nRD9kOWLAxrQep6/_buildManifest.js" defer=""></script><script src="/_next/static/aZJnz9nRD9kOWLAxrQep6/_ssgManifest.js" defer=""></script><style id="jss-server-side">.MuiContainer-root {
+  width: 100%;
+  display: block;
+  box-sizing: border-box;
+  margin-left: auto;
+  margin-right: auto;
+  padding-left: 16px;
+  padding-right: 16px;
 }
-.MuiTypography-body2 {
-  font-size: 0.875rem;
-  font-family: "Matter", "Lato", "Helvetica", sans-serif;
-  font-weight: 550;
-  line-height: 1.43;
-}
-.MuiTypography-body1 {
-  font-size: 1rem;
-  font-family: "Matter", "Lato", "Helvetica", sans-serif;
-  font-weight: 550;
-  line-height: 1.5;
-}
-.MuiTypography-caption {
-  font-size: 0.75rem;
-  font-family: "Matter", "Lato", "Helvetica", sans-serif;
-  font-weight: 550;
-  line-height: 1.66;
-}
-.MuiTypography-button {
-  font-size: 0.875rem;
-  font-family: "Matter", "Lato", "Helvetica", sans-serif;
-  font-weight: 650;
-  line-height: 1.75;
-  text-transform: uppercase;
-}
-.MuiTypography-h1 {
-  font-size: 3.5rem;
-  font-family: "Matter", "Lato", "Helvetica", sans-serif;
-  font-weight: 450;
-  line-height: 1.167;
+@media (min-width:600px) {
+  .MuiContainer-root {
+    padding-left: 24px;
+    padding-right: 24px;
+  }
+}
+  .MuiContainer-disableGutters {
+    padding-left: 0;
+    padding-right: 0;
+  }
+@media (min-width:600px) {
+  .MuiContainer-fixed {
+    max-width: 600px;
+  }
+}
+@media (min-width:960px) {
+  .MuiContainer-fixed {
+    max-width: 960px;
+  }
+}
+@media (min-width:1280px) {
+  .MuiContainer-fixed {
+    max-width: 1280px;
+  }
+}
+@media (min-width:1920px) {
+  .MuiContainer-fixed {
+    max-width: 1920px;
+  }
+}
+@media (min-width:0px) {
+  .MuiContainer-maxWidthXs {
+    max-width: 444px;
+  }
+}
+@media (min-width:600px) {
+  .MuiContainer-maxWidthSm {
+    max-width: 600px;
+  }
+}
+@media (min-width:960px) {
+  .MuiContainer-maxWidthMd {
+    max-width: 960px;
+  }
+}
+@media (min-width:1280px) {
+  .MuiContainer-maxWidthLg {
+    max-width: 1280px;
+  }
+}
+@media (min-width:1920px) {
+  .MuiContainer-maxWidthXl {
+    max-width: 1920px;
+  }
+}
+  html {
+    box-sizing: border-box;
+    -webkit-font-smoothing: antialiased;
+    -moz-osx-font-smoothing: grayscale;
+  }
+  *, *::before, *::after {
+    box-sizing: inherit;
+  }
+  strong, b {
+    font-weight: 700;
+  }
+  body {
+    color: #263238;
+    margin: 0;
+    font-size: 0.875rem;
+    background: radial-gradient(circle farthest-side, #E4D0FA 0%, rgba(255, 0, 0, 0) 40%) top left/200% 100%, radial-gradient(circle farthest-side, #FCA3BE 0%, rgba(255, 0, 0, 0) 40%) top right/180% 150%;;
+    font-family: "Matter", "Lato", "Helvetica", sans-serif;
+    font-weight: 550;
+    line-height: 1.43;
+    background-color: #FFFFFF;
+    background-repeat: no-repeat;
+    background-attachment: fixed;
+  }
+@media print {
+  body {
+    background-color: #fff;
+  }
 }
+  body::backdrop {
+    background-color: #FFFFFF;
+  }
+  .MuiTypography-root {
+    margin: 0;
+  }
+  .MuiTypography-body2 {
+    font-size: 0.875rem;
+    font-family: "Matter", "Lato", "Helvetica", sans-serif;
+    font-weight: 550;
+    line-height: 1.43;
+  }
+  .MuiTypography-body1 {
+    font-size: 1rem;
+    font-family: "Matter", "Lato", "Helvetica", sans-serif;
+    font-weight: 550;
+    line-height: 1.5;
+  }
+  .MuiTypography-caption {
+    font-size: 0.75rem;
+    font-family: "Matter", "Lato", "Helvetica", sans-serif;
+    font-weight: 550;
+    line-height: 1.66;
+  }
+  .MuiTypography-button {
+    font-size: 0.875rem;
+    font-family: "Matter", "Lato", "Helvetica", sans-serif;
+    font-weight: 650;
+    line-height: 1.75;
+    text-transform: uppercase;
+  }
+  .MuiTypography-h1 {
+    font-size: 3.5rem;
+    font-family: "Matter", "Lato", "Helvetica", sans-serif;
+    font-weight: 450;
+    line-height: 1.167;
+  }
 @media (min-width:600px) {
   .MuiTypography-h1 {
     font-size: 4.7129rem;
   }
 }
 @media (min-width:960px) {
   .MuiTypography-h1 {
@@ -220,14 +315,42 @@
   }
   .MuiTypography-displayInline {
     display: inline;
   }
   .MuiTypography-displayBlock {
     display: block;
   }
+  .MuiBreadcrumbs-ol {
+    margin: 0;
+    display: flex;
+    padding: 0;
+    flex-wrap: wrap;
+    list-style: none;
+    align-items: center;
+  }
+  .MuiBreadcrumbs-separator {
+    display: flex;
+    margin-left: 8px;
+    user-select: none;
+    margin-right: 8px;
+  }
+  .jss12 {
+    margin: 5px;
+  }
+  .jss13 {
+    align-items: inherit;
+  }
+  .jss14 {
+    font-size: 18px;
+  }
+  .jss15 {
+    align-items: auto;
+    margin-left: 0.2em;
+    margin-right: 0.2em;
+  }
   .MuiPaper-root {
     color: #263238;
     transition: box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;
     background-color: #fff;
   }
   .MuiPaper-rounded {
     border-radius: 4px;
@@ -306,45 +429,14 @@
   }
   .MuiPaper-elevation23 {
     box-shadow: 0px 11px 14px -7px rgba(0,0,0,0.2),0px 23px 36px 3px rgba(0,0,0,0.14),0px 9px 44px 8px rgba(0,0,0,0.12);
   }
   .MuiPaper-elevation24 {
     box-shadow: 0px 11px 15px -7px rgba(0,0,0,0.2),0px 24px 38px 3px rgba(0,0,0,0.14),0px 9px 46px 8px rgba(0,0,0,0.12);
   }
-  .MuiToolbar-root {
-    display: flex;
-    position: relative;
-    align-items: center;
-  }
-  .MuiToolbar-gutters {
-    padding-left: 16px;
-    padding-right: 16px;
-  }
-@media (min-width:600px) {
-  .MuiToolbar-gutters {
-    padding-left: 24px;
-    padding-right: 24px;
-  }
-}
-  .MuiToolbar-regular {
-    min-height: 56px;
-  }
-@media (min-width:0px) and (orientation: landscape) {
-  .MuiToolbar-regular {
-    min-height: 48px;
-  }
-}
-@media (min-width:600px) {
-  .MuiToolbar-regular {
-    min-height: 64px;
-  }
-}
-  .MuiToolbar-dense {
-    min-height: 48px;
-  }
   .MuiAppBar-root {
     width: 100%;
     display: flex;
     z-index: 1100;
     box-sizing: border-box;
     flex-shrink: 0;
     flex-direction: column;
@@ -393,136 +485,60 @@
   .MuiAppBar-colorInherit {
     color: inherit;
   }
   .MuiAppBar-colorTransparent {
     color: inherit;
     background-color: transparent;
   }
-  .MuiBreadcrumbs-ol {
-    margin: 0;
-    display: flex;
-    padding: 0;
-    flex-wrap: wrap;
-    list-style: none;
-    align-items: center;
+
+  .jss11 {
+    height: 30px;
+    display: [object Object];
+    flex-grow: 1;
   }
-  .MuiBreadcrumbs-separator {
-    display: flex;
-    margin-left: 8px;
-    user-select: none;
-    margin-right: 8px;
+@media (min-width:0px) {
+  .jss11 {
+    display: none;
   }
-  .MuiContainer-root {
-    width: 100%;
+}
+@media (min-width:600px) {
+  .jss11 {
     display: block;
-    box-sizing: border-box;
-    margin-left: auto;
-    margin-right: auto;
+  }
+}
+  .MuiToolbar-root {
+    display: flex;
+    position: relative;
+    align-items: center;
+  }
+  .MuiToolbar-gutters {
     padding-left: 16px;
     padding-right: 16px;
   }
 @media (min-width:600px) {
-  .MuiContainer-root {
+  .MuiToolbar-gutters {
     padding-left: 24px;
     padding-right: 24px;
   }
 }
-  .MuiContainer-disableGutters {
-    padding-left: 0;
-    padding-right: 0;
-  }
-@media (min-width:600px) {
-  .MuiContainer-fixed {
-    max-width: 600px;
-  }
-}
-@media (min-width:960px) {
-  .MuiContainer-fixed {
-    max-width: 960px;
-  }
-}
-@media (min-width:1280px) {
-  .MuiContainer-fixed {
-    max-width: 1280px;
-  }
-}
-@media (min-width:1920px) {
-  .MuiContainer-fixed {
-    max-width: 1920px;
+  .MuiToolbar-regular {
+    min-height: 56px;
   }
-}
-@media (min-width:0px) {
-  .MuiContainer-maxWidthXs {
-    max-width: 444px;
+@media (min-width:0px) and (orientation: landscape) {
+  .MuiToolbar-regular {
+    min-height: 48px;
   }
 }
 @media (min-width:600px) {
-  .MuiContainer-maxWidthSm {
-    max-width: 600px;
-  }
-}
-@media (min-width:960px) {
-  .MuiContainer-maxWidthMd {
-    max-width: 960px;
-  }
-}
-@media (min-width:1280px) {
-  .MuiContainer-maxWidthLg {
-    max-width: 1280px;
-  }
-}
-@media (min-width:1920px) {
-  .MuiContainer-maxWidthXl {
-    max-width: 1920px;
-  }
-}
-  html {
-    box-sizing: border-box;
-    -webkit-font-smoothing: antialiased;
-    -moz-osx-font-smoothing: grayscale;
-  }
-  *, *::before, *::after {
-    box-sizing: inherit;
-  }
-  strong, b {
-    font-weight: 700;
-  }
-  body {
-    color: #263238;
-    margin: 0;
-    font-size: 0.875rem;
-    background: radial-gradient(circle farthest-side, #E4D0FA 0%, rgba(255, 0, 0, 0) 40%) top left/200% 100%, radial-gradient(circle farthest-side, #FCA3BE 0%, rgba(255, 0, 0, 0) 40%) top right/180% 150%;;
-    font-family: "Matter", "Lato", "Helvetica", sans-serif;
-    font-weight: 550;
-    line-height: 1.43;
-    background-color: #FFFFFF;
-    background-repeat: no-repeat;
-    background-attachment: fixed;
-  }
-@media print {
-  body {
-    background-color: #fff;
+  .MuiToolbar-regular {
+    min-height: 64px;
   }
 }
-  body::backdrop {
-    background-color: #FFFFFF;
-  }
-  .jss11 {
-    margin: 5px;
-  }
-  .jss12 {
-    align-items: inherit;
-  }
-  .jss13 {
-    font-size: 18px;
-  }
-  .jss14 {
-    align-items: auto;
-    margin-left: 0.2em;
-    margin-right: 0.2em;
+  .MuiToolbar-dense {
+    min-height: 48px;
   }
   .jss2 {
     width: 100%;
     diplay: flex;
   }
   .jss3 {
     color: black;
@@ -560,8 +576,8 @@
     position: relative;
     font-size: 3em;
     justify-self: flex-end;
   }
   .jss1 {
     padding-left: 64px;
     padding-right: 64px;
-  }</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><div class="jss2"><header class="MuiPaper-root MuiAppBar-root MuiAppBar-positionStatic MuiAppBar-colorPrimary jss3 MuiPaper-elevation4"><div class="MuiToolbar-root MuiToolbar-regular jss6 MuiToolbar-gutters"><div class="jss7"><img src="/static/FeatureForm_Logo_Full_Black.svg" height="30" alt="Featureform" component="div" nowrap="true" style="cursor:pointer" sx="[object Object]"/></div><div class="jss9"></div></div></header></div><div class="MuiContainer-root MuiContainer-maxWidthXl jss1"><div class="jss11"><nav class="MuiTypography-root MuiBreadcrumbs-root jss13 MuiTypography-body1 MuiTypography-colorTextSecondary" style="margin:0.25em" aria-label="breadcrumb"><ol class="MuiBreadcrumbs-ol jss12"><li class="MuiBreadcrumbs-li"><a href="/">Home</a></li><li aria-hidden="true" class="MuiBreadcrumbs-separator jss14"><style data-emotion="css vubbuv">.css-vubbuv{-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;width:1em;height:1em;display:inline-block;fill:currentColor;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;-webkit-transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;font-size:1.5rem;}</style><svg class="MuiSvgIcon-root MuiSvgIcon-fontSizeMedium css-vubbuv" focusable="false" aria-hidden="true" viewBox="0 0 24 24" data-testid="NavigateNextIcon"><path d="M10 6 8.59 7.41 13.17 12l-4.58 4.59L10 18l6-6z"></path></svg></li><li class="MuiBreadcrumbs-li"><a href="/[type]">[type]</a></li><li aria-hidden="true" class="MuiBreadcrumbs-separator jss14"><style data-emotion="css vubbuv">.css-vubbuv{-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;width:1em;height:1em;display:inline-block;fill:currentColor;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;-webkit-transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;font-size:1.5rem;}</style><svg class="MuiSvgIcon-root MuiSvgIcon-fontSizeMedium css-vubbuv" focusable="false" aria-hidden="true" viewBox="0 0 24 24" data-testid="NavigateNextIcon"><path d="M10 6 8.59 7.41 13.17 12l-4.58 4.59L10 18l6-6z"></path></svg></li><li class="MuiBreadcrumbs-li"><b>[entity]</b></li></ol></nav></div><div><div data-testid="notFoundId"><h1>404 Not Found :(</h1></div></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/[type]/[entity]","query":{},"buildId":"XLqQwuMDcHNwRKV5unb2J","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+  }</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><div class="jss2"><header class="MuiPaper-root MuiAppBar-root MuiAppBar-positionStatic MuiAppBar-colorPrimary jss3 MuiPaper-elevation4"><div class="MuiToolbar-root MuiToolbar-regular jss6 MuiToolbar-gutters"><div class="jss7"><img class="MuiBox-root jss11" src="/static/FeatureForm_Logo_Full_Black.svg" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss9"></div></div></header></div><div class="MuiContainer-root MuiContainer-maxWidthXl jss1"><div class="jss12"><nav class="MuiTypography-root MuiBreadcrumbs-root jss14 MuiTypography-body1 MuiTypography-colorTextSecondary" style="margin:0.25em" aria-label="breadcrumb"><ol class="MuiBreadcrumbs-ol jss13"><li class="MuiBreadcrumbs-li"><a href="/">Home</a></li><li aria-hidden="true" class="MuiBreadcrumbs-separator jss15"><style data-emotion="css vubbuv">.css-vubbuv{-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;width:1em;height:1em;display:inline-block;fill:currentColor;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;-webkit-transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;font-size:1.5rem;}</style><svg class="MuiSvgIcon-root MuiSvgIcon-fontSizeMedium css-vubbuv" focusable="false" aria-hidden="true" viewBox="0 0 24 24" data-testid="NavigateNextIcon"><path d="M10 6 8.59 7.41 13.17 12l-4.58 4.59L10 18l6-6z"></path></svg></li><li class="MuiBreadcrumbs-li"><a href="/[type]">[type]</a></li><li aria-hidden="true" class="MuiBreadcrumbs-separator jss15"><style data-emotion="css vubbuv">.css-vubbuv{-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;width:1em;height:1em;display:inline-block;fill:currentColor;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;-webkit-transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;font-size:1.5rem;}</style><svg class="MuiSvgIcon-root MuiSvgIcon-fontSizeMedium css-vubbuv" focusable="false" aria-hidden="true" viewBox="0 0 24 24" data-testid="NavigateNextIcon"><path d="M10 6 8.59 7.41 13.17 12l-4.58 4.59L10 18l6-6z"></path></svg></li><li class="MuiBreadcrumbs-li"><b>[entity]</b></li></ol></nav></div><div><div data-testid="notFoundId"><h1>404 Not Found :(</h1></div></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/[type]/[entity]","query":{},"buildId":"aZJnz9nRD9kOWLAxrQep6","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/[type].html` & `featureform-1.8.1/src/featureform/dashboard/out/[type].html`

 * *Files 3% similar despite different names*

```diff
@@ -1,41 +1,136 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-6ed703bc0f4dd2fe.js" defer=""></script><script src="/_next/static/chunks/framework-3412d1150754b2fb.js" defer=""></script><script src="/_next/static/chunks/main-2715d0c23f47c019.js" defer=""></script><script src="/_next/static/chunks/pages/_app-a764893ff9420ec0.js" defer=""></script><script src="/_next/static/chunks/pages/%5Btype%5D-751a928da9d524e9.js" defer=""></script><script src="/_next/static/XLqQwuMDcHNwRKV5unb2J/_buildManifest.js" defer=""></script><script src="/_next/static/XLqQwuMDcHNwRKV5unb2J/_ssgManifest.js" defer=""></script><style id="jss-server-side">.MuiTypography-root {
-  margin: 0;
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-6ed703bc0f4dd2fe.js" defer=""></script><script src="/_next/static/chunks/framework-3412d1150754b2fb.js" defer=""></script><script src="/_next/static/chunks/main-2715d0c23f47c019.js" defer=""></script><script src="/_next/static/chunks/pages/_app-535a9349f87f23c6.js" defer=""></script><script src="/_next/static/chunks/pages/%5Btype%5D-1354c91ed8b0be2c.js" defer=""></script><script src="/_next/static/aZJnz9nRD9kOWLAxrQep6/_buildManifest.js" defer=""></script><script src="/_next/static/aZJnz9nRD9kOWLAxrQep6/_ssgManifest.js" defer=""></script><style id="jss-server-side">.MuiContainer-root {
+  width: 100%;
+  display: block;
+  box-sizing: border-box;
+  margin-left: auto;
+  margin-right: auto;
+  padding-left: 16px;
+  padding-right: 16px;
 }
-.MuiTypography-body2 {
-  font-size: 0.875rem;
-  font-family: "Matter", "Lato", "Helvetica", sans-serif;
-  font-weight: 550;
-  line-height: 1.43;
-}
-.MuiTypography-body1 {
-  font-size: 1rem;
-  font-family: "Matter", "Lato", "Helvetica", sans-serif;
-  font-weight: 550;
-  line-height: 1.5;
-}
-.MuiTypography-caption {
-  font-size: 0.75rem;
-  font-family: "Matter", "Lato", "Helvetica", sans-serif;
-  font-weight: 550;
-  line-height: 1.66;
-}
-.MuiTypography-button {
-  font-size: 0.875rem;
-  font-family: "Matter", "Lato", "Helvetica", sans-serif;
-  font-weight: 650;
-  line-height: 1.75;
-  text-transform: uppercase;
-}
-.MuiTypography-h1 {
-  font-size: 3.5rem;
-  font-family: "Matter", "Lato", "Helvetica", sans-serif;
-  font-weight: 450;
-  line-height: 1.167;
+@media (min-width:600px) {
+  .MuiContainer-root {
+    padding-left: 24px;
+    padding-right: 24px;
+  }
+}
+  .MuiContainer-disableGutters {
+    padding-left: 0;
+    padding-right: 0;
+  }
+@media (min-width:600px) {
+  .MuiContainer-fixed {
+    max-width: 600px;
+  }
+}
+@media (min-width:960px) {
+  .MuiContainer-fixed {
+    max-width: 960px;
+  }
+}
+@media (min-width:1280px) {
+  .MuiContainer-fixed {
+    max-width: 1280px;
+  }
+}
+@media (min-width:1920px) {
+  .MuiContainer-fixed {
+    max-width: 1920px;
+  }
+}
+@media (min-width:0px) {
+  .MuiContainer-maxWidthXs {
+    max-width: 444px;
+  }
+}
+@media (min-width:600px) {
+  .MuiContainer-maxWidthSm {
+    max-width: 600px;
+  }
+}
+@media (min-width:960px) {
+  .MuiContainer-maxWidthMd {
+    max-width: 960px;
+  }
+}
+@media (min-width:1280px) {
+  .MuiContainer-maxWidthLg {
+    max-width: 1280px;
+  }
+}
+@media (min-width:1920px) {
+  .MuiContainer-maxWidthXl {
+    max-width: 1920px;
+  }
+}
+  html {
+    box-sizing: border-box;
+    -webkit-font-smoothing: antialiased;
+    -moz-osx-font-smoothing: grayscale;
+  }
+  *, *::before, *::after {
+    box-sizing: inherit;
+  }
+  strong, b {
+    font-weight: 700;
+  }
+  body {
+    color: #263238;
+    margin: 0;
+    font-size: 0.875rem;
+    background: radial-gradient(circle farthest-side, #E4D0FA 0%, rgba(255, 0, 0, 0) 40%) top left/200% 100%, radial-gradient(circle farthest-side, #FCA3BE 0%, rgba(255, 0, 0, 0) 40%) top right/180% 150%;;
+    font-family: "Matter", "Lato", "Helvetica", sans-serif;
+    font-weight: 550;
+    line-height: 1.43;
+    background-color: #FFFFFF;
+    background-repeat: no-repeat;
+    background-attachment: fixed;
+  }
+@media print {
+  body {
+    background-color: #fff;
+  }
 }
+  body::backdrop {
+    background-color: #FFFFFF;
+  }
+  .MuiTypography-root {
+    margin: 0;
+  }
+  .MuiTypography-body2 {
+    font-size: 0.875rem;
+    font-family: "Matter", "Lato", "Helvetica", sans-serif;
+    font-weight: 550;
+    line-height: 1.43;
+  }
+  .MuiTypography-body1 {
+    font-size: 1rem;
+    font-family: "Matter", "Lato", "Helvetica", sans-serif;
+    font-weight: 550;
+    line-height: 1.5;
+  }
+  .MuiTypography-caption {
+    font-size: 0.75rem;
+    font-family: "Matter", "Lato", "Helvetica", sans-serif;
+    font-weight: 550;
+    line-height: 1.66;
+  }
+  .MuiTypography-button {
+    font-size: 0.875rem;
+    font-family: "Matter", "Lato", "Helvetica", sans-serif;
+    font-weight: 650;
+    line-height: 1.75;
+    text-transform: uppercase;
+  }
+  .MuiTypography-h1 {
+    font-size: 3.5rem;
+    font-family: "Matter", "Lato", "Helvetica", sans-serif;
+    font-weight: 450;
+    line-height: 1.167;
+  }
 @media (min-width:600px) {
   .MuiTypography-h1 {
     font-size: 4.7129rem;
   }
 }
 @media (min-width:960px) {
   .MuiTypography-h1 {
@@ -220,14 +315,42 @@
   }
   .MuiTypography-displayInline {
     display: inline;
   }
   .MuiTypography-displayBlock {
     display: block;
   }
+  .MuiBreadcrumbs-ol {
+    margin: 0;
+    display: flex;
+    padding: 0;
+    flex-wrap: wrap;
+    list-style: none;
+    align-items: center;
+  }
+  .MuiBreadcrumbs-separator {
+    display: flex;
+    margin-left: 8px;
+    user-select: none;
+    margin-right: 8px;
+  }
+  .jss12 {
+    margin: 5px;
+  }
+  .jss13 {
+    align-items: inherit;
+  }
+  .jss14 {
+    font-size: 18px;
+  }
+  .jss15 {
+    align-items: auto;
+    margin-left: 0.2em;
+    margin-right: 0.2em;
+  }
   .MuiPaper-root {
     color: #263238;
     transition: box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;
     background-color: #fff;
   }
   .MuiPaper-rounded {
     border-radius: 4px;
@@ -306,45 +429,14 @@
   }
   .MuiPaper-elevation23 {
     box-shadow: 0px 11px 14px -7px rgba(0,0,0,0.2),0px 23px 36px 3px rgba(0,0,0,0.14),0px 9px 44px 8px rgba(0,0,0,0.12);
   }
   .MuiPaper-elevation24 {
     box-shadow: 0px 11px 15px -7px rgba(0,0,0,0.2),0px 24px 38px 3px rgba(0,0,0,0.14),0px 9px 46px 8px rgba(0,0,0,0.12);
   }
-  .MuiToolbar-root {
-    display: flex;
-    position: relative;
-    align-items: center;
-  }
-  .MuiToolbar-gutters {
-    padding-left: 16px;
-    padding-right: 16px;
-  }
-@media (min-width:600px) {
-  .MuiToolbar-gutters {
-    padding-left: 24px;
-    padding-right: 24px;
-  }
-}
-  .MuiToolbar-regular {
-    min-height: 56px;
-  }
-@media (min-width:0px) and (orientation: landscape) {
-  .MuiToolbar-regular {
-    min-height: 48px;
-  }
-}
-@media (min-width:600px) {
-  .MuiToolbar-regular {
-    min-height: 64px;
-  }
-}
-  .MuiToolbar-dense {
-    min-height: 48px;
-  }
   .MuiAppBar-root {
     width: 100%;
     display: flex;
     z-index: 1100;
     box-sizing: border-box;
     flex-shrink: 0;
     flex-direction: column;
@@ -393,136 +485,60 @@
   .MuiAppBar-colorInherit {
     color: inherit;
   }
   .MuiAppBar-colorTransparent {
     color: inherit;
     background-color: transparent;
   }
-  .MuiBreadcrumbs-ol {
-    margin: 0;
-    display: flex;
-    padding: 0;
-    flex-wrap: wrap;
-    list-style: none;
-    align-items: center;
+
+  .jss11 {
+    height: 30px;
+    display: [object Object];
+    flex-grow: 1;
   }
-  .MuiBreadcrumbs-separator {
-    display: flex;
-    margin-left: 8px;
-    user-select: none;
-    margin-right: 8px;
+@media (min-width:0px) {
+  .jss11 {
+    display: none;
   }
-  .MuiContainer-root {
-    width: 100%;
+}
+@media (min-width:600px) {
+  .jss11 {
     display: block;
-    box-sizing: border-box;
-    margin-left: auto;
-    margin-right: auto;
+  }
+}
+  .MuiToolbar-root {
+    display: flex;
+    position: relative;
+    align-items: center;
+  }
+  .MuiToolbar-gutters {
     padding-left: 16px;
     padding-right: 16px;
   }
 @media (min-width:600px) {
-  .MuiContainer-root {
+  .MuiToolbar-gutters {
     padding-left: 24px;
     padding-right: 24px;
   }
 }
-  .MuiContainer-disableGutters {
-    padding-left: 0;
-    padding-right: 0;
-  }
-@media (min-width:600px) {
-  .MuiContainer-fixed {
-    max-width: 600px;
-  }
-}
-@media (min-width:960px) {
-  .MuiContainer-fixed {
-    max-width: 960px;
-  }
-}
-@media (min-width:1280px) {
-  .MuiContainer-fixed {
-    max-width: 1280px;
-  }
-}
-@media (min-width:1920px) {
-  .MuiContainer-fixed {
-    max-width: 1920px;
+  .MuiToolbar-regular {
+    min-height: 56px;
   }
-}
-@media (min-width:0px) {
-  .MuiContainer-maxWidthXs {
-    max-width: 444px;
+@media (min-width:0px) and (orientation: landscape) {
+  .MuiToolbar-regular {
+    min-height: 48px;
   }
 }
 @media (min-width:600px) {
-  .MuiContainer-maxWidthSm {
-    max-width: 600px;
-  }
-}
-@media (min-width:960px) {
-  .MuiContainer-maxWidthMd {
-    max-width: 960px;
-  }
-}
-@media (min-width:1280px) {
-  .MuiContainer-maxWidthLg {
-    max-width: 1280px;
-  }
-}
-@media (min-width:1920px) {
-  .MuiContainer-maxWidthXl {
-    max-width: 1920px;
-  }
-}
-  html {
-    box-sizing: border-box;
-    -webkit-font-smoothing: antialiased;
-    -moz-osx-font-smoothing: grayscale;
-  }
-  *, *::before, *::after {
-    box-sizing: inherit;
-  }
-  strong, b {
-    font-weight: 700;
-  }
-  body {
-    color: #263238;
-    margin: 0;
-    font-size: 0.875rem;
-    background: radial-gradient(circle farthest-side, #E4D0FA 0%, rgba(255, 0, 0, 0) 40%) top left/200% 100%, radial-gradient(circle farthest-side, #FCA3BE 0%, rgba(255, 0, 0, 0) 40%) top right/180% 150%;;
-    font-family: "Matter", "Lato", "Helvetica", sans-serif;
-    font-weight: 550;
-    line-height: 1.43;
-    background-color: #FFFFFF;
-    background-repeat: no-repeat;
-    background-attachment: fixed;
-  }
-@media print {
-  body {
-    background-color: #fff;
+  .MuiToolbar-regular {
+    min-height: 64px;
   }
 }
-  body::backdrop {
-    background-color: #FFFFFF;
-  }
-  .jss11 {
-    margin: 5px;
-  }
-  .jss12 {
-    align-items: inherit;
-  }
-  .jss13 {
-    font-size: 18px;
-  }
-  .jss14 {
-    align-items: auto;
-    margin-left: 0.2em;
-    margin-right: 0.2em;
+  .MuiToolbar-dense {
+    min-height: 48px;
   }
   .jss2 {
     width: 100%;
     diplay: flex;
   }
   .jss3 {
     color: black;
@@ -560,8 +576,8 @@
     position: relative;
     font-size: 3em;
     justify-self: flex-end;
   }
   .jss1 {
     padding-left: 64px;
     padding-right: 64px;
-  }</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><div class="jss2"><header class="MuiPaper-root MuiAppBar-root MuiAppBar-positionStatic MuiAppBar-colorPrimary jss3 MuiPaper-elevation4"><div class="MuiToolbar-root MuiToolbar-regular jss6 MuiToolbar-gutters"><div class="jss7"><img src="/static/FeatureForm_Logo_Full_Black.svg" height="30" alt="Featureform" component="div" nowrap="true" style="cursor:pointer" sx="[object Object]"/></div><div class="jss9"></div></div></header></div><div class="MuiContainer-root MuiContainer-maxWidthXl jss1"><div class="jss11"><nav class="MuiTypography-root MuiBreadcrumbs-root jss13 MuiTypography-body1 MuiTypography-colorTextSecondary" style="margin:0.25em" aria-label="breadcrumb"><ol class="MuiBreadcrumbs-ol jss12"><li class="MuiBreadcrumbs-li"><a href="/">Home</a></li><li aria-hidden="true" class="MuiBreadcrumbs-separator jss14"><style data-emotion="css vubbuv">.css-vubbuv{-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;width:1em;height:1em;display:inline-block;fill:currentColor;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;-webkit-transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;font-size:1.5rem;}</style><svg class="MuiSvgIcon-root MuiSvgIcon-fontSizeMedium css-vubbuv" focusable="false" aria-hidden="true" viewBox="0 0 24 24" data-testid="NavigateNextIcon"><path d="M10 6 8.59 7.41 13.17 12l-4.58 4.59L10 18l6-6z"></path></svg></li><li class="MuiBreadcrumbs-li"><b>[type]</b></li></ol></nav></div><div><div data-testid="notFoundId"><h1>404 Not Found :(</h1></div></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/[type]","query":{},"buildId":"XLqQwuMDcHNwRKV5unb2J","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+  }</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><div class="jss2"><header class="MuiPaper-root MuiAppBar-root MuiAppBar-positionStatic MuiAppBar-colorPrimary jss3 MuiPaper-elevation4"><div class="MuiToolbar-root MuiToolbar-regular jss6 MuiToolbar-gutters"><div class="jss7"><img class="MuiBox-root jss11" src="/static/FeatureForm_Logo_Full_Black.svg" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss9"></div></div></header></div><div class="MuiContainer-root MuiContainer-maxWidthXl jss1"><div class="jss12"><nav class="MuiTypography-root MuiBreadcrumbs-root jss14 MuiTypography-body1 MuiTypography-colorTextSecondary" style="margin:0.25em" aria-label="breadcrumb"><ol class="MuiBreadcrumbs-ol jss13"><li class="MuiBreadcrumbs-li"><a href="/">Home</a></li><li aria-hidden="true" class="MuiBreadcrumbs-separator jss15"><style data-emotion="css vubbuv">.css-vubbuv{-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;width:1em;height:1em;display:inline-block;fill:currentColor;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;-webkit-transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;font-size:1.5rem;}</style><svg class="MuiSvgIcon-root MuiSvgIcon-fontSizeMedium css-vubbuv" focusable="false" aria-hidden="true" viewBox="0 0 24 24" data-testid="NavigateNextIcon"><path d="M10 6 8.59 7.41 13.17 12l-4.58 4.59L10 18l6-6z"></path></svg></li><li class="MuiBreadcrumbs-li"><b>[type]</b></li></ol></nav></div><div><div data-testid="notFoundId"><h1>404 Not Found :(</h1></div></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/[type]","query":{},"buildId":"aZJnz9nRD9kOWLAxrQep6","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/Jopdpwd8wB7tMgkcaVnsn/_buildManifest.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/Jopdpwd8wB7tMgkcaVnsn/_buildManifest.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/XLqQwuMDcHNwRKV5unb2J/_buildManifest.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/aZJnz9nRD9kOWLAxrQep6/_buildManifest.js`

 * *Files 11% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,16 @@
 self.__BUILD_MANIFEST = {
     __rewrites: {
         beforeFiles: [],
         afterFiles: [],
         fallback: []
     },
-    "/": ["static/chunks/pages/index-c2ee5b1681e97e4b.js"],
+    "/": ["static/chunks/pages/index-942ec646d90d2132.js"],
     "/404": ["static/chunks/pages/404-baaca4b2f4acc755.js"],
     "/_error": ["static/chunks/pages/_error-3f70f2d61eb8c6dd.js"],
     "/connections": ["static/chunks/pages/connections-1d67ba61869dece6.js"],
+    "/query": ["static/chunks/pages/query-9193959c04ff1e72.js"],
     "/search": ["static/chunks/pages/search-175858e61ba25631.js"],
-    "/[type]": ["static/chunks/pages/[type]-751a928da9d524e9.js"],
-    "/[type]/[entity]": ["static/chunks/pages/[type]/[entity]-b07f3c4463890639.js"],
-    sortedPages: ["/", "/404", "/_app", "/_error", "/connections", "/search", "/[type]", "/[type]/[entity]"]
+    "/[type]": ["static/chunks/pages/[type]-1354c91ed8b0be2c.js"],
+    "/[type]/[entity]": ["static/chunks/pages/[type]/[entity]-92ac9566fcd3bf59.js"],
+    sortedPages: ["/", "/404", "/_app", "/_error", "/connections", "/query", "/search", "/[type]", "/[type]/[entity]"]
 }, self.__BUILD_MANIFEST_CB && self.__BUILD_MANIFEST_CB()
```

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/72a30a16.5298cad0ba46633d.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/72a30a16.5298cad0ba46633d.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/7679.34cabcdac6ff42f5.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/7679.34cabcdac6ff42f5.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/7856.43cc2293f00befb0.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/7856.43cc2293f00befb0.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/ad7f724d.b238476ad0e6f6d2.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/ad7f724d.b238476ad0e6f6d2.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/framework-3412d1150754b2fb.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/framework-3412d1150754b2fb.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/main-2715d0c23f47c019.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/main-2715d0c23f47c019.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/pages/_app-a764893ff9420ec0.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/pages/_app-535a9349f87f23c6.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -41814,29 +41814,29 @@
         },
         62082: function(a) {
             a.exports = ["#{street_name} #{building_number}"]
         },
         91009: function(a) {
             a.exports = ["#{street}"]
         },
-        45793: function(a) {
+        14125: function(a) {
             a.exports = ["Adaptive", "Advanced", "Ameliorated", "Assimilated", "Automated", "Balanced", "Business-focused", "Centralized", "Cloned", "Compatible", "Configurable", "Cross-group", "Cross-platform", "Customer-focused", "Customizable", "Decentralized", "De-engineered", "Devolved", "Digitized", "Distributed", "Diverse", "Down-sized", "Enhanced", "Enterprise-wide", "Ergonomic", "Exclusive", "Expanded", "Extended", "Face to face", "Focused", "Front-line", "Fully-configurable", "Function-based", "Fundamental", "Future-proofed", "Grass-roots", "Horizontal", "Implemented", "Innovative", "Integrated", "Intuitive", "Inverse", "Managed", "Mandatory", "Monitored", "Multi-channelled", "Multi-lateral", "Multi-layered", "Multi-tiered", "Networked", "Object-based", "Open-architected", "Open-source", "Operative", "Optimized", "Optional", "Organic", "Organized", "Persevering", "Persistent", "Phased", "Polarised", "Pre-emptive", "Proactive", "Profit-focused", "Profound", "Programmable", "Progressive", "Public-key", "Quality-focused", "Reactive", "Realigned", "Re-contextualized", "Re-engineered", "Reduced", "Reverse-engineered", "Right-sized", "Robust", "Seamless", "Secured", "Self-enabling", "Sharable", "Stand-alone", "Streamlined", "Switchable", "Synchronised", "Synergistic", "Synergized", "Team-oriented", "Total", "Triple-buffered", "Universal", "Up-sized", "Upgradable", "User-centric", "User-friendly", "Versatile", "Virtual", "Visionary", "Vision-oriented"]
         },
         26390: function(a) {
             a.exports = ["clicks-and-mortar", "value-added", "vertical", "proactive", "robust", "revolutionary", "scalable", "leading-edge", "innovative", "intuitive", "strategic", "e-business", "mission-critical", "sticky", "one-to-one", "24/7", "end-to-end", "global", "B2B", "B2C", "granular", "frictionless", "virtual", "viral", "dynamic", "24/365", "best-of-breed", "killer", "magnetic", "bleeding-edge", "web-enabled", "interactive", "dot-com", "sexy", "back-end", "real-time", "efficient", "front-end", "distributed", "seamless", "extensible", "turn-key", "world-class", "open-source", "cross-platform", "cross-media", "synergistic", "bricks-and-clicks", "out-of-the-box", "enterprise", "integrated", "impactful", "wireless", "transparent", "next-generation", "cutting-edge", "user-centric", "visionary", "customized", "ubiquitous", "plug-and-play", "collaborative", "compelling", "holistic", "rich", "synergies", "web-readiness", "paradigms", "markets", "partnerships", "infrastructures", "platforms", "initiatives", "channels", "eyeballs", "communities", "ROI", "solutions", "e-tailers", "e-services", "action-items", "portals", "niches", "technologies", "content", "vortals", "supply-chains", "convergence", "relationships", "architectures", "interfaces", "e-markets", "e-commerce", "systems", "bandwidth", "infomediaries", "models", "mindshare", "deliverables", "users", "schemas", "networks", "applications", "metrics", "e-business", "functionalities", "experiences", "web services", "methodologies"]
         },
         25359: function(a) {
             a.exports = ["implement", "utilize", "integrate", "streamline", "optimize", "evolve", "transform", "embrace", "enable", "orchestrate", "leverage", "reinvent", "aggregate", "architect", "enhance", "incentivize", "morph", "empower", "envisioneer", "monetize", "harness", "facilitate", "seize", "disintermediate", "synergize", "strategize", "deploy", "brand", "grow", "target", "syndicate", "synthesize", "deliver", "mesh", "incubate", "engage", "maximize", "benchmark", "expedite", "reintermediate", "whiteboard", "visualize", "repurpose", "innovate", "scale", "unleash", "drive", "extend", "engineer", "revolutionize", "generate", "exploit", "transition", "e-enable", "iterate", "cultivate", "matrix", "productize", "redefine", "recontextualize"]
         },
         30226: function(a) {
             a.exports = ["24 hour", "24/7", "3rd generation", "4th generation", "5th generation", "6th generation", "actuating", "analyzing", "asymmetric", "asynchronous", "attitude-oriented", "background", "bandwidth-monitored", "bi-directional", "bifurcated", "bottom-line", "clear-thinking", "client-driven", "client-server", "coherent", "cohesive", "composite", "context-sensitive", "contextually-based", "content-based", "dedicated", "demand-driven", "didactic", "directional", "discrete", "disintermediate", "dynamic", "eco-centric", "empowering", "encompassing", "even-keeled", "executive", "explicit", "exuding", "fault-tolerant", "foreground", "fresh-thinking", "full-range", "global", "grid-enabled", "heuristic", "high-level", "holistic", "homogeneous", "human-resource", "hybrid", "impactful", "incremental", "intangible", "interactive", "intermediate", "leading edge", "local", "logistical", "maximized", "methodical", "mission-critical", "mobile", "modular", "motivating", "multimedia", "multi-state", "multi-tasking", "national", "needs-based", "neutral", "next generation", "non-volatile", "object-oriented", "optimal", "optimizing", "radical", "real-time", "reciprocal", "regional", "responsive", "scalable", "secondary", "solution-oriented", "stable", "static", "systematic", "systemic", "system-worthy", "tangible", "tertiary", "transitional", "uniform", "upward-trending", "user-facing", "value-added", "web-enabled", "well-modulated", "zero administration", "zero defect", "zero tolerance"]
         },
         76534: function(a, b, c) {
             var d = {};
-            a.exports = d, d.suffix = c(55681), d.adjective = c(45793), d.descriptor = c(30226), d.noun = c(78485), d.bs_verb = c(25359), d.bs_noun = c(26390), d.name = c(13042)
+            a.exports = d, d.suffix = c(55681), d.adjective = c(14125), d.descriptor = c(30226), d.noun = c(78485), d.bs_verb = c(25359), d.bs_noun = c(26390), d.name = c(13042)
         },
         13042: function(a) {
             a.exports = ["#{Name.last_name} #{suffix}", "#{Name.last_name} #{suffix}", "#{Name.man_last_name} a #{Name.man_last_name} #{suffix}"]
         },
         78485: function(a) {
             a.exports = ["ability", "access", "adapter", "algorithm", "alliance", "analyzer", "application", "approach", "architecture", "archive", "artificial intelligence", "array", "attitude", "benchmark", "budgetary management", "capability", "capacity", "challenge", "circuit", "collaboration", "complexity", "concept", "conglomeration", "contingency", "core", "customer loyalty", "database", "data-warehouse", "definition", "emulation", "encoding", "encryption", "extranet", "firmware", "flexibility", "focus group", "forecast", "frame", "framework", "function", "functionalities", "Graphic Interface", "groupware", "Graphical User Interface", "hardware", "help-desk", "hierarchy", "hub", "implementation", "info-mediaries", "infrastructure", "initiative", "installation", "instruction set", "interface", "internet solution", "intranet", "knowledge user", "knowledge base", "local area network", "leverage", "matrices", "matrix", "methodology", "middleware", "migration", "model", "moderator", "monitoring", "moratorium", "neural-net", "open architecture", "open system", "orchestration", "paradigm", "parallelism", "policy", "portal", "pricing structure", "process improvement", "product", "productivity", "project", "projection", "protocol", "secured line", "service-desk", "software", "solution", "standardization", "strategy", "structure", "success", "superstructure", "support", "synergy", "system engine", "task-force", "throughput", "time-frame", "toolset", "utilisation", "website", "workforce"]
         },
@@ -42417,20 +42417,20 @@
             a.exports = ["implement", "utilize", "integrate", "streamline", "optimize", "evolve", "transform", "embrace", "enable", "orchestrate", "leverage", "reinvent", "aggregate", "architect", "enhance", "incentivize", "morph", "empower", "envisioneer", "monetize", "harness", "facilitate", "seize", "disintermediate", "synergize", "strategize", "deploy", "brand", "grow", "target", "syndicate", "synthesize", "deliver", "mesh", "incubate", "engage", "maximize", "benchmark", "expedite", "reintermediate", "whiteboard", "visualize", "repurpose", "innovate", "scale", "unleash", "drive", "extend", "engineer", "revolutionize", "generate", "exploit", "transition", "e-enable", "iterate", "cultivate", "matrix", "productize", "redefine", "recontextualize"]
         },
         19699: function(a) {
             a.exports = ["24 hour", "24/7", "3rd generation", "4th generation", "5th generation", "6th generation", "actuating", "analyzing", "asymmetric", "asynchronous", "attitude-oriented", "background", "bandwidth-monitored", "bi-directional", "bifurcated", "bottom-line", "clear-thinking", "client-driven", "client-server", "coherent", "cohesive", "composite", "context-sensitive", "contextually-based", "content-based", "dedicated", "demand-driven", "didactic", "directional", "discrete", "disintermediate", "dynamic", "eco-centric", "empowering", "encompassing", "even-keeled", "executive", "explicit", "exuding", "fault-tolerant", "foreground", "fresh-thinking", "full-range", "global", "grid-enabled", "heuristic", "high-level", "holistic", "homogeneous", "human-resource", "hybrid", "impactful", "incremental", "intangible", "interactive", "intermediate", "leading edge", "local", "logistical", "maximized", "methodical", "mission-critical", "mobile", "modular", "motivating", "multimedia", "multi-state", "multi-tasking", "national", "needs-based", "neutral", "next generation", "non-volatile", "object-oriented", "optimal", "optimizing", "radical", "real-time", "reciprocal", "regional", "responsive", "scalable", "secondary", "solution-oriented", "stable", "static", "systematic", "systemic", "system-worthy", "tangible", "tertiary", "transitional", "uniform", "upward-trending", "user-facing", "value-added", "web-enabled", "well-modulated", "zero administration", "zero defect", "zero tolerance"]
         },
         11206: function(a, b, c) {
             var d = {};
-            a.exports = d, d.suffix = c(29872), d.adjective = c(68395), d.descriptor = c(19699), d.noun = c(98964), d.bs_verb = c(96144), d.bs_adjective = c(97688), d.bs_noun = c(39738), d.name = c(23159)
+            a.exports = d, d.suffix = c(29872), d.adjective = c(68395), d.descriptor = c(19699), d.noun = c(2015), d.bs_verb = c(96144), d.bs_adjective = c(97688), d.bs_noun = c(39738), d.name = c(23159)
         },
         23159: function(a) {
             a.exports = ["#{Name.last_name} #{suffix}", "#{Name.last_name}-#{Name.last_name}", "#{Name.last_name}, #{Name.last_name} and #{Name.last_name}"]
         },
-        98964: function(a) {
+        2015: function(a) {
             a.exports = ["ability", "access", "adapter", "algorithm", "alliance", "analyzer", "application", "approach", "architecture", "archive", "artificial intelligence", "array", "attitude", "benchmark", "budgetary management", "capability", "capacity", "challenge", "circuit", "collaboration", "complexity", "concept", "conglomeration", "contingency", "core", "customer loyalty", "database", "data-warehouse", "definition", "emulation", "encoding", "encryption", "extranet", "firmware", "flexibility", "focus group", "forecast", "frame", "framework", "function", "functionalities", "Graphic Interface", "groupware", "Graphical User Interface", "hardware", "help-desk", "hierarchy", "hub", "implementation", "info-mediaries", "infrastructure", "initiative", "installation", "instruction set", "interface", "internet solution", "intranet", "knowledge user", "knowledge base", "local area network", "leverage", "matrices", "matrix", "methodology", "middleware", "migration", "model", "moderator", "monitoring", "moratorium", "neural-net", "open architecture", "open system", "orchestration", "paradigm", "parallelism", "policy", "portal", "pricing structure", "process improvement", "product", "productivity", "project", "projection", "protocol", "secured line", "service-desk", "software", "solution", "standardization", "strategy", "structure", "success", "superstructure", "support", "synergy", "system engine", "task-force", "throughput", "time-frame", "toolset", "utilisation", "website", "workforce"]
         },
         29872: function(a) {
             a.exports = ["Inc", "and Sons", "LLC", "Group"]
         },
         77848: function(a) {
             a.exports = ["utf8_unicode_ci", "utf8_general_ci", "utf8_bin", "ascii_bin", "ascii_general_ci", "cp1250_bin", "cp1250_general_ci"]
@@ -69234,15 +69234,15 @@
                     this.set(d[0], d[1])
                 }
             }
             i.prototype.clear = d, i.prototype.delete = e, i.prototype.get = f, i.prototype.has = g, i.prototype.set = h, a.exports = i
         },
         38407: function(a, b, c) {
             var d = c(27040),
-                e = c(14125),
+                e = c(61362),
                 f = c(82117),
                 g = c(67518),
                 h = c(54705);
 
             function i(a) {
                 var b = -1,
                     c = null == a ? 0 : a.length;
@@ -70054,15 +70054,15 @@
             }
         },
         27040: function(a) {
             a.exports = function() {
                 this.__data__ = [], this.size = 0
             }
         },
-        14125: function(a, b, c) {
+        61362: function(a, b, c) {
             var d = c(18470),
                 e = Array.prototype.splice;
             a.exports = function(a) {
                 var b = this.__data__,
                     c = d(b, a);
                 return !(c < 0) && (c == b.length - 1 ? b.pop() : e.call(b, c, 1), --this.size, !0)
             }
@@ -87150,85 +87150,41 @@
             var g = d.default.createContext(null);
             b.GlobalLayoutRouterContext = g
         },
         71393: function(a, b, c) {
             "use strict";
             c.r(b), c.d(b, {
                 MyApp: function() {
-                    return at
+                    return au
                 },
                 ThemeWrapper: function() {
-                    return av
+                    return aw
                 },
                 default: function() {
-                    return aw
+                    return ax
                 },
                 views: function() {
-                    return au
+                    return av
                 }
             });
             var d, e = c(26042),
                 f = c(69396),
                 g = c(85893),
-                h = c(67294);
-            c(2989);
-            var i = c(14416),
-                j = function(a) {
-                    var b = a.children,
-                        c = a.store;
-                    return (0, g.jsx)(i.zt, {
-                        store: c,
-                        children: b
-                    })
-                },
-                k = c(49830),
-                l = c(14890);
-            c(67617), c(88802);
-            var m = c(16332),
-                n = c(93432),
-                o = c(5378);
-            c(83023);
-            var p = (0, k.oM)({
-                    name: "homePageSections",
-                    initialState: {
-                        features: [{
-                            type: "TrainingSet",
-                            disabled: !1
-                        }, {
-                            type: "Feature",
-                            disabled: !1
-                        }, {
-                            type: "Entity",
-                            disabled: !1
-                        }, {
-                            type: "Label",
-                            disabled: !1
-                        }, {
-                            type: "Model",
-                            disabled: !1
-                        }, {
-                            type: "Source",
-                            disabled: !1
-                        }, {
-                            type: "Provider",
-                            disabled: !1
-                        }, {
-                            type: "User",
-                            disabled: !1
-                        }, ]
-                    }
-                }),
-                q = p.reducer,
+                h = c(43832),
+                i = c(75834),
+                j = c(41120),
+                k = c(13457),
+                l = c(67294),
+                m = c(13824),
+                n = c(7885),
+                o = c(37958),
+                p = c(41664),
+                q = c.n(p),
                 r = c(11163),
-                s = c(41120),
-                t = c(41664),
-                u = c.n(t),
-                v = c(7885),
-                w = c(37958),
-                x = (0, s.Z)(function(a) {
+                s = (0, j.Z)(function() {
                     return {
                         root: {
                             margin: 5
                         },
                         ol: {
                             alignItems: "inherit"
                         },
@@ -87238,73 +87194,158 @@
                         separator: {
                             marginLeft: "0.2em",
                             marginRight: "0.2em",
                             alignItems: "auto"
                         }
                     }
                 }),
-                y = function() {
-                    for (var a = x(), b = (0, r.useRouter)().asPath.split("?").shift().split("/"); b.length > 0 && 0 === b[0].length;) b.shift();
+                t = function() {
+                    for (var a = s(), b = (0, r.useRouter)().asPath.split("?").shift().split("/"); b.length > 0 && 0 === b[0].length;) b.shift();
                     var c = function(a) {
                             return a ? a[0].toUpperCase() + a.slice(1).toLowerCase() : ""
                         },
                         d = function(a, b) {
                             return a + "/" + b
                         };
                     return (0, g.jsx)("div", {
                         className: a.root,
-                        children: b.length > 0 ? (0, g.jsxs)(v.Z, {
+                        children: b.length > 0 ? (0, g.jsxs)(n.Z, {
                             className: a.breadcrumbs,
                             style: {
                                 margin: "0.25em"
                             },
                             "aria-label": "breadcrumb",
-                            separator: (0, g.jsx)(w.Z, {
+                            separator: (0, g.jsx)(o.Z, {
                                 fontSize: "medium"
                             }),
                             classes: {
                                 separator: a.separator,
                                 ol: a.ol
                             },
-                            children: [(0, g.jsx)(u(), {
+                            children: [(0, g.jsx)(q(), {
                                 href: "/",
                                 children: "Home"
                             }), b.map(function(a, e) {
-                                return (0, g.jsx)(u(), {
+                                return (0, g.jsx)(q(), {
                                     href: "/" + b.slice(0, e + 1).reduce(d),
                                     children: e === b.length - 1 ? (0, g.jsx)("b", {
                                         children: c(a)
                                     }) : c(a)
                                 }, "link-".concat(e))
                             })]
                         }) : (0, g.jsx)("div", {})
                     })
                 },
-                z = y,
-                A = (0, k.oM)({
+                u = t,
+                v = c(49830),
+                w = c(14890),
+                x = (0, v.oM)({
                     name: "breadCrumbs",
                     initialState: [{
                         path: []
                     }, ]
                 }),
-                B = A.reducer;
+                y = x.reducer;
+            c(14731);
+            var z = c(48271);
             c(75457);
-            var C = c(50462);
-            c(88277);
-            var D = c(75820),
-                E = c(70603),
-                F = c(22318),
-                G = c(59122),
-                H = c(89849),
-                I = (0, s.Z)(function(a) {
+            var A = c(50462),
+                B = c(70603),
+                C = c(85333),
+                D = c(94054),
+                E = c(33841),
+                F = c(44355),
+                G = c(86507),
+                H = c(14416),
+                I = (0, v.oM)({
+                    name: "aggregateDropdown",
+                    initialState: {
+                        aggregates: ["avg", "avg", "avg"]
+                    },
+                    reducers: {
+                        changeAggregate: function(a, b) {
+                            a.aggregates[b.payload.graph] = b.payload.aggregate
+                        }
+                    }
+                }),
+                J = I.actions.changeAggregate,
+                K = I.reducer,
+                L = [{
+                    label: "Average",
+                    value: "avg"
+                }, {
+                    label: "Sum",
+                    value: "sum"
+                }, {
+                    label: "Minimum",
+                    value: "min"
+                }, {
+                    label: "Maximum",
+                    value: "max"
+                }, ],
+                M = function(a) {
+                    return {
+                        changeAggregate: function(b, c) {
+                            return a(J({
+                                graph: b,
+                                aggregate: c
+                            }))
+                        }
+                    }
+                };
+            (0, H.$j)(function(a) {
+                return {
+                    aggregates: a.aggregates
+                }
+            }, M)(function(a) {
+                var b = a.graph,
+                    c = a.aggregates,
+                    d = a.changeAggregate,
+                    e = (0, B.Z)(l.useState(c.aggregates[b]), 2),
+                    f = e[0],
+                    h = e[1],
+                    i = function(a) {
+                        h(a.target.value), d(0, a.target.value)
+                    };
+                return (0, g.jsx)("div", {
+                    children: (0, g.jsx)(C.Z, {
+                        sx: {
+                            minWidth: 120
+                        },
+                        children: (0, g.jsxs)(D.Z, {
+                            fullWidth: !0,
+                            children: [(0, g.jsx)(E.Z, {
+                                id: "demo-simple-select-label",
+                                children: "Aggregation Select"
+                            }), (0, g.jsx)(G.Z, {
+                                labelId: "demo-simple-select-label",
+                                id: "demo-simple-select",
+                                value: f,
+                                label: "Aggregation Select",
+                                onChange: i,
+                                children: L.map(function(a) {
+                                    return (0, g.jsx)(F.Z, {
+                                        value: a.value,
+                                        children: a.label
+                                    }, a.label)
+                                })
+                            })]
+                        })
+                    })
+                })
+            });
+            var N = c(59122),
+                O = c(22318),
+                P = c(89849),
+                Q = (0, j.Z)(function() {
                     return {
                         dateRangeView: {}
                     }
                 }),
-                J = [{
+                R = [{
                     value: 0,
                     scaledValue: 262e4,
                     label: "~"
                 }, {
                     value: 25,
                     scaledValue: 262800,
                     label: "6mo"
@@ -87333,243 +87374,201 @@
                     scaledValue: 1,
                     label: "1m"
                 }, {
                     value: 200,
                     scaledValue: 0,
                     label: "now"
                 }, ],
-                K = function(a) {
-                    return [L(a[0]), L(a[1])]
+                S = function(a) {
+                    return [T(a[0]), T(a[1])]
                 },
-                L = function(a) {
+                T = function(a) {
                     if (void 0 !== a) {
                         var b = Math.floor(a / 25),
-                            c = J[b],
+                            c = R[b],
                             d = a % 25;
-                        return 0 === d ? c.scaledValue : d * ((J[b + 1].scaledValue - c.scaledValue) / 25) + c.scaledValue
+                        return 0 === d ? c.scaledValue : d * ((R[b + 1].scaledValue - c.scaledValue) / 25) + c.scaledValue
                     }
                 },
-                M = function(a) {
+                U = function(a) {
                     return {
                         changeTime: function(b) {
-                            return a((0, H.X)({
+                            return a((0, P.X)({
                                 timeRange: b
                             }))
                         }
                     }
                 };
-            (0, i.$j)(function(a) {
+            (0, H.$j)(function(a) {
                 return {
                     timeRange: a.timeRange
                 }
-            }, M)(function(a) {
+            }, U)(function(a) {
                 var b = a.changeTime,
-                    c = I(),
-                    d = (0, E.Z)(h.useState([175, 200]), 2),
+                    c = Q(),
+                    d = (0, B.Z)(l.useState([175, 200]), 2),
                     e = d[0],
                     f = d[1],
-                    i = function(a, b) {
+                    h = function(a, b) {
                         f(b)
                     },
-                    j = function(a, c) {
-                        f(c), b(K(c.map(function(a) {
+                    i = function(a, c) {
+                        f(c), b(S(c.map(function(a) {
                             return a
                         })))
                     };
                 return (0, g.jsxs)("div", {
-                    children: [(0, g.jsx)(G.Z, {
+                    children: [(0, g.jsx)(N.Z, {
                         style: {
                             maxWidth: 500
                         },
                         value: e,
                         min: 0,
                         step: 1,
                         max: 200,
                         valueLabelFormat: function(a) {
                             var b;
                             return (0, g.jsx)("div", {
                                 children: b = a
                             })
                         },
-                        marks: J,
-                        scale: K,
-                        onChange: i,
-                        onChangeCommitted: j,
+                        marks: R,
+                        scale: S,
+                        onChange: h,
+                        onChangeCommitted: i,
                         valueLabelDisplay: "auto"
                     }), (0, g.jsx)("div", {
                         className: c.dateRangeView,
-                        children: K(e).map(function(a, b) {
+                        children: S(e).map(function(a, b) {
                             var c;
-                            return (0, g.jsx)(F.Z, {
+                            return (0, g.jsx)(O.Z, {
                                 variant: "body2",
                                 children: (c = a, new Date(Date.now() - 6e4 * c).toUTCString())
                             }, b)
                         })
                     })]
                 })
             });
-            var N = c(85333),
-                O = c(33841),
-                P = c(44355),
-                Q = c(94054),
-                R = c(86507),
-                S = (0, k.oM)({
-                    name: "aggregateDropdown",
-                    initialState: {
-                        aggregates: ["avg", "avg", "avg"]
-                    },
-                    reducers: {
-                        changeAggregate: function(a, b) {
-                            a.aggregates[b.payload.graph] = b.payload.aggregate
-                        }
-                    }
-                }),
-                T = S.actions.changeAggregate,
-                U = S.reducer,
-                V = [{
-                    label: "Average",
-                    value: "avg"
-                }, {
-                    label: "Sum",
-                    value: "sum"
-                }, {
-                    label: "Minimum",
-                    value: "min"
-                }, {
-                    label: "Maximum",
-                    value: "max"
-                }, ],
-                W = function(a) {
-                    return {
-                        changeAggregate: function(b, c) {
-                            return a(T({
-                                graph: b,
-                                aggregate: c
-                            }))
-                        }
-                    }
-                };
-            (0, i.$j)(function(a) {
-                return {
-                    aggregates: a.aggregates
-                }
-            }, W)(function(a) {
-                var b = a.graph,
-                    c = a.aggregates,
-                    d = a.changeAggregate,
-                    e = (0, E.Z)(h.useState(c.aggregates[b]), 2),
-                    f = e[0],
-                    i = e[1],
-                    j = function(a) {
-                        i(a.target.value), d(0, a.target.value)
-                    };
-                return (0, g.jsx)("div", {
-                    children: (0, g.jsx)(N.Z, {
-                        sx: {
-                            minWidth: 120
-                        },
-                        children: (0, g.jsxs)(Q.Z, {
-                            fullWidth: !0,
-                            children: [(0, g.jsx)(O.Z, {
-                                id: "demo-simple-select-label",
-                                children: "Aggregation Select"
-                            }), (0, g.jsx)(R.Z, {
-                                labelId: "demo-simple-select-label",
-                                id: "demo-simple-select",
-                                value: f,
-                                label: "Aggregation Select",
-                                onChange: j,
-                                children: V.map(function(a) {
-                                    return (0, g.jsx)(P.Z, {
-                                        value: a.value,
-                                        children: a.label
-                                    }, a.label)
-                                })
-                            })]
-                        })
-                    })
-                })
-            });
-            var X, Y = c(47568),
-                Z = c(14924),
-                $ = c(34051),
-                _ = c.n($),
-                aa = (0, k.hg)("metricsSelect/fetchMetrics", (X = (0, Y.Z)(_().mark(function a(b, c) {
+            var V, W = c(47568),
+                X = c(14924),
+                Y = c(34051),
+                Z = c.n(Y),
+                $ = (0, v.hg)("metricsSelect/fetchMetrics", (V = (0, W.Z)(Z().mark(function a(b, c) {
                     var d, e, f, g;
-                    return _().wrap(function(a) {
+                    return Z().wrap(function(a) {
                         for (;;) switch (a.prev = a.next) {
                             case 0:
                                 return d = b.api, e = c.signal, f = "", a.next = 4, d.fetchMetrics(f, e);
                             case 4:
                                 return g = a.sent, a.abrupt("return", g);
                             case 6:
                             case "end":
                                 return a.stop()
                         }
                     }, a)
                 })), function(a, b) {
-                    return X.apply(this, arguments)
+                    return V.apply(this, arguments)
                 }), {
                     condition: function(a, b) {
-                        if (a.api, (0, b.getState)().metricsSelect.loading) return !1
+                        if ((0, b.getState)().metricsSelect.loading) return !1
                     }
                 }),
-                ab = (0, k.oM)({
+                _ = (0, v.oM)({
                     name: "metricsSelect",
                     initialState: {
                         instances: [],
                         metrics: 0
                     },
                     reducers: {
                         modifyInstances: function(a, b) {
                             a.instances = b.payload.instances
                         },
                         modifyMetrics: function(a, b) {
                             a.metrics = b.payload.selection
                         }
                     },
-                    extraReducers: (d = {}, (0, Z.Z)(d, aa.pending, function(a, b) {
+                    extraReducers: (d = {}, (0, X.Z)(d, $.pending, function(a, b) {
                         var c = b.meta.requestId;
                         a.requestId = c, a.resources = null, a.loading = !0, a.failed = !1
-                    }), (0, Z.Z)(d, aa.fulfilled, function(a, b) {
+                    }), (0, X.Z)(d, $.fulfilled, function(a, b) {
                         b.meta.requestId === a.requestId && (a.resources = b.payload.data, a.loading = !1, a.failed = !1)
-                    }), (0, Z.Z)(d, aa.rejected, function(a, b) {
+                    }), (0, X.Z)(d, $.rejected, function(a, b) {
                         b.meta.requestId === a.requestId && (a.loading = !1, a.failed = !0)
                     }), d)
                 });
-            ab.actions.modifyInstances, ab.actions.modifyMetrics;
-            var ac = ab.reducer;
-            c(14731);
-            var ad = c(48271),
-                ae = (0, l.UY)({
-                    resourceList: m.ZP,
-                    selectedVariant: n.ZP,
-                    selectedTags: o.ZP,
-                    homePageSections: q,
-                    breadCrumbs: B,
-                    entityPage: C.Z,
-                    searchResults: D.ZP,
-                    timeRange: H.Z,
-                    metricsSelect: ac,
-                    connectionStatus: ad.Z,
-                    aggregates: U
+            _.actions.modifyInstances, _.actions.modifyMetrics;
+            var aa = _.reducer;
+            c(83023);
+            var ab = (0, v.oM)({
+                    name: "homePageSections",
+                    initialState: {
+                        features: [{
+                            type: "TrainingSet",
+                            disabled: !1
+                        }, {
+                            type: "Feature",
+                            disabled: !1
+                        }, {
+                            type: "Entity",
+                            disabled: !1
+                        }, {
+                            type: "Label",
+                            disabled: !1
+                        }, {
+                            type: "Model",
+                            disabled: !1
+                        }, {
+                            type: "Source",
+                            disabled: !1
+                        }, {
+                            type: "Provider",
+                            disabled: !1
+                        }, {
+                            type: "User",
+                            disabled: !1
+                        }, ]
+                    }
                 }),
-                af = (0, k.xC)({
-                    reducer: ae
+                ac = ab.reducer;
+            c(67617), c(88802);
+            var ad = c(16332),
+                ae = c(5378),
+                af = c(93432);
+            c(88277);
+            var ag = c(75820),
+                ah = (0, w.UY)({
+                    resourceList: ad.ZP,
+                    selectedVariant: af.ZP,
+                    selectedTags: ae.ZP,
+                    homePageSections: ac,
+                    breadCrumbs: y,
+                    entityPage: A.Z,
+                    searchResults: ag.ZP,
+                    timeRange: P.Z,
+                    metricsSelect: aa,
+                    connectionStatus: z.Z,
+                    aggregates: K
+                }),
+                ai = (0, v.xC)({
+                    reducer: ah
                 }),
-                ag = af,
-                ah = c(75834),
-                ai = c(48535),
-                aj = c(13457),
-                ak = c(13824);
-            c(66660);
-            var al = c(45258),
-                am = c(28358),
-                an = (c(17812), c(82067), c(85639), c(38396), c(7169)),
-                ao = (0, s.Z)(function(a) {
+                aj = ai,
+                ak = function(a) {
+                    var b = a.children,
+                        c = a.store;
+                    return (0, g.jsx)(H.zt, {
+                        store: c,
+                        children: b
+                    })
+                },
+                al = c(28889),
+                am = c(45258),
+                an = (c(17812), c(38396), c(85639), c(28358)),
+                ao = (c(82067), c(7169)),
+                ap = (0, j.Z)(function(a) {
                     return {
                         root: {
                             diplay: "flex",
                             width: "100%"
                         },
                         appbar: {
                             background: "transparent",
@@ -87608,114 +87607,114 @@
                             padding: "1em",
                             width: "auto",
                             justifySelf: "flex-end"
                         }
                     }
                 });
 
-            function ap() {
+            function aq() {
                 var a = (0, r.useRouter)(),
-                    b = ao(),
-                    c = (0, E.Z)(h.useState(!1), 2),
+                    b = ap(),
+                    c = (0, B.Z)(l.useState(!1), 2),
                     d = c[0],
                     e = c[1],
-                    f = (0, E.Z)(h.useState(null), 2),
-                    i = f[0],
-                    j = f[1];
-                (0, h.useEffect)(function() {
+                    f = (0, B.Z)(l.useState(null), 2),
+                    h = f[0],
+                    i = f[1];
+                (0, l.useEffect)(function() {
                     "/" !== a.pathname ? e(!0) : e(!1)
                 }, [a]);
-                var k = function(b) {
+                var j = function(b) {
                     null == b || b.preventDefault(), a.push("/")
                 };
                 return (0, g.jsx)("div", {
                     className: b.root,
-                    children: (0, g.jsx)(al.Z, {
+                    children: (0, g.jsx)(am.Z, {
                         position: "static",
                         className: b.appbar,
-                        children: (0, g.jsxs)(am.Z, {
+                        children: (0, g.jsxs)(an.Z, {
                             className: b.toolbar,
                             children: [(0, g.jsx)("div", {
                                 className: b.title,
-                                children: (0, g.jsx)("img", {
+                                children: (0, g.jsx)(al.Z, {
+                                    component: "img",
                                     src: "/static/FeatureForm_Logo_Full_Black.svg",
-                                    height: 30,
                                     alt: "Featureform",
-                                    onClick: k,
-                                    component: "div",
-                                    nowrap: "true",
+                                    onClick: j,
                                     style: {
-                                        cursor: "pointer"
+                                        cursor: "pointer",
+                                        nowrap: !0
                                     },
                                     sx: {
+                                        height: 30,
                                         flexGrow: 1,
                                         display: {
                                             xs: "none",
                                             sm: "block"
                                         }
                                     }
                                 })
                             }), (0, g.jsxs)("div", {
                                 className: b.toolbarRight,
-                                children: [d && (0, g.jsx)(an.Z, {
+                                children: [d && (0, g.jsx)(ao.Z, {
                                     className: b.searchBar,
                                     homePage: !1
                                 }), !1]
                             })]
                         })
                     })
                 })
             }
-            var aq = c(43832);
-            c(99520);
-            var ar = new ak.ZP,
-                as = (0, s.Z)(function(a) {
+            c(2989);
+            var ar = c(48535),
+                as = new m.ZP,
+                at = (0, j.Z)(function(a) {
                     return {
                         pageContainer: {
                             paddingLeft: a.spacing(8),
                             paddingRight: a.spacing(8)
                         }
                     }
                 }),
-                at = function(a) {
+                au = function(a) {
                     var b = a.Component,
                         c = a.pageProps,
-                        d = as();
-                    return (0, g.jsx)(h.StrictMode, {
-                        children: (0, g.jsx)(j, {
-                            store: ag,
-                            children: (0, g.jsxs)(av, {
-                                children: [(0, g.jsx)(ap, {
+                        d = at();
+                    return (0, g.jsx)(l.StrictMode, {
+                        children: (0, g.jsx)(ak, {
+                            store: aj,
+                            children: (0, g.jsxs)(aw, {
+                                children: [(0, g.jsx)(aq, {
                                     className: d.topbar
-                                }), (0, g.jsxs)(aq.Z, {
+                                }), (0, g.jsxs)(h.Z, {
                                     maxWidth: "xl",
                                     className: d.root,
                                     classes: {
                                         maxWidthXl: d.pageContainer
                                     },
-                                    children: [(0, g.jsx)(z, {}), (0, g.jsx)(b, (0, f.Z)((0, e.Z)({}, c), {
-                                        api: ar
+                                    children: [(0, g.jsx)(u, {}), (0, g.jsx)(b, (0, f.Z)((0, e.Z)({}, c), {
+                                        api: as
                                     }))]
                                 })]
                             })
                         })
                     })
                 },
-                au = {
+                av = {
                     RESOURCE_LIST: "ResourceList",
                     EMPTY: "Empty"
                 },
-                av = function(a) {
+                aw = function(a) {
                     var b = a.children;
-                    return (0, g.jsxs)(aj.Z, {
-                        theme: ai.ZP,
-                        children: [(0, g.jsx)(ah.ZP, {}), b]
+                    return (0, g.jsxs)(k.Z, {
+                        theme: ar.ZP,
+                        children: [(0, g.jsx)(i.ZP, {}), b]
                     })
                 },
-                aw = at
+                ax = au
         },
         21286: function(a, b, c) {
             "use strict";
             c.d(b, {
                 Z: function() {
                     return h
                 }
@@ -87963,15 +87962,15 @@
                             return a.json()
                         }).catch(function(a) {
                             console.error(a)
                         })
                     }
                 }, {
                     key: "fetchVariantSearchStub",
-                    value: function(a) {
+                    value: function() {
                         return fetch("/data/lists/search_results_example.json", {
                             headers: {
                                 "Content-Type": "application/json"
                             }
                         }).then(function(a) {
                             return a.json().then(function(a) {
                                 return {
@@ -88061,69 +88060,72 @@
             c.d(b, {
                 Z: function() {
                     return B
                 }
             });
             var d = c(85893),
                 e = c(67294),
-                f = c(48271),
-                g = c(51438),
-                h = c(52951),
-                i = "http://localhost:9090/api/v1",
-                j = function() {
+                f = c(14416),
+                g = c(13824),
+                h = c(51438),
+                i = c(52951),
+                j = "http://localhost:9090/api/v1",
+                k = function() {
                     function a() {
-                        (0, g.Z)(this, a)
+                        (0, h.Z)(this, a)
                     }
-                    return (0, h.Z)(a, [{
+                    return (0, i.Z)(a, [{
                         key: "checkStatus",
                         value: function() {
-                            return fetch("".concat(i, "/label/__name__/values"), {
+                            return fetch("".concat(j, "/label/__name__/values"), {
                                 headers: {
                                     "Content-Type": "application/json"
                                 }
                             }).then(function(a) {
                                 a.json()
                             }).catch(function(a) {
                                 console.error(a)
                             })
                         }
                     }, {
                         key: "fetchInstances",
                         value: function() {
-                            var a = "".concat(i, "/label/__name__/values");
+                            var a = "".concat(j, "/label/__name__/values");
                             return fetch(a, {
                                 headers: {
                                     "Content-Type": "application/json"
                                 }
                             }).then(function(a) {
                                 return a.json()
                             }).catch(function(a) {
                                 console.error(a)
                             })
                         }
                     }, {
                         key: "fetchMetrics",
-                        value: function(a) {
-                            var b = "".concat(i, "/metadata");
-                            return fetch(b, {
+                        value: function() {
+                            var a = "".concat(j, "/metadata");
+                            return fetch(a, {
                                 headers: {
                                     "Content-Type": "application/json"
                                 }
                             }).then(function(a) {
                                 return a.json()
                             }).catch(function(a) {
                                 console.error(a)
                             })
                         }
                     }]), a
                 }(),
-                k = c(41120),
-                l = c(18463),
-                m = c(22318),
-                n = (0, k.Z)(function(a, b) {
+                l = c(48271),
+                m = c(41749),
+                n = c(18463),
+                o = c(41120),
+                p = c(22318),
+                q = (0, o.Z)(function(a) {
                     return {
                         root: {
                             padding: a.spacing(2),
                             width: "100%",
                             height: "100%"
                         },
                         card: {
@@ -88137,98 +88139,95 @@
                         },
                         title: {
                             fontSize: "2em",
                             color: "black"
                         }
                     }
                 }),
-                o = function(a) {
+                r = function(a) {
                     var b = a.detail,
-                        c = n(b.current_status);
+                        c = q(b.current_status);
                     return (0, d.jsx)("div", {
                         className: c.root,
-                        children: (0, d.jsx)(l.Z, {
+                        children: (0, d.jsx)(n.Z, {
                             className: c.card,
                             elevation: 0,
                             children: (0, d.jsxs)("div", {
-                                children: [(0, d.jsx)(m.Z, {
+                                children: [(0, d.jsx)(p.Z, {
                                     className: c.title,
                                     variant: "h5",
                                     children: (0, d.jsx)("b", {
                                         children: b.title
                                     })
-                                }), (0, d.jsx)(m.Z, {
+                                }), (0, d.jsx)(p.Z, {
                                     variant: "body1",
                                     children: b.current_status
                                 })]
                             })
                         })
                     })
                 },
-                p = o,
-                q = c(41749),
-                r = function(a) {
+                s = r,
+                t = function(a) {
                     var b = a.sections;
                     return (0, d.jsx)("div", {
-                        children: (0, d.jsx)(q.Z, {
+                        children: (0, d.jsx)(m.Z, {
                             container: !0,
                             justifyContent: "center",
                             lg: 12,
                             children: b.map(function(a, b) {
-                                return (0, d.jsx)(q.Z, {
+                                return (0, d.jsx)(m.Z, {
                                     item: !0,
                                     xs: 4,
                                     lg: 2,
-                                    children: (0, d.jsx)(p, {
+                                    children: (0, d.jsx)(s, {
                                         detail: a,
                                         id: b
                                     }, "tile-".concat(b))
                                 }, "tile-grid-".concat(b))
                             })
                         })
                     })
                 },
-                s = r,
-                t = function(a) {
+                u = t,
+                v = function(a) {
                     var b = a.statuses,
                         c = [];
                     return Object.entries(b).forEach(function(a) {
                         c.push({
                             title: a[0],
                             current_status: a[1]
                         })
-                    }), (0, d.jsx)(s, {
+                    }), (0, d.jsx)(u, {
                         sections: c
                     })
                 },
-                u = t,
-                v = c(13824),
-                w = c(14416),
+                w = v,
                 x = function(a) {
                     return {
                         fetchStatus: function(b, c) {
-                            return a((0, f.U)({
+                            return a((0, l.U)({
                                 api: b,
                                 resource: c
                             }))
                         }
                     }
                 },
-                y = new j,
-                z = new v.ZP,
+                y = new k,
+                z = new g.ZP,
                 A = function(a) {
                     var b = a.connectionStatus,
                         c = a.fetchStatus;
                     return (0, e.useEffect)(function() {
                         c(y, "metrics"), c(z, "resources")
-                    }, [c]), (0, d.jsx)(u, {
+                    }, [c]), (0, d.jsx)(w, {
                         statuses: b.statuses
                     })
                 },
-                B = (0, w.$j)(function(a) {
+                B = (0, f.$j)(function(a) {
                     return {
                         connectionStatus: a.connectionStatus
                     }
                 }, x)(A)
         },
         48271: function(a, b, c) {
             "use strict";
@@ -88239,21 +88238,21 @@
             });
             var d, e, f = c(47568),
                 g = c(14924),
                 h = c(34051),
                 i = c.n(h),
                 j = c(49830),
                 k = (0, j.hg)("metricsSelect/fetchStatus", (e = (0, f.Z)(i().mark(function a(b, c) {
-                    var d, e, f, g;
+                    var d, e, f;
                     return i().wrap(function(a) {
                         for (;;) switch (a.prev = a.next) {
                             case 0:
-                                return d = b.api, e = b.resource, f = c.signal, a.next = 3, d.checkStatus(f);
+                                return d = b.api, e = c.signal, a.next = 3, d.checkStatus(e);
                             case 3:
-                                return g = a.sent, a.abrupt("return", g);
+                                return f = a.sent, a.abrupt("return", f);
                             case 5:
                             case "end":
                                 return a.stop()
                         }
                     }, a)
                 })), function(a, b) {
                     return e.apply(this, arguments)
@@ -88272,126 +88271,60 @@
                         a.statuses[b.meta.arg.resource] = "connected", a.loading = !1, a.failed = !1
                     }), (0, g.Z)(d, k.rejected, function(a, b) {
                         a.statuses[b.meta.arg.resource] = "failed", a.loading = !1, a.failed = !0
                     }), d)
                 });
             b.Z = l.reducer
         },
-        66660: function(a, b, c) {
-            "use strict";
-            var d = c(99534),
-                e = c(85893);
-            c(67294);
-            var f = c(13824),
-                g = c(67617),
-                h = c(99520),
-                i = c(21286),
-                j = new f.ZP,
-                k = function(a) {
-                    var b = a.type;
-                    (0, d.Z)(a, ["type"]);
-                    var c = i.Z.pathToType[b];
-                    return (0, e.jsx)("div", {
-                        children: c ? (0, e.jsx)(g.Z, {
-                            api: j,
-                            type: c
-                        }) : (0, e.jsx)(h.Z, {})
-                    })
-                };
-            b.Z = k
-        },
         75457: function(a, b, c) {
             "use strict";
             c.d(b, {
                 Z: function() {
-                    return aG
+                    return aK
                 }
             });
-            var d = c(99534),
-                e = c(85893),
-                f = c(67294),
-                g = c(14416),
-                h = c(50462),
-                i = c(26042),
-                j = c(69396),
-                k = c(70603),
-                l = c(45258),
-                m = c(91347),
-                n = c(41423),
-                o = c(45697),
-                p = c.n(o),
-                q = c(41120),
-                r = c(22318),
-                s = c(26283),
-                t = c.n(s),
-                u = c(28889),
-                v = c(41749),
-                w = c(43832),
-                x = c(92863),
-                y = c(16204),
-                z = c(88802),
-                A = c(11163),
-                B = c(30640),
-                C = c(902),
-                D = c(61139),
-                E = c(17852),
-                F = c(84283),
-                G = c(96394),
-                H = c(85639),
-                I = c(64436),
-                J = c(55296),
-                K = (0, q.Z)(function(a) {
-                    return {
-                        formControl: {
-                            margin: a.spacing(1),
-                            minWidth: 120
-                        },
-                        selectEmpty: {
-                            marginTop: a.spacing(2)
-                        }
-                    }
-                }),
-                L = function(a) {
-                    var b = a.variant,
-                        c = a.variants,
-                        d = a.handleVariantChange;
-                    a.entityPage, a.convertTimestampToDate, a.local;
-                    var f = K(),
-                        g = function(a) {
-                            d(a)
-                        };
-                    return (0, e.jsxs)(I.Z, {
-                        className: f.formControl,
-                        children: [(0, e.jsx)(G.Z, {
-                            shrink: !0,
-                            id: "demo-simple-select-placeholder-label-label",
-                            children: "Variant"
-                        }), (0, e.jsx)(J.Z, {
-                            labelId: "demo-simple-select-placeholder-label-label",
-                            id: "demo-simple-select-placeholder-label",
-                            value: b,
-                            onChange: g,
-                            displayEmpty: !0,
-                            className: f.selectEmpty,
-                            children: c.map(function(a) {
-                                return (0, e.jsx)(H.Z, {
-                                    value: a,
-                                    children: a
-                                }, a)
-                            })
-                        })]
-                    })
-                },
-                M = (0, g.$j)(function(a) {
-                    return {
-                        entityPage: a.entityPage,
-                        activeVariants: a.selectedVariant
-                    }
-                })(L),
-                N = (0, q.Z)(function(a) {
+            var d = c(47568),
+                e = c(99534),
+                f = c(34051),
+                g = c.n(f),
+                h = c(85893),
+                i = c(43832),
+                j = c(79895),
+                k = c(67294),
+                l = c(31607),
+                m = c(14416),
+                n = c(21286),
+                o = c(99520),
+                p = c(93432),
+                q = c(50462),
+                r = c(26042),
+                s = c(69396),
+                t = c(70603),
+                u = c(45258),
+                v = c(28889),
+                w = c(16204),
+                x = c(41749),
+                y = c(92863),
+                z = c(41120),
+                A = c(41423),
+                B = c(91347),
+                C = c(22318),
+                D = c(26283),
+                E = c.n(D),
+                F = c(11163),
+                G = c(45697),
+                H = c.n(G),
+                I = c(30640),
+                J = c(17852),
+                K = c(902),
+                L = c(61139),
+                M = c(84283),
+                N = c(48535),
+                O = c(88802),
+                P = (0, z.Z)(function(a) {
                     return {
                         formControl: {
                             margin: a.spacing(1),
                             minWidth: 120
                         },
                         selectEmpty: {
                             marginTop: a.spacing(2)
@@ -88402,141 +88335,77 @@
                             border: "1px solid ".concat(a.palette.border.main)
                         },
                         chip: {
                             margin: a.spacing(.5)
                         }
                     }
                 }),
-                O = function(a) {
+                Q = function(a) {
                     var b = a.attributes,
                         c = a.title,
-                        d = N();
-                    return (0, e.jsxs)(w.Z, {
+                        d = P();
+                    return (0, h.jsxs)(i.Z, {
                         className: d.attributeContainer,
-                        children: [(0, e.jsx)(r.Z, {
+                        children: [(0, h.jsx)(C.Z, {
                             variant: "h6",
                             component: "h5",
                             gutterBottom: !0,
                             children: c
                         }), b ? b.map(function(a) {
-                            return (0, e.jsx)(y.Z, {
+                            return (0, h.jsx)(w.Z, {
                                 label: a,
                                 className: d.chip,
                                 variant: "outlined"
                             }, a)
-                        }) : (0, e.jsx)("div", {})]
+                        }) : (0, h.jsx)("div", {})]
                     })
                 },
-                P = c(89849),
-                Q = c(85333),
-                R = c(33841),
-                S = c(44355),
-                T = c(94054),
-                U = c(86507),
-                V = [{
-                    label: "1h",
-                    value: 60
-                }, {
-                    label: "1d",
-                    value: 1440
-                }, {
-                    label: "1w",
-                    value: 10080
-                }, ],
-                W = function(a) {
-                    return {
-                        changeTime: function(b) {
-                            return a((0, P.X)({
-                                timeRange: b
-                            }))
-                        }
-                    }
-                },
-                X = (0, g.$j)(function(a) {
-                    return {
-                        timeRange: a.timeRange
-                    }
-                }, W)(function(a) {
-                    a.timeRange;
-                    var b = a.changeTime,
-                        c = (0, k.Z)(f.useState(60), 2),
-                        d = c[0],
-                        g = c[1],
-                        h = function(a) {
-                            g(a.target.value), b([a.target.value, 0])
-                        };
-                    return (0, e.jsx)("div", {
-                        children: (0, e.jsx)(Q.Z, {
-                            sx: {
-                                minWidth: 120
-                            },
-                            children: (0, e.jsxs)(T.Z, {
-                                fullWidth: !0,
-                                children: [(0, e.jsx)(R.Z, {
-                                    id: "demo-simple-select-label",
-                                    children: "Time Select"
-                                }), (0, e.jsx)(U.Z, {
-                                    labelId: "demo-simple-select-label",
-                                    id: "demo-simple-select",
-                                    value: d,
-                                    label: "Time Select",
-                                    onChange: h,
-                                    children: V.map(function(a) {
-                                        return (0, e.jsx)(S.Z, {
-                                            value: a.value,
-                                            children: a.label
-                                        }, a.label)
-                                    })
-                                })]
-                            })
-                        })
-                    })
-                }),
-                Y = c(17757),
-                Z = c(13824),
-                $ = (0, q.Z)(function(a) {
+                R = Q,
+                S = c(17757),
+                T = c(13824),
+                U = (0, z.Z)(function() {
                     return {
                         graphBox: {
                             height: "50%"
                         }
                     }
                 }),
-                _ = function(a) {
+                V = function(a) {
                     return parseInt(6e4 * a)
                 },
-                aa = function(a) {
+                W = function(a) {
                     var b = a.query,
                         d = a.time,
-                        g = a.timeRange,
-                        h = a.metricsSelect,
-                        i = a.type,
-                        j = a.name,
-                        k = a.query_type,
+                        e = a.timeRange,
+                        f = a.metricsSelect,
+                        g = a.type,
+                        i = a.name,
+                        j = a.query_type,
                         l = a.add_labels,
                         m = a.remote,
                         n = 1e3;
-                    b.includes("error") ? n = 10 : "latency" === k && "TrainingSet" === i ? n = 10 : "latency" === k && "Feature" === i && (n = .1);
-                    var o = $(),
+                    b.includes("error") ? n = 10 : "latency" === j && "TrainingSet" === g ? n = 10 : "latency" === j && "Feature" === g && (n = .1);
+                    var o = U(),
                         p = l ? Object.keys(l).reduce(function(a, b) {
                             return "".concat(a, " ").concat(b, ':"').concat(l[b], '"')
                         }, "") : "",
-                        q = (0, f.useCallback)(function(a, c, d, e) {
-                            var f = a.getTime() / 1e3,
-                                g = c.getTime() / 1e3,
-                                h = "".concat(Z.LK, "/api/v1/query_range?query=").concat(b).concat(p, "&start=").concat(f, "&end=").concat(g, "&step=").concat(d, "s");
-                            return fetch(h).then(function(a) {
+                        q = (0, k.useCallback)(function(a, c, d) {
+                            var e = a.getTime() / 1e3,
+                                f = c.getTime() / 1e3,
+                                g = "".concat(T.LK, "/api/v1/query_range?query=").concat(b).concat(p, "&start=").concat(e, "&end=").concat(f, "&step=").concat(d, "s");
+                            return fetch(g).then(function(a) {
                                 return a.json()
                             }).then(function(a) {
                                 return a.data
                             }).catch(function(a) {
                                 return console.error(a)
                             })
                         }, [b, p, m]);
-                    (0, f.useEffect)(function() {
-                        var a = new Y.Chart(r.current, {
+                    (0, k.useEffect)(function() {
+                        var a = new S.Chart(r.current, {
                             type: "line",
                             plugins: [c(85394)],
                             options: {
                                 maintainAspectRatio: !1,
                                 fillGaps: !0,
                                 tension: 0,
                                 fill: !0,
@@ -88567,75 +88436,139 @@
                                     }, ]
                                 },
                                 plugins: {
                                     "datasource-prometheus": {
                                         query: q,
                                         timeRange: {
                                             type: "relative",
-                                            start: -_(g.timeRange[0]),
-                                            end: -_(g.timeRange[1]),
+                                            start: -V(e.timeRange[0]),
+                                            end: -V(e.timeRange[1]),
                                             msUpdateInterval: 5e3
                                         }
                                     }
                                 }
                             }
                         });
                         return function() {
                             setTimeout(function() {
                                 return a.destroy()
                             }, 100)
                         }
-                    }, [b, d, g, h.metrics, i, j, p, q, n, ]);
-                    var r = f.useRef(null);
-                    return (0, e.jsx)("div", {
+                    }, [b, d, e, f.metrics, g, i, p, q, n, ]);
+                    var r = k.useRef(null);
+                    return (0, h.jsx)("div", {
                         className: o.graphBox,
-                        children: (0, e.jsx)("canvas", {
+                        children: (0, h.jsx)("canvas", {
                             height: "300vw",
                             style: {
                                 maxHeight: "20em",
                                 width: "100%"
                             },
                             ref: r
                         })
                     })
                 },
-                ab = (0, g.$j)(function(a) {
+                X = (0, m.$j)(function(a) {
                     return {
                         timeRange: a.timeRange,
                         metricsSelect: a.metricsSelect
                     }
-                })(aa),
-                ac = (0, q.Z)(function(a) {
+                })(W),
+                Y = (0, z.Z)(function() {
                     return {
                         root: {
                             maxHeight: "20em"
                         }
                     }
                 }),
-                ad = function(a) {
+                Z = function(a) {
                     var b = a.query,
                         c = a.type,
                         d = a.name,
-                        f = a.query_type,
-                        g = a.add_labels,
-                        h = a.remote,
-                        i = ac();
-                    return (0, e.jsx)("div", {
+                        e = a.query_type,
+                        f = a.add_labels,
+                        g = a.remote,
+                        i = Y();
+                    return (0, h.jsx)("div", {
                         className: i.root,
-                        children: (0, e.jsx)(ab, {
+                        children: (0, h.jsx)(X, {
                             query: b,
                             type: c,
                             name: d,
-                            query_type: f,
-                            add_labels: g,
-                            remote: h
+                            query_type: e,
+                            add_labels: f,
+                            remote: g
                         })
                     })
                 },
-                ae = (0, q.Z)(function(a) {
+                $ = c(85333),
+                _ = c(94054),
+                aa = c(33841),
+                ab = c(44355),
+                ac = c(86507),
+                ad = c(89849),
+                ae = [{
+                    label: "1h",
+                    value: 60
+                }, {
+                    label: "1d",
+                    value: 1440
+                }, {
+                    label: "1w",
+                    value: 10080
+                }, ],
+                af = function(a) {
+                    return {
+                        changeTime: function(b) {
+                            return a((0, ad.X)({
+                                timeRange: b
+                            }))
+                        }
+                    }
+                },
+                ag = (0, m.$j)(function(a) {
+                    return {
+                        timeRange: a.timeRange
+                    }
+                }, af)(function(a) {
+                    var b = a.changeTime,
+                        c = (0, t.Z)(k.useState(60), 2),
+                        d = c[0],
+                        e = c[1],
+                        f = function(a) {
+                            e(a.target.value), b([a.target.value, 0])
+                        };
+                    return (0, h.jsx)("div", {
+                        children: (0, h.jsx)($.Z, {
+                            sx: {
+                                minWidth: 120
+                            },
+                            children: (0, h.jsxs)(_.Z, {
+                                fullWidth: !0,
+                                children: [(0, h.jsx)(aa.Z, {
+                                    id: "demo-simple-select-label",
+                                    children: "Time Select"
+                                }), (0, h.jsx)(ac.Z, {
+                                    labelId: "demo-simple-select-label",
+                                    id: "demo-simple-select",
+                                    value: d,
+                                    label: "Time Select",
+                                    onChange: f,
+                                    children: ae.map(function(a) {
+                                        return (0, h.jsx)(ab.Z, {
+                                            value: a.value,
+                                            children: a.label
+                                        }, a.label)
+                                    })
+                                })]
+                            })
+                        })
+                    })
+                }),
+                ah = (0, z.Z)(function(a) {
                     return {
                         root: {
                             flexGrow: 1,
                             padding: a.spacing(0),
                             backgroundColor: a.palette.background.paper,
                             flexBasis: a.spacing(0),
                             flexDirection: "row",
@@ -88689,15 +88622,15 @@
                             alignItems: "center",
                             "& > *": {
                                 height: "70em"
                             }
                         }
                     }
                 }),
-                af = {
+                ai = {
                     Feature: {
                         Throughput: {
                             query: function(a, b, c) {
                                 return 'rate(test_counter{feature="'.concat(a, '",status="success",key="').concat(b, '"}[').concat(c, "])")
                             },
                             type: "count"
                         },
@@ -88725,116 +88658,113 @@
                             query: function(a, b, c) {
                                 return 'rate(test_counter{feature="'.concat(a, '",key="').concat(b, '",status="error"}[').concat(c, "])")
                             },
                             type: "count"
                         }
                     }
                 },
-                ag = function(a) {
+                aj = function(a) {
                     var b = a.type,
                         c = a.name,
                         d = a.variant,
-                        g = a.timeRange,
-                        h = a.aggregates,
-                        i = ae(),
-                        j = (0, k.Z)(f.useState("min"), 2),
-                        l = (j[0], j[1]),
-                        m = (0, k.Z)(f.useState(!1), 2),
-                        n = m[0],
-                        o = m[1],
-                        p = (0, k.Z)(f.useState("1m"), 2),
-                        q = p[0],
-                        s = p[1],
-                        t = function() {
+                        e = a.timeRange,
+                        f = a.aggregates,
+                        g = ah(),
+                        j = (0, t.Z)(k.useState(!1), 2),
+                        l = j[0],
+                        m = j[1],
+                        n = (0, t.Z)(k.useState("1m"), 2),
+                        o = n[0],
+                        p = n[1],
+                        q = function() {
                             var a;
-                            return "http://localhost:9090/graph?" + Object.entries(af[b]).map(function(a, b) {
-                                var e = (0, k.Z)(a, 2),
-                                    f = (e[0], e[1]);
-                                return "g".concat(b, ".expr=").concat(encodeURIComponent(f.query(c, d, q)), " &g").concat(b, ".tab=0&g").concat(b, ".stacked=0&g").concat(b, ".show_exemplars=0&g").concat(b, ".range_input=1h")
+                            return "http://localhost:9090/graph?" + Object.entries(ai[b]).map(function(a, b) {
+                                var e = (0, t.Z)(a, 2)[1];
+                                return "g".concat(b, ".expr=").concat(encodeURIComponent(e.query(c, d, o)), " &g").concat(b, ".tab=0&g").concat(b, ".stacked=0&g").concat(b, ".show_exemplars=0&g").concat(b, ".range_input=1h")
                             }).join("&")
                         };
-                    (0, f.useEffect)(function() {
-                        fetch("http://localhost:9090/api/v1/labels").then(function(a) {
-                            return o(!0)
-                        }).catch(function(a) {
-                            return o(!1)
-                        }), g.timeRange[0] > 60 ? (l("hour"), s("1h")) : 60 === g.timeRange[0] && (l("min"), s("1m"))
-                    }, [g, h]);
-                    var u = function() {
-                        n && (window.location.href = t())
+                    (0, k.useEffect)(function() {
+                        fetch("http://localhost:9090/api/v1/labels").then(function() {
+                            return m(!0)
+                        }).catch(function() {
+                            return m(!1)
+                        }), e.timeRange[0] > 60 ? p("1h") : 60 === e.timeRange[0] && p("1m")
+                    }, [e, f]);
+                    var r = function() {
+                        l && (window.location.href = q())
                     };
-                    return (0, e.jsxs)("div", {
-                        className: i.root,
-                        children: [(0, e.jsxs)(r.Z, {
+                    return (0, h.jsxs)("div", {
+                        className: g.root,
+                        children: [(0, h.jsxs)(C.Z, {
                             variant: "body1",
-                            className: i.linkPromChip,
-                            children: ["Source:", " ", (0, e.jsx)(y.Z, {
+                            className: g.linkPromChip,
+                            children: ["Source:", " ", (0, h.jsx)(w.Z, {
                                 variant: "outlined",
-                                clickable: n,
-                                className: i.linkChip,
+                                clickable: l,
+                                className: g.linkChip,
                                 size: "small",
-                                color: n ? "secondary" : "error",
-                                onClick: u,
+                                color: l ? "secondary" : "error",
+                                onClick: r,
                                 label: "Prometheus"
                             })]
-                        }), (0, e.jsx)(v.Z, {
+                        }), (0, h.jsx)(x.Z, {
                             container: !0,
                             spacing: 0,
-                            children: (0, e.jsx)(v.Z, {
+                            children: (0, h.jsx)(x.Z, {
                                 item: !0,
                                 xs: 12,
                                 height: "10em",
-                                children: (0, e.jsx)("div", {
-                                    className: i.graph,
-                                    children: (0, e.jsx)(w.Z, {
+                                children: (0, h.jsx)("div", {
+                                    className: g.graph,
+                                    children: (0, h.jsx)(i.Z, {
                                         minheight: "1300px",
-                                        children: Object.entries(af[b]).map(function(a, f) {
-                                            var g = (0, k.Z)(a, 2),
-                                                j = g[0],
-                                                l = g[1];
-                                            return (0, e.jsxs)("div", {
-                                                children: [(0, e.jsxs)("div", {
-                                                    className: i.titleBar,
-                                                    children: [(0, e.jsx)("div", {
-                                                        className: i.graphTitle,
-                                                        children: (0, e.jsx)(r.Z, {
+                                        children: Object.entries(ai[b]).map(function(a, e) {
+                                            var i = (0, t.Z)(a, 2),
+                                                j = i[0],
+                                                k = i[1];
+                                            return (0, h.jsxs)("div", {
+                                                children: [(0, h.jsxs)("div", {
+                                                    className: g.titleBar,
+                                                    children: [(0, h.jsx)("div", {
+                                                        className: g.graphTitle,
+                                                        children: (0, h.jsx)(C.Z, {
                                                             variant: "h6",
                                                             children: j
                                                         })
-                                                    }), (0, e.jsx)("div", {
-                                                        className: i.aggDropdown,
-                                                        children: (0, e.jsx)(X, {})
+                                                    }), (0, h.jsx)("div", {
+                                                        className: g.aggDropdown,
+                                                        children: (0, h.jsx)(ag, {})
                                                     })]
-                                                }), (0, e.jsx)(ad, {
-                                                    query: l.query(c, d, q),
+                                                }), (0, h.jsx)(Z, {
+                                                    query: k.query(c, d, o),
                                                     type: b,
                                                     name: c,
-                                                    query_type: l.type,
-                                                    aggregate: h[f],
-                                                    remote: n
+                                                    query_type: k.type,
+                                                    aggregate: f[e],
+                                                    remote: l
                                                 })]
                                             })
                                         })
                                     })
                                 })
                             })
                         })]
                     })
                 },
-                ah = (0, g.$j)(function(a) {
+                ak = (0, m.$j)(function(a) {
                     return {
                         timeRange: a.timeRange,
                         metricsSelect: a.metricsSelect,
                         aggregates: a.aggregates
                     }
-                })(ag),
-                ai = c(46799),
-                aj = c(85384),
-                ak = c.n(aj),
-                al = (0, q.Z)(function(a) {
+                })(aj),
+                al = c(85384),
+                am = c.n(al),
+                an = c(46799),
+                ao = (0, z.Z)(function(a) {
                     return {
                         root: {
                             flexGrow: 1,
                             padding: a.spacing(0),
                             backgroundColor: a.palette.background.paper,
                             flexBasis: a.spacing(0),
                             flexDirection: "row",
@@ -88873,15 +88803,15 @@
                             alignItems: "center",
                             "& > *": {
                                 height: "40em"
                             }
                         }
                     }
                 }),
-                am = {
+                ap = {
                     Feature: {
                         "Average Latency": "42ms",
                         "95 Latency": "57ms",
                         "99 Latency": "99ms",
                         "Mean Error Rate": "0.1922%"
                     },
                     "Feature Set": {
@@ -88891,15 +88821,15 @@
                         "Mean Error Rate": "0.1922%"
                     },
                     Entity: {
                         Features: 44,
                         "Primary Provider": "Snowflake"
                     }
                 },
-                an = {
+                aq = {
                     plugins: {
                         title: {
                             display: !0,
                             text: "Query Error Summary"
                         }
                     },
                     responsive: !0,
@@ -88908,116 +88838,164 @@
                             stacked: !0
                         },
                         y: {
                             stacked: !0
                         }
                     }
                 },
-                ao = ["Last 1000 queries", "Last 7 days", "Overall"],
-                ap = {
-                    labels: ao,
+                ar = ["Last 1000 queries", "Last 7 days", "Overall"],
+                as = {
+                    labels: ar,
                     datasets: [{
                         label: "Client Errors",
-                        data: ao.map(function() {
-                            return ak().datatype.number({
+                        data: ar.map(function() {
+                            return am().datatype.number({
                                 min: 0,
                                 max: 100
                             })
                         }),
                         backgroundColor: "rgb(255, 99, 132)"
                     }, {
                         label: "Server Errors",
-                        data: ao.map(function() {
-                            return ak().datatype.number({
+                        data: ar.map(function() {
+                            return am().datatype.number({
                                 min: 0,
                                 max: 100
                             })
                         }),
                         backgroundColor: "rgb(75, 192, 192)"
                     }, {
                         label: "Provider Errors",
-                        data: ao.map(function() {
-                            return ak().datatype.number({
+                        data: ar.map(function() {
+                            return am().datatype.number({
                                 min: 0,
                                 max: 100
                             })
                         }),
                         backgroundColor: "rgb(53, 162, 235)"
                     }, ]
                 },
-                aq = function(a) {
-                    var b = a.type;
-                    a.name;
-                    var c = al(),
-                        d = am[b];
-                    return (0, e.jsx)("div", {
+                at = function(a) {
+                    var b = a.type,
+                        c = ao(),
+                        d = ap[b];
+                    return (0, h.jsx)("div", {
                         className: c.root,
-                        children: (0, e.jsx)(v.Z, {
+                        children: (0, h.jsx)(x.Z, {
                             container: !0,
                             spacing: 0,
-                            children: (0, e.jsx)(v.Z, {
+                            children: (0, h.jsx)(x.Z, {
                                 item: !0,
                                 xs: 12,
                                 height: "15em",
-                                children: (0, e.jsx)("div", {
+                                children: (0, h.jsx)("div", {
                                     className: c.graph,
-                                    children: (0, e.jsxs)(w.Z, {
+                                    children: (0, h.jsxs)(i.Z, {
                                         minheight: "800px",
                                         children: [Object.keys(d).map(function(a, b) {
-                                            return (0, e.jsxs)(r.Z, {
+                                            return (0, h.jsxs)(C.Z, {
                                                 variant: "body1",
-                                                children: [(0, e.jsxs)("b", {
+                                                children: [(0, h.jsxs)("b", {
                                                     children: [a, ": "]
                                                 }), d[a]]
-                                            })
-                                        }), (0, e.jsx)(r.Z, {
+                                            }, b)
+                                        }), (0, h.jsx)(C.Z, {
                                             variant: "body1",
-                                            children: (0, e.jsx)("b", {
+                                            children: (0, h.jsx)("b", {
                                                 children: "Error Stats:"
                                             })
-                                        }), (0, e.jsx)("div", {
+                                        }), (0, h.jsx)("div", {
                                             className: c.errorBar,
-                                            children: (0, e.jsx)(ai.$Q, {
-                                                options: an,
-                                                data: ap,
+                                            children: (0, h.jsx)(an.$Q, {
+                                                options: aq,
+                                                data: as,
                                                 className: c.barGraph
                                             })
                                         })]
                                     })
                                 })
                             })
                         })
                     })
                 },
-                ar = c(21286),
-                as = c(48535);
+                au = c(64436),
+                av = c(96394),
+                aw = c(85639),
+                ax = c(55296),
+                ay = (0, z.Z)(function(a) {
+                    return {
+                        formControl: {
+                            margin: a.spacing(1),
+                            minWidth: 120
+                        },
+                        selectEmpty: {
+                            marginTop: a.spacing(2)
+                        }
+                    }
+                }),
+                az = function(a) {
+                    var b = a.variant,
+                        c = a.variants,
+                        d = a.handleVariantChange,
+                        e = ay(),
+                        f = function(a) {
+                            d(a)
+                        };
+                    return (0, h.jsxs)(au.Z, {
+                        className: e.formControl,
+                        children: [(0, h.jsx)(av.Z, {
+                            shrink: !0,
+                            id: "demo-simple-select-placeholder-label-label",
+                            children: "Variant"
+                        }), (0, h.jsx)(ax.Z, {
+                            labelId: "demo-simple-select-placeholder-label-label",
+                            id: "demo-simple-select-placeholder-label",
+                            value: b,
+                            onChange: f,
+                            displayEmpty: !0,
+                            className: e.selectEmpty,
+                            children: c.map(function(a) {
+                                return (0, h.jsx)(aw.Z, {
+                                    value: a,
+                                    children: a
+                                }, a)
+                            })
+                        })]
+                    })
+                },
+                aA = (0, m.$j)(function(a) {
+                    return {
+                        entityPage: a.entityPage,
+                        activeVariants: a.selectedVariant
+                    }
+                })(az);
 
-            function at(a) {
+            function aB(a) {
                 var b = a.children,
                     c = a.value,
-                    f = a.index,
-                    g = (0, d.Z)(a, ["children", "value", "index"]);
-                return (0, e.jsx)("div", (0, j.Z)((0, i.Z)({
+                    d = a.index,
+                    f = (0, e.Z)(a, ["children", "value", "index"]);
+                return (0, h.jsx)("div", (0, s.Z)((0, r.Z)({
                     role: "tabpanel",
-                    hidden: c !== f,
-                    id: "simple-tabpanel-".concat(f),
-                    "aria-labelledby": "simple-tab-".concat(f)
-                }, g), {
-                    children: c === f && (0, e.jsx)(u.Z, {
+                    hidden: c !== d,
+                    id: "simple-tabpanel-".concat(d),
+                    "aria-labelledby": "simple-tab-".concat(d)
+                }, f), {
+                    children: c === d && (0, h.jsx)(v.Z, {
                         p: 3,
                         children: b
                     })
                 }))
             }
-            B.Z.registerLanguage("python", C.Z), B.Z.registerLanguage("sql", D.Z), B.Z.registerLanguage("json", E.Z), at.propTypes = {
-                children: p().node,
-                index: p().any.isRequired,
-                value: p().any.isRequired
+            I.Z.registerLanguage("python", K.Z), I.Z.registerLanguage("sql", L.Z), I.Z.registerLanguage("json", J.Z), aB.propTypes = {
+                children: H().node,
+                index: H().any.isRequired,
+                value: H().any.isRequired
             };
-            var au = (0, q.Z)(function(a) {
+            var aC = (0, z.Z)(function(a) {
                 return {
                     root: {
                         flexGrow: 1,
                         padding: a.spacing(0),
                         backgroundColor: a.palette.background.paper,
                         marginTop: a.spacing(2)
                     },
@@ -89144,540 +89122,550 @@
                     },
                     titleText: {
                         paddingLeft: "1em"
                     }
                 }
             });
 
-            function av(a) {
+            function aD(a) {
                 return {
                     id: "simple-tab-".concat(a),
                     "aria-controls": "simple-tabpanel-".concat(a)
                 }
             }
-            var aw, ax = function(a) {
+            var aE, aF = function(a) {
                     var b, c, d = a.entity,
-                        g = a.setVariant,
-                        h = a.activeVariants,
-                        o = d.resources,
-                        p = ar.Z[o.type],
-                        q = p.type,
-                        u = (0, A.useRouter)(),
-                        C = p.hasMetrics,
-                        D = C + !1,
-                        E = o.name,
-                        G = p.materialIcon,
-                        H = o["default-variant"];
-                    h[d.resources.type][E] ? H = h[d.resources.type][E] : g(d.resources.type, E, o["default-variant"]);
-                    var I = {},
-                        J = {};
-                    Object.keys(c = p.hasVariants ? o.variants[H] : o).forEach(function(a) {
-                        ar.Z.pathToType[a] ? J[ar.Z.pathToType[a]] = c[a] : I[a] = c[a]
-                    }), I.source && (I.source = I.source.Name, I["source-variant"] = I.source.Variant);
-                    var K, L, N = function(a) {
+                        e = a.setVariant,
+                        f = a.activeVariants,
+                        g = d.resources,
+                        j = n.Z[g.type],
+                        l = j.type,
+                        m = (0, F.useRouter)(),
+                        o = j.hasMetrics,
+                        p = o + !1,
+                        q = g.name,
+                        v = j.materialIcon,
+                        z = g["default-variant"];
+                    f[d.resources.type][q] ? z = f[d.resources.type][q] : e(d.resources.type, q, g["default-variant"]);
+                    var G = {},
+                        H = {};
+                    Object.keys(c = j.hasVariants ? g.variants[z] : g).forEach(function(a) {
+                        n.Z.pathToType[a] ? H[n.Z.pathToType[a]] = c[a] : G[a] = c[a]
+                    }), G.source && (G.source = G.source.Name, G["source-variant"] = G.source.Variant);
+                    var J, K, L = function(a) {
                             return new Date(a).toLocaleString("en-US", {
                                 timeZone: Intl.DateTimeFormat().resolvedOptions().timeZone
                             })
                         },
-                        P = o["all-variants"],
-                        Q = au(),
-                        R = (0, k.Z)(f.useState(0), 2),
-                        S = R[0],
-                        T = R[1],
-                        U = function(a) {
-                            g(q, E, a.target.value)
+                        P = g["all-variants"],
+                        Q = aC(),
+                        S = (0, t.Z)(k.useState(0), 2),
+                        T = S[0],
+                        U = S[1],
+                        V = function(a) {
+                            e(l, q, a.target.value)
                         },
-                        V = function(a, b) {
-                            T(b)
+                        W = function(a, b) {
+                            U(b)
                         },
-                        W = function(a) {
+                        X = function(a) {
                             return a[0].toUpperCase() + a.slice(1).toLowerCase()
                         },
-                        X = function(a) {
-                            u.push("/entities/".concat(I.entity))
+                        Y = function() {
+                            m.push("/entities/".concat(G.entity))
                         },
-                        Y = function(a) {
-                            u.push("/sources/".concat(I.source))
+                        Z = function() {
+                            m.push("/sources/".concat(G.source))
                         },
-                        Z = function(a) {
-                            u.push("/labels/".concat(I.label.Name))
+                        $ = function() {
+                            m.push("/labels/".concat(G.label.Name))
                         },
-                        $ = function(a) {
-                            u.push("/users/".concat(I.owner))
+                        _ = function() {
+                            m.push("/users/".concat(G.owner))
                         },
-                        _ = function(a) {
-                            u.push("/providers/".concat(I.provider))
+                        aa = function() {
+                            m.push("/providers/".concat(G.provider))
                         };
-                    return (0, e.jsx)("div", {
-                        children: (0, e.jsxs)(w.Z, {
+                    return (0, h.jsx)("div", {
+                        children: (0, h.jsxs)(i.Z, {
                             maxWidth: "xl",
                             className: Q.border,
-                            children: [(0, e.jsxs)("div", {
+                            children: [(0, h.jsxs)("div", {
                                 className: Q.metadata,
-                                children: [(0, e.jsxs)(v.Z, {
+                                children: [(0, h.jsxs)(x.Z, {
                                     container: !0,
                                     className: Q.topContainer,
                                     justifyContent: "flex-start",
-                                    children: [(0, e.jsx)(v.Z, {
+                                    children: [(0, h.jsx)(x.Z, {
                                         item: !0,
                                         xs: !1,
                                         className: Q.icon
-                                    }), (0, e.jsx)(v.Z, {
+                                    }), (0, h.jsx)(x.Z, {
                                         item: !0,
                                         xs: 12,
                                         lg: 12,
-                                        children: (0, e.jsxs)("div", {
+                                        children: (0, h.jsxs)("div", {
                                             className: Q.resourcesTopRow,
-                                            children: [(0, e.jsxs)("div", {
+                                            children: [(0, h.jsxs)("div", {
                                                 className: Q.title,
-                                                children: [(0, e.jsx)(x.Z, {
-                                                    children: G
-                                                }), (0, e.jsxs)("div", {
+                                                children: [(0, h.jsx)(y.Z, {
+                                                    children: v
+                                                }), (0, h.jsxs)("div", {
                                                     className: Q.titleText,
-                                                    children: [(0, e.jsx)(r.Z, {
+                                                    children: [(0, h.jsx)(C.Z, {
                                                         variant: "h4",
                                                         component: "h4",
-                                                        children: (0, e.jsx)("b", {
-                                                            children: o.name
+                                                        children: (0, h.jsx)("b", {
+                                                            children: g.name
                                                         })
-                                                    }), I.created && (0, e.jsxs)(r.Z, {
+                                                    }), G.created && (0, h.jsxs)(C.Z, {
                                                         variant: "subtitle1",
-                                                        children: ["Created: ", N(I.created)]
+                                                        children: ["Created: ", L(G.created)]
                                                     })]
                                                 })]
-                                            }), P && (0, e.jsx)(M, {
-                                                variant: H,
+                                            }), P && (0, h.jsx)(aA, {
+                                                variant: z,
                                                 variants: P,
-                                                handleVariantChange: U,
-                                                type: q,
-                                                name: E,
-                                                convertTimestampToDate: N
+                                                handleVariantChange: V,
+                                                type: l,
+                                                name: q,
+                                                convertTimestampToDate: L
                                             })]
                                         })
                                     })]
-                                }), Object.keys(I).length > 0 && "NO_STATUS" != I.status && (0, e.jsx)("div", {
+                                }), Object.keys(G).length > 0 && "NO_STATUS" != G.status && (0, h.jsx)("div", {
                                     className: Q.resourcesData,
-                                    children: (0, e.jsxs)(v.Z, {
+                                    children: (0, h.jsxs)(x.Z, {
                                         container: !0,
                                         spacing: 0,
-                                        children: [(0, e.jsxs)(v.Z, {
+                                        children: [(0, h.jsxs)(x.Z, {
                                             item: !0,
                                             xs: 6,
                                             className: Q.resourceMetadata,
-                                            children: [I.description && (0, e.jsxs)(r.Z, {
+                                            children: [G.description && (0, h.jsxs)(C.Z, {
                                                 variant: "body1",
                                                 className: Q.description,
-                                                children: [(0, e.jsx)("b", {
+                                                children: [(0, h.jsx)("b", {
                                                     children: "Description:"
-                                                }), " ", I.description]
-                                            }), I.owner && (0, e.jsxs)("div", {
+                                                }), " ", G.description]
+                                            }), G.owner && (0, h.jsxs)("div", {
                                                 className: Q.linkBox,
-                                                children: [(0, e.jsxs)(r.Z, {
+                                                children: [(0, h.jsxs)(C.Z, {
                                                     variant: "body1",
                                                     className: Q.typeTitle,
-                                                    children: [(0, e.jsx)("b", {
+                                                    children: [(0, h.jsx)("b", {
                                                         children: "Owner:"
                                                     }), " "]
-                                                }), (0, e.jsx)(y.Z, {
+                                                }), (0, h.jsx)(w.Z, {
                                                     variant: "outlined",
                                                     className: Q.linkChip,
                                                     size: "small",
-                                                    onClick: $,
-                                                    label: I.owner
+                                                    onClick: _,
+                                                    label: G.owner
                                                 })]
-                                            }), I.provider && (0, e.jsxs)("div", {
+                                            }), G.provider && (0, h.jsxs)("div", {
                                                 className: Q.linkBox,
-                                                children: [(0, e.jsxs)(r.Z, {
+                                                children: [(0, h.jsxs)(C.Z, {
                                                     variant: "body1",
                                                     className: Q.typeTitle,
-                                                    children: [(0, e.jsx)("b", {
+                                                    children: [(0, h.jsx)("b", {
                                                         children: "Provider:"
                                                     }), " "]
-                                                }), (0, e.jsx)(y.Z, {
+                                                }), (0, h.jsx)(w.Z, {
                                                     variant: "outlined",
                                                     className: Q.linkChip,
                                                     size: "small",
-                                                    onClick: _,
-                                                    label: I.provider
+                                                    onClick: aa,
+                                                    label: G.provider
                                                 })]
-                                            }), I.dimensions && (0, e.jsxs)(r.Z, {
+                                            }), G.dimensions && (0, h.jsxs)(C.Z, {
                                                 variant: "body1",
-                                                children: [(0, e.jsx)("b", {
+                                                children: [(0, h.jsx)("b", {
                                                     children: "Dimensions:"
-                                                }), " ", I.dimensions]
-                                            }), I["data-type"] && (0, e.jsxs)(r.Z, {
+                                                }), " ", G.dimensions]
+                                            }), G["data-type"] && (0, h.jsxs)(C.Z, {
                                                 variant: "body1",
-                                                children: [(0, e.jsx)("b", {
+                                                children: [(0, h.jsx)("b", {
                                                     children: "Data Type:"
-                                                }), " ", I["data-type"]]
-                                            }), I.joined && (0, e.jsxs)(r.Z, {
+                                                }), " ", G["data-type"]]
+                                            }), G.joined && (0, h.jsxs)(C.Z, {
                                                 variant: "body1",
-                                                children: [(0, e.jsx)("b", {
+                                                children: [(0, h.jsx)("b", {
                                                     children: "Joined:"
-                                                }), " ", N(I.joined)]
-                                            }), I.software && (0, e.jsxs)(r.Z, {
+                                                }), " ", L(G.joined)]
+                                            }), G.software && (0, h.jsxs)(C.Z, {
                                                 variant: "body1",
-                                                children: [(0, e.jsx)("b", {
+                                                children: [(0, h.jsx)("b", {
                                                     children: "Software:"
-                                                }), " ", I.software]
-                                            }), I.label && (0, e.jsxs)("div", {
+                                                }), " ", G.software]
+                                            }), G.label && (0, h.jsxs)("div", {
                                                 className: Q.linkBox,
-                                                children: [(0, e.jsxs)(r.Z, {
+                                                children: [(0, h.jsxs)(C.Z, {
                                                     variant: "body1",
                                                     className: Q.typeTitle,
-                                                    children: [(0, e.jsx)("b", {
+                                                    children: [(0, h.jsx)("b", {
                                                         children: "Label: "
                                                     }), " "]
-                                                }), (0, e.jsx)(y.Z, {
+                                                }), (0, h.jsx)(w.Z, {
                                                     variant: "outlined",
                                                     className: Q.linkChip,
                                                     size: "small",
-                                                    onClick: Z,
-                                                    label: I.label.Name
+                                                    onClick: $,
+                                                    label: G.label.Name
                                                 })]
-                                            }), I["provider-type"] && (0, e.jsxs)(r.Z, {
+                                            }), G["provider-type"] && (0, h.jsxs)(C.Z, {
                                                 variant: "body1",
-                                                children: [(0, e.jsx)("b", {
+                                                children: [(0, h.jsx)("b", {
                                                     children: "Provider Type:"
-                                                }), " ", I["provider-type"]]
-                                            }), I.team && (0, e.jsxs)(r.Z, {
+                                                }), " ", G["provider-type"]]
+                                            }), G.team && (0, h.jsxs)(C.Z, {
                                                 variant: "body1",
-                                                children: [(0, e.jsx)("b", {
+                                                children: [(0, h.jsx)("b", {
                                                     children: "Team:"
-                                                }), " ", I.team]
-                                            }), I.status && "NO_STATUS" !== I.status && (0, e.jsxs)(r.Z, {
+                                                }), " ", G.team]
+                                            }), G.status && "NO_STATUS" !== G.status && (0, h.jsxs)(C.Z, {
                                                 variant: "body1",
-                                                children: [(0, e.jsx)("b", {
+                                                children: [(0, h.jsx)("b", {
                                                     children: "Status:"
-                                                }), " ", I.status]
-                                            }), I.error && "" !== I.error && (0, e.jsxs)(r.Z, {
+                                                }), " ", G.status]
+                                            }), G.error && "" !== G.error && (0, h.jsxs)(C.Z, {
                                                 variant: "body1",
-                                                children: [(0, e.jsx)("b", {
+                                                children: [(0, h.jsx)("b", {
                                                     children: "Error Message:"
-                                                }), " ", I.error]
-                                            }), I["source-type"] && (0, e.jsxs)(r.Z, {
+                                                }), " ", G.error]
+                                            }), G["source-type"] && (0, h.jsxs)(C.Z, {
                                                 variant: "body1",
-                                                children: [(0, e.jsx)("b", {
+                                                children: [(0, h.jsx)("b", {
                                                     children: "Source Type:"
-                                                }), " ", I["source-type"]]
-                                            }), I.specifications && (K = I.specifications, L = 0, Object.keys(K).forEach(function(a) {
-                                                "" !== I.specifications[a] && L++
-                                            }), L > 0) && (0, e.jsxs)("div", {
-                                                children: [(0, e.jsx)(r.Z, {
+                                                }), " ", G["source-type"]]
+                                            }), G.specifications && (J = G.specifications, K = 0, Object.keys(J).forEach(function(a) {
+                                                "" !== G.specifications[a] && K++
+                                            }), K > 0) && (0, h.jsxs)("div", {
+                                                children: [(0, h.jsx)(C.Z, {
                                                     variant: "body1",
-                                                    children: (0, e.jsx)("b", {
+                                                    children: (0, h.jsx)("b", {
                                                         children: "Specifications:"
                                                     })
-                                                }), (0, e.jsx)(r.Z, {
+                                                }), (0, h.jsx)(C.Z, {
                                                     variant: "body1",
                                                     component: "h2",
-                                                    children: Object.keys(I.specifications).map(function(a) {
-                                                        return "" !== I.specifications[a] && (0, e.jsxs)("div", {
+                                                    children: Object.keys(G.specifications).map(function(a, b) {
+                                                        return "" !== G.specifications[a] && (0, h.jsxs)("div", {
                                                             style: {
                                                                 marginLeft: 16
                                                             },
-                                                            children: [(0, e.jsxs)("b", {
+                                                            children: [(0, h.jsxs)("b", {
                                                                 children: [a, ": "]
-                                                            }), " ", I.specifications[a]]
-                                                        })
+                                                            }), " ", G.specifications[a]]
+                                                        }, b)
                                                     })
                                                 })]
-                                            }), I.definition && (0, e.jsxs)("div", {
-                                                children: [(0, e.jsx)(r.Z, {
+                                            }), G.definition && (0, h.jsxs)("div", {
+                                                children: [(0, h.jsx)(C.Z, {
                                                     variant: "body1",
-                                                    children: (0, e.jsx)("b", {
+                                                    children: (0, h.jsx)("b", {
                                                         children: "Origin:"
                                                     })
-                                                }), "SQL Transformation" === I["source-type"] ? (0, e.jsx)(B.Z, {
+                                                }), "SQL Transformation" === G["source-type"] ? (0, h.jsx)(I.Z, {
                                                     className: Q.syntax,
                                                     language: "sql",
-                                                    style: F.be,
-                                                    children: I.definition
-                                                }) : (0, e.jsx)(r.Z, {
+                                                    style: M.be,
+                                                    children: G.definition
+                                                }) : (0, h.jsx)(C.Z, {
                                                     variant: "h7",
-                                                    children: (0, e.jsx)("b", {
-                                                        children: I.definition
+                                                    children: (0, h.jsx)("b", {
+                                                        children: G.definition
                                                     })
                                                 })]
-                                            }), I["serialized-config"] && (0, e.jsxs)(r.Z, {
+                                            }), G["serialized-config"] && (0, h.jsxs)(C.Z, {
                                                 variant: "body1",
-                                                children: [(0, e.jsx)("b", {
+                                                children: [(0, h.jsx)("b", {
                                                     children: "Serialized Config:"
-                                                }), " ", I["serialized-config"]]
-                                            }), I.source && (0, e.jsxs)("div", {
+                                                }), " ", G["serialized-config"]]
+                                            }), G.source && (0, h.jsxs)("div", {
                                                 className: Q.linkBox,
-                                                children: [(0, e.jsxs)(r.Z, {
+                                                children: [(0, h.jsxs)(C.Z, {
                                                     variant: "body1",
                                                     className: Q.typeTitle,
-                                                    children: [(0, e.jsx)("b", {
+                                                    children: [(0, h.jsx)("b", {
                                                         children: "Source: "
                                                     }), " "]
-                                                }), (0, e.jsx)(y.Z, {
+                                                }), (0, h.jsx)(w.Z, {
                                                     variant: "outlined",
                                                     className: Q.linkChip,
                                                     size: "small",
-                                                    onClick: Y,
-                                                    label: I.source
+                                                    onClick: Z,
+                                                    label: G.source
                                                 })]
-                                            }), I.entity && (0, e.jsxs)("div", {
+                                            }), G.entity && (0, h.jsxs)("div", {
                                                 className: Q.linkBox,
-                                                children: [(0, e.jsxs)(r.Z, {
+                                                children: [(0, h.jsxs)(C.Z, {
                                                     variant: "body1",
                                                     className: Q.typeTitle,
-                                                    children: [(0, e.jsx)("b", {
+                                                    children: [(0, h.jsx)("b", {
                                                         children: "Entity:"
                                                     }), " "]
-                                                }), (0, e.jsx)(y.Z, {
+                                                }), (0, h.jsx)(w.Z, {
                                                     variant: "outlined",
                                                     className: Q.linkChip,
                                                     size: "small",
-                                                    onClick: X,
-                                                    label: I.entity
+                                                    onClick: Y,
+                                                    label: G.entity
                                                 })]
-                                            }), I.location && !I["is-on-demand"] && (0, e.jsxs)("div", {
+                                            }), G.location && !G["is-on-demand"] && (0, h.jsxs)("div", {
                                                 className: Q.linkBox,
-                                                children: [(0, e.jsxs)(r.Z, {
+                                                children: [(0, h.jsxs)(C.Z, {
                                                     variant: "body1",
                                                     className: Q.typeTitle,
-                                                    children: [(0, e.jsx)("b", {
+                                                    children: [(0, h.jsx)("b", {
                                                         children: "Columns:"
                                                     }), " "]
-                                                }), (0, e.jsxs)(r.Z, {
+                                                }), (0, h.jsxs)(C.Z, {
                                                     variant: "body2",
-                                                    children: ["\xa0", (0, e.jsx)("b", {
+                                                    children: ["\xa0", (0, h.jsx)("b", {
                                                         children: "Entity:"
-                                                    }), " ", I.location.Entity, "\xa0", (0, e.jsx)("b", {
+                                                    }), " ", G.location.Entity, "\xa0", (0, h.jsx)("b", {
                                                         children: "Value:"
-                                                    }), " ", I.location.Value, "\xa0", (0, e.jsx)("b", {
+                                                    }), " ", G.location.Value, "\xa0", (0, h.jsx)("b", {
                                                         children: "Timestamp:"
-                                                    }), " ", I.location.TS]
+                                                    }), " ", G.location.TS]
                                                 })]
-                                            }), I.location && I["is-on-demand"] && (0, e.jsxs)("div", {
+                                            }), G.location && G["is-on-demand"] && (0, h.jsxs)("div", {
                                                 className: Q.linkBox,
-                                                children: [(0, e.jsxs)(r.Z, {
+                                                children: [(0, h.jsxs)(C.Z, {
                                                     variant: "body1",
                                                     className: Q.typeTitle,
-                                                    children: [(0, e.jsx)("b", {
+                                                    children: [(0, h.jsx)("b", {
                                                         children: "Feature Variant Type:"
                                                     }), " "]
-                                                }), (0, e.jsx)(y.Z, {
+                                                }), (0, h.jsx)(w.Z, {
                                                     variant: "outlined",
                                                     className: Q.linkChip,
                                                     size: "small",
                                                     onClick: function() {},
                                                     label: "On-Demand"
                                                 })]
                                             })]
-                                        }), (null === (b = I.tags) || void 0 === b ? void 0 : b.length) > 0 && (0, e.jsx)(v.Z, {
+                                        }), (null === (b = G.tags) || void 0 === b ? void 0 : b.length) > 0 && (0, h.jsx)(x.Z, {
                                             item: !0,
                                             xs: !0,
-                                            children: (0, e.jsx)(O, {
-                                                attributes: I.tags,
+                                            children: (0, h.jsx)(R, {
+                                                attributes: G.tags,
                                                 title: "Tags"
                                             })
-                                        }), Object.keys(I.properties || {}).length > 0 && (0, e.jsx)(v.Z, {
+                                        }), Object.keys(G.properties || {}).length > 0 && (0, h.jsx)(x.Z, {
                                             item: !0,
                                             xs: !0,
-                                            children: (0, e.jsx)(O, {
-                                                attributes: Object.entries(I.properties).map(function(a) {
-                                                    var b = (0, k.Z)(a, 2),
+                                            children: (0, h.jsx)(R, {
+                                                attributes: Object.entries(G.properties).map(function(a) {
+                                                    var b = (0, t.Z)(a, 2),
                                                         c = b[0],
                                                         d = b[1];
                                                     return "".concat(c, ":").concat(d)
                                                 }),
                                                 title: "Properties"
                                             })
                                         })]
                                     })
-                                }), I.config && (0, e.jsxs)("div", {
+                                }), G.config && (0, h.jsxs)("div", {
                                     className: Q.config,
-                                    children: [(0, e.jsx)(r.Z, {
+                                    children: [(0, h.jsx)(C.Z, {
                                         variant: "body1",
-                                        children: (0, e.jsx)("b", {
+                                        children: (0, h.jsx)("b", {
                                             children: "Config:"
                                         })
-                                    }), (0, e.jsx)(B.Z, {
+                                    }), (0, h.jsx)(I.Z, {
                                         className: Q.syntax,
-                                        language: I.language,
-                                        style: F.be,
-                                        children: I.config
+                                        language: G.language,
+                                        style: M.be,
+                                        children: G.config
                                     })]
                                 })]
-                            }), (0, e.jsxs)("div", {
+                            }), (0, h.jsxs)("div", {
                                 className: Q.root,
-                                children: [(0, e.jsx)(l.Z, {
+                                children: [(0, h.jsx)(u.Z, {
                                     position: "static",
                                     className: Q.appbar,
-                                    children: (0, e.jsxs)(m.Z, {
-                                        value: S,
-                                        onChange: V,
+                                    children: (0, h.jsxs)(B.Z, {
+                                        value: T,
+                                        onChange: W,
                                         "aria-label": "simple tabs example",
-                                        children: [C && (0, e.jsx)(n.Z, (0, i.Z)({
+                                        children: [o && (0, h.jsx)(A.Z, (0, r.Z)({
                                             label: "metrics"
-                                        }, av(0))), !1, Object.keys(J).map(function(a, b) {
-                                            return (0, e.jsx)(n.Z, (0, i.Z)({
-                                                label: ar.Z[a].typePlural
-                                            }, av(b + D)), b)
+                                        }, aD(0))), !1, Object.keys(H).map(function(a, b) {
+                                            return (0, h.jsx)(A.Z, (0, r.Z)({
+                                                label: n.Z[a].typePlural
+                                            }, aD(b + p)), b)
                                         })]
                                     })
-                                }), C && (0, e.jsx)(at, {
+                                }), o && (0, h.jsx)(aB, {
                                     className: Q.tabChart,
-                                    value: S,
+                                    value: T,
                                     index: 0,
                                     classes: {
                                         root: Q.tabChart
                                     },
-                                    children: (0, e.jsx)(ah, {
-                                        type: q,
-                                        name: E,
-                                        variant: H
+                                    children: (0, h.jsx)(ak, {
+                                        type: l,
+                                        name: q,
+                                        variant: z
                                     })
-                                }, "metrics"), !1, Object.keys(J).map(function(a, b) {
-                                    return (0, e.jsx)(at, {
+                                }, "metrics"), !1, Object.keys(H).map(function(a, b) {
+                                    return (0, h.jsx)(aB, {
                                         className: Q.tabChart,
-                                        value: S,
-                                        index: b + D,
+                                        value: T,
+                                        index: b + p,
                                         classes: {
                                             root: Q.tabChart
                                         },
-                                        children: (0, e.jsx)(t(), (0, j.Z)((0, i.Z)({
+                                        children: (0, h.jsx)(E(), (0, s.Z)((0, r.Z)({
                                             className: Q.tableRoot,
                                             detailPanel: function(b) {
-                                                return (0, e.jsx)(z._o, {
+                                                return (0, h.jsx)(O._o, {
                                                     type: a,
                                                     name: b.name,
                                                     row: b,
-                                                    setVariant: g
+                                                    setVariant: e
                                                 })
                                             },
-                                            title: W(a),
+                                            title: X(a),
                                             options: {
                                                 toolbar: !1,
                                                 headerStyle: {
-                                                    backgroundColor: as.ZP.palette.border.main,
+                                                    backgroundColor: N.ZP.palette.border.main,
                                                     marginLeft: 3
                                                 }
                                             }
-                                        }, Object.keys(J[a]).length > 0 ? {
+                                        }, Object.keys(H[a]).length > 0 ? {
                                             columns: ["name", "variant"].map(function(a) {
                                                 return {
-                                                    title: W(a),
+                                                    title: X(a),
                                                     field: a
                                                 }
                                             })
                                         } : {}), {
-                                            data: Object.entries(J[a]).map(function(a) {
+                                            data: Object.entries(H[a]).map(function(a) {
                                                 var b = a[0],
                                                     c = a[1],
                                                     d = {
                                                         name: b
                                                     };
                                                 return 1 === c.length ? d.variant = c[0].variant : d.variant = "...", d.variants = Object.values(c), d
                                             }),
                                             onRowClick: function(b, c) {
-                                                return u.push(ar.Z[a].urlPathResource(c.name))
+                                                return m.push(n.Z[a].urlPathResource(c.name))
                                             },
                                             components: {
                                                 Container: function(a) {
-                                                    return (0, e.jsx)("div", (0, i.Z)({
+                                                    return (0, h.jsx)("div", (0, r.Z)({
                                                         className: Q.resourceList,
-                                                        minwidth: "xl"
+                                                        style: {
+                                                            minWidth: "xl"
+                                                        }
                                                     }, a))
                                                 },
                                                 Body: function(a) {
-                                                    return (0, e.jsx)(s.MTableBody, (0, i.Z)({
+                                                    return (0, h.jsx)(D.MTableBody, (0, r.Z)({
                                                         className: Q.tableBody
                                                     }, a))
                                                 },
                                                 Header: function(a) {
-                                                    return (0, e.jsx)(s.MTableHeader, (0, i.Z)({
+                                                    return (0, h.jsx)(D.MTableHeader, (0, r.Z)({
                                                         className: Q.tableHeader
                                                     }, a))
                                                 }
                                             }
                                         }))
                                     }, a)
                                 })]
                             })]
                         })
                     })
                 },
-                ay = c(31607),
-                az = c(79895),
-                aA = c(93432),
-                aB = c(99520),
-                aC = function(a) {
+                aG = function(a) {
                     return {
                         fetch: function(b, c, d) {
-                            return a((0, h.H)({
+                            return a((0, q.H)({
                                 api: b,
                                 type: c,
                                 title: d
                             }))
                         },
                         setVariant: function(b, c, d) {
-                            return a((0, aA.jO)({
+                            return a((0, p.jO)({
                                 type: b,
                                 name: c,
                                 variant: d
                             }))
                         }
                     }
                 },
-                aD = function() {
-                    return (0, e.jsx)("div", {
+                aH = function() {
+                    return (0, h.jsx)("div", {
                         "data-testid": "loadingDotsId",
-                        children: (0, e.jsx)(w.Z, {
+                        children: (0, h.jsx)(i.Z, {
                             maxWidth: "xl",
-                            children: (0, e.jsx)(az.Z, {
+                            children: (0, h.jsx)(j.Z, {
                                 elevation: 3,
-                                children: (0, e.jsx)(w.Z, {
+                                children: (0, h.jsx)(i.Z, {
                                     maxWidth: "sm",
-                                    children: (0, e.jsx)(ay.Z, {
+                                    children: (0, h.jsx)(l.Z, {
                                         type: "ThreeDots",
                                         color: "grey",
                                         height: 40,
                                         width: 40
                                     })
                                 })
                             })
                         })
                     })
                 },
-                aE = function(a) {
+                aI = function(a) {
                     var b, c;
                     return !(null == a ? void 0 : null === (b = a.resources) || void 0 === b ? void 0 : b.name) && !(null == a ? void 0 : null === (c = a.resources) || void 0 === c ? void 0 : c.type)
                 },
-                aF = function(a) {
-                    var b, c = a.api,
-                        g = a.entityPage,
-                        h = a.activeVariants,
+                aJ = function(a) {
+                    var b = a.api,
+                        c = a.entityPage,
+                        f = a.activeVariants,
                         i = a.type,
                         j = a.entity,
-                        k = (0, d.Z)(a, ["api", "entityPage", "activeVariants", "type", "entity"]),
-                        l = ar.Z[ar.Z.pathToType[i]],
-                        m = k.fetch;
-                    return (0, f.useEffect)(function() {
-                        c && i && j && m(c, i, j)
-                    }, [i, j]), (0, e.jsx)("div", {
-                        children: g.failed || !g.loading && aE(g) ? (0, e.jsx)(aB.Z, {}) : g.loading || 0 === Object.keys(b = g).length && b.constructor === Object ? (0, e.jsx)(aD, {}) : (0, e.jsx)(ax, {
-                            entity: g,
-                            setVariant: k.setVariant,
-                            activeVariants: h,
+                        l = (0, e.Z)(a, ["api", "entityPage", "activeVariants", "type", "entity"]),
+                        m = n.Z[n.Z.pathToType[i]],
+                        p = l.fetch;
+                    return (0, k.useEffect)((0, d.Z)(g().mark(function a() {
+                        return g().wrap(function(a) {
+                            for (;;) switch (a.prev = a.next) {
+                                case 0:
+                                    if (!(b && i && j)) {
+                                        a.next = 3;
+                                        break
+                                    }
+                                    return a.next = 3, p(b, i, j);
+                                case 3:
+                                case "end":
+                                    return a.stop()
+                            }
+                        }, a)
+                    })), [i, j]), (0, h.jsx)("div", {
+                        children: c.loading ? (0, h.jsx)(aH, {}) : c.failed || !c.loading && aI(c) ? (0, h.jsx)(o.Z, {}) : (0, h.jsx)(aF, {
+                            entity: c,
+                            setVariant: l.setVariant,
+                            activeVariants: f,
                             typePath: i,
-                            resourceType: l
+                            resourceType: m
                         })
                     })
                 },
-                aG = (0, g.$j)(function(a) {
+                aK = (0, m.$j)(function(a) {
                     return {
                         entityPage: a.entityPage,
                         activeVariants: a.selectedVariant
                     }
-                }, aC)(aF)
+                }, aG)(aJ)
         },
         50462: function(a, b, c) {
             "use strict";
             c.d(b, {
                 H: function() {
                     return k
                 }
@@ -89698,27 +89686,24 @@
                             case 5:
                             case "end":
                                 return a.stop()
                         }
                     }, a)
                 })), function(a, b) {
                     return e.apply(this, arguments)
-                }), {
-                    condition: function(a, b) {
-                        a.api, a.type, a.title, b.getState
-                    }
-                }),
+                })),
                 l = (0, j.oM)({
                     name: "entityPage",
                     initialState: {},
                     extraReducers: (d = {}, (0, g.Z)(d, k.pending, function(a, b) {
                         var c = b.meta.requestId;
                         a.requestId = c, a.resources = null, a.loading = !0, a.failed = !1
                     }), (0, g.Z)(d, k.fulfilled, function(a, b) {
-                        b.meta.requestId === a.requestId && (a.resources = b.payload.data, a.loading = !1, a.failed = !1)
+                        var c;
+                        b.meta.requestId === a.requestId && (a.resources = null === (c = b.payload) || void 0 === c ? void 0 : c.data, a.loading = !1, a.failed = !1)
                     }), (0, g.Z)(d, k.rejected, function(a, b) {
                         b.meta.requestId === a.requestId && (a.loading = !1, a.failed = !0)
                     }), d)
                 });
             b.Z = l.reducer
         },
         89849: function(a, b, c) {
@@ -89746,28 +89731,29 @@
             "use strict";
             c.d(b, {
                 Z: function() {
                     return z
                 }
             });
             var d = c(85893),
-                e = c(67294),
-                f = c(41120),
-                g = c(14416),
-                h = c(7169),
-                i = c(26042),
-                j = c(69396),
-                k = c(99534),
-                l = c(92863),
-                m = c(11163),
-                n = c(282),
-                o = c(28889),
-                p = c(22318),
-                q = c(21286),
-                r = (0, f.Z)(function(a, b) {
+                e = c(41120),
+                f = c(22318),
+                g = c(67294),
+                h = c(14416),
+                i = c(7169),
+                j = c(41749),
+                k = c(26042),
+                l = c(69396),
+                m = c(99534),
+                n = c(28889),
+                o = c(282),
+                p = c(92863),
+                q = c(11163),
+                r = c(21286),
+                s = (0, e.Z)(function(a, b) {
                     return {
                         root: {
                             padding: a.spacing(2),
                             width: "100%",
                             height: "100%"
                         },
                         card: {
@@ -89824,96 +89810,95 @@
                         tileContent: {
                             display: "flex",
                             justifyContent: "space-around"
                         }
                     }
                 });
 
-            function s(a) {
+            function t(a) {
                 var b = a.children,
-                    c = (0, k.Z)(a, ["children"]),
-                    f = (0, e.useState)(!1),
-                    g = f[0],
-                    h = f[1];
-                return ((0, e.useEffect)(function() {
+                    c = (0, m.Z)(a, ["children"]),
+                    e = (0, g.useState)(!1),
+                    f = e[0],
+                    h = e[1];
+                return ((0, g.useEffect)(function() {
                     h(!0)
-                }, []), g) ? (0, d.jsx)("div", (0, j.Z)((0, i.Z)({}, c), {
+                }, []), f) ? (0, d.jsx)("div", (0, l.Z)((0, k.Z)({}, c), {
                     children: b
                 })) : null
             }
-            var t = function(a) {
+            var u = function(a) {
                     var b = a.detail,
                         c = a.id,
-                        e = (0, m.useRouter)(),
-                        f = q.Z[b.type],
-                        g = b.disabled,
-                        h = r(c),
-                        i = h.card;
-                    g && (i = h.buttonDisabled);
-                    var j = function(a) {
-                        e.push(f.urlPath)
+                        e = (0, q.useRouter)(),
+                        g = r.Z[b.type],
+                        h = b.disabled,
+                        i = s(c),
+                        j = i.card;
+                    h && (j = i.buttonDisabled);
+                    var k = function() {
+                        e.push(g.urlPath)
                     };
-                    return (0, d.jsx)(s, {
-                        children: (0, d.jsx)(o.Z, {
+                    return (0, d.jsx)(t, {
+                        children: (0, d.jsx)(n.Z, {
                             sx: {
                                 boxShadow: 3
                             },
                             children: (0, d.jsx)("div", {
-                                className: h.root,
-                                children: (0, d.jsx)(n.Z, {
-                                    className: i,
-                                    onClick: j,
-                                    disabled: g,
+                                className: i.root,
+                                children: (0, d.jsx)(o.Z, {
+                                    className: j,
+                                    onClick: k,
+                                    disabled: h,
                                     focusRipple: !0,
                                     variant: "contained",
                                     children: (0, d.jsxs)("div", {
-                                        className: h.tileContent,
+                                        className: i.tileContent,
                                         children: [(0, d.jsx)("div", {
-                                            children: (0, d.jsx)(l.Z, {
-                                                className: h.icon,
-                                                children: f.materialIcon
+                                            children: (0, d.jsx)(p.Z, {
+                                                className: i.icon,
+                                                children: g.materialIcon
                                             })
                                         }), (0, d.jsx)("div", {
-                                            children: (0, d.jsx)(p.Z, {
-                                                className: h.title,
+                                            children: (0, d.jsx)(f.Z, {
+                                                className: i.title,
                                                 variant: "h5",
                                                 children: (0, d.jsx)("b", {
-                                                    children: f.typePlural
+                                                    children: g.typePlural
                                                 })
                                             })
                                         })]
                                     })
                                 })
                             })
                         })
                     })
                 },
-                u = c(41749),
                 v = function(a) {
                     var b = a.sections;
                     return (0, d.jsx)("div", {
-                        children: (0, d.jsx)(u.Z, {
+                        children: (0, d.jsx)(j.Z, {
                             container: !0,
                             justifyContent: "center",
                             children: b.map(function(a, b) {
-                                return (0, d.jsx)(u.Z, {
+                                return (0, d.jsx)(j.Z, {
                                     item: !0,
                                     xs: 12,
                                     md: 6,
                                     lg: 4,
-                                    children: (0, d.jsx)(t, {
+                                    children: (0, d.jsx)(u, {
                                         detail: a,
                                         id: b
                                     }, "tile-".concat(b))
                                 }, "tile-grid-".concat(b))
                             })
                         })
                     })
                 },
-                w = (0, f.Z)(function(a) {
+                w = (0, e.Z)(function(a) {
                     return {
                         root: {
                             padding: a.spacing(0),
                             alignItems: "center",
                             justifyContent: "center"
                         },
                         search: {
@@ -89954,39 +89939,39 @@
                         c = w();
                     return (0, d.jsxs)("div", {
                         className: c.root,
                         children: [(0, d.jsxs)("div", {
                             className: c.search,
                             children: [(0, d.jsx)("div", {
                                 className: c.searchTitle
-                            }), (0, d.jsx)(h.Z, {
+                            }), (0, d.jsx)(i.Z, {
                                 homePage: !0
                             })]
                         }), (0, d.jsx)("div", {
                             className: c.sections,
                             children: (0, d.jsxs)("div", {
                                 className: c.tilePanel,
                                 children: [(0, d.jsx)("div", {
                                     className: c.title,
-                                    children: (0, d.jsx)(p.Z, {
+                                    children: (0, d.jsx)(f.Z, {
                                         variant: "h5"
                                     })
                                 }), (0, d.jsx)(v, {
                                     sections: b.features
                                 })]
                             })
                         })]
                     })
                 },
                 y = function(a) {
                     return {
                         sections: a.homePageSections
                     }
                 },
-                z = (0, g.$j)(y)(x)
+                z = (0, h.$j)(y)(x)
         },
         99520: function(a, b, c) {
             "use strict";
             var d = c(85893);
             c(67294);
             var e = function() {
                 return (0, d.jsx)("div", {
@@ -90009,32 +89994,27 @@
                 e = c(52951);
 
             function f(a, b) {
                 return (f = Object.setPrototypeOf || function(a, b) {
                     return a.__proto__ = b, a
                 })(a, b)
             }
-            var g = c(26042),
-                h = c(99534);
+            var g = c(26042);
 
-            function i(a) {
-                return (i = Object.setPrototypeOf ? Object.getPrototypeOf : function(a) {
+            function h(a) {
+                return (h = Object.setPrototypeOf ? Object.getPrototypeOf : function(a) {
                     return a.__proto__ || Object.getPrototypeOf(a)
                 })(a)
             }
-            var j = c(85893),
-                k = c(67294),
-                l = c(45697),
-                m = c.n(l),
-                n = c(14416),
-                o = "NOT_FOUND",
-                p = function(a, b) {
+            var i = c(85893),
+                j = "NOT_FOUND",
+                k = function(a, b) {
                     return a === b
                 },
-                q = function(a) {
+                l = function(a) {
                     for (var b = arguments.length, c = Array(b > 1 ? b - 1 : 0), d = 1; d < b; d++) c[d - 1] = arguments[d];
                     return function() {
                         for (var b, d = arguments.length, e = Array(d), f = 0; f < d; f++) e[f] = arguments[f];
                         var g = 0,
                             h = {
                                 memoizeOptions: void 0
                             },
@@ -90077,24 +90057,24 @@
                 }(function(a, b) {
                     var c, d, e, f = "object" == typeof b ? b : {
                             equalityCheck: b
                         },
                         g = f.equalityCheck,
                         h = f.maxSize,
                         i = void 0 === h ? 1 : h,
-                        j = f.resultEqualityCheck,
-                        k = (c = void 0 === g ? p : g, function(a, b) {
+                        l = f.resultEqualityCheck,
+                        m = (c = void 0 === g ? k : g, function(a, b) {
                             if (null === a || null === b || a.length !== b.length) return !1;
                             for (var d = a.length, e = 0; e < d; e++)
                                 if (!c(a[e], b[e])) return !1;
                             return !0
                         }),
-                        l = 1 === i ? (d = k, {
+                        n = 1 === i ? (d = m, {
                             get: function(a) {
-                                return e && d(e.key, a) ? e.value : o
+                                return e && d(e.key, a) ? e.value : j
                             },
                             put: function(a, b) {
                                 e = {
                                     key: a,
                                     value: b
                                 }
                             },
@@ -90111,67 +90091,72 @@
                                 var d = c.findIndex(function(c) {
                                     return b(a, c.key)
                                 });
                                 if (d > -1) {
                                     var e = c[d];
                                     return d > 0 && (c.splice(d, 1), c.unshift(e)), e.value
                                 }
-                                return o
+                                return j
                             }
 
                             function e() {
                                 return c
                             }
                             return {
                                 get: d,
                                 put: function(b, e) {
-                                    d(b) === o && (c.unshift({
+                                    d(b) === j && (c.unshift({
                                         key: b,
                                         value: e
                                     }), c.length > a && c.pop())
                                 },
                                 getEntries: e,
                                 clear: function() {
                                     c = []
                                 }
                             }
-                        }(i, k);
+                        }(i, m);
 
-                    function m() {
-                        var b = l.get(arguments);
-                        if (b === o) {
-                            if (b = a.apply(null, arguments), j) {
-                                var c = l.getEntries().find(function(a) {
-                                    return j(a.value, b)
+                    function o() {
+                        var b = n.get(arguments);
+                        if (b === j) {
+                            if (b = a.apply(null, arguments), l) {
+                                var c = n.getEntries().find(function(a) {
+                                    return l(a.value, b)
                                 });
                                 c && (b = c.value)
                             }
-                            l.put(arguments, b)
+                            n.put(arguments, b)
                         }
                         return b
                     }
-                    return m.clearCache = function() {
-                        return l.clear()
-                    }, m
+                    return o.clearCache = function() {
+                        return n.clear()
+                    }, o
                 }),
-                r = c(16332),
-                s = c(88802),
-                t = c(93432),
-                u = c(5378),
-                v = function() {
-                    return (0, j.jsx)("div", {
-                        children: (0, j.jsx)("h1", {
+                m = c(45697),
+                n = c.n(m),
+                o = c(67294),
+                p = c(14416),
+                q = function() {
+                    return (0, i.jsx)("div", {
+                        children: (0, i.jsx)("h1", {
                             children: "500 Server Error"
                         })
                     })
                 },
+                r = q,
+                s = c(88802),
+                t = c(16332),
+                u = c(5378),
+                v = c(93432),
                 w = function(a, b) {
                     var c = b.type;
                     return function(a) {
-                        var b, d = (b = c, q(function(a) {
+                        var b, d = (b = c, l(function(a) {
                                 return a.resourceList[b].resources
                             }, function(a) {
                                 return a.selectedTags[b]
                             }, function(a) {
                                 return a.selectedVariant[b]
                             }, function(a, b, c) {
                                 if (!a) return null;
@@ -90201,21 +90186,21 @@
                 },
                 x = function(a, b) {
                     return function(a) {
                         return {
                             fetch: function() {
                                 var c = b.type,
                                     d = b.api;
-                                a((0, r.eL)({
+                                a((0, t.eL)({
                                     api: d,
                                     type: c
                                 }))
                             },
                             setVariant: function(b, c, d) {
-                                a((0, t.jO)({
+                                a((0, v.jO)({
                                     type: b,
                                     name: c,
                                     variant: d
                                 }))
                             },
                             toggleTag: function(c) {
                                 var d = b.type;
@@ -90236,169 +90221,168 @@
                                     writable: !0,
                                     configurable: !0
                                 }
                             }), b) {
                             var c, d;
                             c = a, f(c, d = b)
                         }
-                    }(l, a);
-                    var b, c, k = (b = l, c = function() {
+                    }(k, a);
+                    var b, c, j = (b = k, c = function() {
                         if ("undefined" == typeof Reflect || !Reflect.construct || Reflect.construct.sham) return !1;
                         if ("function" == typeof Proxy) return !0;
                         try {
                             return Boolean.prototype.valueOf.call(Reflect.construct(Boolean, [], function() {})), !0
                         } catch (a) {
                             return !1
                         }
                     }(), function() {
-                        var a, d, e, f, g, h = i(f = b);
+                        var a, d, e, f, g, i = h(f = b);
                         if (c) {
-                            var j, k = (j = this, i(j)).constructor;
-                            g = Reflect.construct(h, arguments, k)
-                        } else g = h.apply(this, arguments);
+                            var j, k = (j = this, h(j)).constructor;
+                            g = Reflect.construct(i, arguments, k)
+                        } else g = i.apply(this, arguments);
                         return a = this, (d = g) && ("object" == ((e = d) && e.constructor === Symbol ? "symbol" : typeof e) || "function" == typeof d) ? d : function(a) {
                             if (void 0 === a) throw ReferenceError("this hasn't been initialised - super() hasn't been called");
                             return a
                         }(a)
                     });
 
-                    function l() {
-                        return (0, d.Z)(this, l), k.apply(this, arguments)
+                    function k() {
+                        return (0, d.Z)(this, k), j.apply(this, arguments)
                     }
-                    return (0, e.Z)(l, [{
+                    return (0, e.Z)(k, [{
                         key: "componentDidMount",
                         value: function() {
                             this.props.fetch()
                         }
                     }, {
                         key: "render",
                         value: function() {
-                            var a = this.props,
-                                b = (a.api, a.fetch, (0, h.Z)(a, ["api", "fetch"]));
-                            return b.failed ? (0, j.jsx)(v, {}) : (0, j.jsx)(s.ZP, (0, g.Z)({}, b))
+                            var a = (0, g.Z)({}, this.props);
+                            return delete a.api, delete a.fetch, a.failed ? (0, i.jsx)(r, {}) : (0, i.jsx)(s.ZP, (0, g.Z)({}, a))
                         }
-                    }]), l
-                }(k.Component);
+                    }]), k
+                }(o.Component);
             y.propTypes = {
-                type: m().string.isRequired,
-                api: m().object.isRequired,
-                title: m().string,
-                resources: m().array,
-                loading: m().bool,
-                failed: m().bool
+                type: n().string.isRequired,
+                api: n().object.isRequired,
+                title: n().string,
+                resources: n().array,
+                loading: n().bool,
+                failed: n().bool
             };
-            var z = (0, n.$j)(w, x)(y)
+            var z = (0, p.$j)(w, x)(y)
         },
         88802: function(a, b, c) {
             "use strict";
             c.d(b, {
                 "_o": function() {
                     return D
                 }
             });
             var d = c(26042),
                 e = c(69396),
                 f = c(70603),
-                g = c(85893);
+                g = c(85893),
+                h = c(282),
+                i = c(16204),
+                j = c(43832),
+                k = c(41749),
+                l = c(41120),
+                m = c(22318),
+                n = c(73103),
+                o = c(26283),
+                p = c.n(o),
+                q = c(11163),
+                r = c(45697),
+                s = c.n(r);
             c(67294);
-            var h = c(45697),
-                i = c.n(h),
-                j = c(41120),
-                k = c(11163),
-                l = c(22318),
-                m = c(41749),
-                n = c(16204),
-                o = c(48535),
-                p = c(73103),
-                q = c(26283),
-                r = c.n(q),
-                s = c(30640),
-                t = c(902),
-                u = c(61139),
-                v = c(17852),
-                w = c(43832),
+            var t = c(30640),
+                u = c(17852),
+                v = c(902),
+                w = c(61139),
                 x = c(13824),
-                y = c(282),
-                z = c(21286);
-            s.Z.registerLanguage("python", t.Z), s.Z.registerLanguage("sql", u.Z), s.Z.registerLanguage("json", v.Z);
-            var A = (0, j.Z)(function() {
+                y = c(21286),
+                z = c(48535);
+            t.Z.registerLanguage("python", v.Z), t.Z.registerLanguage("sql", w.Z), t.Z.registerLanguage("json", u.Z);
+            var A = (0, l.Z)(function() {
                     return {
                         root: {
                             background: "rgba(255, 255, 255, 0.5)",
-                            border: "2px solid ".concat(o.ZP.palette.border.main),
+                            border: "2px solid ".concat(z.ZP.palette.border.main),
                             borderRadius: 16,
                             "& > *": {
                                 borderRadius: 16
                             }
                         },
                         noDataPage: {
                             "& > *": {
-                                padding: o.ZP.spacing(1)
+                                padding: z.ZP.spacing(1)
                             }
                         },
                         table: {
                             borderRadius: 16,
                             background: "rgba(255, 255, 255, 1)",
-                            border: "2px solid ".concat(o.ZP.palette.border.main)
+                            border: "2px solid ".concat(z.ZP.palette.border.main)
                         },
                         usageIcon: {
                             color: "red"
                         },
                         variantTableContainer: {
-                            marginLeft: o.ZP.spacing(4),
-                            marginRight: o.ZP.spacing(4)
+                            marginLeft: z.ZP.spacing(4),
+                            marginRight: z.ZP.spacing(4)
                         },
                         variantTable: {
                             background: "rgba(255, 255, 255, 1)",
-                            border: "2px solid ".concat(o.ZP.palette.border.main)
+                            border: "2px solid ".concat(z.ZP.palette.border.main)
                         },
                         detailPanel: {
-                            padding: o.ZP.spacing(4)
+                            padding: z.ZP.spacing(4)
                         },
                         config: {
                             width: "100%"
                         },
                         detailButton: {
-                            margin: o.ZP.spacing(1)
+                            margin: z.ZP.spacing(1)
                         },
                         tag: {
-                            margin: o.ZP.spacing(.1)
+                            margin: z.ZP.spacing(.1)
                         },
                         tableBody: {
-                            border: "2px solid ".concat(o.ZP.palette.border.main),
+                            border: "2px solid ".concat(z.ZP.palette.border.main),
                             background: "white",
                             color: "white",
                             opacity: 1
                         },
                         providerColumn: {},
                         providerLogo: {
                             maxWidth: "6em",
                             maxHeight: "2.5em"
                         },
                         tableToolbar: {
-                            paddingTop: o.ZP.spacing(3),
-                            paddingBottom: o.ZP.spacing(1)
+                            paddingTop: z.ZP.spacing(3),
+                            paddingBottom: z.ZP.spacing(1)
                         }
                     }
                 }),
                 B = function(a) {
                     var b, c = a.title,
                         h = a.resources,
                         i = a.loading,
-                        j = a.failed,
-                        m = a.type,
+                        k = a.failed,
+                        l = a.type,
                         n = a.activeTags,
-                        p = a.activeVariants,
-                        s = void 0 === p ? {} : p,
+                        r = a.activeVariants,
+                        s = void 0 === r ? {} : r,
                         t = a.setVariant,
                         u = a.toggleTag,
                         v = function(a, b) {
                             E.push(E.query.type + "/" + b.name)
                         },
-                        y = {
+                        w = {
                             default: [{
                                 title: "Name",
                                 field: "name"
                             }, {
                                 title: "Description",
                                 field: "description"
                             }, ],
@@ -90436,15 +90420,15 @@
                             }, {
                                 title: "Type",
                                 field: "data-type"
                             }, {
                                 title: "Default Variant",
                                 field: "variants",
                                 render: function(a) {
-                                    return (0, g.jsx)(l.Z, {
+                                    return (0, g.jsx)(m.Z, {
                                         variant: "body1",
                                         children: a["default-variant"]
                                     })
                                 }
                             }, ],
                             Provider: [{
                                 title: "Name",
@@ -90507,50 +90491,50 @@
                                         toggleTag: u
                                     })
                                 }
                             }, {
                                 title: "Default Variant",
                                 field: "variants",
                                 render: function(a) {
-                                    return (0, g.jsx)(l.Z, {
+                                    return (0, g.jsx)(m.Z, {
                                         variant: "body1",
                                         children: J.find(function(b) {
                                             return b.name === a.name
                                         })["default-variant"]
                                     })
                                 }
                             }, ]
                         },
                         B = A(),
-                        E = (0, k.useRouter)(),
+                        E = (0, q.useRouter)(),
                         G = null == h && !i,
-                        H = !z.Z[m].hasVariants,
+                        H = !y.Z[l].hasVariants,
                         I = (b = h || []).map(function(a) {
                             return (0, d.Z)({}, a)
                         }),
                         J = {};
                     return (0, g.jsx)("div", {
-                        children: (0, g.jsx)(r(), (0, d.Z)((0, e.Z)((0, d.Z)({}, H ? {} : {
+                        children: (0, g.jsx)(p(), (0, d.Z)((0, e.Z)((0, d.Z)({}, H ? {} : {
                             detailPanel: function(a) {
                                 return (0, g.jsx)(D, {
                                     name: a.name,
                                     row: a,
-                                    type: m,
+                                    type: l,
                                     setVariant: t
                                 })
                             }
                         }), {
                             className: B.table,
-                            title: (0, g.jsx)(l.Z, {
+                            title: (0, g.jsx)(m.Z, {
                                 variant: "h4",
                                 children: (0, g.jsx)("b", {
-                                    children: z.Z[m].typePlural
+                                    children: y.Z[l].typePlural
                                 })
                             }),
-                            columns: Object.keys(y).includes(c) ? y[c] : y.default,
+                            columns: Object.keys(w).includes(c) ? w[c] : w.default,
                             data: I.map(function(a) {
                                 var b = {};
                                 if (!a.variants) {
                                     var c = !0,
                                         d = !1,
                                         e = void 0;
                                     try {
@@ -90592,57 +90576,57 @@
                                     }
                                 }
                                 var x = [];
                                 return Object.values(a.variants).forEach(function(a) {
                                     x.push(a)
                                 }), b.variants = x, b["default-variant"] = a["default-variant"], b
                             }),
-                            isLoading: G || i || j,
+                            isLoading: G || i || k,
                             onRowClick: v,
                             components: {
                                 Container: function(a) {
-                                    return (0, g.jsx)(w.Z, (0, d.Z)({
+                                    return (0, g.jsx)(j.Z, (0, d.Z)({
                                         maxWidth: "xl",
                                         className: B.root
                                     }, a))
                                 },
                                 Body: function(a) {
-                                    return (0, g.jsx)(q.MTableBody, (0, d.Z)({
+                                    return (0, g.jsx)(o.MTableBody, (0, d.Z)({
                                         style: {
                                             borderRadius: 16
                                         },
                                         className: B.tableBody
                                     }, a))
                                 },
                                 Header: function(a) {
-                                    return (0, g.jsx)(q.MTableHeader, (0, d.Z)({
+                                    return (0, g.jsx)(o.MTableHeader, (0, d.Z)({
                                         className: B.tableBody
                                     }, a))
                                 },
                                 Toolbar: function(a) {
                                     return (0, g.jsx)("div", {
                                         className: B.tableToolbar,
-                                        children: (0, g.jsx)(q.MTableToolbar, (0, d.Z)({}, a))
+                                        children: (0, g.jsx)(o.MTableToolbar, (0, d.Z)({}, a))
                                     })
                                 }
                             },
                             options: {
                                 search: !0,
                                 draggable: !1,
                                 headerStyle: {
                                     backgroundColor: "white",
-                                    color: o.ZP.palette.primary.main,
+                                    color: z.ZP.palette.primary.main,
                                     marginLeft: 3
                                 },
                                 rowStyle: {
                                     opacity: 1,
                                     borderRadius: 16
                                 }
                             }
-                        }), G || i || j ? {} : {
+                        }), G || i || k ? {} : {
                             localization: {
                                 body: {
                                     emptyDataSourceMessage: (0, g.jsx)(F, {
                                         type: c
                                     })
                                 }
                             }
@@ -90651,19 +90635,19 @@
                 },
                 C = function(a) {
                     var b = a.activeTags,
                         c = void 0 === b ? {} : b,
                         d = a.tags,
                         e = a.tagClass,
                         f = a.toggleTag;
-                    return (0, g.jsx)(m.Z, {
+                    return (0, g.jsx)(k.Z, {
                         container: !0,
                         direction: "row",
                         children: (void 0 === d ? [] : d).map(function(a) {
-                            return (0, g.jsx)(n.Z, {
+                            return (0, g.jsx)(i.Z, {
                                 className: e,
                                 color: c[a] ? "secondary" : "default",
                                 onClick: function(b) {
                                     f(a), b.stopPropagation()
                                 },
                                 variant: "outlined",
                                 label: a
@@ -90673,143 +90657,143 @@
                 },
                 D = function(a) {
                     var b = a.name,
                         c = a.setVariant,
                         e = a.type,
                         f = a.row,
                         h = function(a, d) {
-                            c(e, b, d.variant), j.push(z.Z[e].urlPathResource(b))
+                            c(e, b, d.variant), k.push(y.Z[e].urlPathResource(b))
                         },
                         i = A(),
-                        j = (0, k.useRouter)(),
-                        m = [];
+                        k = (0, q.useRouter)(),
+                        l = [];
                     return f.variants.forEach(function(a) {
-                        m.push({
+                        l.push({
                             variant: a.variant,
                             description: a.description
                         })
                     }), (0, g.jsx)("div", {
                         className: i.variantTableContainer,
-                        children: (0, g.jsx)(r(), {
+                        children: (0, g.jsx)(p(), {
                             className: i.variantTable,
-                            title: (0, g.jsx)(l.Z, {
+                            title: (0, g.jsx)(m.Z, {
                                 variant: "h6",
                                 children: (0, g.jsx)("b", {})
                             }),
                             onRowClick: h,
                             components: {
                                 Container: function(a) {
-                                    return (0, g.jsx)(w.Z, (0, d.Z)({
+                                    return (0, g.jsx)(j.Z, (0, d.Z)({
                                         maxWidth: "xl",
                                         className: i.variantTable
                                     }, a))
                                 },
                                 Body: function(a) {
-                                    return (0, g.jsx)(q.MTableBody, (0, d.Z)({
+                                    return (0, g.jsx)(o.MTableBody, (0, d.Z)({
                                         style: {
                                             borderRadius: 16
                                         },
                                         className: i.tableBody
                                     }, a))
                                 },
                                 Header: function(a) {
-                                    return (0, g.jsx)(q.MTableHeader, (0, d.Z)({
+                                    return (0, g.jsx)(o.MTableHeader, (0, d.Z)({
                                         className: i.tableBody
                                     }, a))
                                 },
                                 Toolbar: function(a) {
                                     return (0, g.jsx)("div", {
                                         className: i.tableToolbar,
-                                        children: (0, g.jsx)(q.MTableToolbar, (0, d.Z)({}, a))
+                                        children: (0, g.jsx)(o.MTableToolbar, (0, d.Z)({}, a))
                                     })
                                 }
                             },
                             columns: [{
                                 title: "Variants",
                                 field: "variant"
                             }, {
                                 title: "Description",
                                 field: "description"
                             }, ],
-                            data: m,
+                            data: l,
                             options: {
                                 search: !0,
                                 pageSize: f.variants.length,
                                 maxHeight: "".concat(25, "em"),
                                 toolbar: !1,
                                 draggable: !1,
                                 headerStyle: {
                                     backgroundColor: "white",
-                                    color: o.ZP.palette.primary.main,
+                                    color: z.ZP.palette.primary.main,
                                     marginLeft: 3
                                 },
                                 rowStyle: {
                                     opacity: 1,
                                     borderRadius: 16,
                                     height: "".concat(5, "em")
                                 }
                             }
                         })
                     })
                 },
                 E = {
                     1: {
-                        icon: (0, g.jsx)(p.Z, {}),
+                        icon: (0, g.jsx)(n.Z, {}),
                         label: "Unused"
                     },
                     2: {
-                        icon: (0, g.jsx)(p.Z, {}),
+                        icon: (0, g.jsx)(n.Z, {}),
                         label: "Dissatisfied"
                     },
                     3: {
-                        icon: (0, g.jsx)(p.Z, {}),
+                        icon: (0, g.jsx)(n.Z, {}),
                         label: "Neutral"
                     },
                     4: {
-                        icon: (0, g.jsx)(p.Z, {}),
+                        icon: (0, g.jsx)(n.Z, {}),
                         label: "Satisfied"
                     },
                     5: {
-                        icon: (0, g.jsx)(p.Z, {}),
+                        icon: (0, g.jsx)(n.Z, {}),
                         label: "Frequently used"
                     }
                 },
                 F = function(a) {
                     var b = a.type,
                         c = function() {
                             window.location.href = "https://docs.featureform.com/quickstart"
                         },
                         d = A();
-                    return (0, g.jsx)(w.Z, {
+                    return (0, g.jsx)(j.Z, {
                         children: (0, g.jsxs)("div", {
                             className: d.noDataPage,
-                            children: [(0, g.jsxs)(l.Z, {
+                            children: [(0, g.jsxs)(m.Z, {
                                 variant: "h4",
-                                children: ["No ", z.Z[b].typePlural, " Registered"]
-                            }), (0, g.jsxs)(l.Z, {
+                                children: ["No ", y.Z[b].typePlural, " Registered"]
+                            }), (0, g.jsxs)(m.Z, {
                                 variant: "body1",
                                 children: ["There are no visible ", b.toLowerCase(), "s in your organization."]
-                            }), (0, g.jsx)(l.Z, {
+                            }), (0, g.jsx)(m.Z, {
                                 vairant: "body1",
                                 children: "Check out our docs for step by step instructions to create one."
-                            }), (0, g.jsx)(y.Z, {
+                            }), (0, g.jsx)(h.Z, {
                                 variant: "outlined",
                                 onClick: c,
                                 children: "FeatureForm Docs"
                             })]
                         })
                     })
                 };
             B.propTypes = {
-                title: i().string.isRequired,
-                resources: i().array,
-                loading: i().bool,
-                failed: i().bool,
-                activeVariants: i().object,
-                setVariant: i().func
+                title: s().string.isRequired,
+                resources: s().array,
+                loading: s().bool,
+                failed: s().bool,
+                activeVariants: s().object,
+                setVariant: s().func
             }, b.ZP = B
         },
         16332: function(a, b, c) {
             "use strict";
             c.d(b, {
                 eL: function() {
                     return n
@@ -90951,31 +90935,31 @@
             b.ZP = h.reducer
         },
         7169: function(a, b, c) {
             "use strict";
             var d = c(14924),
                 e = c(70603),
                 f = c(85893),
-                g = c(67294),
-                h = c(41120),
-                i = c(35117),
-                j = c(59693),
-                k = c(88995),
-                l = c(41749),
-                m = c(11163),
-                n = c(43832),
-                o = c(41598),
-                p = (0, h.Z)(function(a) {
-                    return (0, i.Z)({
+                g = c(43832),
+                h = c(41749),
+                i = c(41598),
+                j = c(41120),
+                k = c(35117),
+                l = c(59693),
+                m = c(88995),
+                n = c(11163),
+                o = c(67294),
+                p = (0, j.Z)(function(a) {
+                    return (0, k.Z)({
                         search: (0, d.Z)({
                             position: "relative",
                             borderRadius: a.shape.borderRadius,
-                            backgroundColor: (0, j.Fq)(a.palette.common.white, .15),
+                            backgroundColor: (0, l.Fq)(a.palette.common.white, .15),
                             "&:hover": {
-                                backgroundColor: (0, j.Fq)(a.palette.common.white, .25)
+                                backgroundColor: (0, l.Fq)(a.palette.common.white, .25)
                             },
                             marginLeft: 0,
                             width: "100%"
                         }, a.breakpoints.up("sm"), {
                             marginLeft: a.spacing(1),
                             width: "auto"
                         }),
@@ -91026,48 +91010,48 @@
                         }
                     })
                 }),
                 q = function(a) {
                     var b = a.homePage,
                         c = function(a) {
                             a.preventDefault();
-                            var b = "/search?q=" + (null == j ? void 0 : j.trim());
-                            h.push(b)
+                            var b = "/query?q=" + (null == l ? void 0 : l.trim());
+                            j.push(b)
                         },
                         d = p(),
-                        h = (0, m.useRouter)(),
-                        i = (0, e.Z)(g.useState(""), 2),
-                        j = i[0],
-                        q = i[1];
+                        j = (0, n.useRouter)(),
+                        k = (0, e.Z)(o.useState(""), 2),
+                        l = k[0],
+                        q = k[1];
                     return (0, f.jsx)("div", {
                         className: d.search,
-                        children: (0, f.jsx)(l.Z, {
+                        children: (0, f.jsx)(h.Z, {
                             container: !0,
                             item: !0,
                             justifyContent: "center",
                             direction: "row",
-                            children: (0, f.jsxs)(n.Z, {
+                            children: (0, f.jsxs)(g.Z, {
                                 className: d.border,
                                 children: [(0, f.jsx)("div", {
                                     className: d.searchIcon,
-                                    children: (0, f.jsx)(k.Z, {})
-                                }), (0, f.jsx)(o.Z, {
+                                    children: (0, f.jsx)(m.Z, {})
+                                }), (0, f.jsx)(i.Z, {
                                     placeholder: "Search...",
                                     onChange: function(a) {
                                         var b, c = a.target.value;
                                         if ("" === c) {
                                             q(c);
                                             return
                                         }
                                         var d = null !== (b = a.target.value) && void 0 !== b ? b : "";
                                         d.trim() && q(d)
                                     },
-                                    value: j,
+                                    value: l,
                                     onKeyDown: function(a) {
-                                        "Enter" === a.key && j && c(a)
+                                        "Enter" === a.key && l && c(a)
                                     },
                                     classes: {
                                         root: d.inputRoot,
                                         input: b ? d.inputInputHome : d.inputTopBar
                                     },
                                     inputProps: {
                                         "aria-label": "search",
@@ -91080,56 +91064,58 @@
                 };
             b.Z = q
         },
         88277: function(a, b, c) {
             "use strict";
             c.d(b, {
                 Z: function() {
-                    return E
+                    return F
                 }
             });
             var d = c(99534),
                 e = c(85893),
-                f = c(67294),
-                g = c(14416),
-                h = c(26042),
-                i = c(69396),
-                j = c(45697),
-                k = c.n(j),
-                l = c(41120),
-                m = c(22318),
-                n = c(28889),
+                f = c(11163),
+                g = c(67294),
+                h = c(14416),
+                i = c(93432),
+                j = c(75820),
+                k = c(26042),
+                l = c(69396),
+                m = c(28889),
+                n = c(43832),
                 o = c(62822),
                 p = c(50998),
                 q = c(95757),
-                r = c(43832),
-                s = c(21286),
-                t = c(11163);
+                r = c(41120),
+                s = c(22318),
+                t = c(45697),
+                u = c.n(t),
+                v = c(21286);
             (function(a) {
                 var b = a.children,
                     c = a.value,
                     f = a.index,
                     g = (0, d.Z)(a, ["children", "value", "index"]);
-                return (0, e.jsx)("div", (0, i.Z)((0, h.Z)({
+                return (0, e.jsx)("div", (0, l.Z)((0, k.Z)({
                     role: "tabpanel",
                     hidden: c !== f,
                     id: "simple-tabpanel-".concat(f),
                     "aria-labelledby": "simple-tab-".concat(f)
                 }, g), {
-                    children: c === f && (0, e.jsx)(n.Z, {
+                    children: c === f && (0, e.jsx)(m.Z, {
                         p: 3,
                         children: b
                     })
                 }))
             }).propTypes = {
-                children: k().node,
-                index: k().any.isRequired,
-                value: k().any.isRequired
+                children: u().node,
+                index: u().any.isRequired,
+                value: u().any.isRequired
             };
-            var u = (0, l.Z)(function(a) {
+            var w = (0, r.Z)(function(a) {
                     return {
                         root: {
                             borderRadius: 16,
                             background: "rgba(255, 255, 255, 1)",
                             border: "2px solid ".concat(a.palette.border.main)
                         },
                         appbar: {
@@ -91146,173 +91132,171 @@
                         },
                         resultTitle: {
                             display: "inline",
                             lineHeight: 1.2
                         }
                     }
                 }),
-                v = function(a) {
+                x = function(a) {
+                    var b = a.results,
+                        c = a.search_query,
+                        d = a.setVariant,
+                        f = w();
+                    return (0, e.jsx)("div", {
+                        children: (0, e.jsxs)(n.Z, {
+                            maxWidth: "xl",
+                            className: f.root,
+                            children: [(0, e.jsxs)(s.Z, {
+                                className: f.searchTitle,
+                                variant: "h4",
+                                style: {
+                                    display: "flex"
+                                },
+                                children: [(null == b ? void 0 : b.length) > 0 ? (0, e.jsx)("div", {
+                                    style: {
+                                        color: "gray"
+                                    },
+                                    children: "Results for:\xa0"
+                                }) : (0, e.jsx)("div", {
+                                    style: {
+                                        color: "gray"
+                                    },
+                                    children: "No results for:\xa0"
+                                }), (0, e.jsx)("b", {
+                                    children: c
+                                })]
+                            }), (0, e.jsx)(y, {
+                                contents: b,
+                                setVariant: d
+                            })]
+                        })
+                    })
+                },
+                y = function(a) {
                     var b = a.type,
                         c = a.contents,
                         d = a.setVariant,
-                        f = u(),
+                        f = w(),
                         g = {},
                         h = [];
                     return (null == c ? void 0 : c.length) && (h = c.filter(function(a) {
                         return !(a.Name + "." + a.Variant + "." + a.Type in g) && (g[a.Name + "." + a.Variant + "." + a.Type] = a.Variant, !0)
                     })), (0, e.jsx)("div", {
                         children: (0, e.jsx)(o.Z, {
                             className: f.root,
                             component: "nav",
                             children: h.map(function(a, c) {
-                                return (0, e.jsx)(x, {
+                                return (0, e.jsx)(A, {
                                     type: b,
                                     content: a,
                                     setVariant: d
                                 }, c)
                             })
                         })
                     })
                 },
-                w = {
+                z = Object.freeze({
                     FEATURE: "Feature",
                     FEATURE_VARIANT: "Feature",
                     LABEL: "Label",
                     LABEL_VARIANT: "Label",
                     TRAINING_SET: "TrainingSet",
                     TRAINING_SET_VARIANT: "TrainingSet",
                     SOURCE: "Source",
                     SOURCE_VARIANT: "Source",
                     PROVIDER: "Provider",
                     ENTITY: "Entity",
                     MODEL: "Model",
                     USER: "User"
-                },
-                x = function(a) {
-                    a.type;
-                    var b = a.content,
-                        c = a.setVariant,
-                        d = function(a) {
-                            (null == h ? void 0 : h.hasVariants) && c(a.Type, a.Name, a.Variant), g.push(h.urlPathResource(a.Name))
+                }),
+                A = function(a) {
+                    var b, c = a.content,
+                        d = a.setVariant,
+                        g = function(a) {
+                            (null == j ? void 0 : j.hasVariants) && d(a.Type, a.Name, a.Variant), i.push(j.urlPathResource(a.Name))
                         },
-                        f = u(),
-                        g = (0, t.useRouter)(),
-                        h = s.Z[w[b.Type]];
+                        h = w(),
+                        i = (0, f.useRouter)(),
+                        j = v.Z[z[null === (b = c.Type) || void 0 === b ? void 0 : b.toUpperCase()]];
                     return (0, e.jsx)(e.Fragment, {
                         children: (0, e.jsx)(p.Z, {
                             button: !0,
                             alignItems: "flex-start",
                             onClick: function() {
-                                return d(b)
+                                return g(c)
                             },
                             children: (0, e.jsx)(q.Z, {
                                 primary: (0, e.jsxs)("div", {
                                     children: [(0, e.jsxs)("div", {
                                         children: [(0, e.jsx)("div", {
-                                            className: f.resultTitle
-                                        }), (0, e.jsx)(m.Z, {
-                                            className: f.resultTitle,
+                                            className: h.resultTitle
+                                        }), (0, e.jsx)(s.Z, {
+                                            className: h.resultTitle,
                                             variant: "h6",
-                                            children: b.Name
+                                            children: c.Name
                                         }), " "]
                                     }), (0, e.jsx)("div", {
                                         style: {
                                             width: "0.5em"
                                         },
                                         children: "   "
-                                    }), (0, e.jsx)(m.Z, {
+                                    }), (0, e.jsx)(s.Z, {
                                         style: {
                                             opacity: .5
                                         },
-                                        className: f.resultTitle,
+                                        className: h.resultTitle,
                                         variant: "body1",
-                                        children: b.Variant
+                                        children: c.Variant
                                     })]
                                 })
                             })
                         })
                     })
                 },
-                y = function(a) {
-                    var b = a.results,
-                        c = a.search_query,
-                        d = a.setVariant,
-                        f = u();
-                    return (0, e.jsx)("div", {
-                        children: (0, e.jsxs)(r.Z, {
-                            maxWidth: "xl",
-                            className: f.root,
-                            children: [(0, e.jsxs)(m.Z, {
-                                className: f.searchTitle,
-                                variant: "h4",
-                                style: {
-                                    display: "flex"
-                                },
-                                children: [(null == b ? void 0 : b.length) > 0 ? (0, e.jsx)("div", {
-                                    style: {
-                                        color: "gray"
-                                    },
-                                    children: "Results for:\xa0"
-                                }) : (0, e.jsx)("div", {
-                                    style: {
-                                        color: "gray"
-                                    },
-                                    children: "No results for:\xa0"
-                                }), (0, e.jsx)("b", {
-                                    children: c
-                                })]
-                            }), (0, e.jsx)(v, {
-                                contents: b,
-                                setVariant: d
-                            })]
-                        })
-                    })
-                },
-                z = c(75820),
-                A = c(93432),
-                B = function(a) {
+                B = x,
+                C = function(a) {
                     return {
                         fetch: function(b, c) {
-                            return a((0, z.on)({
+                            return a((0, j.on)({
                                 api: b,
                                 query: c
                             }))
                         },
                         setVariant: function(b, c, d) {
-                            a((0, A.jO)({
+                            a((0, i.jO)({
                                 type: b,
                                 name: c,
                                 variant: d
                             }))
                         }
                     }
                 },
-                C = function(a) {
+                D = function(a) {
                     var b, c = a.searchResults,
-                        g = a.api,
-                        h = a.setVariant,
-                        i = (0, d.Z)(a, ["searchResults", "api", "setVariant"]),
-                        j = (b = (0, t.useRouter)(), new URLSearchParams(b.query)).get("q"),
-                        k = i.fetch;
-                    return (0, f.useEffect)(function() {
-                        k(g, j)
-                    }, [j, g, k]), (0, e.jsx)("div", {
-                        children: (0, e.jsx)(y, {
+                        h = a.api,
+                        i = a.setVariant,
+                        j = (0, d.Z)(a, ["searchResults", "api", "setVariant"]),
+                        k = (b = (0, f.useRouter)(), new URLSearchParams(b.query)).get("q"),
+                        l = j.fetch;
+                    return (0, g.useEffect)(function() {
+                        h && k && l(h, k)
+                    }, [k, h, l]), (0, e.jsx)("div", {
+                        children: (0, e.jsx)(B, {
                             results: null == c ? void 0 : c.resources,
-                            search_query: j,
-                            setVariant: h
+                            search_query: k,
+                            setVariant: i
                         })
                     })
                 },
-                D = function(a) {
+                E = function(a) {
                     return {
                         searchResults: a.searchResults
                     }
                 },
-                E = (0, g.$j)(D, B)(C)
+                F = (0, h.$j)(E, C)(D)
         },
         75820: function(a, b, c) {
             "use strict";
             c.d(b, {
                 on: function() {
                     return k
                 }
@@ -93608,15 +93592,15 @@
             }, g.defaultProps = {
                 height: 80,
                 width: 80,
                 color: "green",
                 label: "audio-loading"
             }
         },
-        18183: function(a, b, c) {
+        98964: function(a, b, c) {
             "use strict";
             Object.defineProperty(b, "__esModule", {
                 value: !0
             }), b.Watch = void 0;
             var d = f(c(67294)),
                 e = f(c(45697));
 
@@ -93698,15 +93682,15 @@
         },
         79560: function(a, b, c) {
             "use strict";
             Object.defineProperty(b, "__esModule", {
                 value: !0
             }), b.Spinner = void 0;
             var d = c(16961),
-                e = c(18183),
+                e = c(98964),
                 f = c(15842),
                 g = c(65861),
                 h = c(78454),
                 i = c(72994),
                 j = c(34983),
                 k = c(88866),
                 l = c(98330),
```

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/pages/index-c2ee5b1681e97e4b.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/pages/index-942ec646d90d2132.js`

 * *Files 26% similar despite different names*

#### js-beautify {}

```diff
@@ -1,36 +1,32 @@
 (self.webpackChunk_N_E = self.webpackChunk_N_E || []).push([
     [5405], {
         75557: function(a, b, c) {
             (window.__NEXT_P = window.__NEXT_P || []).push(["/", function() {
-                return c(88559)
+                return c(53678)
             }])
         },
-        88559: function(a, b, c) {
+        53678: function(a, b, c) {
             "use strict";
-            c.r(b), c.d(b, {
-                default: function() {
-                    return i
-                }
-            });
-            var d = c(85893);
-            next;
-            var e = c(9008),
-                f = c.n(e),
-                g = c(83023),
+            c.r(b);
+            var d = c(85893),
+                e = c(9008),
+                f = c.n(e);
+            c(67294);
+            var g = c(83023),
                 h = function() {
                     return (0, d.jsxs)("div", {
                         children: [(0, d.jsx)(f(), {
                             children: (0, d.jsx)("title", {
                                 children: "Featureform Dashboard"
                             })
                         }), (0, d.jsx)(g.Z, {})]
                     })
-                },
-                i = h
+                };
+            b.default = h
         },
         9008: function(a, b, c) {
             a.exports = c(5443)
         }
     },
     function(a) {
         a.O(0, [9774, 2888, 179], function() {
```

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter/refractor-core-import.d200df4f5651fe3c.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter/refractor-core-import.d200df4f5651fe3c.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_abap.cff854fd7e5b1247.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_abap.cff854fd7e5b1247.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_abnf.a1ff159f2ef1711f.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_abnf.a1ff159f2ef1711f.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_actionscript.efd417c28a28b388.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_actionscript.efd417c28a28b388.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ada.156060425d9edae1.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ada.156060425d9edae1.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_agda.7c059beeef27c79a.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_agda.7c059beeef27c79a.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_al.f8ab011377e6cffa.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_al.f8ab011377e6cffa.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_antlr4.2c3a6fa926d2a251.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_antlr4.2c3a6fa926d2a251.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_apacheconf.a8e9c6e2469ebb48.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_apacheconf.a8e9c6e2469ebb48.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_apl.17fe889a8c792ca2.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_apl.17fe889a8c792ca2.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_applescript.ec5486ed51b5bf2a.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_applescript.ec5486ed51b5bf2a.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_aql.efb695712e3f3aa3.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_aql.efb695712e3f3aa3.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_arduino.681aaa7ec91aa809.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_arduino.681aaa7ec91aa809.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_asciidoc.d34ffa4ca9efdc4d.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_asciidoc.d34ffa4ca9efdc4d.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_asm6502.3eb992d6df117427.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_asm6502.3eb992d6df117427.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_aspnet.0ba8de8f97453373.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_aspnet.0ba8de8f97453373.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_autohotkey.8bd8b23c56f29881.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_autohotkey.8bd8b23c56f29881.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_autoit.f687b627eb6354c6.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_autoit.f687b627eb6354c6.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bash.fa5423ba02f0452a.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bash.fa5423ba02f0452a.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_basic.18dbad942d626219.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_basic.18dbad942d626219.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_batch.8ca1ac5c2d037485.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_batch.8ca1ac5c2d037485.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bbcode.4b540b8d0f463220.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bbcode.4b540b8d0f463220.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bison.3be4b74c3d3e0770.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bison.3be4b74c3d3e0770.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_brightscript.5219a23e15549d0f.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_brightscript.5219a23e15549d0f.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bro.6a3db5175eef5a7c.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bro.6a3db5175eef5a7c.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_c.fba60a9486edee8d.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_c.fba60a9486edee8d.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cil.494c2357f1d5de1e.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cil.494c2357f1d5de1e.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_clike.065b788c95ab7f0a.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_clike.065b788c95ab7f0a.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_clojure.144f4fa5cb5b7c94.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_clojure.144f4fa5cb5b7c94.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cmake.63bd8fd3867951a6.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cmake.63bd8fd3867951a6.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_coffeescript.f3407609f464e5a7.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_coffeescript.f3407609f464e5a7.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_concurnas.807a36085ae57a51.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_concurnas.807a36085ae57a51.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cpp.9073ce25850a9aee.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cpp.9073ce25850a9aee.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_crystal.500857f6d38420ca.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_crystal.500857f6d38420ca.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_csharp.1ab46bae80c6b0ba.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_csharp.1ab46bae80c6b0ba.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_csp.dbb73c45172741db.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_csp.dbb73c45172741db.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_css.c6ce776800cc984e.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_css.c6ce776800cc984e.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cssExtras.9588a637662140d4.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cssExtras.9588a637662140d4.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cypher.899ff7f5c7459114.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cypher.899ff7f5c7459114.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_d.3e486cddc20d2ff9.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_d.3e486cddc20d2ff9.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dart.9db40f270a0b6cb0.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dart.9db40f270a0b6cb0.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dax.f58ad34d65866793.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dax.f58ad34d65866793.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dhall.0ca1a915d1865fb5.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dhall.0ca1a915d1865fb5.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_diff.e343fa532144b7a2.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_diff.e343fa532144b7a2.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_django.6ee6c39cb914f163.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_django.6ee6c39cb914f163.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dnsZoneFile.2a9886e744590498.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dnsZoneFile.2a9886e744590498.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_docker.fde534872e6578fd.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_docker.fde534872e6578fd.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ebnf.35e28e1f6e8a00e4.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ebnf.35e28e1f6e8a00e4.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_eiffel.64ef4de4060b9a23.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_eiffel.64ef4de4060b9a23.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ejs.4c4ccb70f90dea01.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ejs.4c4ccb70f90dea01.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_elixir.a1e48f12166c723b.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_elixir.a1e48f12166c723b.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_elm.6765aa0f50cbaf91.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_elm.6765aa0f50cbaf91.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_erb.e48ed285a1945936.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_erb.e48ed285a1945936.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_erlang.2a114ebcf8dd2d26.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_erlang.2a114ebcf8dd2d26.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_etlua.afcb29f06feae539.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_etlua.afcb29f06feae539.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_excelFormula.62d0fdeee42f5d64.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_excelFormula.62d0fdeee42f5d64.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_factor.ce84f1b770942d68.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_factor.ce84f1b770942d68.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_firestoreSecurityRules.209ede8c07b9e60b.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_firestoreSecurityRules.209ede8c07b9e60b.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_flow.88a9cbf968cf47ec.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_flow.88a9cbf968cf47ec.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_fortran.ca33766cb3d9d13c.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_fortran.ca33766cb3d9d13c.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_fsharp.1aa244fc87692af1.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_fsharp.1aa244fc87692af1.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ftl.0457d46374506e78.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ftl.0457d46374506e78.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gdscript.afa83bf48d38ded2.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gdscript.afa83bf48d38ded2.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gedcom.eae35079f43f4e91.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gedcom.eae35079f43f4e91.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gherkin.1226aeae8764f3d7.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gherkin.1226aeae8764f3d7.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_glsl.aaa801f4d5c6da96.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_glsl.aaa801f4d5c6da96.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gml.18f92cdfb2a6d10f.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gml.18f92cdfb2a6d10f.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_go.e302653e25089bba.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_go.e302653e25089bba.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_graphql.8d0455822c35e9af.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_graphql.8d0455822c35e9af.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_groovy.67837d37705d722b.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_groovy.67837d37705d722b.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haml.9095964d871cb9e5.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haml.9095964d871cb9e5.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_handlebars.3a1658c72e98aa85.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_handlebars.3a1658c72e98aa85.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haskell.c37122cc55c1e696.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haskell.c37122cc55c1e696.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haxe.4e1677441d389a66.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haxe.4e1677441d389a66.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hcl.f5277940e647aca6.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hcl.f5277940e647aca6.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hlsl.f778194f7f56c677.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hlsl.f778194f7f56c677.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_http.80f0633c0c6cabe9.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_http.80f0633c0c6cabe9.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ichigojam.154c28afdb7a6cb3.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ichigojam.154c28afdb7a6cb3.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_icon.ee1eca6d9d8a1a78.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_icon.ee1eca6d9d8a1a78.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_iecst.ae937df11bf15aa5.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_iecst.ae937df11bf15aa5.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ignore.e7db33c594b328a4.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ignore.e7db33c594b328a4.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_inform7.25b80e018be9b4b0.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_inform7.25b80e018be9b4b0.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ini.1305ea3d405b7b77.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ini.1305ea3d405b7b77.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_io.57902ad550c5a076.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_io.57902ad550c5a076.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_j.d8b9ad361d46c928.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_j.d8b9ad361d46c928.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_java.375f3f7b940d3ea2.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_java.375f3f7b940d3ea2.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javadoc.9022ca32626ca861.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javadoc.9022ca32626ca861.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javadoclike.a5b69d2a868cd5a6.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javadoclike.a5b69d2a868cd5a6.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javascript.795b07cdb9c3aad5.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javascript.795b07cdb9c3aad5.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javastacktrace.8ef9f62617bbdae9.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javastacktrace.8ef9f62617bbdae9.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jolie.fe8eb7d347ec2ee8.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jolie.fe8eb7d347ec2ee8.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jq.995d87dae4a1fc6c.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jq.995d87dae4a1fc6c.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsExtras.a681c21d98be5d88.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsExtras.a681c21d98be5d88.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsTemplates.e15b503a789336d0.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsTemplates.e15b503a789336d0.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsdoc.863383140825aabf.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsdoc.863383140825aabf.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_json5.b916560a73dec284.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_json5.b916560a73dec284.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsstacktrace.237affac11d29a8e.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsstacktrace.237affac11d29a8e.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsx.66ae31b67824e2b1.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsx.66ae31b67824e2b1.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_julia.aebde82cc8e430a4.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_julia.aebde82cc8e430a4.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_keyman.20a6fec54a9e6dc8.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_keyman.20a6fec54a9e6dc8.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_kotlin.204d94980c876688.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_kotlin.204d94980c876688.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_latex.3ea6b205c4740fcf.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_latex.3ea6b205c4740fcf.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_latte.6c65a65bc30d6d65.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_latte.6c65a65bc30d6d65.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_less.571cfcc5f39892cf.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_less.571cfcc5f39892cf.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lilypond.b68fc0ec4de9b335.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lilypond.b68fc0ec4de9b335.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_liquid.93e3d518888cf132.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_liquid.93e3d518888cf132.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lisp.eb4c988e1cb1b488.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lisp.eb4c988e1cb1b488.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_livescript.e154b07a04e47729.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_livescript.e154b07a04e47729.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_llvm.3edc24655432e967.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_llvm.3edc24655432e967.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lolcode.920a08022d1f3fb3.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lolcode.920a08022d1f3fb3.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lua.b83366b41cb96d93.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lua.b83366b41cb96d93.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_makefile.cac7a41c308ba41f.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_makefile.cac7a41c308ba41f.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markdown.06f7de54663dea9e.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markdown.06f7de54663dea9e.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markup.0001ba0d552266f8.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markup.0001ba0d552266f8.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markupTemplating.1463fee82d988102.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markupTemplating.1463fee82d988102.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_matlab.29f5102b58bb0786.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_matlab.29f5102b58bb0786.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_mel.18e5992de05c1caa.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_mel.18e5992de05c1caa.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_mizar.2c0399b5c03c3450.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_mizar.2c0399b5c03c3450.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_monkey.bb2faba45e3cee8a.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_monkey.bb2faba45e3cee8a.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_moonscript.e9dce6a537d684a9.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_moonscript.e9dce6a537d684a9.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_n1ql.9924ec6c046bda5b.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_n1ql.9924ec6c046bda5b.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_n4js.68b6d0a9d2b4e3b9.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_n4js.68b6d0a9d2b4e3b9.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nasm.08df2ec010d92ce1.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nasm.08df2ec010d92ce1.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_neon.b4d21d37e14ff2e4.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_neon.b4d21d37e14ff2e4.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nginx.a7f671ec4fed709c.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nginx.a7f671ec4fed709c.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nim.b9b3330a8cc76ae6.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nim.b9b3330a8cc76ae6.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nix.ec8c698fe8cf158f.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nix.ec8c698fe8cf158f.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nsis.17532a14606f8ba0.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nsis.17532a14606f8ba0.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_objectivec.a9a054b060f7e9c4.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_objectivec.a9a054b060f7e9c4.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ocaml.0ce7e66b58933eec.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ocaml.0ce7e66b58933eec.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_opencl.343386871671e433.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_opencl.343386871671e433.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_oz.3dd791c14d6789e9.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_oz.3dd791c14d6789e9.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_parigp.01c2a6558ead9c1d.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_parigp.01c2a6558ead9c1d.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_parser.4080f0c5df8c5411.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_parser.4080f0c5df8c5411.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pascal.714d7fd616dffa60.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pascal.714d7fd616dffa60.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pascaligo.3d9efa4ff03d798d.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pascaligo.3d9efa4ff03d798d.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pcaxis.dc2dc17ec584a4e1.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pcaxis.dc2dc17ec584a4e1.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_peoplecode.00b98a730fe91b5e.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_peoplecode.00b98a730fe91b5e.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_perl.a4fecd65a9c2ecd2.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_perl.a4fecd65a9c2ecd2.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_php.1da6a39f37370ec1.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_php.1da6a39f37370ec1.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_phpExtras.8468f770a82630ef.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_phpExtras.8468f770a82630ef.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_phpdoc.59ba40872e3d9cfe.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_phpdoc.59ba40872e3d9cfe.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_plsql.6fc1cf5b4b2439a3.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_plsql.6fc1cf5b4b2439a3.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_powerquery.c87eb035121d7831.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_powerquery.c87eb035121d7831.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_powershell.56966af030c91702.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_powershell.56966af030c91702.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_processing.ec8607c7392a938f.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_processing.ec8607c7392a938f.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_protobuf.d96df12b0f0a2409.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_protobuf.d96df12b0f0a2409.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pug.6b509aa2c3a57467.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pug.6b509aa2c3a57467.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_puppet.ce519d4962965362.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_puppet.ce519d4962965362.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pure.e3fd8806900462cf.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pure.e3fd8806900462cf.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_purebasic.70942e3d774ada85.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_purebasic.70942e3d774ada85.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_q.1df151a687a188a7.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_q.1df151a687a188a7.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_qml.e36896b667a01ae9.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_qml.e36896b667a01ae9.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_qore.1137d54889243367.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_qore.1137d54889243367.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_r.7ca305d9455cc86f.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_r.7ca305d9455cc86f.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_racket.bee31c56faa733b2.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_racket.bee31c56faa733b2.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_reason.af902fad4bd674df.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_reason.af902fad4bd674df.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_regex.074352f8c0201b38.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_regex.074352f8c0201b38.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_renpy.5938c171f23d6f29.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_renpy.5938c171f23d6f29.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rest.fcefb9b5cfa112e0.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rest.fcefb9b5cfa112e0.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rip.5f599ff53f5c1e9a.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rip.5f599ff53f5c1e9a.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_roboconf.49d8eaad661bcd43.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_roboconf.49d8eaad661bcd43.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_robotframework.883fa1f592ad87e7.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_robotframework.883fa1f592ad87e7.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ruby.f76b4f68b3137a6f.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ruby.f76b4f68b3137a6f.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rust.ca92b5ca27e7312d.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rust.ca92b5ca27e7312d.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sas.33e0e78e18cf156f.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sas.33e0e78e18cf156f.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sass.8436ff53b0701941.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sass.8436ff53b0701941.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scala.7db11a73d01e23d4.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scala.7db11a73d01e23d4.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scheme.a224b3505cc86f4d.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scheme.a224b3505cc86f4d.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scss.fbd015582067d022.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scss.fbd015582067d022.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_shellSession.54615d020c9c44d5.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_shellSession.54615d020c9c44d5.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smali.e44f80bb9100f728.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smali.e44f80bb9100f728.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smalltalk.e89fea8686ec9f90.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smalltalk.e89fea8686ec9f90.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smarty.404a8e12834103cf.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smarty.404a8e12834103cf.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_solidity.537cb7600d04dae8.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_solidity.537cb7600d04dae8.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_solutionFile.53d3dde6d83fdea2.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_solutionFile.53d3dde6d83fdea2.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_soy.51e9adabd56f467a.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_soy.51e9adabd56f467a.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sparql.2aa3288ef8ae3374.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sparql.2aa3288ef8ae3374.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_splunkSpl.095636b50fe9a368.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_splunkSpl.095636b50fe9a368.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sqf.11b0bee7a2de8e94.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sqf.11b0bee7a2de8e94.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_stylus.213bb148fbffff7f.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_stylus.213bb148fbffff7f.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_swift.27d0fee1e44e54b6.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_swift.27d0fee1e44e54b6.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Cs.cd31c8bc90add20f.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Cs.cd31c8bc90add20f.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Templating.c87834ec2ea19f73.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Templating.c87834ec2ea19f73.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Vb.2cf235d46995926d.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Vb.2cf235d46995926d.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tap.a22e7b01443f999b.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tap.a22e7b01443f999b.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tcl.72a4244b8fb7ec0d.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tcl.72a4244b8fb7ec0d.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_textile.e52c4e181b801ddd.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_textile.e52c4e181b801ddd.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_toml.9bf8ce9e1f31a008.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_toml.9bf8ce9e1f31a008.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tsx.f039389d397f2bb4.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tsx.f039389d397f2bb4.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tt2.645259383cf82689.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tt2.645259383cf82689.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_turtle.69d8330a2e17bb57.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_turtle.69d8330a2e17bb57.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_twig.d5bfca25e9d2543d.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_twig.d5bfca25e9d2543d.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_typescript.d8f51be2a38383c6.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_typescript.d8f51be2a38383c6.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_unrealscript.9179623df9a8b80c.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_unrealscript.9179623df9a8b80c.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vala.2e16603251de6f51.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vala.2e16603251de6f51.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vbnet.ac96de8240011055.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vbnet.ac96de8240011055.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_velocity.bc75ee95252e2b47.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_velocity.bc75ee95252e2b47.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_verilog.4e42ac1a89cb8605.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_verilog.4e42ac1a89cb8605.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vhdl.5ab0f6bc359d7c74.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vhdl.5ab0f6bc359d7c74.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vim.6c4d4c01dc147971.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vim.6c4d4c01dc147971.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_visualBasic.c3e43390c4a3ee45.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_visualBasic.c3e43390c4a3ee45.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_warpscript.ccc821a2177dfac0.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_warpscript.ccc821a2177dfac0.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_wasm.3ffc1a78867a6148.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_wasm.3ffc1a78867a6148.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_wiki.b5dc9ed00ff4ea53.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_wiki.b5dc9ed00ff4ea53.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xeora.b31606451a6f896b.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xeora.b31606451a6f896b.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xojo.81cb4d9104c6ac5b.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xojo.81cb4d9104c6ac5b.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xquery.4382c54a41b1309a.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xquery.4382c54a41b1309a.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_yaml.178577f1d765f16b.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_yaml.178577f1d765f16b.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_zig.a535909b59fc6987.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_zig.a535909b59fc6987.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/webpack-6ed703bc0f4dd2fe.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/chunks/webpack-6ed703bc0f4dd2fe.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/media/Matter-Regular.f1ae4ce5.ttf` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/media/Matter-Regular.f1ae4ce5.ttf`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/u8jMEl73MAEGHR4r4U4Dw/_buildManifest.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/u8jMEl73MAEGHR4r4U4Dw/_buildManifest.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/_next/static/xB9Lh8aE_cExc1t6WFtEI/_buildManifest.js` & `featureform-1.8.1/src/featureform/dashboard/out/_next/static/xB9Lh8aE_cExc1t6WFtEI/_buildManifest.js`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/connections.html` & `featureform-1.8.1/src/featureform/dashboard/out/connections.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,42 +1,137 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-6ed703bc0f4dd2fe.js" defer=""></script><script src="/_next/static/chunks/framework-3412d1150754b2fb.js" defer=""></script><script src="/_next/static/chunks/main-2715d0c23f47c019.js" defer=""></script><script src="/_next/static/chunks/pages/_app-a764893ff9420ec0.js" defer=""></script><script src="/_next/static/chunks/pages/connections-1d67ba61869dece6.js" defer=""></script><script src="/_next/static/XLqQwuMDcHNwRKV5unb2J/_buildManifest.js" defer=""></script><script src="/_next/static/XLqQwuMDcHNwRKV5unb2J/_ssgManifest.js" defer=""></script><style id="jss-server-side">.MuiTypography-root {
-  margin: 0;
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-6ed703bc0f4dd2fe.js" defer=""></script><script src="/_next/static/chunks/framework-3412d1150754b2fb.js" defer=""></script><script src="/_next/static/chunks/main-2715d0c23f47c019.js" defer=""></script><script src="/_next/static/chunks/pages/_app-535a9349f87f23c6.js" defer=""></script><script src="/_next/static/chunks/pages/connections-1d67ba61869dece6.js" defer=""></script><script src="/_next/static/aZJnz9nRD9kOWLAxrQep6/_buildManifest.js" defer=""></script><script src="/_next/static/aZJnz9nRD9kOWLAxrQep6/_ssgManifest.js" defer=""></script><style id="jss-server-side">.MuiContainer-root {
+  width: 100%;
+  display: block;
+  box-sizing: border-box;
+  margin-left: auto;
+  margin-right: auto;
+  padding-left: 16px;
+  padding-right: 16px;
 }
-.MuiTypography-body2 {
-  font-size: 0.875rem;
-  font-family: "Matter", "Lato", "Helvetica", sans-serif;
-  font-weight: 550;
-  line-height: 1.43;
-}
-.MuiTypography-body1 {
-  font-size: 1rem;
-  font-family: "Matter", "Lato", "Helvetica", sans-serif;
-  font-weight: 550;
-  line-height: 1.5;
-}
-.MuiTypography-caption {
-  font-size: 0.75rem;
-  font-family: "Matter", "Lato", "Helvetica", sans-serif;
-  font-weight: 550;
-  line-height: 1.66;
-}
-.MuiTypography-button {
-  font-size: 0.875rem;
-  font-family: "Matter", "Lato", "Helvetica", sans-serif;
-  font-weight: 650;
-  line-height: 1.75;
-  text-transform: uppercase;
-}
-.MuiTypography-h1 {
-  font-size: 3.5rem;
-  font-family: "Matter", "Lato", "Helvetica", sans-serif;
-  font-weight: 450;
-  line-height: 1.167;
+@media (min-width:600px) {
+  .MuiContainer-root {
+    padding-left: 24px;
+    padding-right: 24px;
+  }
+}
+  .MuiContainer-disableGutters {
+    padding-left: 0;
+    padding-right: 0;
+  }
+@media (min-width:600px) {
+  .MuiContainer-fixed {
+    max-width: 600px;
+  }
+}
+@media (min-width:960px) {
+  .MuiContainer-fixed {
+    max-width: 960px;
+  }
+}
+@media (min-width:1280px) {
+  .MuiContainer-fixed {
+    max-width: 1280px;
+  }
+}
+@media (min-width:1920px) {
+  .MuiContainer-fixed {
+    max-width: 1920px;
+  }
+}
+@media (min-width:0px) {
+  .MuiContainer-maxWidthXs {
+    max-width: 444px;
+  }
 }
 @media (min-width:600px) {
+  .MuiContainer-maxWidthSm {
+    max-width: 600px;
+  }
+}
+@media (min-width:960px) {
+  .MuiContainer-maxWidthMd {
+    max-width: 960px;
+  }
+}
+@media (min-width:1280px) {
+  .MuiContainer-maxWidthLg {
+    max-width: 1280px;
+  }
+}
+@media (min-width:1920px) {
+  .MuiContainer-maxWidthXl {
+    max-width: 1920px;
+  }
+}
+  html {
+    box-sizing: border-box;
+    -webkit-font-smoothing: antialiased;
+    -moz-osx-font-smoothing: grayscale;
+  }
+  *, *::before, *::after {
+    box-sizing: inherit;
+  }
+  strong, b {
+    font-weight: 700;
+  }
+  body {
+    color: #263238;
+    margin: 0;
+    font-size: 0.875rem;
+    background: radial-gradient(circle farthest-side, #E4D0FA 0%, rgba(255, 0, 0, 0) 40%) top left/200% 100%, radial-gradient(circle farthest-side, #FCA3BE 0%, rgba(255, 0, 0, 0) 40%) top right/180% 150%;;
+    font-family: "Matter", "Lato", "Helvetica", sans-serif;
+    font-weight: 550;
+    line-height: 1.43;
+    background-color: #FFFFFF;
+    background-repeat: no-repeat;
+    background-attachment: fixed;
+  }
+@media print {
+  body {
+    background-color: #fff;
+  }
+}
+  body::backdrop {
+    background-color: #FFFFFF;
+  }
+  .MuiTypography-root {
+    margin: 0;
+  }
+  .MuiTypography-body2 {
+    font-size: 0.875rem;
+    font-family: "Matter", "Lato", "Helvetica", sans-serif;
+    font-weight: 550;
+    line-height: 1.43;
+  }
+  .MuiTypography-body1 {
+    font-size: 1rem;
+    font-family: "Matter", "Lato", "Helvetica", sans-serif;
+    font-weight: 550;
+    line-height: 1.5;
+  }
+  .MuiTypography-caption {
+    font-size: 0.75rem;
+    font-family: "Matter", "Lato", "Helvetica", sans-serif;
+    font-weight: 550;
+    line-height: 1.66;
+  }
+  .MuiTypography-button {
+    font-size: 0.875rem;
+    font-family: "Matter", "Lato", "Helvetica", sans-serif;
+    font-weight: 650;
+    line-height: 1.75;
+    text-transform: uppercase;
+  }
+  .MuiTypography-h1 {
+    font-size: 3.5rem;
+    font-family: "Matter", "Lato", "Helvetica", sans-serif;
+    font-weight: 450;
+    line-height: 1.167;
+  }
+@media (min-width:600px) {
   .MuiTypography-h1 {
     font-size: 4.7129rem;
   }
 }
 @media (min-width:960px) {
   .MuiTypography-h1 {
     font-size: 5.3556rem;
@@ -220,14 +315,42 @@
   }
   .MuiTypography-displayInline {
     display: inline;
   }
   .MuiTypography-displayBlock {
     display: block;
   }
+  .MuiBreadcrumbs-ol {
+    margin: 0;
+    display: flex;
+    padding: 0;
+    flex-wrap: wrap;
+    list-style: none;
+    align-items: center;
+  }
+  .MuiBreadcrumbs-separator {
+    display: flex;
+    margin-left: 8px;
+    user-select: none;
+    margin-right: 8px;
+  }
+  .jss12 {
+    margin: 5px;
+  }
+  .jss13 {
+    align-items: inherit;
+  }
+  .jss14 {
+    font-size: 18px;
+  }
+  .jss15 {
+    align-items: auto;
+    margin-left: 0.2em;
+    margin-right: 0.2em;
+  }
   .MuiGrid-container {
     width: 100%;
     display: flex;
     flex-wrap: wrap;
     box-sizing: border-box;
   }
   .MuiGrid-item {
@@ -804,45 +927,14 @@
   }
   .MuiPaper-elevation23 {
     box-shadow: 0px 11px 14px -7px rgba(0,0,0,0.2),0px 23px 36px 3px rgba(0,0,0,0.14),0px 9px 44px 8px rgba(0,0,0,0.12);
   }
   .MuiPaper-elevation24 {
     box-shadow: 0px 11px 15px -7px rgba(0,0,0,0.2),0px 24px 38px 3px rgba(0,0,0,0.14),0px 9px 46px 8px rgba(0,0,0,0.12);
   }
-  .MuiToolbar-root {
-    display: flex;
-    position: relative;
-    align-items: center;
-  }
-  .MuiToolbar-gutters {
-    padding-left: 16px;
-    padding-right: 16px;
-  }
-@media (min-width:600px) {
-  .MuiToolbar-gutters {
-    padding-left: 24px;
-    padding-right: 24px;
-  }
-}
-  .MuiToolbar-regular {
-    min-height: 56px;
-  }
-@media (min-width:0px) and (orientation: landscape) {
-  .MuiToolbar-regular {
-    min-height: 48px;
-  }
-}
-@media (min-width:600px) {
-  .MuiToolbar-regular {
-    min-height: 64px;
-  }
-}
-  .MuiToolbar-dense {
-    min-height: 48px;
-  }
   .MuiAppBar-root {
     width: 100%;
     display: flex;
     z-index: 1100;
     box-sizing: border-box;
     flex-shrink: 0;
     flex-direction: column;
@@ -891,136 +983,60 @@
   .MuiAppBar-colorInherit {
     color: inherit;
   }
   .MuiAppBar-colorTransparent {
     color: inherit;
     background-color: transparent;
   }
-  .MuiBreadcrumbs-ol {
-    margin: 0;
-    display: flex;
-    padding: 0;
-    flex-wrap: wrap;
-    list-style: none;
-    align-items: center;
+
+  .jss11 {
+    height: 30px;
+    display: [object Object];
+    flex-grow: 1;
   }
-  .MuiBreadcrumbs-separator {
-    display: flex;
-    margin-left: 8px;
-    user-select: none;
-    margin-right: 8px;
+@media (min-width:0px) {
+  .jss11 {
+    display: none;
   }
-  .MuiContainer-root {
-    width: 100%;
+}
+@media (min-width:600px) {
+  .jss11 {
     display: block;
-    box-sizing: border-box;
-    margin-left: auto;
-    margin-right: auto;
+  }
+}
+  .MuiToolbar-root {
+    display: flex;
+    position: relative;
+    align-items: center;
+  }
+  .MuiToolbar-gutters {
     padding-left: 16px;
     padding-right: 16px;
   }
 @media (min-width:600px) {
-  .MuiContainer-root {
+  .MuiToolbar-gutters {
     padding-left: 24px;
     padding-right: 24px;
   }
 }
-  .MuiContainer-disableGutters {
-    padding-left: 0;
-    padding-right: 0;
-  }
-@media (min-width:600px) {
-  .MuiContainer-fixed {
-    max-width: 600px;
-  }
-}
-@media (min-width:960px) {
-  .MuiContainer-fixed {
-    max-width: 960px;
-  }
-}
-@media (min-width:1280px) {
-  .MuiContainer-fixed {
-    max-width: 1280px;
-  }
-}
-@media (min-width:1920px) {
-  .MuiContainer-fixed {
-    max-width: 1920px;
+  .MuiToolbar-regular {
+    min-height: 56px;
   }
-}
-@media (min-width:0px) {
-  .MuiContainer-maxWidthXs {
-    max-width: 444px;
+@media (min-width:0px) and (orientation: landscape) {
+  .MuiToolbar-regular {
+    min-height: 48px;
   }
 }
 @media (min-width:600px) {
-  .MuiContainer-maxWidthSm {
-    max-width: 600px;
-  }
-}
-@media (min-width:960px) {
-  .MuiContainer-maxWidthMd {
-    max-width: 960px;
-  }
-}
-@media (min-width:1280px) {
-  .MuiContainer-maxWidthLg {
-    max-width: 1280px;
-  }
-}
-@media (min-width:1920px) {
-  .MuiContainer-maxWidthXl {
-    max-width: 1920px;
-  }
-}
-  html {
-    box-sizing: border-box;
-    -webkit-font-smoothing: antialiased;
-    -moz-osx-font-smoothing: grayscale;
-  }
-  *, *::before, *::after {
-    box-sizing: inherit;
-  }
-  strong, b {
-    font-weight: 700;
-  }
-  body {
-    color: #263238;
-    margin: 0;
-    font-size: 0.875rem;
-    background: radial-gradient(circle farthest-side, #E4D0FA 0%, rgba(255, 0, 0, 0) 40%) top left/200% 100%, radial-gradient(circle farthest-side, #FCA3BE 0%, rgba(255, 0, 0, 0) 40%) top right/180% 150%;;
-    font-family: "Matter", "Lato", "Helvetica", sans-serif;
-    font-weight: 550;
-    line-height: 1.43;
-    background-color: #FFFFFF;
-    background-repeat: no-repeat;
-    background-attachment: fixed;
-  }
-@media print {
-  body {
-    background-color: #fff;
+  .MuiToolbar-regular {
+    min-height: 64px;
   }
 }
-  body::backdrop {
-    background-color: #FFFFFF;
-  }
-  .jss11 {
-    margin: 5px;
-  }
-  .jss12 {
-    align-items: inherit;
-  }
-  .jss13 {
-    font-size: 18px;
-  }
-  .jss14 {
-    align-items: auto;
-    margin-left: 0.2em;
-    margin-right: 0.2em;
+  .MuiToolbar-dense {
+    min-height: 48px;
   }
   .jss2 {
     width: 100%;
     diplay: flex;
   }
   .jss3 {
     color: black;
@@ -1058,8 +1074,8 @@
     position: relative;
     font-size: 3em;
     justify-self: flex-end;
   }
   .jss1 {
     padding-left: 64px;
     padding-right: 64px;
-  }</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><div class="jss2"><header class="MuiPaper-root MuiAppBar-root MuiAppBar-positionStatic MuiAppBar-colorPrimary jss3 MuiPaper-elevation4"><div class="MuiToolbar-root MuiToolbar-regular jss6 MuiToolbar-gutters"><div class="jss7"><img src="/static/FeatureForm_Logo_Full_Black.svg" height="30" alt="Featureform" component="div" nowrap="true" style="cursor:pointer" sx="[object Object]"/></div><div class="jss9"></div></div></header></div><div class="MuiContainer-root MuiContainer-maxWidthXl jss1"><div class="jss11"><nav class="MuiTypography-root MuiBreadcrumbs-root jss13 MuiTypography-body1 MuiTypography-colorTextSecondary" style="margin:0.25em" aria-label="breadcrumb"><ol class="MuiBreadcrumbs-ol jss12"><li class="MuiBreadcrumbs-li"><a href="/">Home</a></li><li aria-hidden="true" class="MuiBreadcrumbs-separator jss14"><style data-emotion="css vubbuv">.css-vubbuv{-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;width:1em;height:1em;display:inline-block;fill:currentColor;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;-webkit-transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;font-size:1.5rem;}</style><svg class="MuiSvgIcon-root MuiSvgIcon-fontSizeMedium css-vubbuv" focusable="false" aria-hidden="true" viewBox="0 0 24 24" data-testid="NavigateNextIcon"><path d="M10 6 8.59 7.41 13.17 12l-4.58 4.59L10 18l6-6z"></path></svg></li><li class="MuiBreadcrumbs-li"><b>Connections</b></li></ol></nav></div><div><div class="MuiGrid-root MuiGrid-container MuiGrid-justify-content-xs-center MuiGrid-grid-lg-12"></div></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/connections","query":{},"buildId":"XLqQwuMDcHNwRKV5unb2J","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+  }</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><div class="jss2"><header class="MuiPaper-root MuiAppBar-root MuiAppBar-positionStatic MuiAppBar-colorPrimary jss3 MuiPaper-elevation4"><div class="MuiToolbar-root MuiToolbar-regular jss6 MuiToolbar-gutters"><div class="jss7"><img class="MuiBox-root jss11" src="/static/FeatureForm_Logo_Full_Black.svg" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss9"></div></div></header></div><div class="MuiContainer-root MuiContainer-maxWidthXl jss1"><div class="jss12"><nav class="MuiTypography-root MuiBreadcrumbs-root jss14 MuiTypography-body1 MuiTypography-colorTextSecondary" style="margin:0.25em" aria-label="breadcrumb"><ol class="MuiBreadcrumbs-ol jss13"><li class="MuiBreadcrumbs-li"><a href="/">Home</a></li><li aria-hidden="true" class="MuiBreadcrumbs-separator jss15"><style data-emotion="css vubbuv">.css-vubbuv{-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;width:1em;height:1em;display:inline-block;fill:currentColor;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;-webkit-transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;font-size:1.5rem;}</style><svg class="MuiSvgIcon-root MuiSvgIcon-fontSizeMedium css-vubbuv" focusable="false" aria-hidden="true" viewBox="0 0 24 24" data-testid="NavigateNextIcon"><path d="M10 6 8.59 7.41 13.17 12l-4.58 4.59L10 18l6-6z"></path></svg></li><li class="MuiBreadcrumbs-li"><b>Connections</b></li></ol></nav></div><div><div class="MuiGrid-root MuiGrid-container MuiGrid-justify-content-xs-center MuiGrid-grid-lg-12"></div></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/connections","query":{},"buildId":"aZJnz9nRD9kOWLAxrQep6","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/index.html` & `featureform-1.8.1/src/featureform/dashboard/out/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,41 +1,136 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><title>Featureform Dashboard</title><meta name="next-head-count" content="3"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-6ed703bc0f4dd2fe.js" defer=""></script><script src="/_next/static/chunks/framework-3412d1150754b2fb.js" defer=""></script><script src="/_next/static/chunks/main-2715d0c23f47c019.js" defer=""></script><script src="/_next/static/chunks/pages/_app-a764893ff9420ec0.js" defer=""></script><script src="/_next/static/chunks/pages/index-c2ee5b1681e97e4b.js" defer=""></script><script src="/_next/static/XLqQwuMDcHNwRKV5unb2J/_buildManifest.js" defer=""></script><script src="/_next/static/XLqQwuMDcHNwRKV5unb2J/_ssgManifest.js" defer=""></script><style id="jss-server-side">.MuiTypography-root {
-  margin: 0;
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><title>Featureform Dashboard</title><meta name="next-head-count" content="3"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-6ed703bc0f4dd2fe.js" defer=""></script><script src="/_next/static/chunks/framework-3412d1150754b2fb.js" defer=""></script><script src="/_next/static/chunks/main-2715d0c23f47c019.js" defer=""></script><script src="/_next/static/chunks/pages/_app-535a9349f87f23c6.js" defer=""></script><script src="/_next/static/chunks/pages/index-942ec646d90d2132.js" defer=""></script><script src="/_next/static/aZJnz9nRD9kOWLAxrQep6/_buildManifest.js" defer=""></script><script src="/_next/static/aZJnz9nRD9kOWLAxrQep6/_ssgManifest.js" defer=""></script><style id="jss-server-side">.MuiContainer-root {
+  width: 100%;
+  display: block;
+  box-sizing: border-box;
+  margin-left: auto;
+  margin-right: auto;
+  padding-left: 16px;
+  padding-right: 16px;
 }
-.MuiTypography-body2 {
-  font-size: 0.875rem;
-  font-family: "Matter", "Lato", "Helvetica", sans-serif;
-  font-weight: 550;
-  line-height: 1.43;
-}
-.MuiTypography-body1 {
-  font-size: 1rem;
-  font-family: "Matter", "Lato", "Helvetica", sans-serif;
-  font-weight: 550;
-  line-height: 1.5;
-}
-.MuiTypography-caption {
-  font-size: 0.75rem;
-  font-family: "Matter", "Lato", "Helvetica", sans-serif;
-  font-weight: 550;
-  line-height: 1.66;
-}
-.MuiTypography-button {
-  font-size: 0.875rem;
-  font-family: "Matter", "Lato", "Helvetica", sans-serif;
-  font-weight: 650;
-  line-height: 1.75;
-  text-transform: uppercase;
-}
-.MuiTypography-h1 {
-  font-size: 3.5rem;
-  font-family: "Matter", "Lato", "Helvetica", sans-serif;
-  font-weight: 450;
-  line-height: 1.167;
+@media (min-width:600px) {
+  .MuiContainer-root {
+    padding-left: 24px;
+    padding-right: 24px;
+  }
+}
+  .MuiContainer-disableGutters {
+    padding-left: 0;
+    padding-right: 0;
+  }
+@media (min-width:600px) {
+  .MuiContainer-fixed {
+    max-width: 600px;
+  }
+}
+@media (min-width:960px) {
+  .MuiContainer-fixed {
+    max-width: 960px;
+  }
+}
+@media (min-width:1280px) {
+  .MuiContainer-fixed {
+    max-width: 1280px;
+  }
+}
+@media (min-width:1920px) {
+  .MuiContainer-fixed {
+    max-width: 1920px;
+  }
+}
+@media (min-width:0px) {
+  .MuiContainer-maxWidthXs {
+    max-width: 444px;
+  }
+}
+@media (min-width:600px) {
+  .MuiContainer-maxWidthSm {
+    max-width: 600px;
+  }
+}
+@media (min-width:960px) {
+  .MuiContainer-maxWidthMd {
+    max-width: 960px;
+  }
+}
+@media (min-width:1280px) {
+  .MuiContainer-maxWidthLg {
+    max-width: 1280px;
+  }
+}
+@media (min-width:1920px) {
+  .MuiContainer-maxWidthXl {
+    max-width: 1920px;
+  }
+}
+  html {
+    box-sizing: border-box;
+    -webkit-font-smoothing: antialiased;
+    -moz-osx-font-smoothing: grayscale;
+  }
+  *, *::before, *::after {
+    box-sizing: inherit;
+  }
+  strong, b {
+    font-weight: 700;
+  }
+  body {
+    color: #263238;
+    margin: 0;
+    font-size: 0.875rem;
+    background: radial-gradient(circle farthest-side, #E4D0FA 0%, rgba(255, 0, 0, 0) 40%) top left/200% 100%, radial-gradient(circle farthest-side, #FCA3BE 0%, rgba(255, 0, 0, 0) 40%) top right/180% 150%;;
+    font-family: "Matter", "Lato", "Helvetica", sans-serif;
+    font-weight: 550;
+    line-height: 1.43;
+    background-color: #FFFFFF;
+    background-repeat: no-repeat;
+    background-attachment: fixed;
+  }
+@media print {
+  body {
+    background-color: #fff;
+  }
 }
+  body::backdrop {
+    background-color: #FFFFFF;
+  }
+  .MuiTypography-root {
+    margin: 0;
+  }
+  .MuiTypography-body2 {
+    font-size: 0.875rem;
+    font-family: "Matter", "Lato", "Helvetica", sans-serif;
+    font-weight: 550;
+    line-height: 1.43;
+  }
+  .MuiTypography-body1 {
+    font-size: 1rem;
+    font-family: "Matter", "Lato", "Helvetica", sans-serif;
+    font-weight: 550;
+    line-height: 1.5;
+  }
+  .MuiTypography-caption {
+    font-size: 0.75rem;
+    font-family: "Matter", "Lato", "Helvetica", sans-serif;
+    font-weight: 550;
+    line-height: 1.66;
+  }
+  .MuiTypography-button {
+    font-size: 0.875rem;
+    font-family: "Matter", "Lato", "Helvetica", sans-serif;
+    font-weight: 650;
+    line-height: 1.75;
+    text-transform: uppercase;
+  }
+  .MuiTypography-h1 {
+    font-size: 3.5rem;
+    font-family: "Matter", "Lato", "Helvetica", sans-serif;
+    font-weight: 450;
+    line-height: 1.167;
+  }
 @media (min-width:600px) {
   .MuiTypography-h1 {
     font-size: 4.7129rem;
   }
 }
 @media (min-width:960px) {
   .MuiTypography-h1 {
@@ -220,14 +315,62 @@
   }
   .MuiTypography-displayInline {
     display: inline;
   }
   .MuiTypography-displayBlock {
     display: block;
   }
+  .MuiSvgIcon-root {
+    fill: currentColor;
+    width: 1em;
+    height: 1em;
+    display: inline-block;
+    font-size: 1.5rem;
+    transition: fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;
+    flex-shrink: 0;
+    user-select: none;
+  }
+  .MuiSvgIcon-colorPrimary {
+    color: #f7195c;
+  }
+  .MuiSvgIcon-colorSecondary {
+    color: #f7195c;
+  }
+  .MuiSvgIcon-colorAction {
+    color: rgba(0, 0, 0, 0.54);
+  }
+  .MuiSvgIcon-colorError {
+    color: #f7195c;
+  }
+  .MuiSvgIcon-colorDisabled {
+    color: rgba(0, 0, 0, 0.26);
+  }
+  .MuiSvgIcon-fontSizeInherit {
+    font-size: inherit;
+  }
+  .MuiSvgIcon-fontSizeSmall {
+    font-size: 1.25rem;
+  }
+  .MuiSvgIcon-fontSizeLarge {
+    font-size: 2.1875rem;
+  }
+  .jss12 {
+    margin: 5px;
+  }
+  .jss13 {
+    align-items: inherit;
+  }
+  .jss14 {
+    font-size: 18px;
+  }
+  .jss15 {
+    align-items: auto;
+    margin-left: 0.2em;
+    margin-right: 0.2em;
+  }
   .MuiGrid-container {
     width: 100%;
     display: flex;
     flex-wrap: wrap;
     box-sizing: border-box;
   }
   .MuiGrid-item {
@@ -718,48 +861,14 @@
   }
   .MuiGrid-grid-xl-12 {
     flex-grow: 0;
     max-width: 100%;
     flex-basis: 100%;
   }
 }
-  .MuiSvgIcon-root {
-    fill: currentColor;
-    width: 1em;
-    height: 1em;
-    display: inline-block;
-    font-size: 1.5rem;
-    transition: fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;
-    flex-shrink: 0;
-    user-select: none;
-  }
-  .MuiSvgIcon-colorPrimary {
-    color: #f7195c;
-  }
-  .MuiSvgIcon-colorSecondary {
-    color: #f7195c;
-  }
-  .MuiSvgIcon-colorAction {
-    color: rgba(0, 0, 0, 0.54);
-  }
-  .MuiSvgIcon-colorError {
-    color: #f7195c;
-  }
-  .MuiSvgIcon-colorDisabled {
-    color: rgba(0, 0, 0, 0.26);
-  }
-  .MuiSvgIcon-fontSizeInherit {
-    font-size: inherit;
-  }
-  .MuiSvgIcon-fontSizeSmall {
-    font-size: 1.25rem;
-  }
-  .MuiSvgIcon-fontSizeLarge {
-    font-size: 2.1875rem;
-  }
   .MuiPaper-root {
     color: #263238;
     transition: box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;
     background-color: #fff;
   }
   .MuiPaper-rounded {
     border-radius: 4px;
@@ -838,14 +947,86 @@
   }
   .MuiPaper-elevation23 {
     box-shadow: 0px 11px 14px -7px rgba(0,0,0,0.2),0px 23px 36px 3px rgba(0,0,0,0.14),0px 9px 44px 8px rgba(0,0,0,0.12);
   }
   .MuiPaper-elevation24 {
     box-shadow: 0px 11px 15px -7px rgba(0,0,0,0.2),0px 24px 38px 3px rgba(0,0,0,0.14),0px 9px 46px 8px rgba(0,0,0,0.12);
   }
+  .MuiAppBar-root {
+    width: 100%;
+    display: flex;
+    z-index: 1100;
+    box-sizing: border-box;
+    flex-shrink: 0;
+    flex-direction: column;
+  }
+  .MuiAppBar-positionFixed {
+    top: 0;
+    left: auto;
+    right: 0;
+    position: fixed;
+  }
+@media print {
+  .MuiAppBar-positionFixed {
+    position: absolute;
+  }
+}
+  .MuiAppBar-positionAbsolute {
+    top: 0;
+    left: auto;
+    right: 0;
+    position: absolute;
+  }
+  .MuiAppBar-positionSticky {
+    top: 0;
+    left: auto;
+    right: 0;
+    position: sticky;
+  }
+  .MuiAppBar-positionStatic {
+    position: static;
+  }
+  .MuiAppBar-positionRelative {
+    position: relative;
+  }
+  .MuiAppBar-colorDefault {
+    color: rgba(0, 0, 0, 0.87);
+    background-color: #f5f5f5;
+  }
+  .MuiAppBar-colorPrimary {
+    color: #FFFFFF;
+    background-color: #f7195c;
+  }
+  .MuiAppBar-colorSecondary {
+    color: #fff;
+    background-color: #f7195c;
+  }
+  .MuiAppBar-colorInherit {
+    color: inherit;
+  }
+  .MuiAppBar-colorTransparent {
+    color: inherit;
+    background-color: transparent;
+  }
+
+  .jss11 {
+    height: 30px;
+    display: [object Object];
+    flex-grow: 1;
+  }
+@media (min-width:0px) {
+  .jss11 {
+    display: none;
+  }
+}
+@media (min-width:600px) {
+  .jss11 {
+    display: block;
+  }
+}
 @keyframes mui-auto-fill {}
 @keyframes mui-auto-fill-cancel {}
   .MuiInputBase-root {
     color: #263238;
     cursor: text;
     display: inline-flex;
     position: relative;
@@ -985,441 +1166,276 @@
   .MuiToolbar-regular {
     min-height: 64px;
   }
 }
   .MuiToolbar-dense {
     min-height: 48px;
   }
-  .MuiAppBar-root {
-    width: 100%;
-    display: flex;
-    z-index: 1100;
-    box-sizing: border-box;
-    flex-shrink: 0;
-    flex-direction: column;
-  }
-  .MuiAppBar-positionFixed {
-    top: 0;
-    left: auto;
-    right: 0;
-    position: fixed;
-  }
-@media print {
-  .MuiAppBar-positionFixed {
-    position: absolute;
-  }
-}
-  .MuiAppBar-positionAbsolute {
-    top: 0;
-    left: auto;
-    right: 0;
-    position: absolute;
-  }
-  .MuiAppBar-positionSticky {
-    top: 0;
-    left: auto;
-    right: 0;
-    position: sticky;
-  }
-  .MuiAppBar-positionStatic {
-    position: static;
-  }
-  .MuiAppBar-positionRelative {
-    position: relative;
-  }
-  .MuiAppBar-colorDefault {
-    color: rgba(0, 0, 0, 0.87);
-    background-color: #f5f5f5;
-  }
-  .MuiAppBar-colorPrimary {
-    color: #FFFFFF;
-    background-color: #f7195c;
-  }
-  .MuiAppBar-colorSecondary {
-    color: #fff;
-    background-color: #f7195c;
-  }
-  .MuiAppBar-colorInherit {
-    color: inherit;
-  }
-  .MuiAppBar-colorTransparent {
-    color: inherit;
-    background-color: transparent;
-  }
-  .MuiContainer-root {
-    width: 100%;
-    display: block;
-    box-sizing: border-box;
-    margin-left: auto;
-    margin-right: auto;
-    padding-left: 16px;
-    padding-right: 16px;
-  }
-@media (min-width:600px) {
-  .MuiContainer-root {
-    padding-left: 24px;
-    padding-right: 24px;
-  }
-}
-  .MuiContainer-disableGutters {
-    padding-left: 0;
-    padding-right: 0;
-  }
-@media (min-width:600px) {
-  .MuiContainer-fixed {
-    max-width: 600px;
-  }
-}
-@media (min-width:960px) {
-  .MuiContainer-fixed {
-    max-width: 960px;
-  }
-}
-@media (min-width:1280px) {
-  .MuiContainer-fixed {
-    max-width: 1280px;
-  }
-}
-@media (min-width:1920px) {
-  .MuiContainer-fixed {
-    max-width: 1920px;
-  }
-}
-@media (min-width:0px) {
-  .MuiContainer-maxWidthXs {
-    max-width: 444px;
-  }
-}
-@media (min-width:600px) {
-  .MuiContainer-maxWidthSm {
-    max-width: 600px;
-  }
-}
-@media (min-width:960px) {
-  .MuiContainer-maxWidthMd {
-    max-width: 960px;
-  }
-}
-@media (min-width:1280px) {
-  .MuiContainer-maxWidthLg {
-    max-width: 1280px;
-  }
-}
-@media (min-width:1920px) {
-  .MuiContainer-maxWidthXl {
-    max-width: 1920px;
-  }
-}
-  html {
-    box-sizing: border-box;
-    -webkit-font-smoothing: antialiased;
-    -moz-osx-font-smoothing: grayscale;
-  }
-  *, *::before, *::after {
-    box-sizing: inherit;
-  }
-  strong, b {
-    font-weight: 700;
-  }
-  body {
-    color: #263238;
-    margin: 0;
-    font-size: 0.875rem;
-    background: radial-gradient(circle farthest-side, #E4D0FA 0%, rgba(255, 0, 0, 0) 40%) top left/200% 100%, radial-gradient(circle farthest-side, #FCA3BE 0%, rgba(255, 0, 0, 0) 40%) top right/180% 150%;;
-    font-family: "Matter", "Lato", "Helvetica", sans-serif;
-    font-weight: 550;
-    line-height: 1.43;
-    background-color: #FFFFFF;
-    background-repeat: no-repeat;
-    background-attachment: fixed;
-  }
-@media print {
-  body {
-    background-color: #fff;
-  }
-}
-  body::backdrop {
-    background-color: #FFFFFF;
-  }
-  .jss23 {
+  .jss24 {
     width: 100%;
     position: relative;
     margin-left: 0;
     border-radius: 4px;
     background-color: rgba(255, 255, 255, 0.15);
   }
-  .jss23:hover {
+  .jss24:hover {
     background-color: rgba(255, 255, 255, 0.25);
   }
 @media (min-width:600px) {
-  .jss23 {
+  .jss24 {
     width: auto;
     margin-left: 8px;
   }
 }
-  .jss24 {
+  .jss25 {
     height: 100%;
     display: flex;
     padding: 0px 0px;
     position: absolute;
     align-items: center;
     pointer-events: none;
     justify-content: center;
   }
-  .jss25 {
+  .jss26 {
     border: 2px solid #CDD1D9;
     border-radius: 16px;
   }
-  .jss25:hover {
+  .jss26:hover {
     border: 2px solid black;
   }
-  .jss26 {
+  .jss27 {
     color: inherit;
     width: 100%;
     display: flex;
     background: transparent;
     box-shadow: none;
     transition: width 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;
     border-radius: 16px;
   }
-  .jss27 {
+  .jss28 {
     display: flex;
     padding: 8px 6px 3.2px 0px;
     align-self: flex-end;
     background: transparent;
     box-shadow: none;
     transition: width 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;
     padding-left: 32px;
     justify-content: center;
   }
-  .jss28 {
+  .jss29 {
     color: black;
     width: 100%;
     padding: 8px 0px 0px 0px;
     align-self: center;
     background: transparent;
     box-shadow: none;
     transition: width 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;
     padding-left: 32px;
   }
-  .jss29 {
+  .jss30 {
     width: 100%;
     height: 100%;
     padding: 16px;
   }
-  .jss30 {
+  .jss31 {
     width: 100%;
     height: 100%;
     padding: 24px;
     min-width: 12em;
     background: white;
     border-radius: 16px;
     text-transform: none;
   }
-  .jss30:hover {
+  .jss31:hover {
     color: undefined;
   }
-  .jss31 {
+  .jss32 {
     height: 200px;
   }
-  .jss32 {
+  .jss33 {
     width: 100%;
     height: 100%;
   }
-  .jss33 {
+  .jss34 {
     width: 100%;
     height: 100%;
     opacity: 0.3;
     padding: 24px;
     min-width: 12em;
     background: white;
     border-radius: 16px;
     text-transform: none;
   }
-  .jss34 {
+  .jss35 {
     font-size: 2em;
     margin-right: 16px;
   }
-  .jss35 {
+  .jss36 {
     font-size: 2em;
   }
-  .jss36 {
+  .jss37 {
     display: flex;
     justify-content: space-around;
   }
-  .jss37 {
+  .jss38 {
     border: 2px solid #3D0A73;
   }
-  .jss37:hover {
+  .jss38:hover {
     background-color: #CBC3E3;
   }
-  .jss38 {
-    border: 2px solid #3D0A73;
-  }
   .jss39 {
-    color: #3D0A73;
+    border: 2px solid #3D0A73;
   }
   .jss40 {
     color: #3D0A73;
   }
   .jss41 {
-    border: 2px solid #f7195c;
-  }
-  .jss41:hover {
-    background-color: #FFCCCB;
+    color: #3D0A73;
   }
   .jss42 {
     border: 2px solid #f7195c;
   }
+  .jss42:hover {
+    background-color: #FFCCCB;
+  }
   .jss43 {
-    color: #f7195c;
+    border: 2px solid #f7195c;
   }
   .jss44 {
     color: #f7195c;
   }
   .jss45 {
-    border: 2px solid #6a32a6;
-  }
-  .jss45:hover {
-    background-color: #CBC3E3;
+    color: #f7195c;
   }
   .jss46 {
     border: 2px solid #6a32a6;
   }
+  .jss46:hover {
+    background-color: #CBC3E3;
+  }
   .jss47 {
-    color: #6a32a6;
+    border: 2px solid #6a32a6;
   }
   .jss48 {
     color: #6a32a6;
   }
   .jss49 {
-    border: 2px solid #F9477D;
-  }
-  .jss49:hover {
-    background-color: #FFCCCB;
+    color: #6a32a6;
   }
   .jss50 {
     border: 2px solid #F9477D;
   }
+  .jss50:hover {
+    background-color: #FFCCCB;
+  }
   .jss51 {
-    color: #F9477D;
+    border: 2px solid #F9477D;
   }
   .jss52 {
     color: #F9477D;
   }
   .jss53 {
-    border: 2px solid #3D0A73;
-  }
-  .jss53:hover {
-    background-color: #CBC3E3;
+    color: #F9477D;
   }
   .jss54 {
     border: 2px solid #3D0A73;
   }
+  .jss54:hover {
+    background-color: #CBC3E3;
+  }
   .jss55 {
-    color: #3D0A73;
+    border: 2px solid #3D0A73;
   }
   .jss56 {
     color: #3D0A73;
   }
   .jss57 {
-    border: 2px solid #f7195c;
-  }
-  .jss57:hover {
-    background-color: #FFCCCB;
+    color: #3D0A73;
   }
   .jss58 {
     border: 2px solid #f7195c;
   }
+  .jss58:hover {
+    background-color: #FFCCCB;
+  }
   .jss59 {
-    color: #f7195c;
+    border: 2px solid #f7195c;
   }
   .jss60 {
     color: #f7195c;
   }
   .jss61 {
-    border: 2px solid #6a32a6;
-  }
-  .jss61:hover {
-    background-color: #CBC3E3;
+    color: #f7195c;
   }
   .jss62 {
     border: 2px solid #6a32a6;
   }
+  .jss62:hover {
+    background-color: #CBC3E3;
+  }
   .jss63 {
-    color: #6a32a6;
+    border: 2px solid #6a32a6;
   }
   .jss64 {
     color: #6a32a6;
   }
   .jss65 {
+    color: #6a32a6;
+  }
+  .jss66 {
     border: 2px solid #F9477D;
   }
-  .jss65:hover {
+  .jss66:hover {
     background-color: #FFCCCB;
   }
-  .jss66 {
+  .jss67 {
     border: 2px solid #F9477D;
   }
-  .jss67 {
+  .jss68 {
     color: #F9477D;
   }
-  .jss68 {
+  .jss69 {
     color: #F9477D;
   }
-  .jss15 {
+  .jss16 {
     padding: 0;
     align-items: center;
     justify-content: center;
   }
-  .jss16 {
+  .jss17 {
     width: 40%;
     margin: auto;
     padding: 16px;
   }
-  .jss17 {
+  .jss18 {
     width: 100%;
     display: flex;
     padding: 4px;
     flex-wrap: wrap;
     margin-bottom: 16px;
     justify-content: center;
   }
-  .jss18 {
+  .jss19 {
     width: 35%;
     margin: auto;
     opacity: 70%;
     max-height: 1em;
   }
-  .jss19 {
+  .jss20 {
     margin-bottom: 8px;
   }
-  .jss20 {
+  .jss21 {
     padding: 24px;
   }
-  .jss21 {
+  .jss22 {
     padding: 32px;
   }
-  .jss22 {
+  .jss23 {
     opacity: 0;
   }
-  .jss11 {
-    margin: 5px;
-  }
-  .jss12 {
-    align-items: inherit;
-  }
-  .jss13 {
-    font-size: 18px;
-  }
-  .jss14 {
-    align-items: auto;
-    margin-left: 0.2em;
-    margin-right: 0.2em;
-  }
   .jss2 {
     width: 100%;
     diplay: flex;
   }
   .jss3 {
     color: black;
     width: 100%;
@@ -1456,8 +1472,8 @@
     position: relative;
     font-size: 3em;
     justify-self: flex-end;
   }
   .jss1 {
     padding-left: 64px;
     padding-right: 64px;
-  }</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><div class="jss2"><header class="MuiPaper-root MuiAppBar-root MuiAppBar-positionStatic MuiAppBar-colorPrimary jss3 MuiPaper-elevation4"><div class="MuiToolbar-root MuiToolbar-regular jss6 MuiToolbar-gutters"><div class="jss7"><img src="/static/FeatureForm_Logo_Full_Black.svg" height="30" alt="Featureform" component="div" nowrap="true" style="cursor:pointer" sx="[object Object]"/></div><div class="jss9"></div></div></header></div><div class="MuiContainer-root MuiContainer-maxWidthXl jss1"><div class="jss11"><div></div></div><div><div class="jss15"><div class="jss16"><div class="jss17"></div><div class="jss23"><div class="MuiGrid-root MuiGrid-container MuiGrid-item MuiGrid-justify-content-xs-center"><div class="MuiContainer-root jss25 MuiContainer-maxWidthLg"><div class="jss24"><svg class="MuiSvgIcon-root" focusable="false" viewBox="0 0 24 24" aria-hidden="true"><path d="M15.5 14h-.79l-.28-.27C15.41 12.59 16 11.11 16 9.5 16 5.91 13.09 3 9.5 3S3 5.91 3 9.5 5.91 16 9.5 16c1.61 0 3.09-.59 4.23-1.57l.27.28v.79l5 4.99L20.49 19l-4.99-5zm-6 0C7.01 14 5 11.99 5 9.5S7.01 5 9.5 5 14 7.01 14 9.5 11.99 14 9.5 14z"></path></svg></div><div class="MuiInputBase-root jss26"><input type="text" placeholder="Search..." value="" aria-label="search" data-testid="searchInputId" class="MuiInputBase-input jss27"/></div></div></div></div></div><div class="jss20"><div class="jss21"><div class="jss19"><h5 class="MuiTypography-root MuiTypography-h5"></h5></div><div><div class="MuiGrid-root MuiGrid-container MuiGrid-justify-content-xs-center"><div class="MuiGrid-root MuiGrid-item MuiGrid-grid-xs-12 MuiGrid-grid-md-6 MuiGrid-grid-lg-4"></div><div class="MuiGrid-root MuiGrid-item MuiGrid-grid-xs-12 MuiGrid-grid-md-6 MuiGrid-grid-lg-4"></div><div class="MuiGrid-root MuiGrid-item MuiGrid-grid-xs-12 MuiGrid-grid-md-6 MuiGrid-grid-lg-4"></div><div class="MuiGrid-root MuiGrid-item MuiGrid-grid-xs-12 MuiGrid-grid-md-6 MuiGrid-grid-lg-4"></div><div class="MuiGrid-root MuiGrid-item MuiGrid-grid-xs-12 MuiGrid-grid-md-6 MuiGrid-grid-lg-4"></div><div class="MuiGrid-root MuiGrid-item MuiGrid-grid-xs-12 MuiGrid-grid-md-6 MuiGrid-grid-lg-4"></div><div class="MuiGrid-root MuiGrid-item MuiGrid-grid-xs-12 MuiGrid-grid-md-6 MuiGrid-grid-lg-4"></div><div class="MuiGrid-root MuiGrid-item MuiGrid-grid-xs-12 MuiGrid-grid-md-6 MuiGrid-grid-lg-4"></div></div></div></div></div></div></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/","query":{},"buildId":"XLqQwuMDcHNwRKV5unb2J","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+  }</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><div class="jss2"><header class="MuiPaper-root MuiAppBar-root MuiAppBar-positionStatic MuiAppBar-colorPrimary jss3 MuiPaper-elevation4"><div class="MuiToolbar-root MuiToolbar-regular jss6 MuiToolbar-gutters"><div class="jss7"><img class="MuiBox-root jss11" src="/static/FeatureForm_Logo_Full_Black.svg" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss9"></div></div></header></div><div class="MuiContainer-root MuiContainer-maxWidthXl jss1"><div class="jss12"><div></div></div><div><div class="jss16"><div class="jss17"><div class="jss18"></div><div class="jss24"><div class="MuiGrid-root MuiGrid-container MuiGrid-item MuiGrid-justify-content-xs-center"><div class="MuiContainer-root jss26 MuiContainer-maxWidthLg"><div class="jss25"><svg class="MuiSvgIcon-root" focusable="false" viewBox="0 0 24 24" aria-hidden="true"><path d="M15.5 14h-.79l-.28-.27C15.41 12.59 16 11.11 16 9.5 16 5.91 13.09 3 9.5 3S3 5.91 3 9.5 5.91 16 9.5 16c1.61 0 3.09-.59 4.23-1.57l.27.28v.79l5 4.99L20.49 19l-4.99-5zm-6 0C7.01 14 5 11.99 5 9.5S7.01 5 9.5 5 14 7.01 14 9.5 11.99 14 9.5 14z"></path></svg></div><div class="MuiInputBase-root jss27"><input type="text" placeholder="Search..." value="" aria-label="search" data-testid="searchInputId" class="MuiInputBase-input jss28"/></div></div></div></div></div><div class="jss21"><div class="jss22"><div class="jss20"><h5 class="MuiTypography-root MuiTypography-h5"></h5></div><div><div class="MuiGrid-root MuiGrid-container MuiGrid-justify-content-xs-center"><div class="MuiGrid-root MuiGrid-item MuiGrid-grid-xs-12 MuiGrid-grid-md-6 MuiGrid-grid-lg-4"></div><div class="MuiGrid-root MuiGrid-item MuiGrid-grid-xs-12 MuiGrid-grid-md-6 MuiGrid-grid-lg-4"></div><div class="MuiGrid-root MuiGrid-item MuiGrid-grid-xs-12 MuiGrid-grid-md-6 MuiGrid-grid-lg-4"></div><div class="MuiGrid-root MuiGrid-item MuiGrid-grid-xs-12 MuiGrid-grid-md-6 MuiGrid-grid-lg-4"></div><div class="MuiGrid-root MuiGrid-item MuiGrid-grid-xs-12 MuiGrid-grid-md-6 MuiGrid-grid-lg-4"></div><div class="MuiGrid-root MuiGrid-item MuiGrid-grid-xs-12 MuiGrid-grid-md-6 MuiGrid-grid-lg-4"></div><div class="MuiGrid-root MuiGrid-item MuiGrid-grid-xs-12 MuiGrid-grid-md-6 MuiGrid-grid-lg-4"></div><div class="MuiGrid-root MuiGrid-item MuiGrid-grid-xs-12 MuiGrid-grid-md-6 MuiGrid-grid-lg-4"></div></div></div></div></div></div></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/","query":{},"buildId":"aZJnz9nRD9kOWLAxrQep6","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/search.html` & `featureform-1.8.1/src/featureform/dashboard/out/search.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,136 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-6ed703bc0f4dd2fe.js" defer=""></script><script src="/_next/static/chunks/framework-3412d1150754b2fb.js" defer=""></script><script src="/_next/static/chunks/main-2715d0c23f47c019.js" defer=""></script><script src="/_next/static/chunks/pages/_app-a764893ff9420ec0.js" defer=""></script><script src="/_next/static/chunks/pages/search-175858e61ba25631.js" defer=""></script><script src="/_next/static/XLqQwuMDcHNwRKV5unb2J/_buildManifest.js" defer=""></script><script src="/_next/static/XLqQwuMDcHNwRKV5unb2J/_ssgManifest.js" defer=""></script><style id="jss-server-side">.MuiTypography-root {
-  margin: 0;
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-6ed703bc0f4dd2fe.js" defer=""></script><script src="/_next/static/chunks/framework-3412d1150754b2fb.js" defer=""></script><script src="/_next/static/chunks/main-2715d0c23f47c019.js" defer=""></script><script src="/_next/static/chunks/pages/_app-535a9349f87f23c6.js" defer=""></script><script src="/_next/static/chunks/pages/search-175858e61ba25631.js" defer=""></script><script src="/_next/static/aZJnz9nRD9kOWLAxrQep6/_buildManifest.js" defer=""></script><script src="/_next/static/aZJnz9nRD9kOWLAxrQep6/_ssgManifest.js" defer=""></script><style id="jss-server-side">.MuiContainer-root {
+  width: 100%;
+  display: block;
+  box-sizing: border-box;
+  margin-left: auto;
+  margin-right: auto;
+  padding-left: 16px;
+  padding-right: 16px;
 }
-.MuiTypography-body2 {
-  font-size: 0.875rem;
-  font-family: "Matter", "Lato", "Helvetica", sans-serif;
-  font-weight: 550;
-  line-height: 1.43;
-}
-.MuiTypography-body1 {
-  font-size: 1rem;
-  font-family: "Matter", "Lato", "Helvetica", sans-serif;
-  font-weight: 550;
-  line-height: 1.5;
-}
-.MuiTypography-caption {
-  font-size: 0.75rem;
-  font-family: "Matter", "Lato", "Helvetica", sans-serif;
-  font-weight: 550;
-  line-height: 1.66;
-}
-.MuiTypography-button {
-  font-size: 0.875rem;
-  font-family: "Matter", "Lato", "Helvetica", sans-serif;
-  font-weight: 650;
-  line-height: 1.75;
-  text-transform: uppercase;
-}
-.MuiTypography-h1 {
-  font-size: 3.5rem;
-  font-family: "Matter", "Lato", "Helvetica", sans-serif;
-  font-weight: 450;
-  line-height: 1.167;
+@media (min-width:600px) {
+  .MuiContainer-root {
+    padding-left: 24px;
+    padding-right: 24px;
+  }
+}
+  .MuiContainer-disableGutters {
+    padding-left: 0;
+    padding-right: 0;
+  }
+@media (min-width:600px) {
+  .MuiContainer-fixed {
+    max-width: 600px;
+  }
+}
+@media (min-width:960px) {
+  .MuiContainer-fixed {
+    max-width: 960px;
+  }
+}
+@media (min-width:1280px) {
+  .MuiContainer-fixed {
+    max-width: 1280px;
+  }
+}
+@media (min-width:1920px) {
+  .MuiContainer-fixed {
+    max-width: 1920px;
+  }
+}
+@media (min-width:0px) {
+  .MuiContainer-maxWidthXs {
+    max-width: 444px;
+  }
+}
+@media (min-width:600px) {
+  .MuiContainer-maxWidthSm {
+    max-width: 600px;
+  }
+}
+@media (min-width:960px) {
+  .MuiContainer-maxWidthMd {
+    max-width: 960px;
+  }
+}
+@media (min-width:1280px) {
+  .MuiContainer-maxWidthLg {
+    max-width: 1280px;
+  }
+}
+@media (min-width:1920px) {
+  .MuiContainer-maxWidthXl {
+    max-width: 1920px;
+  }
+}
+  html {
+    box-sizing: border-box;
+    -webkit-font-smoothing: antialiased;
+    -moz-osx-font-smoothing: grayscale;
+  }
+  *, *::before, *::after {
+    box-sizing: inherit;
+  }
+  strong, b {
+    font-weight: 700;
+  }
+  body {
+    color: #263238;
+    margin: 0;
+    font-size: 0.875rem;
+    background: radial-gradient(circle farthest-side, #E4D0FA 0%, rgba(255, 0, 0, 0) 40%) top left/200% 100%, radial-gradient(circle farthest-side, #FCA3BE 0%, rgba(255, 0, 0, 0) 40%) top right/180% 150%;;
+    font-family: "Matter", "Lato", "Helvetica", sans-serif;
+    font-weight: 550;
+    line-height: 1.43;
+    background-color: #FFFFFF;
+    background-repeat: no-repeat;
+    background-attachment: fixed;
+  }
+@media print {
+  body {
+    background-color: #fff;
+  }
 }
+  body::backdrop {
+    background-color: #FFFFFF;
+  }
+  .MuiTypography-root {
+    margin: 0;
+  }
+  .MuiTypography-body2 {
+    font-size: 0.875rem;
+    font-family: "Matter", "Lato", "Helvetica", sans-serif;
+    font-weight: 550;
+    line-height: 1.43;
+  }
+  .MuiTypography-body1 {
+    font-size: 1rem;
+    font-family: "Matter", "Lato", "Helvetica", sans-serif;
+    font-weight: 550;
+    line-height: 1.5;
+  }
+  .MuiTypography-caption {
+    font-size: 0.75rem;
+    font-family: "Matter", "Lato", "Helvetica", sans-serif;
+    font-weight: 550;
+    line-height: 1.66;
+  }
+  .MuiTypography-button {
+    font-size: 0.875rem;
+    font-family: "Matter", "Lato", "Helvetica", sans-serif;
+    font-weight: 650;
+    line-height: 1.75;
+    text-transform: uppercase;
+  }
+  .MuiTypography-h1 {
+    font-size: 3.5rem;
+    font-family: "Matter", "Lato", "Helvetica", sans-serif;
+    font-weight: 450;
+    line-height: 1.167;
+  }
 @media (min-width:600px) {
   .MuiTypography-h1 {
     font-size: 4.7129rem;
   }
 }
 @media (min-width:960px) {
   .MuiTypography-h1 {
@@ -220,14 +315,42 @@
   }
   .MuiTypography-displayInline {
     display: inline;
   }
   .MuiTypography-displayBlock {
     display: block;
   }
+  .MuiBreadcrumbs-ol {
+    margin: 0;
+    display: flex;
+    padding: 0;
+    flex-wrap: wrap;
+    list-style: none;
+    align-items: center;
+  }
+  .MuiBreadcrumbs-separator {
+    display: flex;
+    margin-left: 8px;
+    user-select: none;
+    margin-right: 8px;
+  }
+  .jss12 {
+    margin: 5px;
+  }
+  .jss13 {
+    align-items: inherit;
+  }
+  .jss14 {
+    font-size: 18px;
+  }
+  .jss15 {
+    align-items: auto;
+    margin-left: 0.2em;
+    margin-right: 0.2em;
+  }
   .MuiPaper-root {
     color: #263238;
     transition: box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;
     background-color: #fff;
   }
   .MuiPaper-rounded {
     border-radius: 4px;
@@ -306,58 +429,14 @@
   }
   .MuiPaper-elevation23 {
     box-shadow: 0px 11px 14px -7px rgba(0,0,0,0.2),0px 23px 36px 3px rgba(0,0,0,0.14),0px 9px 44px 8px rgba(0,0,0,0.12);
   }
   .MuiPaper-elevation24 {
     box-shadow: 0px 11px 15px -7px rgba(0,0,0,0.2),0px 24px 38px 3px rgba(0,0,0,0.14),0px 9px 46px 8px rgba(0,0,0,0.12);
   }
-  .MuiList-root {
-    margin: 0;
-    padding: 0;
-    position: relative;
-    list-style: none;
-  }
-  .MuiList-padding {
-    padding-top: 8px;
-    padding-bottom: 8px;
-  }
-  .MuiList-subheader {
-    padding-top: 0;
-  }
-  .MuiToolbar-root {
-    display: flex;
-    position: relative;
-    align-items: center;
-  }
-  .MuiToolbar-gutters {
-    padding-left: 16px;
-    padding-right: 16px;
-  }
-@media (min-width:600px) {
-  .MuiToolbar-gutters {
-    padding-left: 24px;
-    padding-right: 24px;
-  }
-}
-  .MuiToolbar-regular {
-    min-height: 56px;
-  }
-@media (min-width:0px) and (orientation: landscape) {
-  .MuiToolbar-regular {
-    min-height: 48px;
-  }
-}
-@media (min-width:600px) {
-  .MuiToolbar-regular {
-    min-height: 64px;
-  }
-}
-  .MuiToolbar-dense {
-    min-height: 48px;
-  }
   .MuiAppBar-root {
     width: 100%;
     display: flex;
     z-index: 1100;
     box-sizing: border-box;
     flex-shrink: 0;
     flex-direction: column;
@@ -406,155 +485,92 @@
   .MuiAppBar-colorInherit {
     color: inherit;
   }
   .MuiAppBar-colorTransparent {
     color: inherit;
     background-color: transparent;
   }
-  .MuiBreadcrumbs-ol {
+
+  .jss11 {
+    height: 30px;
+    display: [object Object];
+    flex-grow: 1;
+  }
+@media (min-width:0px) {
+  .jss11 {
+    display: none;
+  }
+}
+@media (min-width:600px) {
+  .jss11 {
+    display: block;
+  }
+}
+  .MuiList-root {
     margin: 0;
-    display: flex;
     padding: 0;
-    flex-wrap: wrap;
+    position: relative;
     list-style: none;
-    align-items: center;
   }
-  .MuiBreadcrumbs-separator {
+  .MuiList-padding {
+    padding-top: 8px;
+    padding-bottom: 8px;
+  }
+  .MuiList-subheader {
+    padding-top: 0;
+  }
+  .MuiToolbar-root {
     display: flex;
-    margin-left: 8px;
-    user-select: none;
-    margin-right: 8px;
+    position: relative;
+    align-items: center;
   }
-  .MuiContainer-root {
-    width: 100%;
-    display: block;
-    box-sizing: border-box;
-    margin-left: auto;
-    margin-right: auto;
+  .MuiToolbar-gutters {
     padding-left: 16px;
     padding-right: 16px;
   }
 @media (min-width:600px) {
-  .MuiContainer-root {
+  .MuiToolbar-gutters {
     padding-left: 24px;
     padding-right: 24px;
   }
 }
-  .MuiContainer-disableGutters {
-    padding-left: 0;
-    padding-right: 0;
-  }
-@media (min-width:600px) {
-  .MuiContainer-fixed {
-    max-width: 600px;
-  }
-}
-@media (min-width:960px) {
-  .MuiContainer-fixed {
-    max-width: 960px;
-  }
-}
-@media (min-width:1280px) {
-  .MuiContainer-fixed {
-    max-width: 1280px;
-  }
-}
-@media (min-width:1920px) {
-  .MuiContainer-fixed {
-    max-width: 1920px;
+  .MuiToolbar-regular {
+    min-height: 56px;
   }
-}
-@media (min-width:0px) {
-  .MuiContainer-maxWidthXs {
-    max-width: 444px;
+@media (min-width:0px) and (orientation: landscape) {
+  .MuiToolbar-regular {
+    min-height: 48px;
   }
 }
 @media (min-width:600px) {
-  .MuiContainer-maxWidthSm {
-    max-width: 600px;
-  }
-}
-@media (min-width:960px) {
-  .MuiContainer-maxWidthMd {
-    max-width: 960px;
-  }
-}
-@media (min-width:1280px) {
-  .MuiContainer-maxWidthLg {
-    max-width: 1280px;
-  }
-}
-@media (min-width:1920px) {
-  .MuiContainer-maxWidthXl {
-    max-width: 1920px;
-  }
-}
-  html {
-    box-sizing: border-box;
-    -webkit-font-smoothing: antialiased;
-    -moz-osx-font-smoothing: grayscale;
-  }
-  *, *::before, *::after {
-    box-sizing: inherit;
-  }
-  strong, b {
-    font-weight: 700;
-  }
-  body {
-    color: #263238;
-    margin: 0;
-    font-size: 0.875rem;
-    background: radial-gradient(circle farthest-side, #E4D0FA 0%, rgba(255, 0, 0, 0) 40%) top left/200% 100%, radial-gradient(circle farthest-side, #FCA3BE 0%, rgba(255, 0, 0, 0) 40%) top right/180% 150%;;
-    font-family: "Matter", "Lato", "Helvetica", sans-serif;
-    font-weight: 550;
-    line-height: 1.43;
-    background-color: #FFFFFF;
-    background-repeat: no-repeat;
-    background-attachment: fixed;
-  }
-@media print {
-  body {
-    background-color: #fff;
+  .MuiToolbar-regular {
+    min-height: 64px;
   }
 }
-  body::backdrop {
-    background-color: #FFFFFF;
-  }
-  .jss11 {
-    margin: 5px;
-  }
-  .jss12 {
-    align-items: inherit;
-  }
-  .jss13 {
-    font-size: 18px;
-  }
-  .jss14 {
-    align-items: auto;
-    margin-left: 0.2em;
-    margin-right: 0.2em;
+  .MuiToolbar-dense {
+    min-height: 48px;
   }
-  .jss15 {
+  .jss16 {
     border: 2px solid #F5F6F7;
     background: rgba(255, 255, 255, 1);
     border-radius: 16px;
   }
-  .jss16 {
+  .jss17 {
     color: black;
     padding: 0;
     background: transparent;
     box-shadow: none;
     padding-left: 32px;
     padding-right: 32px;
   }
-  .jss17 {
+  .jss18 {
     padding: 8px;
     padding-top: 32px;
   }
-  .jss18 {
+  .jss19 {
     display: inline;
     line-height: 1.2;
   }
   .jss2 {
     width: 100%;
     diplay: flex;
   }
@@ -594,8 +610,8 @@
     position: relative;
     font-size: 3em;
     justify-self: flex-end;
   }
   .jss1 {
     padding-left: 64px;
     padding-right: 64px;
-  }</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><div class="jss2"><header class="MuiPaper-root MuiAppBar-root MuiAppBar-positionStatic MuiAppBar-colorPrimary jss3 MuiPaper-elevation4"><div class="MuiToolbar-root MuiToolbar-regular jss6 MuiToolbar-gutters"><div class="jss7"><img src="/static/FeatureForm_Logo_Full_Black.svg" height="30" alt="Featureform" component="div" nowrap="true" style="cursor:pointer" sx="[object Object]"/></div><div class="jss9"></div></div></header></div><div class="MuiContainer-root MuiContainer-maxWidthXl jss1"><div class="jss11"><nav class="MuiTypography-root MuiBreadcrumbs-root jss13 MuiTypography-body1 MuiTypography-colorTextSecondary" style="margin:0.25em" aria-label="breadcrumb"><ol class="MuiBreadcrumbs-ol jss12"><li class="MuiBreadcrumbs-li"><a href="/">Home</a></li><li aria-hidden="true" class="MuiBreadcrumbs-separator jss14"><style data-emotion="css vubbuv">.css-vubbuv{-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;width:1em;height:1em;display:inline-block;fill:currentColor;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;-webkit-transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;font-size:1.5rem;}</style><svg class="MuiSvgIcon-root MuiSvgIcon-fontSizeMedium css-vubbuv" focusable="false" aria-hidden="true" viewBox="0 0 24 24" data-testid="NavigateNextIcon"><path d="M10 6 8.59 7.41 13.17 12l-4.58 4.59L10 18l6-6z"></path></svg></li><li class="MuiBreadcrumbs-li"><b>Search</b></li></ol></nav></div><div><div><div class="MuiContainer-root jss15 MuiContainer-maxWidthXl"><h4 class="MuiTypography-root jss17 MuiTypography-h4" style="display:flex"><div style="color:gray">No results for: </div><b></b></h4><div><nav class="MuiList-root jss15 MuiList-padding"></nav></div></div></div></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/search","query":{},"buildId":"XLqQwuMDcHNwRKV5unb2J","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+  }</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><div class="jss2"><header class="MuiPaper-root MuiAppBar-root MuiAppBar-positionStatic MuiAppBar-colorPrimary jss3 MuiPaper-elevation4"><div class="MuiToolbar-root MuiToolbar-regular jss6 MuiToolbar-gutters"><div class="jss7"><img class="MuiBox-root jss11" src="/static/FeatureForm_Logo_Full_Black.svg" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss9"></div></div></header></div><div class="MuiContainer-root MuiContainer-maxWidthXl jss1"><div class="jss12"><nav class="MuiTypography-root MuiBreadcrumbs-root jss14 MuiTypography-body1 MuiTypography-colorTextSecondary" style="margin:0.25em" aria-label="breadcrumb"><ol class="MuiBreadcrumbs-ol jss13"><li class="MuiBreadcrumbs-li"><a href="/">Home</a></li><li aria-hidden="true" class="MuiBreadcrumbs-separator jss15"><style data-emotion="css vubbuv">.css-vubbuv{-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;width:1em;height:1em;display:inline-block;fill:currentColor;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;-webkit-transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;font-size:1.5rem;}</style><svg class="MuiSvgIcon-root MuiSvgIcon-fontSizeMedium css-vubbuv" focusable="false" aria-hidden="true" viewBox="0 0 24 24" data-testid="NavigateNextIcon"><path d="M10 6 8.59 7.41 13.17 12l-4.58 4.59L10 18l6-6z"></path></svg></li><li class="MuiBreadcrumbs-li"><b>Search</b></li></ol></nav></div><div><div><div class="MuiContainer-root jss16 MuiContainer-maxWidthXl"><h4 class="MuiTypography-root jss18 MuiTypography-h4" style="display:flex"><div style="color:gray">No results for: </div><b></b></h4><div><nav class="MuiList-root jss16 MuiList-padding"></nav></div></div></div></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/search","query":{},"buildId":"aZJnz9nRD9kOWLAxrQep6","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/static/Apache_Spark_logo.svg` & `featureform-1.8.1/src/featureform/dashboard/out/static/Apache_Spark_logo.svg`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/static/Capital_One_logo.svg` & `featureform-1.8.1/src/featureform/dashboard/out/static/Capital_One_logo.svg`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/static/FeatureForm_Logo_Full_Black.svg` & `featureform-1.8.1/src/featureform/dashboard/out/static/FeatureForm_Logo_Full_Black.svg`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/static/Featureform_logo_pink.svg` & `featureform-1.8.1/src/featureform/dashboard/out/static/Featureform_logo_pink.svg`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/static/Kubernetes_logo.svg` & `featureform-1.8.1/src/featureform/dashboard/out/static/Kubernetes_logo.svg`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/static/Postgresql_elephant.svg` & `featureform-1.8.1/src/featureform/dashboard/out/static/Postgresql_elephant.svg`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/static/Redis_Logo.svg` & `featureform-1.8.1/src/featureform/dashboard/out/static/Redis_Logo.svg`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/static/Snowflake_Logo.svg` & `featureform-1.8.1/src/featureform/dashboard/out/static/Snowflake_Logo.svg`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/static/amazon-dynamoDB.svg` & `featureform-1.8.1/src/featureform/dashboard/out/static/amazon-dynamoDB.svg`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/static/amazon_redshift.svg` & `featureform-1.8.1/src/featureform/dashboard/out/static/amazon_redshift.svg`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/static/amazon_s3.svg` & `featureform-1.8.1/src/featureform/dashboard/out/static/amazon_s3.svg`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/static/apache_cassandra.svg` & `featureform-1.8.1/src/featureform/dashboard/out/static/apache_cassandra.svg`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/static/apache_hadoop.svg` & `featureform-1.8.1/src/featureform/dashboard/out/static/apache_hadoop.svg`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/static/apple-touch-icon.png` & `featureform-1.8.1/src/featureform/dashboard/out/static/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/static/azure_storage_accounts.svg` & `featureform-1.8.1/src/featureform/dashboard/out/static/azure_storage_accounts.svg`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/static/favicon.ico` & `featureform-1.8.1/src/featureform/dashboard/out/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/static/google_bigquery.svg` & `featureform-1.8.1/src/featureform/dashboard/out/static/google_bigquery.svg`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/static/google_cloud_storage.svg` & `featureform-1.8.1/src/featureform/dashboard/out/static/google_cloud_storage.svg`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/static/google_firestore.svg` & `featureform-1.8.1/src/featureform/dashboard/out/static/google_firestore.svg`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/static/logo192.png` & `featureform-1.8.1/src/featureform/dashboard/out/static/logo192.png`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/static/logo512.png` & `featureform-1.8.1/src/featureform/dashboard/out/static/logo512.png`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/static/mongoDB.svg` & `featureform-1.8.1/src/featureform/dashboard/out/static/mongoDB.svg`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard/out/static/safari-pinned-tab.svg` & `featureform-1.8.1/src/featureform/dashboard/out/static/safari-pinned-tab.svg`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/dashboard_metadata.py` & `featureform-1.8.1/src/featureform/dashboard_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,20 @@
 @dashboard_app.route("/<type>/<entity>")
 def entity(type, entity):
     return dashboard_app.send_static_file("[type]/[entity].html")
 
 
 @dashboard_app.route("/search")
 def search():
-    return dashboard_app.send_static_file("search.html")
+    return dashboard_app.send_static_file("query.html")
+
+
+@dashboard_app.route("/query")
+def query():
+    return dashboard_app.send_static_file("query.html")
 
 
 @dashboard_app.route("/static/<asset>")
 def deliver_static(asset):
     return dashboard_app.send_static_file("static/" + asset)
```

### Comparing `featureform-1.8.0/src/featureform/enums.py` & `featureform-1.8.1/src/featureform/enums.py`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/get.py` & `featureform-1.8.1/src/featureform/get.py`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/get_local.py` & `featureform-1.8.1/src/featureform/get_local.py`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/get_test.py` & `featureform-1.8.1/src/featureform/get_test.py`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/list.py` & `featureform-1.8.1/src/featureform/list.py`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/list_local.py` & `featureform-1.8.1/src/featureform/list_local.py`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/list_test.py` & `featureform-1.8.1/src/featureform/list_test.py`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/local_cache.py` & `featureform-1.8.1/src/featureform/local_cache.py`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/local_dash_test.py` & `featureform-1.8.1/src/featureform/local_dash_test.py`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/local_utils.py` & `featureform-1.8.1/src/featureform/local_utils.py`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/proto/metadata.proto` & `featureform-1.8.1/src/featureform/proto/metadata.proto`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/proto/metadata_pb2.py` & `featureform-1.8.1/src/featureform/proto/metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/proto/metadata_pb2_grpc.py` & `featureform-1.8.1/src/featureform/proto/metadata_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/proto/serving.proto` & `featureform-1.8.1/src/featureform/proto/serving.proto`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/proto/serving_pb2.py` & `featureform-1.8.1/src/featureform/proto/serving_pb2.py`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/proto/serving_pb2_grpc.py` & `featureform-1.8.1/src/featureform/proto/serving_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/register.py` & `featureform-1.8.1/src/featureform/register.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from os.path import exists
 from datetime import timedelta
+
 from typeguard import typechecked
 from typing import Dict, Tuple, Callable, List, Union
 import warnings
 import inspect
 
 import dill
 import pandas as pd
 
 from .get import *
 from .list import *
 from .get_local import *
 from .list_local import *
 from .sqlite_metadata import SQLiteMetadata
+from .status_display import display_statuses
 from .tls import insecure_channel, secure_channel
 from .resources import (
     ColumnTypes,
     Model,
     ResourceState,
     Provider,
     RedisConfig,
@@ -52,15 +54,14 @@
     TrainingSet,
     ProviderReference,
     EntityReference,
     SourceReference,
     ExecutorCredentials,
     ResourceRedefinedError,
     ResourceStatus,
-    Transformation,
     K8sArgs,
     AWSCredentials,
     GCPCredentials,
     HDFSConfig,
     K8sResourceSpecs,
     FilePrefix,
     OnDemandFeature,
@@ -2863,14 +2864,27 @@
         if owner == "":
             owner = self.must_get_default_owner()
         if not isinstance(provider, str):
             provider = provider.name()
         for i, nv in enumerate(inputs):
             if not isinstance(nv, tuple):
                 inputs[i] = nv.name_variant()
+            if isinstance(nv, tuple):
+                try:
+                    self._verify_tuple(nv)
+                except TypeError as e:
+                    transformation_message = f"'{name}:{variant}'"
+                    if name == "":
+                        transformation_message = f"with '{variant}' variant"
+
+                    raise TypeError(
+                        f"DF transformation {transformation_message} requires correct inputs "
+                        f" '{nv}' is not a valid tuple: {e}"
+                    )
+
         decorator = DFTransformationDecorator(
             registrar=self,
             name=name,
             variant=variant,
             provider=provider,
             owner=owner,
             description=description,
@@ -2878,14 +2892,33 @@
             args=args,
             tags=tags,
             properties=properties,
         )
         self.__resources.append(decorator)
         return decorator
 
+    def _verify_tuple(self, nv_tuple):
+        if not isinstance(nv_tuple, tuple):
+            raise TypeError(f"not a tuple; received: '{type(nv_tuple).__name__}' type")
+
+        if len(nv_tuple) != 2:
+            raise TypeError(
+                "Tuple must be of length 2, got length {}".format(len(nv_tuple))
+            )
+        if len(nv_tuple) == 2:
+            not_string_tuples = not (
+                isinstance(nv_tuple[0], str) and isinstance(nv_tuple[1], str)
+            )
+            if not_string_tuples:
+                first_position_type = type(nv_tuple[0]).__name__
+                second_position_type = type(nv_tuple[1]).__name__
+                raise TypeError(
+                    f"Tuple must be of type (str, str); got ({first_position_type}, {second_position_type})"
+                )
+
     def ondemand_feature(
         self,
         fn=None,
         *,
         tags: List[str] = None,
         properties: dict = None,
         variant: str = "default",
```

### Comparing `featureform-1.8.0/src/featureform/register_test.py` & `featureform-1.8.1/src/featureform/register_test.py`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/resources.py` & `featureform-1.8.1/src/featureform/resources.py`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/search.py` & `featureform-1.8.1/src/featureform/search.py`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/serving.py` & `featureform-1.8.1/src/featureform/serving.py`

 * *Files 1% similar despite different names*

```diff
@@ -504,15 +504,21 @@
     def feature_df_from_transformation(self, feature):
         df = self.process_transformation(
             feature["source_name"], feature["source_variant"]
         )
         if isinstance(df, pd.Series):
             df = df.to_frame()
             df.reset_index(inplace=True)
-        if feature["source_timestamp"] != "":
+        if feature["source_timestamp"] != "" and feature["source_timestamp"] not in df:
+            raise ValueError(
+                f"Provided timestamp column '{feature['source_timestamp']}' for feature "
+                f"'{feature['name']}:{feature['variant']}' not found in source '{feature['source_name']}:{feature['source_variant']}'; "
+                f"either remove 'timestamp_column' from the feature registration or include it in the source."
+            )
+        elif feature["source_timestamp"] != "":
             df = df[
                 [
                     feature["source_entity"],
                     feature["source_value"],
                     feature["source_timestamp"],
                 ]
             ]
```

### Comparing `featureform-1.8.0/src/featureform/sqlite_metadata.py` & `featureform-1.8.1/src/featureform/sqlite_metadata.py`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/type_objects.py` & `featureform-1.8.1/src/featureform/type_objects.py`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform/version.py` & `featureform-1.8.1/src/featureform/version.py`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/src/featureform.egg-info/PKG-INFO` & `featureform-1.8.1/src/featureform.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featureform
-Version: 1.8.0
+Version: 1.8.1
 Summary: Package for the Featureform Feature Store
 Home-page: https://featureform.com
 Author: FeatureForm, Inc.
 Author-email: hello@featureform.com
 Project-URL: Bug Tracker, https://github.com/featureform/embeddinghub/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

### Comparing `featureform-1.8.0/src/featureform.egg-info/SOURCES.txt` & `featureform-1.8.1/src/featureform.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -26,35 +26,37 @@
 src/featureform/register_test.py
 src/featureform/resources.py
 src/featureform/search.py
 src/featureform/search_local.py
 src/featureform/serving.py
 src/featureform/serving_test.py
 src/featureform/sqlite_metadata.py
+src/featureform/status_display.py
 src/featureform/tls.py
 src/featureform/type_objects.py
 src/featureform/version.py
 src/featureform.egg-info/PKG-INFO
 src/featureform.egg-info/SOURCES.txt
 src/featureform.egg-info/dependency_links.txt
 src/featureform.egg-info/entry_points.txt
 src/featureform.egg-info/requires.txt
 src/featureform.egg-info/top_level.txt
 src/featureform/dashboard/out/404.html
 src/featureform/dashboard/out/[type].html
 src/featureform/dashboard/out/connections.html
 src/featureform/dashboard/out/index.html
+src/featureform/dashboard/out/query.html
 src/featureform/dashboard/out/robots.txt
 src/featureform/dashboard/out/search.html
 src/featureform/dashboard/out/site.webmanifest
 src/featureform/dashboard/out/[type]/[entity].html
 src/featureform/dashboard/out/_next/static/Jopdpwd8wB7tMgkcaVnsn/_buildManifest.js
 src/featureform/dashboard/out/_next/static/Jopdpwd8wB7tMgkcaVnsn/_ssgManifest.js
-src/featureform/dashboard/out/_next/static/XLqQwuMDcHNwRKV5unb2J/_buildManifest.js
-src/featureform/dashboard/out/_next/static/XLqQwuMDcHNwRKV5unb2J/_ssgManifest.js
+src/featureform/dashboard/out/_next/static/aZJnz9nRD9kOWLAxrQep6/_buildManifest.js
+src/featureform/dashboard/out/_next/static/aZJnz9nRD9kOWLAxrQep6/_ssgManifest.js
 src/featureform/dashboard/out/_next/static/chunks/72a30a16.5298cad0ba46633d.js
 src/featureform/dashboard/out/_next/static/chunks/7679.34cabcdac6ff42f5.js
 src/featureform/dashboard/out/_next/static/chunks/7856.43cc2293f00befb0.js
 src/featureform/dashboard/out/_next/static/chunks/ad7f724d.b238476ad0e6f6d2.js
 src/featureform/dashboard/out/_next/static/chunks/framework-3412d1150754b2fb.js
 src/featureform/dashboard/out/_next/static/chunks/main-2715d0c23f47c019.js
 src/featureform/dashboard/out/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
@@ -279,21 +281,22 @@
 src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xojo.81cb4d9104c6ac5b.js
 src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xquery.4382c54a41b1309a.js
 src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_yaml.178577f1d765f16b.js
 src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_yang.28bbfbd268843c68.js
 src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_zig.a535909b59fc6987.js
 src/featureform/dashboard/out/_next/static/chunks/webpack-6ed703bc0f4dd2fe.js
 src/featureform/dashboard/out/_next/static/chunks/pages/404-baaca4b2f4acc755.js
-src/featureform/dashboard/out/_next/static/chunks/pages/[type]-751a928da9d524e9.js
-src/featureform/dashboard/out/_next/static/chunks/pages/_app-a764893ff9420ec0.js
+src/featureform/dashboard/out/_next/static/chunks/pages/[type]-1354c91ed8b0be2c.js
+src/featureform/dashboard/out/_next/static/chunks/pages/_app-535a9349f87f23c6.js
 src/featureform/dashboard/out/_next/static/chunks/pages/_error-3f70f2d61eb8c6dd.js
 src/featureform/dashboard/out/_next/static/chunks/pages/connections-1d67ba61869dece6.js
-src/featureform/dashboard/out/_next/static/chunks/pages/index-c2ee5b1681e97e4b.js
+src/featureform/dashboard/out/_next/static/chunks/pages/index-942ec646d90d2132.js
+src/featureform/dashboard/out/_next/static/chunks/pages/query-9193959c04ff1e72.js
 src/featureform/dashboard/out/_next/static/chunks/pages/search-175858e61ba25631.js
-src/featureform/dashboard/out/_next/static/chunks/pages/[type]/[entity]-b07f3c4463890639.js
+src/featureform/dashboard/out/_next/static/chunks/pages/[type]/[entity]-92ac9566fcd3bf59.js
 src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter/refractor-core-import.d200df4f5651fe3c.js
 src/featureform/dashboard/out/_next/static/css/85a2addfd2efc882.css
 src/featureform/dashboard/out/_next/static/media/Matter-Regular.f1ae4ce5.ttf
 src/featureform/dashboard/out/_next/static/u8jMEl73MAEGHR4r4U4Dw/_buildManifest.js
 src/featureform/dashboard/out/_next/static/u8jMEl73MAEGHR4r4U4Dw/_ssgManifest.js
 src/featureform/dashboard/out/_next/static/xB9Lh8aE_cExc1t6WFtEI/_buildManifest.js
 src/featureform/dashboard/out/_next/static/xB9Lh8aE_cExc1t6WFtEI/_ssgManifest.js
```

### Comparing `featureform-1.8.0/tests/test_class_api.py` & `featureform-1.8.1/tests/test_class_api.py`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/tests/test_cli.py` & `featureform-1.8.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/tests/test_executor_resources.py` & `featureform-1.8.1/tests/test_executor_resources.py`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/tests/test_getting_model.py` & `featureform-1.8.1/tests/test_getting_model.py`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/tests/test_localmode_caching.py` & `featureform-1.8.1/tests/test_localmode_caching.py`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/tests/test_localmode_include_label_ts.py` & `featureform-1.8.1/tests/test_localmode_include_label_ts.py`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/tests/test_localmode_lag_features.py` & `featureform-1.8.1/tests/test_localmode_lag_features.py`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/tests/test_ondemand_features.py` & `featureform-1.8.1/tests/test_ondemand_features.py`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/tests/test_resource_registration.py` & `featureform-1.8.1/tests/test_resource_registration.py`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/tests/test_search.py` & `featureform-1.8.1/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/tests/test_serving_model.py` & `featureform-1.8.1/tests/test_serving_model.py`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/tests/test_source_dataframe.py` & `featureform-1.8.1/tests/test_source_dataframe.py`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/tests/test_spark_provider.py` & `featureform-1.8.1/tests/test_spark_provider.py`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/tests/test_tags_and_properties.py` & `featureform-1.8.1/tests/test_tags_and_properties.py`

 * *Files identical despite different names*

### Comparing `featureform-1.8.0/tests/test_updating_provider.py` & `featureform-1.8.1/tests/test_updating_provider.py`

 * *Files identical despite different names*

