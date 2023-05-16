# Comparing `tmp/dhi-platform-1.0.7.tar.gz` & `tmp/dhi-platform-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dhi-platform-1.0.7.tar", last modified: Tue Apr 25 12:34:07 2023, max compression
+gzip compressed data, was "dhi-platform-1.0.8.tar", last modified: Tue May 16 10:56:02 2023, max compression
```

## Comparing `dhi-platform-1.0.7.tar` & `dhi-platform-1.0.8.tar`

### file list

```diff
@@ -1,181 +1,181 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-25 12:34:07.032268 dhi-platform-1.0.7/
--rw-r--r--   0 vsts      (1001) docker     (123)     1005 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (123)     7342 2023-04-25 12:34:07.032268 dhi-platform-1.0.7/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     6570 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-25 12:34:07.008268 dhi-platform-1.0.7/bin/
--rw-r--r--   0 vsts      (1001) docker     (123)      905 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/bin/plt
--rw-r--r--   0 vsts      (1001) docker     (123)     1245 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/bin/plt.bat
--rw-r--r--   0 vsts      (1001) docker     (123)      103 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (123)     1293 2023-04-25 12:34:07.032268 dhi-platform-1.0.7/setup.cfg
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-25 12:34:07.008268 dhi-platform-1.0.7/src/
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-25 12:34:07.008268 dhi-platform-1.0.7/src/dhi/
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-25 12:34:07.016268 dhi-platform-1.0.7/src/dhi/platform/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)       18 2023-04-25 12:33:59.000000 dhi-platform-1.0.7/src/dhi/platform/_version.py
--rw-r--r--   0 vsts      (1001) docker     (123)    11926 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/args.py
--rw-r--r--   0 vsts      (1001) docker     (123)    12925 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/authentication.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-25 12:34:07.016268 dhi-platform-1.0.7/src/dhi/platform/base/
--rw-r--r--   0 vsts      (1001) docker     (123)    18071 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/base/client.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1394 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/base/constants.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2144 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/base/exceptions.py
--rw-r--r--   0 vsts      (1001) docker     (123)      667 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/base/utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-25 12:34:07.016268 dhi-platform-1.0.7/src/dhi/platform/cli/
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-25 12:34:07.016268 dhi-platform-1.0.7/src/dhi/platform/cli/cfg/
--rw-r--r--   0 vsts      (1001) docker     (123)     4615 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/cfg/login.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-25 12:34:07.016268 dhi-platform-1.0.7/src/dhi/platform/cli/ds/
--rw-r--r--   0 vsts      (1001) docker     (123)     1746 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/ds/append.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2550 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/ds/convert.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2196 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/ds/cp.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2609 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/ds/cpbh.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2914 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/ds/cph.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1227 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/ds/download.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1569 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/ds/downloadc.py
--rw-r--r--   0 vsts      (1001) docker     (123)      831 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/ds/info.py
--rw-r--r--   0 vsts      (1001) docker     (123)      855 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/ds/infor.py
--rw-r--r--   0 vsts      (1001) docker     (123)      818 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/ds/ls.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1138 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/ds/lsh.py
--rw-r--r--   0 vsts      (1001) docker     (123)      728 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/ds/lsra.py
--rw-r--r--   0 vsts      (1001) docker     (123)      560 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/ds/restore.py
--rw-r--r--   0 vsts      (1001) docker     (123)      551 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/ds/rm.py
--rw-r--r--   0 vsts      (1001) docker     (123)      557 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/ds/rmhard.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1742 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/ds/update.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2354 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/ds/upload.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1883 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/ds/uploadstaged.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-25 12:34:07.020268 dhi-platform-1.0.7/src/dhi/platform/cli/eng/
--rw-r--r--   0 vsts      (1001) docker     (123)      596 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/eng/cancel.py
--rw-r--r--   0 vsts      (1001) docker     (123)      689 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/eng/configurations.py
--rw-r--r--   0 vsts      (1001) docker     (123)      755 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/eng/diag.py
--rw-r--r--   0 vsts      (1001) docker     (123)      787 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/eng/engine.py
--rw-r--r--   0 vsts      (1001) docker     (123)      645 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/eng/engines.py
--rw-r--r--   0 vsts      (1001) docker     (123)      830 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/eng/info.py
--rw-r--r--   0 vsts      (1001) docker     (123)      635 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/eng/input.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1936 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/eng/list.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2751 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/eng/listmy.py
--rw-r--r--   0 vsts      (1001) docker     (123)      571 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/eng/rm.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3076 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/eng/run.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3092 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/eng/runp.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2552 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/eng/sbmessages.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-25 12:34:07.020268 dhi-platform-1.0.7/src/dhi/platform/cli/gw/
--rw-r--r--   0 vsts      (1001) docker     (123)      740 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/gw/service.py
--rw-r--r--   0 vsts      (1001) docker     (123)      611 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/gw/services.py
--rw-r--r--   0 vsts      (1001) docker     (123)      366 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/help.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-25 12:34:07.020268 dhi-platform-1.0.7/src/dhi/platform/cli/prj/
--rw-r--r--   0 vsts      (1001) docker     (123)      822 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/prj/capabilities.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1659 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/prj/create.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1656 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/prj/createsub.py
--rw-r--r--   0 vsts      (1001) docker     (123)      812 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/prj/info.py
--rw-r--r--   0 vsts      (1001) docker     (123)      806 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/prj/infor.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1496 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/prj/ls.py
--rw-r--r--   0 vsts      (1001) docker     (123)      978 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/prj/lsh.py
--rw-r--r--   0 vsts      (1001) docker     (123)      708 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/prj/lsr.py
--rw-r--r--   0 vsts      (1001) docker     (123)      740 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/prj/path.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1732 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/prj/prepare.py
--rw-r--r--   0 vsts      (1001) docker     (123)      561 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/prj/restore.py
--rw-r--r--   0 vsts      (1001) docker     (123)      552 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/prj/rm.py
--rw-r--r--   0 vsts      (1001) docker     (123)      558 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/prj/rmhard.py
--rw-r--r--   0 vsts      (1001) docker     (123)      567 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/prj/sas.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1519 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/prj/sub.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1637 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/prj/update.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-25 12:34:07.020268 dhi-platform-1.0.7/src/dhi/platform/cli/prjm/
--rw-r--r--   0 vsts      (1001) docker     (123)     1054 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/prjm/add.py
--rw-r--r--   0 vsts      (1001) docker     (123)      871 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/prjm/all.py
--rw-r--r--   0 vsts      (1001) docker     (123)      667 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/prjm/ls.py
--rw-r--r--   0 vsts      (1001) docker     (123)      741 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/prjm/rm.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-25 12:34:07.024268 dhi-platform-1.0.7/src/dhi/platform/cli/raw/
--rw-r--r--   0 vsts      (1001) docker     (123)      611 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/raw/blocks.py
--rw-r--r--   0 vsts      (1001) docker     (123)      729 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/raw/checksums.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1110 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/raw/copystatus.py
--rw-r--r--   0 vsts      (1001) docker     (123)      684 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/raw/download.py
--rw-r--r--   0 vsts      (1001) docker     (123)      779 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/raw/stagingurls.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1596 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/raw/upload.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-25 12:34:07.024268 dhi-platform-1.0.7/src/dhi/platform/cli/rb/
--rw-r--r--   0 vsts      (1001) docker     (123)      937 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/rb/ls.py
--rw-r--r--   0 vsts      (1001) docker     (123)      934 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/rb/lsmy.py
--rw-r--r--   0 vsts      (1001) docker     (123)      562 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/rb/restore.py
--rw-r--r--   0 vsts      (1001) docker     (123)      559 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/rb/rmds.py
--rw-r--r--   0 vsts      (1001) docker     (123)      559 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/rb/rmprj.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-25 12:34:07.024268 dhi-platform-1.0.7/src/dhi/platform/cli/reader/
--rw-r--r--   0 vsts      (1001) docker     (123)      828 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/reader/info.py
--rw-r--r--   0 vsts      (1001) docker     (123)      817 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/reader/ls.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-25 12:34:07.024268 dhi-platform-1.0.7/src/dhi/platform/cli/tool/
--rw-r--r--   0 vsts      (1001) docker     (123)    26826 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/tool/openapi2py.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-25 12:34:07.024268 dhi-platform-1.0.7/src/dhi/platform/cli/tr/
--rw-r--r--   0 vsts      (1001) docker     (123)      997 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/tr/download.py
--rw-r--r--   0 vsts      (1001) docker     (123)      921 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/tr/info.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1153 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/tr/ls.py
--rw-r--r--   0 vsts      (1001) docker     (123)      959 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/tr/lss.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-25 12:34:07.024268 dhi-platform-1.0.7/src/dhi/platform/cli/ts/
--rw-r--r--   0 vsts      (1001) docker     (123)     1794 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/ts/add.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1572 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/ts/dscreate.py
--rw-r--r--   0 vsts      (1001) docker     (123)      736 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/ts/dsinfo.py
--rw-r--r--   0 vsts      (1001) docker     (123)      723 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/ts/info.py
--rw-r--r--   0 vsts      (1001) docker     (123)      686 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/ts/list.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-25 12:34:07.024268 dhi-platform-1.0.7/src/dhi/platform/cli/writer/
--rw-r--r--   0 vsts      (1001) docker     (123)      827 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/writer/info.py
--rw-r--r--   0 vsts      (1001) docker     (123)      817 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/cli/writer/ls.py
--rw-r--r--   0 vsts      (1001) docker     (123)    14844 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/commonmodels.py
--rw-r--r--   0 vsts      (1001) docker     (123)    10904 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/config.py
--rw-r--r--   0 vsts      (1001) docker     (123)    11456 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/engine.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3191 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/enginehelper.py
--rw-r--r--   0 vsts      (1001) docker     (123)    10421 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/eventing.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9459 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/eventinghelper.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7510 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/fmt.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-25 12:34:07.028268 dhi-platform-1.0.7/src/dhi/platform/generated/
--rw-r--r--   0 vsts      (1001) docker     (123)    30129 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/generated/enginegen.py
--rw-r--r--   0 vsts      (1001) docker     (123)    27842 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/generated/gisgen.py
--rw-r--r--   0 vsts      (1001) docker     (123)    33115 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/generated/jobgen.py
--rw-r--r--   0 vsts      (1001) docker     (123)   450751 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/generated/metadatagen.py
--rw-r--r--   0 vsts      (1001) docker     (123)   154021 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/generated/multidimensionalgen.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3921 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/generated/pubsubgen.py
--rw-r--r--   0 vsts      (1001) docker     (123)    27555 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/generated/rawgen.py
--rw-r--r--   0 vsts      (1001) docker     (123)    31866 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/generated/sharinggen.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9353 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/generated/tilesgen.py
--rw-r--r--   0 vsts      (1001) docker     (123)    83996 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/generated/timeseriesgen.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1468 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/gis.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8171 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/job.py
--rw-r--r--   0 vsts      (1001) docker     (123)    35673 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/metadata.py
--rw-r--r--   0 vsts      (1001) docker     (123)    11244 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/metadatahelper.py
--rw-r--r--   0 vsts      (1001) docker     (123)    18101 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/multidimensional.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-25 12:34:07.028268 dhi-platform-1.0.7/src/dhi/platform/protobufparser/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/protobufparser/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1722 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/protobufparser/api_implementation.py
--rw-r--r--   0 vsts      (1001) docker     (123)    21559 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/protobufparser/containers.py
--rw-r--r--   0 vsts      (1001) docker     (123)    40365 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/protobufparser/decoder.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2006 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/protobufparser/decoderdatetime.py
--rw-r--r--   0 vsts      (1001) docker     (123)    45172 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/protobufparser/descriptor.py
--rw-r--r--   0 vsts      (1001) docker     (123)    28682 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/protobufparser/encoder.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1941 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/protobufparser/enums.py
--rw-r--r--   0 vsts      (1001) docker     (123)    14452 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/protobufparser/message.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8492 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/protobufparser/wire_format.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1483 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/pubsub.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1469 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/raw.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2973 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/rawhelper.py
--rw-r--r--   0 vsts      (1001) docker     (123)    18696 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/sharing.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-25 12:34:07.028268 dhi-platform-1.0.7/src/dhi/platform/tests/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/tests/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-25 12:34:07.032268 dhi-platform-1.0.7/src/dhi/platform/tests/data/
--rw-r--r--   0 vsts      (1001) docker     (123)     2815 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/tests/data/EqD2.dfs2
--rw-r--r--   0 vsts      (1001) docker     (123)      122 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/tests/data/esbjergSmall.txt
--rw-r--r--   0 vsts      (1001) docker     (123)     5360 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/tests/engine_tests.py
--rw-r--r--   0 vsts      (1001) docker     (123)      687 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/tests/exceptions_test.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3778 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/tests/job_tests.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4103 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/tests/metadata_dataset_test.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8704 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/tests/metadata_project_test.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3724 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/tests/multidimensional_test.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3095 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/tests/sharing_test.py
--rw-r--r--   0 vsts      (1001) docker     (123)      510 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/tests/testcredentials.py
--rw-r--r--   0 vsts      (1001) docker     (123)    20051 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/tests/timeseries_test.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6803 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/tests/transfer_test.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7669 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/tests/transfer_tests_integration.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1691 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/tests/upload_download_test.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1478 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/tiles.py
--rw-r--r--   0 vsts      (1001) docker     (123)    21279 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/timeseries.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2676 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/timeserieshelper.py
--rw-r--r--   0 vsts      (1001) docker     (123)    89248 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/transfer.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2397 2023-04-25 12:33:47.000000 dhi-platform-1.0.7/src/dhi/platform/transferhelper.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-25 12:34:07.032268 dhi-platform-1.0.7/src/dhi_platform.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)     7342 2023-04-25 12:34:06.000000 dhi-platform-1.0.7/src/dhi_platform.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     5366 2023-04-25 12:34:07.000000 dhi-platform-1.0.7/src/dhi_platform.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-04-25 12:34:06.000000 dhi-platform-1.0.7/src/dhi_platform.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)      116 2023-04-25 12:34:06.000000 dhi-platform-1.0.7/src/dhi_platform.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        4 2023-04-25 12:34:06.000000 dhi-platform-1.0.7/src/dhi_platform.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-16 10:56:02.500579 dhi-platform-1.0.8/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1005 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (123)     7342 2023-05-16 10:56:02.500579 dhi-platform-1.0.8/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     6570 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-16 10:56:02.480579 dhi-platform-1.0.8/bin/
+-rw-r--r--   0 vsts      (1001) docker     (123)      905 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/bin/plt
+-rw-r--r--   0 vsts      (1001) docker     (123)     1245 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/bin/plt.bat
+-rw-r--r--   0 vsts      (1001) docker     (123)      103 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (123)     1293 2023-05-16 10:56:02.504579 dhi-platform-1.0.8/setup.cfg
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-16 10:56:02.480579 dhi-platform-1.0.8/src/
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-16 10:56:02.476579 dhi-platform-1.0.8/src/dhi/
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-16 10:56:02.484579 dhi-platform-1.0.8/src/dhi/platform/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)       18 2023-05-16 10:55:54.000000 dhi-platform-1.0.8/src/dhi/platform/_version.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    11926 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/args.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    12925 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/authentication.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-16 10:56:02.484579 dhi-platform-1.0.8/src/dhi/platform/base/
+-rw-r--r--   0 vsts      (1001) docker     (123)    18071 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/base/client.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1394 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/base/constants.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2144 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/base/exceptions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      667 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/base/utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-16 10:56:02.484579 dhi-platform-1.0.8/src/dhi/platform/cli/
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-16 10:56:02.484579 dhi-platform-1.0.8/src/dhi/platform/cli/cfg/
+-rw-r--r--   0 vsts      (1001) docker     (123)     4615 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/cli/cfg/login.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-16 10:56:02.488579 dhi-platform-1.0.8/src/dhi/platform/cli/ds/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1746 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/cli/ds/append.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2550 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/cli/ds/convert.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2196 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/cli/ds/cp.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2609 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/cli/ds/cpbh.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2914 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/cli/ds/cph.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1227 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/cli/ds/download.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1569 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/cli/ds/downloadc.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      831 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/cli/ds/info.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      855 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/cli/ds/infor.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      818 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/cli/ds/ls.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1138 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/cli/ds/lsh.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      728 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/cli/ds/lsra.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      560 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/cli/ds/restore.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      551 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/cli/ds/rm.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      557 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/cli/ds/rmhard.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1742 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/cli/ds/update.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2354 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/cli/ds/upload.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1883 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/cli/ds/uploadstaged.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-16 10:56:02.488579 dhi-platform-1.0.8/src/dhi/platform/cli/eng/
+-rw-r--r--   0 vsts      (1001) docker     (123)      596 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/cli/eng/cancel.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      689 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/cli/eng/configurations.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      755 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/cli/eng/diag.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      787 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/cli/eng/engine.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      645 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/cli/eng/engines.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      830 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/cli/eng/info.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      635 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/cli/eng/input.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1936 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/cli/eng/list.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2751 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/cli/eng/listmy.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      571 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/cli/eng/rm.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3076 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/cli/eng/run.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3092 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/cli/eng/runp.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2552 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/cli/eng/sbmessages.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-16 10:56:02.488579 dhi-platform-1.0.8/src/dhi/platform/cli/gw/
+-rw-r--r--   0 vsts      (1001) docker     (123)      740 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/cli/gw/service.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      611 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/cli/gw/services.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      366 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/cli/help.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-16 10:56:02.492579 dhi-platform-1.0.8/src/dhi/platform/cli/prj/
+-rw-r--r--   0 vsts      (1001) docker     (123)      822 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/cli/prj/capabilities.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1659 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/cli/prj/create.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1656 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/cli/prj/createsub.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      812 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/cli/prj/info.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      806 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/cli/prj/infor.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1496 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/cli/prj/ls.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      978 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/cli/prj/lsh.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      708 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/cli/prj/lsr.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      740 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/cli/prj/path.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1732 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/cli/prj/prepare.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      561 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/cli/prj/restore.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      552 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/cli/prj/rm.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      558 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/cli/prj/rmhard.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      567 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/cli/prj/sas.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1519 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/cli/prj/sub.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1637 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/cli/prj/update.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-16 10:56:02.492579 dhi-platform-1.0.8/src/dhi/platform/cli/prjm/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1054 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/cli/prjm/add.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      871 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/cli/prjm/all.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      667 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/cli/prjm/ls.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      741 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/cli/prjm/rm.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-16 10:56:02.492579 dhi-platform-1.0.8/src/dhi/platform/cli/raw/
+-rw-r--r--   0 vsts      (1001) docker     (123)      611 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/cli/raw/blocks.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      729 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/cli/raw/checksums.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1110 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/cli/raw/copystatus.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      684 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/cli/raw/download.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      779 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/cli/raw/stagingurls.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1596 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/cli/raw/upload.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-16 10:56:02.492579 dhi-platform-1.0.8/src/dhi/platform/cli/rb/
+-rw-r--r--   0 vsts      (1001) docker     (123)      937 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/cli/rb/ls.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      934 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/cli/rb/lsmy.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      562 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/cli/rb/restore.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      559 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/cli/rb/rmds.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      559 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/cli/rb/rmprj.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-16 10:56:02.492579 dhi-platform-1.0.8/src/dhi/platform/cli/reader/
+-rw-r--r--   0 vsts      (1001) docker     (123)      828 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/cli/reader/info.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      817 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/cli/reader/ls.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-16 10:56:02.492579 dhi-platform-1.0.8/src/dhi/platform/cli/tool/
+-rw-r--r--   0 vsts      (1001) docker     (123)    26826 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/cli/tool/openapi2py.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-16 10:56:02.492579 dhi-platform-1.0.8/src/dhi/platform/cli/tr/
+-rw-r--r--   0 vsts      (1001) docker     (123)      997 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/cli/tr/download.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      921 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/cli/tr/info.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1153 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/cli/tr/ls.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      959 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/cli/tr/lss.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-16 10:56:02.496579 dhi-platform-1.0.8/src/dhi/platform/cli/ts/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1794 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/cli/ts/add.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1572 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/cli/ts/dscreate.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      736 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/cli/ts/dsinfo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      723 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/cli/ts/info.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      686 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/cli/ts/list.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-16 10:56:02.496579 dhi-platform-1.0.8/src/dhi/platform/cli/writer/
+-rw-r--r--   0 vsts      (1001) docker     (123)      827 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/cli/writer/info.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      817 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/cli/writer/ls.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    14844 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/commonmodels.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    10904 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    11456 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/engine.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3191 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/enginehelper.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    10421 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/eventing.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9459 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/eventinghelper.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7510 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/fmt.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-16 10:56:02.496579 dhi-platform-1.0.8/src/dhi/platform/generated/
+-rw-r--r--   0 vsts      (1001) docker     (123)    30129 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/generated/enginegen.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    27842 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/generated/gisgen.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    33115 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/generated/jobgen.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   450751 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/generated/metadatagen.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   154021 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/generated/multidimensionalgen.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3921 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/generated/pubsubgen.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    27555 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/generated/rawgen.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    32006 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/generated/sharinggen.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9353 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/generated/tilesgen.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    83996 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/generated/timeseriesgen.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1468 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/gis.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8171 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/job.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    35673 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/metadata.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    11244 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/metadatahelper.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    18101 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/multidimensional.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-16 10:56:02.500579 dhi-platform-1.0.8/src/dhi/platform/protobufparser/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/protobufparser/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1722 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/protobufparser/api_implementation.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    21559 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/protobufparser/containers.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    40365 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/protobufparser/decoder.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2006 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/protobufparser/decoderdatetime.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    45172 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/protobufparser/descriptor.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    28682 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/protobufparser/encoder.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1941 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/protobufparser/enums.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    14452 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/protobufparser/message.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8492 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/protobufparser/wire_format.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1483 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/pubsub.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1469 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/raw.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2973 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/rawhelper.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    19727 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/sharing.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-16 10:56:02.500579 dhi-platform-1.0.8/src/dhi/platform/tests/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/tests/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-16 10:56:02.500579 dhi-platform-1.0.8/src/dhi/platform/tests/data/
+-rw-r--r--   0 vsts      (1001) docker     (123)     2815 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/tests/data/EqD2.dfs2
+-rw-r--r--   0 vsts      (1001) docker     (123)      122 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/tests/data/esbjergSmall.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)     5360 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/tests/engine_tests.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      687 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/tests/exceptions_test.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3778 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/tests/job_tests.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4103 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/tests/metadata_dataset_test.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8704 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/tests/metadata_project_test.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3724 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/tests/multidimensional_test.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3404 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/tests/sharing_test.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      510 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/tests/testcredentials.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    20051 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/tests/timeseries_test.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6803 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/tests/transfer_test.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7669 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/tests/transfer_tests_integration.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1691 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/tests/upload_download_test.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1478 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/tiles.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    21279 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/timeseries.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2676 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/timeserieshelper.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    89255 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/transfer.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2397 2023-05-16 10:55:44.000000 dhi-platform-1.0.8/src/dhi/platform/transferhelper.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-16 10:56:02.500579 dhi-platform-1.0.8/src/dhi_platform.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)     7342 2023-05-16 10:56:02.000000 dhi-platform-1.0.8/src/dhi_platform.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     5366 2023-05-16 10:56:02.000000 dhi-platform-1.0.8/src/dhi_platform.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-16 10:56:02.000000 dhi-platform-1.0.8/src/dhi_platform.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)      116 2023-05-16 10:56:02.000000 dhi-platform-1.0.8/src/dhi_platform.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        4 2023-05-16 10:56:02.000000 dhi-platform-1.0.8/src/dhi_platform.egg-info/top_level.txt
```

### Comparing `dhi-platform-1.0.7/LICENSE` & `dhi-platform-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/PKG-INFO` & `dhi-platform-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dhi-platform
-Version: 1.0.7
+Version: 1.0.8
 Summary: MIKE Cloud Platform SDK for Python
 Home-page: https://develop.mike-cloud.com/
 Author: DHI
 Author-email: wdpservice@dhigroup.com
 License: MIT License
 Project-URL: Open API, https://develop.mike-cloud.com/swagger/index.html
 Project-URL: Documentation, https://develop.mike-cloud.com/docs/
