# Comparing `tmp/opencivicdata-3.2.0.tar.gz` & `tmp/opencivicdata-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/opencivicdata-3.2.0.tar", last modified: Thu Mar 26 18:54:08 2020, max compression
+gzip compressed data, was "opencivicdata-3.3.0.tar", last modified: Tue May 16 15:59:36 2023, max compression
```

## Comparing `opencivicdata-3.2.0.tar` & `opencivicdata-3.3.0.tar`

### file list

```diff
@@ -1,114 +1,120 @@
-drwxr-xr-x   0 james      (502) staff       (20)        0 2020-03-26 18:54:08.000000 opencivicdata-3.2.0/
--rw-r--r--   0 james      (502) staff       (20)      105 2019-10-08 14:14:14.000000 opencivicdata-3.2.0/MANIFEST.in
--rw-r--r--   0 james      (502) staff       (20)      624 2020-03-26 18:54:08.000000 opencivicdata-3.2.0/PKG-INFO
--rw-r--r--   0 james      (502) staff       (20)      851 2019-11-25 15:11:24.000000 opencivicdata-3.2.0/README.md
-drwxr-xr-x   0 james      (502) staff       (20)        0 2020-03-26 18:54:08.000000 opencivicdata-3.2.0/opencivicdata/
--rw-r--r--   0 james      (502) staff       (20)        0 2019-10-08 14:14:14.000000 opencivicdata-3.2.0/opencivicdata/__init__.py
--rw-r--r--   0 james      (502) staff       (20)     6495 2020-03-26 18:50:45.000000 opencivicdata-3.2.0/opencivicdata/common.py
-drwxr-xr-x   0 james      (502) staff       (20)        0 2020-03-26 18:54:08.000000 opencivicdata-3.2.0/opencivicdata/core/
--rw-r--r--   0 james      (502) staff       (20)        0 2019-10-08 14:14:14.000000 opencivicdata-3.2.0/opencivicdata/core/__init__.py
-drwxr-xr-x   0 james      (502) staff       (20)        0 2020-03-26 18:54:08.000000 opencivicdata-3.2.0/opencivicdata/core/admin/
--rw-r--r--   0 james      (502) staff       (20)       50 2019-11-25 15:12:54.000000 opencivicdata-3.2.0/opencivicdata/core/admin/__init__.py
--rw-r--r--   0 james      (502) staff       (20)     1599 2019-11-25 15:12:54.000000 opencivicdata-3.2.0/opencivicdata/core/admin/base.py
--rw-r--r--   0 james      (502) staff       (20)     2888 2019-11-25 15:12:54.000000 opencivicdata-3.2.0/opencivicdata/core/admin/organization.py
--rw-r--r--   0 james      (502) staff       (20)     1918 2019-11-25 15:12:54.000000 opencivicdata-3.2.0/opencivicdata/core/admin/other.py
--rw-r--r--   0 james      (502) staff       (20)     2689 2019-11-25 15:12:54.000000 opencivicdata-3.2.0/opencivicdata/core/admin/person.py
--rw-r--r--   0 james      (502) staff       (20)      188 2019-11-25 15:12:54.000000 opencivicdata-3.2.0/opencivicdata/core/apps.py
-drwxr-xr-x   0 james      (502) staff       (20)        0 2020-03-26 18:54:08.000000 opencivicdata-3.2.0/opencivicdata/core/management/
--rw-r--r--   0 james      (502) staff       (20)        0 2019-10-08 14:14:14.000000 opencivicdata-3.2.0/opencivicdata/core/management/__init__.py
-drwxr-xr-x   0 james      (502) staff       (20)        0 2020-03-26 18:54:08.000000 opencivicdata-3.2.0/opencivicdata/core/management/commands/
--rw-r--r--   0 james      (502) staff       (20)        0 2019-10-08 14:14:14.000000 opencivicdata-3.2.0/opencivicdata/core/management/commands/__init__.py
--rw-r--r--   0 james      (502) staff       (20)     2418 2019-11-25 15:12:54.000000 opencivicdata-3.2.0/opencivicdata/core/management/commands/loaddivisions.py
-drwxr-xr-x   0 james      (502) staff       (20)        0 2020-03-26 18:54:08.000000 opencivicdata-3.2.0/opencivicdata/core/migrations/
--rw-r--r--   0 james      (502) staff       (20)    33323 2019-11-25 15:12:56.000000 opencivicdata-3.2.0/opencivicdata/core/migrations/0001_initial.py
--rw-r--r--   0 james      (502) staff       (20)      437 2019-11-25 15:12:54.000000 opencivicdata-3.2.0/opencivicdata/core/migrations/0002_post_maximum_memberships.py
--rw-r--r--   0 james      (502) staff       (20)    41402 2019-11-25 15:12:56.000000 opencivicdata-3.2.0/opencivicdata/core/migrations/0003_field_docs.py
--rw-r--r--   0 james      (502) staff       (20)     3545 2019-11-25 15:12:54.000000 opencivicdata-3.2.0/opencivicdata/core/migrations/0004_auto_20171005_2028.py
--rw-r--r--   0 james      (502) staff       (20)      779 2020-03-26 04:58:36.000000 opencivicdata-3.2.0/opencivicdata/core/migrations/0005_auto_20191031_1507.py
--rw-r--r--   0 james      (502) staff       (20)     1081 2019-11-25 15:12:54.000000 opencivicdata-3.2.0/opencivicdata/core/migrations/0005_auto_20191124_1658.py
--rw-r--r--   0 james      (502) staff       (20)      267 2020-03-26 04:58:36.000000 opencivicdata-3.2.0/opencivicdata/core/migrations/0006_merge_20200103_1432.py
--rw-r--r--   0 james      (502) staff       (20)        0 2019-10-08 14:14:14.000000 opencivicdata-3.2.0/opencivicdata/core/migrations/__init__.py
-drwxr-xr-x   0 james      (502) staff       (20)        0 2020-03-26 18:54:08.000000 opencivicdata-3.2.0/opencivicdata/core/models/
--rw-r--r--   0 james      (502) staff       (20)      480 2019-11-25 15:12:54.000000 opencivicdata-3.2.0/opencivicdata/core/models/__init__.py
--rw-r--r--   0 james      (502) staff       (20)     4522 2019-11-25 15:12:54.000000 opencivicdata-3.2.0/opencivicdata/core/models/base.py
--rw-r--r--   0 james      (502) staff       (20)     4901 2019-11-25 15:12:55.000000 opencivicdata-3.2.0/opencivicdata/core/models/division.py
--rw-r--r--   0 james      (502) staff       (20)     1677 2019-11-25 15:12:54.000000 opencivicdata-3.2.0/opencivicdata/core/models/jurisdiction.py
--rw-r--r--   0 james      (502) staff       (20)    16752 2019-11-25 15:12:55.000000 opencivicdata-3.2.0/opencivicdata/core/models/people_orgs.py
--rw-r--r--   0 james      (502) staff       (20)     3023 2019-11-25 15:12:54.000000 opencivicdata-3.2.0/opencivicdata/divisions.py
-drwxr-xr-x   0 james      (502) staff       (20)        0 2020-03-26 18:54:08.000000 opencivicdata-3.2.0/opencivicdata/elections/
--rw-r--r--   0 james      (502) staff       (20)        0 2019-10-08 14:14:14.000000 opencivicdata-3.2.0/opencivicdata/elections/__init__.py
-drwxr-xr-x   0 james      (502) staff       (20)        0 2020-03-26 18:54:08.000000 opencivicdata-3.2.0/opencivicdata/elections/admin/
--rw-r--r--   0 james      (502) staff       (20)      104 2019-10-08 14:14:14.000000 opencivicdata-3.2.0/opencivicdata/elections/admin/__init__.py
--rw-r--r--   0 james      (502) staff       (20)     1443 2019-11-25 15:12:54.000000 opencivicdata-3.2.0/opencivicdata/elections/admin/candidacy.py
-drwxr-xr-x   0 james      (502) staff       (20)        0 2020-03-26 18:54:08.000000 opencivicdata-3.2.0/opencivicdata/elections/admin/contests/
--rw-r--r--   0 james      (502) staff       (20)        0 2019-10-08 14:14:14.000000 opencivicdata-3.2.0/opencivicdata/elections/admin/contests/__init__.py
--rw-r--r--   0 james      (502) staff       (20)     3250 2019-11-25 15:12:54.000000 opencivicdata-3.2.0/opencivicdata/elections/admin/contests/ballot_measure.py
--rw-r--r--   0 james      (502) staff       (20)     1733 2019-11-25 15:12:54.000000 opencivicdata-3.2.0/opencivicdata/elections/admin/contests/candidate.py
--rw-r--r--   0 james      (502) staff       (20)     1428 2019-11-25 15:12:54.000000 opencivicdata-3.2.0/opencivicdata/elections/admin/contests/party.py
--rw-r--r--   0 james      (502) staff       (20)     1171 2019-11-25 15:12:54.000000 opencivicdata-3.2.0/opencivicdata/elections/admin/election.py
--rw-r--r--   0 james      (502) staff       (20)      198 2019-11-25 15:12:54.000000 opencivicdata-3.2.0/opencivicdata/elections/apps.py
-drwxr-xr-x   0 james      (502) staff       (20)        0 2020-03-26 18:54:08.000000 opencivicdata-3.2.0/opencivicdata/elections/migrations/
--rw-r--r--   0 james      (502) staff       (20)    42491 2019-11-25 15:12:56.000000 opencivicdata-3.2.0/opencivicdata/elections/migrations/0001_initial.py
--rw-r--r--   0 james      (502) staff       (20)      657 2019-11-25 15:12:54.000000 opencivicdata-3.2.0/opencivicdata/elections/migrations/0002_auto_20170731_2047.py
--rw-r--r--   0 james      (502) staff       (20)      398 2019-11-25 15:12:54.000000 opencivicdata-3.2.0/opencivicdata/elections/migrations/0003_election_fk.py
--rw-r--r--   0 james      (502) staff       (20)    12430 2019-11-25 15:12:55.000000 opencivicdata-3.2.0/opencivicdata/elections/migrations/0004_field_docs.py
--rw-r--r--   0 james      (502) staff       (20)     3024 2019-11-25 15:12:55.000000 opencivicdata-3.2.0/opencivicdata/elections/migrations/0005_auto_20170823_1648.py
--rw-r--r--   0 james      (502) staff       (20)     2248 2019-11-25 15:12:55.000000 opencivicdata-3.2.0/opencivicdata/elections/migrations/0006_auto_20171005_2029.py
--rw-r--r--   0 james      (502) staff       (20)     6133 2019-11-25 15:12:55.000000 opencivicdata-3.2.0/opencivicdata/elections/migrations/0007_auto_20171022_0234.py
--rw-r--r--   0 james      (502) staff       (20)     1923 2019-11-25 15:12:55.000000 opencivicdata-3.2.0/opencivicdata/elections/migrations/0008_auto_20181029_1527.py
--rw-r--r--   0 james      (502) staff       (20)        0 2019-10-08 14:14:14.000000 opencivicdata-3.2.0/opencivicdata/elections/migrations/__init__.py
-drwxr-xr-x   0 james      (502) staff       (20)        0 2020-03-26 18:54:08.000000 opencivicdata-3.2.0/opencivicdata/elections/models/
--rw-r--r--   0 james      (502) staff       (20)      718 2019-11-25 15:12:55.000000 opencivicdata-3.2.0/opencivicdata/elections/models/__init__.py
--rw-r--r--   0 james      (502) staff       (20)     3645 2019-11-25 15:12:55.000000 opencivicdata-3.2.0/opencivicdata/elections/models/candidacy.py
-drwxr-xr-x   0 james      (502) staff       (20)        0 2020-03-26 18:54:08.000000 opencivicdata-3.2.0/opencivicdata/elections/models/contests/
--rw-r--r--   0 james      (502) staff       (20)        0 2019-10-08 14:14:14.000000 opencivicdata-3.2.0/opencivicdata/elections/models/contests/__init__.py
--rw-r--r--   0 james      (502) staff       (20)     6084 2019-11-25 15:12:55.000000 opencivicdata-3.2.0/opencivicdata/elections/models/contests/ballot_measure.py
--rw-r--r--   0 james      (502) staff       (20)     1726 2019-11-25 15:12:55.000000 opencivicdata-3.2.0/opencivicdata/elections/models/contests/base.py
--rw-r--r--   0 james      (502) staff       (20)     3970 2019-11-25 15:12:55.000000 opencivicdata-3.2.0/opencivicdata/elections/models/contests/candidate.py
--rw-r--r--   0 james      (502) staff       (20)     2929 2019-11-25 15:12:55.000000 opencivicdata-3.2.0/opencivicdata/elections/models/contests/party.py
--rw-r--r--   0 james      (502) staff       (20)     2705 2019-11-25 15:12:55.000000 opencivicdata-3.2.0/opencivicdata/elections/models/election.py
-drwxr-xr-x   0 james      (502) staff       (20)        0 2020-03-26 18:54:08.000000 opencivicdata-3.2.0/opencivicdata/legislative/
--rw-r--r--   0 james      (502) staff       (20)        0 2019-10-08 14:14:14.000000 opencivicdata-3.2.0/opencivicdata/legislative/__init__.py
-drwxr-xr-x   0 james      (502) staff       (20)        0 2020-03-26 18:54:08.000000 opencivicdata-3.2.0/opencivicdata/legislative/admin/
--rw-r--r--   0 james      (502) staff       (20)       33 2020-03-26 18:52:54.000000 opencivicdata-3.2.0/opencivicdata/legislative/admin/__init__.py
--rw-r--r--   0 james      (502) staff       (20)     3877 2020-03-26 18:48:10.000000 opencivicdata-3.2.0/opencivicdata/legislative/admin/bill.py
--rw-r--r--   0 james      (502) staff       (20)     2879 2020-03-26 18:53:05.000000 opencivicdata-3.2.0/opencivicdata/legislative/admin/event.py
--rw-r--r--   0 james      (502) staff       (20)     1827 2019-11-25 15:12:55.000000 opencivicdata-3.2.0/opencivicdata/legislative/admin/vote.py
--rw-r--r--   0 james      (502) staff       (20)      202 2019-11-25 15:12:55.000000 opencivicdata-3.2.0/opencivicdata/legislative/apps.py
-drwxr-xr-x   0 james      (502) staff       (20)        0 2020-03-26 18:54:08.000000 opencivicdata-3.2.0/opencivicdata/legislative/migrations/
--rw-r--r--   0 james      (502) staff       (20)    44113 2019-11-25 15:12:56.000000 opencivicdata-3.2.0/opencivicdata/legislative/migrations/0001_initial.py
--rw-r--r--   0 james      (502) staff       (20)      769 2019-11-25 15:12:55.000000 opencivicdata-3.2.0/opencivicdata/legislative/migrations/0002_more_extras.py
--rw-r--r--   0 james      (502) staff       (20)     1714 2019-11-25 15:12:55.000000 opencivicdata-3.2.0/opencivicdata/legislative/migrations/0003_time_changes.py
--rw-r--r--   0 james      (502) staff       (20)     5456 2019-11-25 15:12:55.000000 opencivicdata-3.2.0/opencivicdata/legislative/migrations/0004_auto_20171005_2027.py
--rw-r--r--   0 james      (502) staff       (20)     6798 2019-11-25 15:12:55.000000 opencivicdata-3.2.0/opencivicdata/legislative/migrations/0005_auto_20171005_2028.py
--rw-r--r--   0 james      (502) staff       (20)      484 2019-11-25 15:12:55.000000 opencivicdata-3.2.0/opencivicdata/legislative/migrations/0006_billversion_extras.py
--rw-r--r--   0 james      (502) staff       (20)      484 2019-11-25 15:12:55.000000 opencivicdata-3.2.0/opencivicdata/legislative/migrations/0007_auto_20181029_1527.py
--rw-r--r--   0 james      (502) staff       (20)      299 2019-11-25 15:12:55.000000 opencivicdata-3.2.0/opencivicdata/legislative/migrations/0008_longer_event_name.py
--rw-r--r--   0 james      (502) staff       (20)     1832 2019-11-25 15:12:55.000000 opencivicdata-3.2.0/opencivicdata/legislative/migrations/0009_searchablebill.py
--rw-r--r--   0 james      (502) staff       (20)     1793 2019-11-25 15:12:55.000000 opencivicdata-3.2.0/opencivicdata/legislative/migrations/0010_auto_20191031_1507.py
--rw-r--r--   0 james      (502) staff       (20)      606 2019-11-25 15:12:55.000000 opencivicdata-3.2.0/opencivicdata/legislative/migrations/0011_auto_20191124_1658.py
--rw-r--r--   0 james      (502) staff       (20)      471 2020-03-26 04:59:03.000000 opencivicdata-3.2.0/opencivicdata/legislative/migrations/0012_billdocument_extras.py
--rw-r--r--   0 james      (502) staff       (20)      472 2020-03-26 04:58:16.000000 opencivicdata-3.2.0/opencivicdata/legislative/migrations/0013_auto_20200326_0458.py
--rw-r--r--   0 james      (502) staff       (20)        0 2019-10-08 14:14:14.000000 opencivicdata-3.2.0/opencivicdata/legislative/migrations/__init__.py
-drwxr-xr-x   0 james      (502) staff       (20)        0 2020-03-26 18:54:08.000000 opencivicdata-3.2.0/opencivicdata/legislative/models/
--rw-r--r--   0 james      (502) staff       (20)      678 2020-01-13 16:48:33.000000 opencivicdata-3.2.0/opencivicdata/legislative/models/__init__.py
--rw-r--r--   0 james      (502) staff       (20)     7735 2020-03-26 04:58:17.000000 opencivicdata-3.2.0/opencivicdata/legislative/models/bill.py
--rw-r--r--   0 james      (502) staff       (20)     6998 2020-01-13 16:48:33.000000 opencivicdata-3.2.0/opencivicdata/legislative/models/event.py
--rw-r--r--   0 james      (502) staff       (20)      923 2019-11-25 15:12:55.000000 opencivicdata-3.2.0/opencivicdata/legislative/models/session.py
--rw-r--r--   0 james      (502) staff       (20)     3396 2020-02-14 05:58:59.000000 opencivicdata-3.2.0/opencivicdata/legislative/models/vote.py
-drwxr-xr-x   0 james      (502) staff       (20)        0 2020-03-26 18:54:08.000000 opencivicdata-3.2.0/opencivicdata/tests/
--rw-r--r--   0 james      (502) staff       (20)        0 2019-10-08 14:14:14.000000 opencivicdata-3.2.0/opencivicdata/tests/__init__.py
--rw-r--r--   0 james      (502) staff       (20)     6647 2020-01-13 16:48:33.000000 opencivicdata-3.2.0/opencivicdata/tests/conftest.py
--rw-r--r--   0 james      (502) staff       (20)      384 2019-11-25 15:12:55.000000 opencivicdata-3.2.0/opencivicdata/tests/test_division.py
--rw-r--r--   0 james      (502) staff       (20)     2630 2019-11-25 15:12:55.000000 opencivicdata-3.2.0/opencivicdata/tests/test_elections.py
--rw-r--r--   0 james      (502) staff       (20)      693 2019-11-25 15:12:55.000000 opencivicdata-3.2.0/opencivicdata/tests/test_loaddivisions.py
--rw-r--r--   0 james      (502) staff       (20)    14560 2019-11-25 15:12:56.000000 opencivicdata-3.2.0/opencivicdata/tests/test_models.py
--rw-r--r--   0 james      (502) staff       (20)      441 2020-01-13 16:48:33.000000 opencivicdata-3.2.0/opencivicdata/tests/test_settings.py
-drwxr-xr-x   0 james      (502) staff       (20)        0 2020-03-26 18:54:08.000000 opencivicdata-3.2.0/opencivicdata.egg-info/
--rw-r--r--   0 james      (502) staff       (20)      624 2020-03-26 18:54:08.000000 opencivicdata-3.2.0/opencivicdata.egg-info/PKG-INFO
--rw-r--r--   0 james      (502) staff       (20)     4176 2020-03-26 18:54:08.000000 opencivicdata-3.2.0/opencivicdata.egg-info/SOURCES.txt
--rw-r--r--   0 james      (502) staff       (20)        1 2020-03-26 18:54:08.000000 opencivicdata-3.2.0/opencivicdata.egg-info/dependency_links.txt
--rw-r--r--   0 james      (502) staff       (20)       89 2020-03-26 18:54:08.000000 opencivicdata-3.2.0/opencivicdata.egg-info/requires.txt
--rw-r--r--   0 james      (502) staff       (20)       14 2020-03-26 18:54:08.000000 opencivicdata-3.2.0/opencivicdata.egg-info/top_level.txt
--rw-r--r--   0 james      (502) staff       (20)      136 2020-03-26 18:54:08.000000 opencivicdata-3.2.0/setup.cfg
--rw-r--r--   0 james      (502) staff       (20)     1015 2020-03-26 18:51:47.000000 opencivicdata-3.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 15:59:36.010058 opencivicdata-3.3.0/
+-rw-r--r--   0 runner    (1001) docker     (122)      105 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      624 2023-05-16 15:59:36.010058 opencivicdata-3.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      851 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 15:59:35.994058 opencivicdata-3.3.0/opencivicdata/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6495 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/common.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 15:59:35.998058 opencivicdata-3.3.0/opencivicdata/core/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 15:59:35.998058 opencivicdata-3.3.0/opencivicdata/core/admin/
+-rw-r--r--   0 runner    (1001) docker     (122)       50 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/core/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1599 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/core/admin/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2888 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/core/admin/organization.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1918 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/core/admin/other.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2689 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/core/admin/person.py
+-rw-r--r--   0 runner    (1001) docker     (122)      188 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/core/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 15:59:35.998058 opencivicdata-3.3.0/opencivicdata/core/management/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/core/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 15:59:35.998058 opencivicdata-3.3.0/opencivicdata/core/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/core/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2623 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/core/management/commands/loaddivisions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 15:59:35.998058 opencivicdata-3.3.0/opencivicdata/core/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)    33372 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/core/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)      437 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/core/migrations/0002_post_maximum_memberships.py
+-rw-r--r--   0 runner    (1001) docker     (122)    41542 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/core/migrations/0003_field_docs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3559 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/core/migrations/0004_auto_20171005_2028.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1097 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/core/migrations/0005_auto_20191031_1507.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1081 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/core/migrations/0005_auto_20191124_1658.py
+-rw-r--r--   0 runner    (1001) docker     (122)      267 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/core/migrations/0006_merge_20200103_1432.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1575 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/core/migrations/0007_jurisdiction_last_seen_membership_last_seen_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1508 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/core/migrations/0008_auto_20221215_1132.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/core/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 15:59:36.002058 opencivicdata-3.3.0/opencivicdata/core/models/
+-rw-r--r--   0 runner    (1001) docker     (122)      480 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/core/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4661 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/core/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4901 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/core/models/division.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1677 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/core/models/jurisdiction.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16752 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/core/models/people_orgs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3023 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/divisions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 15:59:36.002058 opencivicdata-3.3.0/opencivicdata/elections/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/elections/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 15:59:36.002058 opencivicdata-3.3.0/opencivicdata/elections/admin/
+-rw-r--r--   0 runner    (1001) docker     (122)      104 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/elections/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1443 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/elections/admin/candidacy.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 15:59:36.002058 opencivicdata-3.3.0/opencivicdata/elections/admin/contests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/elections/admin/contests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3250 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/elections/admin/contests/ballot_measure.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1733 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/elections/admin/contests/candidate.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1428 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/elections/admin/contests/party.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1171 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/elections/admin/election.py
+-rw-r--r--   0 runner    (1001) docker     (122)      198 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/elections/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 15:59:36.002058 opencivicdata-3.3.0/opencivicdata/elections/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)    42827 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/elections/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)      657 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/elections/migrations/0002_auto_20170731_2047.py
+-rw-r--r--   0 runner    (1001) docker     (122)      398 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/elections/migrations/0003_election_fk.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12472 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/elections/migrations/0004_field_docs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3059 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/elections/migrations/0005_auto_20170823_1648.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2269 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/elections/migrations/0006_auto_20171005_2029.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6210 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/elections/migrations/0007_auto_20171022_0234.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1944 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/elections/migrations/0008_auto_20181029_1527.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1876 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/elections/migrations/0009_auto_20221208_1041.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1756 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/elections/migrations/0010_auto_20221215_1132.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/elections/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 15:59:36.002058 opencivicdata-3.3.0/opencivicdata/elections/models/
+-rw-r--r--   0 runner    (1001) docker     (122)      718 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/elections/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3645 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/elections/models/candidacy.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 15:59:36.006058 opencivicdata-3.3.0/opencivicdata/elections/models/contests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/elections/models/contests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6084 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/elections/models/contests/ballot_measure.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1726 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/elections/models/contests/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3970 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/elections/models/contests/candidate.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2929 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/elections/models/contests/party.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2705 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/elections/models/election.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 15:59:36.006058 opencivicdata-3.3.0/opencivicdata/legislative/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/legislative/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 15:59:36.006058 opencivicdata-3.3.0/opencivicdata/legislative/admin/
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/legislative/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3877 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/legislative/admin/bill.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2879 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/legislative/admin/event.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1827 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/legislative/admin/vote.py
+-rw-r--r--   0 runner    (1001) docker     (122)      202 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/legislative/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 15:59:36.006058 opencivicdata-3.3.0/opencivicdata/legislative/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)    44134 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/legislative/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)      769 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/legislative/migrations/0002_more_extras.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1714 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/legislative/migrations/0003_time_changes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5477 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/legislative/migrations/0004_auto_20171005_2027.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6798 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/legislative/migrations/0005_auto_20171005_2028.py
+-rw-r--r--   0 runner    (1001) docker     (122)      484 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/legislative/migrations/0006_billversion_extras.py
+-rw-r--r--   0 runner    (1001) docker     (122)      484 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/legislative/migrations/0007_auto_20181029_1527.py
+-rw-r--r--   0 runner    (1001) docker     (122)      299 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/legislative/migrations/0008_longer_event_name.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1832 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/legislative/migrations/0009_searchablebill.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1793 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/legislative/migrations/0010_auto_20191031_1507.py
+-rw-r--r--   0 runner    (1001) docker     (122)      606 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/legislative/migrations/0011_auto_20191124_1658.py
+-rw-r--r--   0 runner    (1001) docker     (122)      471 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/legislative/migrations/0012_billdocument_extras.py
+-rw-r--r--   0 runner    (1001) docker     (122)      472 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/legislative/migrations/0013_auto_20200326_0458.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1035 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/legislative/migrations/0014_bill_last_seen_event_last_seen_voteevent_last_seen.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1007 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/legislative/migrations/0015_auto_20221215_1132.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/legislative/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 15:59:36.010058 opencivicdata-3.3.0/opencivicdata/legislative/models/
+-rw-r--r--   0 runner    (1001) docker     (122)      678 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/legislative/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7735 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/legislative/models/bill.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6998 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/legislative/models/event.py
+-rw-r--r--   0 runner    (1001) docker     (122)      923 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/legislative/models/session.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3396 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/legislative/models/vote.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 15:59:36.010058 opencivicdata-3.3.0/opencivicdata/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6647 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)      384 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/tests/test_division.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2630 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/tests/test_elections.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1552 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/tests/test_loaddivisions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14560 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (122)      441 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/tests/test_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 15:59:35.998058 opencivicdata-3.3.0/opencivicdata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      624 2023-05-16 15:59:35.000000 opencivicdata-3.3.0/opencivicdata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4608 2023-05-16 15:59:35.000000 opencivicdata-3.3.0/opencivicdata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-16 15:59:35.000000 opencivicdata-3.3.0/opencivicdata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       96 2023-05-16 15:59:35.000000 opencivicdata-3.3.0/opencivicdata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       14 2023-05-16 15:59:35.000000 opencivicdata-3.3.0/opencivicdata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      136 2023-05-16 15:59:36.010058 opencivicdata-3.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1021 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `opencivicdata-3.2.0/PKG-INFO` & `opencivicdata-3.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opencivicdata
-Version: 3.2.0
+Version: 3.3.0
 Summary: python opencivicdata library
 Home-page: UNKNOWN
 Author: James Turk
 Author-email: james@openstates.org
 License: BSD
 Description: UNKNOWN
 Platform: any
```

