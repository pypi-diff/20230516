# Comparing `tmp/ncbi_submit-0.4.5.tar.gz` & `tmp/ncbi_submit-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ncbi_submit-0.4.5.tar", max compression
+gzip compressed data, was "ncbi_submit-0.4.6.tar", max compression
```

## Comparing `ncbi_submit-0.4.5.tar` & `ncbi_submit-0.4.6.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rwxr-xr-x   0        0        0     1065 2023-02-28 17:11:56.939831 ncbi_submit-0.4.5/LICENSE
--rwxr-xr-x   0        0        0     9179 2023-03-20 18:23:13.102670 ncbi_submit-0.4.5/README.md
--rwxr-xr-x   0        0        0        0 2023-02-28 17:11:56.939831 ncbi_submit-0.4.5/example/__init__.py
--rwxr-xr-x   0        0        0    15449 2023-02-28 17:11:56.939831 ncbi_submit-0.4.5/example/config.py
--rwxr-xr-x   0        0        0     1281 2023-02-28 17:11:56.939831 ncbi_submit-0.4.5/example/data/Clinical-01-06-23-1-V2A-fastqs/Sequencing_report-01-06-23-1-V2A-All.csv
--rwxr-xr-x   0        0        0   438411 2023-02-28 17:11:56.939831 ncbi_submit-0.4.5/example/data/Clinical-01-06-23-1-V2A-fastqs/fastqs/CORVASEQ-CLT-013517_barcode04.fastq
--rwxr-xr-x   0        0        0   435369 2023-02-28 17:11:56.939831 ncbi_submit-0.4.5/example/data/Clinical-01-06-23-1-V2A-fastqs/fastqs/CORVASEQ-CLT-013522_barcode09.fastq
--rwxr-xr-x   0        0        0      174 2023-02-28 17:11:56.939831 ncbi_submit-0.4.5/example/data/Clinical-01-06-23-1-V2A-fastqs/gisaid_uploader.log
--rwxr-xr-x   0        0        0     2439 2023-02-28 17:11:56.955486 ncbi_submit-0.4.5/example/data/Clinical-01-06-23-1-V2A-fastqs/ncbi/biosample_attributes.tsv
--rwxr-xr-x   0        0        0      545 2023-02-28 17:11:56.955486 ncbi_submit-0.4.5/example/data/Clinical-01-06-23-1-V2A-fastqs/ncbi/genbank-metadata.tsv
--rwxr-xr-x   0        0        0      958 2023-02-28 17:11:56.955486 ncbi_submit-0.4.5/example/data/Clinical-01-06-23-1-V2A-fastqs/ncbi/genbank.xml
--rwxr-xr-x   0        0        0    61930 2023-02-28 17:11:56.955486 ncbi_submit-0.4.5/example/data/Clinical-01-06-23-1-V2A-fastqs/ncbi/genbank.zip
--rwxr-xr-x   0        0        0     1762 2023-02-28 17:11:56.955486 ncbi_submit-0.4.5/example/data/Clinical-01-06-23-1-V2A-fastqs/ncbi/sra-metadata.tsv
--rwxr-xr-x   0        0        0    13878 2023-02-28 17:11:56.955486 ncbi_submit-0.4.5/example/data/Clinical-01-06-23-1-V2A-fastqs/ncbi/sra_biosample.xml
--rwxr-xr-x   0        0        0     2439 2023-03-03 20:53:36.333459 ncbi_submit-0.4.5/example/data/Clinical-01-06-23-1-V2A-fastqs/ncbi_test/biosample_attributes.tsv
--rwxr-xr-x   0        0        0      239 2023-02-28 17:11:56.955486 ncbi_submit-0.4.5/example/data/Clinical-01-06-23-1-V2A-fastqs/ncbi_test/bs_sra_reports/01-06-23-1-V2A/report.1.xml
--rwxr-xr-x   0        0        0      685 2023-02-28 17:11:56.955486 ncbi_submit-0.4.5/example/data/Clinical-01-06-23-1-V2A-fastqs/ncbi_test/bs_sra_reports/01-06-23-1-V2A/report.2.xml
--rwxr-xr-x   0        0        0      832 2023-02-28 17:11:56.955486 ncbi_submit-0.4.5/example/data/Clinical-01-06-23-1-V2A-fastqs/ncbi_test/bs_sra_reports/01-06-23-1-V2A/report.3.xml
--rwxr-xr-x   0        0        0     2641 2023-02-28 17:11:56.955486 ncbi_submit-0.4.5/example/data/Clinical-01-06-23-1-V2A-fastqs/ncbi_test/bs_sra_reports/01-06-23-1-V2A/report.4.xml
--rwxr-xr-x   0        0        0      831 2023-02-28 17:11:56.955486 ncbi_submit-0.4.5/example/data/Clinical-01-06-23-1-V2A-fastqs/ncbi_test/bs_sra_reports/01-06-23-1-V2A/report.5.xml
--rwxr-xr-x   0        0        0     2206 2023-02-28 17:11:56.955486 ncbi_submit-0.4.5/example/data/Clinical-01-06-23-1-V2A-fastqs/ncbi_test/bs_sra_reports/01-06-23-1-V2A/report.6.xml
--rwxr-xr-x   0        0        0     2206 2023-02-28 17:11:56.955486 ncbi_submit-0.4.5/example/data/Clinical-01-06-23-1-V2A-fastqs/ncbi_test/bs_sra_reports/01-06-23-1-V2A/report.xml
--rwxr-xr-x   0        0        0      555 2023-03-03 20:53:36.333459 ncbi_submit-0.4.5/example/data/Clinical-01-06-23-1-V2A-fastqs/ncbi_test/genbank-metadata.tsv
--rwxr-xr-x   0        0        0      963 2023-02-28 17:11:56.955486 ncbi_submit-0.4.5/example/data/Clinical-01-06-23-1-V2A-fastqs/ncbi_test/genbank.xml
--rwxr-xr-x   0        0        0    62291 2023-02-28 17:11:56.971100 ncbi_submit-0.4.5/example/data/Clinical-01-06-23-1-V2A-fastqs/ncbi_test/genbank.zip
--rwxr-xr-x   0        0        0       20 2023-02-20 15:23:12.325638 ncbi_submit-0.4.5/example/data/Clinical-01-06-23-1-V2A-fastqs/ncbi_test/samples2exclude.txt
--rwxr-xr-x   0        0        0     1762 2023-03-03 20:53:36.317839 ncbi_submit-0.4.5/example/data/Clinical-01-06-23-1-V2A-fastqs/ncbi_test/sra-metadata.tsv
--rwxr-xr-x   0        0        0    13878 2023-03-06 22:04:16.090632 ncbi_submit-0.4.5/example/data/Clinical-01-06-23-1-V2A-fastqs/ncbi_test/sra_biosample.xml
--rwxr-xr-x   0        0        0     1307 2023-02-28 17:11:56.971100 ncbi_submit-0.4.5/example/data/Clinical-01-06-23-1-V2A-fastqs/primer_map-01-06-23-1-V2A.csv
--rwxr-xr-x   0        0        0    59880 2023-02-28 17:11:56.971100 ncbi_submit-0.4.5/example/data/Clinical-01-06-23-1-V2A-fastqs/seqs-01-06-23-1-V2A.fasta
--rwxr-xr-x   0        0        0     1117 2023-03-06 21:24:56.686247 ncbi_submit-0.4.5/example/file_getter.py
--rwxr-xr-x   0        0        0     1539 2023-02-28 17:11:56.939831 ncbi_submit-0.4.5/example/template.sbt
--rwxr-xr-x   0        0        0     2491 2023-03-02 22:13:39.412942 ncbi_submit-0.4.5/example/test.sh
--rwxr-xr-x   0        0        0        0 2023-02-28 17:11:56.971100 ncbi_submit-0.4.5/ncbi_submit/__init__.py
--rwxr-xr-x   0        0        0    12876 2023-03-06 19:13:06.635895 ncbi_submit-0.4.5/ncbi_submit/arguments.py
--rwxr-xr-x   0        0        0     6896 2023-03-23 16:07:48.728443 ncbi_submit-0.4.5/ncbi_submit/helpers.py
--rwxr-xr-x   0        0        0    69884 2023-03-23 16:08:48.667850 ncbi_submit-0.4.5/ncbi_submit/ncbi.py
--rwxr-xr-x   0        0        0     2958 2023-03-06 21:13:37.765962 ncbi_submit-0.4.5/ncbi_submit/ncbi_submit.py
--rwxr-xr-x   0        0        0     9523 2023-02-28 17:11:56.971100 ncbi_submit-0.4.5/ncbi_submit/report.py
--rwxr-xr-x   0        0        0       89 2023-03-02 19:16:15.623579 ncbi_submit-0.4.5/ncbi_submit/version.py
--rwxr-xr-x   0        0        0    17635 2023-03-20 19:54:42.126900 ncbi_submit-0.4.5/ncbi_submit/xml_format.py
--rwxr-xr-x   0        0        0      691 2023-03-23 16:11:13.632938 ncbi_submit-0.4.5/pyproject.toml
--rw-r--r--   0        0        0    10014 1970-01-01 00:00:00.000000 ncbi_submit-0.4.5/PKG-INFO
+-rwxr-xr-x   0        0        0     1065 2023-02-28 17:11:56.939831 ncbi_submit-0.4.6/LICENSE
+-rwxr-xr-x   0        0        0     9174 2023-05-16 19:46:17.182783 ncbi_submit-0.4.6/README.md
+-rwxr-xr-x   0        0        0        0 2023-02-28 17:11:56.939831 ncbi_submit-0.4.6/example/__init__.py
+-rwxr-xr-x   0        0        0    15449 2023-02-28 17:11:56.939831 ncbi_submit-0.4.6/example/config.py
+-rwxr-xr-x   0        0        0     1281 2023-02-28 17:11:56.939831 ncbi_submit-0.4.6/example/data/Clinical-01-06-23-1-V2A-fastqs/Sequencing_report-01-06-23-1-V2A-All.csv
+-rwxr-xr-x   0        0        0   438411 2023-02-28 17:11:56.939831 ncbi_submit-0.4.6/example/data/Clinical-01-06-23-1-V2A-fastqs/fastqs/CORVASEQ-CLT-013517_barcode04.fastq
+-rwxr-xr-x   0        0        0   435369 2023-02-28 17:11:56.939831 ncbi_submit-0.4.6/example/data/Clinical-01-06-23-1-V2A-fastqs/fastqs/CORVASEQ-CLT-013522_barcode09.fastq
+-rwxr-xr-x   0        0        0      174 2023-02-28 17:11:56.939831 ncbi_submit-0.4.6/example/data/Clinical-01-06-23-1-V2A-fastqs/gisaid_uploader.log
+-rwxr-xr-x   0        0        0     2439 2023-02-28 17:11:56.955486 ncbi_submit-0.4.6/example/data/Clinical-01-06-23-1-V2A-fastqs/ncbi/biosample_attributes.tsv
+-rwxr-xr-x   0        0        0      545 2023-02-28 17:11:56.955486 ncbi_submit-0.4.6/example/data/Clinical-01-06-23-1-V2A-fastqs/ncbi/genbank-metadata.tsv
+-rwxr-xr-x   0        0        0      958 2023-02-28 17:11:56.955486 ncbi_submit-0.4.6/example/data/Clinical-01-06-23-1-V2A-fastqs/ncbi/genbank.xml
+-rwxr-xr-x   0        0        0    61930 2023-02-28 17:11:56.955486 ncbi_submit-0.4.6/example/data/Clinical-01-06-23-1-V2A-fastqs/ncbi/genbank.zip
+-rwxr-xr-x   0        0        0     1762 2023-02-28 17:11:56.955486 ncbi_submit-0.4.6/example/data/Clinical-01-06-23-1-V2A-fastqs/ncbi/sra-metadata.tsv
+-rwxr-xr-x   0        0        0    13878 2023-02-28 17:11:56.955486 ncbi_submit-0.4.6/example/data/Clinical-01-06-23-1-V2A-fastqs/ncbi/sra_biosample.xml
+-rwxr-xr-x   0        0        0     2439 2023-03-03 20:53:36.333459 ncbi_submit-0.4.6/example/data/Clinical-01-06-23-1-V2A-fastqs/ncbi_test/biosample_attributes.tsv
+-rwxr-xr-x   0        0        0      239 2023-02-28 17:11:56.955486 ncbi_submit-0.4.6/example/data/Clinical-01-06-23-1-V2A-fastqs/ncbi_test/bs_sra_reports/01-06-23-1-V2A/report.1.xml
+-rwxr-xr-x   0        0        0      685 2023-02-28 17:11:56.955486 ncbi_submit-0.4.6/example/data/Clinical-01-06-23-1-V2A-fastqs/ncbi_test/bs_sra_reports/01-06-23-1-V2A/report.2.xml
+-rwxr-xr-x   0        0        0      832 2023-02-28 17:11:56.955486 ncbi_submit-0.4.6/example/data/Clinical-01-06-23-1-V2A-fastqs/ncbi_test/bs_sra_reports/01-06-23-1-V2A/report.3.xml
+-rwxr-xr-x   0        0        0     2641 2023-02-28 17:11:56.955486 ncbi_submit-0.4.6/example/data/Clinical-01-06-23-1-V2A-fastqs/ncbi_test/bs_sra_reports/01-06-23-1-V2A/report.4.xml
+-rwxr-xr-x   0        0        0      831 2023-02-28 17:11:56.955486 ncbi_submit-0.4.6/example/data/Clinical-01-06-23-1-V2A-fastqs/ncbi_test/bs_sra_reports/01-06-23-1-V2A/report.5.xml
+-rwxr-xr-x   0        0        0     2206 2023-02-28 17:11:56.955486 ncbi_submit-0.4.6/example/data/Clinical-01-06-23-1-V2A-fastqs/ncbi_test/bs_sra_reports/01-06-23-1-V2A/report.6.xml
+-rwxr-xr-x   0        0        0     2206 2023-02-28 17:11:56.955486 ncbi_submit-0.4.6/example/data/Clinical-01-06-23-1-V2A-fastqs/ncbi_test/bs_sra_reports/01-06-23-1-V2A/report.xml
+-rwxr-xr-x   0        0        0      555 2023-03-03 20:53:36.333459 ncbi_submit-0.4.6/example/data/Clinical-01-06-23-1-V2A-fastqs/ncbi_test/genbank-metadata.tsv
+-rwxr-xr-x   0        0        0      963 2023-02-28 17:11:56.955486 ncbi_submit-0.4.6/example/data/Clinical-01-06-23-1-V2A-fastqs/ncbi_test/genbank.xml
+-rwxr-xr-x   0        0        0    62291 2023-02-28 17:11:56.971100 ncbi_submit-0.4.6/example/data/Clinical-01-06-23-1-V2A-fastqs/ncbi_test/genbank.zip
+-rwxr-xr-x   0        0        0       20 2023-02-20 15:23:12.325638 ncbi_submit-0.4.6/example/data/Clinical-01-06-23-1-V2A-fastqs/ncbi_test/samples2exclude.txt
+-rwxr-xr-x   0        0        0     1762 2023-03-03 20:53:36.317839 ncbi_submit-0.4.6/example/data/Clinical-01-06-23-1-V2A-fastqs/ncbi_test/sra-metadata.tsv
+-rwxr-xr-x   0        0        0    13878 2023-03-06 22:04:16.090632 ncbi_submit-0.4.6/example/data/Clinical-01-06-23-1-V2A-fastqs/ncbi_test/sra_biosample.xml
+-rwxr-xr-x   0        0        0     1307 2023-02-28 17:11:56.971100 ncbi_submit-0.4.6/example/data/Clinical-01-06-23-1-V2A-fastqs/primer_map-01-06-23-1-V2A.csv
+-rwxr-xr-x   0        0        0    59880 2023-02-28 17:11:56.971100 ncbi_submit-0.4.6/example/data/Clinical-01-06-23-1-V2A-fastqs/seqs-01-06-23-1-V2A.fasta
+-rwxr-xr-x   0        0        0     1117 2023-03-06 21:24:56.686247 ncbi_submit-0.4.6/example/file_getter.py
+-rwxr-xr-x   0        0        0     1539 2023-02-28 17:11:56.939831 ncbi_submit-0.4.6/example/template.sbt
+-rwxr-xr-x   0        0        0     2491 2023-03-02 22:13:39.412942 ncbi_submit-0.4.6/example/test.sh
+-rwxr-xr-x   0        0        0        0 2023-02-28 17:11:56.971100 ncbi_submit-0.4.6/ncbi_submit/__init__.py
+-rwxr-xr-x   0        0        0    12877 2023-05-16 13:01:16.902910 ncbi_submit-0.4.6/ncbi_submit/arguments.py
+-rwxr-xr-x   0        0        0     6896 2023-05-09 16:12:30.875084 ncbi_submit-0.4.6/ncbi_submit/helpers.py
+-rwxr-xr-x   0        0        0    71566 2023-05-16 19:37:10.717232 ncbi_submit-0.4.6/ncbi_submit/ncbi.py
+-rwxr-xr-x   0        0        0     2958 2023-05-09 16:13:12.397090 ncbi_submit-0.4.6/ncbi_submit/ncbi_submit.py
+-rwxr-xr-x   0        0        0     9546 2023-05-09 16:15:47.284697 ncbi_submit-0.4.6/ncbi_submit/report.py
+-rwxr-xr-x   0        0        0       89 2023-03-02 19:16:15.623579 ncbi_submit-0.4.6/ncbi_submit/version.py
+-rwxr-xr-x   0        0        0    17590 2023-05-09 16:17:35.672822 ncbi_submit-0.4.6/ncbi_submit/xml_format.py
+-rwxr-xr-x   0        0        0      691 2023-05-16 19:37:43.321948 ncbi_submit-0.4.6/pyproject.toml
+-rw-r--r--   0        0        0    10009 1970-01-01 00:00:00.000000 ncbi_submit-0.4.6/PKG-INFO
```

### Comparing `ncbi_submit-0.4.5/LICENSE` & `ncbi_submit-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ncbi_submit-0.4.5/README.md` & `ncbi_submit-0.4.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,30 @@
+Metadata-Version: 2.1
+Name: ncbi-submit
+Version: 0.4.6
+Summary: A tool for submitting to NCBI (SRA, BioSample, & GenBank).
+Home-page: https://github.com/enviro-lab/ncbi-submit
+License: MIT
+Keywords: ncbi,submission,upload
+Author: Sam Kunkleman
+Author-email: skunklem@uncc.edu
+Maintainer: Sam Kunkleman
+Maintainer-email: skunklem@uncc.edu
+Requires-Python: >=3.8
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: biopython (>=1.78)
+Requires-Dist: pandas (>=1.5)
+Project-URL: Repository, https://github.com/enviro-lab/ncbi-submit
+Description-Content-Type: text/markdown
+
 # ncbi-submit
 Submitting data to public databases is super important for publically funded laboratories, but it is not always a quick or intuitive process. `ncbi-submit` provides a simple and repeatable way to upload programmatic submissions to NCBI's SRA and GenBank with shared or unique BioProjects and BioSamples. Data can be uploaded as XML or zip files to either the Test or Production environments, and once there, the reports produced by NCBI can be analyzed to check on submission status and get BioSample accessions.
 
 ***
 ## Installation:
 To install from PyPI in a virtual environment `.venv`:
 ```console
@@ -92,22 +115,26 @@
 #### Shell:
 ```console
 ncbi_submit ftp \
     --submit --db bs_sra \
     --test_mode --test_dir \
     --config "${NCBI_CONFIG}" \
     --outdir "${NCBI_DIR}" \
