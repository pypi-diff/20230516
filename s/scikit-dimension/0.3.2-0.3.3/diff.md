# Comparing `tmp/scikit-dimension-0.3.2.tar.gz` & `tmp/scikit-dimension-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/scikit-dimension-0.3.2.tar", last modified: Sun Jul 31 08:27:04 2022, max compression
+gzip compressed data, was "scikit-dimension-0.3.3.tar", last modified: Tue May 16 20:34:24 2023, max compression
```

## Comparing `scikit-dimension-0.3.2.tar` & `scikit-dimension-0.3.3.tar`

### file list

```diff
@@ -1,246 +1,39 @@
-drwxrwxrwx   0 jo        (1000) jo        (1000)        0 2022-07-31 08:27:04.000000 scikit-dimension-0.3.2/
-drwxrwxrwx   0 jo        (1000) jo        (1000)        0 2022-07-31 08:26:42.000000 scikit-dimension-0.3.2/.circleci/
--rwxrwxrwx   0 jo        (1000) jo        (1000)     1454 2022-02-25 09:29:36.000000 scikit-dimension-0.3.2/.circleci/config.yml
--rwxrwxrwx   0 jo        (1000) jo        (1000)      351 2020-08-20 14:04:35.000000 scikit-dimension-0.3.2/.coveragerc
-drwxrwxrwx   0 jo        (1000) jo        (1000)        0 2022-07-31 08:26:42.000000 scikit-dimension-0.3.2/.github/
-drwxrwxrwx   0 jo        (1000) jo        (1000)        0 2022-07-31 08:26:42.000000 scikit-dimension-0.3.2/.github/workflows/
--rwxrwxrwx   0 jo        (1000) jo        (1000)      934 2022-07-30 22:00:55.000000 scikit-dimension-0.3.2/.github/workflows/python-publish.yml
--rwxrwxrwx   0 jo        (1000) jo        (1000)      873 2020-08-22 09:25:42.000000 scikit-dimension-0.3.2/.gitignore
--rwxrwxrwx   0 jo        (1000) jo        (1000)      221 2020-12-08 09:33:41.000000 scikit-dimension-0.3.2/.readthedocs.yml
--rwxrwxrwx   0 jo        (1000) jo        (1000)     1857 2020-12-09 09:41:21.000000 scikit-dimension-0.3.2/.travis.yml
--rwxrwxrwx   0 jo        (1000) jo        (1000)     1520 2020-08-20 14:04:35.000000 scikit-dimension-0.3.2/LICENSE
--rwxrwxrwx   0 jo        (1000) jo        (1000)       25 2020-08-20 14:04:35.000000 scikit-dimension-0.3.2/MANIFEST.in
--rwxrwxrwx   0 jo        (1000) jo        (1000)      901 2022-07-31 08:27:04.000000 scikit-dimension-0.3.2/PKG-INFO
--rwxrwxrwx   0 jo        (1000) jo        (1000)     2456 2022-07-30 22:00:55.000000 scikit-dimension-0.3.2/README.md
--rwxrwxrwx   0 jo        (1000) jo        (1000)     1236 2021-01-02 11:34:44.000000 scikit-dimension-0.3.2/appveyor.yml
-drwxrwxrwx   0 jo        (1000) jo        (1000)        0 2022-07-31 08:27:00.000000 scikit-dimension-0.3.2/doc/
--rwxrwxrwx   0 jo        (1000) jo        (1000)     7037 2020-08-20 14:04:35.000000 scikit-dimension-0.3.2/doc/Makefile
-drwxrwxrwx   0 jo        (1000) jo        (1000)        0 2022-07-31 08:26:42.000000 scikit-dimension-0.3.2/doc/_static/
-drwxrwxrwx   0 jo        (1000) jo        (1000)        0 2022-07-31 08:27:00.000000 scikit-dimension-0.3.2/doc/_static/css/
--rwxrwxrwx   0 jo        (1000) jo        (1000)     4315 2020-12-08 10:36:38.000000 scikit-dimension-0.3.2/doc/_static/css/custom.css
--rwxrwxrwx   0 jo        (1000) jo        (1000)      273 2020-08-20 14:04:35.000000 scikit-dimension-0.3.2/doc/_static/css/project-template.css
-drwxrwxrwx   0 jo        (1000) jo        (1000)        0 2022-07-31 08:26:42.000000 scikit-dimension-0.3.2/doc/_templates/
-drwxrwxrwx   0 jo        (1000) jo        (1000)        0 2022-07-31 08:27:00.000000 scikit-dimension-0.3.2/doc/_templates/autosummary/
--rwxrwxrwx   0 jo        (1000) jo        (1000)      194 2021-01-02 16:48:02.000000 scikit-dimension-0.3.2/doc/_templates/autosummary/base.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      690 2021-01-03 14:51:52.000000 scikit-dimension-0.3.2/doc/_templates/autosummary/class.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      516 2020-12-09 10:07:12.000000 scikit-dimension-0.3.2/doc/api.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)  8170155 2021-06-07 23:48:28.000000 scikit-dimension-0.3.2/doc/basics.ipynb
--rwxrwxrwx   0 jo        (1000) jo        (1000)    17067 2021-01-03 11:24:58.000000 scikit-dimension-0.3.2/doc/conf.py
--rwxrwxrwx   0 jo        (1000) jo        (1000)     4966 2020-12-30 16:25:19.000000 scikit-dimension-0.3.2/doc/contributing.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000) 11416917 2021-03-08 21:33:32.000000 scikit-dimension-0.3.2/doc/detailed_usage.ipynb
--rwxrwxrwx   0 jo        (1000) jo        (1000)     3855 2020-12-30 18:13:53.000000 scikit-dimension-0.3.2/doc/index.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)     1018 2021-01-13 16:35:38.000000 scikit-dimension-0.3.2/doc/installation.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)     6721 2020-07-09 16:08:29.000000 scikit-dimension-0.3.2/doc/make.bat
--rwxrwxrwx   0 jo        (1000) jo        (1000)      819 2021-04-21 15:44:19.000000 scikit-dimension-0.3.2/doc/quick_start.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)     3859 2021-01-03 15:22:35.000000 scikit-dimension-0.3.2/doc/references.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      288 2021-04-21 19:26:06.000000 scikit-dimension-0.3.2/doc/release_notes.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      198 2022-02-25 09:29:36.000000 scikit-dimension-0.3.2/doc/requirements.txt
--rwxrwxrwx   0 jo        (1000) jo        (1000)      280 2021-04-21 18:10:34.000000 scikit-dimension-0.3.2/doc/skdim.datasets.BenchmarkManifolds.generate.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      341 2021-04-21 18:10:34.000000 scikit-dimension-0.3.2/doc/skdim.datasets.BenchmarkManifolds.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      226 2021-04-21 18:10:34.000000 scikit-dimension-0.3.2/doc/skdim.datasets.hyperBall.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      232 2021-04-21 18:10:35.000000 scikit-dimension-0.3.2/doc/skdim.datasets.hyperSphere.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      242 2021-04-21 18:10:35.000000 scikit-dimension-0.3.2/doc/skdim.datasets.hyperTwinPeaks.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      237 2021-04-21 18:10:35.000000 scikit-dimension-0.3.2/doc/skdim.datasets.lineDiskBall.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      240 2021-04-21 18:10:35.000000 scikit-dimension-0.3.2/doc/skdim.datasets.swissRoll3Sph.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      215 2021-04-21 18:10:35.000000 scikit-dimension-0.3.2/doc/skdim.id.CorrInt.fit.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      236 2021-01-02 16:58:50.000000 scikit-dimension-0.3.2/doc/skdim.id.CorrInt.fit_predict.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      247 2021-01-02 16:58:50.000000 scikit-dimension-0.3.2/doc/skdim.id.CorrInt.fit_predict_pw.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      228 2021-04-21 18:10:35.000000 scikit-dimension-0.3.2/doc/skdim.id.CorrInt.fit_pw.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      249 2021-04-21 18:10:40.000000 scikit-dimension-0.3.2/doc/skdim.id.CorrInt.fit_transform.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      260 2021-04-21 18:10:40.000000 scikit-dimension-0.3.2/doc/skdim.id.CorrInt.fit_transform_pw.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      240 2021-04-21 18:10:35.000000 scikit-dimension-0.3.2/doc/skdim.id.CorrInt.get_params.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      222 2021-01-02 16:58:50.000000 scikit-dimension-0.3.2/doc/skdim.id.CorrInt.predict.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      233 2021-01-02 16:58:50.000000 scikit-dimension-0.3.2/doc/skdim.id.CorrInt.predict_pw.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      519 2021-04-21 18:10:35.000000 scikit-dimension-0.3.2/doc/skdim.id.CorrInt.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      240 2021-04-21 18:10:35.000000 scikit-dimension-0.3.2/doc/skdim.id.CorrInt.set_params.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      235 2021-04-21 18:10:40.000000 scikit-dimension-0.3.2/doc/skdim.id.CorrInt.transform.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      246 2021-04-21 18:10:40.000000 scikit-dimension-0.3.2/doc/skdim.id.CorrInt.transform_pw.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      208 2021-04-21 18:10:35.000000 scikit-dimension-0.3.2/doc/skdim.id.DANCo.fit.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      228 2021-01-02 16:58:50.000000 scikit-dimension-0.3.2/doc/skdim.id.DANCo.fit_predict.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      239 2021-01-02 16:58:50.000000 scikit-dimension-0.3.2/doc/skdim.id.DANCo.fit_predict_pw.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      220 2021-04-21 18:10:35.000000 scikit-dimension-0.3.2/doc/skdim.id.DANCo.fit_pw.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      241 2021-04-21 18:10:40.000000 scikit-dimension-0.3.2/doc/skdim.id.DANCo.fit_transform.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      252 2021-04-21 18:10:40.000000 scikit-dimension-0.3.2/doc/skdim.id.DANCo.fit_transform_pw.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      232 2021-04-21 18:10:35.000000 scikit-dimension-0.3.2/doc/skdim.id.DANCo.get_params.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      214 2021-01-02 16:58:50.000000 scikit-dimension-0.3.2/doc/skdim.id.DANCo.predict.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      225 2021-01-02 16:58:50.000000 scikit-dimension-0.3.2/doc/skdim.id.DANCo.predict_pw.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      497 2021-04-21 18:10:35.000000 scikit-dimension-0.3.2/doc/skdim.id.DANCo.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      232 2021-04-21 18:10:35.000000 scikit-dimension-0.3.2/doc/skdim.id.DANCo.set_params.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      227 2021-04-21 18:10:40.000000 scikit-dimension-0.3.2/doc/skdim.id.DANCo.transform.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      238 2021-04-21 18:10:40.000000 scikit-dimension-0.3.2/doc/skdim.id.DANCo.transform_pw.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      201 2021-04-21 18:10:35.000000 scikit-dimension-0.3.2/doc/skdim.id.ESS.fit.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      217 2021-04-21 18:10:35.000000 scikit-dimension-0.3.2/doc/skdim.id.ESS.fit_once.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      220 2021-01-02 16:58:50.000000 scikit-dimension-0.3.2/doc/skdim.id.ESS.fit_predict.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      231 2021-01-02 16:58:50.000000 scikit-dimension-0.3.2/doc/skdim.id.ESS.fit_predict_pw.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      233 2021-04-21 18:10:41.000000 scikit-dimension-0.3.2/doc/skdim.id.ESS.fit_transform.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      244 2021-04-21 18:10:41.000000 scikit-dimension-0.3.2/doc/skdim.id.ESS.fit_transform_pw.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      224 2021-04-21 18:10:36.000000 scikit-dimension-0.3.2/doc/skdim.id.ESS.get_params.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      206 2021-01-02 16:58:51.000000 scikit-dimension-0.3.2/doc/skdim.id.ESS.predict.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      217 2021-01-02 16:58:51.000000 scikit-dimension-0.3.2/doc/skdim.id.ESS.predict_pw.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      477 2021-04-21 18:10:35.000000 scikit-dimension-0.3.2/doc/skdim.id.ESS.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      224 2021-04-21 18:10:36.000000 scikit-dimension-0.3.2/doc/skdim.id.ESS.set_params.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      219 2021-04-21 18:10:41.000000 scikit-dimension-0.3.2/doc/skdim.id.ESS.transform.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      230 2021-04-21 18:10:41.000000 scikit-dimension-0.3.2/doc/skdim.id.ESS.transform_pw.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      274 2021-04-21 18:10:36.000000 scikit-dimension-0.3.2/doc/skdim.id.FisherS.buildSeparabilityGraph.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      255 2021-04-21 18:10:36.000000 scikit-dimension-0.3.2/doc/skdim.id.FisherS.check_symmetric.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      216 2021-04-21 18:10:36.000000 scikit-dimension-0.3.2/doc/skdim.id.FisherS.fit.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      236 2021-01-02 16:58:51.000000 scikit-dimension-0.3.2/doc/skdim.id.FisherS.fit_predict.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      247 2021-01-02 16:58:51.000000 scikit-dimension-0.3.2/doc/skdim.id.FisherS.fit_predict_pw.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      228 2021-04-21 18:10:36.000000 scikit-dimension-0.3.2/doc/skdim.id.FisherS.fit_pw.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      249 2021-04-21 18:10:41.000000 scikit-dimension-0.3.2/doc/skdim.id.FisherS.fit_transform.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      260 2021-04-21 18:10:41.000000 scikit-dimension-0.3.2/doc/skdim.id.FisherS.fit_transform_pw.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      268 2021-04-21 18:10:36.000000 scikit-dimension-0.3.2/doc/skdim.id.FisherS.getSeparabilityGraph.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      240 2021-04-21 18:10:36.000000 scikit-dimension-0.3.2/doc/skdim.id.FisherS.get_params.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      271 2021-04-21 18:10:36.000000 scikit-dimension-0.3.2/doc/skdim.id.FisherS.plotSeparabilityGraph.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      307 2021-04-21 18:10:36.000000 scikit-dimension-0.3.2/doc/skdim.id.FisherS.point_inseparability_to_pointID.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      222 2021-01-02 16:58:51.000000 scikit-dimension-0.3.2/doc/skdim.id.FisherS.predict.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      233 2021-01-02 16:58:51.000000 scikit-dimension-0.3.2/doc/skdim.id.FisherS.predict_pw.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      753 2021-04-21 18:10:36.000000 scikit-dimension-0.3.2/doc/skdim.id.FisherS.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      240 2021-04-21 18:10:36.000000 scikit-dimension-0.3.2/doc/skdim.id.FisherS.set_params.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      235 2021-04-21 18:10:42.000000 scikit-dimension-0.3.2/doc/skdim.id.FisherS.transform.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      246 2021-04-21 18:10:42.000000 scikit-dimension-0.3.2/doc/skdim.id.FisherS.transform_pw.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      199 2021-04-21 18:10:36.000000 scikit-dimension-0.3.2/doc/skdim.id.KNN.fit.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      220 2021-01-02 16:58:51.000000 scikit-dimension-0.3.2/doc/skdim.id.KNN.fit_predict.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      231 2021-01-02 16:58:51.000000 scikit-dimension-0.3.2/doc/skdim.id.KNN.fit_predict_pw.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      212 2021-04-21 18:10:37.000000 scikit-dimension-0.3.2/doc/skdim.id.KNN.fit_pw.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      233 2021-04-21 18:10:42.000000 scikit-dimension-0.3.2/doc/skdim.id.KNN.fit_transform.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      244 2021-04-21 18:10:42.000000 scikit-dimension-0.3.2/doc/skdim.id.KNN.fit_transform_pw.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      224 2021-04-21 18:10:37.000000 scikit-dimension-0.3.2/doc/skdim.id.KNN.get_params.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      206 2021-01-02 16:58:51.000000 scikit-dimension-0.3.2/doc/skdim.id.KNN.predict.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      217 2021-01-02 16:58:51.000000 scikit-dimension-0.3.2/doc/skdim.id.KNN.predict_pw.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      475 2021-04-21 18:10:36.000000 scikit-dimension-0.3.2/doc/skdim.id.KNN.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      224 2021-04-21 18:10:37.000000 scikit-dimension-0.3.2/doc/skdim.id.KNN.set_params.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      219 2021-04-21 18:10:42.000000 scikit-dimension-0.3.2/doc/skdim.id.KNN.transform.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      230 2021-04-21 18:10:42.000000 scikit-dimension-0.3.2/doc/skdim.id.KNN.transform_pw.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      205 2021-04-21 18:10:37.000000 scikit-dimension-0.3.2/doc/skdim.id.MADA.fit.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      224 2021-01-02 16:58:52.000000 scikit-dimension-0.3.2/doc/skdim.id.MADA.fit_predict.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      235 2021-01-02 16:58:52.000000 scikit-dimension-0.3.2/doc/skdim.id.MADA.fit_predict_pw.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      237 2021-04-21 18:10:42.000000 scikit-dimension-0.3.2/doc/skdim.id.MADA.fit_transform.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      248 2021-04-21 18:10:42.000000 scikit-dimension-0.3.2/doc/skdim.id.MADA.fit_transform_pw.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      228 2021-04-21 18:10:37.000000 scikit-dimension-0.3.2/doc/skdim.id.MADA.get_params.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      210 2021-01-02 16:58:52.000000 scikit-dimension-0.3.2/doc/skdim.id.MADA.predict.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      221 2021-01-02 16:58:52.000000 scikit-dimension-0.3.2/doc/skdim.id.MADA.predict_pw.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      458 2021-04-21 18:10:37.000000 scikit-dimension-0.3.2/doc/skdim.id.MADA.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      228 2021-04-21 18:10:37.000000 scikit-dimension-0.3.2/doc/skdim.id.MADA.set_params.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      223 2021-04-21 18:10:42.000000 scikit-dimension-0.3.2/doc/skdim.id.MADA.transform.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      234 2021-04-21 18:10:42.000000 scikit-dimension-0.3.2/doc/skdim.id.MADA.transform_pw.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      200 2021-04-21 18:10:37.000000 scikit-dimension-0.3.2/doc/skdim.id.MLE.fit.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      218 2021-04-21 18:10:37.000000 scikit-dimension-0.3.2/doc/skdim.id.MLE.fit_once.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      227 2021-04-21 18:10:37.000000 scikit-dimension-0.3.2/doc/skdim.id.MLE.fit_predict.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      231 2021-01-02 16:58:52.000000 scikit-dimension-0.3.2/doc/skdim.id.MLE.fit_predict_pw.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      233 2021-04-21 18:10:43.000000 scikit-dimension-0.3.2/doc/skdim.id.MLE.fit_transform.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      244 2021-04-21 18:10:43.000000 scikit-dimension-0.3.2/doc/skdim.id.MLE.fit_transform_pw.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      224 2021-04-21 18:10:37.000000 scikit-dimension-0.3.2/doc/skdim.id.MLE.get_params.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      206 2021-01-02 16:58:52.000000 scikit-dimension-0.3.2/doc/skdim.id.MLE.predict.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      217 2021-01-02 16:58:52.000000 scikit-dimension-0.3.2/doc/skdim.id.MLE.predict_pw.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      509 2021-04-21 18:10:37.000000 scikit-dimension-0.3.2/doc/skdim.id.MLE.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      224 2021-04-21 18:10:37.000000 scikit-dimension-0.3.2/doc/skdim.id.MLE.set_params.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      219 2021-04-21 18:10:43.000000 scikit-dimension-0.3.2/doc/skdim.id.MLE.transform.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      230 2021-04-21 18:10:43.000000 scikit-dimension-0.3.2/doc/skdim.id.MLE.transform_pw.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      201 2021-04-21 18:10:38.000000 scikit-dimension-0.3.2/doc/skdim.id.MOM.fit.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      220 2021-01-02 16:58:52.000000 scikit-dimension-0.3.2/doc/skdim.id.MOM.fit_predict.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      231 2021-01-02 16:58:52.000000 scikit-dimension-0.3.2/doc/skdim.id.MOM.fit_predict_pw.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      233 2021-04-21 18:10:43.000000 scikit-dimension-0.3.2/doc/skdim.id.MOM.fit_transform.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      244 2021-04-21 18:10:43.000000 scikit-dimension-0.3.2/doc/skdim.id.MOM.fit_transform_pw.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      224 2021-04-21 18:10:38.000000 scikit-dimension-0.3.2/doc/skdim.id.MOM.get_params.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      206 2021-01-02 16:58:52.000000 scikit-dimension-0.3.2/doc/skdim.id.MOM.predict.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      217 2021-01-02 16:58:52.000000 scikit-dimension-0.3.2/doc/skdim.id.MOM.predict_pw.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      448 2021-04-21 18:10:38.000000 scikit-dimension-0.3.2/doc/skdim.id.MOM.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      224 2021-04-21 18:10:38.000000 scikit-dimension-0.3.2/doc/skdim.id.MOM.set_params.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      219 2021-04-21 18:10:43.000000 scikit-dimension-0.3.2/doc/skdim.id.MOM.transform.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      230 2021-04-21 18:10:43.000000 scikit-dimension-0.3.2/doc/skdim.id.MOM.transform_pw.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      217 2021-04-21 18:10:38.000000 scikit-dimension-0.3.2/doc/skdim.id.MiND_ML.fit.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      238 2021-01-02 16:58:53.000000 scikit-dimension-0.3.2/doc/skdim.id.MiND_ML.fit_predict.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      249 2021-01-02 16:58:53.000000 scikit-dimension-0.3.2/doc/skdim.id.MiND_ML.fit_predict_pw.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      230 2021-04-21 18:10:38.000000 scikit-dimension-0.3.2/doc/skdim.id.MiND_ML.fit_pw.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      251 2021-04-21 18:10:43.000000 scikit-dimension-0.3.2/doc/skdim.id.MiND_ML.fit_transform.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      262 2021-04-21 18:10:43.000000 scikit-dimension-0.3.2/doc/skdim.id.MiND_ML.fit_transform_pw.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      242 2021-04-21 18:10:38.000000 scikit-dimension-0.3.2/doc/skdim.id.MiND_ML.get_params.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      224 2021-01-02 16:58:53.000000 scikit-dimension-0.3.2/doc/skdim.id.MiND_ML.predict.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      235 2021-01-02 16:58:53.000000 scikit-dimension-0.3.2/doc/skdim.id.MiND_ML.predict_pw.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      521 2021-04-21 18:10:38.000000 scikit-dimension-0.3.2/doc/skdim.id.MiND_ML.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      242 2021-04-21 18:10:38.000000 scikit-dimension-0.3.2/doc/skdim.id.MiND_ML.set_params.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      237 2021-04-21 18:10:43.000000 scikit-dimension-0.3.2/doc/skdim.id.MiND_ML.transform.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      248 2021-04-21 18:10:43.000000 scikit-dimension-0.3.2/doc/skdim.id.MiND_ML.transform_pw.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      201 2021-04-21 18:10:38.000000 scikit-dimension-0.3.2/doc/skdim.id.TLE.fit.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      220 2021-01-02 16:58:53.000000 scikit-dimension-0.3.2/doc/skdim.id.TLE.fit_predict.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      231 2021-01-02 16:58:53.000000 scikit-dimension-0.3.2/doc/skdim.id.TLE.fit_predict_pw.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      233 2021-04-21 18:10:44.000000 scikit-dimension-0.3.2/doc/skdim.id.TLE.fit_transform.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      244 2021-04-21 18:10:44.000000 scikit-dimension-0.3.2/doc/skdim.id.TLE.fit_transform_pw.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      224 2021-04-21 18:10:38.000000 scikit-dimension-0.3.2/doc/skdim.id.TLE.get_params.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      206 2021-01-02 16:58:53.000000 scikit-dimension-0.3.2/doc/skdim.id.TLE.predict.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      217 2021-01-02 16:58:53.000000 scikit-dimension-0.3.2/doc/skdim.id.TLE.predict_pw.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      448 2021-04-21 18:10:38.000000 scikit-dimension-0.3.2/doc/skdim.id.TLE.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      224 2021-04-21 18:10:39.000000 scikit-dimension-0.3.2/doc/skdim.id.TLE.set_params.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      219 2021-04-21 18:10:44.000000 scikit-dimension-0.3.2/doc/skdim.id.TLE.transform.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      230 2021-04-21 18:10:44.000000 scikit-dimension-0.3.2/doc/skdim.id.TLE.transform_pw.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      208 2021-04-21 18:10:39.000000 scikit-dimension-0.3.2/doc/skdim.id.TwoNN.fit.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      228 2021-01-02 16:58:53.000000 scikit-dimension-0.3.2/doc/skdim.id.TwoNN.fit_predict.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      239 2021-01-02 16:58:53.000000 scikit-dimension-0.3.2/doc/skdim.id.TwoNN.fit_predict_pw.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      220 2021-04-21 18:10:39.000000 scikit-dimension-0.3.2/doc/skdim.id.TwoNN.fit_pw.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      241 2021-04-21 18:10:44.000000 scikit-dimension-0.3.2/doc/skdim.id.TwoNN.fit_transform.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      252 2021-04-21 18:10:44.000000 scikit-dimension-0.3.2/doc/skdim.id.TwoNN.fit_transform_pw.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      232 2021-04-21 18:10:39.000000 scikit-dimension-0.3.2/doc/skdim.id.TwoNN.get_params.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      214 2021-01-02 16:58:53.000000 scikit-dimension-0.3.2/doc/skdim.id.TwoNN.predict.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      225 2021-01-02 16:58:54.000000 scikit-dimension-0.3.2/doc/skdim.id.TwoNN.predict_pw.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      497 2021-04-21 18:10:39.000000 scikit-dimension-0.3.2/doc/skdim.id.TwoNN.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      232 2021-04-21 18:10:39.000000 scikit-dimension-0.3.2/doc/skdim.id.TwoNN.set_params.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      227 2021-04-21 18:10:44.000000 scikit-dimension-0.3.2/doc/skdim.id.TwoNN.transform.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      238 2021-04-21 18:10:44.000000 scikit-dimension-0.3.2/doc/skdim.id.TwoNN.transform_pw.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      203 2021-04-21 18:10:39.000000 scikit-dimension-0.3.2/doc/skdim.id.lPCA.fit.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      223 2021-01-02 16:58:54.000000 scikit-dimension-0.3.2/doc/skdim.id.lPCA.fit_predict.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      234 2021-01-02 16:58:54.000000 scikit-dimension-0.3.2/doc/skdim.id.lPCA.fit_predict_pw.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      215 2021-04-21 18:10:39.000000 scikit-dimension-0.3.2/doc/skdim.id.lPCA.fit_pw.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      236 2021-04-21 18:10:45.000000 scikit-dimension-0.3.2/doc/skdim.id.lPCA.fit_transform.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      247 2021-04-21 18:10:45.000000 scikit-dimension-0.3.2/doc/skdim.id.lPCA.fit_transform_pw.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      227 2021-04-21 18:10:39.000000 scikit-dimension-0.3.2/doc/skdim.id.lPCA.get_params.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      209 2021-01-02 16:58:54.000000 scikit-dimension-0.3.2/doc/skdim.id.lPCA.predict.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      220 2021-01-02 16:58:54.000000 scikit-dimension-0.3.2/doc/skdim.id.lPCA.predict_pw.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      486 2021-04-21 18:10:39.000000 scikit-dimension-0.3.2/doc/skdim.id.lPCA.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      227 2021-04-21 18:10:39.000000 scikit-dimension-0.3.2/doc/skdim.id.lPCA.set_params.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      222 2021-04-21 18:10:45.000000 scikit-dimension-0.3.2/doc/skdim.id.lPCA.transform.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      233 2021-04-21 18:10:45.000000 scikit-dimension-0.3.2/doc/skdim.id.lPCA.transform_pw.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)       99 2021-01-02 11:33:56.000000 scikit-dimension-0.3.2/environment.yml
-drwxrwxrwx   0 jo        (1000) jo        (1000)        0 2022-07-31 08:27:00.000000 scikit-dimension-0.3.2/examples/
--rwxrwxrwx   0 jo        (1000) jo        (1000)     1376 2020-12-09 11:28:10.000000 scikit-dimension-0.3.2/examples/plot_separabilityGraph.py
--rwxrwxrwx   0 jo        (1000) jo        (1000)       55 2022-02-25 09:29:37.000000 scikit-dimension-0.3.2/requirements.txt
-drwxrwxrwx   0 jo        (1000) jo        (1000)        0 2022-07-31 08:27:01.000000 scikit-dimension-0.3.2/scikit_dimension.egg-info/
--rwxrwxrwx   0 jo        (1000) jo        (1000)      901 2022-07-31 08:26:33.000000 scikit-dimension-0.3.2/scikit_dimension.egg-info/PKG-INFO
--rwxrwxrwx   0 jo        (1000) jo        (1000)     6988 2022-07-31 08:26:42.000000 scikit-dimension-0.3.2/scikit_dimension.egg-info/SOURCES.txt
--rwxrwxrwx   0 jo        (1000) jo        (1000)        1 2022-07-31 08:26:33.000000 scikit-dimension-0.3.2/scikit_dimension.egg-info/dependency_links.txt
--rwxrwxrwx   0 jo        (1000) jo        (1000)        1 2022-05-25 18:21:08.000000 scikit-dimension-0.3.2/scikit_dimension.egg-info/not-zip-safe
--rwxrwxrwx   0 jo        (1000) jo        (1000)      125 2022-07-31 08:26:33.000000 scikit-dimension-0.3.2/scikit_dimension.egg-info/requires.txt
--rwxrwxrwx   0 jo        (1000) jo        (1000)        6 2022-07-31 08:26:33.000000 scikit-dimension-0.3.2/scikit_dimension.egg-info/top_level.txt
--rwxrwxrwx   0 jo        (1000) jo        (1000)      106 2022-07-31 08:27:04.000000 scikit-dimension-0.3.2/setup.cfg
--rwxrwxrwx   0 jo        (1000) jo        (1000)     3277 2022-02-25 09:29:37.000000 scikit-dimension-0.3.2/setup.py
-drwxrwxrwx   0 jo        (1000) jo        (1000)        0 2022-07-31 08:27:01.000000 scikit-dimension-0.3.2/skdim/
--rwxrwxrwx   0 jo        (1000) jo        (1000)     1696 2022-07-30 22:00:40.000000 scikit-dimension-0.3.2/skdim/__init__.py
--rwxrwxrwx   0 jo        (1000) jo        (1000)    22720 2022-07-30 22:00:40.000000 scikit-dimension-0.3.2/skdim/_commonfuncs.py
--rwxrwxrwx   0 jo        (1000) jo        (1000)     1598 2022-07-31 08:25:57.000000 scikit-dimension-0.3.2/skdim/_version.py
--rwxrwxrwx   0 jo        (1000) jo        (1000)    23468 2022-07-30 22:00:40.000000 scikit-dimension-0.3.2/skdim/datasets.py
-drwxrwxrwx   0 jo        (1000) jo        (1000)        0 2022-07-31 08:27:03.000000 scikit-dimension-0.3.2/skdim/id/
-drwxrwxrwx   0 jo        (1000) jo        (1000)        0 2022-07-31 08:27:04.000000 scikit-dimension-0.3.2/skdim/id/DANCoFit/
--rwxrwxrwx   0 jo        (1000) jo        (1000)    62664 2020-07-09 16:08:29.000000 scikit-dimension-0.3.2/skdim/id/DANCoFit/DANCo_spline_dhat.pkl
--rwxrwxrwx   0 jo        (1000) jo        (1000)    63725 2020-07-09 16:08:29.000000 scikit-dimension-0.3.2/skdim/id/DANCoFit/DANCo_spline_mu.pkl
--rwxrwxrwx   0 jo        (1000) jo        (1000)    62000 2020-07-09 16:08:29.000000 scikit-dimension-0.3.2/skdim/id/DANCoFit/DANCo_spline_tau.pkl
--rwxrwxrwx   0 jo        (1000) jo        (1000)    60000 2020-08-20 14:04:36.000000 scikit-dimension-0.3.2/skdim/id/DANCoFit/dhat
--rwxrwxrwx   0 jo        (1000) jo        (1000)    60042 2020-08-20 14:04:36.000000 scikit-dimension-0.3.2/skdim/id/DANCoFit/mu
--rwxrwxrwx   0 jo        (1000) jo        (1000)    60000 2020-08-20 14:04:36.000000 scikit-dimension-0.3.2/skdim/id/DANCoFit/tau
--rwxrwxrwx   0 jo        (1000) jo        (1000)     3861 2021-01-03 11:49:21.000000 scikit-dimension-0.3.2/skdim/id/_CorrInt.py
--rwxrwxrwx   0 jo        (1000) jo        (1000)    14374 2021-06-08 01:29:46.000000 scikit-dimension-0.3.2/skdim/id/_DANCo.py
--rwxrwxrwx   0 jo        (1000) jo        (1000)     6441 2021-06-08 01:26:07.000000 scikit-dimension-0.3.2/skdim/id/_DANCoUtils.py
--rwxrwxrwx   0 jo        (1000) jo        (1000)    13217 2021-01-13 16:28:36.000000 scikit-dimension-0.3.2/skdim/id/_ESS.py
--rwxrwxrwx   0 jo        (1000) jo        (1000)    28007 2022-07-30 22:00:40.000000 scikit-dimension-0.3.2/skdim/id/_FisherS.py
--rwxrwxrwx   0 jo        (1000) jo        (1000)     5255 2021-01-13 16:28:34.000000 scikit-dimension-0.3.2/skdim/id/_KNN.py
--rwxrwxrwx   0 jo        (1000) jo        (1000)     2834 2021-01-03 14:26:00.000000 scikit-dimension-0.3.2/skdim/id/_MADA.py
--rwxrwxrwx   0 jo        (1000) jo        (1000)    13911 2021-01-13 16:28:29.000000 scikit-dimension-0.3.2/skdim/id/_MLE.py
--rwxrwxrwx   0 jo        (1000) jo        (1000)     2133 2021-01-03 11:47:58.000000 scikit-dimension-0.3.2/skdim/id/_MOM.py
--rwxrwxrwx   0 jo        (1000) jo        (1000)     5113 2021-01-13 16:32:45.000000 scikit-dimension-0.3.2/skdim/id/_MiND_ML.py
--rwxrwxrwx   0 jo        (1000) jo        (1000)     9841 2022-07-31 08:25:22.000000 scikit-dimension-0.3.2/skdim/id/_PCA.py
--rwxrwxrwx   0 jo        (1000) jo        (1000)     5521 2021-01-03 14:22:22.000000 scikit-dimension-0.3.2/skdim/id/_TLE.py
--rwxrwxrwx   0 jo        (1000) jo        (1000)     7085 2021-01-13 16:30:14.000000 scikit-dimension-0.3.2/skdim/id/_TwoNN.py
--rwxrwxrwx   0 jo        (1000) jo        (1000)     1876 2020-12-08 12:51:53.000000 scikit-dimension-0.3.2/skdim/id/__init__.py
-drwxrwxrwx   0 jo        (1000) jo        (1000)        0 2022-07-31 08:27:04.000000 scikit-dimension-0.3.2/skdim/tests/
--rwxrwxrwx   0 jo        (1000) jo        (1000)     1576 2020-08-20 14:04:37.000000 scikit-dimension-0.3.2/skdim/tests/__init__.py
--rwxrwxrwx   0 jo        (1000) jo        (1000)     7056 2021-04-21 17:07:26.000000 scikit-dimension-0.3.2/skdim/tests/test_all_params.py
--rwxrwxrwx   0 jo        (1000) jo        (1000)     9120 2021-03-08 21:33:04.000000 scikit-dimension-0.3.2/skdim/tests/test_results.py
+drwxr-xr-x   0 jbac       (502) staff       (20)        0 2023-05-16 20:34:24.359446 scikit-dimension-0.3.3/
+-rw-r--r--   0 jbac       (502) staff       (20)     1520 2023-05-16 20:22:05.000000 scikit-dimension-0.3.3/LICENSE
+-rw-r--r--   0 jbac       (502) staff       (20)       25 2023-05-16 20:22:05.000000 scikit-dimension-0.3.3/MANIFEST.in
+-rw-r--r--   0 jbac       (502) staff       (20)      901 2023-05-16 20:34:24.359571 scikit-dimension-0.3.3/PKG-INFO
+-rw-r--r--   0 jbac       (502) staff       (20)     2456 2023-05-16 20:22:05.000000 scikit-dimension-0.3.3/README.md
+-rw-r--r--   0 jbac       (502) staff       (20)       55 2023-05-16 20:22:05.000000 scikit-dimension-0.3.3/requirements.txt
+drwxr-xr-x   0 jbac       (502) staff       (20)        0 2023-05-16 20:34:24.355461 scikit-dimension-0.3.3/scikit_dimension.egg-info/
+-rw-r--r--   0 jbac       (502) staff       (20)      901 2023-05-16 20:34:24.000000 scikit-dimension-0.3.3/scikit_dimension.egg-info/PKG-INFO
+-rw-r--r--   0 jbac       (502) staff       (20)      728 2023-05-16 20:34:24.000000 scikit-dimension-0.3.3/scikit_dimension.egg-info/SOURCES.txt
+-rw-r--r--   0 jbac       (502) staff       (20)        1 2023-05-16 20:34:24.000000 scikit-dimension-0.3.3/scikit_dimension.egg-info/dependency_links.txt
+-rw-r--r--   0 jbac       (502) staff       (20)        1 2023-05-16 20:34:24.000000 scikit-dimension-0.3.3/scikit_dimension.egg-info/not-zip-safe
+-rw-r--r--   0 jbac       (502) staff       (20)      125 2023-05-16 20:34:24.000000 scikit-dimension-0.3.3/scikit_dimension.egg-info/requires.txt
+-rw-r--r--   0 jbac       (502) staff       (20)        6 2023-05-16 20:34:24.000000 scikit-dimension-0.3.3/scikit_dimension.egg-info/top_level.txt
+-rw-r--r--   0 jbac       (502) staff       (20)      106 2023-05-16 20:34:24.359964 scikit-dimension-0.3.3/setup.cfg
+-rw-r--r--   0 jbac       (502) staff       (20)     3277 2023-05-16 20:22:05.000000 scikit-dimension-0.3.3/setup.py
+drwxr-xr-x   0 jbac       (502) staff       (20)        0 2023-05-16 20:34:24.356171 scikit-dimension-0.3.3/skdim/
+-rw-r--r--   0 jbac       (502) staff       (20)     1696 2023-05-16 20:22:05.000000 scikit-dimension-0.3.3/skdim/__init__.py
+-rw-r--r--   0 jbac       (502) staff       (20)    23186 2023-05-16 20:29:25.000000 scikit-dimension-0.3.3/skdim/_commonfuncs.py
+-rw-r--r--   0 jbac       (502) staff       (20)     1598 2023-05-16 20:22:50.000000 scikit-dimension-0.3.3/skdim/_version.py
+-rw-r--r--   0 jbac       (502) staff       (20)    23468 2023-05-16 20:22:05.000000 scikit-dimension-0.3.3/skdim/datasets.py
+drwxr-xr-x   0 jbac       (502) staff       (20)        0 2023-05-16 20:34:24.358799 scikit-dimension-0.3.3/skdim/id/
+-rw-r--r--   0 jbac       (502) staff       (20)     3861 2023-05-16 20:22:05.000000 scikit-dimension-0.3.3/skdim/id/_CorrInt.py
+-rw-r--r--   0 jbac       (502) staff       (20)    14374 2023-05-16 20:22:05.000000 scikit-dimension-0.3.3/skdim/id/_DANCo.py
+-rw-r--r--   0 jbac       (502) staff       (20)     6441 2023-05-16 20:22:05.000000 scikit-dimension-0.3.3/skdim/id/_DANCoUtils.py
+-rw-r--r--   0 jbac       (502) staff       (20)    13217 2023-05-16 20:22:05.000000 scikit-dimension-0.3.3/skdim/id/_ESS.py
+-rw-r--r--   0 jbac       (502) staff       (20)    28007 2023-05-16 20:22:05.000000 scikit-dimension-0.3.3/skdim/id/_FisherS.py
+-rw-r--r--   0 jbac       (502) staff       (20)     5255 2023-05-16 20:22:05.000000 scikit-dimension-0.3.3/skdim/id/_KNN.py
+-rw-r--r--   0 jbac       (502) staff       (20)     2834 2023-05-16 20:22:05.000000 scikit-dimension-0.3.3/skdim/id/_MADA.py
+-rw-r--r--   0 jbac       (502) staff       (20)    13911 2023-05-16 20:22:05.000000 scikit-dimension-0.3.3/skdim/id/_MLE.py
+-rw-r--r--   0 jbac       (502) staff       (20)     2133 2023-05-16 20:22:05.000000 scikit-dimension-0.3.3/skdim/id/_MOM.py
+-rw-r--r--   0 jbac       (502) staff       (20)     5113 2023-05-16 20:22:05.000000 scikit-dimension-0.3.3/skdim/id/_MiND_ML.py
+-rw-r--r--   0 jbac       (502) staff       (20)     9841 2023-05-16 20:22:05.000000 scikit-dimension-0.3.3/skdim/id/_PCA.py
+-rw-r--r--   0 jbac       (502) staff       (20)     5521 2023-05-16 20:22:05.000000 scikit-dimension-0.3.3/skdim/id/_TLE.py
+-rw-r--r--   0 jbac       (502) staff       (20)     7085 2023-05-16 20:22:05.000000 scikit-dimension-0.3.3/skdim/id/_TwoNN.py
+-rw-r--r--   0 jbac       (502) staff       (20)     1876 2023-05-16 20:22:05.000000 scikit-dimension-0.3.3/skdim/id/__init__.py
+drwxr-xr-x   0 jbac       (502) staff       (20)        0 2023-05-16 20:34:24.359292 scikit-dimension-0.3.3/skdim/tests/
+-rw-r--r--   0 jbac       (502) staff       (20)     1576 2023-05-16 20:22:05.000000 scikit-dimension-0.3.3/skdim/tests/__init__.py
+-rw-r--r--   0 jbac       (502) staff       (20)     7056 2023-05-16 20:22:05.000000 scikit-dimension-0.3.3/skdim/tests/test_all_params.py
+-rw-r--r--   0 jbac       (502) staff       (20)     9120 2023-05-16 20:22:05.000000 scikit-dimension-0.3.3/skdim/tests/test_results.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `scikit-dimension-0.3.2/LICENSE` & `scikit-dimension-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit-dimension-0.3.2/PKG-INFO` & `scikit-dimension-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit-dimension
-Version: 0.3.2
+Version: 0.3.3
 Summary: scikit-dimension is a Python module for intrinsic dimension estimation built according to the scikit-learn API and distributed under the 3-Clause BSD license..
 Home-page: https://github.com/j-bac/scikit-dimension
 Download-URL: https://github.com/j-bac/scikit-dimension
 Maintainer: Jonathan Bac
 License: BSD-3-clause
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved
```

