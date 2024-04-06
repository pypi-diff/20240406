# Comparing `tmp/smaht_submitr-0.7.0.1b9.tar.gz` & `tmp/smaht_submitr-0.7.0.1b90.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smaht_submitr-0.7.0.1b9.tar", max compression
+gzip compressed data, was "smaht_submitr-0.7.0.1b90.tar", max compression
```

## Comparing `smaht_submitr-0.7.0.1b9.tar` & `smaht_submitr-0.7.0.1b90.tar`

### file list

```diff
@@ -1,50 +1,52 @@
--rw-r--r--   0        0        0     1098 2024-03-20 18:15:36.180092 smaht_submitr-0.7.0.1b9/LICENSE.txt
--rw-r--r--   0        0        0     2601 2024-03-20 18:15:36.180092 smaht_submitr-0.7.0.1b9/README.rst
--rw-r--r--   0        0        0     3447 2024-03-20 18:15:36.220093 smaht_submitr-0.7.0.1b9/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-20 18:15:36.220093 smaht_submitr-0.7.0.1b9/submitr/__init__.py
--rw-r--r--   0        0        0      731 2024-03-20 18:15:36.220093 smaht_submitr-0.7.0.1b9/submitr/base.py
--rw-r--r--   0        0        0      294 2024-03-20 18:15:36.220093 smaht_submitr-0.7.0.1b9/submitr/exceptions.py
--rw-r--r--   0        0        0     2628 2024-03-20 18:15:36.220093 smaht_submitr-0.7.0.1b9/submitr/output.py
--rw-r--r--   0        0        0        0 2024-03-20 18:15:36.220093 smaht_submitr-0.7.0.1b9/submitr/scripts/__init__.py
--rw-r--r--   0        0        0     3677 2024-03-20 18:15:36.220093 smaht_submitr-0.7.0.1b9/submitr/scripts/check_submission.py
--rw-r--r--   0        0        0     4610 2024-03-20 18:15:36.220093 smaht_submitr-0.7.0.1b9/submitr/scripts/cli_utils.py
--rw-r--r--   0        0        0     1775 2024-03-20 18:15:36.220093 smaht_submitr-0.7.0.1b9/submitr/scripts/list_submissions.py
--rw-r--r--   0        0        0      940 2024-03-20 18:15:36.220093 smaht_submitr-0.7.0.1b9/submitr/scripts/make_sample_fastq_file.py
--rw-r--r--   0        0        0     5252 2024-03-20 18:15:36.220093 smaht_submitr-0.7.0.1b9/submitr/scripts/resume_uploads.py
--rw-r--r--   0        0        0     1368 2024-03-20 18:15:36.220093 smaht_submitr-0.7.0.1b9/submitr/scripts/show_upload_info.py
--rw-r--r--   0        0        0     1572 2024-03-20 18:15:36.220093 smaht_submitr-0.7.0.1b9/submitr/scripts/submit_genelist.py
--rw-r--r--   0        0        0    16175 2024-03-20 18:15:36.220093 smaht_submitr-0.7.0.1b9/submitr/scripts/submit_metadata_bundle.py
--rw-r--r--   0        0        0     3437 2024-03-20 18:15:36.220093 smaht_submitr-0.7.0.1b9/submitr/scripts/submit_ontology.py
--rw-r--r--   0        0        0     1616 2024-03-20 18:15:36.220093 smaht_submitr-0.7.0.1b9/submitr/scripts/upload_item_data.py
--rw-r--r--   0        0        0    26913 2024-03-20 18:15:36.220093 smaht_submitr-0.7.0.1b9/submitr/scripts/view_portal_object.py
--rw-r--r--   0        0        0   133280 2024-03-20 18:15:36.220093 smaht_submitr-0.7.0.1b9/submitr/submission.py
--rw-r--r--   0        0        0        0 2024-03-20 18:15:36.220093 smaht_submitr-0.7.0.1b9/submitr/tests/__init__.py
--rw-r--r--   0        0        0      355 2024-03-20 18:15:36.220093 smaht_submitr-0.7.0.1b9/submitr/tests/conftest_settings.py
--rw-r--r--   0        0        0      163 2024-03-20 18:15:36.220093 smaht_submitr-0.7.0.1b9/submitr/tests/data/f1_R1.fastq.gz
--rw-r--r--   0        0        0      165 2024-03-20 18:15:36.220093 smaht_submitr-0.7.0.1b9/submitr/tests/data/f1_R2.fastq.gz
--rw-r--r--   0        0        0      167 2024-03-20 18:15:36.220093 smaht_submitr-0.7.0.1b9/submitr/tests/data/f2_R1.fastq.gz
--rw-r--r--   0        0        0      164 2024-03-20 18:15:36.220093 smaht_submitr-0.7.0.1b9/submitr/tests/data/f2_R2.fastq.gz
--rw-r--r--   0        0        0      272 2024-03-20 18:15:36.220093 smaht_submitr-0.7.0.1b9/submitr/tests/data/simulated_bundle.json
--rw-r--r--   0        0        0    10870 2024-03-20 18:15:36.220093 smaht_submitr-0.7.0.1b9/submitr/tests/data/submission_simple.xlsx
--rw-r--r--   0        0        0    10875 2024-03-20 18:15:36.220093 smaht_submitr-0.7.0.1b9/submitr/tests/data/submission_simple2.xlsx
--rw-r--r--   0        0        0    13306 2024-03-20 18:15:36.220093 smaht_submitr-0.7.0.1b9/submitr/tests/data/submission_test.xlsx
--rw-r--r--   0        0        0    13192 2024-03-20 18:15:36.220093 smaht_submitr-0.7.0.1b9/submitr/tests/data/submission_test_with_errors.xlsx
--rw-r--r--   0        0        0      169 2024-03-20 18:15:36.220093 smaht_submitr-0.7.0.1b9/submitr/tests/data/test1_R1.fastq.gz
--rw-r--r--   0        0        0      168 2024-03-20 18:15:36.220093 smaht_submitr-0.7.0.1b9/submitr/tests/data/test1_R2.fastq.gz
--rw-r--r--   0        0        0     1333 2024-03-20 18:15:36.220093 smaht_submitr-0.7.0.1b9/submitr/tests/test_base.py
--rw-r--r--   0        0        0     2629 2024-03-20 18:15:36.220093 smaht_submitr-0.7.0.1b9/submitr/tests/test_check_submission.py
--rw-r--r--   0        0        0      551 2024-03-20 18:15:36.220093 smaht_submitr-0.7.0.1b9/submitr/tests/test_exceptions.py
--rw-r--r--   0        0        0     1620 2024-03-20 18:15:36.220093 smaht_submitr-0.7.0.1b9/submitr/tests/test_make_sample_fastq_file.py
--rw-r--r--   0        0        0     1421 2024-03-20 18:15:36.220093 smaht_submitr-0.7.0.1b9/submitr/tests/test_misc.py
--rw-r--r--   0        0        0    11277 2024-03-20 18:15:36.220093 smaht_submitr-0.7.0.1b9/submitr/tests/test_resume_uploads.py
--rw-r--r--   0        0        0     2478 2024-03-20 18:15:36.220093 smaht_submitr-0.7.0.1b9/submitr/tests/test_show_upload_info.py
--rw-r--r--   0        0        0   156743 2024-03-20 18:15:36.224094 smaht_submitr-0.7.0.1b9/submitr/tests/test_submission.py
--rw-r--r--   0        0        0     2836 2024-03-20 18:15:36.224094 smaht_submitr-0.7.0.1b9/submitr/tests/test_submit_genelist.py
--rw-r--r--   0        0        0     6796 2024-03-20 18:15:36.224094 smaht_submitr-0.7.0.1b9/submitr/tests/test_submit_metadata_bundle.py
--rw-r--r--   0        0        0     3013 2024-03-20 18:15:36.224094 smaht_submitr-0.7.0.1b9/submitr/tests/test_submit_ontology.py
--rw-r--r--   0        0        0     1300 2024-03-20 18:15:36.224094 smaht_submitr-0.7.0.1b9/submitr/tests/test_testing_helpers.py
--rw-r--r--   0        0        0     3661 2024-03-20 18:15:36.224094 smaht_submitr-0.7.0.1b9/submitr/tests/test_upload_item_data.py
--rw-r--r--   0        0        0     4353 2024-03-20 18:15:36.224094 smaht_submitr-0.7.0.1b9/submitr/tests/test_utils.py
--rw-r--r--   0        0        0     1351 2024-03-20 18:15:36.224094 smaht_submitr-0.7.0.1b9/submitr/tests/testing_helpers.py
--rw-r--r--   0        0        0     6727 2024-03-20 18:15:36.224094 smaht_submitr-0.7.0.1b9/submitr/utils.py
--rw-r--r--   0        0        0     3993 1970-01-01 00:00:00.000000 smaht_submitr-0.7.0.1b9/PKG-INFO
+-rw-r--r--   0        0        0     1098 2024-04-06 21:04:35.837760 smaht_submitr-0.7.0.1b90/LICENSE.txt
+-rw-r--r--   0        0        0     2602 2024-04-06 21:04:35.837760 smaht_submitr-0.7.0.1b90/README.rst
+-rw-r--r--   0        0        0     3422 2024-04-06 21:04:35.877760 smaht_submitr-0.7.0.1b90/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-06 21:04:35.877760 smaht_submitr-0.7.0.1b90/submitr/__init__.py
+-rw-r--r--   0        0        0      731 2024-04-06 21:04:35.877760 smaht_submitr-0.7.0.1b90/submitr/base.py
+-rw-r--r--   0        0        0      294 2024-04-06 21:04:35.877760 smaht_submitr-0.7.0.1b90/submitr/exceptions.py
+-rw-r--r--   0        0        0     2628 2024-04-06 21:04:35.877760 smaht_submitr-0.7.0.1b90/submitr/output.py
+-rw-r--r--   0        0        0    13407 2024-04-06 21:04:35.877760 smaht_submitr-0.7.0.1b90/submitr/progress_bar.py
+-rw-r--r--   0        0        0    10819 2024-04-06 21:04:35.877760 smaht_submitr-0.7.0.1b90/submitr/s3_utils.py
+-rw-r--r--   0        0        0        0 2024-04-06 21:04:35.877760 smaht_submitr-0.7.0.1b90/submitr/scripts/__init__.py
+-rw-r--r--   0        0        0     3844 2024-04-06 21:04:35.877760 smaht_submitr-0.7.0.1b90/submitr/scripts/check_submission.py
+-rw-r--r--   0        0        0     7601 2024-04-06 21:04:35.877760 smaht_submitr-0.7.0.1b90/submitr/scripts/cli_utils.py
+-rw-r--r--   0        0        0     1835 2024-04-06 21:04:35.877760 smaht_submitr-0.7.0.1b90/submitr/scripts/list_submissions.py
+-rw-r--r--   0        0        0      940 2024-04-06 21:04:35.877760 smaht_submitr-0.7.0.1b90/submitr/scripts/make_sample_fastq_file.py
+-rw-r--r--   0        0        0     5718 2024-04-06 21:04:35.877760 smaht_submitr-0.7.0.1b90/submitr/scripts/resume_uploads.py
+-rw-r--r--   0        0        0     1368 2024-04-06 21:04:35.877760 smaht_submitr-0.7.0.1b90/submitr/scripts/show_upload_info.py
+-rw-r--r--   0        0        0     1572 2024-04-06 21:04:35.877760 smaht_submitr-0.7.0.1b90/submitr/scripts/submit_genelist.py
+-rw-r--r--   0        0        0    19866 2024-04-06 21:04:35.877760 smaht_submitr-0.7.0.1b90/submitr/scripts/submit_metadata_bundle.py
+-rw-r--r--   0        0        0     3437 2024-04-06 21:04:35.877760 smaht_submitr-0.7.0.1b90/submitr/scripts/submit_ontology.py
+-rw-r--r--   0        0        0     1616 2024-04-06 21:04:35.877760 smaht_submitr-0.7.0.1b90/submitr/scripts/upload_item_data.py
+-rw-r--r--   0        0        0    28731 2024-04-06 21:04:35.877760 smaht_submitr-0.7.0.1b90/submitr/scripts/view_portal_object.py
+-rw-r--r--   0        0        0   149054 2024-04-06 21:04:35.881760 smaht_submitr-0.7.0.1b90/submitr/submission.py
+-rw-r--r--   0        0        0        0 2024-04-06 21:04:35.881760 smaht_submitr-0.7.0.1b90/submitr/tests/__init__.py
+-rw-r--r--   0        0        0      355 2024-04-06 21:04:35.881760 smaht_submitr-0.7.0.1b90/submitr/tests/conftest_settings.py
+-rw-r--r--   0        0        0      163 2024-04-06 21:04:35.881760 smaht_submitr-0.7.0.1b90/submitr/tests/data/f1_R1.fastq.gz
+-rw-r--r--   0        0        0      165 2024-04-06 21:04:35.881760 smaht_submitr-0.7.0.1b90/submitr/tests/data/f1_R2.fastq.gz
+-rw-r--r--   0        0        0      167 2024-04-06 21:04:35.881760 smaht_submitr-0.7.0.1b90/submitr/tests/data/f2_R1.fastq.gz
+-rw-r--r--   0        0        0      164 2024-04-06 21:04:35.881760 smaht_submitr-0.7.0.1b90/submitr/tests/data/f2_R2.fastq.gz
+-rw-r--r--   0        0        0      272 2024-04-06 21:04:35.881760 smaht_submitr-0.7.0.1b90/submitr/tests/data/simulated_bundle.json
+-rw-r--r--   0        0        0    10870 2024-04-06 21:04:35.881760 smaht_submitr-0.7.0.1b90/submitr/tests/data/submission_simple.xlsx
+-rw-r--r--   0        0        0    10875 2024-04-06 21:04:35.881760 smaht_submitr-0.7.0.1b90/submitr/tests/data/submission_simple2.xlsx
+-rw-r--r--   0        0        0    13306 2024-04-06 21:04:35.881760 smaht_submitr-0.7.0.1b90/submitr/tests/data/submission_test.xlsx
+-rw-r--r--   0        0        0    13192 2024-04-06 21:04:35.881760 smaht_submitr-0.7.0.1b90/submitr/tests/data/submission_test_with_errors.xlsx
+-rw-r--r--   0        0        0      169 2024-04-06 21:04:35.881760 smaht_submitr-0.7.0.1b90/submitr/tests/data/test1_R1.fastq.gz
+-rw-r--r--   0        0        0      168 2024-04-06 21:04:35.881760 smaht_submitr-0.7.0.1b90/submitr/tests/data/test1_R2.fastq.gz
+-rw-r--r--   0        0        0     1333 2024-04-06 21:04:35.881760 smaht_submitr-0.7.0.1b90/submitr/tests/test_base.py
+-rw-r--r--   0        0        0     2629 2024-04-06 21:04:35.881760 smaht_submitr-0.7.0.1b90/submitr/tests/test_check_submission.py
+-rw-r--r--   0        0        0      551 2024-04-06 21:04:35.881760 smaht_submitr-0.7.0.1b90/submitr/tests/test_exceptions.py
+-rw-r--r--   0        0        0     1620 2024-04-06 21:04:35.881760 smaht_submitr-0.7.0.1b90/submitr/tests/test_make_sample_fastq_file.py
+-rw-r--r--   0        0        0     1421 2024-04-06 21:04:35.881760 smaht_submitr-0.7.0.1b90/submitr/tests/test_misc.py
+-rw-r--r--   0        0        0    11606 2024-04-06 21:04:35.881760 smaht_submitr-0.7.0.1b90/submitr/tests/test_resume_uploads.py
+-rw-r--r--   0        0        0     2478 2024-04-06 21:04:35.881760 smaht_submitr-0.7.0.1b90/submitr/tests/test_show_upload_info.py
+-rw-r--r--   0        0        0   157433 2024-04-06 21:04:35.881760 smaht_submitr-0.7.0.1b90/submitr/tests/test_submission.py
+-rw-r--r--   0        0        0     2836 2024-04-06 21:04:35.881760 smaht_submitr-0.7.0.1b90/submitr/tests/test_submit_genelist.py
+-rw-r--r--   0        0        0     6874 2024-04-06 21:04:35.881760 smaht_submitr-0.7.0.1b90/submitr/tests/test_submit_metadata_bundle.py
+-rw-r--r--   0        0        0     3013 2024-04-06 21:04:35.881760 smaht_submitr-0.7.0.1b90/submitr/tests/test_submit_ontology.py
+-rw-r--r--   0        0        0     1300 2024-04-06 21:04:35.881760 smaht_submitr-0.7.0.1b90/submitr/tests/test_testing_helpers.py
+-rw-r--r--   0        0        0     3661 2024-04-06 21:04:35.881760 smaht_submitr-0.7.0.1b90/submitr/tests/test_upload_item_data.py
+-rw-r--r--   0        0        0     4353 2024-04-06 21:04:35.881760 smaht_submitr-0.7.0.1b90/submitr/tests/test_utils.py
+-rw-r--r--   0        0        0     1351 2024-04-06 21:04:35.881760 smaht_submitr-0.7.0.1b90/submitr/tests/testing_helpers.py
+-rw-r--r--   0        0        0    11074 2024-04-06 21:04:35.881760 smaht_submitr-0.7.0.1b90/submitr/utils.py
+-rw-r--r--   0        0        0     3989 1970-01-01 00:00:00.000000 smaht_submitr-0.7.0.1b90/PKG-INFO
```

### Comparing `smaht_submitr-0.7.0.1b9/LICENSE.txt` & `smaht_submitr-0.7.0.1b90/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b9/README.rst` & `smaht_submitr-0.7.0.1b90/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -50,16 +50,16 @@
 
 Installation
 ============
 
 Installing this system involves these steps:
 
 1. Install Python and optionally a virtual environment manager of your choice (e.g. ``pyenv``)..
-3. Install this package with: ``pip install smaht-submitr``
-4. Setup your SMaHT Portal credentials file: ``~/.smaht-keys.json``. See `SMaHT Submitr Credentals <https://submitr.readthedocs.io/en/draft/installation.html>`_ for more in this.
+2. Install this package with: ``pip install smaht-submitr``
+3. Setup your SMaHT Portal credentials file: ``~/.smaht-keys.json``. See `SMaHT Submitr Credentials <https://submitr.readthedocs.io/en/draft/installation.html>`_ for more in this.
 
 See detailed information about installation see: `Installing SMaHT Submitr <https://submitr.readthedocs.io/en/draft/installation.html>`_.
 
 
 Getting Started
 ===============
```

### Comparing `smaht_submitr-0.7.0.1b9/pyproject.toml` & `smaht_submitr-0.7.0.1b90/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "smaht-submitr"
-version = "0.7.0.1b9"  # TODO: To become 0.8.0
+version = "0.7.0.1b90"  # TODO: To become 0.8.0
 description = "Support for uploading file submissions to SMAHT."
 # TODO: Update this email address when a more specific one is available for SMaHT.
 authors = ["SMaHT DAC <smhelp@hms-dbmi.atlassian.net >"]
 license = "MIT"
 readme = "README.rst"
 keywords = ["submitr", "smaht"]
 homepage = "https://github.com/smaht-dac/submitr"
@@ -45,16 +45,15 @@
 ]
 
 [tool.poetry.dependencies]
 
 python = ">=3.8.0,<3.12"
 awscli = ">=1.32.49"
 boto3 = "^1.34.49"
-#dcicutils = "^8.8.0"
-dcicutils = "^8.8.1.1b1"
+dcicutils = "^8.8.2"
 PyYAML = "^6.0.1"
 requests = "^2.31.0"
 
 [tool.poetry.dev-dependencies]
 
 # Coverage
 codacy-coverage = ">=1.3.11"
```

### Comparing `smaht_submitr-0.7.0.1b9/submitr/base.py` & `smaht_submitr-0.7.0.1b90/submitr/base.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b9/submitr/output.py` & `smaht_submitr-0.7.0.1b90/submitr/output.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b9/submitr/scripts/check_submission.py` & `smaht_submitr-0.7.0.1b90/submitr/scripts/check_submission.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,14 +22,15 @@
                            f" Normally this should not be given.")
     args.add_argument('--server', '-s', help="an http or https address of the server to use", default=None)
     args.add_argument("--env", "-e",
                       help="Portal environment name for server/credentials (e.g. in ~/.smaht-keys.json).")
     args.add_argument('--keys', help="Path to keys file (rather than default ~/.smaht-keys.json).", default=None)
     args.add_argument('--directory', '-d', help="Directory of the upload files (if resuming submission).")
     args.add_argument('--directory-only', help="Same as --directory but NOT recursively.", default=False)
+    args.add_argument('--output', help="Output file for results.", default=False)
     args.add_argument('--details', action="store_true", help="More detailed output.", default=False)
     args.add_argument('--timeout', help="Wait timeout for server validation/submission.")
     args.add_argument('--verbose', action="store_true", help="More verbose output.", default=False)
     args.add_argument('--debug', action="store_true", help="Debugging output.", default=False)
     args = args.parse_args(args=simulated_args_for_testing)
 
     if not args.submission_uuid:
@@ -73,13 +74,15 @@
                 server=args.server,
                 env_from_env=env_from_env,
                 show_details=(args.verbose or args.details),
                 check_submission_script=True,
                 verbose=args.verbose,
                 debug=args.debug,
                 upload_directory=upload_directory,