```

### Comparing `dhi-platform-1.0.7/README.md` & `dhi-platform-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/bin/plt` & `dhi-platform-1.0.8/bin/plt`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/bin/plt.bat` & `dhi-platform-1.0.8/bin/plt.bat`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/setup.cfg` & `dhi-platform-1.0.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/args.py` & `dhi-platform-1.0.8/src/dhi/platform/args.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/authentication.py` & `dhi-platform-1.0.8/src/dhi/platform/authentication.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/base/client.py` & `dhi-platform-1.0.8/src/dhi/platform/base/client.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/base/constants.py` & `dhi-platform-1.0.8/src/dhi/platform/base/constants.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/base/exceptions.py` & `dhi-platform-1.0.8/src/dhi/platform/base/exceptions.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/base/utils.py` & `dhi-platform-1.0.8/src/dhi/platform/base/utils.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/cli/cfg/login.py` & `dhi-platform-1.0.8/src/dhi/platform/cli/cfg/login.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/cli/ds/append.py` & `dhi-platform-1.0.8/src/dhi/platform/cli/ds/append.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/cli/ds/convert.py` & `dhi-platform-1.0.8/src/dhi/platform/cli/ds/convert.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/cli/ds/cp.py` & `dhi-platform-1.0.8/src/dhi/platform/cli/ds/cp.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/cli/ds/cpbh.py` & `dhi-platform-1.0.8/src/dhi/platform/cli/ds/cpbh.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/cli/ds/cph.py` & `dhi-platform-1.0.8/src/dhi/platform/cli/ds/cph.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/cli/ds/download.py` & `dhi-platform-1.0.8/src/dhi/platform/cli/ds/download.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/cli/ds/downloadc.py` & `dhi-platform-1.0.8/src/dhi/platform/cli/ds/downloadc.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/cli/ds/info.py` & `dhi-platform-1.0.8/src/dhi/platform/cli/ds/info.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/cli/ds/infor.py` & `dhi-platform-1.0.8/src/dhi/platform/cli/ds/infor.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/cli/ds/ls.py` & `dhi-platform-1.0.8/src/dhi/platform/cli/ds/ls.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/cli/ds/lsh.py` & `dhi-platform-1.0.8/src/dhi/platform/cli/ds/lsh.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/cli/ds/lsra.py` & `dhi-platform-1.0.8/src/dhi/platform/cli/ds/lsra.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/cli/ds/restore.py` & `dhi-platform-1.0.8/src/dhi/platform/cli/ds/restore.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/cli/ds/rm.py` & `dhi-platform-1.0.8/src/dhi/platform/cli/ds/rm.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/cli/ds/rmhard.py` & `dhi-platform-1.0.8/src/dhi/platform/cli/ds/rmhard.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/cli/ds/update.py` & `dhi-platform-1.0.8/src/dhi/platform/cli/ds/update.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/cli/ds/upload.py` & `dhi-platform-1.0.8/src/dhi/platform/cli/ds/upload.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/cli/ds/uploadstaged.py` & `dhi-platform-1.0.8/src/dhi/platform/cli/ds/uploadstaged.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/cli/eng/cancel.py` & `dhi-platform-1.0.8/src/dhi/platform/cli/eng/cancel.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/cli/eng/configurations.py` & `dhi-platform-1.0.8/src/dhi/platform/cli/eng/configurations.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/cli/eng/diag.py` & `dhi-platform-1.0.8/src/dhi/platform/cli/eng/diag.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/cli/eng/engine.py` & `dhi-platform-1.0.8/src/dhi/platform/cli/eng/engine.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/cli/eng/engines.py` & `dhi-platform-1.0.8/src/dhi/platform/cli/eng/engines.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/cli/eng/info.py` & `dhi-platform-1.0.8/src/dhi/platform/cli/eng/info.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/cli/eng/input.py` & `dhi-platform-1.0.8/src/dhi/platform/cli/eng/input.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/cli/eng/list.py` & `dhi-platform-1.0.8/src/dhi/platform/cli/eng/list.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/cli/eng/listmy.py` & `dhi-platform-1.0.8/src/dhi/platform/cli/eng/listmy.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/cli/eng/rm.py` & `dhi-platform-1.0.8/src/dhi/platform/cli/eng/rm.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/cli/eng/run.py` & `dhi-platform-1.0.8/src/dhi/platform/cli/eng/run.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/cli/eng/runp.py` & `dhi-platform-1.0.8/src/dhi/platform/cli/eng/runp.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/cli/eng/sbmessages.py` & `dhi-platform-1.0.8/src/dhi/platform/cli/eng/sbmessages.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/cli/gw/service.py` & `dhi-platform-1.0.8/src/dhi/platform/cli/gw/service.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/cli/gw/services.py` & `dhi-platform-1.0.8/src/dhi/platform/cli/gw/services.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/cli/prj/capabilities.py` & `dhi-platform-1.0.8/src/dhi/platform/cli/prj/capabilities.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/cli/prj/create.py` & `dhi-platform-1.0.8/src/dhi/platform/cli/prj/create.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/cli/prj/createsub.py` & `dhi-platform-1.0.8/src/dhi/platform/cli/prj/createsub.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/cli/prj/info.py` & `dhi-platform-1.0.8/src/dhi/platform/cli/prj/info.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/cli/prj/infor.py` & `dhi-platform-1.0.8/src/dhi/platform/cli/prj/infor.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/cli/prj/ls.py` & `dhi-platform-1.0.8/src/dhi/platform/cli/prj/ls.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/cli/prj/lsh.py` & `dhi-platform-1.0.8/src/dhi/platform/cli/prj/lsh.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/cli/prj/lsr.py` & `dhi-platform-1.0.8/src/dhi/platform/cli/prj/lsr.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/cli/prj/path.py` & `dhi-platform-1.0.8/src/dhi/platform/cli/prj/path.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/cli/prj/prepare.py` & `dhi-platform-1.0.8/src/dhi/platform/cli/prj/prepare.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/cli/prj/restore.py` & `dhi-platform-1.0.8/src/dhi/platform/cli/prj/restore.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/cli/prj/rm.py` & `dhi-platform-1.0.8/src/dhi/platform/cli/prj/rm.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/cli/prj/rmhard.py` & `dhi-platform-1.0.8/src/dhi/platform/cli/prj/rmhard.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/cli/prj/sas.py` & `dhi-platform-1.0.8/src/dhi/platform/cli/prj/sas.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/cli/prj/sub.py` & `dhi-platform-1.0.8/src/dhi/platform/cli/prj/sub.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/cli/prj/update.py` & `dhi-platform-1.0.8/src/dhi/platform/cli/prj/update.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/cli/prjm/add.py` & `dhi-platform-1.0.8/src/dhi/platform/cli/prjm/add.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/cli/prjm/all.py` & `dhi-platform-1.0.8/src/dhi/platform/cli/prjm/all.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/cli/prjm/ls.py` & `dhi-platform-1.0.8/src/dhi/platform/cli/prjm/ls.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/cli/prjm/rm.py` & `dhi-platform-1.0.8/src/dhi/platform/cli/prjm/rm.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/cli/raw/blocks.py` & `dhi-platform-1.0.8/src/dhi/platform/cli/raw/blocks.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/cli/raw/checksums.py` & `dhi-platform-1.0.8/src/dhi/platform/cli/raw/checksums.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/cli/raw/copystatus.py` & `dhi-platform-1.0.8/src/dhi/platform/cli/raw/copystatus.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/cli/raw/download.py` & `dhi-platform-1.0.8/src/dhi/platform/cli/raw/download.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/cli/raw/stagingurls.py` & `dhi-platform-1.0.8/src/dhi/platform/cli/raw/stagingurls.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/cli/raw/upload.py` & `dhi-platform-1.0.8/src/dhi/platform/cli/raw/upload.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/cli/rb/ls.py` & `dhi-platform-1.0.8/src/dhi/platform/cli/rb/ls.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/cli/rb/lsmy.py` & `dhi-platform-1.0.8/src/dhi/platform/cli/rb/lsmy.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/cli/rb/restore.py` & `dhi-platform-1.0.8/src/dhi/platform/cli/rb/restore.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/cli/rb/rmds.py` & `dhi-platform-1.0.8/src/dhi/platform/cli/rb/rmds.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/cli/rb/rmprj.py` & `dhi-platform-1.0.8/src/dhi/platform/cli/rb/rmprj.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/cli/reader/info.py` & `dhi-platform-1.0.8/src/dhi/platform/cli/reader/info.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/cli/reader/ls.py` & `dhi-platform-1.0.8/src/dhi/platform/cli/reader/ls.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/cli/tool/openapi2py.py` & `dhi-platform-1.0.8/src/dhi/platform/cli/tool/openapi2py.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/cli/tr/download.py` & `dhi-platform-1.0.8/src/dhi/platform/cli/tr/download.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/cli/tr/info.py` & `dhi-platform-1.0.8/src/dhi/platform/cli/tr/info.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/cli/tr/ls.py` & `dhi-platform-1.0.8/src/dhi/platform/cli/tr/ls.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/cli/tr/lss.py` & `dhi-platform-1.0.8/src/dhi/platform/cli/tr/lss.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/cli/ts/add.py` & `dhi-platform-1.0.8/src/dhi/platform/cli/ts/add.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/cli/ts/dscreate.py` & `dhi-platform-1.0.8/src/dhi/platform/cli/ts/dscreate.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/cli/ts/dsinfo.py` & `dhi-platform-1.0.8/src/dhi/platform/cli/ts/dsinfo.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/cli/ts/info.py` & `dhi-platform-1.0.8/src/dhi/platform/cli/ts/info.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/cli/ts/list.py` & `dhi-platform-1.0.8/src/dhi/platform/cli/ts/list.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/cli/writer/info.py` & `dhi-platform-1.0.8/src/dhi/platform/cli/writer/info.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/cli/writer/ls.py` & `dhi-platform-1.0.8/src/dhi/platform/cli/writer/ls.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/commonmodels.py` & `dhi-platform-1.0.8/src/dhi/platform/commonmodels.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/config.py` & `dhi-platform-1.0.8/src/dhi/platform/config.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/engine.py` & `dhi-platform-1.0.8/src/dhi/platform/engine.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/enginehelper.py` & `dhi-platform-1.0.8/src/dhi/platform/enginehelper.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/eventing.py` & `dhi-platform-1.0.8/src/dhi/platform/eventing.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/eventinghelper.py` & `dhi-platform-1.0.8/src/dhi/platform/eventinghelper.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/fmt.py` & `dhi-platform-1.0.8/src/dhi/platform/fmt.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/generated/enginegen.py` & `dhi-platform-1.0.8/src/dhi/platform/generated/enginegen.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/generated/gisgen.py` & `dhi-platform-1.0.8/src/dhi/platform/generated/gisgen.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/generated/jobgen.py` & `dhi-platform-1.0.8/src/dhi/platform/generated/jobgen.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/generated/metadatagen.py` & `dhi-platform-1.0.8/src/dhi/platform/generated/metadatagen.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/generated/multidimensionalgen.py` & `dhi-platform-1.0.8/src/dhi/platform/generated/multidimensionalgen.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/generated/pubsubgen.py` & `dhi-platform-1.0.8/src/dhi/platform/generated/pubsubgen.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/generated/rawgen.py` & `dhi-platform-1.0.8/src/dhi/platform/generated/rawgen.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/generated/sharinggen.py` & `dhi-platform-1.0.8/src/dhi/platform/generated/sharinggen.py`

 * *Files 0% similar despite different names*

```diff
@@ -759,52 +759,54 @@
         return self.GetRequest("/api/sharing/catalog/list", queryparams, api_version="1", projectid=projectid)
 
     def CreatePublication(self, projectid, body) -> Response:
         """Publication
 
         POST /api/sharing/publication
         """
