# Comparing `tmp/vinted_scraper-2.2.0.tar.gz` & `tmp/vinted_scraper-2.2.1.tar.gz`

## Comparing `vinted_scraper-2.2.0.tar` & `vinted_scraper-2.2.1.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 vinted_scraper-2.2.0/.gitmodules
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 vinted_scraper-2.2.0/Makefile
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 vinted_scraper-2.2.0/requirements.txt
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 vinted_scraper-2.2.0/.github/dependabot.yml
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 vinted_scraper-2.2.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 vinted_scraper-2.2.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 vinted_scraper-2.2.0/.github/workflows/coverage.yml
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 vinted_scraper-2.2.0/.github/workflows/linter.yml
--rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 vinted_scraper-2.2.0/.github/workflows/release.yml
--rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 vinted_scraper-2.2.0/.github/workflows/test.yml
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 vinted_scraper-2.2.0/.github/workflows/update-reminder.yml
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 vinted_scraper-2.2.0/.github/workflows/update-user-agents.yml
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 vinted_scraper-2.2.0/build-tools/.git
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 vinted_scraper-2.2.0/build-tools/.gitignore
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 vinted_scraper-2.2.0/build-tools/LICENSE
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 vinted_scraper-2.2.0/build-tools/Makefile
--rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 vinted_scraper-2.2.0/build-tools/README.md
--rw-r--r--   0        0        0     2636 2020-02-02 00:00:00.000000 vinted_scraper-2.2.0/build-tools/common.mk
--rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 vinted_scraper-2.2.0/build-tools/common_linters.mk
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 vinted_scraper-2.2.0/build-tools/git.mk
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 vinted_scraper-2.2.0/build-tools/smtp.mk
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 vinted_scraper-2.2.0/build-tools/.github/dependabot.yml
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 vinted_scraper-2.2.0/build-tools/.github/workflows/linter.yml
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 vinted_scraper-2.2.0/build-tools/.github/workflows/update-reminder.yml
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 vinted_scraper-2.2.0/build-tools/image/README.md
--rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 vinted_scraper-2.2.0/build-tools/image/docker.mk
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 vinted_scraper-2.2.0/build-tools/python/.dockerignore
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 vinted_scraper-2.2.0/build-tools/python/Dockerfile
--rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 vinted_scraper-2.2.0/build-tools/python/README.md
--rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 vinted_scraper-2.2.0/build-tools/python/python.mk
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 vinted_scraper-2.2.0/build-tools/python/requirements.txt
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 vinted_scraper-2.2.0/build-tools/python/hooks/pre-commit.bash
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 vinted_scraper-2.2.0/build-tools/python/test/Dockerfile
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 vinted_scraper-2.2.0/build-tools/python/test/__init__.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 vinted_scraper-2.2.0/src/vinted_scraper/__init__.py
--rw-r--r--   0        0        0     5478 2020-02-02 00:00:00.000000 vinted_scraper-2.2.0/src/vinted_scraper/agents.json
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 vinted_scraper-2.2.0/src/vinted_scraper/utils.py
--rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 vinted_scraper-2.2.0/src/vinted_scraper/vintedScraper.py
--rw-r--r--   0        0        0     5884 2020-02-02 00:00:00.000000 vinted_scraper-2.2.0/src/vinted_scraper/vintedWrapper.py
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 vinted_scraper-2.2.0/src/vinted_scraper/models/__init__.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 vinted_scraper-2.2.0/src/vinted_scraper/models/vintedBrand.py
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 vinted_scraper-2.2.0/src/vinted_scraper/models/vintedBundleDiscount.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 vinted_scraper-2.2.0/src/vinted_scraper/models/vintedHighResolution.py
--rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 vinted_scraper-2.2.0/src/vinted_scraper/models/vintedImage.py
--rw-r--r--   0        0        0     7074 2020-02-02 00:00:00.000000 vinted_scraper-2.2.0/src/vinted_scraper/models/vintedItem.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 vinted_scraper-2.2.0/src/vinted_scraper/models/vintedMedia.py
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 vinted_scraper-2.2.0/src/vinted_scraper/models/vintedPaymentMethod.py
--rw-r--r--   0        0        0     4399 2020-02-02 00:00:00.000000 vinted_scraper-2.2.0/src/vinted_scraper/models/vintedUser.py
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 vinted_scraper-2.2.0/tests/__init__.py
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 vinted_scraper-2.2.0/tests/test_models.py
--rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 vinted_scraper-2.2.0/tests/test_quickstart.py
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 vinted_scraper-2.2.0/tests/test_utils.py
--rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 vinted_scraper-2.2.0/tests/test_vinted.py
--rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 vinted_scraper-2.2.0/tests/test_vinted_item.py
--rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 vinted_scraper-2.2.0/tests/test_vinted_search.py
--rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 vinted_scraper-2.2.0/tests/utils.py
--rw-r--r--   0        0        0    13533 2020-02-02 00:00:00.000000 vinted_scraper-2.2.0/tests/samples/item_dummy.json
--rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 vinted_scraper-2.2.0/tests/samples/search_item_dummy.json
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 vinted_scraper-2.2.0/.gitignore
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 vinted_scraper-2.2.0/LICENSE
--rw-r--r--   0        0        0     3964 2020-02-02 00:00:00.000000 vinted_scraper-2.2.0/README.md
--rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 vinted_scraper-2.2.0/pyproject.toml
--rw-r--r--   0        0        0     6479 2020-02-02 00:00:00.000000 vinted_scraper-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/.gitmodules
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/Makefile
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/requirements.txt
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/.github/dependabot.yml
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/.github/workflows/coverage.yml
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/.github/workflows/linter.yml
+-rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/.github/workflows/release.yml
+-rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/.github/workflows/test.yml
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/.github/workflows/update-reminder.yml
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/.github/workflows/update-user-agents.yml
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/build-tools/.git
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/build-tools/.gitignore
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/build-tools/LICENSE
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/build-tools/Makefile
+-rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/build-tools/README.md
+-rw-r--r--   0        0        0     2636 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/build-tools/common.mk
+-rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/build-tools/common_linters.mk
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/build-tools/git.mk
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/build-tools/smtp.mk
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/build-tools/.github/dependabot.yml
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/build-tools/.github/workflows/linter.yml
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/build-tools/.github/workflows/update-reminder.yml
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/build-tools/image/README.md
+-rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/build-tools/image/docker.mk
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/build-tools/python/.dockerignore
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/build-tools/python/Dockerfile
+-rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/build-tools/python/README.md
+-rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/build-tools/python/python.mk
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/build-tools/python/requirements.txt
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/build-tools/python/hooks/pre-commit.bash
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/build-tools/python/test/Dockerfile
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/build-tools/python/test/__init__.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/src/vinted_scraper/__init__.py
+-rw-r--r--   0        0        0     3552 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/src/vinted_scraper/agents.json
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/src/vinted_scraper/utils.py
+-rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/src/vinted_scraper/vintedScraper.py
+-rw-r--r--   0        0        0     5884 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/src/vinted_scraper/vintedWrapper.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/src/vinted_scraper/models/__init__.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/src/vinted_scraper/models/vintedBrand.py
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/src/vinted_scraper/models/vintedBundleDiscount.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/src/vinted_scraper/models/vintedHighResolution.py
+-rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/src/vinted_scraper/models/vintedImage.py
+-rw-r--r--   0        0        0     7074 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/src/vinted_scraper/models/vintedItem.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/src/vinted_scraper/models/vintedMedia.py
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/src/vinted_scraper/models/vintedPaymentMethod.py
+-rw-r--r--   0        0        0     4399 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/src/vinted_scraper/models/vintedUser.py
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/tests/__init__.py
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/tests/test_models.py
+-rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/tests/test_quickstart.py
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/tests/test_utils.py
+-rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/tests/test_vinted.py
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/tests/test_vinted_item.py
+-rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/tests/test_vinted_search.py
+-rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/tests/utils.py
+-rw-r--r--   0        0        0    13533 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/tests/samples/item_dummy.json
+-rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/tests/samples/search_item_dummy.json
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/.gitignore
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/LICENSE
+-rw-r--r--   0        0        0     3964 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/README.md
+-rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/pyproject.toml
+-rw-r--r--   0        0        0     6479 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/PKG-INFO
```

### Comparing `vinted_scraper-2.2.0/Makefile` & `vinted_scraper-2.2.1/Makefile`

 * *Files identical despite different names*

### Comparing `vinted_scraper-2.2.0/.github/ISSUE_TEMPLATE/bug_report.md` & `vinted_scraper-2.2.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `vinted_scraper-2.2.0/.github/workflows/coverage.yml` & `vinted_scraper-2.2.1/.github/workflows/coverage.yml`

 * *Files 1% similar despite different names*