-                upload_directory_recursive=not upload_directory_only
+                upload_directory_recursive=not upload_directory_only,
+                output_file=args.output,
+                note="Checking Submission"
         )
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `smaht_submitr-0.7.0.1b9/submitr/scripts/list_submissions.py` & `smaht_submitr-0.7.0.1b90/submitr/scripts/list_submissions.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
         env_from_env = True
 
     # TODO: handle --mine and --user
 
     with script_catch_errors():
         portal = _define_portal(env=args.env,
                                 env_from_env=env_from_env,
-                                keys_file=args.keys or os.environ.get("SMAHT_KEYS"), report=not args.quiet)
+                                keys_file=args.keys or os.environ.get("SMAHT_KEYS"),
+                                report=not args.quiet, note="Listing Submissions")
         _print_recent_submissions(portal, details=args.details, verbose=args.verbose,
                                   count=args.count, mine=args.mine, user=args.user)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `smaht_submitr-0.7.0.1b9/submitr/scripts/make_sample_fastq_file.py` & `smaht_submitr-0.7.0.1b90/submitr/scripts/make_sample_fastq_file.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b9/submitr/scripts/resume_uploads.py` & `smaht_submitr-0.7.0.1b90/submitr/scripts/resume_uploads.py`

 * *Files 19% similar despite different names*

```diff
@@ -42,49 +42,56 @@
 --help-advanced
   Prints this plus more advanced documentation.
 --help-web
   Opens your browser to the Web based documentation.
   {CustomArgumentParser.HELP_URL}#resuming-uploads
 ===
 """
+_OBSOLETE_OPTIONS = [
+    {"option": "-e", "message": "Use --env."},
+    {"option": "-s", "message": "Use --server."},
+    {"option": "-b", "message": "Use --bundle."},
+    {"option": "--bundle_filename", "message": "Use --bundle."},
+    {"option": "-u", "message": "Use --directory-only; or --directory which searches recusively."},
+    {"option": "-d", "message": "Use --directory-only; or --directory which searches recusively."},
+    {"option": "-nq", "message": "Use --no_query"},
+    {"option": "-nq", "message": "Use --yes"},
+    {"option": "--no_query", "message": "Use --yes"},
+    {"option": "-sf", "message": "Use --directory which defaults to searching recusively."},
+    {"option": "--subfolders", "message": "Use --directory which defaults to searching recusively."}
+]
 
 
 def main(simulated_args_for_testing=None):
-    parser = CustomArgumentParser(_HELP, package="smaht-submitr")
+    parser = CustomArgumentParser(help=_HELP, obsolete_options=_OBSOLETE_OPTIONS)
     parser.add_argument('uuid', nargs="?", help='IngestionSumission UUID (or upload file UUID or accession ID).')
-    parser.add_argument('--server', '-s',
+    parser.add_argument('--server',
                         help="HTTP(S) address of Portal server (e.g. in ~/.smaht-keys.json).")
-    parser.add_argument('--env', '-e',
+    parser.add_argument('--env',
                         help="Portal environment name for server/credentials (e.g. in ~/.smaht-keys.json).")
     parser.add_argument('--app',
                         help=f"An application (default {DEFAULT_APP!r}. Only for debugging."
                              f" Normally this should not be given.")
     parser.add_argument('--bundle', help="location of the original Excel submission file")
-    parser.add_argument('--bundle_filename', '-b', help="Synonym for --bundle.")
     parser.add_argument('--keys', help="Path to keys file (rather than default ~/.smaht-keys.json).", default=None)
-    parser.add_argument('--directory', '-d', help="Directory of the upload files.")
+    parser.add_argument('--directory', help="Directory of the upload files.")
     parser.add_argument('--directory-only', help="Same as --directory but NOT recursively.", default=False)
-    parser.add_argument('--upload_folder', '-u', help="Synonym for --directory.")
+    parser.add_argument('--upload_folder', help="Synonym for --directory.")
+    parser.add_argument('--output', help="Output file for results.", default=False)
     parser.add_argument('--yes', action="store_true",
                         help="Suppress (yes/no) requests for user input.", default=False)
-    parser.add_argument('--no_query', '-nq', action="store_true",
-                        help="Synonym for --yes.", default=False)
-    parser.add_argument('--subfolders', '-sf', action="store_true",
-                        help="Obsolete", default=False)
     args = parser.parse_args(args=simulated_args_for_testing)
 
     directory_only = True
     if args.directory:
         args.upload_folder = args.directory
         directory_only = False
     if args.directory_only:
         args.upload_folder = args.directory_only
         directory_only = True
-    if args.bundle:
-        args.bundle_filename = args.bundle
 
     if args.yes:
         args.no_query = True
 
     if not args.uuid:
         PRINT("Missing submission UUID or referenced file UUID or accession ID.")
         exit(2)
@@ -95,16 +102,16 @@
             PRINT(f"The --keys argument ({keys_file}) must be the name of an existing .json file.")
             exit(1)
 
     if args.upload_folder and not os.path.isdir(args.upload_folder):
         PRINT(f"Directory does not exist: {args.upload_folder}")
         exit(1)
 
-    if args.bundle_filename and not os.path.isdir(os.path.normpath(os.path.dirname(args.bundle_filename))):
-        PRINT(f"Specified bundle file not found: {args.bundle_filename}")
+    if args.bundle and not os.path.isdir(os.path.normpath(os.path.dirname(args.bundle))):
+        PRINT(f"Specified bundle file not found: {args.bundle}")
         exit(1)
 
     if not args.upload_folder and args.directory:
         args.upload_folder = args.directory
 
     if args.upload_folder and not os.path.isdir(args.upload_folder):
         PRINT(f"Specified upload directory not found: {args.upload_folder}")
@@ -117,17 +124,18 @@
 
     with script_catch_errors():
 
         resume_uploads(uuid=args.uuid,
                        env=args.env,
                        env_from_env=env_from_env,
                        keys_file=keys_file,
-                       bundle_filename=args.bundle_filename,
+                       bundle_filename=args.bundle,
                        server=args.server,
                        upload_folder=args.upload_folder,
-                       no_query=args.no_query,
+                       no_query=args.yes,
                        subfolders=not directory_only,
+                       output_file=args.output,
                        app=args.app)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `smaht_submitr-0.7.0.1b9/submitr/scripts/show_upload_info.py` & `smaht_submitr-0.7.0.1b90/submitr/scripts/show_upload_info.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b9/submitr/scripts/submit_genelist.py` & `smaht_submitr-0.7.0.1b90/submitr/scripts/submit_genelist.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b9/submitr/scripts/submit_metadata_bundle.py` & `smaht_submitr-0.7.0.1b90/submitr/scripts/submit_metadata_bundle.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,19 @@
 from .cli_utils import CustomArgumentParser
 from ..base import DEFAULT_APP
 from ..submission import (
     submit_any_ingestion,
     DEFAULT_INGESTION_TYPE,
     DEFAULT_SUBMISSION_PROTOCOL,
     SUBMISSION_PROTOCOLS,
+    _define_portal,
+    _get_consortia,
+    _get_submission_centers,
     _ping,
+    _print_metadata_file_info,
     _pytesting
 )
 
 _HELP = f"""
 ===
 submit-metadata-bundle [VERSION]
 ===
@@ -41,22 +45,22 @@
   Default is to use the consortium associated with your account.
 --submission-center SUBMISSION-CENTER
   To specify your submission center.
   Default is to use the submission center associated with your account.
 --directory DIRECTORY
   To specify a directory containing the files to upload; in addition
   to the default of using the directory containing the submitted file;
-  this directory will be search, recursively.
+  this directory will be searched recursively.
 --keys KEYS-FILE
   To specify an alternate credentials/keys file,
   rather than the default ~/.smaht-keys.json file.
   Alternatively, set your SMAHT_KEYS environment variable.
 --output OUTPUT-FILE
   Writes all logging output to the specified file;
-  and refrains from printing lengthy content to stdout.
+  and refrains from printing lengthy content to output/stdout.
 --verbose
   Displays more verbose output.
 --help
   Displays this documentation.
 --help-advanced
   Displays this plus more advanced documentation.
 --doc
@@ -72,29 +76,43 @@
 --validate-only
   Same as --validate with slightly different command interaction.
   Performs ONLY, but BOTH client-side (local) and
   server-side (remote) validation only WITHOUT submitting.
 --validate-remote-only
   Performs ONLY server-side (remote) validation WITHOUT submitting.
 --validate-local-only
-  Performs ONLY client-side (local) validation WITHOUT submission.
+  Performs ONLY client-side (local) validation WITHOUT submitting.
 --validate-local-skip
   Skips client-side (local) validation.
 --validate-remote-skip
   Skips server-side (remote) validation.
+--noanalyze
+  Skips analysis of parsed metadata WRT creates/updates.
 --patch-only
   Perform ONLY updates (PATCHes) for submitted data.
 --post-only
   Perform ONLY creates (POSTs) for submitted data.
 --directory-only
   Same as --directory but does NOT search recursively.
+--add-submission-center SUBMISSION-CENTER
+  To specify an additional submission center as having access to
+  the ingestion submission (object). Useful when different users
+  will be performing submit-metadata-bundle and resume-uploads.
+--consortia
+  Displays ONLY all known consortia; nothing else.
+--submission-centers
+  Displays ONLY all known submission centers; nothing else.
 --json
   Displays the submitted metadata as formatted JSON.
 --json-only
   Displays ONLY the submitted metadata as formatted JSON; nothing else.
+--info
+  Displays ONLY info about the submitted metadata; nothing else.
+--info
+  Displays ONLY info about the submitted metadata; nothing else.
 --details
   Displays slightly more detailed output.
 --noprogress
   Do not print progress of (client-side) parsing/validation output.
 --timeout SECONDS
   Maximum umber of seconds to wait for server validation or submission.
 --progress-extra
@@ -103,50 +121,64 @@
   Displays some debugging related output.
 --ping
   Pings the server; to test connectivity.
 --yes
   Automatically answer 'yes' to any confirmation questions.
 ===
 """
+_OBSOLETE_OPTIONS = [
+    {"option": "-e", "message": "Use --env."},
+    {"option": "-s", "message": "Use --server."},
+    {"option": "-v", "message": "Use --validate."},
+    {"option": "-u", "message": "Use --directory-only; or --directory which searches recusively."},
+    {"option": "-d", "message": "Use --directory-only; or --directory which searches recusively."},
+    {"option": "-sd", "message": "Use --directory which defaults to searching recusively."},
+    {"option": "-sf", "message": "Use --directory which defaults to searching recusively."}
+]
 
 
 def main(simulated_args_for_testing=None):
-    parser = CustomArgumentParser(_HELP, _HELP_ADVANCED, CustomArgumentParser.HELP_URL, package="smaht-submitr")
+    parser = CustomArgumentParser(help=_HELP, help_advanced=_HELP_ADVANCED,
+                                  help_url=CustomArgumentParser.HELP_URL,
+                                  obsolete_options=_OBSOLETE_OPTIONS)
     parser.add_argument('bundle_filename', nargs="?", help='Local Excel filename that comprises the data bundle.')
-    parser.add_argument('--server', '-s',
+    parser.add_argument('--server',
                         help="HTTP(S) address of Portal server (e.g. in ~/.smaht-keys.json).")
-    parser.add_argument('--env', '-e',
+    parser.add_argument('--env',
                         help="Portal environment name for server/credentials (e.g. in ~/.smaht-keys.json).")
     parser.add_argument('--consortium', help="Consoritium to use for submission.")
     parser.add_argument('--submission-center', help="Submission center to use for submission.")
+    parser.add_argument('--consortia', action="store_true", help="List known consoritia.")
+    parser.add_argument('--submission-centers', action="store_true", help="List known submission centers.")
+    parser.add_argument('--add-submission-center', help="Add submission center to the IngestionSubmission object.")
     parser.add_argument('--post-only', action="store_true",
                         help="Only perform creates (POST) for submitted data.", default=False)
     parser.add_argument('--patch-only', action="store_true",
                         help="Only perform updates (PATCH) for submitted data.", default=False)
     parser.add_argument('--keys', help="Path to keys file (rather than default ~/.smaht-keys.json).", default=None)
     parser.add_argument('--submit', action="store_true",
                         help="Actually submit the metadata for ingestion..", default=False)
-    parser.add_argument('--validate', '-v', action="store_true",
+    parser.add_argument('--validate', action="store_true",
                         help="Perform both client-side and server-side validation first.", default=False)
     parser.add_argument('--validate-only', action="store_true",
                         help="Same as --validate.", default=False)
     parser.add_argument('--validate-local-only', action="store_true",
                         help="Validate submitted data locally only (on client-side).")
     parser.add_argument('--validate-remote-only', action="store_true",
                         help="Only perform validation of submitted data (on server-side).", default=False)
     parser.add_argument('--validate-local-skip', action="store_true",
                         help="Skip the local (client) validation step.", default=False)
     parser.add_argument('--validate-remote-skip', action="store_true",
                         help="Skip the remote (server) validation step.", default=False)
-    parser.add_argument('--directory', '-d', help="Directory of the upload files.")
+    parser.add_argument('--directory', help="Directory of the upload files.")
     parser.add_argument('--directory-only', help="Same as --directory but NOT recursively.", default=False)
-    parser.add_argument('--subfolders', '-sf', action="store_true",  # obsolete
+    parser.add_argument('--subfolders', action="store_true",  # obsolete
                         help="Obsolete", default=False)
-    parser.add_argument('--upload_folder', '-u', help="Same as --directory.")
-    parser.add_argument('--ingestion_type', '--ingestion-type', '-t',
+    parser.add_argument('--upload_folder', help="Same as --directory.")
+    parser.add_argument('--ingestion_type', '--ingestion-type',
                         help=f"The ingestion type (default: {DEFAULT_INGESTION_TYPE}).",
                         default=DEFAULT_INGESTION_TYPE)
     parser.add_argument('--yes', action="store_true",
                         help="Suppress (yes/no) requests for user input.", default=False)
     parser.add_argument('--no_query', '--no-query', '-nq', action="store_true",
                         help="Suppress (yes/no) requests for user input.", default=False)
     parser.add_argument('--ref-nocache', action="store_true",
@@ -161,18 +193,24 @@
                              f" Normally this should not be given.")
     parser.add_argument('--submission_protocol', '--submission-protocol', '-sp',
                         choices=SUBMISSION_PROTOCOLS, default=DEFAULT_SUBMISSION_PROTOCOL,
                         help=f"the submission protocol (default {DEFAULT_SUBMISSION_PROTOCOL!r})")
     parser.add_argument('--noadmin', action="store_true",
                         help="For testing only; assume not admin user.", default=False)
     parser.add_argument('--details', action="store_true", help="More details in output.", default=False)
+    parser.add_argument('--noanalyze', action="store_true",
+                        help="Do not analyze metadata for creates/updates to be done..", default=False)
     parser.add_argument('--json', action="store_true",
                         help="Output the parsed JSON of the metadata file.", default=False)
     parser.add_argument('--json-only', action="store_true",
                         help="Output ONLY the parsed JSON of the metadata file.", default=False)
+    parser.add_argument('--info', action="store_true",
+                        help="Output information about the given metadata file.", default=False)
+    parser.add_argument('--refs', action="store_true",
+                        help="Outputs list of references from the metadata file; only with --info.", default=False)
     parser.add_argument('--output', help="Output file for results.", default=False)
     parser.add_argument('--verbose', action="store_true", help="Debug output.", default=False)
     parser.add_argument('--timeout', help="Wait timeout for server validation/submission.")
     parser.add_argument('--debug', action="store_true", help="Debug output.", default=False)
     parser.add_argument('--debug-sleep', help="Sleep on each row read for troubleshooting/testing.", default=False)
     parser.add_argument('--ping', action="store_true", help="Ping server.", default=False)
     args = parser.parse_args(args=simulated_args_for_testing)
@@ -210,14 +248,36 @@
         if ping_okay:
             PRINT("Ping success. Your connection appears to be OK.")
             exit(0)
         else:
             PRINT("Ping failure. Your connection appears to be problematic.")
             exit(1)
 
+    if args.consortia or (args.bundle_filename and args.bundle_filename.lower() == "consortia"):
+        portal = _define_portal(env=args.env)
+        consortia = _get_consortia(portal)
+        PRINT("Known Consortia:")
+        for consortium in consortia:
+            if ((consortium_name := consortium.get("name")) and
+                (consortium_uuid := consortium.get("uuid"))):  # noqa
+                PRINT(f"- {consortium_name}: {consortium_uuid}")
+        exit(0)
+
+    if (args.submission_centers or
+        (args.bundle_filename and args.bundle_filename.lower() in
+         ["submission_centers", "submission-centers", "submissioncenters"])):
+        portal = _define_portal(env=args.env)
+        submission_centers = _get_submission_centers(portal)
+        PRINT("Known Submission Centers:")
+        for submission_center in submission_centers:
+            if ((submission_center_name := submission_center.get("name")) and
+                (submission_center_uuid := submission_center.get("uuid"))):  # noqa
+                PRINT(f"- {submission_center_name}: {submission_center_uuid}")
+        exit(0)
+
     _setup_validate_related_options(args)
 
     if not args.bundle_filename:
         PRINT("Missing submission file name.")
         exit(2)
 
     if args.upload_folder and not os.path.isdir(args.upload_folder):
@@ -236,38 +296,47 @@
 
     if args.timeout:
         if not args.timeout.isdigit():
             args.timeout = None
         else:
             args.timeout = int(args.timeout)
 
+    if args.info:
+        if not os.path.exists(args.bundle_filename):
+            PRINT(f"File does not exist: {args.bundle_filename}")
+            exit(1)
+        _print_metadata_file_info(args.bundle_filename, env=args.env, refs=args.refs, output_file=args.output)
+        exit(0)
+
     with script_catch_errors():
 
         if not _sanity_check_submitted_file(args.bundle_filename):
             exit(1)
 
         submit_any_ingestion(ingestion_filename=args.bundle_filename, ingestion_type=args.ingestion_type,
                              env=args.env, env_from_env=env_from_env,
                              keys_file=keys_file,
                              server=args.server,
                              consortium=args.consortium,
                              submission_center=args.submission_center,
+                             add_submission_center=args.add_submission_center,
                              no_query=args.no_query,
                              subfolders=not directory_only,
                              app=args.app,
                              submission_protocol=args.submission_protocol,
                              upload_folder=args.upload_folder,
                              show_details=args.details,
                              post_only=args.post_only,
                              patch_only=args.patch_only,
                              submit=args.submit,
                              validate_local_only=args.validate_local_only,
                              validate_remote_only=args.validate_remote_only,
                              validate_local_skip=args.validate_local_skip,
                              validate_remote_skip=args.validate_remote_skip,
+                             noanalyze=args.noanalyze,
                              json_only=args.json_only,
                              ref_nocache=args.ref_nocache,
                              verbose_json=args.json,
                              verbose=args.verbose,
                              noprogress=args.noprogress,
                              output_file=args.output,
                              timeout=args.timeout,
@@ -296,14 +365,17 @@
             return False
 
     return True
 
 
 def _setup_validate_related_options(args: argparse.Namespace):
 
+    if args.info:
+        return
+
     if args.submit:
         if args.validate or args.validate_only or args.validate_local_only or args.validate_remote_only:
             PRINT(f"May not specify both --submit AND validate options.")
             exit(1)
         if args.json_only:
             PRINT(f"May not specify both --submit AND --json-only options.")
             exit(1)
```

### Comparing `smaht_submitr-0.7.0.1b9/submitr/scripts/submit_ontology.py` & `smaht_submitr-0.7.0.1b90/submitr/scripts/submit_ontology.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b9/submitr/scripts/upload_item_data.py` & `smaht_submitr-0.7.0.1b90/submitr/scripts/upload_item_data.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b9/submitr/scripts/view_portal_object.py` & `smaht_submitr-0.7.0.1b90/submitr/scripts/view_portal_object.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,15 @@
 # Note that instead of a uuid you can also actually use a path, for example:
 #   view-local-object /file-formats/vcf_gz_tbi
 #
 # --------------------------------------------------------------------------------------------------
 
 import argparse
 from functools import lru_cache
+import io
 import json
 import pyperclip
 import os
 import sys
 from typing import Callable, List, Optional, Tuple
 import yaml
 from dcicutils.captured_output import captured_output, uncaptured_output
@@ -93,14 +94,18 @@
                         help=f"Application name (one of: smaht, cgap, fourfront).")
     parser.add_argument("--schema", action="store_true", required=False, default=False,
                         help="View named schema rather than object.")
     parser.add_argument("--all", action="store_true", required=False, default=False,
                         help="Include all properties for schema usage.")
     parser.add_argument("--raw", action="store_true", required=False, default=False, help="Raw output.")
     parser.add_argument("--tree", action="store_true", required=False, default=False, help="Tree output for schemas.")
+    parser.add_argument("--post", type=str, required=False, default=None,
+                        help="POST data of the main arg type with data from file specified with this option.")
+    parser.add_argument("--patch", type=str, required=False, default=None,
+                        help="PATCH data of the main arg type with data from file specified with this option.")
     parser.add_argument("--database", action="store_true", required=False, default=False,
                         help="Read from database output.")
     parser.add_argument("--bool", action="store_true", required=False,
                         default=False, help="Only return whether found or not.")
     parser.add_argument("--yaml", action="store_true", required=False, default=False, help="YAML output.")
     parser.add_argument("--copy", "-c", action="store_true", required=False, default=False,
                         help="Copy object data to clipboard.")
@@ -149,14 +154,21 @@
             _print("Known File Formats: None")
         return
 
     if _is_maybe_schema_name(args.uuid):
         args.schema = True
 
     if args.schema:
+        if args.post:
+            if post_data := _read_json_from_file(args.post):
+                if args.verbose:
+                    _print(f"POSTing data from file ({args.post}) as type: {args.uuid}")
+                portal.post_metadata(args.uuid, post_data)
+                if args.verbose:
+                    _print(f"Done POSTing data from file ({args.post}) as type: {args.uuid}")
         schema, schema_name = _get_schema(portal, args.uuid)
         if schema:
             if args.copy:
                 pyperclip.copy(json.dumps(schema, indent=4))
             if not args.raw:
                 if parent_schema_name := _get_parent_schema_name(schema):
                     if schema.get("isAbstract") is True:
@@ -164,14 +176,25 @@
                     else:
                         _print(f"{schema_name} | parent: {parent_schema_name}")
                 else:
                     _print(schema_name)
             _print_schema(schema, details=args.details, more_details=args.details,
                           all=args.all, raw=args.raw, raw_yaml=args.yaml)
             return
+    elif args.patch:
+        if patch_data := _read_json_from_file(args.patch):
+            if args.verbose:
+                _print(f"PATCHing data from file ({args.patch}) for object: {args.uuid}")
+            portal.patch_metadata(args.uuid, patch_data)
+            if args.verbose:
+                _print(f"Done PATCHing data from file ({args.patch}) as type: {args.uuid}")
+            return
+        else:
+            _print(f"No PATCH data found in file: {args.patch}")
+            exit(1)
 
     data = _get_portal_object(portal=portal, uuid=args.uuid, raw=args.raw,
                               database=args.database, check=args.bool, verbose=args.verbose)
     if args.bool:
         if data:
             _print(f"{args.uuid}: found")
             exit(0)
@@ -227,15 +250,18 @@
             return None
         _exit(f"Null response getting Portal object from {portal.server}: {uuid}")
     if response.status_code not in [200, 307]:
         # TODO: Understand why the /me endpoint returns HTTP status code 307, which is only why we mention it above.
         _exit(f"Invalid status code ({response.status_code}) getting Portal object from {portal.server}: {uuid}")
     if not response.json:
         _exit(f"Invalid JSON getting Portal object: {uuid}")
-    return response.json()
+    response = response.json()
+    if raw:
+        response.pop("schema_version", None)
+    return response
 
 
 @lru_cache(maxsize=1)
 def _get_schemas(portal: Portal) -> Optional[dict]:
     return portal.get_schemas()
 
 
@@ -541,14 +567,31 @@
                 extension = branch if pointer == tee else space
                 yield from tree_generator(path, prefix=prefix+extension)
     print(first + ((name_of(root_name) if callable(name_of) else root_name) or "root"))
     for line in tree_generator(root_name, prefix="   "):
         print(line)
 
 
+def _read_json_from_file(file: str) -> Optional[dict]:
+    if not os.path.exists(file):
+        _print(f"Cannot find file: {file}")
+        exit(1)
+    try:
+        with io.open(file, "r") as f:
+            try:
+                return json.load(f)
+            except Exception:
+                _print(f"Cannot parse JSON in file: {file}")
+                exit(1)
+    except Exception as e:
+        print(e)
+        _print(f"Cannot open file: {file}")
+        exit(1)
+
+
 def _print(*args, **kwargs):
     with uncaptured_output():
         PRINT(*args, **kwargs)
     sys.stdout.flush()
 
 
 def _exit(message: Optional[str] = None) -> None:
```

### Comparing `smaht_submitr-0.7.0.1b9/submitr/submission.py` & `smaht_submitr-0.7.0.1b90/submitr/submission.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,56 +2,67 @@
 import boto3
 from botocore.exceptions import NoCredentialsError as BotoNoCredentialsError
 from datetime import datetime
 from functools import lru_cache
 import io
 import json
 import os
-from pathlib import Path
-import pytz
 import re
-import signal
-import subprocess
 import sys
 import time
-from tqdm import tqdm
 from typing import Any, BinaryIO, Dict, List, Optional, Tuple
 import yaml
 
 # get_env_real_url would rely on env_utils
 # from dcicutils.env_utils import get_env_real_url
 from dcicutils.command_utils import yes_or_no
 from dcicutils.common import APP_CGAP, APP_FOURFRONT, APP_SMAHT, OrchestratedApp
 from dcicutils.file_utils import search_for_file
 from dcicutils.function_cache_decorator import function_cache
 from dcicutils.lang_utils import conjoined_list, disjoined_list, there_are
 from dcicutils.misc_utils import (
-    environ_bool, is_uuid, url_path_join, ignorable, normalize_spaces, remove_prefix, str_to_bool
+    environ_bool, is_uuid, url_path_join, ignorable, normalize_spaces, remove_prefix
 )
 from dcicutils.s3_utils import HealthPageKey
 from dcicutils.schema_utils import EncodedSchemaConstants, JsonSchemaConstants, Schema
 from dcicutils.structured_data import Portal, StructuredDataSet
+from dcicutils.submitr.progress_constants import PROGRESS_INGESTER, PROGRESS_LOADXL, PROGRESS_PARSE
+from dcicutils.submitr.ref_lookup_strategy import ref_lookup_strategy
 from typing_extensions import Literal
 from urllib.parse import urlparse
-from .base import DEFAULT_APP
-from .exceptions import PortalPermissionError
-from .scripts.cli_utils import print_boxed
-from .utils import keyword_as_title
-from .output import PRINT, PRINT_OUTPUT, PRINT_STDOUT, SHOW, get_output_file, setup_for_output_file_option
+from submitr.base import DEFAULT_APP
+from submitr.exceptions import PortalPermissionError
+from submitr.output import PRINT, PRINT_OUTPUT, PRINT_STDOUT, SHOW, get_output_file, setup_for_output_file_option
+from submitr.progress_bar import ProgressBar
+from submitr.scripts.cli_utils import get_version
+from submitr.s3_utils import upload_file_to_aws_s3
+from submitr.utils import (
+    format_datetime, format_size, format_path,
+    get_file_checksum, get_file_md5, get_file_md5_like_aws_s3_etag,
+    get_file_modified_datetime, get_file_size, get_s3_bucket_and_key_from_s3_uri,
+    print_boxed, keyword_as_title, tobool
+)
+
+
+def set_output_file(output_file):
+    if output_file:
+        global PRINT, PRINT_OUTPUT, PRINT_STDOUT, SHOW
+        PRINT, PRINT_OUTPUT, PRINT_STDOUT, SHOW = setup_for_output_file_option(output_file)
 
 
 DEFAULT_INGESTION_TYPE = 'metadata_bundle'
 GENERIC_SCHEMA_TYPE = 'FileOther'
 
+
 # Maximum amount of time (approximately) we will wait for a response from server (seconds).
 PROGRESS_TIMEOUT = 60 * 5  # five minutes (note this is for both server validation and submission)
 # How often we actually check the server (seconds).
-PROGRESS_CHECK_SERVER_INTERVAL = 5
+PROGRESS_CHECK_SERVER_INTERVAL = 3  # xyzzy
 # How often the (tqdm) progress meter updates (seconds).
-PROGRESS_INTERVAL = 1.0
+PROGRESS_INTERVAL = 1  # xyzzy
 # How many times the (tqdm) progress meter updates (derived from above).
 PROGRESS_MAX_CHECKS = round(PROGRESS_TIMEOUT / PROGRESS_INTERVAL)
 
 
 class SubmissionProtocol:
     S3 = 's3'
     UPLOAD = 'upload'
@@ -117,15 +128,17 @@
     if not quiet:
         SHOW(f"Portal server recognizes you as{' (admin)' if _is_admin_user(user_record) else ''}:"
              f" {user_record['title']} ({user_record['contact_email']})")
     return user_record
 
 
 def _is_admin_user(user: dict) -> bool:
-    return False if os.environ.get("SMAHT_NOADMIN") else ("admin" in user.get("groups", []))
+    if tobool(os.environ.get("SMAHT_NOADMIN")):
+        return False
+    return "admin" in user.get("groups", []) if isinstance(user, dict) else False
 
 
 def _get_defaulted_institution(institution, user_record, portal=None, quiet=False, verbose=False):
     """
     Returns the given institution or else if none is specified, it tries to infer an institution.
 
     :param institution: the @id of an institution, or None
