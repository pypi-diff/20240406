# Comparing `tmp/libyang-2.8.4.tar.gz` & `tmp/libyang-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libyang-2.8.4.tar", last modified: Wed Feb  7 13:05:08 2024, max compression
+gzip compressed data, was "libyang-3.0.0.tar", last modified: Sat Apr  6 10:11:49 2024, max compression
```

## Comparing `libyang-2.8.4.tar` & `libyang-3.0.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 13:05:08.418774 libyang-2.8.4/
--rw-r--r--   0 root         (0) root         (0)     1073 2024-02-07 13:04:52.000000 libyang-2.8.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)      205 2024-02-07 13:04:52.000000 libyang-2.8.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     9399 2024-02-07 13:05:08.418774 libyang-2.8.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8756 2024-02-07 13:04:52.000000 libyang-2.8.4/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 13:05:08.414774 libyang-2.8.4/cffi/
--rw-r--r--   0 root         (0) root         (0)     1142 2024-02-07 13:04:52.000000 libyang-2.8.4/cffi/build.py
--rw-r--r--   0 root         (0) root         (0)    28831 2024-02-07 13:04:52.000000 libyang-2.8.4/cffi/cdefs.h
--rw-r--r--   0 root         (0) root         (0)      314 2024-02-07 13:04:52.000000 libyang-2.8.4/cffi/source.c
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 13:05:08.422774 libyang-2.8.4/libyang/
--rw-r--r--   0 root         (0) root         (0)        6 2024-02-07 13:05:08.422774 libyang-2.8.4/libyang/VERSION
--rw-r--r--   0 root         (0) root         (0)     3314 2024-02-07 13:04:52.000000 libyang-2.8.4/libyang/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15052 2024-02-07 13:04:52.000000 libyang-2.8.4/libyang/context.py
--rw-r--r--   0 root         (0) root         (0)    45383 2024-02-07 13:04:52.000000 libyang-2.8.4/libyang/data.py
--rw-r--r--   0 root         (0) root         (0)    13430 2024-02-07 13:04:52.000000 libyang-2.8.4/libyang/diff.py
--rw-r--r--   0 root         (0) root         (0)     5749 2024-02-07 13:04:52.000000 libyang-2.8.4/libyang/keyed_list.py
--rw-r--r--   0 root         (0) root         (0)     1941 2024-02-07 13:04:52.000000 libyang-2.8.4/libyang/log.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-07 13:04:52.000000 libyang-2.8.4/libyang/py.typed
--rw-r--r--   0 root         (0) root         (0)    54753 2024-02-07 13:04:52.000000 libyang-2.8.4/libyang/schema.py
--rw-r--r--   0 root         (0) root         (0)     3640 2024-02-07 13:04:52.000000 libyang-2.8.4/libyang/util.py
--rw-r--r--   0 root         (0) root         (0)    18831 2024-02-07 13:04:52.000000 libyang-2.8.4/libyang/xpath.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 13:05:08.418774 libyang-2.8.4/libyang.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9399 2024-02-07 13:05:08.000000 libyang-2.8.4/libyang.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      590 2024-02-07 13:05:08.000000 libyang-2.8.4/libyang.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-07 13:05:08.000000 libyang-2.8.4/libyang.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-07 13:05:08.000000 libyang-2.8.4/libyang.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       50 2024-02-07 13:05:08.000000 libyang-2.8.4/libyang.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-02-07 13:05:08.000000 libyang-2.8.4/libyang.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      289 2024-02-07 13:04:52.000000 libyang-2.8.4/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      713 2024-02-07 13:05:08.422774 libyang-2.8.4/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     5815 2024-02-07 13:04:52.000000 libyang-2.8.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 13:05:08.418774 libyang-2.8.4/tests/
--rw-r--r--   0 root         (0) root         (0)     4067 2024-02-07 13:04:52.000000 libyang-2.8.4/tests/test_context.py
--rw-r--r--   0 root         (0) root         (0)    31525 2024-02-07 13:04:52.000000 libyang-2.8.4/tests/test_data.py
--rw-r--r--   0 root         (0) root         (0)     4499 2024-02-07 13:04:52.000000 libyang-2.8.4/tests/test_diff.py
--rw-r--r--   0 root         (0) root         (0)     3547 2024-02-07 13:04:52.000000 libyang-2.8.4/tests/test_keyedlist.py
--rw-r--r--   0 root         (0) root         (0)    22411 2024-02-07 13:04:52.000000 libyang-2.8.4/tests/test_schema.py
--rw-r--r--   0 root         (0) root         (0)    15307 2024-02-07 13:04:52.000000 libyang-2.8.4/tests/test_xpath.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 10:11:49.907022 libyang-3.0.0/
+-rw-r--r--   0 root         (0) root         (0)     1073 2024-04-06 10:11:36.000000 libyang-3.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      205 2024-04-06 10:11:36.000000 libyang-3.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    11559 2024-04-06 10:11:49.907022 libyang-3.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10916 2024-04-06 10:11:36.000000 libyang-3.0.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 10:11:49.903022 libyang-3.0.0/cffi/
+-rw-r--r--   0 root         (0) root         (0)     1142 2024-04-06 10:11:36.000000 libyang-3.0.0/cffi/build.py
+-rw-r--r--   0 root         (0) root         (0)    29004 2024-04-06 10:11:36.000000 libyang-3.0.0/cffi/cdefs.h
+-rw-r--r--   0 root         (0) root         (0)      243 2024-04-06 10:11:36.000000 libyang-3.0.0/cffi/source.c
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 10:11:49.907022 libyang-3.0.0/libyang/
+-rw-r--r--   0 root         (0) root         (0)        6 2024-04-06 10:11:49.907022 libyang-3.0.0/libyang/VERSION
+-rw-r--r--   0 root         (0) root         (0)     3314 2024-04-06 10:11:36.000000 libyang-3.0.0/libyang/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15234 2024-04-06 10:11:36.000000 libyang-3.0.0/libyang/context.py
+-rw-r--r--   0 root         (0) root         (0)    45877 2024-04-06 10:11:36.000000 libyang-3.0.0/libyang/data.py
+-rw-r--r--   0 root         (0) root         (0)    13429 2024-04-06 10:11:36.000000 libyang-3.0.0/libyang/diff.py
+-rw-r--r--   0 root         (0) root         (0)     5749 2024-04-06 10:11:36.000000 libyang-3.0.0/libyang/keyed_list.py
+-rw-r--r--   0 root         (0) root         (0)     2104 2024-04-06 10:11:36.000000 libyang-3.0.0/libyang/log.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-06 10:11:36.000000 libyang-3.0.0/libyang/py.typed
+-rw-r--r--   0 root         (0) root         (0)    54753 2024-04-06 10:11:36.000000 libyang-3.0.0/libyang/schema.py
+-rw-r--r--   0 root         (0) root         (0)     3640 2024-04-06 10:11:36.000000 libyang-3.0.0/libyang/util.py
+-rw-r--r--   0 root         (0) root         (0)    18831 2024-04-06 10:11:36.000000 libyang-3.0.0/libyang/xpath.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 10:11:49.907022 libyang-3.0.0/libyang.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11559 2024-04-06 10:11:49.000000 libyang-3.0.0/libyang.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      590 2024-04-06 10:11:49.000000 libyang-3.0.0/libyang.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-06 10:11:49.000000 libyang-3.0.0/libyang.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-06 10:11:49.000000 libyang-3.0.0/libyang.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       50 2024-04-06 10:11:49.000000 libyang-3.0.0/libyang.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-04-06 10:11:49.000000 libyang-3.0.0/libyang.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      289 2024-04-06 10:11:36.000000 libyang-3.0.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      713 2024-04-06 10:11:49.907022 libyang-3.0.0/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     5815 2024-04-06 10:11:36.000000 libyang-3.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 10:11:49.907022 libyang-3.0.0/tests/
+-rw-r--r--   0 root         (0) root         (0)     4067 2024-04-06 10:11:36.000000 libyang-3.0.0/tests/test_context.py
+-rw-r--r--   0 root         (0) root         (0)    31724 2024-04-06 10:11:36.000000 libyang-3.0.0/tests/test_data.py
+-rw-r--r--   0 root         (0) root         (0)     4499 2024-04-06 10:11:36.000000 libyang-3.0.0/tests/test_diff.py
+-rw-r--r--   0 root         (0) root         (0)     3547 2024-04-06 10:11:36.000000 libyang-3.0.0/tests/test_keyedlist.py
+-rw-r--r--   0 root         (0) root         (0)    22411 2024-04-06 10:11:36.000000 libyang-3.0.0/tests/test_schema.py
+-rw-r--r--   0 root         (0) root         (0)    15307 2024-04-06 10:11:36.000000 libyang-3.0.0/tests/test_xpath.py
```

### Comparing `libyang-2.8.4/LICENSE` & `libyang-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `libyang-2.8.4/PKG-INFO` & `libyang-3.0.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libyang
-Version: 2.8.4
+Version: 3.0.0
 Summary: CFFI bindings to libyang
 Home-page: https://github.com/CESNET/libyang-python
 Author: Robin Jarry
 Author-email: robin@jarry.cc
 License: MIT
 Keywords: libyang,cffi
 Classifier: Development Status :: 4 - Beta
@@ -248,15 +248,15 @@
 
 #. Clone your own fork into your development machine::
 
       git clone https://github.com/<you>/libyang-python
 
 #. Create a new branch named after what your are working on::
 
-      git checkout -b my-topic
+      git checkout -b my-topic -t origin/master
 
 #. Edit the code and call ``make format`` to ensure your modifications comply
    with the `coding style`__.
 
    __ https://black.readthedocs.io/en/stable/the_black_code_style.html
 
    Your contribution must be licensed under the `MIT License`__ . At least one
@@ -267,29 +267,68 @@
 #. If you are adding a new feature or fixing a bug, please consider adding or
    updating unit tests.
 
 #. Before creating commits, run ``make lint`` and ``make tests`` to check if
    your changes do not break anything. You can also run ``make`` which will run
    both.
 
-#. Create commits by following these simple guidelines:
+#. Once you are happy with your work, you can create a commit (or several
+   commits). Follow these general rules:
 
-   -  Solve only one problem per commit.
-   -  Use a short (less than 72 characters) title on the first line followed by
-      an blank line and a more thorough description body.
-   -  Wrap the body of the commit message should be wrapped at 72 characters too
-      unless it breaks long URLs or code examples.
-   -  If the commit fixes a Github issue, include the following line::
+   -  Address only one issue/topic per commit.
+   -  Describe your changes in imperative mood, e.g. *"make xyzzy do frotz"*
+      instead of *"[This patch] makes xyzzy do frotz"* or *"[I] changed xyzzy to
+      do frotz"*, as if you are giving orders to the codebase to change its
+      behaviour.
+   -  Limit the first line (title) of the commit message to 60 characters.
+   -  Use a short prefix for the commit title for readability with ``git log
+      --oneline``. Do not use the `fix:` nor `feature:` prefixes. See recent
+      commits for inspiration.
+   -  Only use lower case letters for the commit title except when quoting
+      symbols or known acronyms.
+   -  Use the body of the commit message to actually explain what your patch
+      does and why it is useful. Even if your patch is a one line fix, the
+      description is not limited in length and may span over multiple
+      paragraphs. Use proper English syntax, grammar and punctuation.
+   -  If you are fixing an issue, use appropriate ``Closes: <URL>`` or
+      ``Fixes: <URL>`` trailers.
+   -  If you are fixing a regression introduced by another commit, add a
+      ``Fixes: <COMMIT_ID> ("<TITLE>")`` trailer.
+   -  When in doubt, follow the format and layout of the recent existing
+      commits.
+   -  The following trailers are accepted in commits. If you are using multiple
+      trailers in a commit, it's preferred to also order them according to this
+      list.
+
+      *  ``Closes: <URL>``: close the referenced issue or pull request.
+      *  ``Fixes: <SHA> ("<TITLE>")``: reference the commit that introduced
+         a regression.
+      *  ``Link: <URL>``: any useful link to provide context for your commit.
+      *  ``Suggested-by``
+      *  ``Requested-by``
+      *  ``Reported-by``
+      *  ``Co-authored-by``
+      *  ``Tested-by``
+      *  ``Reviewed-by``
+      *  ``Acked-by``
+      *  ``Signed-off-by``: Compulsory!
+
+   There is a great reference for commit messages in the `Linux kernel
+   documentation`__.
+
+   __ https://www.kernel.org/doc/html/latest/process/submitting-patches.html#describe-your-changes
+
+   IMPORTANT: you must sign-off your work using ``git commit --signoff``. Follow
+   the `Linux kernel developer's certificate of origin`__ for more details. All
+   contributions are made under the MIT license. If you do not want to disclose
+   your real name, you may sign-off using a pseudonym. Here is an example::
 