```diff
@@ -27,10 +27,10 @@
       - name: Install dependencies
         run: make py.update
 
       - name: Run Coverage
         run: make coverage
 
       - name: Upload coverage reports to Codecov
-        uses: codecov/codecov-action@v3
+        uses: codecov/codecov-action@v4
         env:
           CODECOV_TOKEN: ${{ secrets.CODECOV_TOKEN }}
```

### Comparing `vinted_scraper-2.2.0/.github/workflows/linter.yml` & `vinted_scraper-2.2.1/.github/workflows/linter.yml`

 * *Files identical despite different names*

### Comparing `vinted_scraper-2.2.0/.github/workflows/release.yml` & `vinted_scraper-2.2.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `vinted_scraper-2.2.0/.github/workflows/test.yml` & `vinted_scraper-2.2.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `vinted_scraper-2.2.0/.github/workflows/update-reminder.yml` & `vinted_scraper-2.2.1/.github/workflows/update-reminder.yml`

 * *Files identical despite different names*

### Comparing `vinted_scraper-2.2.0/build-tools/LICENSE` & `vinted_scraper-2.2.1/build-tools/LICENSE`

 * *Files identical despite different names*

### Comparing `vinted_scraper-2.2.0/build-tools/README.md` & `vinted_scraper-2.2.1/build-tools/README.md`

 * *Files identical despite different names*