@@ -293,15 +306,14 @@
 
     :param submission_centers: the @id of a submission center, or None
     :param user_record: the user record for the authorized user
     :param error_if_none: boolean true if failure to infer a submission center should raise an error,
         and false otherwise.
     :return: the @id of a submission center to use
     """
-    # TODO: Need to support submits_for ...
     def show_submission_centers():
         nonlocal portal
         if portal:
             if submission_centers := _get_submission_centers(portal):
                 SHOW("SUBMISSION CENTERS SUPPORTED:")
                 for submission_center in submission_centers:
                     SHOW(f"- {submission_center.get('name')} ({submission_center.get('uuid')})")
@@ -457,23 +469,28 @@
 # TRY_OLD_PROTOCOL = True
 DEBUG_PROTOCOL = environ_bool("DEBUG_PROTOCOL", default=False)
 
 
 def _initiate_server_ingestion_process(
         portal: Portal,
         ingestion_filename: str,
-        consortia: Optional[List[str]],
-        submission_centers: Optional[List[str]],
+        consortia: Optional[List[str]] = None,
+        submission_centers: Optional[List[str]] = None,
+        add_submission_center: Optional[str] = None,
         is_server_validation: bool = False,
         is_resume_submission: bool = False,
         validation_ingestion_submission_object: Optional[dict] = None,
         post_only: bool = False,
         patch_only: bool = False,
         autoadd: Optional[dict] = None,
-        debug: bool = False) -> str:
+        datafile_size: Optional[Any] = None,
+        datafile_checksum: Optional[Any] = None,
+        user: Optional[dict] = None,
+        debug: bool = False,
+        debug_sleep: Optional[str] = None) -> str:
 
     if isinstance(validation_ingestion_submission_object, dict):
         # This ingestion action is for a submission (rather than for a validation),
         # and we were given an associated validation UUID (i.e. from a previous client
         # initiated server validation); so we record this validation UUID in the actual
         # submission IngestionSubmission object (to be created just below); and we will
         # do the converse below, after the submission IngestionSubmission object creation.
@@ -487,30 +504,36 @@
 
     submission_post_data = {
         "validate_only": is_server_validation,
         "post_only": post_only,
         "patch_only": patch_only,
         "ref_nocache": False,  # Do not do this server-side at all; only client-side for testing.
         "autoadd": json.dumps(autoadd),
-        "ingestion_directory": os.path.dirname(ingestion_filename) if ingestion_filename else None
+        "ingestion_directory": os.path.dirname(ingestion_filename) if ingestion_filename else None,
+        "datafile_size": datafile_size or get_file_size(ingestion_filename),
+        "datafile_checksum": datafile_checksum or get_file_checksum(ingestion_filename),
+        "user": json.dumps(user)
     }
 
     if validation_ingestion_submission_uuid:
         submission_post_data["validation_uuid"] = validation_ingestion_submission_uuid
+    if debug_sleep:
+        submission_post_data["debug_sleep"] = debug_sleep
 
     if is_resume_submission and validation_ingestion_submission_object:
         if validation_parameters := validation_ingestion_submission_object.get("parameters"):
             submission_post_data["validation_datafile"] = validation_parameters.get("datafile")
             submission_post_data["ingestion_directory"] = validation_parameters.get("ingestion_directory")
 
     response = _post_submission(portal=portal,
                                 is_resume_submission=is_resume_submission,
                                 ingestion_filename=ingestion_filename,
                                 consortia=consortia,
                                 submission_centers=submission_centers,
+                                add_submission_center=add_submission_center,
                                 submission_post_data=submission_post_data,
                                 is_server_validation=is_server_validation, debug=debug)
     submission_uuid = response["submission_id"]
 
     if validation_ingestion_submission_uuid and validation_parameters:
         # This ingestion action is for a submission (rather than for a validation),
         # and we were given an associated validation UUID (i.e. from a previous client
@@ -524,24 +547,29 @@
 
 
 def _post_submission(portal: Portal,
                      ingestion_filename: str,
                      consortia: List[str],
                      submission_centers: List[str],
                      submission_post_data: dict,
+                     add_submission_center: Optional[str] = None,
                      ingestion_type: str = DEFAULT_INGESTION_TYPE,
                      submission_protocol: str = DEFAULT_SUBMISSION_PROTOCOL,
                      is_server_validation: bool = False,
                      is_resume_submission: bool = False,
                      debug: bool = False):
+
+    creation_submission_centers = [*submission_centers]
+    if isinstance(add_submission_center, str) and (add_submission_center not in creation_submission_centers):
+        creation_submission_centers.append(add_submission_center)
     creation_post_data = {
         "ingestion_type": ingestion_type,
         "processing_status": {"state": "submitted"},
         "consortia": consortia,
-        "submission_centers": submission_centers
+        "submission_centers": creation_submission_centers
     }
     if is_server_validation:
         creation_post_data["parameters"] = {"validate_only": True}
     # This creates the IngestionSubmission object.
     creation_post_url = url_path_join(portal.server, INGESTION_SUBMISSION_TYPE_NAME)
     creation_response = portal.post(creation_post_url, json=creation_post_data, raise_for_status=True)
     [submission] = creation_response.json()['@graph']
@@ -639,28 +667,30 @@
                          env,
                          institution=None,
                          project=None,
                          lab=None,
                          award=None,
                          consortium=None,
                          submission_center=None,
+                         add_submission_center=None,
                          app: OrchestratedApp = None,
                          upload_folder=None,
                          no_query=False,
                          subfolders=False,
                          submission_protocol=DEFAULT_SUBMISSION_PROTOCOL,
                          submit=False,
                          validate_local_only=False,
                          validate_remote_only=False,
                          validate_local_skip=False,
                          validate_remote_skip=False,
                          post_only=False,
                          patch_only=False,
                          keys_file=None,
                          show_details=False,
+                         noanalyze=False,
                          json_only=False,
                          ref_nocache=False,
                          verbose_json=False,
                          verbose=False,
                          noprogress=False,
                          output_file=None,
                          env_from_env=False,
@@ -703,20 +733,21 @@
     # Setup for output to specified output file, in addition to stdout),
     # except in this case we will not output large amounts of output to stdout.
     if output_file:
         global PRINT, PRINT_OUTPUT, PRINT_STDOUT, SHOW
         PRINT, PRINT_OUTPUT, PRINT_STDOUT, SHOW = setup_for_output_file_option(output_file)
 
     portal = _define_portal(env=env, env_from_env=env_from_env, server=server, app=app,
-                            keys_file=keys_file, report=not json_only or verbose, verbose=verbose)
+                            keys_file=keys_file, report=not json_only or verbose, verbose=verbose,
+                            note="Metadata Validation" if validation else "Metadata Submission")
 
     app_args = _resolve_app_args(institution=institution, project=project, lab=lab, award=award, app=portal.app,
                                  consortium=consortium, submission_center=submission_center)
 
-    if portal.get("/health").status_code != 200:  # TODO: with newer version dcicutils do: if not portal.ping():
+    if not portal.ping():
         SHOW(f"Portal credentials do not seem to work: {portal.keys_file} ({env})")
         exit(1)
 
     user_record = _get_user_record(portal.server, auth=portal.key_pair, quiet=json_only and not verbose)
     # Nevermind: Too confusing for both testing and general usage
     # to have different behaviours for admin and non-admin users.
     # is_admin_user = _is_admin_user(user_record)
@@ -737,41 +768,57 @@
         PRINT(f"DEBUG: validate_local_skip = {validate_local_skip}")
         PRINT(f"DEBUG: validate_remote_skip = {validate_remote_skip}")
 
     metadata_bundles_bucket = get_metadata_bundles_bucket_from_health_path(key=portal.key)
     if not _do_app_arg_defaulting(app_args, user_record, portal, quiet=json_only and not verbose, verbose=verbose):
         pass
     if not json_only:
-        PRINT(f"Submission file to {'validate' if validation else 'ingest'}: {_format_path(ingestion_filename)}")
+        PRINT(f"Submission file to {'validate' if validation else 'ingest'}: {format_path(ingestion_filename)}")
 
     autoadd = None
     if app_args and isinstance(submission_centers := app_args.get("submission_centers"), list):
         if len(submission_centers) == 1:
             def extract_identifying_value_from_path(path: str) -> str:
                 if path.endswith("/"):
                     path = path[:-1]
                 parts = path.split("/")
                 return parts[-1] if parts else ""
             autoadd = {"submission_centers": [extract_identifying_value_from_path(submission_centers[0])]}
         elif len(submission_centers) > 1:
             PRINT(f"Multiple submission centers: {', '.join(submission_centers)}")
             PRINT(f"You must specify onely one submission center using the --submission-center option.")
             exit(1)
+
+    if add_submission_center:
+        if not _is_admin_user(user_record):
+            PRINT("ERROR: Cannot use the --add-submission-center if you are not an admin user.")
+            exit(1)
+        known_submission_centers = _get_submission_centers(portal)
+        found_submission_centers = [submission_center for submission_center in known_submission_centers
+                                    if (submission_center.get("name") == add_submission_center) or
+                                       (submission_center.get("uuid") == add_submission_center)]
+        if not found_submission_centers or not found_submission_centers[0].get("uuid"):
+            PRINT(f"ERROR: Specified submission center ({add_submission_center}) not found. Use one of:")
+            for known_submission_center in known_submission_centers:
+                PRINT(f"- {known_submission_center.get('name')} ({known_submission_center.get('uuid')})")
+            exit(1)
+        add_submission_center = f"/submission-centers/{found_submission_centers[0]['uuid']}/"
+
     if verbose:
         SHOW(f"Metadata bundle upload bucket: {metadata_bundles_bucket}")
 
     if not validate_remote_only and not validate_local_skip:
-        _validate_locally(ingestion_filename, portal,
-                          validation=validation,
-                          validate_local_only=validate_local_only,
-                          autoadd=autoadd, upload_folder=upload_folder, subfolders=subfolders,
-                          exit_immediately_on_errors=exit_immediately_on_errors,
-                          ref_nocache=ref_nocache, output_file=output_file, noprogress=noprogress,
-                          json_only=json_only, verbose_json=verbose_json,
-                          verbose=verbose, debug=debug, debug_sleep=debug_sleep)
+        structured_data = _validate_locally(ingestion_filename, portal,
+                                            validation=validation,
+                                            validate_local_only=validate_local_only,
+                                            autoadd=autoadd, upload_folder=upload_folder, subfolders=subfolders,
+                                            exit_immediately_on_errors=exit_immediately_on_errors,
+                                            ref_nocache=ref_nocache, output_file=output_file, noprogress=noprogress,
+                                            noanalyze=noanalyze, json_only=json_only, verbose_json=verbose_json,
+                                            verbose=verbose, debug=debug, debug_sleep=debug_sleep)
         if validate_local_only:
             # We actually do exit from _validate_locally if validate_local_only is True.
             # This return is just emphasize that fact.
             return
     else:
         PRINT(f"Skipping local (client) validation (as requested via"
               f" {'--validate-remote-only' if validate_remote_only else '--validate-local-skip'}).")
@@ -788,23 +835,28 @@
     # Server validation.
 
     if not validate_local_only and not validate_remote_skip:
 
         SHOW(f"Continuing with additional (server) validation: {portal.server}")
 
         validation_uuid = _initiate_server_ingestion_process(
-            is_server_validation=True,
             portal=portal,
             ingestion_filename=ingestion_filename,
+            is_server_validation=True,
             consortia=app_args.get("consortia"),
             submission_centers=app_args.get("submission_centers"),
+            add_submission_center=add_submission_center,
             post_only=post_only,
             patch_only=patch_only,
             autoadd=autoadd,
-            debug=debug)
+            user={"uuid": user_record.get("uuid"),
+                  "email": user_record.get("email"),
+                  "name": user_record.get("display_title")} if user_record else None,
+            debug=debug,
+            debug_sleep=debug_sleep)
 
         SHOW(f"Validation tracking ID: {validation_uuid}")
 
         server_validation_done, server_validation_status, server_validation_response = _monitor_ingestion_process(
                 validation_uuid, portal.server, portal.env, app=portal.app, keys_file=portal.keys_file,
                 show_details=show_details, report=False, messages=True,
                 validation=True,
@@ -822,29 +874,34 @@
               f" {'--validate-local-only' if validate_local_only else '--validate-remote-skip'}).")
 
     if validation:
         exit(0)
 
     # Server submission.
 
-    SHOW(f"Ready to submit your metadata to {portal.server}: {_format_path(ingestion_filename)}")
+    SHOW(f"Ready to submit your metadata to {portal.server}: {format_path(ingestion_filename)}")
     if not yes_or_no("Continue on with the actual submission?"):
         exit(0)
 
     submission_uuid = _initiate_server_ingestion_process(
-        is_server_validation=False,
-        validation_ingestion_submission_object=server_validation_response,
         portal=portal,
         ingestion_filename=ingestion_filename,
+        is_server_validation=False,
+        validation_ingestion_submission_object=server_validation_response,
         consortia=app_args.get("consortia"),
         submission_centers=app_args.get("submission_centers"),
+        add_submission_center=add_submission_center,
         post_only=post_only,
         patch_only=patch_only,
         autoadd=autoadd,
-        debug=debug)
+        user={"uuid": user_record.get("uuid"),
+              "email": user_record.get("email"),
+              "name": user_record.get("display_title")} if user_record else None,
+        debug=debug,
+        debug_sleep=debug_sleep)
 
     SHOW(f"Submission tracking ID: {submission_uuid}")
 
     submission_done, submission_status, submission_response = _monitor_ingestion_process(
             submission_uuid, portal.server, portal.env, app=portal.app, keys_file=portal.keys_file,
             show_details=show_details, report=False, messages=True,
             validation=False,
@@ -852,23 +909,28 @@
             verbose=verbose, debug=debug, debug_sleep=debug_sleep)
 
     if submission_status != "success":
         exit(1)
 
     PRINT("Submission complete!")
 
+    # Now that submission has successfully complete, review the files to upload and then do it.
+
+    _review_upload_files(structured_data, ingestion_filename,
+                         validation=validation, directory=upload_folder, recursive=subfolders)
+
     do_any_uploads(submission_response, keydict=portal.key, ingestion_filename=ingestion_filename,
                    upload_folder=upload_folder, no_query=no_query,
-                   subfolders=subfolders)
+                   subfolders=subfolders, portal=portal)
 
 
 def _get_recent_submissions(portal: Portal, count: int = 30, name: Optional[str] = None) -> List[dict]:
     url = f"/search/?type=IngestionSubmission&sort=-date_created&from=0&limit={count}"
     if name:
-        # TODO: Does not seem to return the same stuff
+        # TODO: Does not seem to return the same stuff; of not great consequence yet.
         url += f"&q={name}"
     if submissions := portal.get_metadata(url):
         if submissions := submissions.get("@graph"):
             return submissions
     return []
 
 
@@ -903,20 +965,20 @@
         lines.append("===")
         index = 0
         for submission in submissions:
             if details and (index > 0):
                 lines.append("===")
             if verbose:
                 PRINT()
-                _print_submission_summary(portal, submission)
+                _print_submission_summary(portal, submission, verbose=verbose)
                 continue
             submission_uuid = submission.get("uuid")
             submission_created = submission.get("date_created")
             line = f"{submission_uuid}: {_format_portal_object_datetime(submission_created)}"
-            if _tobool(submission.get("parameters", {}).get("validate_only")):
+            if tobool(submission.get("parameters", {}).get("validate_only")):
                 line += f" (V)"
             else:
                 line += f" (S)"
             if submission.get("processing_status", {}).get("outcome") == "success":
                 line += f" ▶ OK"
             lines.append(line)
             if details:
@@ -945,234 +1007,333 @@
 
 
 def _monitor_ingestion_process(uuid: str, server: str, env: str, keys_file: Optional[str] = None,
                                app: Optional[OrchestratedApp] = None,
                                show_details: bool = False,
                                validation: bool = False,
                                env_from_env: bool = False,
-                               verbose: bool = False,
                                report: bool = True, messages: bool = False,
                                nofiles: bool = False, noprogress: bool = False,
                                check_submission_script: bool = False,
                                upload_directory: Optional[str] = None,
                                upload_directory_recursive: bool = False,
                                timeout: Optional[int] = None,
-                               debug: bool = False,
+                               verbose: bool = False, debug: bool = False,
+                               note: Optional[str] = None,
+                               output_file: Optional[str] = None,
                                debug_sleep: Optional[int] = None) -> Tuple[bool, str, dict]:
 
+    if output_file:
+        set_output_file(output_file)
+
     if timeout:
         global PROGRESS_TIMEOUT, PROGRESS_MAX_CHECKS
         PROGRESS_TIMEOUT = timeout
         PROGRESS_MAX_CHECKS = max(round(PROGRESS_TIMEOUT / PROGRESS_INTERVAL), 1)
 
     def define_progress_callback(max_checks: int, title: str, include_status: bool = False) -> None:
-        bar = None
+        nonlocal validation
+        bar = ProgressBar(max_checks, "Calculating",
+                          interrupt_exit=True,
+                          interrupt_message=f"{'validation' if validation else 'submission'} waiting process")
         nchecks = 0
         nchecks_server = 0
         check_status = "Unknown"
         next_check = 0
-        def handle_control_c(signum, frame):  # noqa
-            if yes_or_no("\nCTRL-C: You have interrupted this process. Do you want to TERMINATE processing?"):
-                PRINT("Premature exit.")
-                exit(1)
-            PRINT_STDOUT("Continuing ...")
+        # From (new/2024-03-25) /ingestion-status/{submission_uuid} call.
+        loadxl_total = 0
+        loadxl_started = None
+        loadxl_started_second_round = None
         def progress_report(status: dict) -> None:  # noqa
-            nonlocal bar, max_checks, nchecks, nchecks_server, next_check, check_status, noprogress
+            nonlocal bar, max_checks, nchecks, nchecks_server, next_check, check_status, noprogress, validation
+            nonlocal loadxl_total, loadxl_started, loadxl_started_second_round, verbose
             if noprogress:
                 return
+            # This are from the (new/2024-03-25) /ingestion-status/{submission_uuid} call.
+            # Some of these key name come ultimately from snovault.loadxl.PROGRESS; others
+            # from smaht-portal/ingestion. Note difference between ingester_initiated and
+            # loadxl_started; the former is when the ingester listener is first hit.
+            ingester_initiated = status.get(PROGRESS_INGESTER.INITIATE, None)
+            ingester_parse_started = status.get(PROGRESS_INGESTER.PARSE_LOAD_INITIATE, None)
+            ingester_validate_started = status.get(PROGRESS_INGESTER.VALIDATE_LOAD_INITIATE, None)
+            ingester_queued = status.get(PROGRESS_INGESTER.QUEUED, None)
+            ingester_cleanup = status.get(PROGRESS_INGESTER.CLEANUP, None)
+            ingester_queue_cleanup = status.get(PROGRESS_INGESTER.QUEUE_CLEANUP, None)
+            loadxl_initiated = status.get(PROGRESS_INGESTER.LOADXL_INITIATE, None)
+            loadxl_total = status.get(PROGRESS_LOADXL.TOTAL, 0)
+            loadxl_started = status.get(PROGRESS_LOADXL.START, None)
+            loadxl_item = status.get(PROGRESS_LOADXL.ITEM, 0)
+            loadxl_started_second_round = status.get(PROGRESS_LOADXL.START_SECOND_ROUND, None)
+            loadxl_item_second_round = status.get(PROGRESS_LOADXL.ITEM_SECOND_ROUND, 0)
+            loadxl_done = status.get(PROGRESS_LOADXL.DONE, None)
+            # This string is from the /ingestion-status endpoint, really as a convenience/courtesey
+            # so we don't have to cobble together our own string; but we could also build the
+            # message ourselves manually here from the counts contained in the same response.
+            ingestion_message = (status.get("loadxl_message_verbose", "")
+                                 if verbose else status.get("loadxl_message", ""))
+            # Phases: 0 means waiting for server response; 1 means loadxl round one; 2 means loadxl round two.
+            loadxl_phase = 2 if loadxl_started_second_round is not None else (1 if loadxl_started is not None else 0)
             done = False
-            if status.get("start"):
-                signal.signal(signal.SIGINT, handle_control_c)
-                bar_format = "{l_bar}{bar}| {n_fmt}/{total_fmt} | {rate_fmt} | {elapsed}{postfix} | ETA: {remaining} "
-                bar = tqdm(total=max_checks, desc="Calculating", dynamic_ncols=True, bar_format=bar_format, unit="")
-                return
-            elif status.get("finish") or nchecks >= max_checks:
+            if status.get("finish") or nchecks >= max_checks:
                 check_status = status.get("status")
-                bar.update(max_checks - nchecks)
+                if loadxl_phase == 0:
+                    bar.increment_progress(max_checks - nchecks)
                 done = True
             elif status.get("check_server"):
                 check_status = status.get("status")
                 nchecks_server += 1
             elif status.get("check"):
                 if (next_check := status.get("next")) is not None:
                     next_check = round(status.get("next") or 0)
                 nchecks += 1
-                bar.update(1)
-            message = f"▶ {title} Checks: {nchecks_server}"
+                if loadxl_phase == 0:
+                    bar.increment_progress(1)
+            # message = f"▶ {title} Pings: {nchecks_server}"
+            message = f"▶ Pings: {nchecks_server}"
+            if loadxl_started is None:
+                if loadxl_initiated is not None:
+                    message += f" | Initializing"
+                elif ingester_parse_started is not None:
+                    message += f" | Parsing"
+                elif ingester_validate_started is not None:
+                    message += f" | Validating"
+                elif ingester_initiated is not None:
+                    message += f" | Acknowledged"
+                elif ingester_queued is not None:
+                    message += f" | Queued"
+                else:
+                    message += f" | Waiting on server"
+            else:
+                if loadxl_done is not None:
+                    bar.set_total(loadxl_total)
+                    bar.set_progress(loadxl_total)
+                elif loadxl_phase == 2:
+                    bar.set_total(loadxl_total)
+                    bar.set_progress(loadxl_item_second_round)
+                elif loadxl_phase == 1:
+                    bar.set_total(loadxl_total)
+                    bar.set_progress(loadxl_item)
+                if (ingester_queue_cleanup is not None) or done:
+                    message += " | Done"
+                elif ingester_cleanup is not None:
+                    message += " | Cleanup"
+                elif loadxl_done is not None:
+                    message += " | Finishing Up"
+                if ingestion_message:
+                    message += " | " + ingestion_message
             if include_status:
                 message += f" | Status: {check_status}"
-            message += f" | Next: {'Now' if next_check == 0 else str(next_check) + 's'} ‖ Progress"
+            # message += f" | Next: {'Now' if next_check == 0 else str(next_check) + 's'} ‖ Progress"
             bar.set_description(message)
             if done:
-                bar.close()
-                signal.signal(signal.SIGINT, signal.SIG_DFL)
+                bar.done()
         return progress_report
 
-    portal = _define_portal(env=env, server=server, app=app or DEFAULT_APP, env_from_env=env_from_env, report=report)
+    portal = _define_portal(env=env, server=server, app=app or DEFAULT_APP,
+                            env_from_env=env_from_env, report=report, note=note)
 
     if not (uuid_metadata := portal.get_metadata(uuid)):
         message = f"Submission ID not found: {uuid}" if uuid != "dummy" else "No submission ID specified."
         if _print_recent_submissions(portal, message=message):
             return
         raise Exception(f"Cannot find object given uuid: {uuid}")
     if not portal.is_schema_type(uuid_metadata, INGESTION_SUBMISSION_TYPE_NAME):
         undesired_type = portal.get_schema_type(uuid_metadata)
         raise Exception(f"Given ID is not for a submission or validation: {uuid} ({undesired_type})"
                         f" | Accession: {uuid_metadata.get('accession')}")
-    if _tobool(uuid_metadata.get("parameters", {}).get("validate_only")):
+    if tobool(uuid_metadata.get("parameters", {}).get("validate_only")):
         validation = True
 
     action = "validation" if validation else "ingestion"
     if validation:
         SHOW(f"Waiting (up to about {PROGRESS_TIMEOUT}s) for server validation results.")
     else:
-        SHOW(f"Checking {action} for submission ID: %s ..." % uuid)
+        SHOW(f"Waiting (up to about {PROGRESS_TIMEOUT}s) for submission results.")
+        # SHOW(f"Checking {action} for submission ID: %s ..." % uuid)
 
     started = time.time()
     progress = define_progress_callback(PROGRESS_MAX_CHECKS,
                                         title="Validation" if validation else "Submission",
-                                        include_status=not validation)
-    server_check_count = 0
+                                        include_status=False)  # include_status=not validation
     most_recent_server_check_time = None
     check_submission_script_initial_check_ran = False
     check_done = False
     check_status = None
     check_response = None
+    ingestion_status = {}
     for n in range(PROGRESS_MAX_CHECKS):
-        if ((most_recent_server_check_time is None) or
+        # Do the (new/2024-03-25) portal ingestion-status check here which reads
+        # from Redis where the ingester is (now/2024-03-25) writing.
+        # This is a very cheap call so do it on every progress iteration.
+        ingestion_status = portal.get(f"/ingestion-status/{uuid}")
+        if (ingestion_status.status_code == 200) and (ingestion_status := ingestion_status.json()):
+            loadxl_done = (ingestion_status.get(PROGRESS_LOADXL.DONE, None) is not None)
+        else:
+            ingestion_status = {}
+            loadxl_done = False
+        if (loadxl_done or (most_recent_server_check_time is None) or
             ((time.time() - most_recent_server_check_time) >= PROGRESS_CHECK_SERVER_INTERVAL)):  # noqa
             if most_recent_server_check_time is None:
-                progress({"start": True})
+                progress(ingestion_status)
             else:
-                progress({"check_server": True, "status": (check_status or "unknown").title()})
-            # Do the actual server check here.
+                progress({"check_server": True, "status": (check_status or "unknown").title(), **ingestion_status})
+            # Do the actual portal check here (i.e by fetching the IngestionSubmission object)..
             [check_done, check_status, check_response] = (
                 _check_ingestion_progress(uuid, keypair=portal.key_pair, server=portal.server))
             if check_done:
                 break
             if check_submission_script:
                 if not check_submission_script_initial_check_ran:
                     check_submission_script_initial_check_ran = True
                     PRINT(f"This ID is for a server validation that had not yet completed; waiting for completion.")
                     PRINT(f"Details for this server validation ({uuid}) below:")
-                    _print_submission_summary(portal, check_response, nofiles=nofiles, check_submission_script=True)
-            server_check_count += 1
+                    _print_submission_summary(portal, check_response, nofiles=nofiles,
+                                              check_submission_script=True, verbose=verbose, debug=debug)
             most_recent_server_check_time = time.time()
         progress({"check": True,
-                  "next": PROGRESS_CHECK_SERVER_INTERVAL - (time.time() - most_recent_server_check_time)})
+                  "next": PROGRESS_CHECK_SERVER_INTERVAL - (time.time() - most_recent_server_check_time),
+                  **ingestion_status})
         time.sleep(PROGRESS_INTERVAL)
     if check_done:
         progress({"finish": True, "done": True,
-                  "status": (check_status or "unknown").title(), "response": check_response})
+                  "status": (check_status or "unknown").title(), "response": check_response, **ingestion_status})
     else:
-        progress({"finish": True})
+        progress({"finish": True, **ingestion_status})
 
     if not check_done:
         command_summary = _summarize_submission(uuid=uuid, server=server, env=env, app=portal.app)
         SHOW(f"Timed out (after {round(time.time() - started)}s) WAITING for {action}.")
         SHOW(f"Your {'validation' if validation else 'submission'} is still running on the server.")
         SHOW(f"Use this command to check its status: {command_summary}")
         exit(1)
 
     if (check_submission_script and check_response and
         (check_parameters := check_response.get("parameters", {})) and
-        _tobool(check_parameters.get("validate_only")) and
+        tobool(check_parameters.get("validate_only")) and
         not check_parameters.get("submission_uuid")):  # noqa
         # This is the check-submission script waiting for a VALIDATION (not a submission)
         # to complete, i.e. the server validation part of submit-metadata-bundle had timed
         # out previously. And this which server validation is now complete. We now want
         # to give the user the opportunity to continue with the submission process,
         # ala submit_any_ingestion; see around line 830 of that function.
         if not check_submission_script_initial_check_ran:
             check_submission_script_initial_check_ran = True
             PRINT(f"This ID is for a server validation that had not yet completed but now is.")
             PRINT(f"Details for this server validation ({uuid}) below:")
-            _print_submission_summary(portal, check_response, nofiles=nofiles, check_submission_script=True)
+            _print_submission_summary(portal, check_response, nofiles=nofiles,
+                                      check_submission_script=True, include_errors=True,
+                                      verbose=verbose, debug=debug)
         validation_info = check_response.get("additional_data", {}).get("validation_output")
+        # TODO: Cleanup/unify error structure from client and server!
         if isinstance(validation_info, list):
             validation_errors = [item for item in validation_info if item.lower().startswith("errored")]
             if validation_errors:
-                PRINT("Since server validation errors were encountered: Exiting with no action.")
+                PRINT("\nServer validation errors were encountered for this metadata.")
+                PRINT("You will need to correct any errors and resubmit via submit-metadata-bundle.")
+                exit(1)
+        elif isinstance(validation_info, dict):
+            if validation_info.get("ref") or validation_info.get("validation"):
+                PRINT("\nServer validation errors were encountered for this metadata.")
                 PRINT("You will need to correct any errors and resubmit via submit-metadata-bundle.")
                 exit(1)
         PRINT("Validation results (server): OK")
         if not yes_or_no("Do you want to now continue with the submission for this metadata?"):
             PRINT("Exiting with no action.")
             exit(0)
         # Get parameters for this submission from the validation IngestionSubmission object.
-        if consortium := check_response.get("parameters", {}).get("consortium"):
+        consortia = None
+        submission_centers = None
+        if consortium := check_parameters.get("consortium"):
             consortia = [consortium]
-        if submission_center := check_response.get("parameters", {}).get("submission_center"):
+        if submission_center := check_parameters.get("submission_center"):
             submission_centers = [submission_center]
-        autoadd = check_response.get("parameters", {}).get("autoadd")
         if debug:
             PRINT("DEBUG: Continuing with submission process after a previous server validation timeout.")
         submission_uuid = _initiate_server_ingestion_process(
+            portal=portal,
+            ingestion_filename=None,
             is_server_validation=False,
             is_resume_submission=True,
             validation_ingestion_submission_object=check_response,
-            portal=portal,
-            ingestion_filename=None,
             consortia=consortia,
             submission_centers=submission_centers,
-            autoadd=autoadd)
+            autoadd=check_parameters.get("autoadd"),
+            datafile_size=check_parameters.get("datafile_size"),
+            datafile_checksum=check_parameters.get("datafile_checksum"),
+            user=check_parameters.get("user"),
+            debug=debug,
+            debug_sleep=debug_sleep)
         SHOW(f"Submission tracking ID: {submission_uuid}")
         submission_done, submission_status, submission_response = _monitor_ingestion_process(
                 submission_uuid, portal.server, portal.env, app=portal.app, keys_file=portal.keys_file,
                 show_details=show_details, report=False, messages=True,
                 validation=False,
                 nofiles=True, noprogress=noprogress, timeout=timeout,
                 verbose=verbose, debug=debug, debug_sleep=debug_sleep)
         if submission_status != "success":
             exit(1)
         PRINT("Submission complete!")
         do_any_uploads(submission_response, keydict=portal.key,
-                       upload_folder=upload_directory, subfolders=upload_directory_recursive)
-        # do_any_uploads(submission_response, keydict=portal.key, ingestion_filename=ingestion_filename,
-        #                upload_folder=upload_folder, no_query=no_query,
-        #                subfolders=subfolders)
+                       upload_folder=upload_directory, subfolders=upload_directory_recursive, portal=portal)
         return
 
-    if check_submission_script or verbose or not validation:
+    if check_submission_script or verbose or debug:  # or not validation
         _print_submission_summary(portal, check_response,
-                                  nofiles=nofiles, check_submission_script=check_submission_script)
+                                  nofiles=nofiles, check_submission_script=check_submission_script,
+                                  verbose=verbose, debug=debug)
 
     # If not sucessful then output any validation/submission results.
     if check_status != "success":
         PRINT(f"{'Validation' if validation else 'Submission'} results (server): ERROR"
               f"{f' ({check_status})' if check_status not in ['failure', 'error'] else ''}")
+        printed_newline = False
         if check_response and (additional_data := check_response.get("additional_data")):
             if (validation_info := additional_data.get("validation_output")):
                 if isinstance(validation_info, list):
                     if errors := [info for info in validation_info if info.lower().startswith("error:")]:
+                        if not printed_newline:
+                            PRINT_OUTPUT()
+                            printed_newline = True
                         for error in errors:
-                            PRINT_OUTPUT(f"- {_format_server_error(error, indent=2)}")
+                            PRINT_OUTPUT(f"- {_format_server_error(error, indent=2, debug=debug)}")
                 elif isinstance(validation_info, dict):
                     if ((validation_errors := validation_info.get("validation")) and
                         isinstance(validation_errors, list) and validation_errors):  # noqa
+                        if not printed_newline:
+                            PRINT_OUTPUT()
+                            printed_newline = True
                         PRINT_OUTPUT(f"- Data errors: {len(validation_errors)}")
                         for validation_error in validation_errors:
                             PRINT_OUTPUT(f"    - {_format_issue(validation_error)}")
-                    if ref_errors := (validation_info.get("ref") if debug else validation_info.get("ref_grouped")):
-                        if ref_errors := _validate_references(ref_errors, None):
-                            _print_reference_errors(ref_errors)
-        if check_response and isinstance(other_errors := check_response.get("errors"), list):
+                    if debug:
+                        ref_errors = validation_info.get("ref")
+                    elif not (ref_errors := validation_info.get("ref_grouped")):
+                        ref_errors = validation_info.get("ref")
+                    if ref_errors and (ref_errors := _validate_references(ref_errors, None, debug=debug)):
+                        if not printed_newline:
+                            PRINT_OUTPUT()
+                            printed_newline = True
+                        _print_reference_errors(ref_errors, verbose=verbose, debug=debug)
+        if check_response and isinstance(other_errors := check_response.get("errors"), list) and other_errors:
+            if not printed_newline:
+                PRINT_OUTPUT()
+                printed_newline = True
             for error in other_errors:
                 PRINT_OUTPUT("- " + error)
         if output_file := get_output_file():
             PRINT_STDOUT(f"Exiting with server validation errors; see your output file: {output_file}")
         else:
             PRINT_STDOUT("\nExiting with no action with server validation errors.")
             PRINT_STDOUT("Use the --output FILE option to write errors to a file.")
         exit(1)
 
     return check_done, check_status, check_response
 
 
-def _format_server_error(error: str, indent: int = 0) -> str:
+def _format_server_error(error: str, indent: int = 0, debug: bool = False) -> str:
     """
     Make an attempt at parsing and formatting a server (validation/submission) error.
     If we can't do it then just return the string as given. Here for example is what
     we hope a "typical" server error message looks like:
     'Error: /Software/DAX_SOFTWARE_VEPX Exception encountered on VirtualAppURL: /Software?skip_indexing=true&check_only=true&skip_links=trueBODY: {\'submitted_id\': \'DAX_SOFTWARE_VEPX\', \'category\': [\'Variant Annotation\'], \'title\': \'VEP\', \'version\': \'1.0.1\', \'consortia\': [\'smaht\'], \'submission_centers\': [\'9626d82e-8110-4213-ac75-0a50adf890ff\']}MSG: HTTP POST failed.Raw Exception: Bad response: 422 Unprocessable Entity (not 200 OK or 3xx redirect for http://localhost/Software?skip_indexing=true&check_only=true&skip_links=true)b\'{"@type": ["ValidationFailure", "Error"], "status": "error", "code": 422, "title": "Unprocessable Entity", "description": "Failed validation", "errors": [{"location": "submitted_id", "name": "Submission Code Mismatch", "description": "Submitted ID DAX_SOFTWARE_VEPX start (DAX) does not match options for given submission centers: [\\\'DAC\\\']."}]}\''  # noqa
     """
 
@@ -1216,14 +1377,21 @@
         error = match.group(4)
         body = load_json_fuzzy(body)
         error = load_json_fuzzy(error)
         if path and message and error and body:
             result = f"ERROR: {message} ▶ {path}"
             result += f"\n{format_json_with_indent(error, indent=indent)}"
             result += f"\n{format_json_with_indent(body, indent=indent)}"
+            if not debug and error.get('title') and error.get('code') and error.get('description'):
+                result = f"ERROR: {message} {path}"
+                result += f"\n{indent * ' '}{error.get('title')} ({error.get('code')}): {error.get('description')}"
+                if isinstance(errors := error.get('errors', []), list) and errors:
+                    for error in errors:
+                        result += f"\n{indent * ' '}{error.get('name')} ({error.get('location')})"
+                        result += f"\n{indent * ' '}{error.get('description')}"
             return result
     return error.replace("Error:", "ERROR:")
 
 
 def _check_ingestion_progress(uuid, *, keypair, server) -> Tuple[bool, str, dict]:
     """
     Calls endpoint to get this status of the IngestionSubmission uuid (in outer scope);