### Comparing `opencivicdata-3.2.0/README.md` & `opencivicdata-3.3.0/README.md`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.2.0/opencivicdata/common.py` & `opencivicdata-3.3.0/opencivicdata/common.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.2.0/opencivicdata/core/admin/base.py` & `opencivicdata-3.3.0/opencivicdata/core/admin/base.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.2.0/opencivicdata/core/admin/organization.py` & `opencivicdata-3.3.0/opencivicdata/core/admin/organization.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.2.0/opencivicdata/core/admin/other.py` & `opencivicdata-3.3.0/opencivicdata/core/admin/other.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.2.0/opencivicdata/core/admin/person.py` & `opencivicdata-3.3.0/opencivicdata/core/admin/person.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.2.0/opencivicdata/core/management/commands/loaddivisions.py` & `opencivicdata-3.3.0/opencivicdata/core/management/commands/loaddivisions.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,26 +26,31 @@
 
     print(
         "{} divisions found in the CSV, and {} already in the DB".format(
             len(objects), existing_divisions.count()
         )
     )
 
-    if set(objects) == set(existing_divisions):
+    objects_set = set(objects)
+    existing_divisions_set = set(existing_divisions)
+
+    if objects_set == existing_divisions_set:
         print("The CSV and the DB contents are exactly the same; no work to be done!")
