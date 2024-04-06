# Comparing `tmp/boilersaas-0.6.4.tar.gz` & `tmp/boilersaas-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boilersaas-0.6.4.tar", last modified: Thu Mar 28 14:46:47 2024, max compression
+gzip compressed data, was "boilersaas-0.6.5.tar", last modified: Sat Apr  6 21:56:52 2024, max compression
```

## Comparing `boilersaas-0.6.4.tar` & `boilersaas-0.6.5.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 imac1      (501) staff       (20)        0 2024-03-28 14:46:47.021371 boilersaas-0.6.4/
--rw-r--r--   0 imac1      (501) staff       (20)      274 2024-03-28 14:46:47.021130 boilersaas-0.6.4/PKG-INFO
--rw-r--r--   0 imac1      (501) staff       (20)       94 2024-03-24 17:11:45.000000 boilersaas-0.6.4/pyproject.toml
--rw-r--r--   0 imac1      (501) staff       (20)       38 2024-03-28 14:46:47.021435 boilersaas-0.6.4/setup.cfg
--rw-r--r--   0 imac1      (501) staff       (20)     1300 2024-03-28 14:29:30.000000 boilersaas-0.6.4/setup.py
-drwxr-xr-x   0 imac1      (501) staff       (20)        0 2024-03-28 14:46:47.009421 boilersaas-0.6.4/src/
-drwxr-xr-x   0 imac1      (501) staff       (20)        0 2024-03-28 14:46:47.012068 boilersaas-0.6.4/src/boilersaas/
--rw-r--r--   0 imac1      (501) staff       (20)     1223 2024-03-28 14:06:19.000000 boilersaas-0.6.4/src/boilersaas/__init__.py
--rw-r--r--   0 imac1      (501) staff       (20)     2565 2024-03-28 11:53:17.000000 boilersaas-0.6.4/src/boilersaas/forms.py
--rw-r--r--   0 imac1      (501) staff       (20)     2089 2024-03-24 18:28:30.000000 boilersaas-0.6.4/src/boilersaas/models.py
--rw-r--r--   0 imac1      (501) staff       (20)     8715 2024-03-28 14:32:33.000000 boilersaas-0.6.4/src/boilersaas/routes.py
--rw-r--r--   0 imac1      (501) staff       (20)     3188 2024-03-28 11:55:03.000000 boilersaas-0.6.4/src/boilersaas/signin_social.py
-drwxr-xr-x   0 imac1      (501) staff       (20)        0 2024-03-28 14:46:47.016798 boilersaas-0.6.4/src/boilersaas/templates/
--rw-r--r--   0 imac1      (501) staff       (20)     2544 2024-03-28 12:51:34.000000 boilersaas-0.6.4/src/boilersaas/templates/base.html
--rw-r--r--   0 imac1      (501) staff       (20)     1033 2024-03-28 14:34:15.000000 boilersaas-0.6.4/src/boilersaas/templates/blank.html
-drwxr-xr-x   0 imac1      (501) staff       (20)        0 2024-03-28 14:46:47.017781 boilersaas-0.6.4/src/boilersaas/templates/components/
--rw-r--r--   0 imac1      (501) staff       (20)      576 2024-03-28 14:35:31.000000 boilersaas-0.6.4/src/boilersaas/templates/components/button_signin_facebook.html
--rw-r--r--   0 imac1      (501) staff       (20)     1113 2024-03-28 14:35:41.000000 boilersaas-0.6.4/src/boilersaas/templates/components/button_signin_google.html
--rw-r--r--   0 imac1      (501) staff       (20)      506 2024-03-28 14:35:48.000000 boilersaas-0.6.4/src/boilersaas/templates/components/button_signin_x.html
--rw-r--r--   0 imac1      (501) staff       (20)      817 2024-03-28 14:36:17.000000 boilersaas-0.6.4/src/boilersaas/templates/components/section_social_signin.html
--rw-r--r--   0 imac1      (501) staff       (20)      323 2024-03-28 12:58:49.000000 boilersaas-0.6.4/src/boilersaas/templates/dashboard.html
-drwxr-xr-x   0 imac1      (501) staff       (20)        0 2024-03-28 14:46:47.018694 boilersaas-0.6.4/src/boilersaas/templates/email/
--rw-r--r--   0 imac1      (501) staff       (20)     1276 2024-03-24 17:11:45.000000 boilersaas-0.6.4/src/boilersaas/templates/email/invite_send.html
--rw-r--r--   0 imac1      (501) staff       (20)     1204 2024-03-24 17:11:45.000000 boilersaas-0.6.4/src/boilersaas/templates/email/reset_password.html
--rw-r--r--   0 imac1      (501) staff       (20)     1104 2024-03-24 17:11:45.000000 boilersaas-0.6.4/src/boilersaas/templates/email/welcome.html
--rw-r--r--   0 imac1      (501) staff       (20)      186 2024-03-28 12:59:06.000000 boilersaas-0.6.4/src/boilersaas/templates/for_tailwind.html
--rw-r--r--   0 imac1      (501) staff       (20)      347 2024-03-28 12:59:35.000000 boilersaas-0.6.4/src/boilersaas/templates/index.html
--rw-r--r--   0 imac1      (501) staff       (20)      551 2024-03-24 17:11:45.000000 boilersaas-0.6.4/src/boilersaas/templates/invite_create.html
--rw-r--r--   0 imac1      (501) staff       (20)     1794 2024-03-28 13:51:30.000000 boilersaas-0.6.4/src/boilersaas/templates/invites.html
--rw-r--r--   0 imac1      (501) staff       (20)     1185 2024-03-24 17:11:45.000000 boilersaas-0.6.4/src/boilersaas/templates/login.html
--rw-r--r--   0 imac1      (501) staff       (20)       56 2024-03-24 17:11:45.000000 boilersaas-0.6.4/src/boilersaas/templates/logo.html
--rw-r--r--   0 imac1      (501) staff       (20)     1265 2024-03-24 17:11:45.000000 boilersaas-0.6.4/src/boilersaas/templates/register.html
--rw-r--r--   0 imac1      (501) staff       (20)     1204 2024-03-24 17:11:45.000000 boilersaas-0.6.4/src/boilersaas/templates/register_invite.html
--rw-r--r--   0 imac1      (501) staff       (20)      736 2024-03-28 13:46:39.000000 boilersaas-0.6.4/src/boilersaas/templates/reset_request.html
--rw-r--r--   0 imac1      (501) staff       (20)      662 2024-03-28 13:45:40.000000 boilersaas-0.6.4/src/boilersaas/templates/reset_request_with_token.html
-drwxr-xr-x   0 imac1      (501) staff       (20)        0 2024-03-28 14:46:47.019297 boilersaas-0.6.4/src/boilersaas/translations/
--rw-r--r--   0 imac1      (501) staff       (20)       43 2024-03-24 17:11:45.000000 boilersaas-0.6.4/src/boilersaas/translations/PyBabel.cfg
--rw-r--r--   0 imac1      (501) staff       (20)      630 2024-03-28 13:48:30.000000 boilersaas-0.6.4/src/boilersaas/translations/README.md
-drwxr-xr-x   0 imac1      (501) staff       (20)        0 2024-03-28 14:46:47.009799 boilersaas-0.6.4/src/boilersaas/translations/es/
-drwxr-xr-x   0 imac1      (501) staff       (20)        0 2024-03-28 14:46:47.020041 boilersaas-0.6.4/src/boilersaas/translations/es/LC_MESSAGES/
--rw-r--r--   0 imac1      (501) staff       (20)     3150 2024-03-28 14:43:23.000000 boilersaas-0.6.4/src/boilersaas/translations/es/LC_MESSAGES/messages.mo
--rw-r--r--   0 imac1      (501) staff       (20)     4364 2024-03-28 14:43:13.000000 boilersaas-0.6.4/src/boilersaas/translations/es/LC_MESSAGES/messages.po
--rw-r--r--   0 imac1      (501) staff       (20)     3374 2024-03-28 14:40:29.000000 boilersaas-0.6.4/src/boilersaas/translations/messages.pot
--rw-r--r--   0 imac1      (501) staff       (20)      204 2024-03-24 17:11:45.000000 boilersaas-0.6.4/src/boilersaas/types.py
-drwxr-xr-x   0 imac1      (501) staff       (20)        0 2024-03-28 14:46:47.020804 boilersaas-0.6.4/src/boilersaas/utils/
--rw-r--r--   0 imac1      (501) staff       (20)        0 2024-03-24 17:11:45.000000 boilersaas-0.6.4/src/boilersaas/utils/__init__.py
--rw-r--r--   0 imac1      (501) staff       (20)       59 2024-03-24 17:11:45.000000 boilersaas-0.6.4/src/boilersaas/utils/db.py
--rw-r--r--   0 imac1      (501) staff       (20)     1087 2024-03-28 14:29:50.000000 boilersaas-0.6.4/src/boilersaas/utils/locale.py
--rw-r--r--   0 imac1      (501) staff       (20)      494 2024-03-24 17:11:45.000000 boilersaas-0.6.4/src/boilersaas/utils/mail.py
-drwxr-xr-x   0 imac1      (501) staff       (20)        0 2024-03-28 14:46:47.013141 boilersaas-0.6.4/src/boilersaas.egg-info/
--rw-r--r--   0 imac1      (501) staff       (20)      274 2024-03-28 14:46:46.000000 boilersaas-0.6.4/src/boilersaas.egg-info/PKG-INFO
--rw-r--r--   0 imac1      (501) staff       (20)     1634 2024-03-28 14:46:46.000000 boilersaas-0.6.4/src/boilersaas.egg-info/SOURCES.txt
--rw-r--r--   0 imac1      (501) staff       (20)        1 2024-03-28 14:46:46.000000 boilersaas-0.6.4/src/boilersaas.egg-info/dependency_links.txt
--rw-r--r--   0 imac1      (501) staff       (20)      274 2024-03-28 14:46:46.000000 boilersaas-0.6.4/src/boilersaas.egg-info/requires.txt
--rw-r--r--   0 imac1      (501) staff       (20)       11 2024-03-28 14:46:46.000000 boilersaas-0.6.4/src/boilersaas.egg-info/top_level.txt
+drwxr-xr-x   0 imac1      (501) staff       (20)        0 2024-04-06 21:56:52.642390 boilersaas-0.6.5/
+-rw-r--r--   0 imac1      (501) staff       (20)      274 2024-04-06 21:56:52.642155 boilersaas-0.6.5/PKG-INFO
+-rw-r--r--   0 imac1      (501) staff       (20)       94 2024-03-24 17:11:45.000000 boilersaas-0.6.5/pyproject.toml
+-rw-r--r--   0 imac1      (501) staff       (20)       38 2024-04-06 21:56:52.642439 boilersaas-0.6.5/setup.cfg
+-rw-r--r--   0 imac1      (501) staff       (20)     1300 2024-04-06 21:56:43.000000 boilersaas-0.6.5/setup.py
+drwxr-xr-x   0 imac1      (501) staff       (20)        0 2024-04-06 21:56:52.631697 boilersaas-0.6.5/src/
+drwxr-xr-x   0 imac1      (501) staff       (20)        0 2024-04-06 21:56:52.633743 boilersaas-0.6.5/src/boilersaas/
+-rw-r--r--   0 imac1      (501) staff       (20)     1223 2024-03-28 14:06:19.000000 boilersaas-0.6.5/src/boilersaas/__init__.py
+-rw-r--r--   0 imac1      (501) staff       (20)     2565 2024-03-28 11:53:17.000000 boilersaas-0.6.5/src/boilersaas/forms.py
+-rw-r--r--   0 imac1      (501) staff       (20)     2089 2024-03-24 18:28:30.000000 boilersaas-0.6.5/src/boilersaas/models.py
+-rw-r--r--   0 imac1      (501) staff       (20)     8715 2024-03-28 14:32:33.000000 boilersaas-0.6.5/src/boilersaas/routes.py
+-rw-r--r--   0 imac1      (501) staff       (20)     3188 2024-03-28 11:55:03.000000 boilersaas-0.6.5/src/boilersaas/signin_social.py
+drwxr-xr-x   0 imac1      (501) staff       (20)        0 2024-04-06 21:56:52.638089 boilersaas-0.6.5/src/boilersaas/templates/
+-rw-r--r--   0 imac1      (501) staff       (20)     2555 2024-04-06 21:54:25.000000 boilersaas-0.6.5/src/boilersaas/templates/base.html
+-rw-r--r--   0 imac1      (501) staff       (20)     1033 2024-03-28 14:34:15.000000 boilersaas-0.6.5/src/boilersaas/templates/blank.html
+drwxr-xr-x   0 imac1      (501) staff       (20)        0 2024-04-06 21:56:52.639087 boilersaas-0.6.5/src/boilersaas/templates/components/
+-rw-r--r--   0 imac1      (501) staff       (20)      576 2024-03-28 14:35:31.000000 boilersaas-0.6.5/src/boilersaas/templates/components/button_signin_facebook.html
+-rw-r--r--   0 imac1      (501) staff       (20)     1113 2024-03-28 14:35:41.000000 boilersaas-0.6.5/src/boilersaas/templates/components/button_signin_google.html
+-rw-r--r--   0 imac1      (501) staff       (20)      506 2024-03-28 14:35:48.000000 boilersaas-0.6.5/src/boilersaas/templates/components/button_signin_x.html
+-rw-r--r--   0 imac1      (501) staff       (20)      817 2024-03-28 14:36:17.000000 boilersaas-0.6.5/src/boilersaas/templates/components/section_social_signin.html
+-rw-r--r--   0 imac1      (501) staff       (20)      323 2024-03-28 12:58:49.000000 boilersaas-0.6.5/src/boilersaas/templates/dashboard.html
+drwxr-xr-x   0 imac1      (501) staff       (20)        0 2024-04-06 21:56:52.639894 boilersaas-0.6.5/src/boilersaas/templates/email/
+-rw-r--r--   0 imac1      (501) staff       (20)     1276 2024-03-24 17:11:45.000000 boilersaas-0.6.5/src/boilersaas/templates/email/invite_send.html
+-rw-r--r--   0 imac1      (501) staff       (20)     1204 2024-03-24 17:11:45.000000 boilersaas-0.6.5/src/boilersaas/templates/email/reset_password.html
+-rw-r--r--   0 imac1      (501) staff       (20)     1104 2024-03-24 17:11:45.000000 boilersaas-0.6.5/src/boilersaas/templates/email/welcome.html
+-rw-r--r--   0 imac1      (501) staff       (20)      186 2024-03-28 12:59:06.000000 boilersaas-0.6.5/src/boilersaas/templates/for_tailwind.html
+-rw-r--r--   0 imac1      (501) staff       (20)      347 2024-03-28 12:59:35.000000 boilersaas-0.6.5/src/boilersaas/templates/index.html
+-rw-r--r--   0 imac1      (501) staff       (20)      551 2024-03-24 17:11:45.000000 boilersaas-0.6.5/src/boilersaas/templates/invite_create.html
+-rw-r--r--   0 imac1      (501) staff       (20)     1794 2024-03-28 13:51:30.000000 boilersaas-0.6.5/src/boilersaas/templates/invites.html
+-rw-r--r--   0 imac1      (501) staff       (20)     1185 2024-03-24 17:11:45.000000 boilersaas-0.6.5/src/boilersaas/templates/login.html
+-rw-r--r--   0 imac1      (501) staff       (20)       56 2024-03-24 17:11:45.000000 boilersaas-0.6.5/src/boilersaas/templates/logo.html
+-rw-r--r--   0 imac1      (501) staff       (20)     1265 2024-03-24 17:11:45.000000 boilersaas-0.6.5/src/boilersaas/templates/register.html
+-rw-r--r--   0 imac1      (501) staff       (20)     1204 2024-03-24 17:11:45.000000 boilersaas-0.6.5/src/boilersaas/templates/register_invite.html
+-rw-r--r--   0 imac1      (501) staff       (20)      736 2024-03-28 13:46:39.000000 boilersaas-0.6.5/src/boilersaas/templates/reset_request.html
+-rw-r--r--   0 imac1      (501) staff       (20)      662 2024-03-28 13:45:40.000000 boilersaas-0.6.5/src/boilersaas/templates/reset_request_with_token.html
+drwxr-xr-x   0 imac1      (501) staff       (20)        0 2024-04-06 21:56:52.640525 boilersaas-0.6.5/src/boilersaas/translations/
+-rw-r--r--   0 imac1      (501) staff       (20)       43 2024-03-24 17:11:45.000000 boilersaas-0.6.5/src/boilersaas/translations/PyBabel.cfg
+-rw-r--r--   0 imac1      (501) staff       (20)      630 2024-03-28 13:48:30.000000 boilersaas-0.6.5/src/boilersaas/translations/README.md
+drwxr-xr-x   0 imac1      (501) staff       (20)        0 2024-04-06 21:56:52.632061 boilersaas-0.6.5/src/boilersaas/translations/es/
+drwxr-xr-x   0 imac1      (501) staff       (20)        0 2024-04-06 21:56:52.641094 boilersaas-0.6.5/src/boilersaas/translations/es/LC_MESSAGES/
+-rw-r--r--   0 imac1      (501) staff       (20)     3150 2024-03-28 14:43:23.000000 boilersaas-0.6.5/src/boilersaas/translations/es/LC_MESSAGES/messages.mo
+-rw-r--r--   0 imac1      (501) staff       (20)     4364 2024-03-28 14:43:13.000000 boilersaas-0.6.5/src/boilersaas/translations/es/LC_MESSAGES/messages.po
+-rw-r--r--   0 imac1      (501) staff       (20)     3374 2024-03-28 14:40:29.000000 boilersaas-0.6.5/src/boilersaas/translations/messages.pot
+-rw-r--r--   0 imac1      (501) staff       (20)      204 2024-03-24 17:11:45.000000 boilersaas-0.6.5/src/boilersaas/types.py
+drwxr-xr-x   0 imac1      (501) staff       (20)        0 2024-04-06 21:56:52.641937 boilersaas-0.6.5/src/boilersaas/utils/
+-rw-r--r--   0 imac1      (501) staff       (20)        0 2024-03-24 17:11:45.000000 boilersaas-0.6.5/src/boilersaas/utils/__init__.py
+-rw-r--r--   0 imac1      (501) staff       (20)       59 2024-03-24 17:11:45.000000 boilersaas-0.6.5/src/boilersaas/utils/db.py
+-rw-r--r--   0 imac1      (501) staff       (20)     1087 2024-03-28 14:29:50.000000 boilersaas-0.6.5/src/boilersaas/utils/locale.py
+-rw-r--r--   0 imac1      (501) staff       (20)      494 2024-03-24 17:11:45.000000 boilersaas-0.6.5/src/boilersaas/utils/mail.py
+drwxr-xr-x   0 imac1      (501) staff       (20)        0 2024-04-06 21:56:52.634497 boilersaas-0.6.5/src/boilersaas.egg-info/
+-rw-r--r--   0 imac1      (501) staff       (20)      274 2024-04-06 21:56:52.000000 boilersaas-0.6.5/src/boilersaas.egg-info/PKG-INFO
+-rw-r--r--   0 imac1      (501) staff       (20)     1634 2024-04-06 21:56:52.000000 boilersaas-0.6.5/src/boilersaas.egg-info/SOURCES.txt
+-rw-r--r--   0 imac1      (501) staff       (20)        1 2024-04-06 21:56:52.000000 boilersaas-0.6.5/src/boilersaas.egg-info/dependency_links.txt
+-rw-r--r--   0 imac1      (501) staff       (20)      274 2024-04-06 21:56:52.000000 boilersaas-0.6.5/src/boilersaas.egg-info/requires.txt
+-rw-r--r--   0 imac1      (501) staff       (20)       11 2024-04-06 21:56:52.000000 boilersaas-0.6.5/src/boilersaas.egg-info/top_level.txt
```

### Comparing `boilersaas-0.6.4/setup.py` & `boilersaas-0.6.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="boilersaas",
-    version="0.6.4",
+    version="0.6.5",
     package_dir={"": "src"},
     packages=find_packages(where="src"),
     include_package_data=True,
       package_data={
         # Include templates, translations, and any other non-python files
       "boilersaas": [
             "templates/**/*.html",  # Recursively include all HTML files in templates directory
```

### Comparing `boilersaas-0.6.4/src/boilersaas/__init__.py` & `boilersaas-0.6.5/src/boilersaas/__init__.py`

 * *Files identical despite different names*

### Comparing `boilersaas-0.6.4/src/boilersaas/forms.py` & `boilersaas-0.6.5/src/boilersaas/forms.py`

 * *Files identical despite different names*

### Comparing `boilersaas-0.6.4/src/boilersaas/models.py` & `boilersaas-0.6.5/src/boilersaas/models.py`

 * *Files identical despite different names*

### Comparing `boilersaas-0.6.4/src/boilersaas/routes.py` & `boilersaas-0.6.5/src/boilersaas/routes.py`

 * *Files identical despite different names*

### Comparing `boilersaas-0.6.4/src/boilersaas/signin_social.py` & `boilersaas-0.6.5/src/boilersaas/signin_social.py`

 * *Files identical despite different names*

### Comparing `boilersaas-0.6.4/src/boilersaas/templates/base.html` & `boilersaas-0.6.5/src/boilersaas/templates/base.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 <!DOCTYPE html>
-<html lang="en">
+<html lang="en" data-theme="light">
 
 <head>
     <meta charset="UTF-8">
     <meta name="viewport" content="width=device-width, initial-scale=1.0">
     <title>{{ page_title }}</title>
     <link href="{{url_for('static',filename='css/tailwind/output.css')}}" rel="stylesheet">
 </head>
 
 <body>
     <div class="container mx-auto ">
-        <header class="bg-white border-b-2 border-slate-200">
+        <header class=" border-b-2 border-slate-200">
             <nav class="mx-auto flex  items-center justify-between py-5 " aria-label="Global">
                 <div class="flex lg:flex-1">
                     {% include 'logo.html' %}
                 </div>
 
                 {% if current_user.is_authenticated %}
```

### Comparing `boilersaas-0.6.4/src/boilersaas/templates/blank.html` & `boilersaas-0.6.5/src/boilersaas/templates/blank.html`

 * *Files identical despite different names*

### Comparing `boilersaas-0.6.4/src/boilersaas/templates/components/button_signin_facebook.html` & `boilersaas-0.6.5/src/boilersaas/templates/components/button_signin_facebook.html`

 * *Files identical despite different names*

### Comparing `boilersaas-0.6.4/src/boilersaas/templates/components/button_signin_google.html` & `boilersaas-0.6.5/src/boilersaas/templates/components/button_signin_google.html`

 * *Files identical despite different names*

### Comparing `boilersaas-0.6.4/src/boilersaas/templates/components/section_social_signin.html` & `boilersaas-0.6.5/src/boilersaas/templates/components/section_social_signin.html`

 * *Files identical despite different names*

### Comparing `boilersaas-0.6.4/src/boilersaas/templates/email/invite_send.html` & `boilersaas-0.6.5/src/boilersaas/templates/email/invite_send.html`

 * *Files identical despite different names*

### Comparing `boilersaas-0.6.4/src/boilersaas/templates/email/reset_password.html` & `boilersaas-0.6.5/src/boilersaas/templates/email/reset_password.html`

 * *Files identical despite different names*

### Comparing `boilersaas-0.6.4/src/boilersaas/templates/email/welcome.html` & `boilersaas-0.6.5/src/boilersaas/templates/email/welcome.html`

 * *Files identical despite different names*

### Comparing `boilersaas-0.6.4/src/boilersaas/templates/invite_create.html` & `boilersaas-0.6.5/src/boilersaas/templates/invite_create.html`

 * *Files identical despite different names*

### Comparing `boilersaas-0.6.4/src/boilersaas/templates/invites.html` & `boilersaas-0.6.5/src/boilersaas/templates/invites.html`

 * *Files identical despite different names*

### Comparing `boilersaas-0.6.4/src/boilersaas/templates/login.html` & `boilersaas-0.6.5/src/boilersaas/templates/login.html`

 * *Files identical despite different names*

### Comparing `boilersaas-0.6.4/src/boilersaas/templates/register.html` & `boilersaas-0.6.5/src/boilersaas/templates/register.html`

 * *Files identical despite different names*

### Comparing `boilersaas-0.6.4/src/boilersaas/templates/register_invite.html` & `boilersaas-0.6.5/src/boilersaas/templates/register_invite.html`

 * *Files identical despite different names*

### Comparing `boilersaas-0.6.4/src/boilersaas/templates/reset_request.html` & `boilersaas-0.6.5/src/boilersaas/templates/reset_request.html`

 * *Files identical despite different names*

### Comparing `boilersaas-0.6.4/src/boilersaas/templates/reset_request_with_token.html` & `boilersaas-0.6.5/src/boilersaas/templates/reset_request_with_token.html`

 * *Files identical despite different names*

### Comparing `boilersaas-0.6.4/src/boilersaas/translations/README.md` & `boilersaas-0.6.5/src/boilersaas/translations/README.md`

 * *Files identical despite different names*

### Comparing `boilersaas-0.6.4/src/boilersaas/translations/es/LC_MESSAGES/messages.mo` & `boilersaas-0.6.5/src/boilersaas/translations/es/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `boilersaas-0.6.4/src/boilersaas/translations/es/LC_MESSAGES/messages.po` & `boilersaas-0.6.5/src/boilersaas/translations/es/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `boilersaas-0.6.4/src/boilersaas/translations/messages.pot` & `boilersaas-0.6.5/src/boilersaas/translations/messages.pot`

 * *Files identical despite different names*

### Comparing `boilersaas-0.6.4/src/boilersaas/utils/locale.py` & `boilersaas-0.6.5/src/boilersaas/utils/locale.py`

 * *Files identical despite different names*

### Comparing `boilersaas-0.6.4/src/boilersaas.egg-info/SOURCES.txt` & `boilersaas-0.6.5/src/boilersaas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