@@ -1280,48 +1448,63 @@
         'datafile_source_filename': os.path.basename(ingestion_filename),
         **other_args  # validate_remote_only, and any of institution, project, lab, or award that caller gave us
     }
     return submission_post_data
 
 
 def _print_submission_summary(portal: Portal, result: dict,
-                              nofiles: bool = False, check_submission_script: bool = False) -> None:
+                              nofiles: bool = False,
+                              check_submission_script: bool = False,
+                              include_errors: bool = False,
+                              verbose: bool = False, debug: bool = False) -> None:
     if not result:
         return
     def is_admin_user(user_record: Optional[dict]) -> bool:  # noqa
         nonlocal portal, check_submission_script
         if not check_submission_script or not user_record or not (user_uuid := user_record.get("uuid")):
             return None
         try:
-            user_record = portal.get_metadata(user_uuid)
-            return "admin" in user_record.get("groups", [])
+            return _is_admin_user(portal.get_metadata(user_uuid))
         except Exception:
             return None
     lines = []
     errors = []
     validation_info = None
     submission_type = "Submission"
     validation = None
     was_server_validation_timeout = False
     if submission_parameters := result.get("parameters", {}):
-        if validation := _tobool(submission_parameters.get("validate_only")):
+        if validation := tobool(submission_parameters.get("validate_only")):
             submission_type = "Validation"
         if submission_file := submission_parameters.get("datafile"):
             if submission_file == "null":
                 # This submission was a continuance via check-submission of a
                 # server validation (via submit-metadata-bundle) which timed out;
                 # we will note this fact very subtly in the output.
                 if validation_datafile := submission_parameters.get("validation_datafile"):
                     submission_file = validation_datafile
                     was_server_validation_timeout = True
             lines.append(f"Submission File: {submission_file}")
     if submission_uuid := result.get("uuid"):
         lines.append(f"{submission_type} ID: {submission_uuid}")
     if date_created := _format_portal_object_datetime(result.get("date_created"), True):
         lines.append(f"{submission_type} Time: {date_created}")
+    if submission_parameters:
+        extra_file_info = ""
+        if (datafile_size := submission_parameters.get("datafile_size", None)) is not None:
+            if not isinstance(datafile_size, int) and isinstance(datafile_size, str) and datafile_size.isdigit():
+                datafile_size = int(datafile_size)
+            if isinstance(datafile_size, int):
+                extra_file_info += f"{format_size(datafile_size)}"
+        if datafile_checksum := submission_parameters.get("datafile_checksum"):
+            if extra_file_info:
+                extra_file_info += " | "
+            extra_file_info += f"Checksum: {datafile_checksum}"
+        if extra_file_info:
+            lines.append(f"Submission File Info: {extra_file_info}")
     if validation:
         lines.append(f"Validation Only: Yes ◀ ◀ ◀")
         if submission_parameters and (associated_submission_uuid := submission_parameters.get("submission_uuid")):
             lines.append(f"Associated Submission ID: {associated_submission_uuid}")
     elif submission_parameters and (associated_validation_uuid := submission_parameters.get("validation_uuid")):
         lines.append(f"Associated Validation ID:"
                      f" {associated_validation_uuid}{' (ω)' if was_server_validation_timeout else ''}")