+    elif objects_set.issubset(existing_divisions_set):
+        print("The DB contains all CSV contents; no work to be done!")
     else:
         if bulk:
             # delete old ids and add new ones all at once
             with transaction.atomic():
                 Division.objects.filter(country=country).delete()
                 Division.objects.bulk_create(objects, batch_size=10000)
             print("{} divisions created".format(len(objects)))
         else:
-            to_create = set(objects) - set(existing_divisions)
-            to_delete = set(existing_divisions) - set(objects)
+            to_create = objects_set - existing_divisions_set
+            to_delete = existing_divisions_set - objects_set
             # delete removed ids and add new ones all at once
             with transaction.atomic():
                 for division in to_delete:
                     division.delete()
                 for division in to_create:
                     division.save()
             print("{} divisions deleted".format(len(to_delete)))
```

### Comparing `opencivicdata-3.2.0/opencivicdata/core/migrations/0001_initial.py` & `opencivicdata-3.3.0/opencivicdata/core/migrations/0001_initial.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,16 +76,16 @@
                     "id",
                     opencivicdata.core.models.base.OCDIDField(
                         ocd_type="jurisdiction",
                         serialize=False,
                         validators=[
                             django.core.validators.RegexValidator(
                                 flags=32,
-                                message="ID must match ^ocd-jurisdiction/country:[a-z]{2}(/[^\\W\\d]+:[\\w.~-]+)*/\\w+$",
-                                regex="^ocd-jurisdiction/country:[a-z]{2}(/[^\\W\\d]+:[\\w.~-]+)*/\\w+$",
+                                message="ID must match ^ocd-jurisdiction/country:[a-z]{2}(/[^\\W\\d]+:[\\w.~-]+)*/\\w+$", # noqa
+                                regex="^ocd-jurisdiction/country:[a-z]{2}(/[^\\W\\d]+:[\\w.~-]+)*/\\w+$", # noqa
                             )
                         ],
                     ),
                 ),
                 ("name", models.CharField(max_length=300)),
                 ("url", models.URLField(max_length=2000)),
                 (
@@ -150,15 +150,15 @@
                     "id",
                     opencivicdata.core.models.base.OCDIDField(
                         ocd_type="membership",
                         serialize=False,
                         validators=[
                             django.core.validators.RegexValidator(
                                 flags=32,
-                                message="ID must match ^ocd-membership/[0-9a-f]{8}-([0-9a-f]{4}-){3}[0-9a-f]{12}$",
+                                message="ID must match ^ocd-membership/[0-9a-f]{8}-([0-9a-f]{4}-){3}[0-9a-f]{12}$", # noqa
                                 regex="^ocd-membership/[0-9a-f]{8}-([0-9a-f]{4}-){3}[0-9a-f]{12}$",
                             )
                         ],
                     ),
                 ),
                 (
                     "person_name",
@@ -263,16 +263,16 @@
                     "id",
                     opencivicdata.core.models.base.OCDIDField(
                         ocd_type="organization",
                         serialize=False,
                         validators=[
                             django.core.validators.RegexValidator(
                                 flags=32,
-                                message="ID must match ^ocd-organization/[0-9a-f]{8}-([0-9a-f]{4}-){3}[0-9a-f]{12}$",
-                                regex="^ocd-organization/[0-9a-f]{8}-([0-9a-f]{4}-){3}[0-9a-f]{12}$",
+                                message="ID must match ^ocd-organization/[0-9a-f]{8}-([0-9a-f]{4}-){3}[0-9a-f]{12}$", # noqa
+                                regex="^ocd-organization/[0-9a-f]{8}-([0-9a-f]{4}-){3}[0-9a-f]{12}$", # noqa
                             )
                         ],
                     ),
                 ),
                 ("name", models.CharField(max_length=300)),
                 ("image", models.URLField(blank=True, max_length=2000)),
                 (
@@ -486,15 +486,15 @@
                     "id",
                     opencivicdata.core.models.base.OCDIDField(
                         ocd_type="person",
                         serialize=False,
                         validators=[
                             django.core.validators.RegexValidator(
                                 flags=32,
-                                message="ID must match ^ocd-person/[0-9a-f]{8}-([0-9a-f]{4}-){3}[0-9a-f]{12}$",
+                                message="ID must match ^ocd-person/[0-9a-f]{8}-([0-9a-f]{4}-){3}[0-9a-f]{12}$", # noqa
                                 regex="^ocd-person/[0-9a-f]{8}-([0-9a-f]{4}-){3}[0-9a-f]{12}$",
                             )
                         ],
                     ),
                 ),
                 ("name", models.CharField(db_index=True, max_length=300)),
                 ("sort_name", models.CharField(blank=True, default="", max_length=100)),
@@ -682,15 +682,15 @@
                     "id",
                     opencivicdata.core.models.base.OCDIDField(
                         ocd_type="post",
                         serialize=False,
                         validators=[
                             django.core.validators.RegexValidator(
                                 flags=32,
-                                message="ID must match ^ocd-post/[0-9a-f]{8}-([0-9a-f]{4}-){3}[0-9a-f]{12}$",
+                                message="ID must match ^ocd-post/[0-9a-f]{8}-([0-9a-f]{4}-){3}[0-9a-f]{12}$", # noqa
                                 regex="^ocd-post/[0-9a-f]{8}-([0-9a-f]{4}-){3}[0-9a-f]{12}$",
                             )
                         ],
                     ),
                 ),
                 ("label", models.CharField(max_length=300)),
                 ("role", models.CharField(blank=True, max_length=300)),