-        Fixes: #NNNN
+       Signed-off-by: Robin Jarry <robin@jarry.cc>
 
-   Inspirations:
-
-   https://chris.beams.io/posts/git-commit/
-   https://wiki.openstack.org/wiki/GitCommitMessages
+   __ https://www.kernel.org/doc/html/latest/process/submitting-patches.html#sign-your-work-the-developer-s-certificate-of-origin
 
 #. Push your topic branch in your forked repository::
 
       git push origin my-topic
 
    You should get a message from Github explaining how to create a new pull
    request.
```

### Comparing `libyang-2.8.4/README.rst` & `libyang-3.0.0/README.rst`

 * *Files 20% similar despite different names*

```diff
@@ -228,15 +228,15 @@
 
 #. Clone your own fork into your development machine::
 
       git clone https://github.com/<you>/libyang-python
 
 #. Create a new branch named after what your are working on::
 
-      git checkout -b my-topic
+      git checkout -b my-topic -t origin/master
 
 #. Edit the code and call ``make format`` to ensure your modifications comply
    with the `coding style`__.
 
    __ https://black.readthedocs.io/en/stable/the_black_code_style.html
 
    Your contribution must be licensed under the `MIT License`__ . At least one
@@ -247,29 +247,68 @@
 #. If you are adding a new feature or fixing a bug, please consider adding or
    updating unit tests.
 
 #. Before creating commits, run ``make lint`` and ``make tests`` to check if
    your changes do not break anything. You can also run ``make`` which will run
    both.
 