-        return self.PostRequest("/api/sharing/publication", body, None, api_version="1", projectid=projectid)
+        resource_id = body.get('resourceId', None)
+        return self.PostRequest("/api/sharing/publication", body, None, api_version="1", projectid=projectid, datasetid=resource_id)
 
     def UpdatePublication(self, projectid, body) -> Response:
         """Publication
 
         PUT /api/sharing/publication
         """
-        return self.PutRequest("/api/sharing/publication", body, None, api_version="1", projectid=projectid)
+        resource_id = body.get('resourceId', None)
+        return self.PutRequest("/api/sharing/publication", body, None, api_version="1", projectid=projectid, datasetid=resource_id)
 
     def GetPublicationList(self, projectid, resourceid=None, catalogid=None, sortby=None, sortorder=None, cursor=None, limit=None) -> Response:
         """Publication
 
         GET /api/sharing/publication/list
         """
         queryparams = self.GetQueryParams(ResourceId=resourceid, CatalogId=catalogid, SortBy=sortby, SortOrder=sortorder, Cursor=cursor, Limit=limit)
         return self.GetRequest("/api/sharing/publication/list", queryparams, api_version="1", projectid=projectid)
 
-    def DeletePublication(self, projectid, id) -> Response:
+    def DeletePublication(self, projectid, id, resourceid) -> Response:
         """Publication
 
         DELETE /api/sharing/publication/{id}
         """