```

### Comparing `opencivicdata-3.2.0/opencivicdata/core/migrations/0003_field_docs.py` & `opencivicdata-3.3.0/opencivicdata/core/migrations/0003_field_docs.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     dependencies = [("core", "0002_post_maximum_memberships")]
 
     operations = [
         migrations.AlterField(
             model_name="division",
             name="country",
             field=models.CharField(
-                help_text="An ISO-3166-1 alpha-2 code identifying the county where this division is found.",
+                help_text="An ISO-3166-1 alpha-2 code identifying the county where this division is found.", # noqa
                 max_length=2,
             ),
         ),
         migrations.AlterField(
             model_name="division",
             name="name",
             field=models.CharField(
@@ -193,15 +193,15 @@
         ),
         migrations.AlterField(
             model_name="jurisdiction",
             name="extras",
             field=django.contrib.postgres.fields.jsonb.JSONField(
                 blank=True,
                 default=dict,
-                help_text="A key-value store for storing arbitrary information not covered elsewhere.",
+                help_text="A key-value store for storing arbitrary information not covered elsewhere.", # noqa
             ),
         ),
         migrations.AlterField(
             model_name="jurisdiction",
             name="feature_flags",
             field=django.contrib.postgres.fields.ArrayField(
                 base_field=models.TextField(),
@@ -241,25 +241,25 @@
             ),
         ),
         migrations.AlterField(
             model_name="membership",
             name="end_date",
             field=models.CharField(
                 blank=True,
-                help_text="The date on which the relationship ended in YYYY[-MM[-DD]] string format.",
+                help_text="The date on which the relationship ended in YYYY[-MM[-DD]] string format.", # noqa
                 max_length=10,
             ),
         ),
         migrations.AlterField(
             model_name="membership",
             name="extras",
             field=django.contrib.postgres.fields.jsonb.JSONField(
                 blank=True,
                 default=dict,
-                help_text="A key-value store for storing arbitrary information not covered elsewhere.",
+                help_text="A key-value store for storing arbitrary information not covered elsewhere.", # noqa
             ),
         ),
         migrations.AlterField(
             model_name="membership",
             name="label",
             field=models.CharField(
                 blank=True,
@@ -267,15 +267,15 @@
                 max_length=300,
             ),
         ),
         migrations.AlterField(
             model_name="membership",
             name="on_behalf_of",
             field=models.ForeignKey(
-                help_text="The Organization on whose behalf the Person is a member of the Organization.",
+                help_text="The Organization on whose behalf the Person is a member of the Organization.", # noqa
                 null=True,
                 on_delete=django.db.models.deletion.CASCADE,
                 related_name="memberships_on_behalf_of",
                 to="core.Organization",
             ),
         ),
         migrations.AlterField(
@@ -330,15 +330,15 @@
             ),
         ),
         migrations.AlterField(
             model_name="membership",
             name="start_date",
             field=models.CharField(
                 blank=True,
-                help_text="The date on which the relationship began in YYYY[-MM[-DD]] string format.",
+                help_text="The date on which the relationship began in YYYY[-MM[-DD]] string format.", # noqa
                 max_length=10,
             ),
         ),
         migrations.AlterField(
             model_name="membership",
             name="updated_at",
             field=models.DateTimeField(
@@ -392,15 +392,15 @@
                 max_length=50,
             ),
         ),
         migrations.AlterField(
             model_name="membershipcontactdetail",
             name="value",
             field=models.CharField(
-                help_text="The content of the Contact information like a phone number or email address.",
+                help_text="The content of the Contact information like a phone number or email address.", # noqa
                 max_length=300,
             ),
         ),
         migrations.AlterField(
             model_name="membershiplink",
             name="membership",
             field=models.ForeignKey(
@@ -455,25 +455,25 @@
             ),
         ),
         migrations.AlterField(
             model_name="organization",
             name="dissolution_date",
             field=models.CharField(
                 blank=True,
-                help_text="The dissolution date of the Organization in YYYY[-MM[-DD]] string format.",
+                help_text="The dissolution date of the Organization in YYYY[-MM[-DD]] string format.", # noqa
                 max_length=10,
             ),
         ),
         migrations.AlterField(
             model_name="organization",
             name="extras",
             field=django.contrib.postgres.fields.jsonb.JSONField(
                 blank=True,
                 default=dict,
-                help_text="A key-value store for storing arbitrary information not covered elsewhere.",
+                help_text="A key-value store for storing arbitrary information not covered elsewhere.", # noqa
             ),
         ),
         migrations.AlterField(
             model_name="organization",
             name="founding_date",
             field=models.CharField(
                 blank=True,
@@ -508,15 +508,15 @@
                 help_text="The name of the Organization.", max_length=300
             ),
         ),
         migrations.AlterField(
             model_name="organization",
             name="parent",
             field=models.ForeignKey(
-                help_text="A link to another Organization that serves as this Organization's parent.",
+                help_text="A link to another Organization that serves as this Organization's parent.", # noqa
                 null=True,
                 on_delete=django.db.models.deletion.CASCADE,
                 related_name="children",
                 to="core.Organization",
             ),
         ),
         migrations.AlterField(
@@ -573,15 +573,15 @@
                 max_length=50,
             ),
         ),
         migrations.AlterField(
             model_name="organizationcontactdetail",
             name="value",
             field=models.CharField(
-                help_text="The content of the Contact information like a phone number or email address.",
+                help_text="The content of the Contact information like a phone number or email address.", # noqa
                 max_length=300,
             ),
         ),
         migrations.AlterField(
             model_name="organizationidentifier",
             name="identifier",
             field=models.CharField(
@@ -589,15 +589,15 @@
                 max_length=300,
             ),
         ),
         migrations.AlterField(
             model_name="organizationidentifier",
             name="organization",
             field=models.ForeignKey(
-                help_text="Reference to the Organization identified by this alternative identifier.",
+                help_text="Reference to the Organization identified by this alternative identifier.", # noqa
                 on_delete=django.db.models.deletion.CASCADE,
                 related_name="identifiers",
                 to="core.Organization",
             ),
         ),
         migrations.AlterField(
             model_name="organizationidentifier",
@@ -634,15 +634,15 @@
             ),
         ),
         migrations.AlterField(
             model_name="organizationname",
             name="end_date",
             field=models.CharField(
                 blank=True,
-                help_text="An optional end date for usage of the alternative name in YYYY[-MM[-DD]] string format.",
+                help_text="An optional end date for usage of the alternative name in YYYY[-MM[-DD]] string format.", # noqa
                 max_length=10,
             ),
         ),
         migrations.AlterField(
             model_name="organizationname",
             name="name",
             field=models.CharField(
@@ -669,15 +669,15 @@
             ),
         ),
         migrations.AlterField(
             model_name="organizationname",
             name="start_date",
             field=models.CharField(
                 blank=True,
-                help_text="An optional start date for usage of the alternative name in YYYY[-MM[-DD]] string format.",
+                help_text="An optional start date for usage of the alternative name in YYYY[-MM[-DD]] string format.", # noqa
                 max_length=10,
             ),
         ),
         migrations.AlterField(
             model_name="organizationsource",
             name="note",
             field=models.CharField(
@@ -737,15 +737,15 @@
         ),
         migrations.AlterField(
             model_name="person",
             name="extras",
             field=django.contrib.postgres.fields.jsonb.JSONField(
                 blank=True,
                 default=dict,
-                help_text="A key-value store for storing arbitrary information not covered elsewhere.",
+                help_text="A key-value store for storing arbitrary information not covered elsewhere.", # noqa
             ),
         ),
         migrations.AlterField(
             model_name="person",
             name="family_name",
             field=models.CharField(
                 blank=True, help_text="A Person's family name.", max_length=100
@@ -865,15 +865,15 @@
                 max_length=50,
             ),
         ),
         migrations.AlterField(
             model_name="personcontactdetail",
             name="value",
             field=models.CharField(
-                help_text="The content of the Contact information like a phone number or email address.",
+                help_text="The content of the Contact information like a phone number or email address.", # noqa
                 max_length=300,
             ),
         ),
         migrations.AlterField(
             model_name="personidentifier",
             name="identifier",
             field=models.CharField(
@@ -926,15 +926,15 @@
             ),
         ),
         migrations.AlterField(
             model_name="personname",
             name="end_date",
             field=models.CharField(
                 blank=True,
-                help_text="An optional end date for usage of the alternative name in YYYY[-MM[-DD]] string format.",
+                help_text="An optional end date for usage of the alternative name in YYYY[-MM[-DD]] string format.", # noqa
                 max_length=10,
             ),
         ),
         migrations.AlterField(
             model_name="personname",
             name="name",
             field=models.CharField(
@@ -961,15 +961,15 @@
             ),
         ),
         migrations.AlterField(
             model_name="personname",
             name="start_date",
             field=models.CharField(
                 blank=True,
-                help_text="An optional start date for usage of the alternative name in YYYY[-MM[-DD]] string format.",
+                help_text="An optional start date for usage of the alternative name in YYYY[-MM[-DD]] string format.", # noqa
                 max_length=10,
             ),
         ),
         migrations.AlterField(
             model_name="personsource",
             name="note",
             field=models.CharField(
@@ -1026,15 +1026,15 @@
         ),
         migrations.AlterField(
             model_name="post",
             name="extras",
             field=django.contrib.postgres.fields.jsonb.JSONField(
                 blank=True,
                 default=dict,
-                help_text="A key-value store for storing arbitrary information not covered elsewhere.",
+                help_text="A key-value store for storing arbitrary information not covered elsewhere.", # noqa
             ),
         ),
         migrations.AlterField(
             model_name="post",
             name="label",
             field=models.CharField(
                 help_text="A label describing the Post.", max_length=300
@@ -1130,15 +1130,15 @@
                 max_length=50,
             ),
         ),
         migrations.AlterField(
             model_name="postcontactdetail",
             name="value",
             field=models.CharField(
-                help_text="The content of the Contact information like a phone number or email address.",
+                help_text="The content of the Contact information like a phone number or email address.", # noqa
                 max_length=300,
             ),
         ),
         migrations.AlterField(
             model_name="postlink",
             name="note",
             field=models.CharField(
```

### Comparing `opencivicdata-3.2.0/opencivicdata/core/migrations/0004_auto_20171005_2028.py` & `opencivicdata-3.3.0/opencivicdata/core/migrations/0004_auto_20171005_2028.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
                 to="core.Division",
             ),
         ),
         migrations.AlterField(
             model_name="membership",
             name="on_behalf_of",
             field=models.ForeignKey(
-                help_text="The Organization on whose behalf the Person is a member of the Organization.",
+                help_text="The Organization on whose behalf the Person is a member of the Organization.", # noqa
                 null=True,
                 on_delete=django.db.models.deletion.SET_NULL,
                 related_name="memberships_on_behalf_of",
                 to="core.Organization",
             ),
         ),
         migrations.AlterField(
@@ -74,15 +74,15 @@
                 to="core.Jurisdiction",
             ),
         ),
         migrations.AlterField(
             model_name="organization",
             name="parent",
             field=models.ForeignKey(
-                help_text="A link to another Organization that serves as this Organization's parent.",
+                help_text="A link to another Organization that serves as this Organization's parent.", # noqa
                 null=True,
                 on_delete=django.db.models.deletion.SET_NULL,
                 related_name="children",
                 to="core.Organization",
             ),
         ),
         migrations.AlterField(
```

### Comparing `opencivicdata-3.2.0/opencivicdata/core/migrations/0005_auto_20191124_1658.py` & `opencivicdata-3.3.0/opencivicdata/core/migrations/0005_auto_20191124_1658.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.2.0/opencivicdata/core/models/base.py` & `opencivicdata-3.3.0/opencivicdata/core/models/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,19 @@
 class OCDBase(models.Model):
     """ common base fields across all top-level models """
 
     created_at = models.DateTimeField(
         auto_now_add=True, help_text="The date and time of creation."
     )
     updated_at = models.DateTimeField(
-        auto_now=True, help_text="The date and time of the last update."
+        auto_now_add=True, help_text="The date and time of the last update."
+    )
+    last_seen = models.DateTimeField(
+        auto_now=True,
+        help_text="The last time this object was seen in a scrape."
     )
     extras = JSONField(
         default=dict,
         blank=True,
         help_text="A key-value store for storing arbitrary information not covered elsewhere.",
     )
     locked_fields = ArrayField(base_field=models.TextField(), blank=True, default=list)
```

### Comparing `opencivicdata-3.2.0/opencivicdata/core/models/division.py` & `opencivicdata-3.3.0/opencivicdata/core/models/division.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.2.0/opencivicdata/core/models/jurisdiction.py` & `opencivicdata-3.3.0/opencivicdata/core/models/jurisdiction.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.2.0/opencivicdata/core/models/people_orgs.py` & `opencivicdata-3.3.0/opencivicdata/core/models/people_orgs.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.2.0/opencivicdata/divisions.py` & `opencivicdata-3.3.0/opencivicdata/divisions.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.2.0/opencivicdata/elections/admin/candidacy.py` & `opencivicdata-3.3.0/opencivicdata/elections/admin/candidacy.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.2.0/opencivicdata/elections/admin/contests/ballot_measure.py` & `opencivicdata-3.3.0/opencivicdata/elections/admin/contests/ballot_measure.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.2.0/opencivicdata/elections/admin/contests/candidate.py` & `opencivicdata-3.3.0/opencivicdata/elections/admin/contests/candidate.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.2.0/opencivicdata/elections/admin/contests/party.py` & `opencivicdata-3.3.0/opencivicdata/elections/admin/contests/party.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.2.0/opencivicdata/elections/admin/election.py` & `opencivicdata-3.3.0/opencivicdata/elections/admin/election.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.2.0/opencivicdata/elections/migrations/0001_initial.py` & `opencivicdata-3.3.0/opencivicdata/elections/migrations/0001_initial.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,60 +37,60 @@
                         default=list,
                         size=None,
                     ),
                 ),
                 (
                     "id",
                     opencivicdata.core.models.base.OCDIDField(
-                        help_text="Open Civic Data-style id in the format ``ocd-contest/{{uuid}}``.",
+                        help_text="Open Civic Data-style id in the format ``ocd-contest/{{uuid}}``.", # noqa
                         ocd_type="contest",
                         serialize=False,
                         validators=[
                             django.core.validators.RegexValidator(
                                 flags=32,
-                                message="ID must match ^ocd-contest/[0-9a-f]{8}-([0-9a-f]{4}-){3}[0-9a-f]{12}$",
+                                message="ID must match ^ocd-contest/[0-9a-f]{8}-([0-9a-f]{4}-){3}[0-9a-f]{12}$", # noqa
                                 regex="^ocd-contest/[0-9a-f]{8}-([0-9a-f]{4}-){3}[0-9a-f]{12}$",
                             )
                         ],
                     ),
                 ),
                 (
                     "name",
                     models.CharField(
-                        help_text="Name of the contest, not necessarily as it appears on the ballot.",
+                        help_text="Name of the contest, not necessarily as it appears on the ballot.", # noqa
                         max_length=300,
                     ),
                 ),
                 (
                     "description",
                     models.TextField(
-                        help_text="Text describing the purpose and/or potential outcomes of the ballot measure, not necessarily as it appears on the ballot."
+                        help_text="Text describing the purpose and/or potential outcomes of the ballot measure, not necessarily as it appears on the ballot." # noqa
                     ),
                 ),
                 (
                     "requirement",
                     models.CharField(
                         blank=True,
                         default="50% plus one vote",
-                        help_text="The threshold of votes the ballot measure needs in order to pass.",
+                        help_text="The threshold of votes the ballot measure needs in order to pass.", # noqa
                         max_length=300,
                     ),
                 ),
                 (
                     "classification",
                     models.CharField(
                         blank=True,
-                        help_text='Describes the origin and/or potential outcome of the ballot measure, e.g., "initiative statute", "legislative constitutional amendment".',
+                        help_text='Describes the origin and/or potential outcome of the ballot measure, e.g., "initiative statute", "legislative constitutional amendment".', # noqa
                         max_length=300,
                     ),
                 ),
                 (
                     "division",
                     models.ForeignKey(
-                        help_text="Reference to the Division that defines the political geography of the contest, e.g., a specific Congressional or State Senate district. Should be a subdivision of the Division referenced by the contest's Election.",
+                        help_text="Reference to the Division that defines the political geography of the contest, e.g., a specific Congressional or State Senate district. Should be a subdivision of the Division referenced by the contest's Election.", # noqa
                         on_delete=django.db.models.deletion.CASCADE,
                         related_name="ballotmeasurecontests",
                         related_query_name="ballotmeasurecontests",
                         to="core.Division",
                     ),
                 ),
             ],
@@ -109,15 +109,15 @@
                     ),
                 ),
                 ("identifier", models.CharField(max_length=300)),
                 ("scheme", models.CharField(max_length=300)),
                 (
                     "contest",
                     models.ForeignKey(
-                        help_text="Reference to the BallotMeasureContest linked to the upstream identifier.",
+                        help_text="Reference to the BallotMeasureContest linked to the upstream identifier.", # noqa
                         on_delete=django.db.models.deletion.CASCADE,
                         related_name="identifiers",
                         to="elections.BallotMeasureContest",
                     ),
                 ),
             ],
             options={"db_table": "opencivicdata_ballotmeasurecontestidentifier"},