-#. Create commits by following these simple guidelines:
+#. Once you are happy with your work, you can create a commit (or several
+   commits). Follow these general rules:
 
-   -  Solve only one problem per commit.
-   -  Use a short (less than 72 characters) title on the first line followed by
-      an blank line and a more thorough description body.
-   -  Wrap the body of the commit message should be wrapped at 72 characters too
-      unless it breaks long URLs or code examples.
-   -  If the commit fixes a Github issue, include the following line::
+   -  Address only one issue/topic per commit.
+   -  Describe your changes in imperative mood, e.g. *"make xyzzy do frotz"*
+      instead of *"[This patch] makes xyzzy do frotz"* or *"[I] changed xyzzy to
+      do frotz"*, as if you are giving orders to the codebase to change its
+      behaviour.
+   -  Limit the first line (title) of the commit message to 60 characters.
+   -  Use a short prefix for the commit title for readability with ``git log
+      --oneline``. Do not use the `fix:` nor `feature:` prefixes. See recent
+      commits for inspiration.
+   -  Only use lower case letters for the commit title except when quoting
+      symbols or known acronyms.
+   -  Use the body of the commit message to actually explain what your patch
+      does and why it is useful. Even if your patch is a one line fix, the
+      description is not limited in length and may span over multiple
+      paragraphs. Use proper English syntax, grammar and punctuation.
+   -  If you are fixing an issue, use appropriate ``Closes: <URL>`` or
+      ``Fixes: <URL>`` trailers.
+   -  If you are fixing a regression introduced by another commit, add a
+      ``Fixes: <COMMIT_ID> ("<TITLE>")`` trailer.
+   -  When in doubt, follow the format and layout of the recent existing
+      commits.
+   -  The following trailers are accepted in commits. If you are using multiple
+      trailers in a commit, it's preferred to also order them according to this
+      list.
+
+      *  ``Closes: <URL>``: close the referenced issue or pull request.
+      *  ``Fixes: <SHA> ("<TITLE>")``: reference the commit that introduced
+         a regression.
+      *  ``Link: <URL>``: any useful link to provide context for your commit.
+      *  ``Suggested-by``
+      *  ``Requested-by``
+      *  ``Reported-by``
+      *  ``Co-authored-by``
+      *  ``Tested-by``
+      *  ``Reviewed-by``
+      *  ``Acked-by``
+      *  ``Signed-off-by``: Compulsory!
+
+   There is a great reference for commit messages in the `Linux kernel
+   documentation`__.
+
+   __ https://www.kernel.org/doc/html/latest/process/submitting-patches.html#describe-your-changes
+
+   IMPORTANT: you must sign-off your work using ``git commit --signoff``. Follow
+   the `Linux kernel developer's certificate of origin`__ for more details. All
+   contributions are made under the MIT license. If you do not want to disclose
+   your real name, you may sign-off using a pseudonym. Here is an example::
 
-        Fixes: #NNNN
+       Signed-off-by: Robin Jarry <robin@jarry.cc>
 
-   Inspirations:
-
-   https://chris.beams.io/posts/git-commit/
-   https://wiki.openstack.org/wiki/GitCommitMessages
+   __ https://www.kernel.org/doc/html/latest/process/submitting-patches.html#sign-your-work-the-developer-s-certificate-of-origin
 
 #. Push your topic branch in your forked repository::
 
       git push origin my-topic
 
    You should get a message from Github explaining how to create a new pull
    request.