-        return self.DeleteRequest(f"/api/sharing/publication/{id}", None, api_version="1", projectid=projectid, datasetid=id)
+        return self.DeleteRequest(f"/api/sharing/publication/{id}", None, api_version="1", projectid=projectid, datasetid=resourceid)
 
     def GetPublication(self, projectid, id) -> Response:
         """Publication
 
         GET /api/sharing/publication/{id}
         """
-        return self.GetRequest(f"/api/sharing/publication/{id}", None, api_version="1", projectid=projectid, datasetid=id)
+        return self.GetRequest(f"/api/sharing/publication/{id}", None, api_version="1", projectid=projectid)
 
     def GetPublicationSubscriptionList(self, projectid, id, sortby=None, sortorder=None, cursor=None, limit=None) -> Response:
         """Publication
 
         GET /api/sharing/publication/{id}/subscription/list
         """
         queryparams = self.GetQueryParams(SortBy=sortby, SortOrder=sortorder, Cursor=cursor, Limit=limit)
-        return self.GetRequest(f"/api/sharing/publication/{id}/subscription/list", queryparams, api_version="1", projectid=projectid, datasetid=id)
+        return self.GetRequest(f"/api/sharing/publication/{id}/subscription/list", queryparams, api_version="1", projectid=projectid)
 
     def GetResourceDetail(self, projectid, subscriptionid) -> Response:
         """Publication
 
         GET /api/sharing/publication/{subscriptionId}/resourcedetail
         """
         return self.GetRequest(f"/api/sharing/publication/{subscriptionid}/resourcedetail", None, api_version="1", projectid=projectid)