@@ -133,15 +133,15 @@
                         serialize=False,
                         verbose_name="ID",
                     ),
                 ),
                 (
                     "text",
                     models.CharField(
-                        help_text="Text of the option, not necessarily as it appears on the ballot.",
+                        help_text="Text of the option, not necessarily as it appears on the ballot.", # noqa
                         max_length=300,
                     ),
                 ),
                 (
                     "contest",
                     models.ForeignKey(
                         help_text="Reference to the BallotMeasureContest.",
@@ -166,15 +166,15 @@
                     ),
                 ),
                 ("note", models.CharField(blank=True, max_length=300)),
                 ("url", models.URLField(max_length=2000)),
                 (
                     "contest",
                     models.ForeignKey(
-                        help_text="Reference to the BallotMeasureContest assembled from the source.",
+                        help_text="Reference to the BallotMeasureContest assembled from the source.", # noqa
                         on_delete=django.db.models.deletion.CASCADE,
                         related_name="sources",
                         to="elections.BallotMeasureContest",
                     ),
                 ),
             ],
             options={"db_table": "opencivicdata_ballotmeasurecontestsource"},
@@ -198,21 +198,21 @@
                         default=list,
                         size=None,
                     ),
                 ),
                 (
                     "id",
                     opencivicdata.core.models.base.OCDIDField(
-                        help_text="Open Civic Data-style id in the format ``ocd-candidacy/{{uuid}}``.",
+                        help_text="Open Civic Data-style id in the format ``ocd-candidacy/{{uuid}}``.", # noqa
                         ocd_type="candidacy",
                         serialize=False,
                         validators=[
                             django.core.validators.RegexValidator(
                                 flags=32,
-                                message="ID must match ^ocd-candidacy/[0-9a-f]{8}-([0-9a-f]{4}-){3}[0-9a-f]{12}$",
+                                message="ID must match ^ocd-candidacy/[0-9a-f]{8}-([0-9a-f]{4}-){3}[0-9a-f]{12}$", # noqa
                                 regex="^ocd-candidacy/[0-9a-f]{8}-([0-9a-f]{4}-){3}[0-9a-f]{12}$",
                             )
                         ],
                     ),
                 ),
                 (
                     "candidate_name",
@@ -227,15 +227,15 @@
                         help_text="Specifies when the candidate filed for the contest.",
                         null=True,
                     ),
                 ),
                 (
                     "is_incumbent",
                     models.NullBooleanField(
-                        help_text="Indicates whether the candidate is seeking re-election to a public office he/she currently holds"
+                        help_text="Indicates whether the candidate is seeking re-election to a public office he/she currently holds" # noqa
                     ),
                 ),
                 (
                     "registration_status",
                     models.CharField(
                         choices=[
                             ("filed", "Filed"),
@@ -300,51 +300,51 @@
                         default=list,
                         size=None,
                     ),
                 ),
                 (
                     "id",
                     opencivicdata.core.models.base.OCDIDField(
-                        help_text="Open Civic Data-style id in the format ``ocd-contest/{{uuid}}``.",
+                        help_text="Open Civic Data-style id in the format ``ocd-contest/{{uuid}}``.", # noqa
                         ocd_type="contest",
                         serialize=False,
                         validators=[
                             django.core.validators.RegexValidator(
                                 flags=32,
-                                message="ID must match ^ocd-contest/[0-9a-f]{8}-([0-9a-f]{4}-){3}[0-9a-f]{12}$",
+                                message="ID must match ^ocd-contest/[0-9a-f]{8}-([0-9a-f]{4}-){3}[0-9a-f]{12}$", # noqa
                                 regex="^ocd-contest/[0-9a-f]{8}-([0-9a-f]{4}-){3}[0-9a-f]{12}$",
                             )
                         ],
                     ),
                 ),
                 (
                     "name",
                     models.CharField(
-                        help_text="Name of the contest, not necessarily as it appears on the ballot.",
+                        help_text="Name of the contest, not necessarily as it appears on the ballot.", # noqa
                         max_length=300,
                     ),
                 ),
                 (
                     "previous_term_unexpired",
                     models.BooleanField(
                         default=False,
-                        help_text="Indicates the previous public office holder vacated the post before serving a full term.",
+                        help_text="Indicates the previous public office holder vacated the post before serving a full term.", # noqa
                     ),
                 ),
                 (
                     "number_elected",
                     models.IntegerField(
                         default=1,
-                        help_text="Number of candidates that are elected in the contest, i.e. 'N' of N-of-M.",
+                        help_text="Number of candidates that are elected in the contest, i.e. 'N' of N-of-M.", # noqa
                     ),
                 ),
                 (
                     "division",
                     models.ForeignKey(
-                        help_text="Reference to the Division that defines the political geography of the contest, e.g., a specific Congressional or State Senate district. Should be a subdivision of the Division referenced by the contest's Election.",
+                        help_text="Reference to the Division that defines the political geography of the contest, e.g., a specific Congressional or State Senate district. Should be a subdivision of the Division referenced by the contest's Election.", # noqa
                         on_delete=django.db.models.deletion.CASCADE,
                         related_name="candidatecontests",
                         related_query_name="candidatecontests",
                         to="core.Division",
                     ),
                 ),
             ],
@@ -363,15 +363,15 @@
                     ),
                 ),
                 ("identifier", models.CharField(max_length=300)),
                 ("scheme", models.CharField(max_length=300)),
                 (
                     "contest",
                     models.ForeignKey(
-                        help_text="Reference to the CandidateContest linked to the upstream identifier.",
+                        help_text="Reference to the CandidateContest linked to the upstream identifier.", # noqa
                         on_delete=django.db.models.deletion.CASCADE,
                         related_name="identifiers",
                         to="elections.CandidateContest",
                     ),
                 ),
             ],
             options={"db_table": "opencivicdata_candidatecontestidentifier"},
@@ -388,21 +388,21 @@
                         verbose_name="ID",
                     ),
                 ),
                 (
                     "sort_order",
                     models.IntegerField(
                         default=0,
-                        help_text="Useful for sorting for contests where two or more public offices are at stake, e.g., in a U.S. presidential contest, the President post would have a lower sort order than the Vice President post.",
+                        help_text="Useful for sorting for contests where two or more public offices are at stake, e.g., in a U.S. presidential contest, the President post would have a lower sort order than the Vice President post.", # noqa
                     ),
                 ),
                 (
                     "contest",
                     models.ForeignKey(
-                        help_text="Reference to the CandidateContest in which the Post is at stake.",
+                        help_text="Reference to the CandidateContest in which the Post is at stake.", # noqa
                         on_delete=django.db.models.deletion.CASCADE,
                         related_name="posts",
                         to="elections.CandidateContest",
                     ),
                 ),
                 (
                     "post",
@@ -464,34 +464,34 @@
                         default=list,
                         size=None,
                     ),
                 ),
                 (
                     "id",
                     opencivicdata.core.models.base.OCDIDField(
-                        help_text="Open Civic Data-style id in the format ``ocd-election/{{uuid}}``.",
+                        help_text="Open Civic Data-style id in the format ``ocd-election/{{uuid}}``.", # noqa
                         ocd_type="election",
                         serialize=False,
                         validators=[
                             django.core.validators.RegexValidator(
                                 flags=32,
-                                message="ID must match ^ocd-election/[0-9a-f]{8}-([0-9a-f]{4}-){3}[0-9a-f]{12}$",
+                                message="ID must match ^ocd-election/[0-9a-f]{8}-([0-9a-f]{4}-){3}[0-9a-f]{12}$", # noqa
                                 regex="^ocd-election/[0-9a-f]{8}-([0-9a-f]{4}-){3}[0-9a-f]{12}$",
                             )
                         ],
                     ),
                 ),
                 (
                     "name",
                     models.CharField(help_text="Name of the Election.", max_length=300),
                 ),
                 (
                     "date",
                     models.DateField(
-                        help_text="Final or only date when eligible voters may cast their ballots in the Election. Typically this is also the same date when results of the election's contests are first publicly reported."
+                        help_text="Final or only date when eligible voters may cast their ballots in the Election. Typically this is also the same date when results of the election's contests are first publicly reported." # noqa
                     ),
                 ),
                 (
                     "administrative_organization",
                     models.ForeignKey(
                         help_text="Reference to the Organization that administers the election.",
                         null=True,
@@ -499,15 +499,15 @@
                         related_name="elections",
                         to="core.Organization",
                     ),
                 ),
                 (
                     "division",
                     models.ForeignKey(
-                        help_text="Reference to the Division that defines the broadest political geography of any contest to be decided by the election.",
+                        help_text="Reference to the Division that defines the broadest political geography of any contest to be decided by the election.", # noqa
                         on_delete=django.db.models.deletion.CASCADE,
                         related_name="elections",
                         to="core.Division",
                     ),
                 ),
             ],
             options={"db_table": "opencivicdata_election", "ordering": ("-date",)},
@@ -582,37 +582,37 @@
                         default=list,
                         size=None,
                     ),
                 ),
                 (
                     "id",
                     opencivicdata.core.models.base.OCDIDField(
-                        help_text="Open Civic Data-style id in the format ``ocd-contest/{{uuid}}``.",
+                        help_text="Open Civic Data-style id in the format ``ocd-contest/{{uuid}}``.", # noqa
                         ocd_type="contest",
                         serialize=False,
                         validators=[
                             django.core.validators.RegexValidator(
                                 flags=32,
-                                message="ID must match ^ocd-contest/[0-9a-f]{8}-([0-9a-f]{4}-){3}[0-9a-f]{12}$",
+                                message="ID must match ^ocd-contest/[0-9a-f]{8}-([0-9a-f]{4}-){3}[0-9a-f]{12}$", # noqa
                                 regex="^ocd-contest/[0-9a-f]{8}-([0-9a-f]{4}-){3}[0-9a-f]{12}$",
                             )
                         ],
                     ),
                 ),
                 (
                     "name",
                     models.CharField(
-                        help_text="Name of the contest, not necessarily as it appears on the ballot.",
+                        help_text="Name of the contest, not necessarily as it appears on the ballot.", # noqa
                         max_length=300,
                     ),
                 ),
                 (
                     "division",
                     models.ForeignKey(
-                        help_text="Reference to the Division that defines the political geography of the contest, e.g., a specific Congressional or State Senate district. Should be a subdivision of the Division referenced by the contest's Election.",
+                        help_text="Reference to the Division that defines the political geography of the contest, e.g., a specific Congressional or State Senate district. Should be a subdivision of the Division referenced by the contest's Election.", # noqa
                         on_delete=django.db.models.deletion.CASCADE,
                         related_name="partycontests",
                         related_query_name="partycontests",
                         to="core.Division",
                     ),
                 ),
                 (
@@ -624,15 +624,15 @@
                         related_query_name="partycontests",
                         to="elections.Election",
                     ),
                 ),
                 (
                     "runoff_for_contest",
                     models.OneToOneField(
-                        help_text="If this contest is a runoff to determine the outcome of a previously undecided contest, reference to that PartyContest.",
+                        help_text="If this contest is a runoff to determine the outcome of a previously undecided contest, reference to that PartyContest.", # noqa
                         null=True,
                         on_delete=django.db.models.deletion.CASCADE,
                         to="elections.PartyContest",
                     ),
                 ),
             ],
             options={"db_table": "opencivicdata_partycontest"},
@@ -650,15 +650,15 @@
                     ),
                 ),
                 ("identifier", models.CharField(max_length=300)),
                 ("scheme", models.CharField(max_length=300)),
                 (
                     "contest",
                     models.ForeignKey(
-                        help_text="Reference to the PartyContest linked to the upstream identifier.",
+                        help_text="Reference to the PartyContest linked to the upstream identifier.", # noqa
                         on_delete=django.db.models.deletion.CASCADE,
                         related_name="identifiers",
                         to="elections.PartyContest",
                     ),
                 ),
             ],
             options={"db_table": "opencivicdata_partyidentifier"},
