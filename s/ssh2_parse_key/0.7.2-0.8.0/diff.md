# Comparing `tmp/ssh2_parse_key-0.7.2.tar.gz` & `tmp/ssh2_parse_key-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssh2_parse_key-0.7.2.tar", last modified: Wed Nov  4 09:50:54 2020, max compression
+gzip compressed data, was "ssh2_parse_key-0.8.0.tar", max compression
```

## Comparing `ssh2_parse_key-0.7.2.tar` & `ssh2_parse_key-0.8.0.tar`

### file list

```diff
@@ -1,38 +1,37 @@
--rw-r--r--   0        0        0     1701 2020-11-04 09:50:05.282135 ssh2_parse_key-0.7.2/CHANGELOG.md
--rw-r--r--   0        0        0     2684 2020-11-04 09:50:05.282135 ssh2_parse_key-0.7.2/CONTRIBUTING.md
--rw-r--r--   0        0        0     1076 2020-11-04 09:50:05.282135 ssh2_parse_key-0.7.2/LICENSE
--rw-r--r--   0        0        0     2070 2020-11-04 09:50:05.282135 ssh2_parse_key-0.7.2/README.md
--rw-r--r--   0        0        0       17 2020-11-04 09:50:05.282135 ssh2_parse_key-0.7.2/docs/changelog.md
--rw-r--r--   0        0        0       20 2020-11-04 09:50:05.282135 ssh2_parse_key-0.7.2/docs/contributing.md
--rw-r--r--   0        0        0      689 2020-11-04 09:50:05.282135 ssh2_parse_key-0.7.2/docs/css/mkdocstrings.css
--rw-r--r--   0        0        0       14 2020-11-04 09:50:05.282135 ssh2_parse_key-0.7.2/docs/index.md
--rw-r--r--   0        0        0      125 2020-11-04 09:50:05.282135 ssh2_parse_key-0.7.2/docs/library.md
--rw-r--r--   0        0        0     1084 2020-11-04 09:50:05.282135 ssh2_parse_key-0.7.2/docs/license.md
--rw-r--r--   0        0        0     1380 2020-11-04 09:50:05.282135 ssh2_parse_key-0.7.2/pyproject.toml
--rw-r--r--   0        0        0      211 2020-11-04 09:50:05.282135 ssh2_parse_key-0.7.2/ssh2_parse_key/__init__.py
--rw-r--r--   0        0        0    14795 2020-11-04 09:50:05.282135 ssh2_parse_key-0.7.2/ssh2_parse_key/ssh2_parse_key.py
--rw-r--r--   0        0        0       44 2020-11-04 09:50:05.282135 ssh2_parse_key-0.7.2/tests/__init__.py
--rwxr-xr-x   0        0        0      696 2020-11-04 09:50:05.282135 ssh2_parse_key-0.7.2/tests/data/build_data.sh
--rw-r--r--   0        0        0      672 2020-11-04 09:50:05.282135 ssh2_parse_key-0.7.2/tests/data/test_key_dsa
--rw-r--r--   0        0        0      616 2020-11-04 09:50:05.282135 ssh2_parse_key-0.7.2/tests/data/test_key_dsa.pub
--rw-r--r--   0        0        0      722 2020-11-04 09:50:05.282135 ssh2_parse_key-0.7.2/tests/data/test_key_dsa_rfc4716.pub
--rw-r--r--   0        0        0      227 2020-11-04 09:50:05.282135 ssh2_parse_key-0.7.2/tests/data/test_key_ecdsa
--rw-r--r--   0        0        0      190 2020-11-04 09:50:05.282135 ssh2_parse_key-0.7.2/tests/data/test_key_ecdsa.pub
--rw-r--r--   0        0        0      275 2020-11-04 09:50:05.282135 ssh2_parse_key-0.7.2/tests/data/test_key_ecdsa_rfc4716.pub
--rw-r--r--   0        0        0      432 2020-11-04 09:50:05.282135 ssh2_parse_key-0.7.2/tests/data/test_key_ed25519
--rw-r--r--   0        0        0      112 2020-11-04 09:50:05.282135 ssh2_parse_key-0.7.2/tests/data/test_key_ed25519.pub
--rw-r--r--   0        0        0      202 2020-11-04 09:50:05.282135 ssh2_parse_key-0.7.2/tests/data/test_key_ed25519_rfc4716.pub
--rw-r--r--   0        0        0     2459 2020-11-04 09:50:05.282135 ssh2_parse_key-0.7.2/tests/data/test_key_rsa
--rw-r--r--   0        0        0      580 2020-11-04 09:50:05.282135 ssh2_parse_key-0.7.2/tests/data/test_key_rsa.pub
--rw-r--r--   0        0        0      685 2020-11-04 09:50:05.282135 ssh2_parse_key-0.7.2/tests/data/test_key_rsa_rfc4716.pub
--rw-r--r--   0        0        0     1894 2020-11-04 09:50:05.282135 ssh2_parse_key-0.7.2/tests/test_convert_public_key.py
--rw-r--r--   0        0        0     4067 2020-11-04 09:50:05.282135 ssh2_parse_key-0.7.2/tests/test_handle_crlf_line_ends.py
--rw-r--r--   0        0        0     1040 2020-11-04 09:50:05.282135 ssh2_parse_key-0.7.2/tests/test_load_keys_with_comments.py
--rw-r--r--   0        0        0     1898 2020-11-04 09:50:05.282135 ssh2_parse_key-0.7.2/tests/test_load_multiple_key.py
--rw-r--r--   0        0        0      744 2020-11-04 09:50:05.282135 ssh2_parse_key-0.7.2/tests/test_load_multiple_short.py
--rw-r--r--   0        0        0      995 2020-11-04 09:50:05.282135 ssh2_parse_key-0.7.2/tests/test_load_private_key.py
--rw-r--r--   0        0        0      588 2020-11-04 09:50:05.282135 ssh2_parse_key-0.7.2/tests/test_no_valid_keys.py
--rw-r--r--   0        0        0     1909 2020-11-04 09:50:05.282135 ssh2_parse_key-0.7.2/tests/test_openssh_public_key_load.py
--rw-r--r--   0        0        0     2312 2020-11-04 09:50:05.282135 ssh2_parse_key-0.7.2/tests/test_rfc4716_public_key_load.py
--rw-r--r--   0        0        0     2831 2020-11-04 09:50:54.654117 ssh2_parse_key-0.7.2/setup.py
--rw-r--r--   0        0        0     3110 2020-11-04 09:50:54.654475 ssh2_parse_key-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0     1715 2024-04-06 15:51:12.569777 ssh2_parse_key-0.8.0/CHANGELOG.md
+-rw-r--r--   0        0        0     2693 2023-11-27 11:49:17.759100 ssh2_parse_key-0.8.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1076 2023-11-25 10:07:38.390527 ssh2_parse_key-0.8.0/LICENSE
+-rw-r--r--   0        0        0     2090 2023-11-27 17:01:24.000000 ssh2_parse_key-0.8.0/README.md
+-rw-r--r--   0        0        0       17 2023-11-25 10:07:38.391189 ssh2_parse_key-0.8.0/docs/changelog.md
+-rw-r--r--   0        0        0       20 2023-11-25 10:07:38.391347 ssh2_parse_key-0.8.0/docs/contributing.md
+-rw-r--r--   0        0        0      709 2023-11-25 10:18:34.215438 ssh2_parse_key-0.8.0/docs/css/mkdocstrings.css
+-rw-r--r--   0        0        0       14 2023-11-25 10:07:38.391717 ssh2_parse_key-0.8.0/docs/index.md
+-rw-r--r--   0        0        0      125 2023-11-25 10:07:38.391838 ssh2_parse_key-0.8.0/docs/library.md
+-rw-r--r--   0        0        0     1084 2023-11-25 10:07:38.391944 ssh2_parse_key-0.8.0/docs/license.md
+-rw-r--r--   0        0        0     2653 2024-04-06 15:51:12.568885 ssh2_parse_key-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0      212 2024-04-06 15:51:12.569280 ssh2_parse_key-0.8.0/ssh2_parse_key/__init__.py
+-rw-r--r--   0        0        0    14849 2024-04-06 14:22:21.818276 ssh2_parse_key-0.8.0/ssh2_parse_key/ssh2_parse_key.py
+-rw-r--r--   0        0        0       44 2023-11-25 10:07:38.393248 ssh2_parse_key-0.8.0/tests/__init__.py
+-rwxr-xr-x   0        0        0      696 2023-11-25 10:07:38.393444 ssh2_parse_key-0.8.0/tests/data/build_data.sh
+-rw-r--r--   0        0        0      672 2023-11-25 10:07:38.393574 ssh2_parse_key-0.8.0/tests/data/test_key_dsa
+-rw-r--r--   0        0        0      616 2023-11-25 10:07:38.393746 ssh2_parse_key-0.8.0/tests/data/test_key_dsa.pub
+-rw-r--r--   0        0        0      722 2023-11-25 10:07:38.393952 ssh2_parse_key-0.8.0/tests/data/test_key_dsa_rfc4716.pub
+-rw-r--r--   0        0        0      227 2023-11-25 10:07:38.394106 ssh2_parse_key-0.8.0/tests/data/test_key_ecdsa
+-rw-r--r--   0        0        0      190 2023-11-25 10:07:38.394231 ssh2_parse_key-0.8.0/tests/data/test_key_ecdsa.pub
+-rw-r--r--   0        0        0      275 2023-11-25 10:07:38.394415 ssh2_parse_key-0.8.0/tests/data/test_key_ecdsa_rfc4716.pub
+-rw-r--r--   0        0        0      432 2023-11-25 10:07:38.394569 ssh2_parse_key-0.8.0/tests/data/test_key_ed25519
+-rw-r--r--   0        0        0      112 2023-11-25 10:07:38.394736 ssh2_parse_key-0.8.0/tests/data/test_key_ed25519.pub
+-rw-r--r--   0        0        0      202 2023-11-25 10:07:38.394905 ssh2_parse_key-0.8.0/tests/data/test_key_ed25519_rfc4716.pub
+-rw-r--r--   0        0        0     2459 2023-11-25 10:07:38.395045 ssh2_parse_key-0.8.0/tests/data/test_key_rsa
+-rw-r--r--   0        0        0      580 2023-11-25 10:07:38.395166 ssh2_parse_key-0.8.0/tests/data/test_key_rsa.pub
+-rw-r--r--   0        0        0      685 2023-11-25 10:07:38.395296 ssh2_parse_key-0.8.0/tests/data/test_key_rsa_rfc4716.pub
+-rw-r--r--   0        0        0     2137 2024-04-06 14:22:21.817722 ssh2_parse_key-0.8.0/tests/test_convert_public_key.py
+-rw-r--r--   0        0        0     4432 2024-04-06 14:22:21.817871 ssh2_parse_key-0.8.0/tests/test_handle_crlf_line_ends.py
+-rw-r--r--   0        0        0     1112 2024-04-06 14:22:21.817624 ssh2_parse_key-0.8.0/tests/test_load_keys_with_comments.py
+-rw-r--r--   0        0        0     2151 2024-04-06 14:22:21.817715 ssh2_parse_key-0.8.0/tests/test_load_multiple_key.py
+-rw-r--r--   0        0        0      748 2024-04-06 14:22:21.817576 ssh2_parse_key-0.8.0/tests/test_load_multiple_short.py
+-rw-r--r--   0        0        0     1225 2024-04-06 14:22:21.817644 ssh2_parse_key-0.8.0/tests/test_load_private_key.py
+-rw-r--r--   0        0        0      624 2024-04-06 14:22:21.817565 ssh2_parse_key-0.8.0/tests/test_no_valid_keys.py
+-rw-r--r--   0        0        0     2270 2024-04-06 14:22:21.817710 ssh2_parse_key-0.8.0/tests/test_openssh_public_key_load.py
+-rw-r--r--   0        0        0     2667 2024-04-06 14:22:21.817778 ssh2_parse_key-0.8.0/tests/test_rfc4716_public_key_load.py
+-rw-r--r--   0        0        0     3275 1970-01-01 00:00:00.000000 ssh2_parse_key-0.8.0/PKG-INFO
```

### Comparing `ssh2_parse_key-0.7.2/CHANGELOG.md` & `ssh2_parse_key-0.8.0/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,51 +1,59 @@
 # Changelog