@@ -1339,14 +1522,31 @@
                 lines.append(f"Submitted By: {submitted_by} ({consortia})")
         elif submission_center:
             lines.append(f"Submitted By: {submitted_by} ({submission_center})")
         else:
             lines.append(f"Submitted By: {submitted_by}")
         if is_admin_user(result.get("submitted_by")) is True:
             lines[len(lines) - 1] += " ▶ Admin"
+        # If more than one submission center print on separate line (only first one printed above).
+        if len(submission_centers) > 1:
+            submission_centers_line = ""
+            for submission_center in submission_centers:
+                if submission_centers_line:
+                    submission_centers_line += " | "
+                submission_centers_line += submission_center.get("display_title")
+            lines.append(f"Submission Centers: {submission_centers_line}")
+    if additional_data := result.get("additional_data"):
+        if (validation_info := additional_data.get("validation_output")) and isinstance(validation_info, dict):
+            # TODO: Cleanup/unify error structure from client and server!
+            if ref_errors := _validate_references(validation_info.get("ref"), None):
+                errors.extend(_format_reference_errors(ref_errors, verbose=verbose, debug=debug))
+            if validation_errors := validation_info.get("validation"):
+                errors.append(f"- Validation errors: {len(validation_errors)}")
+                for validation_error in validation_errors:
+                    errors.append(f"  - {_format_issue(validation_error)}")
     if processing_status := result.get("processing_status"):
         summary_lines = []
         if additional_data := result.get("additional_data"):
             if (validation_info := additional_data.get("validation_output")) and isinstance(validation_info, list):
                 if status := [info for info in validation_info if info.lower().startswith("status:")]:
                     summary_lines.append(status[0])
         if state := processing_status.get("state"):
@@ -1406,31 +1606,34 @@
     if additional_data and not nofiles:
         if upload_files := additional_data.get("upload_info"):
             lines.append("===")
             lines.append(f"Upload Files: {len(upload_files)} ...")
             for upload_file in upload_files:
                 upload_file_uuid = upload_file.get("uuid")
                 upload_file_name = upload_file.get("filename")
-                upload_file_accession_name, upload_file_type = _get_upload_file_info(portal, upload_file_uuid)
+                if verbose:
+                    upload_file_accession_name, upload_file_type = _get_upload_file_info(portal, upload_file_uuid)
+                else:
+                    upload_file_accession_name = None
+                    upload_file_type = None
                 lines.append("===")
                 lines.append(f"Upload File: {upload_file_name}")
                 lines.append(f"Upload File ID: {upload_file_uuid}")
                 if upload_file_accession_name:
                     lines.append(f"Upload File Accession Name: {upload_file_accession_name}")
                 if upload_file_type:
                     lines.append(f"Upload File Type: {upload_file_type}")
     if lines:
         lines = ["===", f"SMaHT {'Validation' if validation else 'Submission'} Summary [UUID]", "==="] + lines + ["==="]
-        if errors:
+        if errors and include_errors:
             lines += ["ERRORS ITEMIZED BELOW ...", "==="]
-        print_boxed(lines, right_justified_macro=("[UUID]", lambda: submission_uuid))
-        if errors:
+        print_boxed(lines, right_justified_macro=("[UUID]", lambda: submission_uuid), printf=PRINT)
+        if errors and include_errors:
             for error in errors:
-                # PRINT(error.replace("Error:", "ERROR:"))
-                PRINT(_format_server_error(error))
+                PRINT(f"- {_format_server_error(error, indent=2, debug=debug)}")
 
 
 def _show_upload_info(uuid, server=None, env=None, keydict=None, app: str = None,
                       show_primary_result=True,
                       show_validation_output=True,
                       show_processing_status=True,
                       show_datafile_url=True,
@@ -1536,85 +1739,122 @@
     if show_datafile_url and result.get('parameters'):
         datafile_url = result['parameters'].get('datafile_url')
         if datafile_url:
             SHOW("----- DataFile URL -----")
             SHOW(datafile_url)
 
 
-def do_any_uploads(res, keydict, upload_folder=None, ingestion_filename=None, no_query=False, subfolders=False):
+def do_any_uploads(res, keydict, upload_folder=None, ingestion_filename=None,
+                   no_query=False, subfolders=False, portal=None):
 
     def display_file_info(upload_file_info: dict) -> None:
         nonlocal upload_folder, subfolders
         file = upload_file_info.get("filename")
         file_uuid = upload_file_info.get("uuid")
         if file:
             if file_paths := search_for_file(file, location=upload_folder, recursive=subfolders):
                 if len(file_paths) == 1:
-                    PRINT(f"File to upload: {_format_path(file_paths[0])}"
-                          f" ({_format_file_size(_get_file_size(file_paths[0]))})")
+                    PRINT(f"File to upload to AWS S3: {format_path(file_paths[0])}"
+                          f" ({format_size(get_file_size(file_paths[0]))})")
                     return True
                 else:
                     PRINT(f"No upload attempted for file {file} because multiple"
                           f" copies were found in folder {upload_folder}: {', '.join(file_paths)}.")
                     return False
-            PRINT(f"ERROR: Cannot find file to upload: {_format_path(file)} ({file_uuid})")
+            PRINT(f"WARNING: Cannot find file to upload to AWS S3: {format_path(file)} ({file_uuid})")
         return False
 
     upload_info = _get_section(res, 'upload_info')
     if not upload_folder:
         if ingestion_directory := res.get("parameters", {}).get("ingestion_directory"):
             if os.path.isdir(ingestion_directory):
                 upload_folder = ingestion_directory
     if not upload_folder and ingestion_filename:
         if ingestion_directory := os.path.dirname(ingestion_filename):
             upload_folder = ingestion_directory
+    resume_upload_commands = []
+    resume_upload_commands_missing = []
+    noupload = False
     if upload_info:
         files_to_upload = []
         for upload_file_info in upload_info:
             if display_file_info(upload_file_info):
                 files_to_upload.append(upload_file_info)
+                if portal:
+                    resume_upload_commands.append(f"resume-uploads --env {portal.env} {upload_file_info.get('uuid')}")
+            elif portal:
+                resume_upload_commands_missing.append(
+                    f"resume-uploads --env {portal.env} {upload_file_info.get('uuid')}")
         if len(files_to_upload) == 0:
             return
         if no_query:
             do_uploads(files_to_upload, auth=keydict, no_query=no_query, folder=upload_folder,
-                       subfolders=subfolders)
+                       subfolders=subfolders, portal=portal)
         else:
             message = ("Upload this file?" if len(files_to_upload) == 1
                        else f"Upload these {len(files_to_upload)} files?")
             if yes_or_no(message):
                 do_uploads(files_to_upload, auth=keydict,
                            no_query=no_query, folder=upload_folder,
-                           subfolders=subfolders)
+                           subfolders=subfolders, portal=portal)
             else:
+                noupload = True
                 SHOW("No uploads attempted.")
+                if resume_upload_commands:
+                    resume_upload_commands += resume_upload_commands_missing
+                    nresume_upload_commands = len(resume_upload_commands)
+                    if yes_or_no(f"Do you want to see the resume-uploads"
+                                 f" command{'s' if nresume_upload_commands != 1 else ''} to use to"
+                                 f" upload {'these' if nresume_upload_commands != 1 else 'this'} separately?"):
+                        for resume_upload_command in resume_upload_commands:
+                            PRINT(f"▶ {resume_upload_command}")
+    if not noupload and resume_upload_commands_missing:
+        nresume_upload_commands_missing = len(resume_upload_commands_missing)
+        PRINT(f"There {'were' if nresume_upload_commands_missing != 1 else 'was'}"
+              f" {nresume_upload_commands_missing} missing"
+              f" file{'s' if nresume_upload_commands_missing != 1 else ''} as mentioned above.")
+        if yes_or_no(f"Do you want to see the resume-uploads"
+                     f" command{'s' if nresume_upload_commands_missing != 1 else ''}"
+                     f" to use to upload {'these' if nresume_upload_commands_missing != 1 else 'this'} separately?"):
+            for resume_upload_command_missing in resume_upload_commands_missing:
+                PRINT(f"▶ {resume_upload_command_missing}")
 
 
 def resume_uploads(uuid, server=None, env=None, bundle_filename=None, keydict=None,
-                   upload_folder=None, no_query=False, subfolders=False, app=None, keys_file=None, env_from_env=False):
+                   upload_folder=None, no_query=False, subfolders=False,
+                   output_file=None, app=None, keys_file=None, env_from_env=False):
     """
     Uploads the files associated with a given ingestion submission. This is useful if you answered "no" to the query
     about uploading your data and then later are ready to do that upload.
 
     :param uuid: a string guid that identifies the ingestion submission
     :param server: the server to upload to
     :param env: the portal environment to upload to
     :param bundle_filename: the bundle file to be uploaded
     :param keydict: keydict-style auth, a dictionary of 'key', 'secret', and 'server'
     :param upload_folder: folder in which to find files to upload (default: same as ingestion_filename)
     :param no_query: bool to suppress requests for user input
     :param subfolders: bool to search subdirectories within upload_folder for files
     """
 
+    if output_file:
+        global PRINT, PRINT_OUTPUT, PRINT_STDOUT, SHOW
+        PRINT, PRINT_OUTPUT, PRINT_STDOUT, SHOW = setup_for_output_file_option(output_file)
+
     portal = _define_portal(key=keydict, keys_file=keys_file, env=env,
-                            server=server, app=app, env_from_env=env_from_env, report=True)
+                            server=server, app=app, env_from_env=env_from_env,
+                            report=True, note="Resuming File Upload")
 
-    if not (response := portal.get_metadata(uuid)):
+    if not (response := portal.get_metadata(uuid, raise_exception=False)):
         if accession_id := _extract_accession_id(uuid):
-            if not (response := portal.get_metadata(uuid := accession_id)):
-                raise Exception(f"Given accession ID not found: {uuid}")
+            if not (response := portal.get_metadata(accession_id)):
+                raise Exception(f"Given accession ID not found: {accession_id}")
+            if (display_title := response.get("display_title")) and not (uuid == display_title):
+                raise Exception(f"Accession ID found but wrong filename: {accession_id} vs {uuid}")
+            uuid = accession_id
         else:
             raise Exception(f"Given ID not found: {uuid}")
 
     if not portal.is_schema_type(response, INGESTION_SUBMISSION_TYPE_NAME):
 
         # Subsume function of upload-item-data into resume-uploads for convenience.
         if portal.is_schema_type(response, FILE_TYPE_NAME):
@@ -1623,24 +1863,25 @@
                               no_query=no_query, app=app, report=False)
             return
 
         undesired_type = portal.get_schema_type(response)
         raise Exception(f"Given ID is not an {INGESTION_SUBMISSION_TYPE_NAME} type: {uuid} ({undesired_type})")
 
     if submission_parameters := response.get("parameters", {}):
-        if _tobool(submission_parameters.get("validate_only")):
+        if tobool(submission_parameters.get("validate_only")):
             PRINT(f"This submission ID ({uuid}) is for a validation not an actual submission.")
             exit(1)
 
     do_any_uploads(response,
                    keydict=portal.key,
                    ingestion_filename=bundle_filename,
                    upload_folder=upload_folder,
                    no_query=no_query,
-                   subfolders=subfolders)
+                   subfolders=subfolders,
+                   portal=portal)
 
 
 @function_cache(serialize_key=True)
 def _get_health_page(key: dict) -> dict:
     return Portal(key).get_health().json()
 
 
@@ -1684,55 +1925,32 @@
     :param auth: auth info in the form of a dictionary containing 'key', 'secret', and 'server',
         and possibly other useful information such as an encryption key id.
     """
 
     if DEBUG_PROTOCOL:  # pragma: no cover
         PRINT(f"Upload credentials contain {conjoined_list(list(upload_credentials.keys()))}.")
     try:
-        s3_encrypt_key_id = get_s3_encrypt_key_id(upload_credentials=upload_credentials, auth=auth)
-        extra_env = dict(AWS_ACCESS_KEY_ID=upload_credentials['AccessKeyId'],
-                         AWS_SECRET_ACCESS_KEY=upload_credentials['SecretAccessKey'],
-                         AWS_SECURITY_TOKEN=upload_credentials['SessionToken'])
-        env = dict(os.environ, **extra_env)
+        s3_uri = upload_credentials["upload_url"]
+        aws_credentials = {
+            "AWS_ACCESS_KEY_ID": upload_credentials["AccessKeyId"],
+            "AWS_SECRET_ACCESS_KEY": upload_credentials["SecretAccessKey"],
+            "AWS_SECURITY_TOKEN": upload_credentials["SessionToken"]
+        }
+        aws_kms_key_id = get_s3_encrypt_key_id(upload_credentials=upload_credentials, auth=auth)
     except Exception as e:
         raise ValueError("Upload specification is not in good form. %s: %s" % (e.__class__.__name__, e))
 
-    start = time.time()
-    try:
-        file_size = 0
-        formatted_file_size = ""
-        try:
-            file_size = _get_file_size(path)
-            formatted_file_size = _format_file_size(file_size)
-        except Exception:
-            pass
-        source = path
-        target = upload_credentials['upload_url']
-        SHOW(f"Uploading {_format_path(source)}{f' ({formatted_file_size})' if formatted_file_size else ''}"
-             f" to: {target}")
-        command = ['aws', 's3', 'cp']
-        if s3_encrypt_key_id:
-            command = command + ['--sse', 'aws:kms', '--sse-kms-key-id', s3_encrypt_key_id]
-        command = command + ['--only-show-errors', source, target]
-        options = {}
-        if _running_on_windows_native():
-            options = {"shell": True}
-        if DEBUG_PROTOCOL:  # pragma: no cover
-            PRINT(f"DEBUG CLI: {' '.join(command)} | ENV INCLUDES: {conjoined_list(list(extra_env.keys()))}")
-        subprocess.check_call(command, env=env, **options)
-    except subprocess.CalledProcessError as e:
-        raise RuntimeError("Upload failed with exit code %d" % e.returncode)
-    else:
-        end = time.time()
-        duration = end - start
-        if formatted_file_size:
-            SHOW(f"Upload of {os.path.basename(source)}: OK ->"
-                 f" {'%.1f' % duration}s | {formatted_file_size} | {(file_size / duration):.1f}bps")
-        else:
-            SHOW(f"Upload of {os.path.basename(source)}: OK -> {'%.1f' % duration} seconds")
+    upload_file_to_aws_s3(file=path,
+                          s3_uri=s3_uri,
+                          aws_credentials=aws_credentials,
+                          aws_kms_key_id=aws_kms_key_id,
+                          print_progress=True,
+                          print_function=PRINT,
+                          verify_upload=True,
+                          catch_interrupt=True)
 
 
 def _running_on_windows_native():
     return os.name == 'nt'
 
 
 def compute_file_post_data(filename, context_attributes):
@@ -1770,15 +1988,15 @@
                                                                            filename=filename, payload_data=post_item)
 
     execute_prearranged_upload(filename, upload_credentials=upload_credentials, auth=auth)
 
     return metadata
 
 
-def upload_file_to_uuid(filename, uuid, auth):
+def upload_file_to_uuid(filename, uuid, auth, first_time=False, portal=None):
     """
     Upload file to a target environment.
 
     :param filename: the name of a file to upload.
     :param uuid: the item into which the filename is to be uploaded.
     :param auth: auth info in the form of a dictionary containing 'key', 'secret', and 'server'.
     :returns: item metadata dict or None
@@ -1789,44 +2007,63 @@
     # filename here should not include path
     patch_data = {'filename': os.path.basename(filename)}
 
     response = Portal(auth).patch_metadata(object_id=uuid, data=patch_data)
 
     metadata, upload_credentials = extract_metadata_and_upload_credentials(response,
                                                                            method='PATCH', uuid=uuid,
-                                                                           filename=filename, payload_data=patch_data)
-
+                                                                           filename=filename,
+                                                                           payload_data=patch_data,
+                                                                           portal=portal)
+
+    if first_time:
+        if upload_url := upload_credentials.get('upload_url'):
+            s3_bucket, _ = get_s3_bucket_and_key_from_s3_uri(upload_url)
+            if s3_bucket:
+                # This assumes all files are going to the same bucket;
+                # which I think is a pretty solid assumption.
+                PRINT(f"Upload file destination AWS S3 bucket: {s3_bucket}")
     execute_prearranged_upload(filename, upload_credentials=upload_credentials, auth=auth)
 
     return metadata
 
 
-def extract_metadata_and_upload_credentials(response, filename, method, payload_data, uuid=None, schema_name=None):
+def extract_metadata_and_upload_credentials(response, filename, method, payload_data,
+                                            uuid=None, schema_name=None, portal=None):
     try:
         [metadata] = response['@graph']
         upload_credentials = metadata['upload_credentials']
     except Exception as e:
         if DEBUG_PROTOCOL:  # pragma: no cover
             PRINT(f"Problem trying to {method} to get upload credentials.")
             PRINT(f" payload_data={payload_data}")
             if uuid:
                 PRINT(f" uuid={uuid}")
             if schema_name:
                 PRINT(f" schema_name={schema_name}")
             PRINT(f" response={response}")
             PRINT(f"Got error {type(e)}: {e}")
-        raise RuntimeError(f"Unable to obtain upload credentials for file {filename}.")
+        file_status = None
+        if portal and uuid:
+            try:
+                file_status = portal.get_metadata(uuid).get("status")
+            except Exception:
+                pass
+        message = f"Unable to obtain upload credentials for file {filename}."
+        if file_status:
+            message += f" File status: {file_status}"
+        raise RuntimeError(message)
     return metadata, upload_credentials
 
 
 # This can be set to True in unusual situations, but normally will be False to avoid unnecessary querying.
 SUBMITR_SELECTIVE_UPLOADS = environ_bool("SUBMITR_SELECTIVE_UPLOADS")
 
 
-def do_uploads(upload_spec_list, auth, folder=None, no_query=False, subfolders=False):
+def do_uploads(upload_spec_list, auth, folder=None, no_query=False, subfolders=False, portal=None):
     """
     Uploads the files mentioned in the give upload_spec_list.
 
     If any files have associated extra files, upload those as well.
 
     :param upload_spec_list: a list of upload_spec dictionaries, each of the form {'filename': ..., 'uuid': ...},
         representing uploads to be formed.
@@ -1836,14 +2073,15 @@
     :param no_query: bool to suppress requests for user input
     :param subfolders: bool to search subdirectories within upload_folder for files
     :return: None
     """
     folder = folder or os.path.curdir
     if subfolders:
         folder = os.path.join(folder, '**')
+    first_time = True
     for upload_spec in upload_spec_list:
         file_name = upload_spec["filename"]
         if not (file_paths := search_for_file(file_name, location=folder, recursive=subfolders)) or len(file_paths) > 1:
             if len(file_paths) > 1:
                 SHOW(f"No upload attempted for file {file_name} because multiple copies"
                      f" were found in folder {folder}: {', '.join(file_paths)}.")
             else:
@@ -1852,26 +2090,27 @@
         file_path = file_paths[0]
         uuid = upload_spec['uuid']
         uploader_wrapper = UploadMessageWrapper(uuid, no_query=no_query)
         wrapped_upload_file_to_uuid = uploader_wrapper.wrap_upload_function(
             upload_file_to_uuid, file_path
         )
         file_metadata = wrapped_upload_file_to_uuid(
-            filename=file_path, uuid=uuid, auth=auth
+            filename=file_path, uuid=uuid, auth=auth, first_time=first_time, portal=portal
         )
         if file_metadata:
             extra_files_credentials = file_metadata.get("extra_files_creds", [])
             if extra_files_credentials:
                 _upload_extra_files(
                     extra_files_credentials,
                     uploader_wrapper,
                     folder,
                     auth,
                     recursive=subfolders,
                 )
+        first_time = False
 
 
 class UploadMessageWrapper:
     """Class to provide consistent queries/messages to user when
     uploading file(s) to given File UUID.
     """
 
@@ -1986,23 +2225,24 @@
         if not (item_filename := uuid_metadata.get("filename")):
             raise Exception(f"Cannot determine file name: {uuid}")
 
     if not (item_filename_found := search_for_file(item_filename, location=directory,
                                                    recursive=recursive, single=True)):
         raise Exception(f"File not found: {item_filename}")
     else:
+        PRINT(f"File to upload to AWS S3: {format_path(item_filename_found)}")
         item_filename = item_filename_found
 
     if not no_query:
-        file_size = _format_file_size(_get_file_size(item_filename))
-        if not yes_or_no(f"Upload {_format_path(item_filename)} ({file_size}) to {server}?"):
+        file_size = format_size(get_file_size(item_filename))
+        if not yes_or_no(f"Upload {format_path(item_filename)} ({file_size}) to {server}?"):
             SHOW("Aborting submission.")
             exit(1)
 
-    upload_file_to_uuid(filename=item_filename, uuid=uuid, auth=portal.key)
+    upload_file_to_uuid(filename=item_filename, uuid=uuid, auth=portal.key, portal=portal)
 
 
 def _show_detailed_results(uuid: str, metadata_bundles_bucket: str) -> None:
 
     PRINT(f"----- Detailed Info -----")
 
     submission_results_location, submission_results = _fetch_submission_results(metadata_bundles_bucket, uuid)
@@ -2051,161 +2291,101 @@
 
 
 def _validate_locally(ingestion_filename: str, portal: Portal, autoadd: Optional[dict] = None,
                       validation: bool = False, validate_local_only: bool = False,
                       upload_folder: Optional[str] = None,
                       subfolders: bool = False, exit_immediately_on_errors: bool = False,
                       ref_nocache: bool = False, output_file: Optional[str] = None,
-                      json_only: bool = False, noprogress: bool = False,
+                      noanalyze: bool = False, json_only: bool = False, noprogress: bool = False,
                       verbose_json: bool = False, verbose: bool = False, quiet: bool = False,
-                      debug: bool = False, debug_sleep: Optional[str] = None) -> int:
+                      debug: bool = False, debug_sleep: Optional[str] = None) -> StructuredDataSet:
 