```

### Comparing `libyang-2.8.4/cffi/build.py` & `libyang-3.0.0/cffi/build.py`

 * *Files identical despite different names*

### Comparing `libyang-2.8.4/cffi/cdefs.h` & `libyang-3.0.0/cffi/cdefs.h`

 * *Files 1% similar despite different names*

```diff
@@ -175,18 +175,18 @@
 #define LY_LOLOG ...
 #define LY_LOSTORE ...
 #define LY_LOSTORE_LAST ...
 int ly_log_options(int);
 
 LY_LOG_LEVEL ly_log_level(LY_LOG_LEVEL);
 extern "Python" void lypy_log_cb(LY_LOG_LEVEL, const char *, const char *);
-void ly_set_log_clb(void (*)(LY_LOG_LEVEL, const char *, const char *), int);
-struct ly_err_item *ly_err_first(const struct ly_ctx *);
+void ly_set_log_clb(void (*)(LY_LOG_LEVEL, const char *, const char *, const char *, uint64_t));
+const struct ly_err_item *ly_err_first(const struct ly_ctx *);
+const struct ly_err_item *ly_err_last(const struct ly_ctx *);
 void ly_err_clean(struct ly_ctx *, struct ly_err_item *);
-LY_VECODE ly_vecode(const struct ly_ctx *);
 
 #define LYS_UNKNOWN ...
 #define LYS_CONTAINER ...
 #define LYS_CHOICE ...
 #define LYS_LEAF ...
 #define LYS_LEAFLIST ...
 #define LYS_LIST ...
@@ -234,22 +234,23 @@
     struct lysc_ext_instance *exts;
     void *priv;
     ...;
 };
 
 struct ly_err_item {
     LY_LOG_LEVEL level;
-    LY_ERR no;
+    LY_ERR err;
     LY_VECODE vecode;
     char *msg;
-    char *path;
+    char *data_path;
+    char *schema_path;
+    uint64_t line;
     char *apptag;
     struct ly_err_item *next;
     struct ly_err_item *prev;
-    ...;
 };
 
 struct lyd_node {
     uint32_t hash;
     uint32_t flags;
     const struct lysc_node *schema;
     struct lyd_node_inner *parent;
@@ -257,19 +258,20 @@
     struct lyd_node *prev;
     struct lyd_meta *meta;
     void *priv;
 };
 
 LY_ERR lys_set_implemented(struct lys_module *,	const char **);
 
+#define LYD_NEW_VAL_OUTPUT ...
+#define LYD_NEW_VAL_BIN ...
+#define LYD_NEW_VAL_CANON ...
+#define LYD_NEW_META_CLEAR_DFLT ...
 #define LYD_NEW_PATH_UPDATE ...
-#define LYD_NEW_PATH_OUTPUT ...
-#define LYD_NEW_PATH_OPAQ   ...
-#define LYD_NEW_PATH_BIN_VALUE ...
-#define LYD_NEW_PATH_CANON_VALUE ...
+#define LYD_NEW_PATH_OPAQ ...
 LY_ERR lyd_new_path(struct lyd_node *, const struct ly_ctx *, const char *, const char *, uint32_t, struct lyd_node **);
 LY_ERR lyd_find_xpath(const struct lyd_node *, const char *, struct ly_set **);
 void lyd_unlink_siblings(struct lyd_node *node);
 void lyd_unlink_tree(struct lyd_node *node);
 void lyd_free_all(struct lyd_node *node);
 void lyd_free_tree(struct lyd_node *node);
 