### Comparing `scikit-dimension-0.3.2/README.md` & `scikit-dimension-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `scikit-dimension-0.3.2/scikit_dimension.egg-info/PKG-INFO` & `scikit-dimension-0.3.3/scikit_dimension.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit-dimension
-Version: 0.3.2
+Version: 0.3.3
 Summary: scikit-dimension is a Python module for intrinsic dimension estimation built according to the scikit-learn API and distributed under the 3-Clause BSD license..
 Home-page: https://github.com/j-bac/scikit-dimension
 Download-URL: https://github.com/j-bac/scikit-dimension
 Maintainer: Jonathan Bac
 License: BSD-3-clause
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved
```

### Comparing `scikit-dimension-0.3.2/setup.py` & `scikit-dimension-0.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `scikit-dimension-0.3.2/skdim/__init__.py` & `scikit-dimension-0.3.3/skdim/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-dimension-0.3.2/skdim/_commonfuncs.py` & `scikit-dimension-0.3.3/skdim/_commonfuncs.py`

 * *Files 3% similar despite different names*

```diff
@@ -106,18 +106,19 @@
     """Use a global estimator as a pointwise one by creating kNN neighborhoods"""
     if precomputed_knn is not None:
         knn = precomputed_knn
     else:
         _, knn = get_nn(data, k=n_neighbors, n_jobs=n_jobs)
 
     if n_jobs > 1:
-        pool = mp.Pool(n_jobs)
-        results = pool.map(class_instance.fit, [data[i, :] for i in knn])
-        pool.close()
-        return np.array([r.dimension_ for r in results])
+        with mp.Pool(n_jobs) as pool:
+            # Asynchronously apply the `fit` function to each data point and collect the results
+            results = [pool.apply_async(class_instance.fit, (X[i, :],)) for i in knn]
+            # Retrieve the computed dimensions
+        return np.array([r.get().dimension_ for r in results])
     else:
         return np.array([class_instance.fit(data[i, :]).dimension_ for i in knn])
 
 
 # class DocInheritorBase(type):
 #    """ A metaclass to append GlobalEstimator or LocalEstimator Attributes section docstring to each estimator"""
 #
@@ -234,18 +235,19 @@
 
         if precomputed_knn is not None:
             knnidx = precomputed_knn
         else:
             _, knnidx = get_nn(X, k=n_neighbors, n_jobs=n_jobs)
 
         if n_jobs > 1:
-            pool = mp.Pool(n_jobs)
-            results = pool.map(self.fit, [X[i, :] for i in knnidx])
-            pool.close()
-            self.dimension_pw_ = np.array([r.dimension_ for r in results])
+            with mp.Pool(n_jobs) as pool:
+                # Asynchronously apply the `fit` function to each data point and collect the results
+                results = [pool.apply_async(self.fit, (X[i, :],)) for i in knnidx]
+                # Retrieve the computed dimensions
+                self.dimension_pw_ = np.array([r.get().dimension_ for r in results])
         else:
             self.dimension_pw_ = np.array(
                 [self.fit(X[i, :]).dimension_ for i in knnidx]
             )
 
         if smooth:
             self.dimension_pw_smooth_ = np.zeros(len(knnidx))
@@ -316,18 +318,19 @@
 
         if precomputed_knn is not None:
             knnidx = precomputed_knn
         else:
             _, knnidx = get_nn(X, k=n_neighbors, n_jobs=n_jobs)
 
         if n_jobs > 1:
-            pool = mp.Pool(n_jobs)
-            results = pool.map(self.fit, [X[i, :] for i in knnidx])
-            pool.close()
-            dimension_pw_ = np.array([r.dimension_ for r in results])
+            with mp.Pool(n_jobs) as pool:
+                # Asynchronously apply the `fit` function to each data point and collect the results
+                results = [pool.apply_async(self.fit, (X[i, :],)) for i in knnidx]
+                # Retrieve the computed dimensions
+                dimension_pw_ = np.array([r.get().dimension_ for r in results])
         else:
             dimension_pw_ = np.array([self.fit(X[i, :]).dimension_ for i in knnidx])
 
         if smooth:
             dimension_pw_smooth_ = np.zeros(len(knnidx))
             for i, point_nn in enumerate(knnidx):
                 dimension_pw_smooth_[i] = np.mean(
```