-    # N.B. This same bit of code is in smaht-portal; not sure best way to share;
-    # It really should not go in dcicutils (structured_data) as this know pretty
-    # specific details about our (SMaHT) schemas, namely, submitted_id and accession.
-    def ref_lookup_strategy(type_name: str, schema: dict, value: str) -> (int, Optional[str]):
-        #
-        # FYI: Note this situation WRT object lookups ...
-        #
-        # /{submitted_id}                # NOT FOUND
-        # /UnalignedReads/{submitted_id} # OK
-        # /SubmittedFile/{submitted_id}  # OK
-        # /File/{submitted_id}           # NOT FOUND
-        #
-        # /{accession}                   # OK
-        # /UnalignedReads/{accession}    # NOT FOUND
-        # /SubmittedFile/{accession}     # NOT FOUND
-        # /File/{accession}              # OK
-        #
-        def ref_validator(schema: Optional[dict],
-                          property_name: Optional[str], property_value: Optional[str]) -> Optional[bool]:
-            """
-            Returns False iff the type represented by the given schema, can NOT be referenced by
-            the given property name with the given property value, otherwise returns None.
-
-            For example, if the schema is for the UnalignedReads type and the property name
-            is accession, then we will return False iff the given property value is NOT a properly
-            formatted accession ID. Otherwise, we will return None, which indicates that the
-            caller (in dcicutils.structured_data.Portal.ref_exists) will continue executing
-            its default behavior, which is to check other ways in which the given type can NOT
-            be referenced by the given value, i.e. it checks other identifying properties for
-            the type and makes sure any patterns (e.g. for submitted_id or uuid) are ahered to.
-
-            The goal (in structured_data) being to detect if a type is being referenced in such
-            a way that cannot possibly be allowed, i.e. because none of its identifying types
-            are in the required form (if indeed there any requirements). Note that it is guaranteed
-            that the given property name is indeed an identifying property for the given type.
-            """
-            if property_format := schema.get("properties", {}).get(property_name, {}).get("format"):
-                if (property_format == "accession") and (property_name == "accession"):
-                    if not _is_accession_id(property_value):
-                        return False
-            return None
-
-        if not schema and value:
-            nonlocal portal
-            if not (schema := portal.get_schema(type_name)):
-                return Portal.LOOKUP_DEFAULT, ref_validator
-        if value and (schema_properties := schema.get("properties")):
-            if schema_properties.get("accession") and _is_accession_id(value):
-                # Case: lookup by accession (only by root).
-                return Portal.LOOKUP_ROOT, ref_validator
-            elif schema_property_info_submitted_id := schema_properties.get("submitted_id"):
-                if schema_property_pattern_submitted_id := schema_property_info_submitted_id.get("pattern"):
-                    if re.match(schema_property_pattern_submitted_id, value):
-                        # Case: lookup by submitted_id (only by specified type).
-                        return Portal.LOOKUP_SPECIFIED_TYPE, ref_validator
-        return Portal.LOOKUP_DEFAULT, ref_validator
+    if json_only:
+        noprogress = True
 
     structured_data = None  # TEMPORARY WORKAROUND FOR DCICUTILS BUG
 
     def define_progress_callback(debug: bool = False) -> None:
-        bar = None
         nsheets = 0
         nrows = 0
         nrows_processed = 0
         nrefs_total = 0
         nrefs_resolved = 0
         nrefs_unresolved = 0
         nrefs_lookup = 0
-        nrefs_cache_hit = 0
+        nrefs_exists_cache_hit = 0
+        nrefs_lookup_cache_hit = 0
         nrefs_invalid = 0
+        bar = ProgressBar(nrows, "Calculating", interrupt_exit=True)
 
-        def handle_control_c(signum, frame):  # noqa
-            if yes_or_no("\nCTRL-C: You have interrupted this process. Do you want to TERMINATE processing?"):
-                PRINT("Premature exit.")
-                exit(1)
-            PRINT_STDOUT("Continuing ...")
         def progress_report(status: dict) -> None:  # noqa
             nonlocal bar, nsheets, nrows, nrows_processed, verbose, noprogress
-            nonlocal nrefs_total, nrefs_resolved, nrefs_unresolved, nrefs_lookup, nrefs_cache_hit, nrefs_invalid
+            nonlocal nrefs_total, nrefs_resolved, nrefs_unresolved, nrefs_lookup
+            nonlocal nrefs_exists_cache_hit, nrefs_lookup_cache_hit, nrefs_invalid
             if noprogress:
                 return
             increment = 1
-            if status.get("start"):
-                signal.signal(signal.SIGINT, handle_control_c)
-                nsheets = status.get("sheets") or 0
-                nrows = status.get("rows") or 0
+            if status.get(PROGRESS_PARSE.LOAD_START):
+                nsheets = status.get(PROGRESS_PARSE.LOAD_COUNT_SHEETS) or 0
+                nrows = status.get(PROGRESS_PARSE.LOAD_COUNT_ROWS) or 0
                 if nrows > 0:
+                    bar.set_total(nrows)
                     if nsheets > 0:
                         PRINT(
                             f"Parsing submission file which has{' only' if nsheets == 1 else ''}"
                             f" {nsheets} sheet{'s' if nsheets != 1 else ''} and a total of {nrows} rows.")
                     else:
                         PRINT(f"Parsing submission file which has a total of {nrows} row{'s' if nrows != 1 else ''}.")
                 elif nsheets > 0:
                     PRINT(f"Parsing submission file which has {nsheets} sheet{'s' if nsheets != 1 else ''}.")
                 else:
                     PRINT(f"Parsing submission file which has a total of {nrows} row{'s' if nrows != 1 else ''}.")
-                bar_format = "{l_bar}{bar}| {n_fmt}/{total_fmt} | {rate_fmt} | {elapsed}{postfix} | ETA: {remaining} "
-                bar = tqdm(total=nrows, desc="Calculating", dynamic_ncols=True, bar_format=bar_format, unit="")
                 return
-            elif status.get("finish"):
-                bar.close()
-                signal.signal(signal.SIGINT, signal.SIG_DFL)
-                return
-            elif status.get("parse"):
-                nrows_processed += increment
-                nrefs_total = status.get("refs") or 0
-                nrefs_resolved = status.get("refs_found") or 0
-                nrefs_unresolved = status.get("refs_not_found") or 0
-                nrefs_lookup = status.get("refs_lookup") or 0
-                nrefs_cache_hit = status.get("refs_cache_hit") or 0
-                if not status.get("refs_cache_hit"):  # TEMPORARY WORKAROUND FOR DCICUTILS BUG
-                    if structured_data:
-                        nrefs_cache_hit = structured_data.ref_exists_cache_hit_count
-                nrefs_invalid = status.get("refs_invalid") or 0
-                bar.update(increment)
-            else:
-                bar.update(increment)
+            elif status.get(PROGRESS_PARSE.LOAD_ITEM) or status.get(PROGRESS_PARSE.LOAD_DONE):
+                if not status.get(PROGRESS_PARSE.LOAD_DONE):
+                    nrows_processed += increment
+                nrefs_total = status.get(PROGRESS_PARSE.LOAD_COUNT_REFS) or 0
+                nrefs_resolved = status.get(PROGRESS_PARSE.LOAD_COUNT_REFS_FOUND) or 0
+                nrefs_unresolved = status.get(PROGRESS_PARSE.LOAD_COUNT_REFS_NOT_FOUND) or 0
+                nrefs_lookup = status.get(PROGRESS_PARSE.LOAD_COUNT_REFS_LOOKUP) or 0
+                nrefs_exists_cache_hit = status.get(PROGRESS_PARSE.LOAD_COUNT_REFS_EXISTS_CACHE_HIT) or 0
+                nrefs_lookup_cache_hit = status.get(PROGRESS_PARSE.LOAD_COUNT_REFS_LOOKUP_CACHE_HIT) or 0
+                nrefs_invalid = status.get(PROGRESS_PARSE.LOAD_COUNT_REFS_INVALID) or 0
+                if not status.get(PROGRESS_PARSE.LOAD_DONE):
+                    bar.increment_progress(increment)
+            elif not status.get(PROGRESS_PARSE.LOAD_DONE):
+                bar.increment_progress(increment)
             message = f"▶ Rows: {nrows} | Parsed: {nrows_processed}"
             if nrefs_total > 0:
                 message += f" ‖ Refs: {nrefs_total}"
                 if nrefs_unresolved > 0:
                     message += f" | Unresolved: {nrefs_unresolved}"
-                if verbose and (nrefs_lookup > 0):
+                if nrefs_lookup > 0:
                     message += f" | Lookups: {nrefs_lookup}"
                 if nrefs_invalid > 0:
                     message += f" | Invalid: {nrefs_invalid}"
-                if verbose and (nrefs_cache_hit > 0):
-                    message += f" | Hits: {nrefs_cache_hit}"
-            message += " | Progress"
+                if (verbose or debug) and (nrefs_exists_cache_hit > 0):
+                    message += f" | Hits: {nrefs_exists_cache_hit}"
+                    if debug:
+                        message += f" [{nrefs_lookup_cache_hit}]"
             bar.set_description(message)
+            if status.get(PROGRESS_PARSE.LOAD_DONE):
+                bar.done()
 
         return progress_report
 
     if debug:
         PRINT("DEBUG: Starting client validation.")
 
     structured_data = StructuredDataSet(None, portal, autoadd=autoadd,
                                         ref_lookup_strategy=ref_lookup_strategy,
                                         ref_lookup_nocache=ref_nocache,
-                                        progress=None if noprogress else define_progress_callback(),
+                                        progress=None if noprogress else define_progress_callback(debug=debug),
                                         debug_sleep=debug_sleep)
-    structured_data._load_file(ingestion_filename)
+    structured_data.load_file(ingestion_filename)
 
     if debug:
         PRINT("DEBUG: Finished client validation.")
 
     if debug:
         PRINT_OUTPUT(f"DEBUG: Reference total count: {structured_data.ref_total_count}")
         PRINT_OUTPUT(f"DEBUG: Reference total found count: {structured_data.ref_total_found_count}")
@@ -2225,60 +2405,90 @@
     if json_only:
         PRINT_OUTPUT(json.dumps(structured_data.data, indent=4))
         exit(1)
     if verbose_json:
         PRINT_OUTPUT(f"Parsed JSON:")
         PRINT_OUTPUT(json.dumps(structured_data.data, indent=4))
     validation_okay = _validate_data(structured_data, portal, ingestion_filename,
-                                     upload_folder, recursive=subfolders, debug=debug)
+                                     upload_folder, recursive=subfolders, verbose=verbose, debug=debug)
     if validation_okay:
         PRINT("Validation results (preliminary): OK")
     elif exit_immediately_on_errors:
+        if verbose:
+            _print_structured_data_verbose(portal, structured_data, ingestion_filename, upload_folder=upload_folder,
+                                           recursive=subfolders, validation=validation, noanalyze=True, verbose=verbose)
         if output_file:
             PRINT_STDOUT(f"Exiting with preliminary validation errors; see your output file: {output_file}")
         else:
-            PRINT_STDOUT(f"\nExiting with preliminary validation errors.")
+            if not verbose:
+                PRINT_STDOUT()
+            PRINT_STDOUT(f"Exiting with preliminary validation errors.")
             PRINT_STDOUT("Use the --output FILE option to write errors to a file.")
         exit(1)
 
-    # Check files separately because we might want to let them get away with missing files.
-    nfiles_found, file_validation_errors = _validate_files(structured_data, ingestion_filename,
-                                                           upload_folder, recursive=subfolders)
-    if file_validation_errors:
-        nfiles = len(file_validation_errors)
-        PRINT(f"However there {'are' if nfiles != 1 else 'is'} {nfiles} file{'s' if nfiles != 1 else ''}"
-              f" referenced which {'are' if nfiles != 1 else 'is'} missing.")
-        if yes_or_no(f"Do you want to see a list of these {nfiles} missing file{'s' if nfiles != 1 else ''}?"):
-            for error in file_validation_errors:
-                PRINT(f"- {error}")
-        if not yes_or_no(f"Do you want to continue {'validation' if validation else 'submitting'}"
-                         f" even with {nfiles} file{'s' if nfiles != 1 else ''} missing?"):
-            exit(1)
-    if nfiles_found > 0:
-        PRINT(f"Files referenced for upload (and which exist): {nfiles_found}")
-    elif not file_validation_errors:
-        PRINT("No files to upload were referenced.")
+    # They don't want to present upload file info on validate, only on submit.
+    # _review_upload_files(structured_data, ingestion_filename,
+    #                      validation=validation, directory=upload_folder, recursive=subfolders)
 
     if verbose:
         _print_structured_data_verbose(portal, structured_data, ingestion_filename, upload_folder=upload_folder,
                                        recursive=subfolders, validation=validation, verbose=verbose)
     elif not quiet:
-        _print_structured_data_status(portal, structured_data, validation=validation,
-                                      report_updates_only=True, noprogress=noprogress, verbose=verbose, debug=debug)
+        if not noanalyze:
+            _print_structured_data_status(portal, structured_data, validation=validation,
+                                          report_updates_only=True, noprogress=noprogress, verbose=verbose, debug=debug)
+        else:
+            PRINT("Skipping analysis of metadata wrt creates/updates to be done (via --noanalyze).")
     if not validation_okay:
         if not yes_or_no(f"There are some preliminary errors outlined above;"
                          f" do you want to continue with {'validation' if validation else 'submission'}?"):
             exit(1)
     if validate_local_only:
         PRINT("Terminating as requested (via --validate-local-only).")
         exit(0 if validation_okay else 1)
 
+    return structured_data
+
+
+def _review_upload_files(structured_data: StructuredDataSet, ingestion_filename: str, validation: bool = False,
+                         directory: Optional[str] = None, recursive: bool = False) -> None:
+
+    nfiles_found, file_validation_errors = _validate_files(structured_data, ingestion_filename,
+                                                           upload_folder=directory, recursive=recursive)
+    if file_validation_errors:
+        nfiles = len(file_validation_errors)
+        if nfiles_found > 0:
+            PRINT(f"WARNING: There {'is' if nfiles == 1 else 'are'} {nfiles}"
+                  f" file{'' if nfiles == 1 else 's'} referenced which are missing.")
+        else:
+            PRINT(f"WARNING: All {nfiles} file{'' if nfiles == 1 else 's'} are missing.")
+        if not (show_missing_files := (nfiles <= 3)):
+            show_missing_files = yes_or_no(f"Do you want to see a list of these {nfiles}"
+                                           f" missing file{'' if nfiles == 1 else 's'}?")
+        if show_missing_files:
+            for error in sorted(file_validation_errors):
+                PRINT(f"- {error}")
+        if nfiles_found == 0:
+            PRINT("No files found for upload.")
+            exit(1)
+        if not validation:
+            if not yes_or_no(f"Do you want to continue even with"
+                             f" {'this' if nfiles == 1 else 'these'} missing file{'' if nfiles == 1 else 's'}?"):
+                exit(1)
+        else:
+            PRINT(f"Continuing even with {'this' if nfiles == 1 else 'these'}"
+                  f" missing file{'' if nfiles == 1 else 's'} as noted above.")
+    if nfiles_found > 0:
+        PRINT(f"Files referenced for upload (and which exist): {nfiles_found}")
+    elif not file_validation_errors:
+        PRINT("No files to upload were referenced.")
+
 
 def _validate_data(structured_data: StructuredDataSet, portal: Portal, ingestion_filename: str,
-                   upload_folder: str, recursive: bool, debug: bool = False) -> bool:
+                   upload_folder: str, recursive: bool, verbose: bool = False, debug: bool = False) -> bool:
     nerrors = 0
 
     if initial_validation_errors := _validate_initial(structured_data, portal):
         nerrors += len(initial_validation_errors)
 
     if ref_validation_errors := _validate_references(structured_data.ref_errors, ingestion_filename, debug=debug):
         nerrors += len(ref_validation_errors)
@@ -2286,81 +2496,121 @@
     structured_data.validate()
     if data_validation_errors := structured_data.validation_errors:
         nerrors += len(data_validation_errors)
 
     if nerrors > 0:
         PRINT_OUTPUT("Validation results (preliminary): ERROR")
 
+    printed_newline = False
+
     if initial_validation_errors:
+        if not printed_newline:
+            PRINT_OUTPUT()
+            printed_newline = True
         PRINT_OUTPUT(f"- Initial errors: {len(initial_validation_errors)}")
         for error in initial_validation_errors:
             PRINT_OUTPUT(f"  - ERROR: {error}")
 
     if data_validation_errors:
+        if not printed_newline:
+            PRINT_OUTPUT()
+            printed_newline = True
         PRINT_OUTPUT(f"- Data errors: {len(data_validation_errors)}")
         for error in data_validation_errors:
             PRINT_OUTPUT(f"  - ERROR: {_format_issue(error, ingestion_filename)}")
 
     if ref_validation_errors:
-        _print_reference_errors(ref_validation_errors)
+        if not printed_newline:
+            PRINT_OUTPUT()
+            printed_newline = True
+        _print_reference_errors(ref_validation_errors, verbose=verbose, debug=debug)
         # PRINT_OUTPUT(f"- Reference errors: {len(ref_validation_errors)}")
         # if debug:
         #     for error in ref_validation_errors:
         #         PRINT_OUTPUT(f"  - ERROR: {error}")
         # else:
         #     for error in ref_validation_errors:
         #         PRINT_OUTPUT(f"  - ERROR: {error['ref']} (refs: {error['count']})")
 
     return not (nerrors > 0)
 
 
 def _validate_references(ref_errors: Optional[List[dict]], ingestion_filename: str, debug: bool = False) -> List[str]:
+    def normalize(ref_errors: Optional[List[dict]]) -> None:  # noqa
+        # Server sends back fill path to "file"; adjust to basename; fix on server (TODO).
+        if isinstance(ref_errors, list):
+            for ref_error in ref_errors:
+                if isinstance(src := ref_error.get("src"), dict) and isinstance(file := src.get("file"), str):
+                    src["file"] = os.path.basename(file)
+    normalize(ref_errors)
     ref_validation_errors = []
     ref_validation_errors_truncated = None
     if isinstance(ref_errors, list):
         for ref_error in ref_errors:
             if debug:
                 ref_validation_errors.append(f"{_format_issue(ref_error, ingestion_filename)}")
             elif ref_error.get("truncated") is True:
                 ref_validation_errors_truncated = {"ref": f"{_format_issue(ref_error, ingestion_filename)}"}
             elif ref_error.get("ref"):
+                # TODO: Can we actually get here?
                 ref_validation_errors.append(ref_error)
             else:
                 if ref := ref_error.get("error"):
-                    if ref_error := [r for r in ref_validation_errors if r.get("ref") == ref]:
-                        ref_error[0]["count"] += 1
+                    if ref_error_existing := [r for r in ref_validation_errors if r.get("ref") == ref]:
+                        ref_error_existing = ref_error_existing[0]
+                        ref_error_existing["count"] += 1
+                        if isinstance(src := ref_error.get("src"), dict):
+                            if isinstance(ref_error_existing.get("srcs"), list):
+                                ref_error_existing["srcs"].append(src)
+                            else:
+                                ref_error_existing["srcs"] = [src]
                     else:
-                        ref_validation_errors.append({"ref": ref, "count": 1})
+                        ref_validation_error = {"ref": ref, "count": 1}
+                        if isinstance(src := ref_error.get("src"), dict):
+                            ref_validation_error["srcs"] = [src]
+                        ref_validation_errors.append(ref_validation_error)
     if debug:
         ref_validation_errors = sorted(ref_validation_errors)
     else:
         ref_validation_errors = sorted(ref_validation_errors, key=lambda item: item.get("ref"))
     if ref_validation_errors_truncated:
         ref_validation_errors.append(ref_validation_errors_truncated)
     return ref_validation_errors
 
 
-def _print_reference_errors(ref_errors: List[dict], debug: bool = False) -> None:
+def _print_reference_errors(ref_errors: List[dict], verbose: bool = False, debug: bool = False) -> None:
+    if errors := _format_reference_errors(ref_errors=ref_errors, verbose=verbose, debug=debug):
+        for error in errors:
+            PRINT_OUTPUT(error)
+
+
+def _format_reference_errors(ref_errors: List[dict], verbose: bool = False, debug: bool = False) -> List[str]:
+    errors = []
     if isinstance(ref_errors, list) and ref_errors:
-        nref_errors = len([r for r in ref_errors if not r.get('ref', '').startswith('Truncated')])
-        PRINT_OUTPUT(f"- Reference errors: {nref_errors}")
+        nref_errors = len([r for r in ref_errors
+                           if (not isinstance(r, dict)) or (not r.get('ref', '').startswith('Truncated'))])
+        errors.append(f"- Reference errors: {nref_errors}")
         if debug:
             for ref_error in ref_errors:
-                PRINT_OUTPUT(f"  - ERROR: {ref_error}")
+                errors.append(f"  - ERROR: {ref_error}")
         else:
             truncated = None
             for ref_error in ref_errors:
                 if ref_error["ref"].startswith("Truncated"):
                     truncated = ref_error["ref"]
                 elif isinstance(count := ref_error.get("count"), int):
-                    PRINT_OUTPUT(f"  - ERROR: {ref_error['ref']} (refs: {count})")
+                    errors.append(f"  - ERROR: {ref_error['ref']} (refs: {count})")
+                    if verbose and isinstance(srcs := ref_error.get("srcs"), list):
+                        for src in srcs:
+                            errors.append(f"    - {_format_src(src)}")
                 else:
-                    PRINT_OUTPUT(f"  - ERROR: {ref_error['ref']}")
+                    errors.append(f"  - ERROR: {ref_error['ref']}")
             if truncated:
-                PRINT_OUTPUT(f"  - {truncated}")
+                errors.append(f"  - {truncated}")
+    return errors
 
 
 def _validate_files(structured_data: StructuredDataSet, ingestion_filename: str,
                     upload_folder: str, recursive: bool) -> Tuple[int, List[str]]:
     file_validation_errors = []
     if files := structured_data.upload_files_located(location=[upload_folder,
                                                                os.path.dirname(ingestion_filename) or "."],
@@ -2398,17 +2648,17 @@
                                     f"Missing required property ({missing_required_property})"
                                     f" for type: {schema_name}")
     return initial_validation_errors
 
 
 def _print_structured_data_verbose(portal: Portal, structured_data: StructuredDataSet, ingestion_filename: str,
                                    upload_folder: str, recursive: bool, validation: bool = False,
-                                   noprogress: bool = False, verbose: bool = False) -> None:
+                                   noanalyze: bool = False, noprogress: bool = False, verbose: bool = False) -> None:
     if (reader_warnings := structured_data.reader_warnings):
-        PRINT_OUTPUT(f"\n> Parser WARNINGS:")
+        PRINT_OUTPUT(f"\n> Parser warnings:")
         for reader_warning in reader_warnings:
             PRINT_OUTPUT(f"  - {_format_issue(reader_warning, ingestion_filename)}")
     PRINT_OUTPUT(f"\n> Types submitting:")
     for type_name in sorted(structured_data.data):
         PRINT_OUTPUT(f"  - {type_name}: {len(structured_data.data[type_name])}"
                      f" object{'s' if len(structured_data.data[type_name]) != 1 else ''}")
     if resolved_refs := structured_data.resolved_refs:
@@ -2422,89 +2672,82 @@
         if files_found := [file for file in files if file.get("path")]:
             for file in files_found:
                 path = file.get("path")
                 if not printed_header:
                     PRINT_OUTPUT(f"\n> Resolved file references:")
                     printed_header = True
                 PRINT_OUTPUT(f"  - {file.get('type')}: {file.get('file')} -> {path}"
-                             f" [{_format_file_size(_get_file_size(path))}]")
+                             f" [{format_size(get_file_size(path))}]")
     PRINT_OUTPUT()