@@ -610,14 +612,15 @@
     struct lysp_qname *uniques;
     uint32_t min;
     uint32_t max;
     ...;
 };
 
 struct lysc_type {
+    const char *name;
     struct lysc_ext_instance *exts;
     struct lyplg_type *plugin;
     LY_DATA_TYPE basetype;
     uint32_t refcount;
 };
 
 struct lysp_type {
@@ -637,14 +640,15 @@
     uint8_t require_instance;
     uint16_t flags;
 };
 
 struct lysp_qname {
     const char *str;
     const struct lysp_module *mod;
+    ...;
 };
 
 struct lysp_node {
     struct lysp_node *parent;
     uint16_t nodetype;
     uint16_t flags;
     struct lysp_node *next;
@@ -678,15 +682,14 @@
 
 struct lysc_ext {
     const char *name;
     const char *argname;
     struct lysc_ext_instance *exts;
     struct lyplg_ext *plugin;
     struct lys_module *module;
-    uint32_t refcount;
     uint16_t flags;
 };
 
 #define LYS_GETNEXT_WITHCHOICE ...
 #define LYS_GETNEXT_NOCHOICE ...
 #define LYS_GETNEXT_WITHCASE ...
 #define LYS_GETNEXT_INTONPCONT ...
@@ -699,19 +702,18 @@
 const struct lysc_node_notif* lysc_node_notifs(const struct lysc_node *);
 
 typedef enum {
     LYD_PATH_STD,
     LYD_PATH_STD_NO_LAST_PRED
 } LYD_PATH_TYPE;
 
-LY_ERR lyd_new_term(struct lyd_node *, const struct lys_module *, const char *, const char *, ly_bool, struct lyd_node **);
+LY_ERR lyd_new_term(struct lyd_node *, const struct lys_module *, const char *, const char *, uint32_t, struct lyd_node **);
 char* lyd_path(const struct lyd_node *, LYD_PATH_TYPE, char *, size_t);
 LY_ERR lyd_new_inner(struct lyd_node *, const struct lys_module *, const char *, ly_bool, struct lyd_node **);
-LY_ERR lyd_new_list(struct lyd_node *, const struct lys_module *, const char *, ly_bool, struct lyd_node **, ...);
-LY_ERR lyd_new_list2(struct lyd_node *, const struct lys_module *, const char *, const char *, ly_bool, struct lyd_node **);
+LY_ERR lyd_new_list(struct lyd_node *, const struct lys_module *, const char *, uint32_t, struct lyd_node **node, ...);
 
 struct lyd_node_inner {
     union {
         struct lyd_node node;
         struct {
             uint32_t hash;
             uint32_t flags;
@@ -817,31 +819,34 @@
     const char *eapptag;
     const char *dsc;
     const char *ref;
     struct lysp_ext_instance *exts;
 };
 
 struct lysc_type_num {
+    const char *name;
     struct lysc_ext_instance *exts;
     struct lyplg_type *plugin;
     LY_DATA_TYPE basetype;
     uint32_t refcount;
     struct lysc_range *range;
 };
 
 struct lysc_type_dec {
+    const char *name;
     struct lysc_ext_instance *exts;
     struct lyplg_type *plugin;
     LY_DATA_TYPE basetype;
     uint32_t refcount;
     uint8_t fraction_digits;
     struct lysc_range *range;
 };
 
 struct lysc_type_str {
+    const char *name;
     struct lysc_ext_instance *exts;
     struct lyplg_type *plugin;
     LY_DATA_TYPE basetype;
     uint32_t refcount;
     struct lysc_range *length;
     struct lysc_pattern **patterns;
 };
@@ -855,66 +860,72 @@
         int32_t value;
         uint32_t position;
     };
     uint16_t flags;
 };
 
 struct lysc_type_enum {
+    const char *name;
     struct lysc_ext_instance *exts;
     struct lyplg_type *plugin;
     LY_DATA_TYPE basetype;
     uint32_t refcount;
     struct lysc_type_bitenum_item *enums;
 };
 
 struct lysc_type_bits {
+    const char *name;
     struct lysc_ext_instance *exts;
     struct lyplg_type *plugin;
     LY_DATA_TYPE basetype;
     uint32_t refcount;
     struct lysc_type_bitenum_item *bits;
 };
 
 struct lysc_type_leafref {
+    const char *name;
     struct lysc_ext_instance *exts;
     struct lyplg_type *plugin;
     LY_DATA_TYPE basetype;
     uint32_t refcount;
     struct lyxp_expr *path;
     struct lysc_prefix *prefixes;
-    const struct lys_module *cur_mod;
     struct lysc_type *realtype;
     uint8_t require_instance;
 };
 
 struct lysc_type_identityref {
+    const char *name;
     struct lysc_ext_instance *exts;
     struct lyplg_type *plugin;
     LY_DATA_TYPE basetype;
     uint32_t refcount;
     struct lysc_ident **bases;
 };
 
 struct lysc_type_instanceid {
+    const char *name;
     struct lysc_ext_instance *exts;
     struct lyplg_type *plugin;
     LY_DATA_TYPE basetype;
     uint32_t refcount;
     uint8_t require_instance;
 };
 
 struct lysc_type_union {
+    const char *name;
     struct lysc_ext_instance *exts;
     struct lyplg_type *plugin;
     LY_DATA_TYPE basetype;
     uint32_t refcount;
     struct lysc_type **types;
 };
 
 struct lysc_type_bin {
+    const char *name;
     struct lysc_ext_instance *exts;
     struct lyplg_type *plugin;
     LY_DATA_TYPE basetype;
     uint32_t refcount;
     struct lysc_range *length;
 };
 
@@ -1049,15 +1060,15 @@
 #define LYD_IMPLICIT_NO_CONFIG ...
 #define LYD_IMPLICIT_OUTPUT ...
 #define LYD_IMPLICIT_NO_DEFAULTS ...
 
 LY_ERR lyd_new_implicit_tree(struct lyd_node *, uint32_t, struct lyd_node **);
 LY_ERR lyd_new_implicit_all(struct lyd_node **, const struct ly_ctx *, uint32_t, struct lyd_node **);
 
-LY_ERR lyd_new_meta(const struct ly_ctx *, struct lyd_node *, const struct lys_module *, const char *, const char *, ly_bool, struct lyd_meta **);
+LY_ERR lyd_new_meta(const struct ly_ctx *, struct lyd_node *, const struct lys_module *, const char *, const char *, uint32_t, struct lyd_meta **);
 
 struct ly_opaq_name {
     const char *name;
     const char *prefix;
 
     union {
         const char *module_ns;
```

### Comparing `libyang-2.8.4/libyang/__init__.py` & `libyang-3.0.0/libyang/__init__.py`

 * *Files identical despite different names*

### Comparing `libyang-2.8.4/libyang/context.py` & `libyang-3.0.0/libyang/context.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 from typing import IO, Any, Iterator, Optional, Union
 
 from _libyang import ffi, lib
 from .data import (
     DNode,
     data_format,
     data_type,
+    newval_flags,
     parser_flags,
-    path_flags,
     validation_flags,
 )
 from .schema import Module, SNode, schema_in_format
 from .util import DataType, IOType, LibyangError, c2str, data_load, str2c
 
 
 # -------------------------------------------------------------------------------------
@@ -113,16 +113,20 @@
         msg %= args
 
         if self.cdata:
             err = lib.ly_err_first(self.cdata)
             while err:
                 if err.msg:
                     msg += ": %s" % c2str(err.msg)
-                if err.path:
-                    msg += ": %s" % c2str(err.path)
+                if err.data_path:
+                    msg += ": Data path: %s" % c2str(err.data_path)
+                if err.schema_path:
+                    msg += ": Schema path: %s" % c2str(err.schema_path)
+                if err.line != 0:
+                    msg += " (line %u)" % err.line
                 err = err.next
             lib.ly_err_clean(self.cdata, ffi.NULL)
 
         return LibyangError(msg)
 
     def parse_module(
         self,
@@ -230,40 +234,38 @@
 
     def create_data_path(
         self,
         path: str,
         parent: Optional[DNode] = None,
         value: Any = None,
         update: bool = True,
-        no_parent_ret: bool = True,
         rpc_output: bool = False,
         force_return_value: bool = True,
     ) -> Optional[DNode]:
         if self.cdata is None:
             raise RuntimeError("context already destroyed")
         if value is not None:
             if isinstance(value, bool):
                 value = str(value).lower()
             elif not isinstance(value, str):
                 value = str(value)
-        flags = path_flags(
-            update=update, no_parent_ret=no_parent_ret, rpc_output=rpc_output
-        )
+        flags = newval_flags(update=update, rpc_output=rpc_output)
         dnode = ffi.new("struct lyd_node **")
         ret = lib.lyd_new_path(
             parent.cdata if parent else ffi.NULL,
             self.cdata,
             str2c(path),
             str2c(value),
             flags,
             dnode,
         )
         dnode = dnode[0]
         if ret != lib.LY_SUCCESS:
-            if lib.ly_vecode(self.cdata) != lib.LYVE_SUCCESS:
+            err = lib.ly_err_last(self.cdata)
+            if err != ffi.NULL and err.vecode != lib.LYVE_SUCCESS:
                 raise self.error("cannot create data path: %s", path)
             lib.ly_err_clean(self.cdata, ffi.NULL)
         if not dnode and not force_return_value:
             return None
 
         if not dnode and parent:
             # This can happen when path points to an already created leaf and
```

### Comparing `libyang-2.8.4/libyang/data.py` & `libyang-3.0.0/libyang/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,22 +73,38 @@
         return lib.LYD_XML
     if fmt_string == "lyb":
         return lib.LYD_LYB
     raise ValueError("unknown data format: %r" % fmt_string)
 
 
 # -------------------------------------------------------------------------------------
-def path_flags(
-    update: bool = False, rpc_output: bool = False, no_parent_ret: bool = False
+def newval_flags(
+    rpc_output: bool = False,
+    bin_value: bool = False,
+    canon_value: bool = False,
+    meta_clear_default: bool = False,
+    update: bool = False,
+    opaq: bool = False,
 ) -> int:
+    """
+    Translate from booleans to newvaloptions flags.
+    """
     flags = 0
+    if rpc_output:
+        flags |= lib.LYD_NEW_VAL_OUTPUT
+    if bin_value:
+        flags |= lib.LYD_NEW_VAL_BIN
+    if canon_value:
+        flags |= lib.LYD_NEW_VAL_CANON
+    if meta_clear_default:
+        flags |= lib.LYD_NEW_META_CLEAR_DFLT
     if update:
         flags |= lib.LYD_NEW_PATH_UPDATE
-    if rpc_output:
-        flags |= lib.LYD_NEW_PATH_OUTPUT
+    if opaq:
+        flags |= lib.LYD_NEW_PATH_OPAQ
     return flags
 
 
 # -------------------------------------------------------------------------------------
 def parser_flags(
     lyb_mod_update: bool = False,
     no_state: bool = False,
@@ -295,21 +311,22 @@
         while item != ffi.NULL:
             if c2str(item.name) == name:
                 lib.lyd_free_meta_single(item)
                 break
             item = item.next
 
     def new_meta(self, name: str, value: str, clear_dflt: bool = False):
+        flags = newval_flags(meta_clear_default=clear_dflt)
         ret = lib.lyd_new_meta(
             ffi.NULL,
             self.cdata,
             ffi.NULL,
             str2c(name),
             str2c(value),
-            clear_dflt,
+            flags,
             ffi.NULL,
         )
         if ret != lib.LY_SUCCESS:
             raise self.context.error("cannot create meta")
 
     def attrs(self) -> DNodeAttrs:
         if not self.attributes:
@@ -362,28 +379,23 @@
         value: str,
         opt_update: bool = False,
         opt_output: bool = False,
         opt_opaq: bool = False,
         opt_bin_value: bool = False,
         opt_canon_value: bool = False,
     ):
-        opt = 0
-        if opt_update:
-            opt |= lib.LYD_NEW_PATH_UPDATE
-        if opt_output:
-            opt |= lib.LYD_NEW_PATH_OUTPUT
-        if opt_opaq:
-            opt |= lib.LYD_NEW_PATH_OPAQ
-        if opt_bin_value:
-            opt |= lib.LYD_NEW_PATH_BIN_VALUE
-        if opt_canon_value:
-            opt |= lib.LYD_NEW_PATH_CANON_VALUE
-
+        flags = newval_flags(
+            update=opt_update,
+            rpc_output=opt_output,
+            opaq=opt_opaq,
+            bin_value=opt_bin_value,
+            canon_value=opt_canon_value,
+        )
         ret = lib.lyd_new_path(
-            self.cdata, ffi.NULL, str2c(path), str2c(value), opt, ffi.NULL
+            self.cdata, ffi.NULL, str2c(path), str2c(value), flags, ffi.NULL
         )
         if ret != lib.LY_SUCCESS:
             raise self.context.error("cannot get module")
 
     def insert_child(self, node):
         ret = lib.lyd_insert_child(self.cdata, node.cdata)
         if ret != lib.LY_SUCCESS:
@@ -1001,15 +1013,18 @@
             lib.free(path)
 
 
 # -------------------------------------------------------------------------------------
 @DNode.register(SNode.CONTAINER)
 class DContainer(DNode):
     def create_path(
-        self, path: str, value: Any = None, rpc_output: bool = False
+        self,
+        path: str,
+        value: Any = None,
+        rpc_output: bool = False,
     ) -> Optional[DNode]:
         return self.context.create_data_path(
             path, parent=self, value=value, rpc_output=rpc_output
         )
 
     def children(self, no_keys=False) -> Iterator[DNode]:
         if no_keys:
@@ -1175,16 +1190,22 @@
         if value is not None:
             if isinstance(value, bool):
                 value = str(value).lower()
             elif not isinstance(value, str):
                 value = str(value)
 
         n = ffi.new("struct lyd_node **")
+        flags = newval_flags(rpc_output=in_rpc_output)
         ret = lib.lyd_new_term(
-            _parent, module.cdata, str2c(name), str2c(value), in_rpc_output, n
+            _parent,
+            module.cdata,
+            str2c(name),
+            str2c(value),
+            flags,
+            n,
         )
 
         if ret != lib.LY_SUCCESS:
             if _parent:
                 parent_path = repr(DNode.new(module.context, _parent).path())
             else:
                 parent_path = "module %r" % module.name()
@@ -1207,19 +1228,20 @@
                 parent_path,
             )
         created.append(n[0])
         return n[0]
 
     def _create_list(_parent, module, name, key_values, in_rpc_output=False):
         n = ffi.new("struct lyd_node **")
+        flags = newval_flags(rpc_output=in_rpc_output)
         ret = lib.lyd_new_list(
             _parent,
             module.cdata,
             str2c(name),
-            in_rpc_output,
+            flags,
             n,
             *[str2c(str(i)) for i in key_values],
         )
         if ret != lib.LY_SUCCESS:
             if _parent:
                 parent_path = repr(DNode.new(module.context, _parent).path())
             else:
```

### Comparing `libyang-2.8.4/libyang/diff.py` & `libyang-3.0.0/libyang/diff.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     differences.
 
     :arg ctx_old:
         The first context.
     :arg ctx_new:
         The second context.
     :arg exclude_node_cb:
-        Optionnal user callback that will be called with each node that is found in each
+        Optional user callback that will be called with each node that is found in each
         context. If the callback returns a "trueish" value, the node will be excluded
         from the diff (as well as all its children).
     :arg use_data_path:
         Use data path instead of schema path to compare the nodes. Using data path
         ignores choices and cases.
 
     :return:
```

### Comparing `libyang-2.8.4/libyang/keyed_list.py` & `libyang-3.0.0/libyang/keyed_list.py`

 * *Files identical despite different names*

### Comparing `libyang-2.8.4/libyang/log.py` & `libyang-3.0.0/libyang/log.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,21 +16,26 @@
     lib.LY_LLWRN: logging.WARNING,
     lib.LY_LLVRB: logging.INFO,
     lib.LY_LLDBG: logging.DEBUG,
 }
 
 
 @ffi.def_extern(name="lypy_log_cb")
-def libyang_c_logging_callback(level, msg, path):
+def libyang_c_logging_callback(level, msg, data_path, schema_path, line):
     args = [c2str(msg)]
-    if path:
-        fmt = "%s: %s"
-        args.append(c2str(path))
-    else:
-        fmt = "%s"
+    fmt = "%s"
+    if data_path:
+        fmt += ": %s"
+        args.append(c2str(data_path))
+    if schema_path:
+        fmt += ": %s"
+        args.append(c2str(schema_path))
+    if line != 0:
+        fmt += " line %u"
+        args.append(str(line))
     LOG.log(LOG_LEVELS.get(level, logging.NOTSET), fmt, *args)
 
 
 def configure_logging(enable_py_logger: bool, level: int = logging.ERROR) -> None:
     """
     Configure libyang logging behaviour.
 
@@ -47,14 +52,14 @@
     """
     for ly_lvl, py_lvl in LOG_LEVELS.items():
         if py_lvl == level:
             lib.ly_log_level(ly_lvl)
             break
     if enable_py_logger:
         lib.ly_log_options(lib.LY_LOLOG | lib.LY_LOSTORE)
-        lib.ly_set_log_clb(lib.lypy_log_cb, True)
+        lib.ly_set_log_clb(lib.lypy_log_cb)
     else:
         lib.ly_log_options(lib.LY_LOSTORE)
-        lib.ly_set_log_clb(ffi.NULL, False)
+        lib.ly_set_log_clb(ffi.NULL)
 
 
 configure_logging(False, logging.ERROR)
```

### Comparing `libyang-2.8.4/libyang/schema.py` & `libyang-3.0.0/libyang/schema.py`

 * *Files identical despite different names*

### Comparing `libyang-2.8.4/libyang/util.py` & `libyang-3.0.0/libyang/util.py`

 * *Files identical despite different names*

### Comparing `libyang-2.8.4/libyang/xpath.py` & `libyang-3.0.0/libyang/xpath.py`

 * *Files identical despite different names*

### Comparing `libyang-2.8.4/libyang.egg-info/PKG-INFO` & `libyang-3.0.0/libyang.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libyang
-Version: 2.8.4
+Version: 3.0.0
 Summary: CFFI bindings to libyang
 Home-page: https://github.com/CESNET/libyang-python
 Author: Robin Jarry
 Author-email: robin@jarry.cc
 License: MIT
 Keywords: libyang,cffi
 Classifier: Development Status :: 4 - Beta
@@ -248,15 +248,15 @@
 
 #. Clone your own fork into your development machine::
 
       git clone https://github.com/<you>/libyang-python
 
 #. Create a new branch named after what your are working on::
 
-      git checkout -b my-topic
+      git checkout -b my-topic -t origin/master
 
 #. Edit the code and call ``make format`` to ensure your modifications comply
    with the `coding style`__.
 
    __ https://black.readthedocs.io/en/stable/the_black_code_style.html
 
    Your contribution must be licensed under the `MIT License`__ . At least one
@@ -267,29 +267,68 @@
 #. If you are adding a new feature or fixing a bug, please consider adding or
    updating unit tests.
 
 #. Before creating commits, run ``make lint`` and ``make tests`` to check if
    your changes do not break anything. You can also run ``make`` which will run
    both.
 
-#. Create commits by following these simple guidelines:
+#. Once you are happy with your work, you can create a commit (or several
+   commits). Follow these general rules:
 
-   -  Solve only one problem per commit.
-   -  Use a short (less than 72 characters) title on the first line followed by
-      an blank line and a more thorough description body.
-   -  Wrap the body of the commit message should be wrapped at 72 characters too
-      unless it breaks long URLs or code examples.
-   -  If the commit fixes a Github issue, include the following line::
+   -  Address only one issue/topic per commit.
+   -  Describe your changes in imperative mood, e.g. *"make xyzzy do frotz"*
+      instead of *"[This patch] makes xyzzy do frotz"* or *"[I] changed xyzzy to
+      do frotz"*, as if you are giving orders to the codebase to change its
+      behaviour.
+   -  Limit the first line (title) of the commit message to 60 characters.
+   -  Use a short prefix for the commit title for readability with ``git log
+      --oneline``. Do not use the `fix:` nor `feature:` prefixes. See recent
+      commits for inspiration.
+   -  Only use lower case letters for the commit title except when quoting
+      symbols or known acronyms.
+   -  Use the body of the commit message to actually explain what your patch
+      does and why it is useful. Even if your patch is a one line fix, the
+      description is not limited in length and may span over multiple
+      paragraphs. Use proper English syntax, grammar and punctuation.
+   -  If you are fixing an issue, use appropriate ``Closes: <URL>`` or
+      ``Fixes: <URL>`` trailers.
+   -  If you are fixing a regression introduced by another commit, add a
+      ``Fixes: <COMMIT_ID> ("<TITLE>")`` trailer.
+   -  When in doubt, follow the format and layout of the recent existing
+      commits.
+   -  The following trailers are accepted in commits. If you are using multiple
+      trailers in a commit, it's preferred to also order them according to this
+      list.
+
+      *  ``Closes: <URL>``: close the referenced issue or pull request.
+      *  ``Fixes: <SHA> ("<TITLE>")``: reference the commit that introduced
+         a regression.
+      *  ``Link: <URL>``: any useful link to provide context for your commit.
+      *  ``Suggested-by``
+      *  ``Requested-by``
+      *  ``Reported-by``
+      *  ``Co-authored-by``
+      *  ``Tested-by``
+      *  ``Reviewed-by``
+      *  ``Acked-by``
+      *  ``Signed-off-by``: Compulsory!
+
+   There is a great reference for commit messages in the `Linux kernel
+   documentation`__.
+
+   __ https://www.kernel.org/doc/html/latest/process/submitting-patches.html#describe-your-changes
+
+   IMPORTANT: you must sign-off your work using ``git commit --signoff``. Follow
+   the `Linux kernel developer's certificate of origin`__ for more details. All
+   contributions are made under the MIT license. If you do not want to disclose
+   your real name, you may sign-off using a pseudonym. Here is an example::
 
-        Fixes: #NNNN
+       Signed-off-by: Robin Jarry <robin@jarry.cc>
 
-   Inspirations:
-
-   https://chris.beams.io/posts/git-commit/
-   https://wiki.openstack.org/wiki/GitCommitMessages
+   __ https://www.kernel.org/doc/html/latest/process/submitting-patches.html#sign-your-work-the-developer-s-certificate-of-origin
 
 #. Push your topic branch in your forked repository::
 
       git push origin my-topic
 
    You should get a message from Github explaining how to create a new pull
    request.
```

### Comparing `libyang-2.8.4/libyang.egg-info/SOURCES.txt` & `libyang-3.0.0/libyang.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `libyang-2.8.4/setup.cfg` & `libyang-3.0.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `libyang-2.8.4/setup.py` & `libyang-3.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `libyang-2.8.4/tests/test_context.py` & `libyang-3.0.0/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `libyang-2.8.4/tests/test_data.py` & `libyang-3.0.0/tests/test_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,23 +130,23 @@
         "proto": "https",
         "host": "github.com",
         "path": "/CESNET/libyang-python",
         "enabled": false
       },
       {
         "proto": "http",
+        "host": "barfoo.com",
+        "path": "/barfoo/index.html"
+      },
+      {
+        "proto": "http",
         "host": "foobar.com",
         "port": 8080,
         "path": "/index.html",
         "enabled": true
-      },
-      {
-        "proto": "http",
-        "host": "barfoo.com",
-        "path": "/barfoo/index.html"
       }
     ],
     "number": [
       1000,
       2000,
       3000
     ],