### Comparing `vinted_scraper-2.2.0/build-tools/common.mk` & `vinted_scraper-2.2.1/build-tools/common.mk`

 * *Files identical despite different names*

### Comparing `vinted_scraper-2.2.0/build-tools/common_linters.mk` & `vinted_scraper-2.2.1/build-tools/common_linters.mk`

 * *Files identical despite different names*

### Comparing `vinted_scraper-2.2.0/build-tools/git.mk` & `vinted_scraper-2.2.1/build-tools/git.mk`

 * *Files identical despite different names*

### Comparing `vinted_scraper-2.2.0/build-tools/.github/workflows/linter.yml` & `vinted_scraper-2.2.1/build-tools/.github/workflows/linter.yml`

 * *Files identical despite different names*

### Comparing `vinted_scraper-2.2.0/build-tools/.github/workflows/update-reminder.yml` & `vinted_scraper-2.2.1/build-tools/.github/workflows/update-reminder.yml`

 * *Files identical despite different names*

### Comparing `vinted_scraper-2.2.0/build-tools/image/docker.mk` & `vinted_scraper-2.2.1/build-tools/image/docker.mk`

 * *Files identical despite different names*

### Comparing `vinted_scraper-2.2.0/build-tools/python/Dockerfile` & `vinted_scraper-2.2.1/build-tools/python/Dockerfile`

 * *Files identical despite different names*

### Comparing `vinted_scraper-2.2.0/build-tools/python/README.md` & `vinted_scraper-2.2.1/build-tools/python/README.md`

 * *Files identical despite different names*

### Comparing `vinted_scraper-2.2.0/build-tools/python/python.mk` & `vinted_scraper-2.2.1/build-tools/python/python.mk`

 * *Files identical despite different names*