### Comparing `scikit-dimension-0.3.2/skdim/_version.py` & `scikit-dimension-0.3.3/skdim/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,8 +25,8 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 #
-__version__ = "0.3.2"
+__version__ = "0.3.3"
```

### Comparing `scikit-dimension-0.3.2/skdim/datasets.py` & `scikit-dimension-0.3.3/skdim/datasets.py`

 * *Files identical despite different names*

### Comparing `scikit-dimension-0.3.2/skdim/id/_CorrInt.py` & `scikit-dimension-0.3.3/skdim/id/_CorrInt.py`

 * *Files identical despite different names*

### Comparing `scikit-dimension-0.3.2/skdim/id/_DANCo.py` & `scikit-dimension-0.3.3/skdim/id/_DANCo.py`

 * *Files identical despite different names*

### Comparing `scikit-dimension-0.3.2/skdim/id/_DANCoUtils.py` & `scikit-dimension-0.3.3/skdim/id/_DANCoUtils.py`

 * *Files identical despite different names*

### Comparing `scikit-dimension-0.3.2/skdim/id/_ESS.py` & `scikit-dimension-0.3.3/skdim/id/_ESS.py`

 * *Files identical despite different names*

### Comparing `scikit-dimension-0.3.2/skdim/id/_FisherS.py` & `scikit-dimension-0.3.3/skdim/id/_FisherS.py`

 * *Files identical despite different names*

### Comparing `scikit-dimension-0.3.2/skdim/id/_KNN.py` & `scikit-dimension-0.3.3/skdim/id/_KNN.py`

 * *Files identical despite different names*

### Comparing `scikit-dimension-0.3.2/skdim/id/_MADA.py` & `scikit-dimension-0.3.3/skdim/id/_MADA.py`

 * *Files identical despite different names*

### Comparing `scikit-dimension-0.3.2/skdim/id/_MLE.py` & `scikit-dimension-0.3.3/skdim/id/_MLE.py`

 * *Files identical despite different names*

### Comparing `scikit-dimension-0.3.2/skdim/id/_MOM.py` & `scikit-dimension-0.3.3/skdim/id/_MOM.py`

 * *Files identical despite different names*

### Comparing `scikit-dimension-0.3.2/skdim/id/_MiND_ML.py` & `scikit-dimension-0.3.3/skdim/id/_MiND_ML.py`

 * *Files identical despite different names*

### Comparing `scikit-dimension-0.3.2/skdim/id/_PCA.py` & `scikit-dimension-0.3.3/skdim/id/_PCA.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
     verbose: bool, default=False
     explained_variance: bool, default=False
         If True, lPCA.fit(X) expects as input 
         a precomputed explained_variance vector: X = sklearn.decomposition.PCA().fit(X).explained_variance_
     
     Attributes
     ----------
-    gaps:
+    gap_:
         Ratio of each PC's explained variance (except the last) 
         with the following PC's explained variance
     """
 
     def __init__(
         self,
         ver="FO",
```

### Comparing `scikit-dimension-0.3.2/skdim/id/_TLE.py` & `scikit-dimension-0.3.3/skdim/id/_TLE.py`

 * *Files identical despite different names*

### Comparing `scikit-dimension-0.3.2/skdim/id/_TwoNN.py` & `scikit-dimension-0.3.3/skdim/id/_TwoNN.py`

 * *Files identical despite different names*

### Comparing `scikit-dimension-0.3.2/skdim/id/__init__.py` & `scikit-dimension-0.3.3/skdim/id/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-dimension-0.3.2/skdim/tests/__init__.py` & `scikit-dimension-0.3.3/skdim/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-dimension-0.3.2/skdim/tests/test_all_params.py` & `scikit-dimension-0.3.3/skdim/tests/test_all_params.py`

 * *Files identical despite different names*

### Comparing `scikit-dimension-0.3.2/skdim/tests/test_results.py` & `scikit-dimension-0.3.3/skdim/tests/test_results.py`

 * *Files identical despite different names*