@@ -278,15 +278,17 @@
                 "xml",
                 validate_present=True,
                 validate_multi_error=True,
             )
         self.assertEqual(
             str(cm.exception),
             'failed to parse data tree: Invalid boolean value "abcd".: '
-            'List instance is missing its key "host".',
+            "Data path: /yolo-system:conf/url[proto='https']/enabled (line 6): "
+            'List instance is missing its key "host".: '
+            "Data path: /yolo-system:conf/url[proto='https'] (line 7)",
         )
 
     XML_STATE = """<state xmlns="urn:yang:yolo:system">
   <hostname>foo</hostname>
   <url>
     <proto>https</proto>
     <host>github.com</host>
@@ -804,15 +806,15 @@
     <enabled yang:operation="replace" yang:orig-default="false" yang:orig-value="false">true</enabled>
   </url>
   <url yang:operation="none">
     <proto>http</proto>
     <host>foobar.com</host>
     <enabled yang:operation="replace" yang:orig-default="false" yang:orig-value="true">false</enabled>
   </url>
-  <url yang:operation="create">
+  <url yang:operation="create" yang:key="[proto='http'][host='foobar.com']">
     <proto>ftp</proto>
     <host>github.com</host>
     <path>/CESNET/libyang-python</path>
     <enabled>false</enabled>
   </url>
   <number yang:operation="delete" yang:orig-position="1">2000</number>
   <speed yang:operation="replace" yang:orig-default="false" yang:orig-value="1234">5432</speed>
```

### Comparing `libyang-2.8.4/tests/test_diff.py` & `libyang-3.0.0/tests/test_diff.py`

 * *Files identical despite different names*

### Comparing `libyang-2.8.4/tests/test_keyedlist.py` & `libyang-3.0.0/tests/test_keyedlist.py`

 * *Files identical despite different names*

### Comparing `libyang-2.8.4/tests/test_schema.py` & `libyang-3.0.0/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `libyang-2.8.4/tests/test_xpath.py` & `libyang-3.0.0/tests/test_xpath.py`

 * *Files identical despite different names*