### Comparing `vinted_scraper-2.2.0/src/vinted_scraper/agents.json` & `vinted_scraper-2.2.1/src/vinted_scraper/agents.json`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.3235294117647059%*

 * *Differences: {'0': "{'ua': 'Mozilla/5.0 (Linux; Android 10; K) AppleWebKit/537.36 (KHTML, like Gecko) "*

 * *      "Chrome/123.0.0.0 Mobile Safari/537.3', 'pct': 32.05}",*

 * * '1': "{'ua': 'Mozilla/5.0 (Linux; Android 10; K) AppleWebKit/537.36 (KHTML, like Gecko) "*

 * *      "Chrome/122.0.0.0 Mobile Safari/537.3', 'pct': 26.92}",*

 * * '10': "{'ua': 'Mozilla/5.0 (iPhone; CPU iPhone OS 17_1_2 like Mac OS X) AppleWebKit/605.1.15 "*

 * *       "(KHTML, like Gecko) Version/17.1.2 Mobile/15E148 Safari/604.', 'pct': 1.28}",*

 * * '11': "{'ua': 'Mozilla/ […]*

```diff
@@ -1,138 +1,90 @@
 [
     {
-        "pct": 42.78,
-        "ua": "Mozilla/5.0 (Linux; Android 10; K) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/120.0.0.0 Mobile Safari/537.3"
-    },
-    {
-        "pct": 20.62,
-        "ua": "Mozilla/5.0 (iPhone; CPU iPhone OS 17_1_2 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/17.1.2 Mobile/15E148 Safari/604."
-    },
-    {
-        "pct": 6.19,
-        "ua": "Mozilla/5.0 (iPhone; CPU iPhone OS 17_2_1 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/17.2 Mobile/15E148 Safari/604."
-    },
-    {
-        "pct": 4.12,
-        "ua": "Mozilla/5.0 (Linux; Android 9; JAT-L41) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/84.0.4147.125 Mobile Safari/537.3"
-    },
-    {
-        "pct": 2.06,
-        "ua": "Mozilla/5.0 (iPhone; CPU iPhone OS 16_6_1 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/16.6 Mobile/15E148 Safari/604."
-    },
-    {
-        "pct": 2.06,
-        "ua": "Mozilla/5.0 (iPhone; CPU iPhone OS 12_5_7 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/12.1.2 Mobile/15E148 Safari/604."
-    },
-    {
-        "pct": 2.06,
-        "ua": "Mozilla/5.0 (iPhone; CPU iPhone OS 16_7 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) CriOS/120.0.6099.119 Mobile/15E148 Safari/604."
-    },
-    {
-        "pct": 2.06,
-        "ua": "Mozilla/5.0 (iPhone; CPU iPhone OS 16_7_1 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/16.6 Mobile/15E148 Safari/604."
+        "pct": 32.05,
+        "ua": "Mozilla/5.0 (Linux; Android 10; K) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/123.0.0.0 Mobile Safari/537.3"
     },
     {
-        "pct": 1.55,
-        "ua": "Mozilla/5.0 (iPhone; CPU iPhone OS 17_1 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) CriOS/120.0.6099.119 Mobile/15E148 Safari/604."
+        "pct": 26.92,
+        "ua": "Mozilla/5.0 (Linux; Android 10; K) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/122.0.0.0 Mobile Safari/537.3"
     },
     {
-        "pct": 1.03,
-        "ua": "Mozilla/5.0 (Linux; Android 8.0.0; WAS-LX1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/91.0.4472.164 Mobile Safari/537.3"
+        "pct": 10.26,
+        "ua": "Mozilla/5.0 (iPhone; CPU iPhone OS 17_3_1 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/17.3.1 Mobile/15E148 Safari/604."
     },
     {
-        "pct": 1.03,
-        "ua": "Mozilla/5.0 (Linux; Android 13; SAMSUNG SM-G990B2) AppleWebKit/537.36 (KHTML, like Gecko) SamsungBrowser/23.0 Chrome/115.0.0.0 Mobile Safari/537.3"
+        "pct": 3.85,
+        "ua": "Mozilla/5.0 (Linux; Android 10; K) AppleWebKit/537.36 (KHTML, like Gecko) SamsungBrowser/24.0 Chrome/117.0.0.0 Mobile Safari/537.3"
     },
     {
-        "pct": 1.03,
-        "ua": "Mozilla/5.0 (Linux; Android 13; SAMSUNG SM-G980F) AppleWebKit/537.36 (KHTML, like Gecko) SamsungBrowser/23.0 Chrome/115.0.0.0 Mobile Safari/537.3"
-    },
-    {
-        "pct": 1.03,
-        "ua": "Mozilla/5.0 (Linux; Android 12; SAMSUNG SM-A415F) AppleWebKit/537.36 (KHTML, like Gecko) SamsungBrowser/23.0 Chrome/115.0.0.0 Mobile Safari/537.3"
+        "pct": 2.56,
+        "ua": "Mozilla/5.0 (iPhone; CPU iPhone OS 12_1 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/12.0 Mobile/15E148 Safari/604."
     },
     {
-        "pct": 1.03,
-        "ua": "Mozilla/5.0 (Linux; Android 10; K) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/119.0.0.0 Mobile Safari/537.3"
-    },
-    {
-        "pct": 1.03,
-        "ua": "Mozilla/5.0 (iPhone; CPU iPhone OS 17_1 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) GSA/273.0.547966426 Mobile/15E148 Safari/604."
-    },
-    {
-        "pct": 1.03,
-        "ua": "Mozilla/5.0 (iPhone; CPU iPhone OS 17_1_1 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/17.1.1 Mobile/15E148 Safari/604."
-    },
-    {
-        "pct": 0.52,
-        "ua": "Mozilla/5.0 (Linux; Android 12; SAMSUNG SM-G975F) AppleWebKit/537.36 (KHTML, like Gecko) SamsungBrowser/23.0 Chrome/115.0.0.0 Mobile Safari/537.3"
-    },
-    {
-        "pct": 0.52,
-        "ua": "Mozilla/5.0 (Linux; Android 11; moto e20 Build/RONS31.267-94-14) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/120.0.6099.144 Mobile Safari/537.3"
+        "pct": 2.56,
+        "ua": "Mozilla/5.0 (iPhone; CPU iPhone OS 17_2_1 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/17.2 Mobile/15E148 Safari/604."
     },
     {
-        "pct": 0.52,
-        "ua": "Mozilla/5.0 (Linux; Android 14; SAMSUNG SM-A336B) AppleWebKit/537.36 (KHTML, like Gecko) SamsungBrowser/23.0 Chrome/115.0.0.0 Mobile Safari/537.3"
+        "pct": 2.56,
+        "ua": "Mozilla/5.0 (Linux; Android 10; K) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/120.0.0.0 Mobile Safari/537.3"
     },
     {
-        "pct": 0.52,
-        "ua": "Mozilla/5.0 (Linux; Android 11; SAMSUNG SM-A405FN) AppleWebKit/537.36 (KHTML, like Gecko) SamsungBrowser/23.0 Chrome/115.0.0.0 Mobile Safari/537.3"
+        "pct": 1.28,
+        "ua": "Mozilla/5.0 (iPhone; CPU iPhone OS 17_4 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) GSA/308.0.615969171 Mobile/15E148 Safari/604."
     },
     {
-        "pct": 0.52,
-        "ua": "Mozilla/5.0 (Linux; Android 10; MAR-LX1A; HMSCore 6.12.4.312; GMSCore 23.48.16) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/99.0.4844.88 HuaweiBrowser/14.0.2.311 Mobile Safari/537.3"
+        "pct": 1.28,
+        "ua": "Mozilla/5.0 (iPhone; CPU iPhone OS 15_8 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) CriOS/123.0.6312.52 Mobile/15E148 Safari/604."
     },
     {
-        "pct": 0.52,
-        "ua": "Mozilla/5.0 (Linux; Android 10; K) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/121.0.0.0 Mobile Safari/537.3"
+        "pct": 1.28,
+        "ua": "Mozilla/5.0 (iPhone; CPU iPhone OS 16_7 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) CriOS/123.0.6312.52 Mobile/15E148 Safari/604."
     },
     {
-        "pct": 0.52,
-        "ua": "Mozilla/5.0 (Linux; Android 10; K) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/114.0.0.0 Mobile Safari/537.3"
+        "pct": 1.28,
+        "ua": "Mozilla/5.0 (iPhone; CPU iPhone OS 17_1_2 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/17.1.2 Mobile/15E148 Safari/604."
     },
     {
-        "pct": 0.52,
-        "ua": "Mozilla/5.0 (Linux; Android 13; SAMSUNG SM-S901B) AppleWebKit/537.36 (KHTML, like Gecko) SamsungBrowser/23.0 Chrome/115.0.0.0 Mobile Safari/537.3"
+        "pct": 1.28,
+        "ua": "Mozilla/5.0 (Linux; Android 10; K) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/118.0.0.0 Mobile Safari/537.3"
     },
     {
-        "pct": 0.52,
-        "ua": "Mozilla/5.0 (Linux; Android 14; SAMSUNG SM-G990B) AppleWebKit/537.36 (KHTML, like Gecko) SamsungBrowser/23.0 Chrome/115.0.0.0 Mobile Safari/537.3"
+        "pct": 1.28,
+        "ua": "Mozilla/5.0 (Linux; Android 14; SAMSUNG SM-A546B) AppleWebKit/537.36 (KHTML, like Gecko) SamsungBrowser/23.0 Chrome/115.0.0.0 Mobile Safari/537.3"
     },
     {
-        "pct": 0.52,
-        "ua": "Mozilla/5.0 (Linux; Android 14; SAMSUNG SM-S911B) AppleWebKit/537.36 (KHTML, like Gecko) SamsungBrowser/23.0 Chrome/115.0.0.0 Mobile Safari/537.3"
+        "pct": 1.28,
+        "ua": "Mozilla/5.0 (Linux; Android 10; Redmi Note 7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/83.0.4103.106 Mobile Safari/537.3"
     },
     {
-        "pct": 0.52,
-        "ua": "Mozilla/5.0 (iPhone; CPU iPhone OS 15_8 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/15.6.6 Mobile/15E148 Safari/604."
+        "pct": 1.28,
+        "ua": "Mozilla/5.0 (Linux; Android 10; moto e(6i) Build/QOH30.280-26) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/122.0.6261.119 Mobile Safari/537.3"
     },
     {
-        "pct": 0.52,
-        "ua": "Mozilla/5.0 (iPhone; CPU iPhone OS 16_1 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/16.1 Mobile/15E148 Safari/604."
+        "pct": 1.28,
+        "ua": "Mozilla/5.0 (Linux; Android 11; SAMSUNG SM-A202F) AppleWebKit/537.36 (KHTML, like Gecko) SamsungBrowser/23.0 Chrome/115.0.0.0 Mobile Safari/537.3"
     },
     {
-        "pct": 0.52,
-        "ua": "Mozilla/5.0 (iPhone; CPU iPhone OS 16_2 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/16.2 Mobile/15E148 Safari/604."
+        "pct": 1.28,
+        "ua": "Mozilla/5.0 (Linux; Android 11; SAMSUNG SM-A705FN) AppleWebKit/537.36 (KHTML, like Gecko) SamsungBrowser/23.0 Chrome/115.0.0.0 Mobile Safari/537.3"
     },
     {
-        "pct": 0.52,
-        "ua": "Mozilla/5.0 (iPhone; CPU iPhone OS 16_6 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/16.6 Mobile/15E148 Safari/604."
+        "pct": 1.28,
+        "ua": "Mozilla/5.0 (Linux; Android 13; SAMSUNG SM-G980F) AppleWebKit/537.36 (KHTML, like Gecko) SamsungBrowser/23.0 Chrome/115.0.0.0 Mobile Safari/537.3"
     },
     {
-        "pct": 0.52,
-        "ua": "Mozilla/5.0 (iPhone; CPU iPhone OS 16_7 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) GSA/295.0.590048842 Mobile/15E148 Safari/604."
+        "pct": 1.28,
+        "ua": "Mozilla/5.0 (Linux; Android 7.0; SM-G930V Build/NRD90M) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/59.0.3071.125 Mobile Safari/537.36 (compatible; Google-Read-Aloud; +https://support.google.com/webmasters/answer/1061943"
     },
     {
-        "pct": 0.52,
-        "ua": "Mozilla/5.0 (iPhone; CPU iPhone OS 16_7_2 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/16.6 Mobile/15E148 Safari/604."
+        "pct": 1.28,
+        "ua": "Mozilla/5.0 (Linux; Android 9; SAMSUNG SM-J530F) AppleWebKit/537.36 (KHTML, like Gecko) SamsungBrowser/23.0 Chrome/115.0.0.0 Mobile Safari/537.3"
     },
     {
-        "pct": 0.52,
-        "ua": "Mozilla/5.0 (iPhone; CPU iPhone OS 17_0_2 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/17.0 Mobile/15E148 Safari/604."
+        "pct": 1.28,
+        "ua": "Mozilla/5.0 (Linux; Android 10; K) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/119.0.0.0 Mobile Safari/537.3"
     },
     {
-        "pct": 0.52,
-        "ua": "Mozilla/5.0 (Linux; Android 10; K) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/110.0.0.0 Mobile Safari/537.3"
+        "pct": 1.28,
+        "ua": "Mozilla/5.0 (iPhone; CPU iPhone OS 17_4 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/17.4 Mobile/15E148 Safari/604."
     }
 ]
```

### Comparing `vinted_scraper-2.2.0/src/vinted_scraper/vintedScraper.py` & `vinted_scraper-2.2.1/src/vinted_scraper/vintedScraper.py`

 * *Files identical despite different names*

### Comparing `vinted_scraper-2.2.0/src/vinted_scraper/vintedWrapper.py` & `vinted_scraper-2.2.1/src/vinted_scraper/vintedWrapper.py`

 * *Files identical despite different names*

### Comparing `vinted_scraper-2.2.0/src/vinted_scraper/models/__init__.py` & `vinted_scraper-2.2.1/src/vinted_scraper/models/__init__.py`

 * *Files identical despite different names*

### Comparing `vinted_scraper-2.2.0/src/vinted_scraper/models/vintedBrand.py` & `vinted_scraper-2.2.1/src/vinted_scraper/models/vintedBrand.py`

 * *Files identical despite different names*

### Comparing `vinted_scraper-2.2.0/src/vinted_scraper/models/vintedBundleDiscount.py` & `vinted_scraper-2.2.1/src/vinted_scraper/models/vintedBundleDiscount.py`

 * *Files identical despite different names*

### Comparing `vinted_scraper-2.2.0/src/vinted_scraper/models/vintedImage.py` & `vinted_scraper-2.2.1/src/vinted_scraper/models/vintedImage.py`

 * *Files identical despite different names*

### Comparing `vinted_scraper-2.2.0/src/vinted_scraper/models/vintedItem.py` & `vinted_scraper-2.2.1/src/vinted_scraper/models/vintedItem.py`

 * *Files identical despite different names*

### Comparing `vinted_scraper-2.2.0/src/vinted_scraper/models/vintedPaymentMethod.py` & `vinted_scraper-2.2.1/src/vinted_scraper/models/vintedPaymentMethod.py`

 * *Files identical despite different names*

### Comparing `vinted_scraper-2.2.0/src/vinted_scraper/models/vintedUser.py` & `vinted_scraper-2.2.1/src/vinted_scraper/models/vintedUser.py`

 * *Files identical despite different names*

### Comparing `vinted_scraper-2.2.0/tests/test_models.py` & `vinted_scraper-2.2.1/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `vinted_scraper-2.2.0/tests/test_quickstart.py` & `vinted_scraper-2.2.1/tests/test_quickstart.py`

 * *Files identical despite different names*

### Comparing `vinted_scraper-2.2.0/tests/test_vinted.py` & `vinted_scraper-2.2.1/tests/test_vinted.py`

 * *Files identical despite different names*

### Comparing `vinted_scraper-2.2.0/tests/test_vinted_item.py` & `vinted_scraper-2.2.1/tests/test_vinted_item.py`

 * *Files identical despite different names*

### Comparing `vinted_scraper-2.2.0/tests/test_vinted_search.py` & `vinted_scraper-2.2.1/tests/test_vinted_search.py`

 * *Files identical despite different names*

### Comparing `vinted_scraper-2.2.0/tests/utils.py` & `vinted_scraper-2.2.1/tests/utils.py`

 * *Files identical despite different names*

### Comparing `vinted_scraper-2.2.0/tests/samples/item_dummy.json` & `vinted_scraper-2.2.1/tests/samples/item_dummy.json`

 * *Files identical despite different names*

### Comparing `vinted_scraper-2.2.0/tests/samples/search_item_dummy.json` & `vinted_scraper-2.2.1/tests/samples/search_item_dummy.json`

 * *Files identical despite different names*

### Comparing `vinted_scraper-2.2.0/.gitignore` & `vinted_scraper-2.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `vinted_scraper-2.2.0/LICENSE` & `vinted_scraper-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vinted_scraper-2.2.0/README.md` & `vinted_scraper-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `vinted_scraper-2.2.0/pyproject.toml` & `vinted_scraper-2.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "vinted_scraper"
-version = "2.2.0"
+version = "2.2.1"
 description = "A very simple Python package that scrapes the Vinted website to retrieve information about its items."
 readme = "README.md"
 requires-python = ">= 3.6"
 license = { file = "LICENSE" }
 authors = [
     { name = "Giglium" }
 ]
```

### Comparing `vinted_scraper-2.2.0/PKG-INFO` & `vinted_scraper-2.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: vinted_scraper
-Version: 2.2.0
+Version: 2.2.1
 Summary: A very simple Python package that scrapes the Vinted website to retrieve information about its items.
 Project-URL: Changelog, https://github.com/Giglium/vinted_scraper/releases
 Project-URL: Documentation, https://github.com/Giglium/vinted_scraper
 Project-URL: Homepage, https://github.com/Giglium/vinted_scraper
 Project-URL: Issues, https://github.com/Giglium/vinted_scraper/issues
 Project-URL: Source, https://github.com/Giglium/vinted_scraper
 Author: Giglium
```