```

### Comparing `dhi-platform-1.0.7/src/dhi/platform/generated/tilesgen.py` & `dhi-platform-1.0.8/src/dhi/platform/generated/tilesgen.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/generated/timeseriesgen.py` & `dhi-platform-1.0.8/src/dhi/platform/generated/timeseriesgen.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/gis.py` & `dhi-platform-1.0.8/src/dhi/platform/gis.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/job.py` & `dhi-platform-1.0.8/src/dhi/platform/job.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/metadata.py` & `dhi-platform-1.0.8/src/dhi/platform/metadata.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/metadatahelper.py` & `dhi-platform-1.0.8/src/dhi/platform/metadatahelper.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/multidimensional.py` & `dhi-platform-1.0.8/src/dhi/platform/multidimensional.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/protobufparser/api_implementation.py` & `dhi-platform-1.0.8/src/dhi/platform/protobufparser/api_implementation.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/protobufparser/containers.py` & `dhi-platform-1.0.8/src/dhi/platform/protobufparser/containers.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/protobufparser/decoder.py` & `dhi-platform-1.0.8/src/dhi/platform/protobufparser/decoder.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/protobufparser/decoderdatetime.py` & `dhi-platform-1.0.8/src/dhi/platform/protobufparser/decoderdatetime.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/protobufparser/descriptor.py` & `dhi-platform-1.0.8/src/dhi/platform/protobufparser/descriptor.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/protobufparser/encoder.py` & `dhi-platform-1.0.8/src/dhi/platform/protobufparser/encoder.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/protobufparser/enums.py` & `dhi-platform-1.0.8/src/dhi/platform/protobufparser/enums.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/protobufparser/message.py` & `dhi-platform-1.0.8/src/dhi/platform/protobufparser/message.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/protobufparser/wire_format.py` & `dhi-platform-1.0.8/src/dhi/platform/protobufparser/wire_format.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/pubsub.py` & `dhi-platform-1.0.8/src/dhi/platform/pubsub.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/raw.py` & `dhi-platform-1.0.8/src/dhi/platform/raw.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/rawhelper.py` & `dhi-platform-1.0.8/src/dhi/platform/rawhelper.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/sharing.py` & `dhi-platform-1.0.8/src/dhi/platform/sharing.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,14 +38,25 @@
             'IntraTenant': self.INTRA_TENANT,
             'Public': self.PUBLIC,
         }
         if catalog_type in options:
             return options[catalog_type]
         else:
             raise MikeCloudException("Invalid catalog type", catalog_type)