@@ -750,52 +750,52 @@
                         default=list,
                         size=None,
                     ),
                 ),
                 (
                     "id",
                     opencivicdata.core.models.base.OCDIDField(
-                        help_text="Open Civic Data-style id in the format ``ocd-contest/{{uuid}}``.",
+                        help_text="Open Civic Data-style id in the format ``ocd-contest/{{uuid}}``.", # noqa
                         ocd_type="contest",
                         serialize=False,
                         validators=[
                             django.core.validators.RegexValidator(
                                 flags=32,
-                                message="ID must match ^ocd-contest/[0-9a-f]{8}-([0-9a-f]{4}-){3}[0-9a-f]{12}$",
+                                message="ID must match ^ocd-contest/[0-9a-f]{8}-([0-9a-f]{4}-){3}[0-9a-f]{12}$", # noqa
                                 regex="^ocd-contest/[0-9a-f]{8}-([0-9a-f]{4}-){3}[0-9a-f]{12}$",
                             )
                         ],
                     ),
                 ),
                 (
                     "name",
                     models.CharField(
-                        help_text="Name of the contest, not necessarily as it appears on the ballot.",
+                        help_text="Name of the contest, not necessarily as it appears on the ballot.", # noqa
                         max_length=300,
                     ),
                 ),
                 (
                     "description",
                     models.TextField(
-                        help_text="Text describing the purpose and/or potential outcomes of the contest, not necessarily as it appears on the ballot."
+                        help_text="Text describing the purpose and/or potential outcomes of the contest, not necessarily as it appears on the ballot." # noqa
                     ),
                 ),
                 (
                     "requirement",
                     models.CharField(
                         blank=True,
                         default="50% plus one vote",
-                        help_text="The threshold of votes need in order to retain the officeholder.",
+                        help_text="The threshold of votes need in order to retain the officeholder.", # noqa
                         max_length=300,
                     ),
                 ),
                 (
                     "division",
                     models.ForeignKey(
-                        help_text="Reference to the Division that defines the political geography of the contest, e.g., a specific Congressional or State Senate district. Should be a subdivision of the Division referenced by the contest's Election.",
+                        help_text="Reference to the Division that defines the political geography of the contest, e.g., a specific Congressional or State Senate district. Should be a subdivision of the Division referenced by the contest's Election.", # noqa
                         on_delete=django.db.models.deletion.CASCADE,
                         related_name="retentioncontests",
                         related_query_name="retentioncontests",
                         to="core.Division",
                     ),
                 ),
                 (
@@ -807,23 +807,23 @@
                         related_query_name="retentioncontests",
                         to="elections.Election",
                     ),
                 ),
                 (
                     "membership",
                     models.ForeignKey(
-                        help_text="Reference to the Membership that represents the tenure of a person in a specific public office.",
+                        help_text="Reference to the Membership that represents the tenure of a person in a specific public office.", # noqa
                         on_delete=django.db.models.deletion.CASCADE,
                         to="core.Membership",
                     ),
                 ),
                 (
                     "runoff_for_contest",
                     models.OneToOneField(
-                        help_text="If this contest is a runoff to determine the outcome of a previously undecided contest, reference to that RetentionContest.",
+                        help_text="If this contest is a runoff to determine the outcome of a previously undecided contest, reference to that RetentionContest.", # noqa
                         null=True,
                         on_delete=django.db.models.deletion.CASCADE,
                         related_name="runoff_contest",
                         to="elections.RetentionContest",
                     ),
                 ),
             ],
@@ -842,15 +842,15 @@
                     ),
                 ),
                 ("identifier", models.CharField(max_length=300)),
                 ("scheme", models.CharField(max_length=300)),
                 (
                     "contest",
                     models.ForeignKey(
-                        help_text="Reference to the RetentionContest linked to the upstream identifier.",
+                        help_text="Reference to the RetentionContest linked to the upstream identifier.", # noqa
                         on_delete=django.db.models.deletion.CASCADE,
                         related_name="identifiers",
                         to="elections.RetentionContest",
                     ),
                 ),
             ],
             options={"db_table": "opencivicdata_retentionidentifier"},
@@ -866,15 +866,15 @@
                         serialize=False,
                         verbose_name="ID",
                     ),
                 ),
                 (
                     "text",
                     models.CharField(
-                        help_text="Text of the option, not necessarily as it appears on the ballot.",
+                        help_text="Text of the option, not necessarily as it appears on the ballot.", # noqa
                         max_length=300,
                     ),
                 ),
                 (
                     "contest",
                     models.ForeignKey(
                         help_text="Reference to the RetentionContest.",
@@ -923,37 +923,37 @@
                 to="elections.Election",
             ),
         ),
         migrations.AddField(
             model_name="candidatecontest",
             name="party",
             field=models.ForeignKey(
-                help_text="If the contest is among candidates of the same political party, e.g., a partisan primary election, reference to the Party.",
+                help_text="If the contest is among candidates of the same political party, e.g., a partisan primary election, reference to the Party.", # noqa
                 null=True,
                 on_delete=django.db.models.deletion.CASCADE,
                 related_name="candidate_contests",
                 to="core.Organization",
             ),
         ),
         migrations.AddField(
             model_name="candidatecontest",
             name="runoff_for_contest",
             field=models.OneToOneField(
-                help_text="If this contest is a runoff to determine the outcome of a previously undecided contest, reference to that CandidateContest.",
+                help_text="If this contest is a runoff to determine the outcome of a previously undecided contest, reference to that CandidateContest.", # noqa
                 null=True,
                 on_delete=django.db.models.deletion.CASCADE,
                 related_name="runoff_contest",
                 to="elections.CandidateContest",
             ),
         ),
         migrations.AddField(
             model_name="candidacy",
             name="contest",
             field=models.ForeignKey(
-                help_text="Reference to an OCD CandidateContest representing the contest in which the candidate is competing.",
+                help_text="Reference to an OCD CandidateContest representing the contest in which the candidate is competing.", # noqa
                 on_delete=django.db.models.deletion.CASCADE,
                 related_name="candidacies",
                 to="elections.CandidateContest",
             ),
         ),
         migrations.AddField(
             model_name="candidacy",
@@ -976,25 +976,25 @@
                 to="core.Person",
             ),
         ),
         migrations.AddField(
             model_name="candidacy",
             name="post",
             field=models.ForeignKey(
-                help_text="Reference to Post represents the public office for which the candidate is competing.",
+                help_text="Reference to Post represents the public office for which the candidate is competing.", # noqa
                 on_delete=django.db.models.deletion.CASCADE,
                 related_name="candidacies",
                 to="core.Post",
             ),
         ),
         migrations.AddField(
             model_name="candidacy",
             name="top_ticket_candidacy",
             field=models.ForeignKey(
-                help_text="If the candidate is running as part of ticket, e.g., a Vice Presidential candidate running with a Presidential candidate, reference to candidacy at the top of the ticket.",
+                help_text="If the candidate is running as part of ticket, e.g., a Vice Presidential candidate running with a Presidential candidate, reference to candidacy at the top of the ticket.", # noqa
                 null=True,
                 on_delete=django.db.models.deletion.CASCADE,
                 related_name="ticket",
                 to="elections.Candidacy",
             ),
         ),
         migrations.AddField(
@@ -1008,15 +1008,15 @@
                 to="elections.Election",
             ),
         ),
         migrations.AddField(
             model_name="ballotmeasurecontest",
             name="runoff_for_contest",
             field=models.OneToOneField(
-                help_text="If this contest is a runoff to determine the outcome of a previously undecided contest, reference to that BallotMeasureContest.",
+                help_text="If this contest is a runoff to determine the outcome of a previously undecided contest, reference to that BallotMeasureContest.", # noqa
                 null=True,
                 on_delete=django.db.models.deletion.CASCADE,
                 related_name="runoff_contest",
                 to="elections.BallotMeasureContest",
             ),
         ),
     ]