-    _print_structured_data_status(portal, structured_data,
-                                  validation=validation,
-                                  report_updates_only=True, noprogress=noprogress, verbose=verbose)
+    if not noanalyze:
+        _print_structured_data_status(portal, structured_data,
+                                      validation=validation,
+                                      report_updates_only=True, noprogress=noprogress, verbose=verbose)
+    else:
+        PRINT("Skipping analysis of metadata wrt creates/updates to be done (via --noanalyze).")
 
 
 def _print_structured_data_status(portal: Portal, structured_data: StructuredDataSet,
                                   validation: bool = False,
                                   report_updates_only: bool = False,
                                   noprogress: bool = False, verbose: bool = False, debug: bool = False) -> None:
 
     if verbose:
         report_updates_only = False
 
     def define_progress_callback(debug: bool = False) -> None:
-        bar = None
         ntypes = 0
         nobjects = 0
         ncreates = 0
         nupdates = 0
         nlookups = 0
-        # started = time.time()
-        def handle_control_c(signum, frame):  # noqa
-            if yes_or_no("\nCTRL-C: You have interrupted this process. Do you want to TERMINATE processing?"):
-                if bar:
-                    bar.close()
-                PRINT("Premature exit.")
-                exit(1)
-            PRINT_STDOUT("Continuing ...")
+        bar = ProgressBar(nobjects, "Calculating", interrupt_exit=True, interrupt_message="analysis")
         def progress_report(status: dict) -> None:  # noqa
-            nonlocal bar, ntypes, nobjects, ncreates, nupdates, nlookups, debug, noprogress
+            nonlocal bar, ntypes, nobjects, ncreates, nupdates, nlookups, noprogress
             if noprogress:
                 return
             increment = 1
-            if status.get("start"):
-                signal.signal(signal.SIGINT, handle_control_c)
-                ntypes = status.get("types")
-                nobjects = status.get("objects")
+            if status.get(PROGRESS_PARSE.ANALYZE_START):
+                ntypes = status.get(PROGRESS_PARSE.ANALYZE_COUNT_TYPES)
+                nobjects = status.get(PROGRESS_PARSE.ANALYZE_COUNT_ITEMS)
+                bar.set_total(nobjects)
                 PRINT(f"Analyzing submission file which has {ntypes} type{'s' if ntypes != 1 else ''}"
                       f" and a total of {nobjects} object{'s' if nobjects != 1 else ''}.")
-                bar_format = "{l_bar}{bar}| {n_fmt}/{total_fmt} | {rate_fmt} | {elapsed}{postfix} | ETA: {remaining} "
-                bar = tqdm(total=nobjects, desc="Calculating", dynamic_ncols=True, bar_format=bar_format, unit="")
                 return
-            elif status.get("finish"):
-                if bar:
-                    bar.close()
-                signal.signal(signal.SIGINT, signal.SIG_DFL)
+            elif status.get(PROGRESS_PARSE.ANALYZE_DONE):
+                bar.done()
                 return
-            elif status.get("create"):
+            elif status.get(PROGRESS_PARSE.ANALYZE_CREATE):
                 ncreates += increment
-                nlookups += status.get("lookups") or 0
-                bar.update(increment)
-            elif status.get("update"):
+                nlookups += status.get(PROGRESS_PARSE.ANALYZE_LOOKUPS) or 0
+                bar.increment_progress(increment)
+            elif status.get(PROGRESS_PARSE.ANALYZE_UPDATE):
                 nupdates += increment
-                nlookups += status.get("lookups") or 0
-                bar.update(increment)
+                nlookups += status.get(PROGRESS_PARSE.ANALYZE_LOOKUPS) or 0
+                bar.increment_progress(increment)
             else:
-                nlookups += status.get("lookups") or 0
-                bar.update(increment)
+                nlookups += status.get(PROGRESS_PARSE.ANALYZE_LOOKUPS) or 0
+                bar.increment_progress(increment)
             # duration = time.time() - started
             # nprocessed = ncreates + nupdates
             # rate = nprocessed / duration
             # nremaining = nobjects - nprocessed
             # duration_remaining = (nremaining / rate) if rate > 0 else 0
             message = (
                 f"▶ Items: {nobjects} | Checked: {ncreates + nupdates}"
                 f" ‖ Creates: {ncreates} | Updates: {nupdates} | Lookups: {nlookups}")
             # if debug:
             #    message += f" | Rate: {rate:.1f}%"
-            message += " | Progress"
+            # message += " | Progress" # xyzzy
             bar.set_description(message)
         return progress_report
 
-    diffs = structured_data.compare(progress=define_progress_callback())
+    # TODO: Allow abort of compare by returning some value from the
+    # progress callback that just breaks out of the loop in structured_data.
+    diffs = structured_data.compare(progress=define_progress_callback(debug=debug))
 
     ncreates = 0
     nupdates = 0
     nsubstantive_updates = 0
     for object_type in diffs:
         for object_info in diffs[object_type]:
             if object_info.uuid:
@@ -2516,21 +2759,21 @@
 
     to_or_which_would = "which would" if validation else "to"
 
     if ncreates > 0:
         if nupdates > 0:
             message = f"Objects {to_or_which_would} be -> Created: {ncreates} | Updated: {nupdates}"
             if nsubstantive_updates == 0:
-                message += " (but no substantive differences)"
+                message += " (no substantive differences)"
         else:
             message = f"Objects {to_or_which_would} be created: {ncreates}"
     elif nupdates:
         message = f"Objects {to_or_which_would} be updated: {nupdates}"
         if nsubstantive_updates == 0:
-            message += " (but no substantive differences)"
+            message += " (no substantive differences)"
     else:
         message = "No objects {to_or_which_would} create or update."
         return
 
     if report_updates_only and nsubstantive_updates == 0:
         PRINT(f"{message}")
         return
@@ -2559,15 +2802,15 @@
                 printed_type = True
             PRINT(f"  - OBJECT: {object_info.path}")
             if not object_info.uuid:
                 PRINT(f"    Does not exist -> {will_or_would} be CREATED")
             else:
                 message = f"    Already exists -> {object_info.uuid} -> {will_or_would} be UPDATED"
                 if not object_info.diffs:
-                    message += " (but NO substantive diffs)"
+                    message += " (no substantive diffs)"
                     PRINT(message)
                 else:
                     message += " (substantive DIFFs below)"
                     PRINT(message)
                     for diff_path in object_info.diffs:
                         if (diff := object_info.diffs[diff_path]).creating_value:
                             PRINT(f"     CREATE {diff_path}: {diff.value}")
@@ -2583,65 +2826,71 @@
     json_string = json.dumps(data, indent=4)
     json_string = f"\n{prefix}".join(json_string.split("\n"))
     PRINT_OUTPUT(prefix, end="")
     PRINT_OUTPUT(json_string)
 
 
 def _format_issue(issue: dict, original_file: Optional[str] = None) -> str:
-    def src_string(issue: dict) -> str:
-        if not isinstance(issue, dict) or not isinstance(issue_src := issue.get("src"), dict):
-            return ""
-        show_file = original_file and (original_file.endswith(".zip") or
-                                       original_file.endswith(".tgz") or original_file.endswith(".gz"))
-        src_file = issue_src.get("file") if show_file else ""
-        src_type = issue_src.get("type")
-        src_column = issue_src.get("column")
-        src_row = issue_src.get("row", 0)
-        if src_file:
-            src = f"{os.path.basename(src_file)}"
-            sep = ":"
-        else:
-            src = ""
-            sep = "."
-        if src_type:
-            src += (sep if src else "") + src_type
-            sep = "."
-        if src_column:
-            src += (sep if src else "") + src_column
-        if src_row > 0:
-            src += (" " if src else "") + f"[{src_row}]"
-        if not src:
-            if issue.get("warning"):
-                src = "Warning"
-            elif issue.get("error"):
-                src = "Error"
-            else:
-                src = "Issue"
-        return src
     issue_message = None
     if issue:
         if error := issue.get("error"):
             issue_message = error.replace("'$.", "'")
             issue_message = error.replace("Validation error at '$': ", "")
         elif warning := issue.get("warning"):
             issue_message = warning
         elif issue.get("truncated"):
             return f"Truncated result set | More: {issue.get('more')} | See: {issue.get('details')}"
-    return f"{src_string(issue)}: {issue_message}" if issue_message else ""
+    return f"{_format_src(issue)}: {issue_message}" if issue_message else ""
+
+
+def _format_src(issue: dict) -> str:
+    def file_without_extension(file: str) -> str:
+        if isinstance(file, str):
+            if file.endswith(".gz"):
+                file = file[:-3]
+            if (dot := file.rfind(".")) > 0:
+                file = file[:dot]
+        return file
+    if not isinstance(issue, dict):
+        return ""
+    if not isinstance(issue_src := issue.get("src"), dict):
+        issue_src = issue
+    if src_type := issue_src.get("type"):
+        src = src_type
+    elif src_sheet := issue_src.get("sheet"):
+        src = src_sheet
+    elif src_file := file_without_extension(issue_src.get("file")):
+        src = src_file
+    else:
+        src = ""
+    if src_column := issue_src.get("column"):
+        src = f"{src}.{src_column}" if src else src_column
+    if (src_row := issue_src.get("row", 0)) > 0:
+        src = f"{src} [{src_row}]" if src else f"[{src_row}]"
+    if not src:
+        if issue.get("warning"):
+            src = "Warning"
+        elif issue.get("error"):
+            src = "Error"
+        else:
+            src = "Issue"
+    return src
 
 
 def _define_portal(key: Optional[dict] = None, env: Optional[str] = None, server: Optional[str] = None,
-                   app: Optional[str] = None, keys_file: Optional[str] = None,
-                   env_from_env: bool = False,
-                   report: bool = False, verbose: bool = False) -> Portal:
+                   app: Optional[str] = None, keys_file: Optional[str] = None, env_from_env: bool = False,
+                   report: bool = False, verbose: bool = False, note: Optional[str] = None) -> Portal:
 
     def get_default_keys_file():
         nonlocal app
         return os.path.expanduser(os.path.join(Portal.KEYS_FILE_DIRECTORY, f".{app.lower()}-keys.json"))
 
+    if not env and not env_from_env:
+        env_from_env = os.environ.get("SMAHT_ENV")
+
     raise_exception = True
     if not app:
         app = DEFAULT_APP
         app_default = True
     else:
         app_default = False
     portal = None
@@ -2664,40 +2913,44 @@
                     exit(1)
         except Exception:
             pass
         if raise_exception:
             raise Exception(
                 f"No portal key defined; setup your ~/.{app or 'smaht'}-keys.json file and use the --env argument.")
     if report:
+        message = f"SMaHT submitr version: {get_version()}"
+        if note:
+            message += f" | {note}"
+        PRINT(message)
         if verbose:
             PRINT(f"Portal app name is{' (default)' if app_default else ''}: {app}")
         PRINT(f"Portal environment (in keys file) is: {portal.env}{' (from SMAHT_ENV)' if env_from_env else ''}")
-        PRINT(f"Portal keys file is: {portal.keys_file}")
+        PRINT(f"Portal keys file is: {format_path(portal.keys_file)}")
         PRINT(f"Portal server is: {portal.server}")
         if portal.key_id and len(portal.key_id) > 2:
             PRINT(f"Portal key prefix is: {portal.key_id[:2]}******")
     return portal
 
 
 @lru_cache(maxsize=1)
 def _get_consortia(portal: Portal) -> List[str]:
     results = []
-    if consortia := portal.get_metadata("/consortia"):
+    if consortia := portal.get_metadata("/consortia?limit=1000"):
         consortia = sorted(consortia.get("@graph", []), key=lambda key: key.get("identifier"))
         for consortium in consortia:
             if ((consortium_name := consortium.get("identifier")) and
                 (consortium_uuid := consortium.get("uuid"))):  # noqa
                 results.append({"name": consortium_name, "uuid": consortium_uuid})
     return results
 
 
 @lru_cache(maxsize=1)
 def _get_submission_centers(portal: Portal) -> List[str]:
     results = []
-    if submission_centers := portal.get_metadata("/submission-centers"):
+    if submission_centers := portal.get_metadata("/submission-centers?limit=1000"):
         submission_centers = sorted(submission_centers.get("@graph", []), key=lambda key: key.get("identifier"))
         for submission_center in submission_centers:
             if ((submission_center_name := submission_center.get("identifier")) and
                 (submission_center_uuid := submission_center.get("uuid"))):  # noqa
                 results.append({"name": submission_center_name, "uuid": submission_center_uuid})
     return results
 
@@ -2713,54 +2966,57 @@
         if value.endswith(".gz"):
             value = value[:-3]
         value, _ = os.path.splitext(value)
         if _is_accession_id(value):
             return value
 
 
-def _tobool(value: Any, fallback: bool = False) -> bool:
-    if isinstance(value, bool):
-        return value
-    elif isinstance(value, str):
-        try:
-            return str_to_bool(value)
-        except Exception:
-            return fallback
-    else:
-        return fallback
-
-
-def _get_file_size(file: str) -> int:
-    return os.path.getsize(file)
-
-
-def _format_file_size(nbytes: int) -> str:
-    for unit in ["b", "Kb", "Mb", "Gb", "Tb", "Pb", "Eb", "Zb"]:
-        if abs(nbytes) < 1024.0:
-            return f"{nbytes:3.1f}{unit}"
-        nbytes /= 1024.0
-    return f"{nbytes:.1f}Yb"
-
-
 def _format_portal_object_datetime(value: str, verbose: bool = False) -> Optional[str]:  # noqa
-    try:
-        dt = datetime.fromisoformat(value).replace(tzinfo=pytz.utc)
-        tzlocal = datetime.now().astimezone().tzinfo
-        if verbose:
-            return dt.astimezone(tzlocal).strftime(f"%A, %B %-d, %Y | %-I:%M %p %Z")
-        else:
-            return dt.astimezone(tzlocal).strftime(f"%Y-%m-%d %H:%M:%S %Z")
-    except Exception:
-        return None
+    return format_datetime(datetime.fromisoformat(value))
 
 
-def _format_path(path: str) -> str:
-    if os.path.isabs(path) and path.startswith(os.path.expanduser("~")):
-        path = "~/" + Path(path).relative_to(Path.home()).as_posix()
-    return path
+def _print_metadata_file_info(file: str, env: str, refs: bool = False, output_file: Optional[str] = None) -> None:
+    if output_file:
+        set_output_file(output_file)
+    PRINT(f"Metadata File: {os.path.basename(file)}")
+    if size := get_file_size(file):
+        PRINT(f"Size: {format_size(size)} ({size})")
+    if modified := get_file_modified_datetime(file):
+        PRINT(f"Modified: {modified}")
+    if md5 := get_file_md5(file):
+        PRINT(f"MD5: {md5}")
+    if etag := get_file_md5_like_aws_s3_etag(file):
+        PRINT(f"S3 ETag: {etag}{' | Same as MD5' if md5 == etag else ''}")
+    sheet_lines = []
+    if file.endswith(".xlsx") or file.endswith(".xls"):
+        from dcicutils.data_readers import Excel
+        excel = Excel(file)
+        nrows_total = 0
+        nsheets = 0
+        for sheet_name in sorted(excel.sheet_names):
+            nsheets += 1
+            nrows = 0
+            for row in excel.sheet_reader(sheet_name):
+                nrows += 1
+            sheet_lines.append(f"- Sheet: {sheet_name} ▶ Rows: {nrows}")
+            nrows_total += nrows
+        sheet_lines = "\n" + "\n".join(sheet_lines)
+        PRINT(f"Sheets: {nsheets} | Rows: {nrows_total}{sheet_lines}")
+    if refs is True:
+        portal = _define_portal(env=env)
+        structured_data = StructuredDataSet(file, portal, norefs=True)
+        refs = structured_data.resolved_refs
+        PRINT(f"References: {len(refs) or 'None'}")
+        if output_file and len(refs) > 7:
+            PRINT_STDOUT(f"- See your output file: {output_file}")
+            for ref in sorted(refs):
+                PRINT_OUTPUT(f"- {ref}")
+        else:
+            for ref in sorted(refs):
+                PRINT(f"- {ref}")
 
 
 def _ping(app: str, env: str, server: str, keys_file: str,
           env_from_env: bool = False, verbose: bool = False) -> bool:
     portal = _define_portal(env=env, server=server, app=app, keys_file=keys_file,
                             env_from_env=env_from_env, report=verbose)
     return portal.ping()
```

### Comparing `smaht_submitr-0.7.0.1b9/submitr/tests/data/submission_simple.xlsx` & `smaht_submitr-0.7.0.1b90/submitr/tests/data/submission_simple.xlsx`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b9/submitr/tests/data/submission_simple2.xlsx` & `smaht_submitr-0.7.0.1b90/submitr/tests/data/submission_simple2.xlsx`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b9/submitr/tests/data/submission_test.xlsx` & `smaht_submitr-0.7.0.1b90/submitr/tests/data/submission_test.xlsx`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b9/submitr/tests/data/submission_test_with_errors.xlsx` & `smaht_submitr-0.7.0.1b90/submitr/tests/data/submission_test_with_errors.xlsx`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b9/submitr/tests/test_base.py` & `smaht_submitr-0.7.0.1b90/submitr/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b9/submitr/tests/test_check_submission.py` & `smaht_submitr-0.7.0.1b90/submitr/tests/test_check_submission.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b9/submitr/tests/test_exceptions.py` & `smaht_submitr-0.7.0.1b90/submitr/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b9/submitr/tests/test_make_sample_fastq_file.py` & `smaht_submitr-0.7.0.1b90/submitr/tests/test_make_sample_fastq_file.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b9/submitr/tests/test_misc.py` & `smaht_submitr-0.7.0.1b90/submitr/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b9/submitr/tests/test_resume_uploads.py` & `smaht_submitr-0.7.0.1b90/submitr/tests/test_resume_uploads.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,117 +34,123 @@
                         if expect_called:
                             assert mock_resume_uploads.called_with(**expect_call_args)
                         assert output == expect_output
 
     test_it(args_in=[], expect_exit_code=2, expect_called=False,
             expect_output=["Missing submission UUID or referenced file UUID or accession ID."])  # Missing args
     test_it(args_in=['some-guid'], expect_exit_code=0, expect_called=True, expect_call_args={
-        'bundle_filename': None,
+        'bundle': None,
         'env': None,
         'server': None,
         'uuid': 'some-guid',
         'upload_folder': None,
         'no_query': False,
         'subfolders': False,
     })
     expect_call_args = {
-        'bundle_filename': '${tmpdir}/some.file',
+        'bundle': '${tmpdir}/some.file',
         'env': None,
         'server': None,
         'uuid': 'some-guid',
         'upload_folder': None,
         'no_query': False,
         'subfolders': False,
     }