+        
+    @property
+    def name(self):
+        options = {
+            'INTRA_TENANT': 'IntraTenant',
+            'PUBLIC': 'Public',
+        }
+        if self._name_ in options:
+            return options[self._name_]
+        else:
+            raise MikeCloudException("Invalid catalog type", self._name_)
 
 
 class SubscriptionMode(Enum):
     OPEN = 100
     ON_APPROVAL = 200
 
     @classmethod
@@ -54,14 +65,25 @@
             'Open': self.OPEN,
             'OnApproval': self.ON_APPROVAL,
         }
         if mode in options:
             return options[mode]
         else:
             raise MikeCloudException("Invalid subscription mode", mode)
+    
+    @property
+    def name(self):
+        options = {
+            'OPEN': 'Open',
+            'ON_APPROVAL': 'OnApproval'
+        }
+        if self._name_ in options:
+            return options[self._name_]
+        else:
+            raise MikeCloudException("Invalid subscription mode", self._name_)
 
 
 class PublicationResourceType(Enum):
     DATASET = 100
     FOLDER = 200
 
     @classmethod
@@ -101,24 +123,24 @@
         self._id = id
         self._created_at = created_at
         self._created_by = created_by
         self._updated_at = updated_at
         self._updated_by = updated_by
         self._deleted_at = deleted_at
         self._deleted_by = deleted_by