-    -u "${ncbi_username}" \
-    -p "${ncbi_password}" \
     --fastq_dir "${FASTQS}"
+# wait a while and try this to download reports and view submission status
+ncbi_submit ftp \
+    --check --db bs_sra \
+    --test_mode --test_dir \
+    --config "${NCBI_CONFIG}" \
+    --outdir "${NCBI_DIR}" 
 ```
 #### Python:
 ```python
 ncbi.submit(db="bs_sra)
-# wait awhile and try this to download reports and view submission status
+# wait a while and try this to download reports and view submission status
 ncbi.check(db="bs_sra)
 ```
 
 ### GenBank submission
 (NOTE: not fully tested)
 To link your fasta in GenBank to the associated reads, you'll want to add in the BioSample accessions before submitting.
 * Acquire BioSample accessions via one of these methods:
@@ -119,29 +146,25 @@
 
 Then run `ncbi_submit ftp --submit` to submit to GenBank
 
 #### Shell:
 ```console
 # dowload report.xml files to get accesssions and add them to genbank.tsv
 ncbi_submit file_prep --prep_genbank \
-    -u "${ncbi_username}" \
-    -p "${ncbi_password}" \
     --outdir "${NCBI_DIR}" \
     --config ${NCBI_CONFIG} \
     --fasta "${GENERIC_CONSENSUS//PLATE/$PLATE}" \
     --plate "${PLATE}"
 
 # submit to GenBank (NOTE: db='gb')
 ncbi_submit ftp \
     --submit --db gb \
     --test_mode --test_dir \
     --config "${NCBI_CONFIG}" \
     --outdir "${NCBI_DIR}" \
-    -u "${ncbi_username}" \
-    -p "${ncbi_password}" \
     --fastq_dir "${FASTQS}"
 ```
 #### Python:
 ```python
 # dowload report.xml files to get accesssions
 ncbi.check(db="bs_sra")
 # prepare genbank submission files and submit
@@ -156,22 +179,20 @@
 ***
 ### Check Submission Status
 Wait awhile (10+ minutes) for NCBI to start processing the submission. Then run this to download reports and view submission status.
 This works for whichever db you want to check on. If not specified, you'll get results on all submitted dbs.
 
 #### Shell:
 ```console
-# check GenBank submission (NOTE: db='gb')
+# check status of GenBank submission (NOTE: db='gb')
 ncbi_submit ftp \
     --check --db gb \
     --test_mode --test_dir \
     --config "${NCBI_CONFIG}" \
-    --outdir "${NCBI_DIR}" \
-    -u "${ncbi_username}" \
-    -p "${ncbi_password}"
+    --outdir "${NCBI_DIR}"
 ```
 #### Python:
 ```python
 # check GenBank submission (NOTE: db='gb')
 ncbi.check(db="gb)
 ```
 
@@ -198,7 +219,8 @@
 | XML | link | create | create |  | [SRA submission w/ new BioSample & existing BioProject](https://www.ncbi.nlm.nih.gov/viewvc/v1/trunk/submit/public-docs/sra/samples/sra.submission.bs.run.xml?view=co)
 | XML | link | link | create |  | [SRA submission w/ existing BioSample & BioProject](https://www.ncbi.nlm.nih.gov/viewvc/v1/trunk/submit/public-docs/sra/samples/sra.submission.run.xml?view=co)
 | XML |  |  |  | create | [GenBank XML](https://www.ncbi.nlm.nih.gov/viewvc/v1/trunk/submit/public-docs/genbank/SARS-CoV-2/submission.xml?view=co)
 | doc |  |  |  | example | [Example GenBank submission zip](https://www.ncbi.nlm.nih.gov/viewvc/v1/trunk/submit/public-docs/genbank/SARS-CoV-2/)
 | XSD |  | schema |  |  | [BioSample XML Schema](https://www.ncbi.nlm.nih.gov/viewvc/v1/trunk/submit/public-docs/biosample/biosample.xsd?revision=71107&view=co)
 | XSD | schema |  |  |  | [BioProject XML Schema](https://www.ncbi.nlm.nih.gov/viewvc/v1/trunk/submit/public-docs/bioproject/bioproject.xsd?view=co)
 | err | validate |  |  |  | [Submission Error Explanations](https://www.ncbi.nlm.nih.gov/projects/biosample/docs/submission/validation/errors.xml)
+
```

### Comparing `ncbi_submit-0.4.5/example/config.py` & `ncbi_submit-0.4.6/example/config.py`

 * *Files identical despite different names*

### Comparing `ncbi_submit-0.4.5/example/data/Clinical-01-06-23-1-V2A-fastqs/Sequencing_report-01-06-23-1-V2A-All.csv` & `ncbi_submit-0.4.6/example/data/Clinical-01-06-23-1-V2A-fastqs/Sequencing_report-01-06-23-1-V2A-All.csv`

 * *Files identical despite different names*

### Comparing `ncbi_submit-0.4.5/example/data/Clinical-01-06-23-1-V2A-fastqs/fastqs/CORVASEQ-CLT-013517_barcode04.fastq` & `ncbi_submit-0.4.6/example/data/Clinical-01-06-23-1-V2A-fastqs/fastqs/CORVASEQ-CLT-013517_barcode04.fastq`

 * *Files identical despite different names*

### Comparing `ncbi_submit-0.4.5/example/data/Clinical-01-06-23-1-V2A-fastqs/fastqs/CORVASEQ-CLT-013522_barcode09.fastq` & `ncbi_submit-0.4.6/example/data/Clinical-01-06-23-1-V2A-fastqs/fastqs/CORVASEQ-CLT-013522_barcode09.fastq`

 * *Files identical despite different names*

### Comparing `ncbi_submit-0.4.5/example/data/Clinical-01-06-23-1-V2A-fastqs/ncbi/biosample_attributes.tsv` & `ncbi_submit-0.4.6/example/data/Clinical-01-06-23-1-V2A-fastqs/ncbi/biosample_attributes.tsv`

 * *Files identical despite different names*

### Comparing `ncbi_submit-0.4.5/example/data/Clinical-01-06-23-1-V2A-fastqs/ncbi/genbank-metadata.tsv` & `ncbi_submit-0.4.6/example/data/Clinical-01-06-23-1-V2A-fastqs/ncbi/genbank-metadata.tsv`

 * *Files identical despite different names*

### Comparing `ncbi_submit-0.4.5/example/data/Clinical-01-06-23-1-V2A-fastqs/ncbi/genbank.xml` & `ncbi_submit-0.4.6/example/data/Clinical-01-06-23-1-V2A-fastqs/ncbi/genbank.xml`

 * *Files identical despite different names*

### Comparing `ncbi_submit-0.4.5/example/data/Clinical-01-06-23-1-V2A-fastqs/ncbi/genbank.zip` & `ncbi_submit-0.4.6/example/data/Clinical-01-06-23-1-V2A-fastqs/ncbi/genbank.zip`

 * *Files identical despite different names*

### Comparing `ncbi_submit-0.4.5/example/data/Clinical-01-06-23-1-V2A-fastqs/ncbi/sra-metadata.tsv` & `ncbi_submit-0.4.6/example/data/Clinical-01-06-23-1-V2A-fastqs/ncbi/sra-metadata.tsv`

 * *Files identical despite different names*

### Comparing `ncbi_submit-0.4.5/example/data/Clinical-01-06-23-1-V2A-fastqs/ncbi/sra_biosample.xml` & `ncbi_submit-0.4.6/example/data/Clinical-01-06-23-1-V2A-fastqs/ncbi/sra_biosample.xml`

 * *Files identical despite different names*

### Comparing `ncbi_submit-0.4.5/example/data/Clinical-01-06-23-1-V2A-fastqs/ncbi_test/biosample_attributes.tsv` & `ncbi_submit-0.4.6/example/data/Clinical-01-06-23-1-V2A-fastqs/ncbi_test/biosample_attributes.tsv`

 * *Files identical despite different names*

### Comparing `ncbi_submit-0.4.5/example/data/Clinical-01-06-23-1-V2A-fastqs/ncbi_test/bs_sra_reports/01-06-23-1-V2A/report.2.xml` & `ncbi_submit-0.4.6/example/data/Clinical-01-06-23-1-V2A-fastqs/ncbi_test/bs_sra_reports/01-06-23-1-V2A/report.2.xml`

 * *Files identical despite different names*

### Comparing `ncbi_submit-0.4.5/example/data/Clinical-01-06-23-1-V2A-fastqs/ncbi_test/bs_sra_reports/01-06-23-1-V2A/report.3.xml` & `ncbi_submit-0.4.6/example/data/Clinical-01-06-23-1-V2A-fastqs/ncbi_test/bs_sra_reports/01-06-23-1-V2A/report.3.xml`

 * *Files identical despite different names*

### Comparing `ncbi_submit-0.4.5/example/data/Clinical-01-06-23-1-V2A-fastqs/ncbi_test/bs_sra_reports/01-06-23-1-V2A/report.4.xml` & `ncbi_submit-0.4.6/example/data/Clinical-01-06-23-1-V2A-fastqs/ncbi_test/bs_sra_reports/01-06-23-1-V2A/report.4.xml`

 * *Files identical despite different names*

### Comparing `ncbi_submit-0.4.5/example/data/Clinical-01-06-23-1-V2A-fastqs/ncbi_test/bs_sra_reports/01-06-23-1-V2A/report.5.xml` & `ncbi_submit-0.4.6/example/data/Clinical-01-06-23-1-V2A-fastqs/ncbi_test/bs_sra_reports/01-06-23-1-V2A/report.5.xml`

 * *Files identical despite different names*

### Comparing `ncbi_submit-0.4.5/example/data/Clinical-01-06-23-1-V2A-fastqs/ncbi_test/bs_sra_reports/01-06-23-1-V2A/report.6.xml` & `ncbi_submit-0.4.6/example/data/Clinical-01-06-23-1-V2A-fastqs/ncbi_test/bs_sra_reports/01-06-23-1-V2A/report.6.xml`

 * *Files identical despite different names*

### Comparing `ncbi_submit-0.4.5/example/data/Clinical-01-06-23-1-V2A-fastqs/ncbi_test/bs_sra_reports/01-06-23-1-V2A/report.xml` & `ncbi_submit-0.4.6/example/data/Clinical-01-06-23-1-V2A-fastqs/ncbi_test/bs_sra_reports/01-06-23-1-V2A/report.xml`

 * *Files identical despite different names*

### Comparing `ncbi_submit-0.4.5/example/data/Clinical-01-06-23-1-V2A-fastqs/ncbi_test/genbank-metadata.tsv` & `ncbi_submit-0.4.6/example/data/Clinical-01-06-23-1-V2A-fastqs/ncbi_test/genbank-metadata.tsv`

 * *Files identical despite different names*

### Comparing `ncbi_submit-0.4.5/example/data/Clinical-01-06-23-1-V2A-fastqs/ncbi_test/genbank.xml` & `ncbi_submit-0.4.6/example/data/Clinical-01-06-23-1-V2A-fastqs/ncbi_test/genbank.xml`

 * *Files identical despite different names*

### Comparing `ncbi_submit-0.4.5/example/data/Clinical-01-06-23-1-V2A-fastqs/ncbi_test/genbank.zip` & `ncbi_submit-0.4.6/example/data/Clinical-01-06-23-1-V2A-fastqs/ncbi_test/genbank.zip`

 * *Files identical despite different names*

### Comparing `ncbi_submit-0.4.5/example/data/Clinical-01-06-23-1-V2A-fastqs/ncbi_test/sra-metadata.tsv` & `ncbi_submit-0.4.6/example/data/Clinical-01-06-23-1-V2A-fastqs/ncbi_test/sra-metadata.tsv`

 * *Files identical despite different names*

### Comparing `ncbi_submit-0.4.5/example/data/Clinical-01-06-23-1-V2A-fastqs/ncbi_test/sra_biosample.xml` & `ncbi_submit-0.4.6/example/data/Clinical-01-06-23-1-V2A-fastqs/ncbi_test/sra_biosample.xml`

 * *Files identical despite different names*

### Comparing `ncbi_submit-0.4.5/example/data/Clinical-01-06-23-1-V2A-fastqs/primer_map-01-06-23-1-V2A.csv` & `ncbi_submit-0.4.6/example/data/Clinical-01-06-23-1-V2A-fastqs/primer_map-01-06-23-1-V2A.csv`

 * *Files identical despite different names*

### Comparing `ncbi_submit-0.4.5/example/data/Clinical-01-06-23-1-V2A-fastqs/seqs-01-06-23-1-V2A.fasta` & `ncbi_submit-0.4.6/example/data/Clinical-01-06-23-1-V2A-fastqs/seqs-01-06-23-1-V2A.fasta`

 * *Files identical despite different names*

### Comparing `ncbi_submit-0.4.5/example/file_getter.py` & `ncbi_submit-0.4.6/example/file_getter.py`

 * *Files identical despite different names*

### Comparing `ncbi_submit-0.4.5/example/template.sbt` & `ncbi_submit-0.4.6/example/template.sbt`

 * *Files identical despite different names*

### Comparing `ncbi_submit-0.4.5/example/test.sh` & `ncbi_submit-0.4.6/example/test.sh`

 * *Files identical despite different names*

### Comparing `ncbi_submit-0.4.5/ncbi_submit/arguments.py` & `ncbi_submit-0.4.6/ncbi_submit/arguments.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 import textwrap, argparse
 
 # TODO: simplify arguments? eliminate subprasers? Add in checks for args arequired for any given task
 
 def add_file_prep_args(parser_file_prep):
     ## file_prep
-    parser_file_prep.add_argument("--fastq_dir",type=Path,required=True,
+    parser_file_prep.add_argument("--fastq_dir",type=Path,required=False,
         help="Path to directory containing one compiled fastq file for each sample")
     parser_file_prep.add_argument("--seq_report",type=Path,required=True,
         help="Path to sequencing report CSV")
     parser_file_prep.add_argument("--plate",required=True,
         help="Unique run or plate identifier")
     parser_file_prep.add_argument("--barcode_map",type=Path,required=False,default=None,
         help="Path to barcode map TSV. Used as reference to check that all samples are accounted for.")
```

### Comparing `ncbi_submit-0.4.5/ncbi_submit/helpers.py` & `ncbi_submit-0.4.6/ncbi_submit/helpers.py`

 * *Files identical despite different names*

### Comparing `ncbi_submit-0.4.5/ncbi_submit/ncbi.py` & `ncbi_submit-0.4.6/ncbi_submit/ncbi.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 """A main class for preparing data and interacting with ncbi.
 """
 
 from ftplib import FTP
 from io import StringIO
 import os, logging
 from pathlib import Path
-from textwrap import dedent
 import pandas as pd
 from ncbi_submit.helpers import *
 from ncbi_submit.report import Report
 from ncbi_submit.xml_format import SRA_BioSample_Submission,GenBank_Submission
 from zipfile import ZipFile
 from Bio import SeqIO
 
@@ -52,14 +51,20 @@
         self.submitted_samples_file = cf.get("submitted_samples")
         self.ftp = None
         self.test_dir = test_dir if test_dir==True else cf.get("test_dir",test_dir)
         self.test_mode = test_mode if test_mode==True else cf.get("test_mode",test_mode)
         self.use_existing = use_existing
         self.vary_spuid = vary_spuid
 
+        # varify files exist if provided
+        for name,path in {"fastq_dir":fastq_dir,"seq_report":seq_report,"barcode_map":barcode_map,"gisaid_log":gisaid_log,"primer_map":primer_map,"fasta":fasta}.items():
+            if path and not Path(path).exists():
+                print(f"The provided file does not exist:\n{name}: {path}")
+                warn("")
+
         # set plate-specific details
         self.fastq_dir = Path(fastq_dir) if fastq_dir else None
         self.seq_report = Path(seq_report) if seq_report else None
         self.plate = plate
         self.outdir = self._set_outdir(outdir)
         self.exclude_file = self.outdir / "samples2exclude.txt"
         self.barcode_map = None if barcode_map==None else Path(barcode_map) # only required for file prep
@@ -215,15 +220,15 @@
             return
         if not Path(self.submitted_samples_file).exists():
             logging.warning(f"Couldn't find file: {self.submitted_samples_file}. Not checking for previously submitted samples.")
             return
         submitted = pd.read_csv(self.submitted_samples_file,header=None,names=["already_submitted"])["already_submitted"].unique()
         attempted_duplicate = df[df["sample_name"].isin(submitted)]
         if len(attempted_duplicate) > 0:
-            raise ValueError(f"The following sample(s) appear to have already been submitted.\n\n{attempted_duplicate}\n\n * To submit anyway,  remove that sample name from the file ({self.submitted_samples_file}) or temporarily comment out the variable `submitted_samples` in the `config_file`. \n * To exclude a sample from submission, add it to {self.exclude_file}")
+            raise ValueError(f"The following sample(s) appear to have already been submitted.\n\n{attempted_duplicate}\n\n * To submit anyway, remove any offending sample name from the file '{self.submitted_samples_file}' or temporarily comment out the variable `submitted_samples` in the `config_file`. \n * To exclude a sample from submission, add it to '{self.exclude_file}'")
 
     def _findExcludables(self):
         """Returns list of samples to exclude (if found in file `self.exclude_file`)"""
 
         excludables = []
         if self.exclude_file.exists():
             with self.exclude_file.open() as fh:
@@ -283,41 +288,62 @@
             
             # add derived attributes
             # ensure these are added to the df and list of expected columns
             if not starting_cols:
                 starting_cols = [col for col in ["Sample #","Test date","Sample ID","bioproject_accession","Primer Scheme"] if col in seq_report_df.columns]
                 renamed_cols = {"Test date":"collection_date","Sample #":"sample_name","Sample ID":"sample_title"}
                 ct_cols = []
-                print("starting_cols:",starting_cols)
+                # print("starting_cols:",starting_cols)
                 for i,col in self.sars_cov_2_diag_pcr_ct_values.items():
                     pcr_ct_col_name = f'sars_cov_2_diag_pcr_ct_value_{i}'
                     # set col to be included in starting columns
                     starting_cols.append(col)
                     # set col to be renamed
                     renamed_cols[col] = pcr_ct_col_name
                     # set new col to be added
                     ct_cols.extend([pcr_ct_col_name,f'sars_cov_2_diag_gene_name_{i}'])
-                print("starting_cols:",starting_cols)
-                print("renamed_cols:",renamed_cols)
+                # print("starting_cols:",starting_cols)
+                # print("renamed_cols:",renamed_cols)
                 biosample_df = seq_report_df[starting_cols].rename(columns=renamed_cols)
             else:
                 biosample_df = seq_report_df
 
+            # ensure all data is present
+            if biosample_df.isnull().values.any():
+                print(f"Metadata file '{self.seq_report}' is missing some data.")
+                warn("")
+
+
             # merge in gisaid accessions
             if not self.gisaid_df.empty:
                 # biosample = pd.merge(biosample,gisaid,on="sample_name_short",how='right')
                 biosample_df = pd.merge(biosample_df,self.gisaid_df,on="sample_name",how='right')
                 biosample_df = biosample_df[biosample_df["gisaid_accession"].notna()]
+                if biosample_df.isnull().values.any():
+                    print(f"\nThe gisaid data (from '{self.gisaid_log}') contains sample(s) not found in your metadata file '{self.seq_report}':")
+                    for col in biosample_df.columns:
+                        if biosample_df[col].isna().values.any():
+                            break
+                    samples_missing_metadata = biosample_df[biosample_df[col].isna()]["sample_name"].tolist()
+                    print(samples_missing_metadata)
+                    self._offer_skip_option(samples_missing_metadata)
+                    warn("")
             else:
                 biosample_df['gisaid_accession'] = 'missing'
             if ignore_dates:
                 biosample_df['isolate'] = ''
             else:
                 biosample_df['isolate'] = "SARS-CoV-2/human/USA/" + biosample_df["sample_name"].astype(str) + "/" + pd.DatetimeIndex(biosample_df['collection_date']).strftime('%Y')
+                # print(biosample_df[["sample_name",'isolate',"collection_date","gisaid_accession"]])
+                # print(biosample_df[biosample_df["sample_name"]=="CORVASEQ-CLT-002803"].squeeze())
+                # print(biosample_df['isolate'])
             biosample_df["collection_date"] = pd.to_datetime(biosample_df["collection_date"]) # ensures dates are in the desired format
+            no_date = biosample_df[biosample_df["collection_date"].isna()]
+            if not no_date.empty:
+                warn(f"Missing collection date for these samples:\n{no_date}")
             biosample_df['gisaid_accession'] = biosample_df['gisaid_accession'].apply(lambda x: x if str(x)!='nan' else 'missing')
 
             # add config defaults/overrides
             for k,col in self.biosample_presets.items():
                 if not k in ("bioproject_accession","bioproject_test_accession","all_cols"):
                     biosample_df[k] = col
 
@@ -604,29 +630,29 @@
                 "primer_scheme":"Primer Scheme",
                 "primer scheme":"Primer Scheme",
                 })
             if "Primer Scheme" in primers.columns:
                 primers = primers[["sample_name","Primer Scheme"]]
                 df = df.merge(primers,on="sample_name")
                 try_others = False
-                primer_map_failed = False
+                # primer_map_failed = False
             else: # if Primer Scheme column missing from file
                 if not self.primer_scheme:
                     raise AttributeError(f"'Primer Scheme' must be a field in the `primer_map` file '{self.primer_map}'. Alternatively, provide `primer_scheme` as an argument.")
                 else:
                     try_others = True
-                    primer_map_failed = True
-        if try_others == True:
-            # if no primer_map or 'Primer Scheme' column isn't found therein, use default for all samples
-            if self.primer_scheme:
-                df["Primer Scheme"] = self.primer_scheme
-            # If there's only one possible scheme in config, use it
-            elif len(self.allowed_schemes) == 1:
-                df["Primer Scheme"] = self.allowed_schemes[0]
-            else: raise AttributeError(f"'Primer Scheme' must be a field in your `seq_report` file '{self.primer_scheme}' \n or else one of the arguments `--primer_map` or `--primer_scheme` must be provided")
+                    # primer_map_failed = True
+            if try_others == True:
+                # if no primer_map or 'Primer Scheme' column isn't found therein, use default for all samples
+                if self.primer_scheme:
+                    df["Primer Scheme"] = self.primer_scheme
+                # If there's only one possible scheme in config, use it
+                elif len(self.allowed_schemes) == 1:
+                    df["Primer Scheme"] = self.allowed_schemes[0]
+                else: raise AttributeError(f"'Primer Scheme' must be a field in your `seq_report` file '{self.primer_scheme}' \n or else one of the arguments `--primer_map` or `--primer_scheme` must be provided")
         
         # verify primer schemes are allowed based on config
         if len(self.allowed_schemes) == 0: raise AttributeError(f"'allowed_schemes' must be specified in `config_file` '{self.config_file}'")
         extra_schemes = set(df["Primer Scheme"].unique()) - set(self.allowed_schemes)
         if len(extra_schemes) > 0:
             raise ValueError(f"The following scheme(s) are not among the `allowed_schemes` listed in the `config_file` '{self.config_file}':\n{extra_schemes}")
 
@@ -673,16 +699,15 @@
             else:
                 sra_df = sra_df[sra_df["sample_name"].notna()]
 
             # add derived attributes
             sra_df["library_ID"] = sra_df["sample_name"]
             # remove any sampes that are supposed to be excluded
             if self.exclude_file.exists():
-                with self.exclude_file.open() as fh:
-                    sra_df = sra_df[~sra_df["sample_name"].isin(set([line.strip() for line in fh]))]
+                sra_df = sra_df[~sra_df["sample_name"].isin(self._findExcludables())]
             sra_df = self._addFilenames(sra_df)
             sra_df = sra_df.dropna(subset=["filename"])
             sra_df = sra_df[sra_df["filename"]!=None]
             sra_df = self._add_primer_schemes(sra_df)
             for col in ("amplicon_PCR_primer_scheme","design_description","sequencing_protocol_name"):
                 sra_df[col] = sra_df["Primer Scheme"].apply(lambda scheme: self.protocol_scheme[scheme][col])
             sra_df = sra_df.drop(columns=["Primer Scheme"])
@@ -762,15 +787,15 @@
 
     def verifyUnsubmittable(self,samples_to_maybe_exclude,warning=""):
         """Prints warning and recommends marking samples for exclusion if needed"""
 
         if len(samples_to_maybe_exclude) != 0:
             logging.warning(warning)
             print(self._offer_skip_option(samples_to_maybe_exclude))
-            exit(1)
+            warn("")
 
     def getAllowedSamples(self,all_samples=None):
         """Returns collection of allowed samples from gisaid logfile or else all_samples
         
         Args:
             all_samples (Collection): default samples if no gisaid-submitted-samples exist to limit by
         """
@@ -1154,14 +1179,15 @@
             for file in ("genbank.zip","genbank.xml"):
                 self.upload_if_not_there(file)
         
         # biosample/sra
         if db == "bs_sra":
             self.upload_if_not_there("sra_biosample.xml")
             # move to directory containing fastqs files to upload
+            if not self.fastq_dir: raise AttributeError("`fastq_dir` is required when submitting samples")
             os.chdir(self.fastq_dir)
             # find and upload all (fastq) files in any column labeled "filename*"
             sra_df = self._prep_sra_df(use_existing=True)
 
             fn_cols = [col for col in sra_df.columns if col.startswith("filename")]
             for i,row in sra_df.iterrows():
                 sample_name = row["sample_name"]
```

### Comparing `ncbi_submit-0.4.5/ncbi_submit/ncbi_submit.py` & `ncbi_submit-0.4.6/ncbi_submit/ncbi_submit.py`

 * *Files identical despite different names*

### Comparing `ncbi_submit-0.4.5/ncbi_submit/report.py` & `ncbi_submit-0.4.6/ncbi_submit/report.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 """Some useful classes for analyzing report.xml files
 """
 
-
+from xml.dom import minidom
 import io
 import re
 
 
 class ActionReader:
     """Stores/retrieves details about a submission action from NCBI's report*.xml files"""
 
@@ -85,15 +85,14 @@
     def __init__(self,report_file) -> None:
         """Create an object to store and parse details about a report*.xml file 
 
         Args:
             report_file (str | Path): path to a report*.xml file
         """
 
-        from xml.dom import minidom
         self.report_file = report_file
         self.dom = minidom.parse(io.open(report_file))
         self.submission_status,self.submission_id = self._getSubmissionDetails()
         self.status_dicts = {}
         # self._createStatusDict()
         self.sra_actions,self.biosample_actions,self.genbank_actions = {},{},{}
         self.system_errors = 0 # number of sra samples where error_source=="system"
@@ -157,15 +156,16 @@
             report.append("status\t\tsamples")
             num_actions = 0
             for status,samples in status_dict.items():
                 num_actions += len(samples)
                 report.append(f"{status}\t{len(samples)}")
             num_processed_error = len(status_dict["processed-error"])
             if num_processed_error > 0 and "BioSample" in db:
-                report.append("For help with BioSample errors, see:\n  https://www.ncbi.nlm.nih.gov/projects/biosample/docs/submission/validation/errors.xml")
+                report.append("For help with BioSample errors, see:")
+                report.append("  https://www.ncbi.nlm.nih.gov/projects/biosample/docs/submission/validation/errors.xml")
             if num_processed_error > 0:
                 # if only some samples failed, list them
                 if num_actions != num_processed_error:
                     failed:list = status_dict["processed-error"]
                     report.append(f"failed samples: {failed}")
                 # if all SRA samples have both `status="processed-error"` and `error_source="system"` --> probably complete
                 elif self.system_errors == num_processed_error and test_dir and db=="SRA":
```

### Comparing `ncbi_submit-0.4.5/ncbi_submit/xml_format.py` & `ncbi_submit-0.4.6/ncbi_submit/xml_format.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 #!/usr/bin/env python3
 """Classes for converting NCBI TSVs to XML files for submission."""
 
 import datetime
 from abc import ABC, abstractmethod
-from pathlib import Path
 from textwrap import indent,dedent
-import pandas as pd
 from ncbi_submit.helpers import series2dict,get_bioproject_spuid
 # from ncbi_submit.ncbi import NCBI # only use for testing (with typing hints) - otherwise causes circular import
 
 class Action(ABC):
     """Converts details about an individual sample to an XML action"""
 
     def __init__(self,ncbi,indent_by=2) -> None:
```

### Comparing `ncbi_submit-0.4.5/pyproject.toml` & `ncbi_submit-0.4.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ncbi-submit"
-version = "0.4.5"
+version = "0.4.6"
 description = "A tool for submitting to NCBI (SRA, BioSample, & GenBank)."
 license = "MIT"
 authors = [
     "Sam Kunkleman <skunklem@uncc.edu>",
 ]
 maintainers = [
     "Sam Kunkleman <skunklem@uncc.edu>",
```

### Comparing `ncbi_submit-0.4.5/PKG-INFO` & `ncbi_submit-0.4.6/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,7 @@
-Metadata-Version: 2.1
-Name: ncbi-submit
-Version: 0.4.5
-Summary: A tool for submitting to NCBI (SRA, BioSample, & GenBank).
-Home-page: https://github.com/enviro-lab/ncbi-submit
-License: MIT
-Keywords: ncbi,submission,upload
-Author: Sam Kunkleman
-Author-email: skunklem@uncc.edu
-Maintainer: Sam Kunkleman
-Maintainer-email: skunklem@uncc.edu
-Requires-Python: >=3.8
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: biopython (>=1.78)
-Requires-Dist: pandas (>=1.5)
-Project-URL: Repository, https://github.com/enviro-lab/ncbi-submit
-Description-Content-Type: text/markdown
-
 # ncbi-submit
 Submitting data to public databases is super important for publically funded laboratories, but it is not always a quick or intuitive process. `ncbi-submit` provides a simple and repeatable way to upload programmatic submissions to NCBI's SRA and GenBank with shared or unique BioProjects and BioSamples. Data can be uploaded as XML or zip files to either the Test or Production environments, and once there, the reports produced by NCBI can be analyzed to check on submission status and get BioSample accessions.
 
 ***
 ## Installation:
 To install from PyPI in a virtual environment `.venv`:
 ```console
@@ -115,22 +92,26 @@
 #### Shell:
 ```console
 ncbi_submit ftp \
     --submit --db bs_sra \
     --test_mode --test_dir \
     --config "${NCBI_CONFIG}" \
     --outdir "${NCBI_DIR}" \
-    -u "${ncbi_username}" \
-    -p "${ncbi_password}" \
     --fastq_dir "${FASTQS}"
+# wait a while and try this to download reports and view submission status
+ncbi_submit ftp \
+    --check --db bs_sra \
+    --test_mode --test_dir \
+    --config "${NCBI_CONFIG}" \
+    --outdir "${NCBI_DIR}" 
 ```
 #### Python:
 ```python
 ncbi.submit(db="bs_sra)
-# wait awhile and try this to download reports and view submission status
+# wait a while and try this to download reports and view submission status
 ncbi.check(db="bs_sra)
 ```
 
 ### GenBank submission
 (NOTE: not fully tested)
 To link your fasta in GenBank to the associated reads, you'll want to add in the BioSample accessions before submitting.
 * Acquire BioSample accessions via one of these methods:
@@ -142,29 +123,25 @@
 
 Then run `ncbi_submit ftp --submit` to submit to GenBank
 
 #### Shell:
 ```console
 # dowload report.xml files to get accesssions and add them to genbank.tsv
 ncbi_submit file_prep --prep_genbank \
-    -u "${ncbi_username}" \
-    -p "${ncbi_password}" \
     --outdir "${NCBI_DIR}" \
     --config ${NCBI_CONFIG} \
     --fasta "${GENERIC_CONSENSUS//PLATE/$PLATE}" \
     --plate "${PLATE}"
 
 # submit to GenBank (NOTE: db='gb')
 ncbi_submit ftp \
     --submit --db gb \
     --test_mode --test_dir \
     --config "${NCBI_CONFIG}" \
     --outdir "${NCBI_DIR}" \
-    -u "${ncbi_username}" \
-    -p "${ncbi_password}" \
     --fastq_dir "${FASTQS}"
 ```
 #### Python:
 ```python
 # dowload report.xml files to get accesssions
 ncbi.check(db="bs_sra")
 # prepare genbank submission files and submit
@@ -179,22 +156,20 @@
 ***
 ### Check Submission Status
 Wait awhile (10+ minutes) for NCBI to start processing the submission. Then run this to download reports and view submission status.
 This works for whichever db you want to check on. If not specified, you'll get results on all submitted dbs.
 
 #### Shell:
 ```console
-# check GenBank submission (NOTE: db='gb')
+# check status of GenBank submission (NOTE: db='gb')
 ncbi_submit ftp \
     --check --db gb \
     --test_mode --test_dir \
     --config "${NCBI_CONFIG}" \
-    --outdir "${NCBI_DIR}" \
-    -u "${ncbi_username}" \
-    -p "${ncbi_password}"
+    --outdir "${NCBI_DIR}"
 ```
 #### Python:
 ```python
 # check GenBank submission (NOTE: db='gb')
 ncbi.check(db="gb)
 ```
 
@@ -221,8 +196,7 @@
 | XML | link | create | create |  | [SRA submission w/ new BioSample & existing BioProject](https://www.ncbi.nlm.nih.gov/viewvc/v1/trunk/submit/public-docs/sra/samples/sra.submission.bs.run.xml?view=co)
 | XML | link | link | create |  | [SRA submission w/ existing BioSample & BioProject](https://www.ncbi.nlm.nih.gov/viewvc/v1/trunk/submit/public-docs/sra/samples/sra.submission.run.xml?view=co)
 | XML |  |  |  | create | [GenBank XML](https://www.ncbi.nlm.nih.gov/viewvc/v1/trunk/submit/public-docs/genbank/SARS-CoV-2/submission.xml?view=co)
 | doc |  |  |  | example | [Example GenBank submission zip](https://www.ncbi.nlm.nih.gov/viewvc/v1/trunk/submit/public-docs/genbank/SARS-CoV-2/)
 | XSD |  | schema |  |  | [BioSample XML Schema](https://www.ncbi.nlm.nih.gov/viewvc/v1/trunk/submit/public-docs/biosample/biosample.xsd?revision=71107&view=co)
 | XSD | schema |  |  |  | [BioProject XML Schema](https://www.ncbi.nlm.nih.gov/viewvc/v1/trunk/submit/public-docs/bioproject/bioproject.xsd?view=co)
 | err | validate |  |  |  | [Submission Error Explanations](https://www.ncbi.nlm.nih.gov/projects/biosample/docs/submission/validation/errors.xml)
-
```