+
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 
 <!-- insertion marker -->
-[0.7.2] - 2020-11-04
+[0.8.0] - 2024-04-06
 --------------------
+## [0.7.2] - 2020-11-04
+
 - Removed debug print statement mistakenly left in place
 
-[0.7.1] - 2020-10-29
---------------------
+## [0.7.1] - 2020-10-29
+
 - Fixed bug where parsing multiple keys could fail as the parser managed
   to almagamate them into  an unparsable block
 - Tweaks to README and infrastructure
 
 ## [0.6.2]  - 2020-10-16
+
 - Failed tag and docs generation fixed.  No functional changes
 
 ## [0.5.0]  - 2020-10-16
+
 - Swapped the [classforge](https://classforge.io/) base classing to
   [attrs](https://www.attrs.org)
 - Added a lot of additional type annotations to assist with attrs conversion -
   this also assists in the documentation markup,  These needed to be carefully
   handled to make portable to python under travis.  Aditionally the
   `OrderedDict[str, str]` annotation completely broke mkdocs/mkdocstrings.
 
 ## [0.4.0]  - 2020-10-16
+
 ### Packaging
+
 - Switched to using poetry for development and release
 - Updated the `pre-commit` pipeline, with some minor formatting reworks
 - Switch to [MkDocs](https://www.mkdocs.org/) for documentation, along with
   [mkdocstrings](https://github.com/pawamoy/mkdocstrings/) for API documentation
 
 ## [0.3.x]  - 2020-09-27
+
 - Fixed up documentation
 - Added a few additional tests
 - This is now reasonably presentable
 
-
 ## [0.2.x]  - 2020-09-25
+
 - First release
 - Documentation build
 - CI and release automation
 
-
 ## [0.1.0]  - 2020-05-07
+
 - First builds - never release on PyPI.
 
 ----
```

### Comparing `ssh2_parse_key-0.7.2/CONTRIBUTING.md` & `ssh2_parse_key-0.8.0/CONTRIBUTING.md`

 * *Files 10% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 Contributions are welcome, and they are greatly appreciated! Every little bit
 helps, and credit will always be given.
 
 You can contribute in many ways:
 
 ## Report Bugs
 
-Report bugs at https://github.com/nigelm/ssh2_parse_key/issues.
+Report bugs at <https://github.com/nigelm/ssh2_parse_key/issues>.
 
 If you are reporting a bug, please include:
 
-- Your operating system name and version.
-- Any details about your local setup that might be helpful in troubleshooting.
-- Detailed steps to reproduce the bug.
+-   Your operating system name and version.
+-   Any details about your local setup that might be helpful in troubleshooting.
+-   Detailed steps to reproduce the bug.
 
 ## Fix Bugs
 
 Look through the GitHub issues for bugs. Anything tagged with "bug" and "help
 wanted" is open to whoever wants to implement it.
 
 ## Implement Features
@@ -29,65 +29,62 @@
 
 `ssh2_parse_key` could always use more documentation, whether as part of the
 official docs, in docstrings, or even on the web in blog posts, articles, and
 such.
 
 ## Submit Feedback
 
-The best way to send feedback is to file an issue at https://github.com/nigelm/ssh2_parse_key/issues.
+The best way to send feedback is to file an issue at
+<https://github.com/nigelm/ssh2_parse_key/issues>.
 
 If you are proposing a feature:
 
-- Explain in detail how it would work.
-- Keep the scope as narrow as possible, to make it easier to implement.
-- Remember that this is a volunteer-driven project, and that contributions
-  are welcome :)
+-   Explain in detail how it would work.
+-   Keep the scope as narrow as possible, to make it easier to implement.
+-   Remember that this is a volunteer-driven project, and that contributions are
+    welcome :)
 
-## Get Started!
+## Get Started
 
-Ready to contribute? Here's how to set up `ssh2_parse_key` for local development.
+Ready to contribute? Here's how to set up `ssh2_parse_key` for local
+development.
 
 1. Fork the `ssh2_parse_key` repo on GitHub.
 2. Clone your fork locally::
 
-    $ git clone git@github.com:your_name_here/ssh2_parse_key.git
+    $ git clone <git@github.com>:your_name_here/ssh2_parse_key.git
 
-3. We use `poetry` for development, this is how you set up your fork for local development
+3. We use `poetry` for development, this is how you set up your fork for local
+   development
 
-    $ cd ssh2_parse_key/
-    $ poetry install
+    $ cd ssh2_parse_key/ $ poetry install
 
 4. Create a branch for local development::
 
     $ git checkout -b name-of-your-bugfix-or-feature
 
-   Now you can make your changes locally.
+    Now you can make your changes locally.
 
-5. When you're done making changes, use pre-commit to do basic checks and ensure formatting
-   is consitant, and check that your changes pass the tests::
+5. When you're done making changes, use pre-commit to do basic checks and ensure
+   formatting is consitant, and check that your changes pass the tests::
 
-    $ pre-commit run
-    $ poetry run pytest
-    $ poetry run make docs    # generate local docs for checking
+    $ pre-commit run $ poetry run pytest $ poetry run make docs # generate local
+    docs for checking
 
-   pre-commit may need to be installed onto your system.
+    pre-commit may need to be installed onto your system.
 
 6. Commit your changes and push your branch to GitHub::
 
-    $ git add .
-    $ git commit -m "Your detailed description of your changes."
-    $ git push origin name-of-your-bugfix-or-feature
+    $ git add . $ git commit -m "Your detailed description of your changes." $
+    git push origin name-of-your-bugfix-or-feature
 
 7. Submit a pull request through the GitHub website.
 
+## Deploying
 
-# Deploying
+A reminder for the maintainers on how to deploy. Make sure all your changes are
+committed (including an entry in HISTORY.rst). Then run::
 
-A reminder for the maintainers on how to deploy.
-Make sure all your changes are committed (including an entry in HISTORY.rst).
-Then run::
-
-$ bump2version patch # possible: major / minor / patch
-$ git push
-$ git push --tags
+$ bump2version patch # possible: major / minor / patch $ git push $ git push
+--tags
 
 Travis will then deploy to PyPI if tests pass.
```

### Comparing `ssh2_parse_key-0.7.2/LICENSE` & `ssh2_parse_key-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ssh2_parse_key-0.7.2/README.md` & `ssh2_parse_key-0.8.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 # ssh2_parse_key
 
-[![ci](https://img.shields.io/travis/nigelm/ssh2_parse_key.svg)](https://travis-ci.com/nigelm/ssh2_parse_key)
+[![ci](https://img.shields.io/travis/com/nigelm/ssh2_parse_key.svg)](https://travis-ci.com/nigelm/ssh2_parse_key)
 [![documentation](https://img.shields.io/badge/docs-mkdocs%20material-blue.svg?style=flat)](https://nigelm.github.io/ssh2_parse_key/)
 [![pypi version](https://img.shields.io/pypi/v/ssh2_parse_key.svg)](https://pypi.python.org/pypi/ssh2_parse_key)
 
-Parses ssh2 public keys in either openssh or RFC4716/Secsh formats and
-converts to either format.
+Parses ssh2 public keys in either openssh or RFC4716/Secsh formats and converts
+to either format.
 
 At this point any attempt to work with private keys will raise an exception.
 
-----
+---
 
 ## Features
 
-- Reads public keys of the following encryption types:-
-    - `ssh-rsa`
-    - `ssh-dss`
-    - `ecdsa-sha2-nistp256`
-    - `ssh-ed25519`
-- Reads either Openssh or RFC4716 format public keys
-- Can read input sets with either or both formats in
-- Can output either format for any key
+-   Reads public keys of the following encryption types:-
+    -   `ssh-rsa`
+    -   `ssh-dss`
+    -   `ecdsa-sha2-nistp256`
+    -   `ssh-ed25519`
+-   Reads either Openssh or RFC4716 format public keys
+-   Can read input sets with either or both formats in
+-   Can output either format for any key
 
-----
+---
 
 ## Installation
 
 With `pip`:
+
 ```bash
 python3.6 -m pip install ssh2_parse_key
 ```
 
-----
+---
 
 ## Usage
 
 To use SSH2 Key Parsing in a project
 
 ```python
 from ssh2_parse_key import Ssh2Key
@@ -48,28 +49,31 @@
 
 # alternatively
 data = Path("/path/to/public_key").read_text()
 keys = Ssh2Key.parse(data)
 
 # now those keys can be dealt with...
 for public_key in keys:
-    print(f"This is a {key.type} key")
+    print(f"This is a {key.key_type} key")
     print(f"It uses {key.encryption} encryption")
     print(f"comment = {key.comment}")
     print(f"subject = {key.subject}")
 
     print("RFC4716 format representation")
     print(key.rfc4716())
 
     print("OpenSSH representation")
     print(key.openssh())
 ```
 
-----
+---
 
 ## Credits
 
-The package is strongly based on the perl [`Parse::SSH2::PublicKey`](https://metacpan.org/pod/Parse::SSH2::PublicKey) module.
+The package is strongly based on the perl
+[`Parse::SSH2::PublicKey`](https://metacpan.org/pod/Parse::SSH2::PublicKey)
+module.
 
-Development on the python version was done by [`Nigel Metheringham <nigelm@cpan.org>`](https://github.com/nigelm/)
+Development on the python version was done by
+[`Nigel Metheringham <nigelm@cpan.org>`](https://github.com/nigelm/)
 
-----
+---
```

### Comparing `ssh2_parse_key-0.7.2/docs/css/mkdocstrings.css` & `ssh2_parse_key-0.8.0/docs/css/mkdocstrings.css`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 /* Indentation. */
 div.doc-contents:not(.first) {
-  padding-left: 25px;
-  border-left: 4px solid rgba(230, 230, 230);
-  margin-bottom: 80px;
+    padding-left: 25px;
+    border-left: 4px solid rgba(230, 230, 230);
+    margin-bottom: 80px;
 }
 
 /* Don't capitalize names. */
 h5.doc-heading {
-  text-transform: none !important;
+    text-transform: none !important;
 }
 
 /* Don't use vertical space on hidden ToC entries. */
 .hidden-toc::before {
-  margin-top: 0 !important;
-  padding-top: 0 !important;
+    margin-top: 0 !important;
+    padding-top: 0 !important;
 }
 
 /* Don't show permalink of hidden ToC entries. */
 .hidden-toc a.headerlink {
-  display: none;
+    display: none;
 }
 
 /* Avoid breaking parameters name, etc. in table cells. */
 td code {
-  word-break: normal !important;
+    word-break: normal !important;
 }
 
 /* For pieces of Markdown rendered in table cells. */
 td p {
-  margin-top: 0 !important;
-  margin-bottom: 0 !important;
+    margin-top: 0 !important;
+    margin-bottom: 0 !important;
 }
```

### Comparing `ssh2_parse_key-0.7.2/docs/license.md` & `ssh2_parse_key-0.8.0/docs/license.md`

 * *Files identical despite different names*

### Comparing `ssh2_parse_key-0.7.2/ssh2_parse_key/ssh2_parse_key.py` & `ssh2_parse_key-0.8.0/ssh2_parse_key/ssh2_parse_key.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """Main module for `ssh2_parse_key` - provides `Ssh2Key()`"""
+
 import base64
+import os
 import re
 import struct
 import textwrap
-import typing
 from collections import OrderedDict
-from os import PathLike
-from typing import List
-from typing import Match
+from pathlib import Path
+from re import Match
+from typing import Self
 
 import attr
 
 SSH2_KEY_TYPES = ("public", "private")
 SSH2_KEY_ENCRYPTIONS = ("ssh-rsa", "ssh-dss", "ecdsa-sha2-nistp256", "ssh-ed25519")
 OPENSSH_PUBKEY_PATTERN = re.compile(
     r"""
@@ -52,46 +53,44 @@
     re.VERBOSE,
 )
 INT_LEN = 4
 
 
 @attr.s(slots=True, frozen=True, kw_only=True)
 class Ssh2Key:
-    """
-    Encapsulates an ssh public key
+    """Encapsulates an ssh public key
 
     An `Ssh2Key` object is immutable after creation.  Typically you would create
     `Ssh2Key` objects by using `parse()` or `parse_file()` class methods.
 
     Attributes:
         key: The ssh key itself, Base64 string
         type: one of `public` or `private`
         encryption: one of `ssh-rsa`, `ssh-dss`, `ecdsa-sha2-nistp256`, `ssh-ed25519`
         headers: Any headers for the key - eg Comment.
 
     """
 
     key: str = attr.ib()
-    type: str = attr.ib(
+    key_type: str = attr.ib(
         default="public",
         validator=attr.validators.in_(SSH2_KEY_TYPES),
     )
     encryption: str = attr.ib(
         default="ssh-rsa",
         validator=attr.validators.in_(SSH2_KEY_ENCRYPTIONS),
     )
     headers = attr.ib(
         type=OrderedDict,
         default=attr.Factory(OrderedDict),
     )  # type: OrderedDict[str, str]
 
     @classmethod
-    def parse(cls, data: str) -> "List[Ssh2Key]":
-        """
-        Creates a set of `Ssh2Key` objects from a string of ssh key data
+    def parse(cls: type[Self], data: str) -> list[Self]:  # noqa: PLR0912
+        """Creates a set of `Ssh2Key` objects from a string of ssh key data
 
         Accepts a block of text containing SSH2 public keys (in either OpenSSH or
         SECSH format) and parses out SSH2 public keys returning them as `Ssh2Key`
         Objects.
 
         Arguments:
             data: A multiline string of ssh key data in OpenSSH or SECSH format
@@ -101,64 +100,63 @@
             ValueError: No valid ssh keys found
 
         Returns:
             keys: A list of  `Ssh2Key` objects
 
         """
         lines = data.splitlines()  # break the input into lines
-        keys: "List[Ssh2Key]" = []
+        keys: list[Self] = []
         inside_keyblock = False  # where we are
-        keyblock: "List[str]" = []
+        keyblock: list[str] = []
         keytype = ""
         pubpriv = ""
 
         for line in lines:
             matches = KEY_BOUNDARY_PATTERN.match(line)
-            if inside_keyblock and matches and matches.group("beginend") == "END":
-                inside_keyblock = False  # no longer within a keyblock
-                if keytype == matches.group("keytype") and pubpriv == matches.group(
-                    "pubpriv",
-                ):
-                    if keytype in ["OPENSSH", "DSA", "EC", "RSA"]:
-                        key = cls._parse_openssh(keyblock, keytype, pubpriv)
-                    elif keytype == "SSH2":
-                        key = cls._parse_secsh(keyblock, pubpriv)
-                    else:
-                        raise ValueError(
-                            f"Unrecognised type of ssh key {keytype}",
-                        )
-                    if key:
-                        keys.append(key)
-                keyblock = []  # fresh keyblock for next key
-            elif inside_keyblock:
-                keyblock.append(line)
+            if inside_keyblock:
+                if matches and matches.group("beginend") == "END":
+                    inside_keyblock = False  # no longer within a keyblock
+                    if keytype == matches.group("keytype") and pubpriv == matches.group(
+                        "pubpriv",
+                    ):
+                        if keytype in ["OPENSSH", "DSA", "EC", "RSA"]:
+                            keys.append(cls._parse_openssh(keyblock, keytype, pubpriv))
+                        elif keytype == "SSH2":
+                            keys.append(cls._parse_secsh(keyblock, pubpriv))
+                        else:
+                            msg = f"Unrecognised type of ssh key {keytype}"
+                            raise ValueError(
+                                msg,
+                            )
+                    keyblock = []  # fresh keyblock for next key
+                else:
+                    keyblock.append(line)
             elif matches and matches.group("beginend") == "BEGIN":
                 keytype = matches.group("keytype")
                 pubpriv = matches.group("pubpriv")
                 inside_keyblock = True  # inside a new keyblock
             else:
                 # check for OpenSSH format -- all on one line
                 matches = OPENSSH_PUBKEY_PATTERN.match(line)
                 if matches:
                     keys.append(cls._parse_openssh_oneline(matches))
-
                 else:
                     # raise ValueError("Unrecognised type of ssh key")
                     pass  # ignore for now
 
         if len(keys) == 0:
-            raise ValueError("No valid ssh keys found")
+            msg = "No valid ssh keys found"
+            raise ValueError(msg)
 
         # return the assemblage of keys
         return keys
 
     @classmethod
-    def parse_file(cls, filepath: "PathLike[str]") -> "List[Ssh2Key]":
-        """
-        Creates a set of `Ssh2Key` objects from a file of ssh key data
+    def parse_file(cls: type[Self], filepath: str | os.PathLike[str]) -> list[Self]:
+        """Creates a set of `Ssh2Key` objects from a file of ssh key data
 
         Accepts a block of text containing SSH2 public keys (in either OpenSSH or
         SECSH format) and parses out SSH2 public keys returning them as `Ssh2Key`
         Objects.
 
         Arguments:
             filepath: Pathname of a file of ssh key data in OpenSSH or SECSH format
@@ -167,43 +165,43 @@
             IOError: From underlying open/read
             ValueError: Unrecognised type of ssh key
             ValueError: No valid ssh keys found
 
         Returns:
             keys: A list of  `Ssh2Key` objects
         """
-        with open(filepath) as f:
-            data = f.read()
-            return cls.parse(data)
+        return cls.parse(Path(filepath).read_text())
 
     @classmethod
-    def _parse_openssh_oneline(cls, matches: Match):
+    def _parse_openssh_oneline(cls: type[Self], matches: Match) -> Self:
         """Build a openssh public key from regex match components."""
         key = matches.group("key")
         encryption = matches.group("encryption")
         headers = OrderedDict([("Comment", matches.group("comment"))])
-        return cls(key=key, type="public", encryption=encryption, headers=headers)
+        return cls(key=key, key_type="public", encryption=encryption, headers=headers)
 
     @classmethod
-    def _parse_openssh(cls, keyblock: "List[str]", keytype: str, pubpriv: str) -> None:
+    def _parse_openssh(cls: type[Self], keyblock: list[str], keytype: str, pubpriv: str) -> Self:  # noqa: ARG003
         """Decode an openssh keyblock into a key object."""
-        raise ValueError("Cannot currently decode openssh format keyblocks")
+        msg = "Cannot currently decode openssh format keyblocks"
+        raise ValueError(msg)
 
     @classmethod
-    def _parse_secsh(cls, keyblock: "List[str]", pubpriv: str) -> "Ssh2Key":
+    def _parse_secsh(cls: type[Self], keyblock: list[str], pubpriv: str) -> Self:
         """Decode an secsh/RFC4716 keyblock into a key object."""
         if pubpriv != "PUBLIC":
-            raise ValueError("Can only decode secsh public keys")
+            msg = "Can only decode secsh public keys"
+            raise ValueError(msg)
         headers, data, key = cls._initial_parse_keyblock(keyblock)
-        current_position, encryption = cls._unpack_by_int(data, 0)
-        encryption = encryption.decode()
-        return cls(key=key, type="public", encryption=encryption, headers=headers)
+        current_position, encryption_bytes = cls._unpack_by_int(data, 0)
+        encryption = encryption_bytes.decode()
+        return cls(key=key, key_type="public", encryption=encryption, headers=headers)
 
     @classmethod
-    def _initial_parse_keyblock(cls, keyblock: "List[str]") -> tuple:
+    def _initial_parse_keyblock(cls: type[Self], keyblock: "list[str]") -> tuple:
         headers = OrderedDict([("Comment", "")])  # default empty comment
         in_header = False
         header = ""
         value = ""
         index = 0
         for line in keyblock:
             if in_header:
@@ -231,63 +229,60 @@
                     break  # all out of headers
             index = index + 1
         data = base64.b64decode("".join(keyblock[index:]))
         key = base64.b64encode(data).decode()  # build clean version without spaces etc
         return (headers, data, key)
 
     @classmethod
-    def _unpack_by_int(cls, data: bytes, current_position: int):
+    def _unpack_by_int(cls: type[Self], data: bytes, current_position: int) -> tuple[int, bytes]:
         """Returns a tuple with (location of next data field, contents of requested data field)."""
         # Unpack length of data field
         try:
             requested_data_length = struct.unpack(
                 ">I",
-                data[current_position : current_position + INT_LEN],  # noqa: E203
+                data[current_position : current_position + INT_LEN],
             )[0]
-        except struct.error:
-            raise ValueError("Unable to unpack %s bytes from the data" % INT_LEN)
+        except struct.error as err:
+            raise ValueError("Unable to unpack %s bytes from the data" % INT_LEN) from err
 
         # Move pointer to the beginning of the data field
         current_position += INT_LEN
         remaining_data_length = len(data[current_position:])
 
         if remaining_data_length < requested_data_length:
+            msg = f"Requested {requested_data_length} bytes, but only {remaining_data_length} bytes available."
             raise ValueError(
-                "Requested %s bytes, but only %s bytes available."
-                % (requested_data_length, remaining_data_length),
+                msg,
             )
 
-        next_data = data[
-            current_position : current_position + requested_data_length  # noqa: E203
-        ]
+        next_data = data[current_position : current_position + requested_data_length]
         # Move pointer to the end of the data field
         current_position += requested_data_length
         return current_position, next_data
 
-    def secsh(self) -> str:
-        """
-        Returns an SSH public key in SECSH format (as specified in RFC4716).
+    def secsh(self: Self) -> str:
+        """Returns an SSH public key in SECSH format (as specified in RFC4716).
+
         Preserves headers and the order of headers.  Returned as a single
         string including newlines and with terminating newline.
 
         See http://tools.ietf.org/html/rfc4716
 
-        Arguments:
-
         Raises:
             ValueError: Unable to output secsh format private keys
 
         Returns:
             string: Single secsh key as a string including newlines and with terminating newline.
         """
-        lines: "List[str]" = []
-        if self.type == "public":
+        lines: "list[str]" = []
+        if self.key_type == "public":
             key_header_chunk = "SSH2 PUBLIC KEY"
         else:
-            raise ValueError("Unable to output secsh format private keys")
+            msg = "Unable to output secsh format private keys"
+            raise ValueError(msg)
             key_header_chunk = "SSH2 ENCRYPTED PRIVATE KEY"
 
         # add the wrapping header
         lines.append(f"---- BEGIN {key_header_chunk} ----")
 
         # add the headers, if any
         if len(self.headers):
@@ -300,51 +295,47 @@
         # add the wrapping footer
         lines.append(f"---- END {key_header_chunk} ----")
         lines.append("")  # force terminating newline
 
         # return the assembled string
         return "\n".join(lines)
 
-    def rfc4716(self) -> str:
-        """
-        Returns an SSH public key in SECSH format (as specified in RFC4716).
+    def rfc4716(self: Self) -> str:
+        """Returns an SSH public key in SECSH format (as specified in RFC4716).
+
         Preserves headers and the order of headers.  Returned as a single
         string including newlines and with terminating newline.
 
         Alias - ``rfc4716()`` just calls ``secsh()``
 
         See http://tools.ietf.org/html/rfc4716
 
-        Arguments:
-
         Raises:
             ValueError: Unable to output secsh format private keys
 
         Returns:
             string: Single secsh key as a string including newlines and with terminating newline.
         """
         return self.secsh()
 
-    def openssh(self) -> str:
-        """
-        Returns an SSH public/private key in OpenSSH format. Preserves 'comment'
+    def openssh(self: Self) -> str:
+        """Returns an SSH public/private key in OpenSSH format. Preserves 'comment'
+
         field parsed from either SECSH or OpenSSH.  Returned as a single
         string including newlines and with terminating newline.
 
-        Arguments:
-
         Raises:
             ValueError: Unable to output openssh format private keys
 
         Returns:
             string: Single openssh key as a string including newlines and with terminating newline.
         """
-        lines: "List[str]" = []
-        if self.type == "public":
-            lines.append(" ".join([self.encryption, self.key, self.comment()]))
+        lines: list[str] = []
+        if self.key_type == "public":
+            lines.append(f"{self.encryption} {self.key} {self.comment()}")
         else:
             # ## Initial code to deal with private keys not used
             # # private key - obviously!
             # # add the wrapping header
             # lines.append(f"---- BEGIN {self.encryption} PRIVATE KEY ----")
             #
             # # add the headers, if any
@@ -353,50 +344,44 @@
             #         self._encode_header(lines, header, value, 64)
             #
             # # add the key content
             # lines.extend(textwrap.wrap(self.key, 64))
             #
             # # add the wrapping footer
             # lines.append(f"---- END {self.encryption} PRIVATE KEY ----")
-            raise ValueError("Unable to output openssh format private keys")
+            msg = "Unable to output openssh format private keys"
+            raise ValueError(msg)
         lines.append("")  # force terminating newline
 
         # return the assembled string
         return "\n".join(lines)
 
-    def comment(self) -> str:
-        """
-        Returns the comment header from a ssh key object.
-
-        Arguments:
+    def comment(self: Self) -> str:
+        """Returns the comment header from a ssh key object.
 
         Returns:
             string: Comment field or an empty string.
         """
         if "Comment" in self.headers:
             return self.headers["Comment"]
-        else:
-            return ""
+        return ""
 
-    def subject(self) -> "typing.Union[str, None]":
-        """
-        Returns the subject header from a ssh key object.
-
-        Arguments:
+    def subject(self: Self) -> str | None:
+        """Returns the subject header from a ssh key object.
 
         Returns:
             string: Subject field or `None`.
         """
         if "Subject" in self.headers:
             return self.headers["Subject"]
         return None
 
     def _encode_header(
-        self,
-        data: "List[str]",
+        self: Self,
+        data: "list[str]",
         header: str,
         value: str,
         limit: int,
     ) -> None:
         bits = textwrap.wrap(f"{header}: {value}", limit)
         last = bits.pop()
         for bit in bits:
```

### Comparing `ssh2_parse_key-0.7.2/tests/data/build_data.sh` & `ssh2_parse_key-0.8.0/tests/data/build_data.sh`

 * *Files identical despite different names*

### Comparing `ssh2_parse_key-0.7.2/tests/data/test_key_dsa` & `ssh2_parse_key-0.8.0/tests/data/test_key_dsa`

 * *Files identical despite different names*

### Comparing `ssh2_parse_key-0.7.2/tests/data/test_key_dsa.pub` & `ssh2_parse_key-0.8.0/tests/data/test_key_dsa.pub`

 * *Files identical despite different names*

### Comparing `ssh2_parse_key-0.7.2/tests/data/test_key_dsa_rfc4716.pub` & `ssh2_parse_key-0.8.0/tests/data/test_key_dsa_rfc4716.pub`

 * *Files identical despite different names*

### Comparing `ssh2_parse_key-0.7.2/tests/data/test_key_rsa` & `ssh2_parse_key-0.8.0/tests/data/test_key_rsa`

 * *Files identical despite different names*

### Comparing `ssh2_parse_key-0.7.2/tests/data/test_key_rsa.pub` & `ssh2_parse_key-0.8.0/tests/data/test_key_rsa.pub`

 * *Files identical despite different names*

### Comparing `ssh2_parse_key-0.7.2/tests/data/test_key_rsa_rfc4716.pub` & `ssh2_parse_key-0.8.0/tests/data/test_key_rsa_rfc4716.pub`

 * *Files identical despite different names*

### Comparing `ssh2_parse_key-0.7.2/tests/test_convert_public_key.py` & `ssh2_parse_key-0.8.0/tests/test_convert_public_key.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,48 +1,51 @@
-#!/usr/bin/env python
-"""
-Tests for `ssh2_parse_key` package - convert keys.
+"""Tests for `ssh2_parse_key` package - convert keys.
 
 Loads keys in one format, converts to the other, and
 check if they are the same as the test data (which was
 generated using the openssh tools).
 """
+
+from pathlib import Path
+
 import pytest
 
 from ssh2_parse_key import Ssh2Key
 
 convert_pubkey_tests = [
     ("dsa", "ssh-dss"),
     ("ecdsa", "ecdsa-sha2-nistp256"),
     ("ed25519", "ssh-ed25519"),
     ("rsa", "ssh-rsa"),
 ]
 
 
-@pytest.mark.parametrize("format,encryption", convert_pubkey_tests)
-def test_convert_openssh_to_rfc4716(shared_datadir, format, encryption):
-    openssh_filename = f"test_key_{format}.pub"
+@pytest.mark.parametrize(("data_format", "encryption"), convert_pubkey_tests)
+def test_convert_openssh_to_rfc4716(shared_datadir: Path, data_format: str, encryption: str) -> None:  # noqa: ARG001
+    """Test the conversion from openssh -> rfc4716."""
+    openssh_filename = f"test_key_{data_format}.pub"
     openssh_contents = (shared_datadir / openssh_filename).read_text()
     openssh_pubkey = Ssh2Key.parse(openssh_contents)[0]
-    rfc4716_filename = f"test_key_{format}_rfc4716.pub"
+    rfc4716_filename = f"test_key_{data_format}_rfc4716.pub"
     rfc4716_contents = (shared_datadir / rfc4716_filename).read_text()
     rfc4716_pubkey = Ssh2Key.parse(rfc4716_contents)[0]
     # force the comments to be the same
     rfc4716_pubkey.headers["Comment"] = openssh_pubkey.comment()
     #
     # check the generated openssh version matches the loaded one
     assert rfc4716_pubkey.openssh() == openssh_contents
 
 
-@pytest.mark.parametrize("format,encryption", convert_pubkey_tests)
-def test_convert_rfc4716_to_openssh(shared_datadir, format, encryption):
-    openssh_filename = f"test_key_{format}.pub"
+@pytest.mark.parametrize(("data_format", "encryption"), convert_pubkey_tests)
+def test_convert_rfc4716_to_openssh(shared_datadir: Path, data_format: str, encryption: str) -> None:  # noqa: ARG001
+    """Test the conversion from rfc4716 ->openssh."""
+    openssh_filename = f"test_key_{data_format}.pub"
     openssh_contents = (shared_datadir / openssh_filename).read_text()
     openssh_pubkey = Ssh2Key.parse(openssh_contents)[0]
-    rfc4716_filename = f"test_key_{format}_rfc4716.pub"
+    rfc4716_filename = f"test_key_{data_format}_rfc4716.pub"
     rfc4716_contents = (shared_datadir / rfc4716_filename).read_text()
     rfc4716_pubkey = Ssh2Key.parse(rfc4716_contents)[0]
     # force the comments to be the same
     openssh_pubkey.headers["Comment"] = rfc4716_pubkey.comment()
     #
     # check the generated openssh version matches the loaded one
     assert openssh_pubkey.secsh() == rfc4716_contents
```

### Comparing `ssh2_parse_key-0.7.2/tests/test_load_keys_with_comments.py` & `ssh2_parse_key-0.8.0/tests/test_load_keys_with_comments.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,39 @@
-#!/usr/bin/env python
-"""
-Tests for `ssh2_parse_key` package - load keys with comments.
+"""Tests for `ssh2_parse_key` package - load keys with comments.
 
 Uses a test from the multiple keys tests but puts # comment
 lines in between the keys to see if that breaks things.
 """
+
+from pathlib import Path
+
 import pytest  # noqa: F401
 
 from ssh2_parse_key import Ssh2Key
 
 multiple_key_tests = [
     "dsa",
     "ecdsa",
     "ed25519",
     "rsa",
 ]
 
 
-def test_load_multiple_mixed_pubkey_key(shared_datadir):
+def test_load_multiple_mixed_pubkey_key(shared_datadir: Path) -> None:
+    """Test a mix of public keys."""
     key_contents = []
-    for format in multiple_key_tests:
-        openssh_filename = f"test_key_{format}.pub"
+    for data_format in multiple_key_tests:
+        openssh_filename = f"test_key_{data_format}.pub"
         openssh_contents = (shared_datadir / openssh_filename).read_text()
         key_contents.append(openssh_contents)
-        rfc4716_filename = f"test_key_{format}.pub"
+        rfc4716_filename = f"test_key_{data_format}.pub"
         rfc4716_contents = (shared_datadir / rfc4716_filename).read_text()
         key_contents.append(rfc4716_contents)
     all_keys = "\n# comment\n".join(key_contents)
-    print(all_keys)
+    # print(all_keys)
     keys = Ssh2Key.parse(all_keys)
     assert len(keys) == len(multiple_key_tests) * 2
     for key in keys:
         assert isinstance(key, Ssh2Key)
 
 
 # end
```

### Comparing `ssh2_parse_key-0.7.2/tests/test_load_multiple_short.py` & `ssh2_parse_key-0.8.0/tests/test_load_multiple_short.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-#!/usr/bin/env python
 """Tests for `ssh2_parse_key` package - loading multiple short keys."""
+
 import pytest  # noqa: F401
 
 from ssh2_parse_key import Ssh2Key
 
 
-def test_load_inline():
+def test_load_inline() -> None:
     """This exposed a bug in the parser previously"""
     key_contents = (
         "---- BEGIN SSH2 PUBLIC KEY ----\n"
         "Comment: my-key@example.org\n"
         "AAAAC3NzaC1lZDI1NTE5AAAAIHV8K5j1UNZSmAl4Xq7Yp8Qe1nN74B5NA7UyZDvz0H4M\n"
         "---- END SSH2 PUBLIC KEY ----\n"
         "---- BEGIN SSH2 PUBLIC KEY ----\n"
         "Comment: my-key@example.org\n"
         "AAAAC3NzaC1lZDI1NTE5AAAAIHV8K5j1UNZSmAl4Xq7Yp8Qe1nN74B5NA7UyZDvz0H4M\n"
         "---- END SSH2 PUBLIC KEY ----\n"
     )
     keys = Ssh2Key.parse(key_contents)
-    assert len(keys) == 2
+    assert len(keys) == 2  # noqa: PLR2004
```

### Comparing `ssh2_parse_key-0.7.2/tests/test_no_valid_keys.py` & `ssh2_parse_key-0.8.0/tests/test_no_valid_keys.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-#!/usr/bin/env python
-"""
-Tests for `ssh2_parse_key` package - load keys with comments.
+"""Tests for `ssh2_parse_key` package - load keys with comments.
 
 Uses a test from the multiple keys tests but puts # comment
 lines in between the keys to see if that breaks things.
 """
-import pytest  # noqa: F401
+
+import pytest
 
 from ssh2_parse_key import Ssh2Key
 
 invalid_key_tests = [
     "",  # empty
     "\n\n\n\n\n",  # only blank lines
     "\n# comment\n#comment\n\n\n",  # only comment lines
 ]
 
 
-def test_load_no_valid_key_key():
+def test_load_no_valid_key_key() -> None:
+    """Test what happens if keys are invalid."""
     for content in invalid_key_tests:
-        with pytest.raises(ValueError):
+        with pytest.raises(ValueError):  # noqa: PT011
             keys = Ssh2Key.parse(content)  # noqa: F841
 
 
 # end
```

### Comparing `ssh2_parse_key-0.7.2/tests/test_openssh_public_key_load.py` & `ssh2_parse_key-0.8.0/tests/test_openssh_public_key_load.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,57 +1,62 @@
-#!/usr/bin/env python
 """Tests for `ssh2_parse_key` package - loading openssh keys."""
+
+from pathlib import Path
+
 import pytest
 
 from ssh2_parse_key import Ssh2Key
 
 openssh_pubkey_tests = [
     ("dsa", "ssh-dss", "Test ssh key in dsa format"),
     ("ecdsa", "ecdsa-sha2-nistp256", "Test ssh key in ecdsa format"),
     ("ed25519", "ssh-ed25519", "Test ssh key in ed25519 format"),
     ("rsa", "ssh-rsa", "Test ssh key in rsa format"),
 ]
 
 
-@pytest.mark.parametrize("format,encryption,comment", openssh_pubkey_tests)
-def test_openssh_public_key_load(shared_datadir, format, encryption, comment):
-    filename = f"test_key_{format}.pub"
+@pytest.mark.parametrize(("data_format", "encryption", "comment"), openssh_pubkey_tests)
+def test_openssh_public_key_load(shared_datadir: Path, data_format: str, encryption: str, comment: str) -> None:
+    """Test openssh public key loading."""
+    filename = f"test_key_{data_format}.pub"
     contents = (shared_datadir / filename).read_text()
     pubkeys = Ssh2Key.parse(contents)
     pubkey = pubkeys[0]
     assert len(pubkeys) == 1
     assert pubkey.encryption == encryption
-    assert pubkey.type == "public"
+    assert pubkey.key_type == "public"
     assert pubkey.comment() == comment
-    assert len(pubkey.key) > 65
+    assert len(pubkey.key) > 65  # noqa: PLR2004
     #
     # check the key round trips OK (will break if any additional crap in file)
     assert contents == pubkey.openssh()
 
 
-@pytest.mark.parametrize("format,encryption,comment", openssh_pubkey_tests)
-def test_openssh_public_key_file(shared_datadir, format, encryption, comment):
-    filename = f"test_key_{format}.pub"
+@pytest.mark.parametrize(("data_format", "encryption", "comment"), openssh_pubkey_tests)
+def test_openssh_public_key_file(shared_datadir: Path, data_format: str, encryption: str, comment: str) -> None:
+    """Test openssh public key parsing."""
+    filename = f"test_key_{data_format}.pub"
     pubkeys = Ssh2Key.parse_file(shared_datadir / filename)
     pubkey = pubkeys[0]
     assert len(pubkeys) == 1
     assert pubkey.encryption == encryption
-    assert pubkey.type == "public"
+    assert pubkey.key_type == "public"
     assert pubkey.comment() == comment
-    assert len(pubkey.key) > 65
+    assert len(pubkey.key) > 65  # noqa: PLR2004
 
 
-@pytest.mark.parametrize("format,encryption,comment", openssh_pubkey_tests)
+@pytest.mark.parametrize(("data_format", "encryption", "comment"), openssh_pubkey_tests)
 def test_openssh_public_key_compare_load_file(
-    shared_datadir,
-    format,
-    encryption,
-    comment,
-):
-    filename = f"test_key_{format}.pub"
+    shared_datadir: Path,
+    data_format: str,
+    encryption: str,  # noqa: ARG001
+    comment: str,  # noqa: ARG001
+) -> None:
+    """Test file loading is correct."""
+    filename = f"test_key_{data_format}.pub"
     contents = (shared_datadir / filename).read_text()
     pubkey = Ssh2Key.parse(contents)[0]
     fpubkey = Ssh2Key.parse_file(shared_datadir / filename)[0]
     assert pubkey == fpubkey
 
 
 # end
```

### Comparing `ssh2_parse_key-0.7.2/tests/test_rfc4716_public_key_load.py` & `ssh2_parse_key-0.8.0/tests/test_rfc4716_public_key_load.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,11 @@
-#!/usr/bin/env python
 """Tests for `ssh2_parse_key` package - loading RFC4716 keys."""
+
+from pathlib import Path
+
 import pytest
 
 from ssh2_parse_key import Ssh2Key
 
 rfc4716_pubkey_tests = [
     # The comment fields get mangled by the openssh ssh-keygen conversion function
     (
@@ -25,51 +27,54 @@
         "rsa",
         "ssh-rsa",
         '"3072-bit RSA, converted by someone@keytests.example.org fro"',
     ),
 ]
 
 
-@pytest.mark.parametrize("format,encryption,comment", rfc4716_pubkey_tests)
-def test_rfc4716_public_key_load(shared_datadir, format, encryption, comment):
-    filename = f"test_key_{format}_rfc4716.pub"
+@pytest.mark.parametrize(("data_format", "encryption", "comment"), rfc4716_pubkey_tests)
+def test_rfc4716_public_key_load(shared_datadir: Path, data_format: str, encryption: str, comment: str) -> None:
+    """Test with rfc4716 public key."""
+    filename = f"test_key_{data_format}_rfc4716.pub"
     contents = (shared_datadir / filename).read_text()
     pubkeys = Ssh2Key.parse(contents)
     pubkey = pubkeys[0]
     assert len(pubkeys) == 1
     assert pubkey.encryption == encryption
-    assert pubkey.type == "public"
+    assert pubkey.key_type == "public"
     assert pubkey.comment() == comment
-    assert len(pubkey.key) > 65
+    assert len(pubkey.key) > 65  # noqa: PLR2004
     #
     # check the key round trips OK (will break if any additional crap in file)
     assert contents == pubkey.secsh()
     assert contents == pubkey.rfc4716()
 
 
-@pytest.mark.parametrize("format,encryption,comment", rfc4716_pubkey_tests)
-def test_rfc4716_public_key_file(shared_datadir, format, encryption, comment):
-    filename = f"test_key_{format}_rfc4716.pub"
+@pytest.mark.parametrize(("data_format", "encryption", "comment"), rfc4716_pubkey_tests)
+def test_rfc4716_public_key_file(shared_datadir: Path, data_format: str, encryption: str, comment: str) -> None:
+    """Test with rfc4716 public key."""
+    filename = f"test_key_{data_format}_rfc4716.pub"
     pubkeys = Ssh2Key.parse_file(shared_datadir / filename)
     pubkey = pubkeys[0]
     assert len(pubkeys) == 1
     assert pubkey.encryption == encryption
-    assert pubkey.type == "public"
+    assert pubkey.key_type == "public"
     assert pubkey.comment() == comment
-    assert len(pubkey.key) > 65
+    assert len(pubkey.key) > 65  # noqa: PLR2004
 
 
-@pytest.mark.parametrize("format,encryption,comment", rfc4716_pubkey_tests)
+@pytest.mark.parametrize(("data_format", "encryption", "comment"), rfc4716_pubkey_tests)
 def test_rfc4716_public_key_compare_load_file(
-    shared_datadir,
-    format,
-    encryption,
-    comment,
-):
-    filename = f"test_key_{format}_rfc4716.pub"
+    shared_datadir: Path,
+    data_format: str,
+    encryption: str,  # noqa: ARG001
+    comment: str,  # noqa: ARG001
+) -> None:
+    """Test with rfc4716 public key."""
+    filename = f"test_key_{data_format}_rfc4716.pub"
     contents = (shared_datadir / filename).read_text()
     pubkey = Ssh2Key.parse(contents)[0]
     fpubkey = Ssh2Key.parse_file(shared_datadir / filename)[0]
     assert pubkey == fpubkey
 
 
 # end
```

### Comparing `ssh2_parse_key-0.7.2/setup.py` & `ssh2_parse_key-0.8.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,108 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: ssh2_parse_key
+Version: 0.8.0
+Summary: Parses ssh2 keys and converts to multiple formats.
+Home-page: https://pypi.org/project/ssh2-parse-key/
+License: MIT
+Author: Nigel Metheringham
+Author-email: nigelm@cpan.org
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: BSD License
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: attrs (>=20.2.0)
+Project-URL: Documentation, https://nigelm.github.io/ssh2_parse_key/
+Project-URL: Repository, https://github.com/nigelm/ssh2_parse_key
+Description-Content-Type: text/markdown
+
+# ssh2_parse_key
+
+[![ci](https://img.shields.io/travis/com/nigelm/ssh2_parse_key.svg)](https://travis-ci.com/nigelm/ssh2_parse_key)
+[![documentation](https://img.shields.io/badge/docs-mkdocs%20material-blue.svg?style=flat)](https://nigelm.github.io/ssh2_parse_key/)
+[![pypi version](https://img.shields.io/pypi/v/ssh2_parse_key.svg)](https://pypi.python.org/pypi/ssh2_parse_key)
+
+Parses ssh2 public keys in either openssh or RFC4716/Secsh formats and converts
+to either format.
+
+At this point any attempt to work with private keys will raise an exception.
+
+---
+
+## Features
+
+-   Reads public keys of the following encryption types:-
+    -   `ssh-rsa`
+    -   `ssh-dss`
+    -   `ecdsa-sha2-nistp256`
+    -   `ssh-ed25519`
+-   Reads either Openssh or RFC4716 format public keys
+-   Can read input sets with either or both formats in
+-   Can output either format for any key
+
+---
+
+## Installation
+
+With `pip`:
+
+```bash
+python3.6 -m pip install ssh2_parse_key
+```
+
+---
+
+## Usage
+
+To use SSH2 Key Parsing in a project
+
+```python
+from ssh2_parse_key import Ssh2Key
+
+# although you can create the object from internal data the normal method
+# would be to use the parse() or parse_file() which return a list of Ssh2Key objects.
+# Ssh2Key objects are immutable.
+# Load one or more keys in either openssh or RFC4716 from a file
+keys = Ssh2Key.parse_file("/path/to/public_key")
+
+# alternatively
+data = Path("/path/to/public_key").read_text()
+keys = Ssh2Key.parse(data)
+
+# now those keys can be dealt with...
+for public_key in keys:
+    print(f"This is a {key.key_type} key")
+    print(f"It uses {key.encryption} encryption")
+    print(f"comment = {key.comment}")
+    print(f"subject = {key.subject}")
+
+    print("RFC4716 format representation")
+    print(key.rfc4716())
+
+    print("OpenSSH representation")
+    print(key.openssh())
+```
+
+---
+
+## Credits
+
+The package is strongly based on the perl
+[`Parse::SSH2::PublicKey`](https://metacpan.org/pod/Parse::SSH2::PublicKey)
+module.
 
-packages = \
-['ssh2_parse_key']
+Development on the python version was done by
+[`Nigel Metheringham <nigelm@cpan.org>`](https://github.com/nigelm/)
 
-package_data = \
-{'': ['*']}
+---
 
-install_requires = \
-['attrs>=20.2.0,<21.0.0']
-
-setup_kwargs = {
-    'name': 'ssh2-parse-key',
-    'version': '0.7.2',
-    'description': 'Parses ssh2 keys and converts to multiple formats.',
-    'long_description': '# ssh2_parse_key\n\n[![ci](https://img.shields.io/travis/nigelm/ssh2_parse_key.svg)](https://travis-ci.com/nigelm/ssh2_parse_key)\n[![documentation](https://img.shields.io/badge/docs-mkdocs%20material-blue.svg?style=flat)](https://nigelm.github.io/ssh2_parse_key/)\n[![pypi version](https://img.shields.io/pypi/v/ssh2_parse_key.svg)](https://pypi.python.org/pypi/ssh2_parse_key)\n\nParses ssh2 public keys in either openssh or RFC4716/Secsh formats and\nconverts to either format.\n\nAt this point any attempt to work with private keys will raise an exception.\n\n----\n\n## Features\n\n- Reads public keys of the following encryption types:-\n    - `ssh-rsa`\n    - `ssh-dss`\n    - `ecdsa-sha2-nistp256`\n    - `ssh-ed25519`\n- Reads either Openssh or RFC4716 format public keys\n- Can read input sets with either or both formats in\n- Can output either format for any key\n\n----\n\n## Installation\n\nWith `pip`:\n```bash\npython3.6 -m pip install ssh2_parse_key\n```\n\n----\n\n## Usage\n\nTo use SSH2 Key Parsing in a project\n\n```python\nfrom ssh2_parse_key import Ssh2Key\n\n# although you can create the object from internal data the normal method\n# would be to use the parse() or parse_file() which return a list of Ssh2Key objects.\n# Ssh2Key objects are immutable.\n# Load one or more keys in either openssh or RFC4716 from a file\nkeys = Ssh2Key.parse_file("/path/to/public_key")\n\n# alternatively\ndata = Path("/path/to/public_key").read_text()\nkeys = Ssh2Key.parse(data)\n\n# now those keys can be dealt with...\nfor public_key in keys:\n    print(f"This is a {key.type} key")\n    print(f"It uses {key.encryption} encryption")\n    print(f"comment = {key.comment}")\n    print(f"subject = {key.subject}")\n\n    print("RFC4716 format representation")\n    print(key.rfc4716())\n\n    print("OpenSSH representation")\n    print(key.openssh())\n```\n\n----\n\n## Credits\n\nThe package is strongly based on the perl [`Parse::SSH2::PublicKey`](https://metacpan.org/pod/Parse::SSH2::PublicKey) module.\n\nDevelopment on the python version was done by [`Nigel Metheringham <nigelm@cpan.org>`](https://github.com/nigelm/)\n\n----\n',
-    'author': 'Nigel Metheringham',
-    'author_email': 'nigelm@cpan.org',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://pypi.org/project/ssh2-parse-key/',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.6,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