```

### Comparing `opencivicdata-3.2.0/opencivicdata/elections/migrations/0002_auto_20170731_2047.py` & `opencivicdata-3.3.0/opencivicdata/elections/migrations/0002_auto_20170731_2047.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.2.0/opencivicdata/elections/migrations/0004_field_docs.py` & `opencivicdata-3.3.0/opencivicdata/elections/migrations/0004_field_docs.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         ),
         migrations.AlterField(
             model_name="ballotmeasurecontest",
             name="extras",
             field=django.contrib.postgres.fields.jsonb.JSONField(
                 blank=True,
                 default=dict,
-                help_text="A key-value store for storing arbitrary information not covered elsewhere.",
+                help_text="A key-value store for storing arbitrary information not covered elsewhere.", # noqa
             ),
         ),
         migrations.AlterField(
             model_name="ballotmeasurecontest",
             name="updated_at",
             field=models.DateTimeField(
                 auto_now=True, help_text="The date and time of the last update."
@@ -76,15 +76,15 @@
         ),
         migrations.AlterField(
             model_name="candidacy",
             name="extras",
             field=django.contrib.postgres.fields.jsonb.JSONField(
                 blank=True,
                 default=dict,
-                help_text="A key-value store for storing arbitrary information not covered elsewhere.",
+                help_text="A key-value store for storing arbitrary information not covered elsewhere.", # noqa
             ),
         ),
         migrations.AlterField(
             model_name="candidacy",
             name="updated_at",
             field=models.DateTimeField(
                 auto_now=True, help_text="The date and time of the last update."
@@ -115,15 +115,15 @@
         ),
         migrations.AlterField(
             model_name="candidatecontest",
             name="extras",
             field=django.contrib.postgres.fields.jsonb.JSONField(
                 blank=True,
                 default=dict,
-                help_text="A key-value store for storing arbitrary information not covered elsewhere.",
+                help_text="A key-value store for storing arbitrary information not covered elsewhere.", # noqa
             ),
         ),
         migrations.AlterField(
             model_name="candidatecontest",
             name="updated_at",
             field=models.DateTimeField(
                 auto_now=True, help_text="The date and time of the last update."
@@ -170,15 +170,15 @@
         ),
         migrations.AlterField(
             model_name="election",
             name="extras",
             field=django.contrib.postgres.fields.jsonb.JSONField(
                 blank=True,
                 default=dict,
-                help_text="A key-value store for storing arbitrary information not covered elsewhere.",
+                help_text="A key-value store for storing arbitrary information not covered elsewhere.", # noqa
             ),
         ),
         migrations.AlterField(
             model_name="election",
             name="updated_at",
             field=models.DateTimeField(
                 auto_now=True, help_text="The date and time of the last update."
@@ -245,15 +245,15 @@
         ),
         migrations.AlterField(
             model_name="partycontest",
             name="extras",
             field=django.contrib.postgres.fields.jsonb.JSONField(
                 blank=True,
                 default=dict,
-                help_text="A key-value store for storing arbitrary information not covered elsewhere.",
+                help_text="A key-value store for storing arbitrary information not covered elsewhere.", # noqa
             ),
         ),
         migrations.AlterField(
             model_name="partycontest",
             name="updated_at",
             field=models.DateTimeField(
                 auto_now=True, help_text="The date and time of the last update."
@@ -300,15 +300,15 @@
         ),
         migrations.AlterField(
             model_name="retentioncontest",
             name="extras",
             field=django.contrib.postgres.fields.jsonb.JSONField(
                 blank=True,
                 default=dict,
-                help_text="A key-value store for storing arbitrary information not covered elsewhere.",
+                help_text="A key-value store for storing arbitrary information not covered elsewhere.", # noqa
             ),
         ),
         migrations.AlterField(
             model_name="retentioncontest",
             name="updated_at",
             field=models.DateTimeField(
                 auto_now=True, help_text="The date and time of the last update."
```

### Comparing `opencivicdata-3.2.0/opencivicdata/elections/migrations/0005_auto_20170823_1648.py` & `opencivicdata-3.3.0/opencivicdata/elections/migrations/0006_auto_20171005_2029.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,76 +1,57 @@
 # -*- coding: utf-8 -*-
-# Generated by Django 1.10 on 2017-08-23 16:48
+# Generated by Django 1.11.5 on 2017-10-05 20:29
 from __future__ import unicode_literals
 
 from django.db import migrations, models
 import django.db.models.deletion
 
 
 class Migration(migrations.Migration):
 
-    dependencies = [("elections", "0004_field_docs")]
+    dependencies = [("elections", "0005_auto_20170823_1648")]
 
     operations = [
         migrations.AlterField(
             model_name="candidacy",
             name="party",
             field=models.ForeignKey(
-                help_text="Reference to the Organization representing the political party that nominated the candidate or would nominate the candidate (as in the case of a partisan primary).",
+                help_text="Reference to the Organization representing the political party that nominated the candidate or would nominate the candidate (as in the case of a partisan primary).", # noqa
                 null=True,
-                on_delete=django.db.models.deletion.CASCADE,
+                on_delete=django.db.models.deletion.SET_NULL,
                 related_name="candidacies",
                 to="core.Organization",
             ),
         ),
         migrations.AlterField(
-            model_name="candidacy",
-            name="post",
-            field=models.ForeignKey(
-                help_text="Reference to Post representing the public office for which the candidate is seeking election.",
-                on_delete=django.db.models.deletion.CASCADE,
-                related_name="candidacies",
-                to="core.Post",
-            ),
-        ),
-        migrations.AlterField(
             model_name="candidatecontest",
             name="party",
             field=models.ForeignKey(
-                help_text="If the contest is among candidates of the same political party, e.g., a partisan primary election, reference to the Organization representing that party.",
+                help_text="If the contest is among candidates of the same political party, e.g., a partisan primary election, reference to the Organization representing that party.", # noqa
                 null=True,
-                on_delete=django.db.models.deletion.CASCADE,
+                on_delete=django.db.models.deletion.SET_NULL,
                 related_name="candidate_contests",
                 to="core.Organization",
             ),
         ),
         migrations.AlterField(
-            model_name="candidatecontestpost",
-            name="post",
-            field=models.ForeignKey(
-                help_text="Reference to the Post representing a public office at stake in the CandidateContest.",
-                on_delete=django.db.models.deletion.CASCADE,
-                related_name="contests",
-                to="core.Post",
-            ),
-        ),
-        migrations.AlterField(
-            model_name="partycontestoption",
-            name="contest",
+            model_name="election",
+            name="administrative_organization",
             field=models.ForeignKey(
-                help_text="Reference to the PartyContest in which the party is an option.",
-                on_delete=django.db.models.deletion.CASCADE,
-                related_name="parties",
-                to="elections.PartyContest",
+                help_text="Reference to the Organization that administers the election.",
+                null=True,
+                on_delete=django.db.models.deletion.SET_NULL,
+                related_name="elections",
+                to="core.Organization",
             ),
         ),
         migrations.AlterField(
-            model_name="partycontestoption",
-            name="party",
+            model_name="election",
+            name="division",
             field=models.ForeignKey(
-                help_text="Reference to an Organization representing a political party voters may choose in the contest.",
-                on_delete=django.db.models.deletion.CASCADE,
-                related_name="party_contests",
-                to="core.Organization",
+                help_text="Reference to the Division that defines the broadest political geography of any contest to be decided by the election.", # noqa
+                on_delete=django.db.models.deletion.PROTECT,
+                related_name="elections",
+                to="core.Division",
             ),
         ),
     ]
```

### Comparing `opencivicdata-3.2.0/opencivicdata/elections/migrations/0006_auto_20171005_2029.py` & `opencivicdata-3.3.0/opencivicdata/elections/migrations/0005_auto_20170823_1648.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,57 +1,76 @@
 # -*- coding: utf-8 -*-
-# Generated by Django 1.11.5 on 2017-10-05 20:29
+# Generated by Django 1.10 on 2017-08-23 16:48
 from __future__ import unicode_literals
 
 from django.db import migrations, models
 import django.db.models.deletion
 
 
 class Migration(migrations.Migration):
 
-    dependencies = [("elections", "0005_auto_20170823_1648")]
+    dependencies = [("elections", "0004_field_docs")]
 
     operations = [
         migrations.AlterField(
             model_name="candidacy",
             name="party",
             field=models.ForeignKey(
-                help_text="Reference to the Organization representing the political party that nominated the candidate or would nominate the candidate (as in the case of a partisan primary).",
+                help_text="Reference to the Organization representing the political party that nominated the candidate or would nominate the candidate (as in the case of a partisan primary).", # noqa
                 null=True,
-                on_delete=django.db.models.deletion.SET_NULL,
+                on_delete=django.db.models.deletion.CASCADE,
                 related_name="candidacies",
                 to="core.Organization",
             ),
         ),
         migrations.AlterField(
+            model_name="candidacy",
+            name="post",
+            field=models.ForeignKey(
+                help_text="Reference to Post representing the public office for which the candidate is seeking election.", # noqa
+                on_delete=django.db.models.deletion.CASCADE,
+                related_name="candidacies",
+                to="core.Post",
+            ),
+        ),
+        migrations.AlterField(
             model_name="candidatecontest",
             name="party",
             field=models.ForeignKey(
-                help_text="If the contest is among candidates of the same political party, e.g., a partisan primary election, reference to the Organization representing that party.",
+                help_text="If the contest is among candidates of the same political party, e.g., a partisan primary election, reference to the Organization representing that party.", # noqa
                 null=True,
-                on_delete=django.db.models.deletion.SET_NULL,
+                on_delete=django.db.models.deletion.CASCADE,
                 related_name="candidate_contests",
                 to="core.Organization",
             ),
         ),
         migrations.AlterField(
-            model_name="election",
-            name="administrative_organization",
+            model_name="candidatecontestpost",
+            name="post",
             field=models.ForeignKey(
-                help_text="Reference to the Organization that administers the election.",
-                null=True,
-                on_delete=django.db.models.deletion.SET_NULL,
-                related_name="elections",
-                to="core.Organization",
+                help_text="Reference to the Post representing a public office at stake in the CandidateContest.", # noqa
+                on_delete=django.db.models.deletion.CASCADE,
+                related_name="contests",
+                to="core.Post",
             ),
         ),
         migrations.AlterField(
-            model_name="election",
-            name="division",
+            model_name="partycontestoption",
+            name="contest",
             field=models.ForeignKey(
-                help_text="Reference to the Division that defines the broadest political geography of any contest to be decided by the election.",
-                on_delete=django.db.models.deletion.PROTECT,
-                related_name="elections",
-                to="core.Division",
+                help_text="Reference to the PartyContest in which the party is an option.",
+                on_delete=django.db.models.deletion.CASCADE,
+                related_name="parties",
+                to="elections.PartyContest",
+            ),
+        ),
+        migrations.AlterField(
+            model_name="partycontestoption",
+            name="party",
+            field=models.ForeignKey(
+                help_text="Reference to an Organization representing a political party voters may choose in the contest.", # noqa
+                on_delete=django.db.models.deletion.CASCADE,
+                related_name="party_contests",
+                to="core.Organization",
             ),
         ),
     ]
```

### Comparing `opencivicdata-3.2.0/opencivicdata/elections/migrations/0007_auto_20171022_0234.py` & `opencivicdata-3.3.0/opencivicdata/elections/migrations/0007_auto_20171022_0234.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,121 +11,121 @@
     dependencies = [("elections", "0006_auto_20171005_2029")]
 
     operations = [
         migrations.AlterField(
             model_name="ballotmeasurecontest",
             name="division",
             field=models.ForeignKey(
-                help_text="Reference to the Division that defines the political geography of the contest, e.g., a specific Congressional or State Senate district. Should be a subdivision of the Division referenced by the contest's Election.",
+                help_text="Reference to the Division that defines the political geography of the contest, e.g., a specific Congressional or State Senate district. Should be a subdivision of the Division referenced by the contest's Election.", # noqa
                 on_delete=django.db.models.deletion.PROTECT,
                 related_name="ballotmeasurecontests",
                 related_query_name="ballotmeasurecontests",
                 to="core.Division",
             ),
         ),
         migrations.AlterField(
             model_name="ballotmeasurecontest",
             name="runoff_for_contest",
             field=models.OneToOneField(
-                help_text="If this contest is a runoff to determine the outcome of a previously undecided contest, reference to that BallotMeasureContest.",
+                help_text="If this contest is a runoff to determine the outcome of a previously undecided contest, reference to that BallotMeasureContest.", # noqa
                 null=True,
                 on_delete=django.db.models.deletion.SET_NULL,
                 related_name="runoff_contest",
                 to="elections.BallotMeasureContest",
             ),
         ),
         migrations.AlterField(
             model_name="candidacy",
             name="post",
             field=models.ForeignKey(
-                help_text="Reference to Post representing the public office for which the candidate is seeking election.",
+                help_text="Reference to Post representing the public office for which the candidate is seeking election.", # noqa
                 on_delete=django.db.models.deletion.PROTECT,
                 related_name="candidacies",
                 to="core.Post",
             ),
         ),
         migrations.AlterField(
             model_name="candidacy",
             name="top_ticket_candidacy",
             field=models.ForeignKey(
-                help_text="If the candidate is running as part of ticket, e.g., a Vice Presidential candidate running with a Presidential candidate, reference to candidacy at the top of the ticket.",
+                help_text="If the candidate is running as part of ticket, e.g., a Vice Presidential candidate running with a Presidential candidate, reference to candidacy at the top of the ticket.", # noqa
                 null=True,
                 on_delete=django.db.models.deletion.SET_NULL,
                 related_name="ticket",
                 to="elections.Candidacy",
             ),
         ),
         migrations.AlterField(
             model_name="candidatecontest",
             name="division",
             field=models.ForeignKey(
-                help_text="Reference to the Division that defines the political geography of the contest, e.g., a specific Congressional or State Senate district. Should be a subdivision of the Division referenced by the contest's Election.",
+                help_text="Reference to the Division that defines the political geography of the contest, e.g., a specific Congressional or State Senate district. Should be a subdivision of the Division referenced by the contest's Election.", # noqa
                 on_delete=django.db.models.deletion.PROTECT,
                 related_name="candidatecontests",
                 related_query_name="candidatecontests",
                 to="core.Division",
             ),
         ),
         migrations.AlterField(
             model_name="candidatecontest",
             name="runoff_for_contest",
             field=models.OneToOneField(
-                help_text="If this contest is a runoff to determine the outcome of a previously undecided contest, reference to that CandidateContest.",
+                help_text="If this contest is a runoff to determine the outcome of a previously undecided contest, reference to that CandidateContest.", # noqa
                 null=True,
                 on_delete=django.db.models.deletion.SET_NULL,
                 related_name="runoff_contest",
                 to="elections.CandidateContest",
             ),
         ),
         migrations.AlterField(
             model_name="partycontest",
             name="division",
             field=models.ForeignKey(
-                help_text="Reference to the Division that defines the political geography of the contest, e.g., a specific Congressional or State Senate district. Should be a subdivision of the Division referenced by the contest's Election.",
+                help_text="Reference to the Division that defines the political geography of the contest, e.g., a specific Congressional or State Senate district. Should be a subdivision of the Division referenced by the contest's Election.", # noqa
                 on_delete=django.db.models.deletion.PROTECT,
                 related_name="partycontests",
                 related_query_name="partycontests",
                 to="core.Division",
             ),
         ),
         migrations.AlterField(
             model_name="partycontest",
             name="runoff_for_contest",
             field=models.OneToOneField(
-                help_text="If this contest is a runoff to determine the outcome of a previously undecided contest, reference to that PartyContest.",
+                help_text="If this contest is a runoff to determine the outcome of a previously undecided contest, reference to that PartyContest.", # noqa
                 null=True,
                 on_delete=django.db.models.deletion.SET_NULL,
                 to="elections.PartyContest",
             ),
         ),
         migrations.AlterField(
             model_name="retentioncontest",
             name="division",
             field=models.ForeignKey(
-                help_text="Reference to the Division that defines the political geography of the contest, e.g., a specific Congressional or State Senate district. Should be a subdivision of the Division referenced by the contest's Election.",
+                help_text="Reference to the Division that defines the political geography of the contest, e.g., a specific Congressional or State Senate district. Should be a subdivision of the Division referenced by the contest's Election.", # noqa
                 on_delete=django.db.models.deletion.PROTECT,
                 related_name="retentioncontests",
                 related_query_name="retentioncontests",
                 to="core.Division",
             ),
         ),
         migrations.AlterField(
             model_name="retentioncontest",
             name="membership",
             field=models.ForeignKey(
-                help_text="Reference to the Membership that represents the tenure of a person in a specific public office.",
+                help_text="Reference to the Membership that represents the tenure of a person in a specific public office.", # noqa
                 on_delete=django.db.models.deletion.PROTECT,
                 to="core.Membership",
             ),
         ),
         migrations.AlterField(
             model_name="retentioncontest",
             name="runoff_for_contest",
             field=models.OneToOneField(
-                help_text="If this contest is a runoff to determine the outcome of a previously undecided contest, reference to that RetentionContest.",
+                help_text="If this contest is a runoff to determine the outcome of a previously undecided contest, reference to that RetentionContest.", # noqa
                 null=True,
                 on_delete=django.db.models.deletion.SET_NULL,
                 related_name="runoff_contest",
                 to="elections.RetentionContest",
             ),
         ),
     ]
```

### Comparing `opencivicdata-3.2.0/opencivicdata/elections/migrations/0008_auto_20181029_1527.py` & `opencivicdata-3.3.0/opencivicdata/elections/migrations/0008_auto_20181029_1527.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,39 +9,39 @@
     dependencies = [("elections", "0007_auto_20171022_0234")]
 
     operations = [
         migrations.AlterField(
             model_name="candidacy",
             name="party",
             field=models.ForeignKey(
-                help_text="Reference to the Organization representing the political party that nominated the candidate or would nominate the candidate (as in the case of a partisan primary).",
+                help_text="Reference to the Organization representing the political party that nominated the candidate or would nominate the candidate (as in the case of a partisan primary).", # noqa
                 limit_choices_to={"classification": "party"},
                 null=True,
                 on_delete=django.db.models.deletion.SET_NULL,
                 related_name="candidacies",
                 to="core.Organization",
             ),
         ),
         migrations.AlterField(
             model_name="candidatecontest",
             name="party",
             field=models.ForeignKey(
-                help_text="If the contest is among candidates of the same political party, e.g., a partisan primary election, reference to the Organization representing that party.",
+                help_text="If the contest is among candidates of the same political party, e.g., a partisan primary election, reference to the Organization representing that party.", # noqa
                 limit_choices_to={"classification": "party"},
                 null=True,
                 on_delete=django.db.models.deletion.SET_NULL,
                 related_name="candidate_contests",
                 to="core.Organization",
             ),
         ),
         migrations.AlterField(
             model_name="partycontestoption",
             name="party",
             field=models.ForeignKey(
-                help_text="Reference to an Organization representing a political party voters may choose in the contest.",
+                help_text="Reference to an Organization representing a political party voters may choose in the contest.", # noqa
                 limit_choices_to={"classification": "party"},
                 on_delete=django.db.models.deletion.CASCADE,
                 related_name="party_contests",
                 to="core.Organization",
             ),
         ),
     ]
```

### Comparing `opencivicdata-3.2.0/opencivicdata/elections/models/__init__.py` & `opencivicdata-3.3.0/opencivicdata/elections/models/__init__.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.2.0/opencivicdata/elections/models/candidacy.py` & `opencivicdata-3.3.0/opencivicdata/elections/models/candidacy.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.2.0/opencivicdata/elections/models/contests/ballot_measure.py` & `opencivicdata-3.3.0/opencivicdata/elections/models/contests/ballot_measure.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.2.0/opencivicdata/elections/models/contests/base.py` & `opencivicdata-3.3.0/opencivicdata/elections/models/contests/base.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.2.0/opencivicdata/elections/models/contests/candidate.py` & `opencivicdata-3.3.0/opencivicdata/elections/models/contests/candidate.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.2.0/opencivicdata/elections/models/contests/party.py` & `opencivicdata-3.3.0/opencivicdata/elections/models/contests/party.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.2.0/opencivicdata/elections/models/election.py` & `opencivicdata-3.3.0/opencivicdata/elections/models/election.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.2.0/opencivicdata/legislative/admin/bill.py` & `opencivicdata-3.3.0/opencivicdata/legislative/admin/bill.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.2.0/opencivicdata/legislative/admin/event.py` & `opencivicdata-3.3.0/opencivicdata/legislative/admin/event.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.2.0/opencivicdata/legislative/admin/vote.py` & `opencivicdata-3.3.0/opencivicdata/legislative/admin/vote.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.2.0/opencivicdata/legislative/migrations/0001_initial.py` & `opencivicdata-3.3.0/opencivicdata/legislative/migrations/0001_initial.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
                     "id",
                     opencivicdata.core.models.base.OCDIDField(
                         ocd_type="bill",
                         serialize=False,
                         validators=[
                             django.core.validators.RegexValidator(
                                 flags=32,
-                                message="ID must match ^ocd-bill/[0-9a-f]{8}-([0-9a-f]{4}-){3}[0-9a-f]{12}$",
+                                message="ID must match ^ocd-bill/[0-9a-f]{8}-([0-9a-f]{4}-){3}[0-9a-f]{12}$", # noqa
                                 regex="^ocd-bill/[0-9a-f]{8}-([0-9a-f]{4}-){3}[0-9a-f]{12}$",
                             )
                         ],
                     ),
                 ),
                 ("identifier", models.CharField(max_length=100)),
                 ("title", models.TextField()),
@@ -440,15 +440,15 @@
                     "id",
                     opencivicdata.core.models.base.OCDIDField(
                         ocd_type="event",
                         serialize=False,
                         validators=[
                             django.core.validators.RegexValidator(
                                 flags=32,
-                                message="ID must match ^ocd-event/[0-9a-f]{8}-([0-9a-f]{4}-){3}[0-9a-f]{12}$",
+                                message="ID must match ^ocd-event/[0-9a-f]{8}-([0-9a-f]{4}-){3}[0-9a-f]{12}$", # noqa
                                 regex="^ocd-event/[0-9a-f]{8}-([0-9a-f]{4}-){3}[0-9a-f]{12}$",
                             )
                         ],
                     ),
                 ),
                 ("name", models.CharField(max_length=300)),
                 ("description", models.TextField()),
@@ -1033,15 +1033,15 @@
                     "id",
                     opencivicdata.core.models.base.OCDIDField(
                         ocd_type="vote",
                         serialize=False,
                         validators=[
                             django.core.validators.RegexValidator(
                                 flags=32,
-                                message="ID must match ^ocd-vote/[0-9a-f]{8}-([0-9a-f]{4}-){3}[0-9a-f]{12}$",
+                                message="ID must match ^ocd-vote/[0-9a-f]{8}-([0-9a-f]{4}-){3}[0-9a-f]{12}$", # noqa
                                 regex="^ocd-vote/[0-9a-f]{8}-([0-9a-f]{4}-){3}[0-9a-f]{12}$",
                             )
                         ],
                     ),
                 ),
                 ("identifier", models.CharField(blank=True, max_length=300)),
                 ("motion_text", models.TextField()),
```

### Comparing `opencivicdata-3.2.0/opencivicdata/legislative/migrations/0002_more_extras.py` & `opencivicdata-3.3.0/opencivicdata/legislative/migrations/0002_more_extras.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.2.0/opencivicdata/legislative/migrations/0003_time_changes.py` & `opencivicdata-3.3.0/opencivicdata/legislative/migrations/0003_time_changes.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.2.0/opencivicdata/legislative/migrations/0004_auto_20171005_2027.py` & `opencivicdata-3.3.0/opencivicdata/legislative/migrations/0004_auto_20171005_2027.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         ),
         migrations.AlterField(
             model_name="bill",
             name="extras",
             field=django.contrib.postgres.fields.jsonb.JSONField(
                 blank=True,
                 default=dict,
-                help_text="A key-value store for storing arbitrary information not covered elsewhere.",
+                help_text="A key-value store for storing arbitrary information not covered elsewhere.", # noqa
             ),
         ),
         migrations.AlterField(
             model_name="bill",
             name="updated_at",
             field=models.DateTimeField(
                 auto_now=True, help_text="The date and time of the last update."
@@ -75,15 +75,15 @@
         ),
         migrations.AlterField(
             model_name="event",
             name="extras",
             field=django.contrib.postgres.fields.jsonb.JSONField(
                 blank=True,
                 default=dict,
-                help_text="A key-value store for storing arbitrary information not covered elsewhere.",
+                help_text="A key-value store for storing arbitrary information not covered elsewhere.", # noqa
             ),
         ),
         migrations.AlterField(
             model_name="event",
             name="updated_at",
             field=models.DateTimeField(
                 auto_now=True, help_text="The date and time of the last update."
@@ -130,15 +130,15 @@
         ),
         migrations.AlterField(
             model_name="voteevent",
             name="extras",
             field=django.contrib.postgres.fields.jsonb.JSONField(
                 blank=True,
                 default=dict,
-                help_text="A key-value store for storing arbitrary information not covered elsewhere.",
+                help_text="A key-value store for storing arbitrary information not covered elsewhere.", # noqa
             ),
         ),
         migrations.AlterField(
             model_name="voteevent",
             name="updated_at",
             field=models.DateTimeField(
                 auto_now=True, help_text="The date and time of the last update."
```

### Comparing `opencivicdata-3.2.0/opencivicdata/legislative/migrations/0005_auto_20171005_2028.py` & `opencivicdata-3.3.0/opencivicdata/legislative/migrations/0005_auto_20171005_2028.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.2.0/opencivicdata/legislative/migrations/0009_searchablebill.py` & `opencivicdata-3.3.0/opencivicdata/legislative/migrations/0009_searchablebill.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.2.0/opencivicdata/legislative/migrations/0010_auto_20191031_1507.py` & `opencivicdata-3.3.0/opencivicdata/legislative/migrations/0010_auto_20191031_1507.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.2.0/opencivicdata/legislative/migrations/0011_auto_20191124_1658.py` & `opencivicdata-3.3.0/opencivicdata/legislative/migrations/0011_auto_20191124_1658.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.2.0/opencivicdata/legislative/models/__init__.py` & `opencivicdata-3.3.0/opencivicdata/legislative/models/__init__.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.2.0/opencivicdata/legislative/models/bill.py` & `opencivicdata-3.3.0/opencivicdata/legislative/models/bill.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.2.0/opencivicdata/legislative/models/event.py` & `opencivicdata-3.3.0/opencivicdata/legislative/models/event.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.2.0/opencivicdata/legislative/models/session.py` & `opencivicdata-3.3.0/opencivicdata/legislative/models/session.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.2.0/opencivicdata/legislative/models/vote.py` & `opencivicdata-3.3.0/opencivicdata/legislative/models/vote.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.2.0/opencivicdata/tests/conftest.py` & `opencivicdata-3.3.0/opencivicdata/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.2.0/opencivicdata/tests/test_elections.py` & `opencivicdata-3.3.0/opencivicdata/tests/test_elections.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.2.0/opencivicdata/tests/test_loaddivisions.py` & `opencivicdata-3.3.0/opencivicdata/tests/test_loaddivisions.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,50 @@
+import os
+
 import pytest
 from django.core.management import call_command
+
+from opencivicdata.divisions import Division as FileDivision
 from opencivicdata.core.models import Division
 
 
 @pytest.mark.django_db
-def test_loaddivisions():
+def test_loaddivisions(capsys):
     assert Division.objects.count() == 0
+
     call_command("loaddivisions", "in")
+
     assert Division.objects.count() > 0
     assert Division.objects.count() == Division.objects.filter(country="in").count()
     assert (
         Division.objects.filter(country="in", subtype1="state", subtype2="").count()
         == 29
     )
 
     # Include a (very weak) check for idempotency
     call_command("loaddivisions", "in")
+
     assert (
         Division.objects.filter(country="in", subtype1="state", subtype2="").count()
         == 29
     )
+
+    # The FileDivision's cache is a mutable class attribute, which is shared
+    # between instances. Reset it, so calling the command with a CSV specified
+    # does not use divisions cached from previous runs.
+    FileDivision._cache = {}
+
+    test_dir = os.path.abspath(os.path.dirname(__file__))
+    os.environ["OCD_DIVISION_CSV"] = os.path.join(
+        test_dir, "fixtures", "country-in-subset.csv"
+    )
+
+    call_command("loaddivisions", "in")
+
+    out, _ = capsys.readouterr()
+    last_message = out.splitlines()[-1]
+
+    assert last_message == "The DB contains all CSV contents; no work to be done!"
+
+    # Unset the CSV environment variable so subsequent division tests reload
+    # divisions from source instead of breaking.
+    os.environ.pop("OCD_DIVISION_CSV")
```

### Comparing `opencivicdata-3.2.0/opencivicdata/tests/test_models.py` & `opencivicdata-3.3.0/opencivicdata/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.2.0/opencivicdata.egg-info/PKG-INFO` & `opencivicdata-3.3.0/opencivicdata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opencivicdata
-Version: 3.2.0
+Version: 3.3.0
 Summary: python opencivicdata library
 Home-page: UNKNOWN
 Author: James Turk
 Author-email: james@openstates.org
 License: BSD
 Description: UNKNOWN
 Platform: any
```

### Comparing `opencivicdata-3.2.0/opencivicdata.egg-info/SOURCES.txt` & `opencivicdata-3.3.0/opencivicdata.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -23,14 +23,16 @@
 opencivicdata/core/migrations/0001_initial.py
 opencivicdata/core/migrations/0002_post_maximum_memberships.py
 opencivicdata/core/migrations/0003_field_docs.py
 opencivicdata/core/migrations/0004_auto_20171005_2028.py
 opencivicdata/core/migrations/0005_auto_20191031_1507.py
 opencivicdata/core/migrations/0005_auto_20191124_1658.py
 opencivicdata/core/migrations/0006_merge_20200103_1432.py
+opencivicdata/core/migrations/0007_jurisdiction_last_seen_membership_last_seen_and_more.py
+opencivicdata/core/migrations/0008_auto_20221215_1132.py
 opencivicdata/core/migrations/__init__.py
 opencivicdata/core/models/__init__.py
 opencivicdata/core/models/base.py
 opencivicdata/core/models/division.py
 opencivicdata/core/models/jurisdiction.py
 opencivicdata/core/models/people_orgs.py
 opencivicdata/elections/__init__.py
@@ -46,14 +48,16 @@
 opencivicdata/elections/migrations/0002_auto_20170731_2047.py
 opencivicdata/elections/migrations/0003_election_fk.py
 opencivicdata/elections/migrations/0004_field_docs.py
 opencivicdata/elections/migrations/0005_auto_20170823_1648.py
 opencivicdata/elections/migrations/0006_auto_20171005_2029.py
 opencivicdata/elections/migrations/0007_auto_20171022_0234.py
 opencivicdata/elections/migrations/0008_auto_20181029_1527.py
+opencivicdata/elections/migrations/0009_auto_20221208_1041.py
+opencivicdata/elections/migrations/0010_auto_20221215_1132.py
 opencivicdata/elections/migrations/__init__.py
 opencivicdata/elections/models/__init__.py
 opencivicdata/elections/models/candidacy.py
 opencivicdata/elections/models/election.py
 opencivicdata/elections/models/contests/__init__.py
 opencivicdata/elections/models/contests/ballot_measure.py
 opencivicdata/elections/models/contests/base.py
@@ -74,14 +78,16 @@
 opencivicdata/legislative/migrations/0007_auto_20181029_1527.py
 opencivicdata/legislative/migrations/0008_longer_event_name.py
 opencivicdata/legislative/migrations/0009_searchablebill.py
 opencivicdata/legislative/migrations/0010_auto_20191031_1507.py
 opencivicdata/legislative/migrations/0011_auto_20191124_1658.py
 opencivicdata/legislative/migrations/0012_billdocument_extras.py
 opencivicdata/legislative/migrations/0013_auto_20200326_0458.py
+opencivicdata/legislative/migrations/0014_bill_last_seen_event_last_seen_voteevent_last_seen.py
+opencivicdata/legislative/migrations/0015_auto_20221215_1132.py
 opencivicdata/legislative/migrations/__init__.py
 opencivicdata/legislative/models/__init__.py
 opencivicdata/legislative/models/bill.py
 opencivicdata/legislative/models/event.py
 opencivicdata/legislative/models/session.py
 opencivicdata/legislative/models/vote.py
 opencivicdata/tests/__init__.py
```

### Comparing `opencivicdata-3.2.0/setup.py` & `opencivicdata-3.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 #!/usr/bin/env python
 from setuptools import setup, find_packages
 
 install_requires = ["Django>=2.2", "psycopg2-binary"]
 
 extras_require = {
-    "dev": ["pytest>=3.6", "pytest-cov", "pytest-django", "coveralls", "flake8"]
+    "dev": ["pytest>=3.6", "pytest-cov", "pytest-django", "coveralls==3.2.0", "flake8"]
 }
 
-
 setup(
     name="opencivicdata",
-    version="3.2.0",
+    version="3.3.0",
     author="James Turk",
     author_email="james@openstates.org",
     license="BSD",
     description="python opencivicdata library",
     long_description="",
     url="",
     packages=find_packages(),
```