-        self._name = name,
-        self._description = description,
-        self._location = location,
-        self._metadata = metadata,
-        self._properties = properties,
-        self._resource_id = resource_id,
-        self._resource_type = resource_type,
-        self._discoverable = discoverable,
-        self._subscription_mode = subscription_mode,
-        self._published_until = published_until,
+        self._name = name
+        self._description = description
+        self._location = location
+        self._metadata = metadata
+        self._properties = properties
+        self._resource_id = resource_id
+        self._resource_type = resource_type
+        self._discoverable = discoverable
+        self._subscription_mode = subscription_mode
+        self._published_until = published_until
         self._row_version = row_version
 
     @property
     def id(self):
         return self._id
 
     @property
@@ -191,19 +213,20 @@
         deleted_at = None if body.get("deletedAt", None) is None else datetime.datetime.strptime(body["deletedAt"][:26], constants.DATETIMEFORMAT)
         published_until = None if body.get("publishedUntil", None) is None else datetime.datetime.strptime(body["publishedUntil"][:26], constants.DATETIMEFORMAT)
         return cls(
             id = body["id"],
             created_at = datetime.datetime.strptime(body["createdAt"][:26], constants.DATETIMEFORMAT),
             created_by = body["createdBy"],
             updated_at = updated_at,
-            updated_by = body["updatedBy"],
+            updated_by = body.get("updatedBy", None),
             deleted_at = deleted_at,
-            deleted_by = None if "deletedBy" not in body else body["deletedBy"],
+            deleted_by = body.get("deletedBy", None),
             name = body["name"],
-            description = None if "description" not in body else body["description"],
+            description = body.get("description", None),
+            location = body.get("location", None),
             metadata = body["metadata"],
             properties = body["properties"],
             resource_id = body["resourceId"],
             resource_type = PublicationResourceType.from_string(body["resourceType"]),
             subscription_mode = SubscriptionMode.from_string(body["subscriptionMode"]),
             discoverable = body["discoverable"],
             published_until = published_until,
@@ -283,21 +306,21 @@
             body["metadata"] = self._metadata
         if self._properties is not None:
             body["properties"] = self._properties
         if self._resource_id is not None:
             body["resourceId"] = self._resource_id
         if self._location is not None:
             body["location"] = self._location
-
         return body
 
 
 class CreatePublicationInput:
-    def __init__(self, name: str, resource_id:str, description: str = None, metadata: dict = {}, subscription_mode:SubscriptionMode = SubscriptionMode.OPEN, discoverable=True, resource_type:PublicationResourceType=PublicationResourceType.DATASET, published_until:datetime.datetime=None):
+    def __init__(self, name: str, catalog_id:str, resource_id:str, description: str = None, metadata: dict = {}, subscription_mode:SubscriptionMode = SubscriptionMode.OPEN, discoverable=True, resource_type:PublicationResourceType=PublicationResourceType.DATASET, published_until:datetime.datetime=None):
         self._name = name
+        self._catalog_id = catalog_id
         self._resource_id = resource_id
         self._description = "" if description is None else description
         self._subscription_mode = subscription_mode
         self._discoverable = discoverable
         self._resource_type = resource_type
         self._published_until = published_until
         self._metadata = metadata
@@ -308,14 +331,22 @@
         return self._name
 
     @name.setter
     def name(self, name):
         self._name = name
 
     @property 
+    def catalog_id(self) -> str:
+        return self._catalog_id
+
+    @catalog_id.setter
+    def catalog_id(self, catalog_id):
+        self._catalog_id = catalog_id
+
+    @property 
     def resource_id(self) -> str:
         return self._resource_id
 
     @resource_id.setter
     def resource_id(self, resource_id):
         self._resource_id = resource_id
     
@@ -357,30 +388,30 @@
     @published_until.setter
     def published_until(self, published_until):
         self._published_until = published_until
 
     def body(self):
         body = {
             "name": self._name,
+            "catalogId": self._catalog_id,
             "resourceId": self._resource_id,
             "description": self._description,
-            "subspcriptionMode": self._subscription_mode,
+            "subspcriptionMode": self._subscription_mode.name,
             "discoverable": self._discoverable,
-            "resourceType": self._resource_type
+            "resourceType": self._resource_type.name.title()
         }
 
         if self._metadata:
             body["metadata"] = self._metadata
 
         if self._properties:
             body["properties"] = self._properties
 
         if self._published_until is not None:
             body["publishedUntil"] = self._published_until.strftime(constants.DATETIMEFORMAT)
-        
         return body
 
 
 class CatalogOutput:
     def __init__(
         self,
         id: str,
@@ -428,17 +459,17 @@
         updated_at = None if body.get("updatedAt", None) is None else datetime.datetime.strptime(body["updatedAt"][:26], constants.DATETIMEFORMAT)
         deleted_at = None if body.get("deletedAt", None) is None else datetime.datetime.strptime(body["deletedAt"][:26], constants.DATETIMEFORMAT)
         return cls(
             id = body["id"],
             created_at = datetime.datetime.strptime(body["createdAt"][:26], constants.DATETIMEFORMAT),
             created_by = body["createdBy"],
             updated_at = updated_at,
-            updated_by = body["updatedBy"],
+            updated_by = body.get("updatedBy", None),
             deleted_at = deleted_at,
-            deleted_by = None if "deletedBy" not in body else body["deletedBy"],
+            deleted_by = body.get("deletedBy", None),
             name = body["name"],
             catalog_type = CatalogType.from_string(body["catalogType"])
         )
 
 
 class CreateCatalogInput:
     def __init__(self, name: str, catalog_type:CatalogType = CatalogType.PUBLIC):
@@ -460,15 +491,15 @@
     @catalog_type.setter
     def catalog_type(self, catalog_type:CatalogType):
         self._catalog_type = catalog_type
 
     def body(self):
         return {
             "name": self._name,
-            "catalogType": self._catalog_type
+            "catalogType": self._catalog_type.name
         }
 
 
 class SharingClientV1(SharingGenClientV1):
     def __init__(self, inspectFnc=SharingGenClientV1.DefaultInspectFnc, **kwargs):
         super().__init__(inspectFnc, **kwargs)
 
@@ -529,24 +560,25 @@
         :param input: EditPublicationInput instance defining the new properties of the publication
         :return: updated publication details
         :rtype: PublicationOutput
         """
         response = self._client1.UpdatePublication(project_id, input.body())
         return PublicationOutput.from_body(response.Body)
 
-    def delete_publication(self, project_id, publication_id) -> bool:
+    def delete_publication(self, project_id, publication_id, resource_id) -> bool:
         """
         Delete publication, the publication is deleted permanently
         
         :param project_id: Project ID of the publication
         :param publication_id: ID of the publication
+        :param resource_id: ID of the project or dataset the publication refers to, needed for authorization evaluation
         :return: True if the request was successful, raises otherwise
         :rtype: bool
         """
-        response = self._client1.DeletePublication(project_id, publication_id)
+        response = self._client1.DeletePublication(project_id, publication_id, resource_id)
         return response.IsOk
     
     def create_catalog(self, project_id, input:CreateCatalogInput) -> str:
         """
         Create catalog
         
         :param project_id: ID of the project where the catalog should reside in
```

### Comparing `dhi-platform-1.0.7/src/dhi/platform/tests/data/EqD2.dfs2` & `dhi-platform-1.0.8/src/dhi/platform/tests/data/EqD2.dfs2`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/tests/engine_tests.py` & `dhi-platform-1.0.8/src/dhi/platform/tests/engine_tests.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/tests/exceptions_test.py` & `dhi-platform-1.0.8/src/dhi/platform/tests/exceptions_test.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/tests/job_tests.py` & `dhi-platform-1.0.8/src/dhi/platform/tests/job_tests.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/tests/metadata_dataset_test.py` & `dhi-platform-1.0.8/src/dhi/platform/tests/metadata_dataset_test.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/tests/metadata_project_test.py` & `dhi-platform-1.0.8/src/dhi/platform/tests/metadata_project_test.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/tests/multidimensional_test.py` & `dhi-platform-1.0.8/src/dhi/platform/tests/multidimensional_test.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/tests/sharing_test.py` & `dhi-platform-1.0.8/src/dhi/platform/tests/sharing_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,38 +35,41 @@
         dataset = self._timeseriesclient.create_timeseries_dataset_from_schema(project_id, name, description)
         return dataset.id
 
     def skip_test_create_update_delete_publication_is_ok(self):
         project = self._create_project()
         self._projects_to_delete.append(project.id)
 
+        t = datetime.datetime.now().strftime('%Y%m%d%H%M%S')
         ds_name = "Py TS"
         ds_description = "Test TS dataset"
         dataset_id = self._create_ts_dataset(project.id, ds_name, ds_description)
 
         dataset = self._metadataclient.get_dataset(dataset_id)
         self.assertIsNotNone(dataset)
 
-        catalog_id = self._sharingclient.create_catalog(project.id, sharing.CreateCatalogInput("Pytest catalog"))
+        tenant_id = '980552ba-58a1-4742-9248-cbcf3b3a4ece' # dhi1 in DEV0
+        #catalog_id = self._sharingclient.create_catalog(tenant_id, sharing.CreateCatalogInput(f"Pytest test catalog {t}"))
+        catalog_id = '70e9d380-9ac5-4d1e-a3e2-8fd00e715da6' # FIKR's catalog in DEV0
 
         catalogs = list(self._sharingclient.list_catalogs(project.id))
 
         self.assertTrue(len(catalogs) > 0)
 
-        publication_id = self._sharingclient.create_publication(project.id, sharing.CreatePublicationInput("PyTest", dataset.id, "Pytest publication", {"foo", "bar"}))
+        publication_id = self._sharingclient.create_publication(project.id, sharing.CreatePublicationInput(f"PyTest {t}", catalog_id, dataset.id, "Pytest publication", {"foo": "bar"}))
 
         publication = self._sharingclient.get_publication(project.id, publication_id)
 
-        publication_updated = self._sharingclient.update_publication(project.id, sharing.EditPublicationInput(publication_id, publication.name, publication.resource_id, metadata = {"foo": "spam", "eggs": 1}))
+        publication_updated = self._sharingclient.update_publication(project.id, sharing.EditPublicationInput(publication_id, publication.name, publication.resource_id, metadata = {"foo": "spam", "eggs": 1}, row_version=publication.row_version))
 
         self.assertEqual(publication_updated.name, publication.name)
         self.assertEqual(publication_updated.metadata["foo"], "spam")
         self.assertEqual(publication_updated.metadata["eggs"], 1)
 
-        self._sharingclient.delete_publication(project.id, publication_id)
+        self._sharingclient.delete_publication(project.id, publication_id, publication.resource_id)
 
         deleted = self._metadataclient.delete_dataset(dataset_id, permanently=True)
         self.assertTrue(deleted)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `dhi-platform-1.0.7/src/dhi/platform/tests/timeseries_test.py` & `dhi-platform-1.0.8/src/dhi/platform/tests/timeseries_test.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/tests/transfer_test.py` & `dhi-platform-1.0.8/src/dhi/platform/tests/transfer_test.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/tests/transfer_tests_integration.py` & `dhi-platform-1.0.8/src/dhi/platform/tests/transfer_tests_integration.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/tests/upload_download_test.py` & `dhi-platform-1.0.8/src/dhi/platform/tests/upload_download_test.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/tiles.py` & `dhi-platform-1.0.8/src/dhi/platform/tiles.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/timeseries.py` & `dhi-platform-1.0.8/src/dhi/platform/timeseries.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/timeserieshelper.py` & `dhi-platform-1.0.8/src/dhi/platform/timeserieshelper.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi/platform/transfer.py` & `dhi-platform-1.0.8/src/dhi/platform/transfer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1322,15 +1322,15 @@
             "originalFileName": self._original_file_name,
             "uploadUrl": self._upload_url,
             "readerName": self._reader_name,
             "writerName": self._writer_name
         }
         
         if self._transformations:
-            body["transformations"] = [t for t in self._transformations]
+            body["transformations"] = [t.body() for t in self._transformations]
 
         if self._reader_parameters:
             body["readerParameters"] = [{"name": p[0], "value": p[1]} for p in self._reader_parameters]
         
         if self._writer_parameters:
             body["writerParameters"] = [{"name": p[0], "value": p[1]} for p in self._writer_parameters]
```

### Comparing `dhi-platform-1.0.7/src/dhi/platform/transferhelper.py` & `dhi-platform-1.0.8/src/dhi/platform/transferhelper.py`

 * *Files identical despite different names*

### Comparing `dhi-platform-1.0.7/src/dhi_platform.egg-info/PKG-INFO` & `dhi-platform-1.0.8/src/dhi_platform.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dhi-platform
-Version: 1.0.7
+Version: 1.0.8
 Summary: MIKE Cloud Platform SDK for Python
 Home-page: https://develop.mike-cloud.com/
 Author: DHI
 Author-email: wdpservice@dhigroup.com
 License: MIT License
 Project-URL: Open API, https://develop.mike-cloud.com/swagger/index.html
 Project-URL: Documentation, https://develop.mike-cloud.com/docs/
```

### Comparing `dhi-platform-1.0.7/src/dhi_platform.egg-info/SOURCES.txt` & `dhi-platform-1.0.8/src/dhi_platform.egg-info/SOURCES.txt`

 * *Files identical despite different names*