-    test_it(args_in=['-b', '${tmpdir}/some.file', 'some-guid'],
+    test_it(args_in=['--bundle', '${tmpdir}/some.file', 'some-guid'],
             expect_exit_code=0,
             expect_called=True,
             expect_call_args=expect_call_args)
-    test_it(args_in=['some-guid', '-b', 'some.file'],
+    test_it(args_in=['some-guid', '--bundle', 'some.file'],
             expect_exit_code=0,
             expect_called=True,
             expect_call_args=expect_call_args)
     expect_call_args = {
-        'bundle_filename': '${tmpdir}/some.file',
+        'bundle': '${tmpdir}/some.file',
         'env': 'some-env',
         'server': None,
         'uuid': 'some-guid',
         'upload_folder': None,
         'no_query': False,
         'subfolders': False,
     }
-    test_it(args_in=['some-guid', '-b', 'some.file', '-e', 'some-env'],
+    test_it(args_in=['some-guid', '--bundle', 'some.file', '--env', 'some-env'],
             expect_exit_code=0,
             expect_called=True,
             expect_call_args=expect_call_args)
-    test_it(args_in=['-b', '${tmpdir}/some.file', '-e', 'some-env', 'some-guid'],
+    test_it(args_in=['--bundle', '${tmpdir}/some.file', '--env', 'some-env', 'some-guid'],
             expect_exit_code=0,
             expect_called=True,
             expect_call_args=expect_call_args)
     expect_call_args = {
-        'bundle_filename': '${tmpdir}/some.file',
+        'bundle': '${tmpdir}/some.file',
         'env': 'some-env',
         'server': 'http://some.server',
         'uuid': 'some-guid',
         'upload_folder': None,
         'no_query': False,
         'subfolders': False,
     }
-    test_it(args_in=['some-guid', '-b', '${tmpdir}/some.file', '-e', 'some-env', '-s', 'http://some.server'],
+    test_it(args_in=['some-guid', '--bundle', '${tmpdir}/some.file',
+                     '--env', 'some-env', '--server', 'http://some.server'],
             expect_exit_code=0,
             expect_called=True,
             expect_call_args=expect_call_args)
-    test_it(args_in=['-b', '${tmpdir}/some.file', '-e', 'some-env', '-s', 'http://some.server', 'some-guid'],
+    test_it(args_in=['--bundle', '${tmpdir}/some.file', '--env',
+                     'some-env', '--server', 'http://some.server', 'some-guid'],
             expect_exit_code=0,
             expect_called=True,
             expect_call_args=expect_call_args)
     expect_call_args = {
-        'bundle_filename': '${tmpdir}/some.file',
+        'bundle': '${tmpdir}/some.file',
         'env': 'some-env',
         'server': 'http://some.server',
         'uuid': 'some-guid',
         'upload_folder': '${tmpdir}/a-folder',
         'no_query': False,
         'subfolders': False,
     }
-    test_it(args_in=['some-guid', '-b',
-                     '${tmpdir}/some.file', '-e', 'some-env', '-s', 'http://some.server', '-u', '${tmpdir}/a-folder'],
+    test_it(args_in=['some-guid', '--bundle',
+                     '${tmpdir}/some.file', '--env', 'some-env',
+                     '--server', 'http://some.server', '--directory', '${tmpdir}/a-folder'],
             expect_exit_code=0,
             expect_called=True,
             expect_call_args=expect_call_args)
-    test_it(args_in=['-b', '${tmpdir}/some.file', '-e', 'some-env', '-s', 'http://some.server', 'some-guid',
-                     '--upload_folder', '${tmpdir}/a-folder'],
+    test_it(args_in=['--bundle', '${tmpdir}/some.file', '--env', 'some-env',
+                     '--server', 'http://some.server', 'some-guid',
+                     '--directory', '${tmpdir}/a-folder'],
             expect_exit_code=0,
             expect_called=True,
             expect_call_args=expect_call_args)
     expect_call_args = {
-        'bundle_filename': '${tmpdir}/some.file',
+        'bundle': '${tmpdir}/some.file',
         'env': None,
         'server': 'http://some.server',
         'uuid': 'some-guid',
         'upload_folder': '${tmpdir}/a-folder',
         'no_query': True,
         'subfolders': False,
     }
-    test_it(args_in=['some-guid', '-b',
-                     '${tmpdir}/some.file', '-s', 'http://some.server', '-u', '${tmpdir}/a-folder', '-nq'],
+    test_it(args_in=['some-guid', '--bundle',
+                     '${tmpdir}/some.file', '--server', 'http://some.server',
+                     '--directory', '${tmpdir}/a-folder', '--yes'],
             expect_exit_code=0,
             expect_called=True,
             expect_call_args=expect_call_args)
     expect_call_args = {
-        'bundle_filename': '${tmpdir}/some.file',
+        'bundle': '${tmpdir}/some.file',
         'env': None,
         'server': 'http://some.server',
         'uuid': 'some-guid',
         'upload_folder': '${tmpdir}/a-folder',
         'no_query': True,
         'subfolders': True,
     }
-    test_it(args_in=['some-guid', '-b',
-                     '${tmpdir}/some.file', '-s', 'http://some.server', '-u', '${tmpdir}/a-folder', '-nq', '-sf'],
+    test_it(args_in=['some-guid', '--bundle',
+                     '${tmpdir}/some.file', '--server', 'http://some.server',
+                     '--directory', '${tmpdir}/a-folder', '--yes'],
             expect_exit_code=0,
             expect_called=True,
             expect_call_args=expect_call_args)
 
 
 SAMPLE_UPLOAD_INFO = [
     {'uuid': 'df6e0e21-e575-4bd1-b81f-60d78e23a544', 'filename': 'f1.fastq.gz'},
@@ -162,15 +168,15 @@
 
 
 def test_c4_383_regression_action():
     """
     Check that bug C4-383 is really fixed.
 
     This bug involves resume_uploads not merging the uploaded file against the current directory
-    when no bundle_filename or upload_folder is given. The present behavior is to merge against
+    when no bundle or upload_folder is given. The present behavior is to merge against
     the parent directory.
     """
     output = []
     with temporary_directory() as current_dir:
         for upload_info in SAMPLE_UPLOAD_INFO:
             upload_info["filename"] = os.path.join(current_dir, upload_info["filename"])
             open(upload_info["filename"], "w")
@@ -183,15 +189,15 @@
                 with mock.patch.object(os.path, "curdir", current_dir):
                     with mock.patch.object(submission_module, "yes_or_no", return_value=True):
                         with mock.patch.object(submission_module, "upload_file_to_uuid") as mock_upload_file_to_uuid:
                             with mock.patch("requests.get") as mock_requests_get:
                                 with mock.patch(
                                         "dcicutils.portal_utils.Portal.get_metadata") as mock_requests_get_metadata:
 
-                                    def mocked_requests_get_metadata(url):
+                                    def mocked_requests_get_metadata(url, raise_exception=True):
                                         return INGESTION_FRAGMENT_WITH_UPLOAD_INFO
 
                                     def mocked_requests_get(url, raise_for_status=False, *args, **kwargs):
                                         if "/profiles" in url:
                                             return MockResponse(200, json={})
                                         ignored(args, kwargs)
                                         assert "ingestion-submissions" in url
@@ -219,9 +225,10 @@
                                             assert e.code == 0
                                         joined_filename = os.path.join(current_dir, SAMPLE_UPLOAD_INFO[-1]['filename'])
                                         # Make sure this is doing what we expect.
                                         assert current_dir + "/" in joined_filename
                                         # Make sure the inner upload actually uploads to the current dir.
                                         mock_upload_file_to_uuid.assert_called_with(auth=fake_keydict,
                                                                                     filename=joined_filename,
-                                                                                    uuid=SAMPLE_UPLOAD_INFO[-1]['uuid'])
+                                                                                    uuid=SAMPLE_UPLOAD_INFO[-1]['uuid'],
+                                                                                    first_time=False, portal=mock.ANY)
                                         assert output == []
```

### Comparing `smaht_submitr-0.7.0.1b9/submitr/tests/test_show_upload_info.py` & `smaht_submitr-0.7.0.1b90/submitr/tests/test_show_upload_info.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b9/submitr/tests/test_submission.py` & `smaht_submitr-0.7.0.1b90/submitr/tests/test_submission.py`

 * *Files 1% similar despite different names*

```diff
@@ -661,15 +661,16 @@
                     )
                     mock_yes_or_no.assert_called_with("Upload these %s files?" % n_uploads)
                     mock_uploads.assert_called_with(
                         SOME_UPLOAD_INFO,
                         auth=SOME_KEYDICT,
                         folder=tmpdir,  # the folder part of given SOME_BUNDLE_FILENAME
                         no_query=False,
-                        subfolders=False
+                        subfolders=False,
+                        portal=mock.ANY
                     )
                     assert shown.lines == []
 
                 with shown_output() as shown:
                     do_any_uploads(
                         res=SOME_UPLOAD_INFO_RESULT,
                         keydict=SOME_KEYDICT,
@@ -678,15 +679,16 @@
                     )
                     mock_yes_or_no.assert_called_with("Upload these %s files?" % n_uploads)
                     mock_uploads.assert_called_with(
                         SOME_UPLOAD_INFO,
                         auth=SOME_KEYDICT,
                         folder=os.path.join(tmpdir, SOME_OTHER_BUNDLE_FOLDER[1:]),  # passed straight through
                         no_query=False,
-                        subfolders=False
+                        subfolders=False,
+                        portal=mock.ANY
                     )
                     assert shown.lines == []
 
                 with shown_output() as shown:
                     do_any_uploads(
                         res=SOME_UPLOAD_INFO_RESULT,
                         keydict=SOME_KEYDICT,
@@ -695,34 +697,36 @@
                     )
                     mock_yes_or_no.assert_called_with("Upload these %s files?" % n_uploads)
                     mock_uploads.assert_called_with(
                         SOME_UPLOAD_INFO,
                         auth=SOME_KEYDICT,
                         folder=tmpdir,  # No folder
                         no_query=False,
-                        subfolders=False
+                        subfolders=False,
+                        portal=mock.ANY
                     )
                     assert shown.lines == []
 
                 with shown_output() as shown:
                     do_any_uploads(
                         res=SOME_UPLOAD_INFO_RESULT,
                         keydict=SOME_KEYDICT,
                         # from which a folder can be inferred
                         ingestion_filename=os.path.join(tmpdir, SOME_BUNDLE_FILENAME[1:]),
                         no_query=False,
-                        subfolders=True,
+                        subfolders=True
                     )
                     mock_uploads.assert_called_with(
                         SOME_UPLOAD_INFO,
                         auth=SOME_KEYDICT,
                         # the folder part of given SOME_BUNDLE_FILENAME
                         folder=os.path.join(tmpdir, SOME_BUNDLE_FILENAME_FOLDER[1:]),
                         no_query=False,
-                        subfolders=True
+                        subfolders=True,
+                        portal=mock.ANY
                     )
                     assert shown.lines == []
 
         with mock.patch.object(submission_module, "do_uploads") as mock_uploads:
 
             # n_uploads = len(SOME_UPLOAD_INFO)
 
@@ -736,15 +740,16 @@
                 )
                 mock_uploads.assert_called_with(
                     SOME_UPLOAD_INFO,
                     auth=SOME_KEYDICT,
                     # the folder part of given SOME_BUNDLE_FILENAME
                     folder=os.path.join(tmpdir, SOME_BUNDLE_FILENAME_FOLDER[1:]),
                     no_query=True,
-                    subfolders=False
+                    subfolders=False,
+                    portal=mock.ANY
                 )
                 assert shown.lines == []
 
 
 def test_resume_uploads():
 
     with mock.patch.object(command_utils_module, "script_catch_errors", script_dont_catch_errors):
@@ -757,15 +762,16 @@
                                        keydict=SOME_KEYDICT)
                         mock_do_any_uploads.assert_called_with(
                             some_response_json,
                             keydict=SOME_KEYDICT,
                             ingestion_filename=SOME_BUNDLE_FILENAME,
                             upload_folder=None,
                             no_query=False,
-                            subfolders=False)
+                            subfolders=False,
+                            portal=mock.ANY)
 
     with mock.patch.object(command_utils_module, "script_catch_errors", script_dont_catch_errors):
         with mock.patch.object(submission_module, "_resolve_server", return_value=SOME_SERVER):
             with mock.patch("requests.get", return_value=FakeResponse(401, json=SOME_BAD_RESULT)):
                 with mock.patch("dcicutils.portal_utils.Portal.get_metadata", return_value=SOME_BAD_RESULT):
                     with mock.patch.object(submission_module, "do_any_uploads") as mock_do_any_uploads:
                         with pytest.raises(Exception):
@@ -805,15 +811,15 @@
     with mock.patch.object(os, "name", os_name):
         with mock.patch.object(platform, "system") as mock_system:
             mock_system.side_effect = mocked_system
             yield
 
 
 @pytest.mark.parametrize("os_simulation_mode", OS_SIMULATION_MODE_NAMES)
-def test_execute_prearranged_upload(os_simulation_mode: str):
+def obsolete_test_execute_prearranged_upload(os_simulation_mode: str):
     Portal.KEYS_FILE_DIRECTORY = "/dummy"
     with os_simulation(simulation_mode=os_simulation_mode):
         with mock.patch.object(os, "environ", SOME_ENVIRON.copy()):
             with shown_output() as shown:
                 with pytest.raises(ValueError):
                     bad_credentials = SOME_UPLOAD_CREDENTIALS.copy()
                     bad_credentials.pop('SessionToken')
@@ -936,23 +942,25 @@
         assert get_s3_encrypt_key_id_from_health_page(auth='not-used-by-mock') == mocked_s3_encrypt_key_id
 
 
 def test_upload_file_to_uuid():
 
     with mock.patch("dcicutils.portal_utils.Portal.patch_metadata", return_value=SOME_UPLOAD_CREDENTIALS_RESULT):
         with mock.patch.object(submission_module, "execute_prearranged_upload") as mocked_upload:
-            metadata = upload_file_to_uuid(filename=SOME_FILENAME, uuid=SOME_UUID, auth=SOME_AUTH)
+            metadata = upload_file_to_uuid(filename=SOME_FILENAME, uuid=SOME_UUID,
+                                           auth=SOME_AUTH, first_time=False, portal=None)
             assert metadata == SOME_FILE_METADATA
             mocked_upload.assert_called_with(SOME_FILENAME, auth=SOME_AUTH,
                                              upload_credentials=SOME_UPLOAD_CREDENTIALS)
 
     with mock.patch("dcicutils.portal_utils.Portal.patch_metadata", return_value=SOME_BAD_RESULT):
         with mock.patch.object(submission_module, "execute_prearranged_upload") as mocked_upload:
             try:
-                upload_file_to_uuid(filename=SOME_FILENAME, uuid=SOME_UUID, auth=SOME_AUTH)
+                upload_file_to_uuid(filename=SOME_FILENAME, uuid=SOME_UUID,
+                                    auth=SOME_AUTH, first_time=False, portal=None)
             except Exception as e:
                 assert str(e).startswith("Unable to obtain upload credentials")
             else:
                 raise Exception("Expected error was not raised.")  # pragma: no cover - we hope this never happens
             assert mocked_upload.call_count == 0
 
 
@@ -978,15 +986,15 @@
 def test_do_uploads(tmp_path):
 
     @contextlib.contextmanager
     def mock_uploads():
 
         uploaded = {}
 
-        def mocked_upload_file(filename, uuid, auth):
+        def mocked_upload_file(filename, uuid, auth, first_time=False, portal=None):
             if auth != SOME_AUTH:
                 raise Exception("Bad auth")
             uploaded[uuid] = filename
 
         with mock.patch.object(submission_module, "upload_file_to_uuid", mocked_upload_file):
             yield uploaded  # This starts out empty when yielded, but as uploads occur will get populated.
 
@@ -1089,15 +1097,17 @@
             auth=SOME_AUTH,
             folder=subfolder,
             no_query=True,
         )
         mock_upload.assert_called_with(
             filename=file_path,
             uuid=uuid,
-            auth=SOME_AUTH
+            auth=SOME_AUTH,
+            first_time=True,
+            portal=mock.ANY
         )
 
     with shown_output() as shown:
         with mock.patch.object(submission_module, "upload_file_to_uuid") as mock_upload:
             # File not found, so pass join of folder and file.
             do_uploads(
                 upload_spec_list,
@@ -1116,15 +1126,17 @@
             folder=folder,
             no_query=True,
             subfolders=True,
         )
         mock_upload.assert_called_with(
             filename=file_path,
             uuid=uuid,
-            auth=SOME_AUTH
+            auth=SOME_AUTH,
+            first_time=True,
+            portal=mock.ANY
         )
 
     with mock.patch.object(submission_module, "upload_file_to_uuid") as mock_upload:
         # Multiple matching files found; show lines and don't call for upload.
         with shown_output() as shown:
             another_file_path = folder / "foo.fastq.gz"
             another_file_path.write_text("")
@@ -1198,15 +1210,16 @@
             mocked_portal_key_property.return_value = SOME_KEYDICT
             with mock.patch.object(submission_module, "yes_or_no", return_value=True):
                 with mock.patch.object(submission_module, "upload_file_to_uuid") as mock_upload:
                     with mock.patch("dcicutils.portal_utils.Portal.get_metadata", return_value={"@type": "File"}):
                         with mock.patch("dcicutils.portal_utils.Portal.get_schemas", return_value={}):
                             _upload_item_data(item_filename=some_filename,
                                               uuid=SOME_UUID, server=SOME_SERVER, env=SOME_ENV)
-                            mock_upload.assert_called_with(filename=some_filename, uuid=SOME_UUID, auth=SOME_KEYDICT)
+                            mock_upload.assert_called_with(filename=some_filename,
+                                                           uuid=SOME_UUID, auth=SOME_KEYDICT, portal=mock.ANY)
 
         with mock.patch.object(Portal, "key", new_callable=mock.PropertyMock) as mocked_portal_key_property:
             mocked_portal_key_property.return_value = SOME_KEYDICT
             with mock.patch.object(submission_module, "yes_or_no", return_value=False):
                 with mock.patch.object(submission_module, "upload_file_to_uuid") as mock_upload:
                     with mock.patch("dcicutils.portal_utils.Portal.get_metadata", return_value={"@type": "File"}):
                         with mock.patch("dcicutils.portal_utils.Portal.get_schemas", return_value={}):
@@ -1224,15 +1237,16 @@
         with mock.patch.object(Portal, "key", new_callable=mock.PropertyMock) as mocked_portal_key_property:
             mocked_portal_key_property.return_value = SOME_KEYDICT
             with mock.patch.object(submission_module, "upload_file_to_uuid") as mock_upload:
                 with mock.patch("dcicutils.portal_utils.Portal.get_metadata", return_value={"@type": "File"}):
                     with mock.patch("dcicutils.portal_utils.Portal.get_schemas", return_value={}):
                         _upload_item_data(item_filename=some_filename, uuid=SOME_UUID,
                                           server=SOME_SERVER, env=SOME_ENV, no_query=True)
-                        mock_upload.assert_called_with(filename=some_filename, uuid=SOME_UUID, auth=SOME_KEYDICT)
+                        mock_upload.assert_called_with(filename=some_filename,
+                                                       uuid=SOME_UUID, auth=SOME_KEYDICT, portal=mock.ANY)
 
 
 def get_today_datetime_for_time(time_to_use):
     today = datetime.date.today()
     time = datetime.time.fromisoformat(time_to_use)
     datetime_at_time_to_use = datetime.datetime.fromisoformat(
         f"{today.isoformat()}T{time.isoformat()}"
```

### Comparing `smaht_submitr-0.7.0.1b9/submitr/tests/test_submit_genelist.py` & `smaht_submitr-0.7.0.1b90/submitr/tests/test_submit_genelist.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b9/submitr/tests/test_submit_metadata_bundle.py` & `smaht_submitr-0.7.0.1b90/submitr/tests/test_submit_metadata_bundle.py`

 * *Files 24% similar despite different names*

```diff
@@ -54,21 +54,21 @@
         # 'project': "some-project",
         'validate_remote_only': True,
         'upload_folder': None,
         'no_query': False,
         'subfolders': False,
     }
     test_it(args_in=["--env", "some-env",  # "--institution", "some-institution",
-                     "-s", "some-server", "-v",  # "-p", "some-project",
+                     "--server", "some-server", "--validate",  # "-p", "some-project",
                      some_file],
             expect_exit_code=0,
             expect_called=True,
             expect_call_args=expect_call_args)
     test_it(args_in=[some_file, "--env", "some-env",  # "--institution", "some-institution",
-                     "-s", "some-server", "--validate-only"],  # , "--project", "some-project"],
+                     "--server", "some-server", "--validate-only"],  # , "--project", "some-project"],
             expect_exit_code=0,
             expect_called=True,
             expect_call_args=expect_call_args)
     expect_call_args = {
         'ingestion_filename': some_file,
         'ingestion_type': DEFAULT_INGESTION_TYPE,
         'env': "some-env",
@@ -78,27 +78,27 @@
         'validate_remote_only': False,
         'upload_folder': 'a-folder',
         'no_query': False,
         'subfolders': False,
     }
     test_it(args_in=["--env", "some-env",
                      # "--institution", "some-institution",
-                     "-s", "some-server",
+                     "--server", "some-server",
                      # "-p", "some-project",
-                     '-u', 'a-folder',
+                     '--directory', 'a-folder',
                      some_file],
             expect_exit_code=0,
             expect_called=True,
             expect_call_args=expect_call_args)
     test_it(args_in=[some_file,
                      "--env", "some-env",
                      # "--institution", "some-institution",
-                     "-s", "some-server",
+                     "--server", "some-server",
                      # "--project", "some-project",
-                     '--upload_folder', 'a-folder'],
+                     '--directory', 'a-folder'],
             expect_exit_code=0,
             expect_called=True,
             expect_call_args=expect_call_args)
     expect_call_args = {
         'ingestion_filename': some_file,
         'ingestion_type': 'simulated_bundle',
         'env': "some-env",
@@ -108,30 +108,30 @@
         'validate_remote_only': True,
         'upload_folder': 'a-folder',
         'no_query': False,
         'subfolders': False,
     }
     test_it(args_in=["--env", "some-env",
                      # "--institution", "some-institution",
-                     "-s", "some-server",
-                     "-v",
+                     "--server", "some-server",
+                     "--validate",
                      # "-p", "some-project",
-                     '-u', 'a-folder',
-                     '-t', 'simulated_bundle',
+                     '--directory', 'a-folder',
+                     '--ingestion_type', 'simulated_bundle',
                      some_file],
             expect_exit_code=0,
             expect_called=True,
             expect_call_args=expect_call_args)
     test_it(args_in=[some_file,
                      "--env", "some-env",
                      # "--institution", "some-institution",
-                     "-s", "some-server",
+                     "--server", "some-server",
                      "--validate-only",
                      # "--project", "some-project",
-                     '--upload_folder', 'a-folder',
+                     '--directory', 'a-folder',
                      '--ingestion_type', 'simulated_bundle'],
             expect_exit_code=0,
             expect_called=True,
             expect_call_args=expect_call_args)
     expect_call_args = {
         'ingestion_filename': some_file,
         'ingestion_type': DEFAULT_INGESTION_TYPE,
@@ -141,22 +141,22 @@
         # 'project': "some-project",
         'validate_remote_only': True,
         'upload_folder': None,
         'no_query': True,
         'subfolders': True,
     }
     test_it(args_in=["--env", "some-env",  # "--institution", "some-institution",
-                     "-s", "some-server", "-v",  # "-p", "some-project",
-                     some_file, '-nq', '-sf'],
+                     "--server", "some-server", "--validate",  # "-p", "some-project",
+                     some_file, '--yes'],
             expect_exit_code=0,
             expect_called=True,
             expect_call_args=expect_call_args)
     test_it(args_in=["--env", "some-env",  # "--institution", "some-institution",
-                     "-s", "some-server", "-v",  # "-p", "some-project",
-                     some_file, '--no_query', '--subfolders'],
+                     "--server", "some-server", "--validate",  # "-p", "some-project",
+                     some_file, '--yes'],
             expect_exit_code=0,
             expect_called=True,
             expect_call_args=expect_call_args)
 
 
 def _create_some_temporary_file() -> str:
     some_file = tempfile.NamedTemporaryFile(delete=False)
```

### Comparing `smaht_submitr-0.7.0.1b9/submitr/tests/test_submit_ontology.py` & `smaht_submitr-0.7.0.1b90/submitr/tests/test_submit_ontology.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b9/submitr/tests/test_testing_helpers.py` & `smaht_submitr-0.7.0.1b90/submitr/tests/test_testing_helpers.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b9/submitr/tests/test_upload_item_data.py` & `smaht_submitr-0.7.0.1b90/submitr/tests/test_upload_item_data.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b9/submitr/tests/test_utils.py` & `smaht_submitr-0.7.0.1b90/submitr/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b9/submitr/tests/testing_helpers.py` & `smaht_submitr-0.7.0.1b90/submitr/tests/testing_helpers.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b9/PKG-INFO` & `smaht_submitr-0.7.0.1b90/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smaht-submitr
-Version: 0.7.0.1b9
+Version: 0.7.0.1b90
 Summary: Support for uploading file submissions to SMAHT.
 Home-page: https://github.com/smaht-dac/submitr
 License: MIT
 Keywords: submitr,smaht
 Author: SMaHT DAC
 Author-email: smhelp@hms-dbmi.atlassian.net 
 Requires-Python: >=3.8.0,<3.12
@@ -23,15 +23,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Database :: Database Engines/Servers
 Requires-Dist: PyYAML (>=6.0.1,<7.0.0)
 Requires-Dist: awscli (>=1.32.49)
 Requires-Dist: boto3 (>=1.34.49,<2.0.0)
-Requires-Dist: dcicutils (>=8.8.1.1b1,<9.0.0.0)
+Requires-Dist: dcicutils (>=8.8.2,<9.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Project-URL: Repository, https://github.com/smaht-dac/submitr.git
 Description-Content-Type: text/x-rst
 
 
 .. image:: https://staging.smaht.org/static/img/docs/submitr_logo.png
     :target: https://pypi.org/project/smaht-submitr/
@@ -84,16 +84,16 @@
 
 Installation
 ============
 
 Installing this system involves these steps:
 
 1. Install Python and optionally a virtual environment manager of your choice (e.g. ``pyenv``)..
-3. Install this package with: ``pip install smaht-submitr``
-4. Setup your SMaHT Portal credentials file: ``~/.smaht-keys.json``. See `SMaHT Submitr Credentals <https://submitr.readthedocs.io/en/draft/installation.html>`_ for more in this.
+2. Install this package with: ``pip install smaht-submitr``
+3. Setup your SMaHT Portal credentials file: ``~/.smaht-keys.json``. See `SMaHT Submitr Credentials <https://submitr.readthedocs.io/en/draft/installation.html>`_ for more in this.
 
 See detailed information about installation see: `Installing SMaHT Submitr <https://submitr.readthedocs.io/en/draft/installation.html>`_.
 
 
 Getting Started
 ===============
```

