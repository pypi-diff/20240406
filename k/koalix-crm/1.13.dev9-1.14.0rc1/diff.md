# Comparing `tmp/koalix-crm-1.13.dev9.tar.gz` & `tmp/koalix-crm-1.14.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/koalix-crm-1.13.dev9.tar", last modified: Sat Mar 28 17:08:48 2020, max compression
+gzip compressed data, was "koalix-crm-1.14.0rc1.tar", last modified: Sat Apr  6 11:47:58 2024, max compression
```

## Comparing `koalix-crm-1.13.dev9.tar` & `koalix-crm-1.14.0rc1.tar`

### file list

```diff
@@ -1,453 +1,456 @@
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1181 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/global_support_functions.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     2326 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/plugin.py
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/subscriptions/
--rw-r--r--   0 jenkins    (112) jenkins    (116)       26 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/subscriptions/views.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     3449 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/subscriptions/admin.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     4326 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/subscriptions/models.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/subscriptions/__init__.py
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/subscriptions/migrations/
--rw-r--r--   0 jenkins    (112) jenkins    (116)     6490 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/subscriptions/migrations/0004_auto_20181013_2213.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     3715 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/subscriptions/migrations/0001_initial.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     3603 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/subscriptions/migrations/0003_auto_20171110_1732.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)       24 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/subscriptions/migrations/__init__.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     3604 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/subscriptions/migrations/0002_auto_20171009_1949.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     5735 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/subscriptions/migrations/0005_auto_20181013_2228.py
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/subscriptions/const/
--rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/subscriptions/const/__init__.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      175 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/subscriptions/const/events.py
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/subscriptions/locale/
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/subscriptions/locale/pt_BR/
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/subscriptions/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 jenkins    (112) jenkins    (116)     2910 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/subscriptions/locale/pt_BR/LC_MESSAGES/django.po
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1648 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/subscriptions/locale/pt_BR/LC_MESSAGES/django.mo
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/subscriptions/locale/de/
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/subscriptions/locale/de/LC_MESSAGES/
--rw-r--r--   0 jenkins    (112) jenkins    (116)     2873 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/subscriptions/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1507 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/subscriptions/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/__init__.py
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/static/
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/static/default_templates/
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/static/default_templates/en/
--rw-r--r--   0 jenkins    (112) jenkins    (116)    10746 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/static/default_templates/en/profitlossstatement.xsl
--rw-r--r--   0 jenkins    (112) jenkins    (116)    11838 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/static/default_templates/en/balancesheet.xsl
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/static/default_templates/de/
--rw-r--r--   0 jenkins    (112) jenkins    (116)    10401 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/static/default_templates/de/profitlossstatement.xsl
--rw-r--r--   0 jenkins    (112) jenkins    (116)    10486 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/static/default_templates/de/balancesheet.xsl
--rw-r--r--   0 jenkins    (112) jenkins    (116)      663 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/exceptions.py
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/management/
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/management/commands/
--rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/management/commands/__init__.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/management/__init__.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     3550 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/views.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      623 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/admin.py
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/factories/
--rw-r--r--   0 jenkins    (112) jenkins    (116)      330 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/factories/factory_product_category.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/factories/__init__.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      374 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/models.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/__init__.py
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/rest/
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1524 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/rest/account_rest.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/rest/__init__.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     2866 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/rest/product_categorie_rest.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     2650 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/rest/restinterface.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     5414 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/rest/booking_rest.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      720 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/rest/accounting_period_rest.py
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/accounting/
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1664 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/accounting/product_category.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)    11316 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/accounting/accounting_period.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     8768 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/accounting/account.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/accounting/__init__.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     3405 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/accounting/booking.py
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/migrations/
--rw-r--r--   0 jenkins    (112) jenkins    (116)      780 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/migrations/0008_auto_20181012_2056.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     4451 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/migrations/0001_initial.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1633 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/migrations/0010_auto_20181216_2224.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1285 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/migrations/0007_auto_20180422_2105.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)       24 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/migrations/__init__.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     3463 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/migrations/0006_auto_20180422_2048.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     6726 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/migrations/0005_auto_20171110_1732.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     6786 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/migrations/0004_auto_20171009_1949.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      404 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/migrations/0003_remove_account_originalamount.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     2146 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/migrations/0002_auto_20170705_1702.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1030 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/migrations/0009_auto_20181012_2056.py
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/tests/
--rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/tests/__init__.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)    11709 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/tests/test_accountingModelTest.py
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/const/
--rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/const/__init__.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      207 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/const/accountTypeChoices.py
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/locale/
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/locale/pt_BR/
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 jenkins    (112) jenkins    (116)     7519 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/locale/pt_BR/LC_MESSAGES/django.po
--rw-r--r--   0 jenkins    (112) jenkins    (116)     4242 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/locale/pt_BR/LC_MESSAGES/django.mo
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/locale/de/
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/locale/de/LC_MESSAGES/
--rw-r--r--   0 jenkins    (112) jenkins    (116)     6010 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0 jenkins    (112) jenkins    (116)     2778 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/accounting/locale/de/LC_MESSAGES/django.mo
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/
--rw-r--r--   0 jenkins    (112) jenkins    (116)      943 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/exceptions.py
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/user_extension/
--rw-r--r--   0 jenkins    (112) jenkins    (116)     4427 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/user_extension/document_template.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/user_extension/__init__.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     7364 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/user_extension/user_extension.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1042 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/user_extension/text_paragraph.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     5285 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/user_extension/template_set.py
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/management/
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/management/commands/
--rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/management/commands/__init__.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/management/__init__.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1838 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/admin.py
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/factories/
--rw-r--r--   0 jenkins    (112) jenkins    (116)     3347 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/factories/factory_document_template.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      696 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/factories/factory_user_extension.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/factories/__init__.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      258 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/factories/factory_template_set.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      325 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/models.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/__init__.py
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/rest/
--rw-r--r--   0 jenkins    (112) jenkins    (116)    16815 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/rest/template_set_rest.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/rest/__init__.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      695 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/rest/user_extension_rest.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      356 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/rest/user_rest.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     3975 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/rest/document_template_rest.py
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/migrations/
--rw-r--r--   0 jenkins    (112) jenkins    (116)     9678 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/migrations/0001_initial.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     7474 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/migrations/0003_auto_20171110_1732.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1230 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/migrations/0005_auto_20180612_1924.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)    10481 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/migrations/0004_auto_20171210_2126.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)       24 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/migrations/__init__.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      637 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/migrations/0007_auto_20180702_1628.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     6874 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/migrations/0002_auto_20171009_1949.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     2212 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/migrations/0006_auto_20180701_2128.py
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/const/
--rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/const/__init__.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      229 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/const/purpose.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     4427 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/test_support_functions.py
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/crm/
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/crm/templates/
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/crm/templates/crm/
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/crm/templates/crm/admin/
--rw-r--r--   0 jenkins    (112) jenkins    (116)     5940 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/templates/crm/admin/time_reporting.html
--rw-r--r--   0 jenkins    (112) jenkins    (116)      579 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/templates/crm/admin/set_timezone.html
--rw-r--r--   0 jenkins    (112) jenkins    (116)      842 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/templates/crm/admin/create_work_report.html
--rw-r--r--   0 jenkins    (112) jenkins    (116)      983 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/templates/crm/admin/register_payment.html
--rw-r--r--   0 jenkins    (112) jenkins    (116)      647 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/templates/crm/admin/exception.html
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/crm/static/
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/crm/static/default_templates/
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/crm/static/default_templates/generic/
--rw-r--r--   0 jenkins    (112) jenkins    (116)    54101 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/static/default_templates/generic/logo.jpg
--rw-r--r--   0 jenkins    (112) jenkins    (116)   122303 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/static/default_templates/generic/dejavusans-bold.xml
--rw-r--r--   0 jenkins    (112) jenkins    (116)     5699 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/static/default_templates/generic/fontconfig.xml
--rw-r--r--   0 jenkins    (112) jenkins    (116)   704128 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/static/default_templates/generic/DejaVuSans-Bold.ttf
--rw-r--r--   0 jenkins    (112) jenkins    (116)   756072 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/static/default_templates/generic/DejaVuSans.ttf
--rw-r--r--   0 jenkins    (112) jenkins    (116)   156738 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/static/default_templates/generic/dejavusans.xml
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/crm/static/default_templates/en/
--rw-r--r--   0 jenkins    (112) jenkins    (116)    50534 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/static/default_templates/en/purchaseconfirmation.xsl
--rw-r--r--   0 jenkins    (112) jenkins    (116)    50629 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/static/default_templates/en/purchaseorder.xsl
--rw-r--r--   0 jenkins    (112) jenkins    (116)    50508 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/static/default_templates/en/deliveryorder.xsl
--rw-r--r--   0 jenkins    (112) jenkins    (116)    50599 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/static/default_templates/en/invoice.xsl
--rw-r--r--   0 jenkins    (112) jenkins    (116)    50630 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/static/default_templates/en/quote.xsl
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/crm/static/default_templates/de/
--rwxr-xr-x   0 jenkins    (112) jenkins    (116)    27411 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/static/default_templates/de/work_report.xsl
--rw-r--r--   0 jenkins    (112) jenkins    (116)    50534 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/static/default_templates/de/purchaseconfirmation.xsl
--rw-r--r--   0 jenkins    (112) jenkins    (116)    50629 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/static/default_templates/de/purchaseorder.xsl
--rw-r--r--   0 jenkins    (112) jenkins    (116)    50507 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/static/default_templates/de/deliveryorder.xsl
--rw-r--r--   0 jenkins    (112) jenkins    (116)    50540 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/static/default_templates/de/invoice.xsl
--rw-r--r--   0 jenkins    (112) jenkins    (116)    30645 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/static/default_templates/de/project_report.xsl
--rw-r--r--   0 jenkins    (112) jenkins    (116)    50629 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/static/default_templates/de/quote.xsl
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/crm/reporting/
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1232 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/reporting/task_status.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     2183 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/reporting/generic_task_link.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     2782 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/reporting/generic_project_link.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     7885 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/reporting/work.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1001 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/reporting/resource.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1458 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/reporting/estimation_status.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1440 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/reporting/agreement_status.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)    26869 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/reporting/project.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     3037 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/reporting/agreement.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1543 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/reporting/reporting_period_status.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/reporting/__init__.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1032 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/reporting/resource_price.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      861 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/reporting/agreement_type.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1416 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/reporting/project_status.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     7245 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/reporting/estimation.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      864 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/reporting/urls.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)    27663 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/reporting/task.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1023 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/reporting/resource_type.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      614 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/reporting/resource_manager.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      870 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/reporting/project_link_type.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)    13725 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/reporting/human_resource.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      855 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/reporting/task_link_type.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)    11426 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/reporting/reporting_period.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     2183 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/exceptions.py
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/crm/management/
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/crm/management/commands/
--rw-r--r--   0 jenkins    (112) jenkins    (116)     4865 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/management/commands/koalixcrm_install_defaulttemplates.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/management/commands/__init__.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/management/__init__.py
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/crm/contact/
--rw-r--r--   0 jenkins    (112) jenkins    (116)     5279 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/contact/customer.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      384 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/contact/email_address.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1149 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/contact/customer_billing_cycle.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1988 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/contact/person.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/contact/__init__.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     2629 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/contact/postal_address.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1313 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/contact/supplier.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      380 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/contact/phone_address.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      574 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/contact/customer_group.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     9916 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/contact/contact.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     4282 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/contact/call.py
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/crm/product/
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1844 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/product/tax.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     2101 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/product/currency_transform.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1035 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/product/product_price.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/product/__init__.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     2131 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/product/unit_transform.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     5867 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/product/product_type.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      455 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/product/product.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1809 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/product/unit.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     2971 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/product/customer_group_transform.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1933 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/product/currency.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     6455 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/product/price.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     4447 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/admin.py
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/crm/middleware/
--rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/middleware/__init__.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      428 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/middleware/timezoneMiddleware.py
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/
--rw-r--r--   0 jenkins    (112) jenkins    (116)      915 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_reporting_period_status.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      488 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_project_status.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      848 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_agreement_status.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      346 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_delivery_note.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1072 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_project.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      689 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_sales_document_position.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      552 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_currency.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      297 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_purchase_confirmation.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      751 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_customer_group_transform.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      377 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_resource_manager.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      496 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_customer_group.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      657 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_unit_transform.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      422 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_payment_reminder.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      313 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_resource_type.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      691 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_human_resource.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1658 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_sales_document.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/__init__.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      790 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_customer.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      965 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_contract.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1173 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_generic_project_link.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1981 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_agreement.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      723 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_currency_transform.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      321 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_tax.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      538 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_project_link_type.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      443 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_purchase_order.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      594 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_task_link_type.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      453 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_contact.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      512 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_resource.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1670 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_estimation.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1170 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_generic_task_link.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      457 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_postal_address.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      383 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_customer_billing_cycle.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      371 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_invoice.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1501 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_resource_price.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      868 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_estimation_status.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      239 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_product.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      953 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_work.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      788 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_task_status.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      679 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_task.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      299 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_quote.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      974 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_product_type.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      649 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_reporting_period.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      318 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_agreement_type.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1133 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_user.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      655 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_unit.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1829 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_product_price.py
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/crm/views/
--rw-r--r--   0 jenkins    (112) jenkins    (116)     4600 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/views/pdfexport.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      354 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/views/set_timezone.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     4103 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/views/time_tracking.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     2129 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/views/user_extension_missing.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     6226 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/views/work_entry_form.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/views/__init__.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     2132 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/views/create_work_report.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     2120 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/views/template_set_missing.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1948 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/views/user_is_not_human_resource.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     5633 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/views/create_task.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     2140 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/views/reporting_period_missing.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1964 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/views/range_selection_form.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     3001 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/views/newdocument.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     2635 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/views/renderer.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     3957 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/views/work_entry_formset.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     2885 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/models.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/__init__.py
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/crm/rest/
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1592 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/rest/resource_manager_rest.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     2894 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/rest/unit_rest.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      383 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/rest/currency_rest.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      728 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/rest/resource_type_rest.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     5586 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/rest/project_rest.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     2739 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/rest/resource_rest.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     7180 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/rest/contact_rest.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     3417 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/rest/customer_rest.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      944 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/rest/agreement_status_rest.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     4701 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/rest/work_rest.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     3711 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/rest/estimation_rest.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/rest/__init__.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     2987 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/rest/tax_rest.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      906 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/rest/customer_billing_cycle_rest.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      555 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/rest/customer_group_rest.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      644 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/rest/task_status_rest.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      662 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/rest/project_status_rest.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     3801 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/rest/product_rest.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)    10754 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/rest/restinterface.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     3623 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/rest/task_rest.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     5956 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/rest/agreement_rest.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      734 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/rest/agreement_type_rest.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      962 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/rest/estimation_status_rest.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     4073 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/rest/human_resource_rest.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     4438 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/rest/resource_price_rest.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      969 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/rest/reporting_period_status_rest.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     3607 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/rest/reporting_period_rest.py
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1332 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0036_auto_20180626_2059.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      605 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0029_auto_20180611_1903.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      858 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0008_auto_20180104_2042.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      616 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0044_reportingperiod_status.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      600 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0039_auto_20180702_1635.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      521 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0047_work_worked_hours.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      457 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0010_auto_20180104_2138.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     7581 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0015_auto_20180111_2043.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     6072 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0025_auto_20180413_1937.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1428 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0048_auto_20181012_2056.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)    53282 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0001_initial.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     5968 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0027_auto_20180606_2034.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     2448 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0011_auto_20180104_2152.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      403 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0058_auto_20190401_2009.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1791 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0007_auto_20171210_2126.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     2269 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0038_auto_20180702_1628.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      705 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0024_auto_20180122_2121.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     3366 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0032_auto_20180612_1925.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     2741 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0051_auto_20181014_2302.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      547 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0002_auto_20170927_2042.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1150 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0021_purchaseorder.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      574 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0041_auto_20180724_1657.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      766 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0020_auto_20180116_2056.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     2217 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0018_auto_20180111_2031.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1854 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0017_auto_20180111_2022.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     4572 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0056_auto_20181216_2224.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)       24 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/__init__.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      989 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0028_auto_20180611_1835.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      751 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0022_auto_20180117_2020.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      473 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0037_auto_20180701_2128.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)    41477 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0005_auto_20171110_1732.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      624 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0012_auto_20180105_1840.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     2741 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0052_auto_20181014_2304.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     4850 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0006_auto_20171210_1805.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     2753 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0004_auto_20171009_2008.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     2407 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0050_auto_20181014_2300.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      389 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0046_auto_20180805_2051.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1316 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0016_auto_20180111_2011.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1557 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0045_auto_20180805_2047.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      600 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0035_auto_20180619_1924.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1095 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0026_auto_20180507_1957.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      575 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0040_auto_20180724_1657.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      698 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0014_auto_20180108_2048.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1149 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0055_auto_20181022_1937.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      265 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0057_merge_20190106_1510.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)    17512 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0053_auto_20181014_2305.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      496 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0054_auto_20181020_1845.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     6285 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0009_auto_20180104_2111.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      576 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0056_auto_20190102_2230.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     2144 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0013_auto_20180105_2159.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1685 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0034_genericprojectlink.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)    42385 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0003_auto_20171009_1949.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1542 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0049_auto_20181014_2258.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      732 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0033_auto_20180612_1936.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      576 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0042_auto_20180724_1816.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      486 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0023_auto_20180119_2102.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1955 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0019_auto_20180112_2020.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      514 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0031_auto_20180612_1924.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1085 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0030_auto_20180611_1930.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      981 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0043_reportingperiodstatus.py
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/crm/tests/
--rw-r--r--   0 jenkins    (112) jenkins    (116)     2510 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_poject_admin_view.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     6017 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_work_delete.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     5602 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_user_is_not_human_resource.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     3500 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_task_planned_costs.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     6608 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_view_work_entry_form.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     3624 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_task_update_last_status_update.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     3350 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_supplier_admin_view.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     5090 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_create_sales_document_from_contract.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     3754 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_time_tracking_add_row.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     4363 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_incomplete_sales_document_position.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     5120 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_task_effective_effort.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)    16626 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_calculations_document.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     5670 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_project_planned_costs.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     5647 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_task_effective_duration.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     2045 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_create_task.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/tests/__init__.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     5232 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_create_sales_document_from_quote.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     6510 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_task_effective_costs_with_agreement.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     7340 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_delete_of_empty_row.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     6337 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_create_sales_document_from_invoice.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     5667 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_task_effective_costs_no_agreement.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     5986 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_project_effective_costs.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1105 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_version_increase.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     3864 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_task_planned_effort.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     2991 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_task_constructor.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     3260 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_task_planned_duration.py
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/crm/const/
--rw-r--r--   0 jenkins    (112) jenkins    (116)      188 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/const/postaladdressprefix.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)    10650 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/const/country.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/const/__init__.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      955 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/const/status.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      935 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/const/purpose.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     2152 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/inlinemixin.py
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/crm/documents/
--rw-r--r--   0 jenkins    (112) jenkins    (116)    13462 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/documents/contract.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)    21434 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/documents/sales_document.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     3204 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/documents/payment_reminder.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1326 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/documents/purchase_confirmation.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     5232 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/documents/calculations.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     9519 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/documents/invoice.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/documents/__init__.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     3578 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/documents/quote.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     5038 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/documents/pdf_export.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1983 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/documents/purchase_order.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     5730 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/documents/sales_document_position.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1627 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/documents/delivery_note.py
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/crm/locale/
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/crm/locale/pt_BR/
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/crm/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 jenkins    (112) jenkins    (116)    62091 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/locale/pt_BR/LC_MESSAGES/django.po
--rw-r--r--   0 jenkins    (112) jenkins    (116)    30449 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/locale/pt_BR/LC_MESSAGES/django.mo
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/crm/locale/de/
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalixcrm/crm/locale/de/LC_MESSAGES/
--rw-r--r--   0 jenkins    (112) jenkins    (116)    45333 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0 jenkins    (112) jenkins    (116)    20733 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/crm/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 jenkins    (112) jenkins    (116)       55 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/koalixcrm/version.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      492 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/MANIFEST.in
--rw-r--r--   0 jenkins    (112) jenkins    (116)     3123 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/README.md
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalix_crm.egg-info/
--rw-r--r--   0 jenkins    (112) jenkins    (116)      271 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalix_crm.egg-info/requires.txt
--rw-r--r--   0 jenkins    (112) jenkins    (116)        1 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalix_crm.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (112) jenkins    (116)      480 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalix_crm.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (112) jenkins    (116)        1 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalix_crm.egg-info/not-zip-safe
--rw-r--r--   0 jenkins    (112) jenkins    (116)    18113 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalix_crm.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (112) jenkins    (116)       26 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/koalix_crm.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (112) jenkins    (116)      480 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/PKG-INFO
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/projectsettings/
-drwxr-xr-x   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/projectsettings/settings/
--rw-r--r--   0 jenkins    (112) jenkins    (116)      469 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/projectsettings/settings/development_sqlite_settings.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      451 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/projectsettings/settings/development_sqlite_settings_linux.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)        0 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/projectsettings/settings/__init__.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)     4055 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/projectsettings/settings/base_settings.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      508 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/projectsettings/settings/production_settings.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      676 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/projectsettings/settings/heroku_settings.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      589 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/projectsettings/settings/docker_production_settings.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      509 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/projectsettings/settings/docker_development_settings.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)      461 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/projectsettings/settings/development_settings.py
--rw-r--r--   0 jenkins    (112) jenkins    (116)       38 2020-03-28 17:08:48.000000 koalix-crm-1.13.dev9/setup.cfg
--rw-r--r--   0 jenkins    (112) jenkins    (116)     1433 2020-03-28 17:00:31.000000 koalix-crm-1.13.dev9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.091992 koalix-crm-1.14.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4115 2024-04-06 11:47:58.091992 koalix-crm-1.14.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.091992 koalix-crm-1.14.0rc1/koalix_crm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4115 2024-04-06 11:47:57.000000 koalix-crm-1.14.0rc1/koalix_crm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    18178 2024-04-06 11:47:58.000000 koalix-crm-1.14.0rc1/koalix_crm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 11:47:57.000000 koalix-crm-1.14.0rc1/koalix_crm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 11:47:57.000000 koalix-crm-1.14.0rc1/koalix_crm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-06 11:47:57.000000 koalix-crm-1.14.0rc1/koalix_crm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-06 11:47:57.000000 koalix-crm-1.14.0rc1/koalix_crm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.019991 koalix-crm-1.14.0rc1/koalixcrm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.019991 koalix-crm-1.14.0rc1/koalixcrm/accounting/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/accounting/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.023991 koalix-crm-1.14.0rc1/koalixcrm/accounting/accounting/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/accounting/accounting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8814 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/accounting/accounting/account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11362 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/accounting/accounting/accounting_period.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3451 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/accounting/accounting/booking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/accounting/accounting/product_category.py
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/accounting/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.023991 koalix-crm-1.14.0rc1/koalixcrm/accounting/const/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/accounting/const/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/accounting/const/accountTypeChoices.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/accounting/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.023991 koalix-crm-1.14.0rc1/koalixcrm/accounting/factories/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/accounting/factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/accounting/factories/factory_product_category.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.011991 koalix-crm-1.14.0rc1/koalixcrm/accounting/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.011991 koalix-crm-1.14.0rc1/koalixcrm/accounting/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.023991 koalix-crm-1.14.0rc1/koalixcrm/accounting/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/accounting/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     6010 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/accounting/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.011991 koalix-crm-1.14.0rc1/koalixcrm/accounting/locale/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.023991 koalix-crm-1.14.0rc1/koalixcrm/accounting/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     4242 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/accounting/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     7519 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/accounting/locale/pt_BR/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.023991 koalix-crm-1.14.0rc1/koalixcrm/accounting/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/accounting/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.023991 koalix-crm-1.14.0rc1/koalixcrm/accounting/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/accounting/management/commands/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.023991 koalix-crm-1.14.0rc1/koalixcrm/accounting/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     4451 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/accounting/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/accounting/migrations/0002_auto_20170705_1702.py
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/accounting/migrations/0003_remove_account_originalamount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6786 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/accounting/migrations/0004_auto_20171009_1949.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6726 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/accounting/migrations/0005_auto_20171110_1732.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/accounting/migrations/0006_auto_20180422_2048.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/accounting/migrations/0007_auto_20180422_2105.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/accounting/migrations/0008_auto_20181012_2056.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/accounting/migrations/0009_auto_20181012_2056.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/accounting/migrations/0010_auto_20181216_2224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/accounting/migrations/0011_auto_20240329_2207.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/accounting/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/accounting/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.027991 koalix-crm-1.14.0rc1/koalixcrm/accounting/rest/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/accounting/rest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/accounting/rest/account_rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/accounting/rest/accounting_period_rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5414 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/accounting/rest/booking_rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/accounting/rest/product_categorie_rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/accounting/rest/restinterface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.011991 koalix-crm-1.14.0rc1/koalixcrm/accounting/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.011991 koalix-crm-1.14.0rc1/koalixcrm/accounting/static/default_templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.027991 koalix-crm-1.14.0rc1/koalixcrm/accounting/static/default_templates/de/
+-rw-r--r--   0 runner    (1001) docker     (127)    10486 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/accounting/static/default_templates/de/balancesheet.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)    10401 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/accounting/static/default_templates/de/profitlossstatement.xsl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.027991 koalix-crm-1.14.0rc1/koalixcrm/accounting/static/default_templates/en/
+-rw-r--r--   0 runner    (1001) docker     (127)    11838 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/accounting/static/default_templates/en/balancesheet.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)    10746 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/accounting/static/default_templates/en/profitlossstatement.xsl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.027991 koalix-crm-1.14.0rc1/koalixcrm/accounting/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/accounting/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11709 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/accounting/tests/test_accountingModelTest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/accounting/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.027991 koalix-crm-1.14.0rc1/koalixcrm/crm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4447 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.027991 koalix-crm-1.14.0rc1/koalixcrm/crm/const/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/const/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10649 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/const/country.py
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/const/postaladdressprefix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/const/purpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/const/status.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.031991 koalix-crm-1.14.0rc1/koalixcrm/crm/contact/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/contact/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/contact/call.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10009 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/contact/contact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5278 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/contact/customer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/contact/customer_billing_cycle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/contact/customer_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/contact/email_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/contact/person.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/contact/phone_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/contact/postal_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/contact/supplier.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.031991 koalix-crm-1.14.0rc1/koalixcrm/crm/documents/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/documents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5323 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/documents/calculations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13508 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/documents/contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/documents/delivery_note.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9515 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/documents/invoice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/documents/payment_reminder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/documents/pdf_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/documents/purchase_confirmation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/documents/purchase_order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/documents/quote.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21527 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/documents/sales_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5776 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/documents/sales_document_position.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.039991 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_agreement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_agreement_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_agreement_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_contact.py
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_currency.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_currency_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_customer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_customer_billing_cycle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_customer_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_customer_group_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_delivery_note.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_estimation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_estimation_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_generic_project_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_generic_task_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_human_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_invoice.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_payment_reminder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_postal_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_product.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_product_price.py
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_product_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_project_link_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_project_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_purchase_confirmation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_purchase_order.py
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_quote.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_reporting_period.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_reporting_period_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_resource_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_resource_price.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_resource_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_sales_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_sales_document_position.py
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_task_link_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_task_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_tax.py
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_unit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_unit_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_work.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/inlinemixin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.011991 koalix-crm-1.14.0rc1/koalixcrm/crm/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.011991 koalix-crm-1.14.0rc1/koalixcrm/crm/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.039991 koalix-crm-1.14.0rc1/koalixcrm/crm/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    20733 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    45333 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.011991 koalix-crm-1.14.0rc1/koalixcrm/crm/locale/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.043991 koalix-crm-1.14.0rc1/koalixcrm/crm/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    30449 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    62091 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/locale/pt_BR/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.043991 koalix-crm-1.14.0rc1/koalixcrm/crm/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.043991 koalix-crm-1.14.0rc1/koalixcrm/crm/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4864 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/management/commands/koalixcrm_install_defaulttemplates.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.043991 koalix-crm-1.14.0rc1/koalixcrm/crm/middleware/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/middleware/timezoneMiddleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.055992 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)    53282 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0002_auto_20170927_2042.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42385 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0003_auto_20171009_1949.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2753 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0004_auto_20171009_2008.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41477 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0005_auto_20171110_1732.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4850 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0006_auto_20171210_1805.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0007_auto_20171210_2126.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0008_auto_20180104_2042.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6285 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0009_auto_20180104_2111.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0010_auto_20180104_2138.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0011_auto_20180104_2152.py
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0012_auto_20180105_1840.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0013_auto_20180105_2159.py
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0014_auto_20180108_2048.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7588 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0015_auto_20180111_2043.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0016_auto_20180111_2011.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0017_auto_20180111_2022.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0018_auto_20180111_2031.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0019_auto_20180112_2020.py
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0020_auto_20180116_2056.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0021_purchaseorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0022_auto_20180117_2020.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0023_auto_20180119_2102.py
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0024_auto_20180122_2121.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6072 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0025_auto_20180413_1937.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0026_auto_20180507_1957.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5968 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0027_auto_20180606_2034.py
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0028_auto_20180611_1835.py
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0029_auto_20180611_1903.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0030_auto_20180611_1930.py
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0031_auto_20180612_1924.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3366 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0032_auto_20180612_1925.py
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0033_auto_20180612_1936.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0034_genericprojectlink.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0035_auto_20180619_1924.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0036_auto_20180626_2059.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0037_auto_20180701_2128.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0038_auto_20180702_1628.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0039_auto_20180702_1635.py
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0040_auto_20180724_1657.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0041_auto_20180724_1657.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0042_auto_20180724_1816.py
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0043_reportingperiodstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0044_reportingperiod_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0045_auto_20180805_2047.py
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0046_auto_20180805_2051.py
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0047_work_worked_hours.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0048_auto_20181012_2056.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0049_auto_20181014_2258.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0050_auto_20181014_2300.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0051_auto_20181014_2302.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0052_auto_20181014_2304.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17512 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0053_auto_20181014_2305.py
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0054_auto_20181020_1845.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0055_auto_20181022_1937.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4572 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0056_auto_20181216_2224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0056_auto_20190102_2230.py
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0057_merge_20190106_1510.py
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0058_auto_20190401_2009.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7902 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0059_auto_20240329_2207.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.055992 koalix-crm-1.14.0rc1/koalixcrm/crm/product/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/product/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/product/currency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/product/currency_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/product/customer_group_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6501 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/product/price.py
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/product/product.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/product/product_price.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5913 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/product/product_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/product/tax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/product/unit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/product/unit_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.059991 koalix-crm-1.14.0rc1/koalixcrm/crm/reporting/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/reporting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/reporting/agreement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/reporting/agreement_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/reporting/agreement_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7290 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/reporting/estimation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/reporting/estimation_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/reporting/generic_project_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/reporting/generic_task_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13724 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/reporting/human_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26915 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/reporting/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/reporting/project_link_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/reporting/project_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11482 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/reporting/reporting_period.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/reporting/reporting_period_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/reporting/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/reporting/resource_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/reporting/resource_price.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/reporting/resource_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27719 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/reporting/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/reporting/task_link_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/reporting/task_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/reporting/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7931 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/reporting/work.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.063991 koalix-crm-1.14.0rc1/koalixcrm/crm/rest/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/rest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5956 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/rest/agreement_rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/rest/agreement_status_rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/rest/agreement_type_rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7180 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/rest/contact_rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/rest/currency_rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/rest/customer_billing_cycle_rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/rest/customer_group_rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/rest/customer_rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3711 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/rest/estimation_rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/rest/estimation_status_rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/rest/human_resource_rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/rest/product_rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5586 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/rest/project_rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/rest/project_status_rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3607 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/rest/reporting_period_rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/rest/reporting_period_status_rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/rest/resource_manager_rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4438 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/rest/resource_price_rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/rest/resource_rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/rest/resource_type_rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10754 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/rest/restinterface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/rest/task_rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/rest/task_status_rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/rest/tax_rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/rest/unit_rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/rest/work_rest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.015991 koalix-crm-1.14.0rc1/koalixcrm/crm/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.015991 koalix-crm-1.14.0rc1/koalixcrm/crm/static/default_templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.067992 koalix-crm-1.14.0rc1/koalixcrm/crm/static/default_templates/de/
+-rw-r--r--   0 runner    (1001) docker     (127)    50507 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/static/default_templates/de/deliveryorder.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)    50540 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/static/default_templates/de/invoice.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)    30645 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/static/default_templates/de/project_report.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)    50534 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/static/default_templates/de/purchaseconfirmation.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)    50629 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/static/default_templates/de/purchaseorder.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)    50629 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/static/default_templates/de/quote.xsl
+-rwxr-xr-x   0 runner    (1001) docker     (127)    27411 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/static/default_templates/de/work_report.xsl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.067992 koalix-crm-1.14.0rc1/koalixcrm/crm/static/default_templates/en/
+-rw-r--r--   0 runner    (1001) docker     (127)    50508 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/static/default_templates/en/deliveryorder.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)    50599 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/static/default_templates/en/invoice.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)    50534 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/static/default_templates/en/purchaseconfirmation.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)    50629 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/static/default_templates/en/purchaseorder.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)    50630 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/static/default_templates/en/quote.xsl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.071992 koalix-crm-1.14.0rc1/koalixcrm/crm/static/default_templates/generic/
+-rw-r--r--   0 runner    (1001) docker     (127)   704128 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/static/default_templates/generic/DejaVuSans-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   756072 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/static/default_templates/generic/DejaVuSans.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   122303 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/static/default_templates/generic/dejavusans-bold.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   156738 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/static/default_templates/generic/dejavusans.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/static/default_templates/generic/fontconfig.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    54101 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/static/default_templates/generic/logo.jpg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.015991 koalix-crm-1.14.0rc1/koalixcrm/crm/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.015991 koalix-crm-1.14.0rc1/koalixcrm/crm/templates/crm/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.071992 koalix-crm-1.14.0rc1/koalixcrm/crm/templates/crm/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/templates/crm/admin/create_work_report.html
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/templates/crm/admin/exception.html
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/templates/crm/admin/register_payment.html
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/templates/crm/admin/set_timezone.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5940 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/templates/crm/admin/time_reporting.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.075991 koalix-crm-1.14.0rc1/koalixcrm/crm/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16626 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_calculations_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4283 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_create_sales_document_from_contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6333 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_create_sales_document_from_invoice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5228 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_create_sales_document_from_quote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_create_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6894 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_delete_of_empty_row.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4363 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_incomplete_sales_document_position.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_project_admin_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5986 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_project_effective_costs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5670 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_project_planned_costs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_supplier_admin_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_task_constructor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5667 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_task_effective_costs_no_agreement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6510 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_task_effective_costs_with_agreement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5647 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_task_effective_duration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5120 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_task_effective_effort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3500 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_task_planned_costs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3260 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_task_planned_duration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3864 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_task_planned_effort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_task_update_last_status_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_time_tracking_add_row.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5535 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_user_is_not_human_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_version_increase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5833 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_view_work_entry_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6017 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_work_delete.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.079991 koalix-crm-1.14.0rc1/koalixcrm/crm/views/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5632 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/views/create_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/views/create_work_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/views/newdocument.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4599 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/views/pdfexport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/views/range_selection_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/views/renderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/views/reporting_period_missing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/views/set_timezone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/views/template_set_missing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4102 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/views/time_tracking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/views/user_extension_missing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/views/user_is_not_human_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6226 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/views/work_entry_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3957 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/views/work_entry_formset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.079991 koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.079991 koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/const/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/const/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/const/purpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.083992 koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/factories/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/factories/factory_document_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/factories/factory_template_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/factories/factory_user_extension.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.083992 koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.083992 koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/management/commands/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.083992 koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     9678 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6874 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/migrations/0002_auto_20171009_1949.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7474 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/migrations/0003_auto_20171110_1732.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10481 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/migrations/0004_auto_20171210_2126.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/migrations/0005_auto_20180612_1924.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/migrations/0006_auto_20180701_2128.py
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/migrations/0007_auto_20180702_1628.py
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/migrations/0008_auto_20240329_2207.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.083992 koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/rest/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/rest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3975 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/rest/document_template_rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16815 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/rest/template_set_rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/rest/user_extension_rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/rest/user_rest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.087992 koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/user_extension/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/user_extension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4473 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/user_extension/document_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5331 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/user_extension/template_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/user_extension/text_paragraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7410 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/user_extension/user_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/global_support_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.087992 koalix-crm-1.14.0rc1/koalixcrm/subscriptions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/subscriptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/subscriptions/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.087992 koalix-crm-1.14.0rc1/koalixcrm/subscriptions/const/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/subscriptions/const/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/subscriptions/const/events.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.015991 koalix-crm-1.14.0rc1/koalixcrm/subscriptions/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.015991 koalix-crm-1.14.0rc1/koalixcrm/subscriptions/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.087992 koalix-crm-1.14.0rc1/koalixcrm/subscriptions/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/subscriptions/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/subscriptions/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.015991 koalix-crm-1.14.0rc1/koalixcrm/subscriptions/locale/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.087992 koalix-crm-1.14.0rc1/koalixcrm/subscriptions/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/subscriptions/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/subscriptions/locale/pt_BR/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.087992 koalix-crm-1.14.0rc1/koalixcrm/subscriptions/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     3715 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/subscriptions/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3604 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/subscriptions/migrations/0002_auto_20171009_1949.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3603 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/subscriptions/migrations/0003_auto_20171110_1732.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6490 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/subscriptions/migrations/0004_auto_20181013_2213.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5735 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/subscriptions/migrations/0005_auto_20181013_2228.py
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/subscriptions/migrations/0006_auto_20240329_2207.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/subscriptions/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4466 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/subscriptions/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/subscriptions/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.087992 koalix-crm-1.14.0rc1/koalixcrm/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/test/UITests.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4473 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/test/test_support_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.015991 koalix-crm-1.14.0rc1/projectsettings/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.091992 koalix-crm-1.14.0rc1/projectsettings/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/projectsettings/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/projectsettings/settings/base_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/projectsettings/settings/development_docker_sqlite_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/projectsettings/settings/production_docker_postgres_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 11:47:58.091992 koalix-crm-1.14.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `koalix-crm-1.13.dev9/koalixcrm/global_support_functions.py` & `koalix-crm-1.14.0rc1/koalixcrm/global_support_functions.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/plugin.py` & `koalix-crm-1.14.0rc1/koalixcrm/plugin.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/subscriptions/admin.py` & `koalix-crm-1.14.0rc1/koalixcrm/subscriptions/admin.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 from django.contrib import admin
 from django.http import HttpResponseRedirect
-from django.utils.translation import ugettext as _
+from django.utils.translation import gettext as _
 from koalixcrm.subscriptions.models import *
 
 
 class AdminSubscriptionEvent(admin.TabularInline):
     model = SubscriptionEvent
     extra = 1
     classes = ('collapse-open',)
```

### Comparing `koalix-crm-1.13.dev9/koalixcrm/subscriptions/models.py` & `koalix-crm-1.14.0rc1/koalixcrm/subscriptions/models.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # -*- coding: utf-8 -*-
 
 from datetime import *
 from django.db import models
-from django.utils.translation import ugettext as _
+from django.utils.translation import gettext as _
 from filebrowser.fields import FileBrowseField
 from koalixcrm.subscriptions.const.events import *
 import koalixcrm.crm.documents
 
 
 class Subscription(models.Model):
+    id = models.BigAutoField(primary_key=True)
     contract = models.ForeignKey('crm.Contract', on_delete=models.CASCADE, verbose_name=_('Subscription Type'))
     subscription_type = models.ForeignKey('SubscriptionType', on_delete=models.CASCADE, verbose_name=_('Subscription Type'), null=True)
 
     def create_subscription_from_contract(self, contract):
         self.contract = contract
         self.save()
         return self
@@ -47,14 +48,15 @@
     class Meta:
         app_label = "subscriptions"
         verbose_name = _('Subscription')
         verbose_name_plural = _('Subscriptions')
 
 
 class SubscriptionEvent(models.Model):
+    id = models.BigAutoField(primary_key=True)
     subscriptions = models.ForeignKey('Subscription',
                                       on_delete=models.CASCADE,
                                       verbose_name=_('Subscription'))
     event_date = models.DateField(verbose_name=_("Event Date"),
                                   blank=True, null=True)
     event = models.CharField(max_length=1, choices=SUBSCRITIONEVENTS,
                              verbose_name=_('Event'))
@@ -65,14 +67,15 @@
     class Meta:
         app_label = "subscriptions"
         verbose_name = _('Subscription Event')
         verbose_name_plural = _('Subscription Events')
 
 
 class SubscriptionType(models.Model):
+    id = models.BigAutoField(primary_key=True)
     product_type = models.ForeignKey('crm.ProductType',
                                      verbose_name=_('Product Type'),
                                      on_delete=models.deletion.SET_NULL,
                                      null=True,
                                      blank=True)
     cancellation_period = models.IntegerField(verbose_name=_("Cancellation Period (months)"),
                                               blank=True,
```

### Comparing `koalix-crm-1.13.dev9/koalixcrm/subscriptions/migrations/0004_auto_20181013_2213.py` & `koalix-crm-1.14.0rc1/koalixcrm/subscriptions/migrations/0004_auto_20181013_2213.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/subscriptions/migrations/0001_initial.py` & `koalix-crm-1.14.0rc1/koalixcrm/subscriptions/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/subscriptions/migrations/0003_auto_20171110_1732.py` & `koalix-crm-1.14.0rc1/koalixcrm/subscriptions/migrations/0003_auto_20171110_1732.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/subscriptions/migrations/0002_auto_20171009_1949.py` & `koalix-crm-1.14.0rc1/koalixcrm/subscriptions/migrations/0002_auto_20171009_1949.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/subscriptions/migrations/0005_auto_20181013_2228.py` & `koalix-crm-1.14.0rc1/koalixcrm/subscriptions/migrations/0005_auto_20181013_2228.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/subscriptions/locale/pt_BR/LC_MESSAGES/django.po` & `koalix-crm-1.14.0rc1/koalixcrm/subscriptions/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/subscriptions/locale/pt_BR/LC_MESSAGES/django.mo` & `koalix-crm-1.14.0rc1/koalixcrm/subscriptions/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/subscriptions/locale/de/LC_MESSAGES/django.po` & `koalix-crm-1.14.0rc1/koalixcrm/subscriptions/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/subscriptions/locale/de/LC_MESSAGES/django.mo` & `koalix-crm-1.14.0rc1/koalixcrm/subscriptions/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/accounting/static/default_templates/en/profitlossstatement.xsl` & `koalix-crm-1.14.0rc1/koalixcrm/accounting/static/default_templates/en/profitlossstatement.xsl`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/accounting/static/default_templates/en/balancesheet.xsl` & `koalix-crm-1.14.0rc1/koalixcrm/accounting/static/default_templates/en/balancesheet.xsl`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/accounting/static/default_templates/de/profitlossstatement.xsl` & `koalix-crm-1.14.0rc1/koalixcrm/accounting/static/default_templates/de/profitlossstatement.xsl`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/accounting/static/default_templates/de/balancesheet.xsl` & `koalix-crm-1.14.0rc1/koalixcrm/accounting/static/default_templates/de/balancesheet.xsl`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/accounting/exceptions.py` & `koalix-crm-1.14.0rc1/koalixcrm/accounting/exceptions.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/accounting/views.py` & `koalix-crm-1.14.0rc1/koalixcrm/accounting/views.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from os import path
 from wsgiref.util import FileWrapper
 from django.http import Http404
 from django.http import HttpResponse
 from django.http import HttpResponseRedirect
 from koalixcrm.crm.exceptions import *
 from koalixcrm.djangoUserExtension.exceptions import *
-from django.utils.translation import ugettext as _
+from django.utils.translation import gettext as _
 
 
 def export_pdf(calling_model_admin, request, whereToCreateFrom, whatToCreate, redirectTo):
     """This method exports PDFs provided by different Models in the accounting application
 
         Args:
           calling_model_admin (ModelAdmin):  The calling ModelAdmin must be provided for error message response.
```

### Comparing `koalix-crm-1.13.dev9/koalixcrm/accounting/admin.py` & `koalix-crm-1.14.0rc1/koalixcrm/accounting/admin.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/accounting/rest/account_rest.py` & `koalix-crm-1.14.0rc1/koalixcrm/accounting/rest/account_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/accounting/rest/product_categorie_rest.py` & `koalix-crm-1.14.0rc1/koalixcrm/accounting/rest/product_categorie_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/accounting/rest/restinterface.py` & `koalix-crm-1.14.0rc1/koalixcrm/accounting/rest/restinterface.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/accounting/rest/booking_rest.py` & `koalix-crm-1.14.0rc1/koalixcrm/accounting/rest/booking_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/accounting/rest/accounting_period_rest.py` & `koalix-crm-1.14.0rc1/koalixcrm/accounting/rest/accounting_period_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/accounting/accounting/product_category.py` & `koalix-crm-1.14.0rc1/koalixcrm/accounting/accounting/product_category.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # -*- coding: utf-8 -*-
 from django.db import models
 from django.contrib import admin
-from django.utils.translation import ugettext as _
+from django.utils.translation import gettext as _
 from koalixcrm.accounting.models import Account
 
 
 class ProductCategory(models.Model):
+    id = models.BigAutoField(primary_key=True)
     title = models.CharField(verbose_name=_("Product Category Title"),
                              max_length=50)
     profit_account = models.ForeignKey(Account,
                                        on_delete=models.CASCADE,
                                        verbose_name=_("Profit Account"),
                                        limit_choices_to={"account_type": "E"},
                                        related_name="db_profit_account")
```

### Comparing `koalix-crm-1.13.dev9/koalixcrm/accounting/accounting/accounting_period.py` & `koalix-crm-1.14.0rc1/koalixcrm/accounting/accounting/accounting_period.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 # -*- coding: utf-8 -*-
 
 from datetime import *
 from django.db import models
 from django.contrib import admin
-from django.utils.translation import ugettext as _
+from django.utils.translation import gettext as _
 from django import forms
 from koalixcrm.accounting.models import Account
 from koalixcrm.crm.documents.pdf_export import PDFExport
 from koalixcrm.accounting.exceptions import AccountingPeriodNotFound
 from koalixcrm.accounting.exceptions import TemplateSetMissingInAccountingPeriod
 from koalixcrm.accounting.models import InlineBookings
 
 
 class AccountingPeriod(models.Model):
     """Accounting period represents the equivalent of the business logic element of a fiscal year
     the accounting period is referred in the booking and is used as a supporting object to generate
     balance sheets and profit/loss statements"""
+    id = models.BigAutoField(primary_key=True)
     title = models.CharField(max_length=200, verbose_name=_("Title"))  # For example "Year 2009", "1st Quarter 2009"
     begin = models.DateField(verbose_name=_("Begin"))
     end = models.DateField(verbose_name=_("End"))
     template_set_balance_sheet = models.ForeignKey("djangoUserExtension.DocumentTemplate",
                                                    on_delete=models.CASCADE,
                                                    verbose_name=_("Referred template for balance sheet"),
                                                    related_name='db_balancesheet_template_set',
```

### Comparing `koalix-crm-1.13.dev9/koalixcrm/accounting/accounting/account.py` & `koalix-crm-1.14.0rc1/koalixcrm/accounting/accounting/account.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # -*- coding: utf-8 -*-
 from django.db import models
 from django.contrib import admin
-from django.utils.translation import ugettext as _
+from django.utils.translation import gettext as _
 from django import forms
 
 from koalixcrm.accounting.const.accountTypeChoices import *
 from koalixcrm.accounting.exceptions import AccountingPeriodNotFound
 from koalixcrm.crm.documents.pdf_export import PDFExport
 
 
 class Account(models.Model):
+    id = models.BigAutoField(primary_key=True)
     account_number = models.IntegerField(verbose_name=_("Account Number"))
     title = models.CharField(verbose_name=_("Account Title"),
                              max_length=50)
     account_type = models.CharField(verbose_name=_("Account Type"),
                                     max_length=1,
                                     choices=ACCOUNTTYPECHOICES)
     description = models.TextField(verbose_name=_("Description"), null=True, blank=True)
```

### Comparing `koalix-crm-1.13.dev9/koalixcrm/accounting/accounting/booking.py` & `koalix-crm-1.14.0rc1/koalixcrm/accounting/accounting/booking.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # -*- coding: utf-8 -*-
 from django.contrib import admin
 from django.db import models
-from django.utils.translation import ugettext as _
+from django.utils.translation import gettext as _
 
 
 class Booking(models.Model):
+    id = models.BigAutoField(primary_key=True)
     from_account = models.ForeignKey('Account', on_delete=models.CASCADE, verbose_name=_("From Account"), related_name="db_booking_fromaccount")
     to_account = models.ForeignKey('Account', on_delete=models.CASCADE, verbose_name=_("To Account"), related_name="db_booking_toaccount")
     amount = models.DecimalField(max_digits=20, decimal_places=2, verbose_name=_("Amount"))
     description = models.CharField(verbose_name=_("Description"), max_length=120, null=True, blank=True)
     booking_reference = models.ForeignKey('crm.Invoice', on_delete=models.CASCADE, verbose_name=_("Booking Reference"), null=True, blank=True)
     booking_date = models.DateTimeField(verbose_name=_("Booking at"))
     accounting_period = models.ForeignKey('AccountingPeriod', on_delete=models.CASCADE, verbose_name=_("AccountingPeriod"))
```

### Comparing `koalix-crm-1.13.dev9/koalixcrm/accounting/migrations/0008_auto_20181012_2056.py` & `koalix-crm-1.14.0rc1/koalixcrm/accounting/migrations/0008_auto_20181012_2056.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/accounting/migrations/0001_initial.py` & `koalix-crm-1.14.0rc1/koalixcrm/accounting/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/accounting/migrations/0010_auto_20181216_2224.py` & `koalix-crm-1.14.0rc1/koalixcrm/accounting/migrations/0010_auto_20181216_2224.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/accounting/migrations/0007_auto_20180422_2105.py` & `koalix-crm-1.14.0rc1/koalixcrm/accounting/migrations/0007_auto_20180422_2105.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/accounting/migrations/0006_auto_20180422_2048.py` & `koalix-crm-1.14.0rc1/koalixcrm/accounting/migrations/0006_auto_20180422_2048.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/accounting/migrations/0005_auto_20171110_1732.py` & `koalix-crm-1.14.0rc1/koalixcrm/accounting/migrations/0005_auto_20171110_1732.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/accounting/migrations/0004_auto_20171009_1949.py` & `koalix-crm-1.14.0rc1/koalixcrm/accounting/migrations/0004_auto_20171009_1949.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/accounting/migrations/0002_auto_20170705_1702.py` & `koalix-crm-1.14.0rc1/koalixcrm/accounting/migrations/0002_auto_20170705_1702.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/accounting/migrations/0009_auto_20181012_2056.py` & `koalix-crm-1.14.0rc1/koalixcrm/accounting/migrations/0009_auto_20181012_2056.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/accounting/tests/test_accountingModelTest.py` & `koalix-crm-1.14.0rc1/koalixcrm/accounting/tests/test_accountingModelTest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/accounting/locale/pt_BR/LC_MESSAGES/django.po` & `koalix-crm-1.14.0rc1/koalixcrm/accounting/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/accounting/locale/pt_BR/LC_MESSAGES/django.mo` & `koalix-crm-1.14.0rc1/koalixcrm/accounting/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/accounting/locale/de/LC_MESSAGES/django.po` & `koalix-crm-1.14.0rc1/koalixcrm/accounting/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/accounting/locale/de/LC_MESSAGES/django.mo` & `koalix-crm-1.14.0rc1/koalixcrm/accounting/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/exceptions.py` & `koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/exceptions.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/user_extension/document_template.py` & `koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/user_extension/document_template.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 # -*- coding: utf-8 -*-
 
 from django.db import models
 from django.contrib import admin
-from django.utils.translation import ugettext as _
+from django.utils.translation import gettext as _
 
 from filebrowser.fields import FileBrowseField
 
 from koalixcrm.djangoUserExtension.user_extension.text_paragraph import InlineTextParagraph
 from koalixcrm.global_support_functions import xstr
 from koalixcrm.crm.exceptions import *
 
 
 class DocumentTemplate(models.Model):
+    id = models.BigAutoField(primary_key=True)
     title = models.CharField(verbose_name=_("Title"),
                              max_length=100,
                              blank=True,
                              null=True)
     xsl_file = FileBrowseField(verbose_name=_("XSL File"),
                                max_length=200)
     fop_config_file = FileBrowseField(verbose_name=_("FOP Configuration File"),
```

### Comparing `koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/user_extension/user_extension.py` & `koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/user_extension/user_extension.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 # -*- coding: utf-8 -*-
 
 from django.db import models
 from django.contrib import admin
-from django.utils.translation import ugettext as _
+from django.utils.translation import gettext as _
 
 from koalixcrm.crm.contact.postal_address import PostalAddress
 from koalixcrm.crm.contact.phone_address import PhoneAddress
 from koalixcrm.crm.contact.email_address import EmailAddress
 from koalixcrm.djangoUserExtension.const.purpose import *
 from koalixcrm.djangoUserExtension.exceptions import *
 from koalixcrm.global_support_functions import xstr
 
 
 class UserExtension(models.Model):
+    id = models.BigAutoField(primary_key=True)
     user = models.ForeignKey("auth.User",
                              on_delete=models.CASCADE,
                              blank=False,
                              null=False)
     default_template_set = models.ForeignKey("TemplateSet", on_delete=models.CASCADE)
     default_currency = models.ForeignKey("crm.Currency", on_delete=models.CASCADE)
```

### Comparing `koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/user_extension/text_paragraph.py` & `koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/user_extension/text_paragraph.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # -*- coding: utf-8 -*-
 
 from django.db import models
 from django.contrib import admin
-from django.utils.translation import ugettext as _
+from django.utils.translation import gettext as _
 
 from koalixcrm.crm.const.purpose import *
 
 
 class TextParagraphInDocumentTemplate(models.Model):
+    id = models.BigAutoField(primary_key=True)
     document_template = models.ForeignKey("djangoUserExtension.DocumentTemplate", on_delete=models.CASCADE)
     purpose = models.CharField(verbose_name=_("Purpose"), max_length=2, choices=PURPOSESTEXTPARAGRAPHINDOCUMENTS)
     text_paragraph = models.TextField(verbose_name=_("Text"), blank=False, null=False)
 
     class Meta:
         app_label = "crm"
         verbose_name = _('TextParagraphInDocumentTemplate')
```

### Comparing `koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/user_extension/template_set.py` & `koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/user_extension/template_set.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # -*- coding: utf-8 -*-
 
 from django.db import models
 from django.contrib import admin
-from django.utils.translation import ugettext as _
+from django.utils.translation import gettext as _
 
 from koalixcrm.global_support_functions import xstr
 from koalixcrm.crm.exceptions import *
 
 
 class TemplateSet(models.Model):
+    id = models.BigAutoField(primary_key=True)
     title = models.CharField(verbose_name=_("Title"),
                              max_length=100)
     invoice_template = models.ForeignKey("InvoiceTemplate",
                                          on_delete=models.CASCADE,
                                          blank=True,
                                          null=True)
     quote_template = models.ForeignKey("QuoteTemplate",
```

### Comparing `koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/admin.py` & `koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/admin.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/factories/factory_document_template.py` & `koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/factories/factory_document_template.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/factories/factory_user_extension.py` & `koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/factories/factory_user_extension.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/rest/template_set_rest.py` & `koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/rest/template_set_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/rest/user_extension_rest.py` & `koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/rest/user_extension_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/rest/document_template_rest.py` & `koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/rest/document_template_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/migrations/0001_initial.py` & `koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/migrations/0003_auto_20171110_1732.py` & `koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/migrations/0003_auto_20171110_1732.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/migrations/0005_auto_20180612_1924.py` & `koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/migrations/0005_auto_20180612_1924.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/migrations/0004_auto_20171210_2126.py` & `koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/migrations/0004_auto_20171210_2126.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/migrations/0007_auto_20180702_1628.py` & `koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/migrations/0007_auto_20180702_1628.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/migrations/0002_auto_20171009_1949.py` & `koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/migrations/0002_auto_20171009_1949.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/djangoUserExtension/migrations/0006_auto_20180701_2128.py` & `koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/migrations/0006_auto_20180701_2128.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/test_support_functions.py` & `koalix-crm-1.14.0rc1/koalixcrm/test/test_support_functions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 # -*- coding: utf-8 -*-
-
-from selenium.common.exceptions import NoSuchElementException
 import time
+from selenium.common.exceptions import NoSuchElementException
 from selenium.common.exceptions import TimeoutException
 from selenium.webdriver.support.ui import WebDriverWait
 from selenium.webdriver.support import expected_conditions
 from selenium.webdriver.common.by import By
 from selenium.webdriver.common.keys import Keys
 
 
-def assert_when_element_does_not_exist(testcase, xpath):
+def fail_when_element_does_not_exist(testcase, xpath):
     try:
-        testcase.selenium.find_element_by_xpath(xpath)
+        testcase.selenium.find_element('xpath', xpath)
     except NoSuchElementException:
-        testcase.assertTrue(True, xpath+" does not exist")
+        testcase.assertTrue(False, xpath+" should exist but it does not")
+        pass
 
 
-def assert_when_element_exists(testcase, xpath):
+def fail_when_element_exists(testcase, xpath):
     try:
-        testcase.selenium.find_element_by_xpath(xpath)
+        testcase.selenium.find_element('xpath', xpath)
+        testcase.assertTrue(False, xpath+" should not exist but it does")
     except NoSuchElementException:
-        testcase.assertTrue(True, xpath+" does exist")
-
+        pass
 
 def assert_when_element_is_not_equal_to(testcase, xpath, string):
     try:
-        element = testcase.selenium.find_element_by_xpath(xpath)
+        element = testcase.selenium.find_element('xpath', xpath)
         if element.text != string:
             print("issue")
     except NoSuchElementException:
         return
 
 
 def create_sales_document_from_reference(test_case,
@@ -39,50 +39,50 @@
                                          document_type,
                                          action_name,
                                          template_name,
                                          template_to_select):
     selenium = test_case.selenium
     selenium.get('%s%s' % (test_case.live_server_url, '/admin/crm/'+reference_type+'/'))
     time.sleep(1)
-    assert_when_element_does_not_exist(test_case,
+    fail_when_element_does_not_exist(test_case,
                                        '/html/body/div/article/div/form/section/div/table/tbody/tr/td[1]/input')
-    assert_when_element_does_not_exist(test_case, '/html/body/div/article/div/form/footer/ul/li/div/select')
-    assert_when_element_does_not_exist(test_case, '/html/body/div/article/div/form/footer/ul/li/div/button')
-    contract_1 = selenium.find_element_by_xpath(
+    fail_when_element_does_not_exist(test_case, '/html/body/div/article/div/form/footer/ul/li/div/select')
+    fail_when_element_does_not_exist(test_case, '/html/body/div/article/div/form/footer/ul/li/div/button')
+    contract_1 = selenium.find_element('xpath', 
         '/html/body/div/article/div/form/section/div/table/tbody/tr/td[1]/input')
     if not contract_1.is_selected():
         contract_1.send_keys(Keys.SPACE)
-    action_create_offer = selenium.find_element_by_xpath(
+    action_create_offer = selenium.find_element('xpath', 
         '/html/body/div/article/div/form/footer/ul/li/div/select/option[@value="'+action_name+'"]')
     action_create_offer.click()
-    ok_button = selenium.find_element_by_xpath('/html/body/div/article/div/form/footer/ul/li/div/button')
+    ok_button = selenium.find_element('xpath', '/html/body/div/article/div/form/footer/ul/li/div/button')
     ok_button.send_keys(Keys.RETURN)
     time.sleep(1)
     try:
         element_present = expected_conditions.presence_of_element_located((By.ID, 'id_title'))
         WebDriverWait(selenium, timeout).until(element_present)
     except TimeoutException:
         print("Timed out waiting for page to load")
-    assert_when_element_does_not_exist(test_case, '/html/body/div/article/ul/li')
-    document_type_template = selenium.find_element_by_xpath(
+    fail_when_element_does_not_exist(test_case, '/html/body/div/article/ul/li')
+    document_type_template = selenium.find_element('xpath', 
         '//*[@id="id_'+template_name+'"]/option[@value="' +
         template_to_select.id.__str__() + '"]')
     document_type_template.click()
-    save_button = selenium.find_element_by_xpath('/html/body/div/article/div/form/div/footer/ul/li[2]/input')
+    save_button = selenium.find_element('xpath', '/html/body/div/article/div/form/div/footer/ul/li[2]/input')
     save_button.send_keys(Keys.RETURN)
     time.sleep(1)
     selenium.get('%s%s' % (test_case.live_server_url, '/admin/crm/'+reference_type+'/'))
-    contract_1 = selenium.find_element_by_xpath(
+    contract_1 = selenium.find_element('xpath', 
         '/html/body/div/article/div/form/section/div/table/tbody/tr/td[1]/input')
     if not contract_1.is_selected():
         contract_1.send_keys(Keys.SPACE)
-    action_create_sales_document = selenium.find_element_by_xpath(
+    action_create_sales_document = selenium.find_element('xpath', 
         '/html/body/div/article/div/form/footer/ul/li/div/select/option[@value="'+action_name+'"]')
     action_create_sales_document.click()
-    ok_button = selenium.find_element_by_xpath('/html/body/div/article/div/form/footer/ul/li/div/button')
+    ok_button = selenium.find_element('xpath', '/html/body/div/article/div/form/footer/ul/li/div/button')
     ok_button.send_keys(Keys.RETURN)
     time.sleep(1)
     try:
         element_present = expected_conditions.presence_of_element_located((By.ID, 'id_title'))
         WebDriverWait(selenium, timeout).until(element_present)
     except TimeoutException:
         print("Timed out waiting for page to load")
```

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/templates/crm/admin/time_reporting.html` & `koalix-crm-1.14.0rc1/koalixcrm/crm/templates/crm/admin/time_reporting.html`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/templates/crm/admin/set_timezone.html` & `koalix-crm-1.14.0rc1/koalixcrm/crm/templates/crm/admin/set_timezone.html`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/templates/crm/admin/create_work_report.html` & `koalix-crm-1.14.0rc1/koalixcrm/crm/templates/crm/admin/create_work_report.html`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/templates/crm/admin/register_payment.html` & `koalix-crm-1.14.0rc1/koalixcrm/crm/templates/crm/admin/register_payment.html`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/templates/crm/admin/exception.html` & `koalix-crm-1.14.0rc1/koalixcrm/crm/templates/crm/admin/exception.html`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/static/default_templates/generic/logo.jpg` & `koalix-crm-1.14.0rc1/koalixcrm/crm/static/default_templates/generic/logo.jpg`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/static/default_templates/generic/dejavusans-bold.xml` & `koalix-crm-1.14.0rc1/koalixcrm/crm/static/default_templates/generic/dejavusans-bold.xml`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/static/default_templates/generic/fontconfig.xml` & `koalix-crm-1.14.0rc1/koalixcrm/crm/static/default_templates/generic/fontconfig.xml`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/static/default_templates/generic/DejaVuSans-Bold.ttf` & `koalix-crm-1.14.0rc1/koalixcrm/crm/static/default_templates/generic/DejaVuSans-Bold.ttf`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/static/default_templates/generic/DejaVuSans.ttf` & `koalix-crm-1.14.0rc1/koalixcrm/crm/static/default_templates/generic/DejaVuSans.ttf`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/static/default_templates/generic/dejavusans.xml` & `koalix-crm-1.14.0rc1/koalixcrm/crm/static/default_templates/generic/dejavusans.xml`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/static/default_templates/en/purchaseconfirmation.xsl` & `koalix-crm-1.14.0rc1/koalixcrm/crm/static/default_templates/en/purchaseconfirmation.xsl`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/static/default_templates/en/purchaseorder.xsl` & `koalix-crm-1.14.0rc1/koalixcrm/crm/static/default_templates/de/purchaseorder.xsl`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/static/default_templates/en/deliveryorder.xsl` & `koalix-crm-1.14.0rc1/koalixcrm/crm/static/default_templates/en/deliveryorder.xsl`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/static/default_templates/en/invoice.xsl` & `koalix-crm-1.14.0rc1/koalixcrm/crm/static/default_templates/en/invoice.xsl`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/static/default_templates/en/quote.xsl` & `koalix-crm-1.14.0rc1/koalixcrm/crm/static/default_templates/en/quote.xsl`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/static/default_templates/de/work_report.xsl` & `koalix-crm-1.14.0rc1/koalixcrm/crm/static/default_templates/de/work_report.xsl`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/static/default_templates/de/purchaseconfirmation.xsl` & `koalix-crm-1.14.0rc1/koalixcrm/crm/static/default_templates/de/purchaseconfirmation.xsl`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/static/default_templates/de/purchaseorder.xsl` & `koalix-crm-1.14.0rc1/koalixcrm/crm/static/default_templates/en/purchaseorder.xsl`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/static/default_templates/de/deliveryorder.xsl` & `koalix-crm-1.14.0rc1/koalixcrm/crm/static/default_templates/de/deliveryorder.xsl`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/static/default_templates/de/invoice.xsl` & `koalix-crm-1.14.0rc1/koalixcrm/crm/static/default_templates/de/invoice.xsl`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/static/default_templates/de/project_report.xsl` & `koalix-crm-1.14.0rc1/koalixcrm/crm/static/default_templates/de/project_report.xsl`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/static/default_templates/de/quote.xsl` & `koalix-crm-1.14.0rc1/koalixcrm/crm/static/default_templates/de/quote.xsl`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/reporting/task_status.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/reporting/task_status.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # -*- coding: utf-8 -*-
 
 from django.db import models
-from django.utils.translation import ugettext as _
+from django.utils.translation import gettext as _
 from django.contrib import admin
 from rest_framework import serializers
 
 
 class TaskStatus(models.Model):
+    id = models.BigAutoField(primary_key=True)
     title = models.CharField(verbose_name=_("Title"), max_length=250, blank=False, null=False)
     description = models.TextField(verbose_name=_("Text"), blank=True, null=True)
     is_done = models.BooleanField(verbose_name=_("Status represents task done"),)
 
     class Meta:
         app_label = "crm"
         verbose_name = _('Task Status')
```

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/reporting/generic_task_link.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/reporting/generic_task_link.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # -*- coding: utf-8 -*-
 
 from django.db import models
-from django.utils.translation import ugettext as _
+from django.utils.translation import gettext as _
 from django.contrib.contenttypes.fields import GenericForeignKey
 from django.contrib.contenttypes.models import ContentType
 from django.contrib import admin
 
 
 class GenericTaskLink(models.Model):
+    id = models.BigAutoField(primary_key=True)
     task = models.ForeignKey("Task",
                              on_delete=models.CASCADE,
                              verbose_name=_('Task'),
                              blank=False, null=False)
     task_link_type = models.ForeignKey("TaskLinkType",
                                        on_delete=models.CASCADE,
                                        verbose_name=_('Task Link Type'),
@@ -44,12 +45,12 @@
     readonly_fields = ('task_link_type',
                        'content_type',
                        'object_id',
                        'date_of_creation',
                        'last_modified_by')
     extra = 0
 
-    def has_add_permission(self, request):
+    def has_add_permission(self, request, obj=None):
         return False
 
     def has_delete_permission(self, request, obj=None):
         return False
```

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/reporting/generic_project_link.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/reporting/generic_project_link.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # -*- coding: utf-8 -*-
 
 from django.db import models
-from django.utils.translation import ugettext as _
+from django.utils.translation import gettext as _
 from django.contrib.contenttypes.fields import GenericForeignKey
 from django.contrib.contenttypes.models import ContentType
 from django.contrib import admin
 from django.contrib.contenttypes.admin import GenericTabularInline
 
 
 class GenericProjectLink(models.Model):
+    id = models.BigAutoField(primary_key=True)
     project = models.ForeignKey("Project",
                                 on_delete=models.CASCADE,
                                 verbose_name=_('Project'),
                                 blank=False,
                                 null=False)
     project_link_type = models.ForeignKey("ProjectLinkType",
                                           on_delete=models.CASCADE,
@@ -45,15 +46,15 @@
     readonly_fields = ('project_link_type',
                        'content_type',
                        'object_id',
                        'date_of_creation',
                        'last_modified_by')
     extra = 0
 
-    def has_add_permission(self, request):
+    def has_add_permission(self, request, obj=None):
         return False
 
     def has_delete_permission(self, request, obj=None):
         return False
 
 
 class InlineGenericProjectLink(GenericTabularInline):
@@ -61,12 +62,12 @@
     readonly_fields = ('project_link_type',
                        'content_type',
                        'object_id',
                        'date_of_creation',
                        'last_modified_by')
     extra = 0
 
-    def has_add_permission(self, request):
+    def has_add_permission(self, request, obj=None):
         return False
 
     def has_delete_permission(self, request, obj=None):
         return False
```

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/reporting/work.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/reporting/work.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 # -*- coding: utf-8 -*-
 
 from django.db import models
 from django.forms import ValidationError
 from django.contrib import admin
 from django.utils.html import format_html
-from django.utils.translation import ugettext as _
+from django.utils.translation import gettext as _
 from koalixcrm.crm.documents.pdf_export import PDFExport
 from koalixcrm.global_support_functions import *
 from koalixcrm.crm.exceptions import ReportingPeriodDoneDeleteNotPossible
 from django.contrib import messages
 
 
 class Work(models.Model):
+    id = models.BigAutoField(primary_key=True)
     human_resource = models.ForeignKey("HumanResource", on_delete=models.CASCADE)
     date = models.DateField(verbose_name=_("Date"),
                             blank=False,
                             null=False)
     start_time = models.DateTimeField(verbose_name=_("Start Time"),
                                       blank=True,
                                       null=True)
```

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/reporting/resource.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/reporting/resource.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # -*- coding: utf-8 -*-
 
 from django.db import models
-from django.utils.translation import ugettext as _
+from django.utils.translation import gettext as _
 
 
 class Resource(models.Model):
+    id = models.BigAutoField(primary_key=True)
     resource_manager = models.ForeignKey("ResourceManager",
                                          on_delete=models.CASCADE,
                                          verbose_name=_("Manager"),
                                          blank=True,
                                          null=True)
     resource_type = models.ForeignKey("ResourceType",
                                       on_delete=models.CASCADE,
```

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/reporting/estimation_status.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/reporting/estimation_status.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # -*- coding: utf-8 -*-
 
 from django.db import models
-from django.utils.translation import ugettext as _
+from django.utils.translation import gettext as _
 from django.contrib import admin
 from rest_framework import serializers
 
 
 class EstimationStatus(models.Model):
+    id = models.BigAutoField(primary_key=True)
     title = models.CharField(verbose_name=_("Title"),
                              max_length=250,
                              blank=False,
                              null=False)
     description = models.TextField(verbose_name=_("Text"),
                                    blank=True,
                                    null=True)
```

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/reporting/agreement_status.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/reporting/agreement_type.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,49 +1,33 @@
 # -*- coding: utf-8 -*-
 
 from django.db import models
-from django.utils.translation import ugettext as _
+from django.utils.translation import gettext as _
 from django.contrib import admin
-from rest_framework import serializers
 
 
-class AgreementStatus(models.Model):
-    title = models.CharField(verbose_name=_("Title"),
-                             max_length=250,
-                             blank=False,
-                             null=False)
-    description = models.TextField(verbose_name=_("Text"),
-                                   blank=True,
-                                   null=True)
-    is_agreed = models.BooleanField(verbose_name=_("Status represents agreement exists"),)
+class AgreementType(models.Model):
+    id = models.BigAutoField(primary_key=True)
+    title = models.CharField(verbose_name=_("Title"), max_length=300, blank=False, null=False)
+    description = models.TextField(verbose_name=_("Text"), blank=True, null=True)
 
     class Meta:
         app_label = "crm"
-        verbose_name = _('Agreement Status')
-        verbose_name_plural = _('Agreement Status')
+        verbose_name = _('Agreement Type')
+        verbose_name_plural = _('Agreement Type')
 
     def __str__(self):
         return str(self.id) + " " + str(self.title)
 
 
-class AgreementStatusAdminView(admin.ModelAdmin):
+class AgreementTypeAdminView(admin.ModelAdmin):
     list_display = ('id',
                     'title',
-                    'description',
-                    'is_agreed')
+                    'description')
 
     fieldsets = (
-        (_('Agreement Status'), {
+        (_('AgreementType'), {
             'fields': ('title',
-                       'description',
-                       'is_agreed')
+                       'description')
         }),
     )
     save_as = True
-
-
-class AgreementStatusJSONSerializer(serializers.HyperlinkedModelSerializer):
-    class Meta:
-        model = AgreementStatus
-        fields = ('id',
-                  'title',
-                  'description',)
```

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/reporting/project.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/reporting/project.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,28 +2,29 @@
 
 import os
 from decimal import *
 from datetime import *
 from django.conf import settings
 from django.db import models
 from django.contrib import admin
-from django.utils.translation import ugettext as _
+from django.utils.translation import gettext as _
 from django.utils.html import format_html
 from koalixcrm.crm.reporting.generic_project_link import GenericLinkInlineAdminView
 from koalixcrm.crm.reporting.reporting_period import ReportingPeriodInlineAdminView, ReportingPeriod
 from koalixcrm.crm.reporting.task import TaskInlineAdminView
 from koalixcrm.crm.documents.pdf_export import PDFExport
 from koalixcrm.crm.exceptions import TemplateSetMissingInContract
 from koalixcrm.crm.models import Task
 import matplotlib.dates as mdates
 from matplotlib import pyplot
 import pandas
 
 
 class Project(models.Model):
+    id = models.BigAutoField(primary_key=True)
     project_manager = models.ForeignKey('auth.User', on_delete=models.CASCADE, limit_choices_to={'is_staff': True},
                                         verbose_name=_("Staff"),
                                         related_name="db_rel_project_staff",
                                         blank=True,
                                         null=True)
     project_name = models.CharField(verbose_name=_("Project name"),
                                     max_length=100,
```

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/reporting/agreement.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/reporting/agreement.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # -*- coding: utf-8 -*-
 
 from django.db import models
 from django.contrib import admin
-from django.utils.translation import ugettext as _
+from django.utils.translation import gettext as _
 from koalixcrm.crm.reporting.resource_price import ResourcePrice
 
 
 class Agreement(models.Model):
     """The Agreement describes the contract between the steer-co or the customer with the project manager"""
+    id = models.BigAutoField(primary_key=True)
     task = models.ForeignKey("Task",
                              on_delete=models.CASCADE,
                              verbose_name=_('Task'),
                              blank=False,
                              null=False)
     resource = models.ForeignKey("Resource", on_delete=models.CASCADE)
     unit = models.ForeignKey("Unit", on_delete=models.CASCADE)
```

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/reporting/reporting_period_status.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/reporting/project_status.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,53 +1,50 @@
 # -*- coding: utf-8 -*-
 
 from django.db import models
-from django.utils.translation import ugettext as _
+from django.utils.translation import gettext as _
 from django.contrib import admin
 from rest_framework import serializers
 
 
-class ReportingPeriodStatus(models.Model):
+class ProjectStatus(models.Model):
+    id = models.BigAutoField(primary_key=True)
     title = models.CharField(verbose_name=_("Title"),
                              max_length=250,
                              blank=False,
                              null=False)
     description = models.TextField(verbose_name=_("Text"),
                                    blank=True,
                                    null=True)
-    is_done = models.BooleanField(verbose_name=_("Status represents reporting period is closed"),)
+    is_done = models.BooleanField(verbose_name=_("Status represents project is done"),)
 
     class Meta:
         app_label = "crm"
-        verbose_name = _('Reporting Period Status')
-        verbose_name_plural = _('Reporting Period Status')
+        verbose_name = _('Project Status')
+        verbose_name_plural = _('Project Status')
 
     def __str__(self):
-        if self.title:
-            return str(self.title)
-        else:
-            return str(self.id)
+        return str(self.id) + " " + str(self.title)
 
 
-class OptionReportingPeriodStatus(admin.ModelAdmin):
+class OptionProjectStatus(admin.ModelAdmin):
     list_display = ('id',
                     'title',
                     'description',
                     'is_done')
 
     fieldsets = (
-        (_('Task Status'), {
+        (_('Project Status'), {
             'fields': ('title',
                        'description',
                        'is_done')
         }),
     )
     save_as = True
 
 
-class TaskStatusJSONSerializer(serializers.HyperlinkedModelSerializer):
+class ProjectStatusJSONSerializer(serializers.HyperlinkedModelSerializer):
     class Meta:
-        model = ReportingPeriodStatus
+        model = ProjectStatus
         fields = ('id',
                   'title',
-                  'description',
-                  'is_done')
+                  'description',)
```

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/reporting/resource_price.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/reporting/resource_price.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 
 from django.db import models
 from django.contrib import admin
-from django.utils.translation import ugettext as _
+from django.utils.translation import gettext as _
 from koalixcrm.crm.product.price import Price
 from koalixcrm.crm.reporting.resource import Resource
 
 
 class ResourcePrice(Price):
     resource = models.ForeignKey(Resource,
                                  on_delete=models.CASCADE,
```

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/reporting/agreement_type.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/reporting/resource_type.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,38 @@
 # -*- coding: utf-8 -*-
 
 from django.db import models
-from django.utils.translation import ugettext as _
+from django.utils.translation import gettext as _
 from django.contrib import admin
 
 
-class AgreementType(models.Model):
-    title = models.CharField(verbose_name=_("Title"), max_length=300, blank=False, null=False)
-    description = models.TextField(verbose_name=_("Text"), blank=True, null=True)
-
-    class Meta:
-        app_label = "crm"
-        verbose_name = _('Agreement Type')
-        verbose_name_plural = _('Agreement Type')
+class ResourceType(models.Model):
+    id = models.BigAutoField(primary_key=True)
+    title = models.CharField(verbose_name=_("Title"),
+                             max_length=300,
+                             blank=False,
+                             null=False)
+    description = models.TextField(verbose_name=_("Text"),
+                                   blank=True,
+                                   null=True)
 
     def __str__(self):
         return str(self.id) + " " + str(self.title)
 
+    class Meta:
+        app_label = "crm"
+        verbose_name = _('Resource Link Type')
+        verbose_name_plural = _('Resource Link Type')
+
 
-class AgreementTypeAdminView(admin.ModelAdmin):
+class ResourceTypeAdminView(admin.ModelAdmin):
     list_display = ('id',
                     'title',
                     'description')
 
     fieldsets = (
-        (_('AgreementType'), {
+        (_('ResourceType'), {
             'fields': ('title',
                        'description')
         }),
     )
     save_as = True
```

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/reporting/project_status.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/reporting/reporting_period_status.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,49 +1,54 @@
 # -*- coding: utf-8 -*-
 
 from django.db import models
-from django.utils.translation import ugettext as _
+from django.utils.translation import gettext as _
 from django.contrib import admin
 from rest_framework import serializers
 
 
-class ProjectStatus(models.Model):
+class ReportingPeriodStatus(models.Model):
+    id = models.BigAutoField(primary_key=True)
     title = models.CharField(verbose_name=_("Title"),
                              max_length=250,
                              blank=False,
                              null=False)
     description = models.TextField(verbose_name=_("Text"),
                                    blank=True,
                                    null=True)
-    is_done = models.BooleanField(verbose_name=_("Status represents project is done"),)
+    is_done = models.BooleanField(verbose_name=_("Status represents reporting period is closed"),)
 
     class Meta:
         app_label = "crm"
-        verbose_name = _('Project Status')
-        verbose_name_plural = _('Project Status')
+        verbose_name = _('Reporting Period Status')
+        verbose_name_plural = _('Reporting Period Status')
 
     def __str__(self):
-        return str(self.id) + " " + str(self.title)
+        if self.title:
+            return str(self.title)
+        else:
+            return str(self.id)
 
 
-class OptionProjectStatus(admin.ModelAdmin):
+class OptionReportingPeriodStatus(admin.ModelAdmin):
     list_display = ('id',
                     'title',
                     'description',
                     'is_done')
 
     fieldsets = (
-        (_('Project Status'), {
+        (_('Task Status'), {
             'fields': ('title',
                        'description',
                        'is_done')
         }),
     )
     save_as = True
 
 
-class ProjectStatusJSONSerializer(serializers.HyperlinkedModelSerializer):
+class TaskStatusJSONSerializer(serializers.HyperlinkedModelSerializer):
     class Meta:
-        model = ProjectStatus
+        model = ReportingPeriodStatus
         fields = ('id',
                   'title',
-                  'description',)
+                  'description',
+                  'is_done')
```

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/reporting/estimation.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/reporting/estimation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 
 from django.db import models
 from django.contrib import admin
-from django.utils.translation import ugettext as _
+from django.utils.translation import gettext as _
 from koalixcrm.crm.reporting.resource_price import ResourcePrice
 from decimal import *
 from django.core.exceptions import ValidationError
 from django.forms import BaseInlineFormSet
 from koalixcrm.crm.exceptions import ReportingPeriodNotFound
 
 
 class Estimation(models.Model):
     """The estimation describes the estimated amount of resources which is still required to finish a task
     the estimation is done within a reporting period that is not yet closed. The estimation is done only considering
     all effective efforts that was reported in the previous and closed reporting periods"""
-
+    id = models.BigAutoField(primary_key=True)
     task = models.ForeignKey("Task",
                              on_delete=models.CASCADE,
                              verbose_name=_('Task'),
                              blank=False,
                              null=False)
     resource = models.ForeignKey("Resource",
                                  on_delete=models.CASCADE)
```

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/reporting/urls.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/reporting/urls.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/reporting/task.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/reporting/task.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 
 from decimal import *
 from django.db import models
-from django.utils.translation import ugettext as _
+from django.utils.translation import gettext as _
 from django.contrib import admin
 from django.utils.html import format_html
 from koalixcrm.crm.reporting.agreement import Agreement
 from koalixcrm.crm.reporting.agreement import AgreementInlineAdminView
 from koalixcrm.crm.reporting.estimation import EstimationInlineAdminView
 from koalixcrm.crm.reporting.generic_task_link import InlineGenericTaskLink
 from koalixcrm.crm.reporting.work import WorkInlineAdminView, Work
@@ -17,14 +17,15 @@
 from koalixcrm.crm.exceptions import ReportingPeriodNotFound
 from rest_framework import serializers
 from koalixcrm import global_support_functions
 
 
 class Task(models.Model):
     """ The Task model"""
+    id = models.BigAutoField(primary_key=True)
     title = models.CharField(verbose_name=_("Title"),
                              max_length=100,
                              blank=True,
                              null=True)
     project = models.ForeignKey("Project",
                                 on_delete=models.CASCADE,
                                 verbose_name=_('Project'),
@@ -618,12 +619,12 @@
                        'effective_effort_overall',
                        'effective_costs_confirmed',
                        'effective_costs_not_confirmed')
         }),
     )
     extra = 1
 
-    def has_add_permission(self, request):
+    def has_add_permission(self, request, obj=None):
         return True
 
     def has_delete_permission(self, request, obj=None):
         return False
```

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/reporting/resource_type.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/reporting/task_link_type.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,33 @@
 # -*- coding: utf-8 -*-
 
 from django.db import models
-from django.utils.translation import ugettext as _
+from django.utils.translation import gettext as _
 from django.contrib import admin
 
 
-class ResourceType(models.Model):
-    title = models.CharField(verbose_name=_("Title"),
-                             max_length=300,
-                             blank=False,
-                             null=False)
-    description = models.TextField(verbose_name=_("Text"),
-                                   blank=True,
-                                   null=True)
-
-    def __str__(self):
-        return str(self.id) + " " + str(self.title)
+class TaskLinkType(models.Model):
+    id = models.BigAutoField(primary_key=True)
+    title = models.CharField(verbose_name=_("Title"), max_length=300, blank=False, null=False)
+    description = models.TextField(verbose_name=_("Text"), blank=True, null=True)
 
     class Meta:
         app_label = "crm"
-        verbose_name = _('Resource Link Type')
-        verbose_name_plural = _('Resource Link Type')
+        verbose_name = _('Task Link Type')
+        verbose_name_plural = _('Task Link Type')
+
+    def __str__(self):
+        return str(self.id) + " " + str(self.title)
 
 
-class ResourceTypeAdminView(admin.ModelAdmin):
+class OptionTaskLinkType(admin.ModelAdmin):
     list_display = ('id',
                     'title',
                     'description')
 
     fieldsets = (
-        (_('ResourceType'), {
+        (_('TaskLinkType'), {
             'fields': ('title',
                        'description')
         }),
     )
     save_as = True
```

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/reporting/resource_manager.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/reporting/resource_manager.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # -*- coding: utf-8 -*-
 
 from django.db import models
 from django.contrib import admin
 from koalixcrm.djangoUserExtension.user_extension.user_extension import UserExtension
-from django.utils.translation import ugettext as _
+from django.utils.translation import gettext as _
 
 
 class ResourceManager(models.Model):
+    id = models.BigAutoField(primary_key=True)
     user = models.ForeignKey(UserExtension,
                              on_delete=models.CASCADE,
                              verbose_name=_("User"))
 
 
 class ResourceManagerAdminView(admin.ModelAdmin):
     list_display = ('id',
```

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/reporting/project_link_type.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/reporting/project_link_type.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # -*- coding: utf-8 -*-
 
 from django.db import models
-from django.utils.translation import ugettext as _
+from django.utils.translation import gettext as _
 from django.contrib import admin
 
 
 class ProjectLinkType(models.Model):
+    id = models.BigAutoField(primary_key=True)
     title = models.CharField(verbose_name=_("Title"), max_length=300, blank=False, null=False)
     description = models.TextField(verbose_name=_("Text"), blank=True, null=True)
 
     class Meta:
         app_label = "crm"
         verbose_name = _('Project Link Type')
         verbose_name_plural = _('Project Link Type')
```

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/reporting/human_resource.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/reporting/human_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 import datetime
 from dateutil.relativedelta import *
 from django.db import models
 from django.contrib import admin
-from django.utils.translation import ugettext as _
+from django.utils.translation import gettext as _
 from koalixcrm.djangoUserExtension.user_extension.user_extension import UserExtension
 from koalixcrm.crm.reporting.resource import Resource
 from koalixcrm.crm.reporting.resource_price import ResourcePriceInlineAdminView
 from koalixcrm.crm.reporting.work import Work
 from koalixcrm.crm.documents.pdf_export import PDFExport
```

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/reporting/task_link_type.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/product/product_price.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,37 @@
 # -*- coding: utf-8 -*-
 
 from django.db import models
-from django.utils.translation import ugettext as _
 from django.contrib import admin
+from django.utils.translation import gettext as _
+from koalixcrm.crm.product.price import Price
 
 
-class TaskLinkType(models.Model):
-    title = models.CharField(verbose_name=_("Title"), max_length=300, blank=False, null=False)
-    description = models.TextField(verbose_name=_("Text"), blank=True, null=True)
-
-    class Meta:
-        app_label = "crm"
-        verbose_name = _('Task Link Type')
-        verbose_name_plural = _('Task Link Type')
+class ProductPrice(Price):
+    product_type = models.ForeignKey("ProductType",
+                                     on_delete=models.CASCADE,
+                                     verbose_name=_("Product Type"))
 
     def __str__(self):
-        return str(self.id) + " " + str(self.title)
+        return str(self.price) + " " + str(self.currency.short_name)
 
+    class Meta:
+        app_label = "crm"
+        verbose_name = _('Product Price')
+        verbose_name_plural = _('Product Prices')
 
-class OptionTaskLinkType(admin.ModelAdmin):
-    list_display = ('id',
-                    'title',
-                    'description')
 
+class ProductPriceInlineAdminView(admin.TabularInline):
+    model = ProductPrice
+    extra = 1
+    classes = ['collapse']
     fieldsets = (
-        (_('TaskLinkType'), {
-            'fields': ('title',
-                       'description')
+        ('', {
+            'fields': ('price',
+                       'currency',
+                       'unit',
+                       'valid_from',
+                       'valid_until',
+                       'customer_group')
         }),
     )
-    save_as = True
+    allow_add = True
```

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/reporting/reporting_period.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/reporting/reporting_period.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 # -*- coding: utf-8 -*-
 
 from datetime import *
 from django.db import models
 from django.contrib import admin
-from django.utils.translation import ugettext as _
+from django.utils.translation import gettext as _
 from koalixcrm.crm.documents.pdf_export import PDFExport
 from koalixcrm.crm.exceptions import ReportingPeriodNotFound
 from koalixcrm.crm.reporting.work import WorkInlineAdminView
 from rest_framework import serializers
 from django.core.exceptions import ValidationError
 from django.forms import ModelForm
 
 
 class ReportingPeriod(models.Model):
     """The reporting period is referred in the work, in the expenses and purchase orders, it is used as a
        supporting object to generate project reports"""
+    id = models.BigAutoField(primary_key=True)
     project = models.ForeignKey("Project",
                                 on_delete=models.CASCADE,
                                 verbose_name=_("Project"),
                                 blank=False,
                                 null=False)
     title = models.CharField(max_length=200,
                              verbose_name=_("Title"),
@@ -263,15 +264,15 @@
                        'title',
                        'begin',
                        'end',
                        'status')
         }),
     )
 
-    def has_add_permission(self, request):
+    def has_add_permission(self, request, obj=None):
         return False
 
     def has_delete_permission(self, request, obj=None):
         return False
 
 
 class ProjectJSONSerializer(serializers.HyperlinkedModelSerializer):
```

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/exceptions.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/exceptions.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/management/commands/koalixcrm_install_defaulttemplates.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/management/commands/koalixcrm_install_defaulttemplates.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from os import path
 
 from koalixcrm import crm
 from koalixcrm import djangoUserExtension
 from django.contrib.auth.models import User
 from django.core.management.base import BaseCommand
 from filebrowser.base import FileObject
-from django.utils.translation import ugettext as _
+from django.utils.translation import gettext as _
 from django.conf import settings
 
 DEFAULT_FILE = 'dashboard.py'
 
 
 class Command(BaseCommand):
     help = (
```

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/contact/customer.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/contact/customer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 from django.http import HttpResponseRedirect
 from django.db import models
 from django.contrib import admin
-from django.utils.translation import ugettext as _
+from django.utils.translation import gettext as _
 from koalixcrm.plugin import *
 from koalixcrm.crm.contact.contact import Contact, ContactCall, ContactVisit,\
     PeopleInlineAdmin, PostalAddressForContact, ContactPostalAddress, \
     ContactPhoneAddress, ContactEmailAddress, CityFilter, StateFilter
 from koalixcrm.crm.documents.contract import Contract
```

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/contact/customer_billing_cycle.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/contact/customer_billing_cycle.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # -*- coding: utf-8 -*-
 
 from django.db import models
 from django.contrib import admin
-from django.utils.translation import ugettext as _
+from django.utils.translation import gettext as _
 
 
 class CustomerBillingCycle(models.Model):
+    id = models.BigAutoField(primary_key=True)
     name = models.CharField(max_length=300,
                             verbose_name=_("Name"))
     time_to_payment_date = models.IntegerField(verbose_name=_("Days To Payment Date"))
     payment_reminder_time_to_payment = models.IntegerField(verbose_name=_("Payment Reminder, Days To Payment Date "))
 
     class Meta:
         app_label = "crm"
```

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/contact/person.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/contact/person.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # -*- coding: utf-8 -*-
 
 from django.db import models
-from django.utils.translation import ugettext as _
+from django.utils.translation import gettext as _
 from koalixcrm.crm.const.postaladdressprefix import *
 
 
 class Person(models.Model):
+    id = models.BigAutoField(primary_key=True)
     prefix = models.CharField(max_length=1,
                               choices=POSTALADDRESSPREFIX,
                               verbose_name=_("Prefix"),
                               blank=True,
                               null=True)
     name = models.CharField(max_length=100,
                             verbose_name=_("Name"),
```

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/contact/postal_address.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/contact/postal_address.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # -*- coding: utf-8 -*-
 
 from django.db import models
-from django.utils.translation import ugettext as _
+from django.utils.translation import gettext as _
 from koalixcrm.crm.const.country import *
 from koalixcrm.crm.const.postaladdressprefix import *
 
 
 class PostalAddress(models.Model):
+    id = models.BigAutoField(primary_key=True)
     prefix = models.CharField(max_length=1,
                               choices=POSTALADDRESSPREFIX,
                               verbose_name=_("Prefix"), blank=True,
                               null=True)
     name = models.CharField(max_length=100,
                             verbose_name=_("Name"),
                             blank=True,
```

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/contact/supplier.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/contact/supplier.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 
 from django.db import models
 from django.contrib import admin
-from django.utils.translation import ugettext as _
+from django.utils.translation import gettext as _
 from koalixcrm.crm.contact.contact import Contact
 from koalixcrm.crm.contact.contact import ContactPostalAddress
 from koalixcrm.crm.contact.contact import ContactPhoneAddress
 from koalixcrm.crm.contact.contact import ContactEmailAddress
 
 
 class Supplier(Contact):
```

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/contact/customer_group.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/contact/customer_group.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # -*- coding: utf-8 -*-
 
 from django.db import models
 from django.contrib import admin
-from django.utils.translation import ugettext as _
+from django.utils.translation import gettext as _
 
 
 class CustomerGroup(models.Model):
+    id = models.BigAutoField(primary_key=True)
     name = models.CharField(max_length=300)
 
     def __str__(self):
         return str(self.id) + ' ' + self.name
 
     class Meta:
         app_label = "crm"
```

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/contact/contact.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/contact/contact.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 # -*- coding: utf-8 -*-
 
 from django.contrib import admin
-from django.utils.translation import ugettext as _
+from django.utils.translation import gettext as _
 from koalixcrm.crm.contact.phone_address import PhoneAddress
 from koalixcrm.crm.contact.email_address import EmailAddress
 from koalixcrm.crm.contact.postal_address import PostalAddress
 from koalixcrm.crm.contact.call import Call
 from koalixcrm.crm.contact.person import *
 from koalixcrm.crm.const.purpose import *
 from koalixcrm.global_support_functions import xstr
 from koalixcrm.crm.inlinemixin import LimitedAdminInlineMixin
 
 
 class Contact(models.Model):
+    id = models.BigAutoField(primary_key=True)
     name = models.CharField(max_length=300,
                             verbose_name=_("Name"))
     date_of_creation = models.DateTimeField(verbose_name=_("Created at"),
                                             auto_now_add=True)
     last_modification = models.DateTimeField(verbose_name=_("Last modified"),
                                              auto_now=True)
     last_modified_by = models.ForeignKey('auth.User',
@@ -124,14 +125,15 @@
             'fields': ('email', 'purpose',)
         }),
     )
     allow_add = True
 
 
 class ContactPersonAssociation(models.Model):
+    id = models.BigAutoField(primary_key=True)
     contact = models.ForeignKey(Contact, on_delete=models.CASCADE, related_name='person_association', blank=True, null=True)
     person = models.ForeignKey(Person, on_delete=models.CASCADE, related_name='contact_association', blank=True, null=True)
 
     class Meta:
         app_label = "crm"
         verbose_name = _('Contacts')
         verbose_name_plural = _('Contacts')
```

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/contact/call.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/contact/call.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # -*- coding: utf-8 -*-
 
 from datetime import *
 from django.db import models
 from django.contrib import admin
-from django.utils.translation import ugettext as _
+from django.utils.translation import gettext as _
 from django.utils import timezone
 from koalixcrm.crm.const.status import *
 
 
 class Call(models.Model):
+    id = models.BigAutoField(primary_key=True)
     staff = models.ForeignKey('auth.User',
                               on_delete=models.CASCADE,
                               limit_choices_to={'is_staff': True},
                               verbose_name=_("Staff"),
                               related_name="db_relcallstaff",
                               blank=True,
                               null=True)
```

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/product/tax.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/product/tax.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # -*- coding: utf-8 -*-
 
 from django.db import models
 from django.contrib import admin
-from django.utils.translation import ugettext as _
+from django.utils.translation import gettext as _
 
 
 class Tax(models.Model):
+    id = models.BigAutoField(primary_key=True)
     tax_rate = models.DecimalField(max_digits=5,
                                    decimal_places=2,
                                    verbose_name=_("Taxrate in Percentage"))
     name = models.CharField(verbose_name=_("Taxname"),
                             max_length=100)
     account_activa = models.ForeignKey('accounting.Account',
                                        on_delete=models.CASCADE,
```

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/product/currency_transform.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/product/currency_transform.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # -*- coding: utf-8 -*-
 
 from django.db import models
 from django.contrib import admin
-from django.utils.translation import ugettext as _
+from django.utils.translation import gettext as _
 
 
 class CurrencyTransform(models.Model):
+    id = models.BigAutoField(primary_key=True)
     from_currency = models.ForeignKey('Currency',
                                       on_delete=models.CASCADE,
                                       blank=False,
                                       null=False,
                                       verbose_name=_("From Currency"),
                                       related_name="db_reltransformfromcurrency")
     to_currency = models.ForeignKey('Currency',
```

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/product/unit_transform.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/product/unit_transform.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # -*- coding: utf-8 -*-
 
 from django.db import models
 from django.contrib import admin
-from django.utils.translation import ugettext as _
+from django.utils.translation import gettext as _
 
 
 class UnitTransform(models.Model):
+    id = models.BigAutoField(primary_key=True)
     from_unit = models.ForeignKey('Unit',
                                   on_delete=models.CASCADE,
                                   verbose_name=_("From Unit"),
                                   blank=False,
                                   null=False,
                                   related_name="db_reltransfromfromunit")
     to_unit = models.ForeignKey('Unit',
```

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/product/product_type.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/product/product_type.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 # -*- coding: utf-8 -*-
 
 from django.contrib import admin
 from django.db import models
-from django.utils.translation import ugettext as _
+from django.utils.translation import gettext as _
 
 from koalixcrm.crm.product.product_price import ProductPrice
 from koalixcrm.crm.product.product_price import ProductPriceInlineAdminView
 from koalixcrm.crm.product.unit_transform import UnitTransformInlineAdminView
 from koalixcrm.crm.product.customer_group_transform import CustomerGroupTransformInlineAdminView
 from koalixcrm.crm.product.currency_transform import CurrencyTransformInlineAdminView
 
 
 class ProductType(models.Model):
+    id = models.BigAutoField(primary_key=True)
     description = models.TextField(verbose_name=_("Description"),
                                    null=True,
                                    blank=True)
     title = models.CharField(verbose_name=_("Title"),
                              max_length=200)
     product_type_identifier = models.CharField(verbose_name=_("Product Number"),
                                                max_length=200,
```

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/product/unit.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/product/unit.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # -*- coding: utf-8 -*-
 
 from django.db import models
 from django.contrib import admin
-from django.utils.translation import ugettext as _
+from django.utils.translation import gettext as _
 
 
 class Unit(models.Model):
+    id = models.BigAutoField(primary_key=True)
     description = models.CharField(verbose_name=_("Description"),
                                    max_length=100)
     short_name = models.CharField(verbose_name=_("Displayed Name After Quantity In The Position"),
                                   max_length=3)
     is_a_fraction_of = models.ForeignKey('self',
                                          on_delete=models.CASCADE,
                                          blank=True,
```

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/product/customer_group_transform.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/product/customer_group_transform.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # -*- coding: utf-8 -*-
 
 from django.db import models
 from django.contrib import admin
-from django.utils.translation import ugettext as _
+from django.utils.translation import gettext as _
 
 
 class CustomerGroupTransform(models.Model):
+    id = models.BigAutoField(primary_key=True)
     from_customer_group = models.ForeignKey('CustomerGroup',
                                             on_delete=models.CASCADE,
                                             verbose_name=_("From Customer Group"),
                                             related_name="db_reltransfromfromcustomergroup",
                                             blank=False,
                                             null=False)
     to_customer_group = models.ForeignKey('CustomerGroup',
```

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/product/currency.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/product/currency.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # -*- coding: utf-8 -*-
 
 from decimal import Decimal
 from django.db import models
 from django.contrib import admin
-from django.utils.translation import ugettext as _
+from django.utils.translation import gettext as _
 
 
 class Currency(models.Model):
+    id = models.BigAutoField(primary_key=True)
     description = models.CharField(verbose_name=_("Description"),
                                    max_length=100)
     short_name = models.CharField(verbose_name=_("Displayed Name After Prices"),
                                   max_length=3)
     rounding = models.DecimalField(max_digits=5,
                                    decimal_places=2,
                                    verbose_name=_("Rounding"),
```

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/product/price.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/product/price.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # -*- coding: utf-8 -*-
 
 from django.db import models
-from django.utils.translation import ugettext as _
+from django.utils.translation import gettext as _
 from koalixcrm.crm.product.currency import Currency
 from koalixcrm.crm.product.unit import Unit
 from koalixcrm.crm.contact.customer_group import CustomerGroup
 from koalixcrm.crm.product.unit_transform import UnitTransform
 from koalixcrm.crm.product.customer_group_transform import CustomerGroupTransform
 from koalixcrm.crm.product.currency_transform import CurrencyTransform
 
 
 class Price(models.Model):
+    id = models.BigAutoField(primary_key=True)
     unit = models.ForeignKey(Unit,
                              on_delete=models.CASCADE,
                              blank=False,
                              verbose_name=_("Unit"))
     currency = models.ForeignKey(Currency,
                                  on_delete=models.CASCADE,
                                  verbose_name='Currency',
```

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/admin.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/admin.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_reporting_period_status.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_reporting_period_status.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_agreement_status.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_agreement_status.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_project.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_project.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_sales_document_position.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_sales_document_position.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_currency.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_currency.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_customer_group_transform.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_customer_group_transform.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_unit_transform.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_unit_transform.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_human_resource.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_human_resource.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_sales_document.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_sales_document.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_customer.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_customer.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_contract.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_contract.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_generic_project_link.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_generic_project_link.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_agreement.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_agreement.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_currency_transform.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_currency_transform.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_project_link_type.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_project_link_type.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_task_link_type.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_task_link_type.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_resource.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_resource.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_estimation.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_estimation.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_generic_task_link.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_generic_task_link.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_resource_price.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_resource_price.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_estimation_status.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_estimation_status.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_work.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_work.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_task_status.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_task_status.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_task.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_task.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_product_type.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_product_type.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_reporting_period.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_reporting_period.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_user.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_user.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_unit.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_unit.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/factories/factory_product_price.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_product_price.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/views/pdfexport.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/views/pdfexport.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 from os import path
 from wsgiref.util import FileWrapper
 from subprocess import CalledProcessError
 from django.http import Http404
 from django.http import HttpResponse
 from django.http import HttpResponseRedirect
-from django.utils.translation import ugettext as _
+from django.utils.translation import gettext as _
 from koalixcrm.crm.exceptions import *
 from koalixcrm.djangoUserExtension.exceptions import *
 from django.contrib import messages
 
 
 class PDFExportView:
```

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/views/time_tracking.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/views/time_tracking.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 import datetime
 from django.http import HttpResponseRedirect, Http404
 from django.contrib import messages
 from django.shortcuts import render
-from django.utils.translation import ugettext as _
+from django.utils.translation import gettext as _
 from django.template.context_processors import csrf
 from django.contrib.auth.decorators import login_required
 from koalixcrm.djangoUserExtension.models import UserExtension
 from koalixcrm.crm.exceptions import ReportingPeriodNotFound
 from koalixcrm.crm.exceptions import UserIsNoHumanResource
 from koalixcrm.djangoUserExtension.exceptions import UserExtensionMissing, TooManyUserExtensionsAvailable
 from koalixcrm.crm.views.range_selection_form import RangeSelectionForm
```

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/views/user_extension_missing.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/views/user_extension_missing.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/views/work_entry_form.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/views/work_entry_form.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/views/create_work_report.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/views/create_work_report.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/views/template_set_missing.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/views/template_set_missing.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/views/user_is_not_human_resource.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/views/user_is_not_human_resource.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/views/create_task.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/views/create_task.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 from django.http import Http404
 from django.http import HttpResponseRedirect
 from django.shortcuts import render
 from django.core.exceptions import ObjectDoesNotExist
-from django.utils.translation import ugettext as _
+from django.utils.translation import gettext as _
 from django.contrib.contenttypes.models import ContentType
 from koalixcrm.crm.exceptions import *
 from koalixcrm.djangoUserExtension.exceptions import *
 from koalixcrm.crm.documents.sales_document import SalesDocument
 from koalixcrm.crm.documents.sales_document_position import SalesDocumentPosition
 from koalixcrm.crm.reporting.task import Task
 from koalixcrm.crm.reporting.generic_task_link import GenericTaskLink
```

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/views/reporting_period_missing.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/views/reporting_period_missing.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/views/range_selection_form.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/views/range_selection_form.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/views/newdocument.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/views/newdocument.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 from django.http import Http404
 from django.http import HttpResponseRedirect
-from django.utils.translation import ugettext as _
+from django.utils.translation import gettext as _
 from django.contrib import messages
 from koalixcrm.crm.exceptions import *
 
 
 class CreateNewDocumentView:
     def create_new_document(calling_model_admin, request, calling_model, requested_document_type, redirect_to):
         """This method exports PDFs provided by different Models in the crm application
```

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/views/renderer.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/views/renderer.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/views/work_entry_formset.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/views/work_entry_formset.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/models.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/models.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/rest/resource_manager_rest.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/rest/resource_manager_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/rest/unit_rest.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/rest/unit_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/rest/resource_type_rest.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/rest/resource_type_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/rest/project_rest.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/rest/project_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/rest/resource_rest.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/rest/resource_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/rest/contact_rest.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/rest/contact_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/rest/customer_rest.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/rest/customer_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/rest/agreement_status_rest.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/rest/agreement_status_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/rest/work_rest.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/rest/work_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/rest/estimation_rest.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/rest/estimation_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/rest/tax_rest.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/rest/tax_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/rest/customer_billing_cycle_rest.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/rest/customer_billing_cycle_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/rest/customer_group_rest.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/rest/customer_group_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/rest/task_status_rest.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/rest/task_status_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/rest/project_status_rest.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/rest/project_status_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/rest/product_rest.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/rest/product_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/rest/restinterface.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/rest/restinterface.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/rest/task_rest.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/rest/task_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/rest/agreement_rest.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/rest/agreement_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/rest/agreement_type_rest.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/rest/agreement_type_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/rest/estimation_status_rest.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/rest/estimation_status_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/rest/human_resource_rest.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/rest/human_resource_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/rest/resource_price_rest.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/rest/resource_price_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/rest/reporting_period_status_rest.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/rest/reporting_period_status_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/rest/reporting_period_rest.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/rest/reporting_period_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0036_auto_20180626_2059.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0036_auto_20180626_2059.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0029_auto_20180611_1903.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0029_auto_20180611_1903.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0008_auto_20180104_2042.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0008_auto_20180104_2042.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0044_reportingperiod_status.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0044_reportingperiod_status.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0039_auto_20180702_1635.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0039_auto_20180702_1635.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0047_work_worked_hours.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0047_work_worked_hours.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0015_auto_20180111_2043.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0015_auto_20180111_2043.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,19 +35,19 @@
         renamed_model.name = "SalesDocument"
         state.models["crm", "salesdocument"] = renamed_model
         # Repoint all fields pointing to the old model to the new one.
         old_model_tuple = "crm", "salescontract"
         old_remote_model = '%s.%s' % ("crm", "salescontract")
         new_remote_model = '%s.%s' % ("crm", "SalesDocument")
         to_reload = []
-        for (model_app_label, model_name), model_state in state.models.items():
+        for (model_app_label, model_name), model_state in list(state.models.items()):
             if model_name != "salescontract" and model_name != "salesdocument":
                 new_model_state = model_state
                 model_with_new_base = state.models[model_app_label, model_name]
-                for index, (name, field) in enumerate(model_state.fields):
+                for index, (name, field) in enumerate(model_state.fields.items()):
                     changed_field = None
                     remote_field = field.remote_field
                     if remote_field:
                         remote_model_tuple = self._get_model_tuple(
                             remote_field.model, model_app_label, model_name
                         )
                         if remote_model_tuple == old_model_tuple:
@@ -61,15 +61,15 @@
                             )
                             if through_model_tuple == old_model_tuple:
                                 if changed_field is None:
                                     changed_field = field.clone()
                                 changed_field.remote_field.through = new_remote_model
                     if changed_field:
                         new_model_state = model_state.clone()
-                        new_model_state.fields[index] = name, changed_field
+                        new_model_state.fields[name] = changed_field
                         model_changed = True
                         if old_remote_model in model_state.bases:
                             new_bases = []
                             for base in model_state.bases:
                                 if old_remote_model == base:
                                     new_bases.append(new_remote_model.lower())
                                     new_model_state.bases = tuple(new_bases)
```

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0025_auto_20180413_1937.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0025_auto_20180413_1937.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0048_auto_20181012_2056.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0048_auto_20181012_2056.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0001_initial.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0027_auto_20180606_2034.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0027_auto_20180606_2034.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0011_auto_20180104_2152.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0011_auto_20180104_2152.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0007_auto_20171210_2126.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0007_auto_20171210_2126.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0038_auto_20180702_1628.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0038_auto_20180702_1628.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0024_auto_20180122_2121.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0024_auto_20180122_2121.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0032_auto_20180612_1925.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0032_auto_20180612_1925.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0051_auto_20181014_2302.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0051_auto_20181014_2302.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0002_auto_20170927_2042.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0002_auto_20170927_2042.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0021_purchaseorder.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0021_purchaseorder.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0041_auto_20180724_1657.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0041_auto_20180724_1657.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0020_auto_20180116_2056.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0020_auto_20180116_2056.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0018_auto_20180111_2031.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0018_auto_20180111_2031.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,41 +2,46 @@
 # Generated by Django 1.11.4 on 2018-01-11 20:31
 from __future__ import unicode_literals
 
 from django.db import migrations
 
 
 class Migration(migrations.Migration):
-    atomic = False
+    atomic = True
 
     dependencies = [
         ('crm', '0017_auto_20180111_2022'),
     ]
 
     operations = [
         migrations.AlterModelOptions(
             name='textparagraphinsalesdocument',
             options={'verbose_name': 'Text Paragraph In Sales Document', 'verbose_name_plural': 'Text Paragraphs In Sales Documents'},
         ),
         migrations.RenameField(
-            model_name='deliverynote',
+            model_name='quote',
             old_name='salescontract_ptr',
             new_name='salesdocument_ptr',
         ),
         migrations.RenameField(
-            model_name='emailaddressforsalesdocument',
-            old_name='contract',
-            new_name='sales_document',
+            model_name='invoice',
+            old_name='salescontract_ptr',
+            new_name='salesdocument_ptr',
         ),
         migrations.RenameField(
-            model_name='invoice',
+            model_name='deliverynote',
             old_name='salescontract_ptr',
             new_name='salesdocument_ptr',
         ),
         migrations.RenameField(
+            model_name='emailaddressforsalesdocument',
+            old_name='contract',
+            new_name='sales_document',
+        ),
+        migrations.RenameField(
             model_name='paymentreminder',
             old_name='salescontract_ptr',
             new_name='salesdocument_ptr',
         ),
         migrations.RenameField(
             model_name='phoneaddressforsalesdocument',
             old_name='contract',
@@ -44,27 +49,22 @@
         ),
         migrations.RenameField(
             model_name='postaladdressforsalesdocument',
             old_name='contract',
             new_name='sales_document',
         ),
         migrations.RenameField(
-            model_name='purchaseconfirmation',
-            old_name='salescontract_ptr',
-            new_name='salesdocument_ptr',
-        ),
-        migrations.RenameField(
-            model_name='quote',
-            old_name='salescontract_ptr',
-            new_name='salesdocument_ptr',
-        ),
-        migrations.RenameField(
             model_name='salesdocumentposition',
             old_name='contract',
             new_name='sales_document',
         ),
         migrations.RenameField(
             model_name='textparagraphinsalesdocument',
             old_name='sales_contract',
             new_name='sales_document',
         ),
+        migrations.RenameField(
+            model_name='purchaseconfirmation',
+            old_name='salescontract_ptr',
+            new_name='salesdocument_ptr',
+        ),
     ]
```

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0017_auto_20180111_2022.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0017_auto_20180111_2022.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0056_auto_20181216_2224.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0056_auto_20181216_2224.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0028_auto_20180611_1835.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0028_auto_20180611_1835.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0022_auto_20180117_2020.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0022_auto_20180117_2020.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0005_auto_20171110_1732.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0005_auto_20171110_1732.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0012_auto_20180105_1840.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0012_auto_20180105_1840.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0052_auto_20181014_2304.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0052_auto_20181014_2304.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0006_auto_20171210_1805.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0006_auto_20171210_1805.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0004_auto_20171009_2008.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0004_auto_20171009_2008.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0050_auto_20181014_2300.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0050_auto_20181014_2300.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0016_auto_20180111_2011.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0016_auto_20180111_2011.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0045_auto_20180805_2047.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0045_auto_20180805_2047.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0035_auto_20180619_1924.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0035_auto_20180619_1924.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0026_auto_20180507_1957.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0026_auto_20180507_1957.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0040_auto_20180724_1657.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0040_auto_20180724_1657.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0014_auto_20180108_2048.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0014_auto_20180108_2048.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0055_auto_20181022_1937.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0055_auto_20181022_1937.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0053_auto_20181014_2305.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0053_auto_20181014_2305.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0009_auto_20180104_2111.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0009_auto_20180104_2111.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0056_auto_20190102_2230.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0056_auto_20190102_2230.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0013_auto_20180105_2159.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0013_auto_20180105_2159.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0034_genericprojectlink.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0034_genericprojectlink.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0003_auto_20171009_1949.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0003_auto_20171009_1949.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0049_auto_20181014_2258.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0049_auto_20181014_2258.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0033_auto_20180612_1936.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0033_auto_20180612_1936.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0042_auto_20180724_1816.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0042_auto_20180724_1816.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0019_auto_20180112_2020.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0019_auto_20180112_2020.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0031_auto_20180612_1924.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0031_auto_20180612_1924.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0030_auto_20180611_1930.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0030_auto_20180611_1930.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/migrations/0043_reportingperiodstatus.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0043_reportingperiodstatus.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_poject_admin_view.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_project_admin_view.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,55 +1,51 @@
 # -*- coding: utf-8 -*-
 import pytest
-from django.test import LiveServerTestCase
-from selenium import webdriver
-from selenium.common.exceptions import TimeoutException
-from selenium.webdriver.support.ui import WebDriverWait
+from koalixcrm.test.test_support_functions import *
+from koalixcrm.crm.factories.factory_user import AdminUserFactory
+from koalixcrm.test.UITests import UITests
 from selenium.webdriver.support import expected_conditions
 from selenium.webdriver.common.by import By
-from selenium.webdriver.common.keys import Keys
-from koalixcrm.crm.factories.factory_user import AdminUserFactory
 
 
-class TestProjectAdminView(LiveServerTestCase):
+class TestProjectAdminView(UITests):
 
     def setUp(self):
-        firefox_options = webdriver.firefox.options.Options()
-        firefox_options.set_headless(headless=True)
-        self.selenium = webdriver.Firefox(firefox_options=firefox_options)
+        super().setUp()
         self.test_user = AdminUserFactory.create()
 
     def tearDown(self):
-        self.selenium.quit()
+        super().tearDown()
 
     @pytest.mark.front_end_tests
     def test_project_admin(self):
         selenium = self.selenium
         # login
         selenium.get('%s%s' % (self.live_server_url, '/admin/crm/project/'))
         # the browser will be redirected to the login page
-        timeout = 5
+        timeout = 10
         try:
             element_present = expected_conditions.presence_of_element_located((By.ID, 'id_username'))
             WebDriverWait(selenium, timeout).until(element_present)
         except TimeoutException:
             print("Timed out waiting for page to load")
-        username = selenium.find_element_by_xpath('//*[@id="id_username"]')
-        password = selenium.find_element_by_xpath('//*[@id="id_password"]')
-        submit_button = selenium.find_element_by_xpath('/html/body/div/article/div/div/form/div/ul/li/input')
+        username = selenium.find_element('xpath', '//*[@id="id_username"]')
+        password = selenium.find_element('xpath', '//*[@id="id_password"]')
+        submit_button = selenium.find_element('xpath', '/html/body/div/article/div/div/form/div/ul/li/input')
         username.send_keys("admin")
         password.send_keys("admin")
-        submit_button.send_keys(Keys.RETURN)
+        time.sleep(5)
+        self.selenium.get('%s%s' % (self.live_server_url, '/admin/crm/project/'))
         try:
             element_present = expected_conditions.presence_of_element_located((By.ID,
                                                                                '/html/body/div/article/header/ul/li/a'))
             WebDriverWait(selenium, timeout).until(element_present)
         except TimeoutException:
             print("Timed out waiting for page to load")
         # find the form element
         selenium.get('%s%s' % (self.live_server_url, '/admin/crm/project/add'))
 
         try:
-            element_present = expected_conditions.presence_of_element_located((By.ID, '//*[@id="id_project_status"]'))
+            element_present = expected_conditions.presence_of_element_located((By.ID, 'id_project_status'))
             WebDriverWait(selenium, timeout).until(element_present)
         except TimeoutException:
             print("Timed out waiting for page to load")
```

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_work_delete.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_work_delete.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_user_is_not_human_resource.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_user_is_not_human_resource.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,68 +1,67 @@
 import pytest
-from django.test import LiveServerTestCase
-from selenium import webdriver
 from selenium.webdriver.support.ui import Select
-from koalixcrm.test_support_functions import *
+from koalixcrm.test.test_support_functions import *
+from koalixcrm.test.UITests import UITests
 from koalixcrm.crm.factories.factory_user import AdminUserFactory
 from koalixcrm.crm.factories.factory_customer import StandardCustomerFactory
 from koalixcrm.crm.factories.factory_customer_group import StandardCustomerGroupFactory
 from koalixcrm.crm.factories.factory_currency import StandardCurrencyFactory
 from koalixcrm.djangoUserExtension.factories.factory_user_extension import StandardUserExtensionFactory
 
 
-class TimeTrackingAddRow(LiveServerTestCase):
+class TimeTrackingAddRow(UITests):
 
     def setUp(self):
-        firefox_options = webdriver.firefox.options.Options()
-        firefox_options.set_headless(headless=True)
-        self.selenium = webdriver.Firefox(firefox_options=firefox_options)
+        super().setUp()
         self.test_user = AdminUserFactory.create()
         self.test_customer_group = StandardCustomerGroupFactory.create()
         self.test_customer = StandardCustomerFactory.create(is_member_of=(self.test_customer_group,))
         self.test_currency = StandardCurrencyFactory.create()
         self.test_user_extension = StandardUserExtensionFactory.create(user=self.test_user)
 
     def tearDown(self):
-        self.selenium.quit()
+        super().tearDown()
 
     @pytest.mark.front_end_tests
     def test_add_new_row(self):
         selenium = self.selenium
         # login
         selenium.get('%s%s' % (self.live_server_url, '/koalixcrm/crm/reporting/time_tracking/'))
         # the browser will be redirected to the login page
         timeout = 5
         try:
             element_present = expected_conditions.presence_of_element_located((By.ID, 'id_username'))
             WebDriverWait(selenium, timeout).until(element_present)
         except TimeoutException:
             print("Timed out waiting for page to load")
-        username = selenium.find_element_by_xpath('//*[@id="id_username"]')
-        password = selenium.find_element_by_xpath('//*[@id="id_password"]')
-        submit_button = selenium.find_element_by_xpath('/html/body/div/article/div/div/form/div/ul/li/input')
+        username = selenium.find_element('xpath', '//*[@id="id_username"]')
+        password = selenium.find_element('xpath', '//*[@id="id_password"]')
+        submit_button = selenium.find_element('xpath', '/html/body/div/article/div/div/form/div/ul/li/input')
         username.send_keys("admin")
         password.send_keys("admin")
         submit_button.send_keys(Keys.RETURN)
+        time.sleep(5)
+        selenium.get('%s%s' % (self.live_server_url, '/koalixcrm/crm/reporting/time_tracking/'))
         # after the login, the browser is redirected to the target url /koalixcrm/crm/reporting/time_tracking
         try:
             element_present = expected_conditions.presence_of_element_located((By.ID, 'id_next_steps'))
             WebDriverWait(selenium, timeout).until(element_present)
         except TimeoutException:
             print("Timed out waiting for page to load")
 
         # Because the user is not equipped with a corresponding human_resource, the user must receive an exception
         # screen giving im the possibility to select what he wants to do next
         # In this test_step it is checked whether the form contains the required fields. the test will then select
         # to return to the start page instead of defining a new human resource
 
-        assert_when_element_does_not_exist(self, '//*[@id="id_next_steps"]')
-        assert_when_element_does_not_exist(self, 'confirm_selection')
-        submit_button = selenium.find_element_by_xpath('/html/body/div/article/div/form/table/tbody/tr[3]/td/input[2]')
-        selection = Select(selenium.find_element_by_xpath('//*[@id="id_next_steps"]'))
+        fail_when_element_does_not_exist(self, '//*[@id="id_next_steps"]')
+        fail_when_element_does_not_exist(self, '//*[@name="confirm_selection"]')
+        submit_button = selenium.find_element('xpath', '/html/body/div/article/div/form/table/tbody/tr[3]/td/input[2]')
+        selection = Select(selenium.find_element('xpath', '//*[@id="id_next_steps"]'))
         selection.select_by_value("return_to_start")
         submit_button.send_keys(Keys.RETURN)
         try:
             element_present = expected_conditions.presence_of_element_located((By.ID, 'grp-content-title'))
             WebDriverWait(selenium, timeout).until(element_present)
         except TimeoutException:
             print("Timed out waiting for page to load")
@@ -75,18 +74,18 @@
 
         selenium.get('%s%s' % (self.live_server_url, '/koalixcrm/crm/reporting/time_tracking/'))
         try:
             element_present = expected_conditions.presence_of_element_located((By.ID, 'id_next_steps'))
             WebDriverWait(selenium, timeout).until(element_present)
         except TimeoutException:
             print("Timed out waiting for page to load")
-        assert_when_element_does_not_exist(self, '//*[@id="id_next_steps"]')
-        assert_when_element_does_not_exist(self, 'confirm_selection')
-        submit_button = selenium.find_element_by_xpath('/html/body/div/article/div/form/table/tbody/tr[3]/td/input[2]')
-        selection = Select(selenium.find_element_by_xpath('//*[@id="id_next_steps"]'))
+        fail_when_element_does_not_exist(self, '//*[@id="id_next_steps"]')
+        fail_when_element_does_not_exist(self, '//*[@name="confirm_selection"]')
+        submit_button = selenium.find_element('xpath', '/html/body/div/article/div/form/table/tbody/tr[3]/td/input[2]')
+        selection = Select(selenium.find_element('xpath', '//*[@id="id_next_steps"]'))
         selection.select_by_value("create_human_resource")
         submit_button.send_keys(Keys.RETURN)
         try:
             element_present = expected_conditions.presence_of_element_located((By.ID, 'grp-content-title'))
             WebDriverWait(selenium, timeout).until(element_present)
         except TimeoutException:
             print("Timed out waiting for page to load")
```

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_task_planned_costs.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_task_planned_costs.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_view_work_entry_form.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_delete_of_empty_row.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,110 +1,113 @@
 # -*- coding: utf-8 -*-
 import pytest
-import time
 import datetime
-from django.contrib.staticfiles.testing import StaticLiveServerTestCase
-from selenium import webdriver
-from selenium.common.exceptions import TimeoutException
-from selenium.webdriver.support.ui import WebDriverWait
-from selenium.webdriver.support import expected_conditions
-from selenium.webdriver.common.by import By
-from selenium.webdriver.common.keys import Keys
-from koalixcrm.test_support_functions import *
+from koalixcrm.test.test_support_functions import *
 from koalixcrm.crm.factories.factory_user import AdminUserFactory
 from koalixcrm.crm.factories.factory_customer import StandardCustomerFactory
 from koalixcrm.crm.factories.factory_customer_group import StandardCustomerGroupFactory
 from koalixcrm.crm.factories.factory_currency import StandardCurrencyFactory
 from koalixcrm.djangoUserExtension.factories.factory_user_extension import StandardUserExtensionFactory
 from koalixcrm.crm.factories.factory_reporting_period import StandardReportingPeriodFactory
 from koalixcrm.crm.factories.factory_task import StandardTaskFactory
 from koalixcrm.crm.reporting.work import Work
+from koalixcrm.test.UITests import UITests
+from selenium.webdriver.support import expected_conditions
+from selenium.webdriver.common.by import By
+from selenium.webdriver.common.keys import Keys
 from koalixcrm.crm.factories.factory_human_resource import StandardHumanResourceFactory
 
 
-class TimeTrackingWorkEntry(StaticLiveServerTestCase):
+class TimeTrackingWorkEntry(UITests):
 
-    @classmethod
-    def setUpClass(cls):
-        super(TimeTrackingWorkEntry, cls).setUpClass()
-        firefox_options = webdriver.firefox.options.Options()
-        firefox_options.set_headless(headless=True)
-        cls.selenium = webdriver.Firefox(firefox_options=firefox_options)
-        cls.selenium.implicitly_wait(10)
-        cls.test_user = AdminUserFactory.create()
-        cls.test_customer_group = StandardCustomerGroupFactory.create()
-        cls.test_customer = StandardCustomerFactory.create(is_member_of=(cls.test_customer_group,))
-        cls.test_currency = StandardCurrencyFactory.create()
-        cls.test_user_extension = StandardUserExtensionFactory.create(user=cls.test_user)
-        cls.test_human_resource = StandardHumanResourceFactory.create(user=cls.test_user_extension)
-        cls.test_customer_group = StandardCustomerGroupFactory.create()
-        cls.test_customer = StandardCustomerFactory.create(is_member_of=(cls.test_customer_group,))
-        cls.test_currency = StandardCurrencyFactory.create()
-        cls.test_reporting_period = StandardReportingPeriodFactory.create()
-        cls.test_1st_task = StandardTaskFactory.create(title="1st Test Task",
-                                                       project=cls.test_reporting_period.project,
-                                                       )
+    def setUp(self):
+        super().setUp()
+        self.test_user = AdminUserFactory.create()
+        self.test_customer_group = StandardCustomerGroupFactory.create()
+        self.test_customer = StandardCustomerFactory.create(is_member_of=(self.test_customer_group,))
+        self.test_user_extension = StandardUserExtensionFactory.create(user=self.test_user)
+        self.test_human_resource = StandardHumanResourceFactory.create(user=self.test_user_extension)
+        self.test_currency = StandardCurrencyFactory.create()
+        self.test_reporting_period = StandardReportingPeriodFactory.create()
+        self.test_1st_task = StandardTaskFactory.create(
+            title="1st Test Task",
+            project=self.test_reporting_period.project,)
 
-    @classmethod
-    def tearDownClass(cls):
-        cls.selenium.quit()
-        super(TimeTrackingWorkEntry, cls).tearDownClass()
+    def tearDown(self):
+        super().tearDown()
 
     @pytest.mark.front_end_tests
-    def test_registration_of_work(self):
-        selenium = self.selenium
+    def test_delete_of_new_blank_row(self):
         # login
-        selenium.get('%s%s' % (self.live_server_url, '/koalixcrm/crm/reporting/time_tracking/'))
+        self.selenium.get('%s%s' % (self.live_server_url, '/koalixcrm/crm/reporting/time_tracking/'))
         # the browser will be redirected to the login page
         timeout = 5
         try:
             element_present = expected_conditions.presence_of_element_located((By.ID, 'id_username'))
-            WebDriverWait(selenium, timeout).until(element_present)
+            WebDriverWait(self.selenium, timeout).until(element_present)
         except TimeoutException:
             print("Timed out waiting for page to load")
-        username = selenium.find_element_by_xpath('//*[@id="id_username"]')
-        password = selenium.find_element_by_xpath('//*[@id="id_password"]')
-        submit_button = selenium.find_element_by_xpath('/html/body/div/article/div/div/form/div/ul/li/input')
+        username = self.selenium.find_element('xpath', '//*[@id="id_username"]')
+        password = self.selenium.find_element('xpath', '//*[@id="id_password"]')
+        submit_button = self.selenium.find_element('xpath', '/html/body/div/article/div/div/form/div/ul/li/input')
         username.send_keys("admin")
         password.send_keys("admin")
         submit_button.send_keys(Keys.RETURN)
-        # after the login, the browser is redirected to the target url /koalixcrm/crm/reporting/time_tracking
+        time.sleep(5)
+        self.selenium.get('%s%s' % (self.live_server_url, '/koalixcrm/crm/reporting/time_tracking/'))
         try:
             element_present = expected_conditions.presence_of_element_located((By.ID, 'id_form-0-project'))
-            WebDriverWait(selenium, timeout).until(element_present)
+            WebDriverWait(self.selenium, timeout).until(element_present)
         except TimeoutException:
             print("Timed out waiting for page to load")
         # find the form element
-        assert_when_element_does_not_exist(self, '//*[@id="id_form-0-project"]')
-        assert_when_element_does_not_exist(self, '//*[@id="id_form-0-task"]')
-        assert_when_element_does_not_exist(self, '//*[@id="id_form-0-datetime_start_0]')
-        assert_when_element_does_not_exist(self, '//*[@id="id_form-0-datetime_stop_0"]')
-        assert_when_element_does_not_exist(self, '//*[@id="id_form-0-datetime_start_1]')
-        assert_when_element_does_not_exist(self, '//*[@id="id_form-0-datetime_stop_1"]')
-        assert_when_element_does_not_exist(self, '//*[@id="id_form-0-worked_hours"]')
-        assert_when_element_does_not_exist(self, '//*[@id="id_form-0-description"]')
-        assert_when_element_does_not_exist(self, 'save')
-        project = selenium.find_element_by_xpath('//*[@id="id_form-0-project"]')
-        datetime_start_date = selenium.find_element_by_xpath('//*[@id="id_form-0-datetime_start_0"]')
-        datetime_start_time = selenium.find_element_by_xpath('//*[@id="id_form-0-datetime_start_1"]')
-        datetime_stop_date = selenium.find_element_by_xpath('//*[@id="id_form-0-datetime_stop_0"]')
-        datetime_stop_time = selenium.find_element_by_xpath('//*[@id="id_form-0-datetime_stop_1"]')
-        description = selenium.find_element_by_xpath('//*[@id="id_form-0-description"]')
+        fail_when_element_does_not_exist(self, '//*[@id="id_form-0-project"]')
+        fail_when_element_does_not_exist(self, '//*[@id="id_form-0-task"]')
+        fail_when_element_does_not_exist(self, '//*[@id="id_form-0-datetime_start_0"]')
+        fail_when_element_does_not_exist(self, '//*[@id="id_form-0-datetime_stop_0"]')
+        fail_when_element_does_not_exist(self, '//*[@id="id_form-0-datetime_start_1"]')
+        fail_when_element_does_not_exist(self, '//*[@id="id_form-0-datetime_stop_1"]')
+        fail_when_element_does_not_exist(self, '//*[@id="id_form-0-worked_hours"]')
+        fail_when_element_does_not_exist(self, '//*[@id="id_form-0-description"]')
+        fail_when_element_does_not_exist(self, '//*[@name="save"]')
+        # check existence of a second form before pressing add more
+        fail_when_element_exists(self, '//*[@id="id_form-1-project"]')
+        add_more_button = self.selenium.find_element('xpath', '//*[@id="add_more"]')
+        add_more_button.send_keys(Keys.RETURN)
+        time.sleep(1)
+        # check existence of a second form after pressing add more
+        fail_when_element_does_not_exist(self, '//*[@id="id_form-1-project"]')
+        add_more_button = self.selenium.find_element('xpath', '//*[@id="add_more"]')
+        add_more_button.send_keys(Keys.RETURN)
+        delete_form = expected_conditions.presence_of_element_located((By.ID, 'id_form-1-DELETE'))
+        delete_checkbox = self.selenium.find_element(By.ID, 'id_form-1-DELETE')
+        if not delete_checkbox.is_selected():
+            delete_checkbox.send_keys(Keys.SPACE)
+        # check existence of a second form after pressing add more
+        fail_when_element_does_not_exist(self, '//*[@id="id_form-2-project"]')
+        project = self.selenium.find_element('xpath', '//*[@id="id_form-2-project"]')
+        datetime_start_date = self.selenium.find_element('xpath', '//*[@id="id_form-2-datetime_start_0"]')
+        datetime_start_time = self.selenium.find_element('xpath', '//*[@id="id_form-2-datetime_start_1"]')
+        datetime_stop_date = self.selenium.find_element('xpath', '//*[@id="id_form-2-datetime_stop_0"]')
+        datetime_stop_time = self.selenium.find_element('xpath', '//*[@id="id_form-2-datetime_stop_1"]')
+        description = self.selenium.find_element('xpath', '//*[@id="id_form-2-description"]')
         project.send_keys(self.test_reporting_period.project.id.__str__())
         datetime_start_date.send_keys(datetime.date.today().__str__())
         datetime_stop_date.send_keys(datetime.date.today().__str__())
         datetime_start_time.send_keys(datetime.time(11, 55).__str__())
         datetime_stop_time.send_keys(datetime.time(12, 55).__str__())
         description.send_keys("This is a test work entered through the front-end")
-        task = selenium.find_element_by_xpath('//*[@id="id_form-0-task"]/option[text()="'+self.test_1st_task.title+'"]')
+        task = self.selenium.find_element('xpath', '//*[@id="id_form-2-task"]/option[text()="'+self.test_1st_task.title+'"]')
         task.click()
-        save_button = selenium.find_element_by_name('save')
+        save_button = self.selenium.find_element('xpath', '//*[@name="save"]')
         save_button.send_keys(Keys.RETURN)
         time.sleep(1)
         try:
             element_present = expected_conditions.presence_of_element_located((By.ID, 'id_form-1-project'))
-            WebDriverWait(selenium, timeout).until(element_present)
+            WebDriverWait(self.selenium, timeout).until(element_present)
         except TimeoutException:
             print("Timed out waiting for page to load")
-        assert_when_element_does_not_exist(self, '//*[@id="id_form-1-task"]')
+        fail_when_element_does_not_exist(self, '//*[@id="id_form-1-task"]')
+        fail_when_element_exists(self, '//*[@id="id_form-2-task"]')
         work = Work.objects.get(description="This is a test work entered through the front-end")
         self.assertEqual(type(work), Work)
+        work.delete()
```

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_task_update_last_status_update.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_task_update_last_status_update.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_supplier_admin_view.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_supplier_admin_view.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,69 +1,68 @@
 # -*- coding: utf-8 -*-
 import pytest
-from django.test import LiveServerTestCase
-from selenium import webdriver
+from koalixcrm.test.test_support_functions import *
 from selenium.common.exceptions import TimeoutException
 from selenium.webdriver.support.ui import WebDriverWait
 from selenium.webdriver.support import expected_conditions
 from selenium.webdriver.common.by import By
 from selenium.webdriver.common.keys import Keys
 from koalixcrm.crm.factories.factory_user import AdminUserFactory
 from koalixcrm.crm.contact.supplier import Supplier
+from koalixcrm.test.UITests import UITests
 
 
-class TestSupplierAdminView(LiveServerTestCase):
+class TestSupplierAdminView(UITests):
 
     def setUp(self):
-        firefox_options = webdriver.firefox.options.Options()
-        firefox_options.set_headless(headless=True)
-        self.selenium = webdriver.Firefox(firefox_options=firefox_options)
+        super().setUp()
         self.test_user = AdminUserFactory.create()
 
     def tearDown(self):
-        self.selenium.quit()
+        super().tearDown()
 
     @pytest.mark.front_end_tests
     def test_supplier_admin(self):
-        selenium = self.selenium
         # login
-        selenium.get('%s%s' % (self.live_server_url, '/admin/crm/supplier/'))
+        self.selenium.get('%s%s' % (self.live_server_url, '/admin/crm/supplier/'))
         # the browser will be redirected to the login page
-        timeout = 5
+        timeout = 10
         try:
             element_present = expected_conditions.presence_of_element_located((By.ID, 'id_username'))
-            WebDriverWait(selenium, timeout).until(element_present)
+            WebDriverWait(self.selenium, timeout).until(element_present)
         except TimeoutException:
             print("Timed out waiting for page to load")
-        username = selenium.find_element_by_xpath('//*[@id="id_username"]')
-        password = selenium.find_element_by_xpath('//*[@id="id_password"]')
-        submit_button = selenium.find_element_by_xpath('/html/body/div/article/div/div/form/div/ul/li/input')
+        username = self.selenium.find_element('xpath', '//*[@id="id_username"]')
+        password = self.selenium.find_element('xpath', '//*[@id="id_password"]')
+        submit_button = self.selenium.find_element('xpath', '/html/body/div/article/div/div/form/div/ul/li/input')
         username.send_keys("admin")
         password.send_keys("admin")
         submit_button.send_keys(Keys.RETURN)
+        time.sleep(5)
+        self.selenium.get('%s%s' % (self.live_server_url, '/admin/crm/supplier/'))
         try:
             element_present = expected_conditions.presence_of_element_located((By.ID,
                                                                                '/html/body/div/article/header/ul/li/a'))
-            WebDriverWait(selenium, timeout).until(element_present)
+            WebDriverWait(self.selenium, timeout).until(element_present)
         except TimeoutException:
             print("Timed out waiting for page to load")
         # find the form element
-        selenium.get('%s%s' % (self.live_server_url, '/admin/crm/supplier/add'))
+        self.selenium.get('%s%s' % (self.live_server_url, '/admin/crm/supplier/add'))
 
         try:
-            element_present = expected_conditions.presence_of_element_located((By.ID, '//*[@id="id_name"]'))
-            WebDriverWait(selenium, timeout).until(element_present)
+            element_present = expected_conditions.presence_of_element_located((By.ID, 'id_name'))
+            WebDriverWait(self.selenium, timeout).until(element_present)
         except TimeoutException:
             print("Timed out waiting for page to load")
-        name = selenium.find_element_by_xpath('//*[@id="id_name"]')
+        name = self.selenium.find_element('xpath', '//*[@id="id_name"]')
         name.send_keys("This is the name of a supplier")
-        submit_button = selenium.find_element_by_xpath('/html/body/div/article/div/form/div/footer/ul/li[1]/input')
+        submit_button = self.selenium.find_element('xpath', '/html/body/div/article/div/form/div/footer/ul/li[1]/input')
         submit_button.send_keys(Keys.RETURN)
         try:
             element_present = expected_conditions.presence_of_element_located((By.ID,
                                                                                '/html/body/div/article/header/ul/li/a'))
-            WebDriverWait(selenium, timeout).until(element_present)
+            WebDriverWait(self.selenium, timeout).until(element_present)
         except TimeoutException:
             print("Timed out waiting for page to load")
         supplier = Supplier.objects.get(name="This is the name of a supplier")
         self.assertEqual(type(supplier), Supplier)
```

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_create_sales_document_from_contract.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_create_sales_document_from_quote.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 # -*- coding: utf-8 -*-
 import pytest
 import os
 from django.contrib.staticfiles.testing import StaticLiveServerTestCase
 from selenium import webdriver
-from koalixcrm.test_support_functions import *
+from koalixcrm.test.test_support_functions import *
 from koalixcrm.crm.factories.factory_contract import StandardContractFactory
+from koalixcrm.crm.factories.factory_quote import StandardQuoteFactory
 from koalixcrm.crm.factories.factory_user import AdminUserFactory
 from koalixcrm.crm.factories.factory_customer_group import StandardCustomerGroupFactory
 from koalixcrm.djangoUserExtension.factories.factory_document_template import StandardQuoteTemplateFactory
 from koalixcrm.djangoUserExtension.factories.factory_document_template import StandardInvoiceTemplateFactory
 from koalixcrm.djangoUserExtension.factories.factory_document_template import StandardPurchaseOrderTemplateFactory
 from koalixcrm.crm.documents.quote import Quote
 from koalixcrm.crm.documents.invoice import Invoice
 from koalixcrm.crm.documents.purchase_order import PurchaseOrder
 
 
 class CreateSalesDocumentFromContract(StaticLiveServerTestCase):
+
     @classmethod
     def setUpClass(cls):
         super(CreateSalesDocumentFromContract, cls).setUpClass()
         firefox_options = webdriver.firefox.options.Options()
-        firefox_options.set_headless(headless=True)
-        cls.selenium = webdriver.Firefox(firefox_options=firefox_options)
+        firefox_options.add_argument("--headless")
+        cls.selenium = webdriver.Firefox(options=firefox_options)
         cls.selenium.implicitly_wait(10)
         cls.test_user = AdminUserFactory.create()
         cls.test_customer_group = StandardCustomerGroupFactory.create()
         cls.test_contract = StandardContractFactory.create()
+        cls.test_quote = StandardQuoteFactory.create(contract=cls.test_contract)
         cls.test_quote_template = StandardQuoteTemplateFactory.create()
         cls.test_invoice_template = StandardInvoiceTemplateFactory.create()
         cls.test_purchase_order_template = StandardPurchaseOrderTemplateFactory.create()
 
     @classmethod
     def tearDownClass(cls):
         cls.selenium.quit()
@@ -40,28 +43,28 @@
             directory = os.getcwd() + "/test_results/Screenshots/"
             if not os.path.exists(directory):
                 os.makedirs(directory)
             self.selenium.save_screenshot(directory + "%s.png" % "test_name")
         super(CreateSalesDocumentFromContract, self).tearDown()
 
     @pytest.mark.front_end_tests
-    def test_create_sales_document_from_contract(self):
+    def test_create_sales_document_from_quote(self):
         selenium = self.selenium
         # login
-        selenium.get('%s%s' % (self.live_server_url, '/admin/crm/contract/'))
+        selenium.get('%s%s' % (self.live_server_url, '/admin/crm/quote/'))
         # the browser will be redirected to the login page
         timeout = 2
         try:
             element_present = expected_conditions.presence_of_element_located((By.ID, 'id_username'))
             WebDriverWait(selenium, timeout).until(element_present)
         except TimeoutException:
             print("Timed out waiting for page to load")
-        username = selenium.find_element_by_xpath('//*[@id="id_username"]')
-        password = selenium.find_element_by_xpath('//*[@id="id_password"]')
-        submit_button = selenium.find_element_by_xpath('/html/body/div/article/div/div/form/div/ul/li/input')
+        username = selenium.find_element('xpath', '//*[@id="id_username"]')
+        password = selenium.find_element('xpath', '//*[@id="id_password"]')
+        submit_button = selenium.find_element('xpath', '/html/body/div/article/div/div/form/div/ul/li/input')
         username.send_keys("admin")
         password.send_keys("admin")
         submit_button.send_keys(Keys.RETURN)
         # after the login, the browser is redirected to the target url /koalixcrm/crm/contract
         try:
             element_present = expected_conditions.presence_of_element_located((By.ID, 'id_form-0-project'))
             WebDriverWait(selenium, timeout).until(element_present)
@@ -72,19 +75,19 @@
                                    "template_name": "quote_template",
                                    "template_to_select": self.test_quote_template},
                            Invoice: {"action_name": "create_invoice",
                                      "template_name": "invoice_template",
                                      "template_to_select": self.test_invoice_template},
                            PurchaseOrder: {"action_name": "create_purchase_order",
                                            "template_name": "purchase_order_template",
-                                           "template_to_select": self.test_purchase_order_template}
+                                           "template_to_select": self.test_purchase_order_template},
                            }
         for document_type in test_parameters:
             test_parameter = test_parameters[document_type]
             create_sales_document_from_reference(test_case=self,
                                                  timeout=timeout,
                                                  document_type=document_type,
-                                                 reference_type="contract",
-                                                 reference_id=self.test_contract,
+                                                 reference_type="quote",
+                                                 reference_id=self.test_quote,
                                                  action_name=test_parameter["action_name"],
                                                  template_name=test_parameter["template_name"],
                                                  template_to_select=test_parameter["template_to_select"])
```

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_time_tracking_add_row.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_time_tracking_add_row.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,66 +1,67 @@
 import pytest
-from django.test import LiveServerTestCase
-from selenium import webdriver
-from koalixcrm.test_support_functions import *
+from koalixcrm.test.test_support_functions import *
 from koalixcrm.crm.factories.factory_user import AdminUserFactory
 from koalixcrm.crm.factories.factory_customer import StandardCustomerFactory
 from koalixcrm.crm.factories.factory_customer_group import StandardCustomerGroupFactory
 from koalixcrm.crm.factories.factory_currency import StandardCurrencyFactory
 from koalixcrm.crm.factories.factory_human_resource import StandardHumanResourceFactory
 from koalixcrm.djangoUserExtension.factories.factory_user_extension import StandardUserExtensionFactory
+from koalixcrm.test.UITests import UITests
 
 
-class TimeTrackingAddRow(LiveServerTestCase):
+class TimeTrackingAddRow(UITests):
 
     def setUp(self):
-        firefox_options = webdriver.firefox.options.Options()
-        firefox_options.set_headless(headless=True)
-        self.selenium = webdriver.Firefox(firefox_options=firefox_options)
+        super().setUp()
         self.test_user = AdminUserFactory.create()
         self.test_customer_group = StandardCustomerGroupFactory.create()
         self.test_customer = StandardCustomerFactory.create(is_member_of=(self.test_customer_group,))
         self.test_currency = StandardCurrencyFactory.create()
         self.test_user_extension = StandardUserExtensionFactory.create(user=self.test_user)
         self.test_human_resource = StandardHumanResourceFactory.create(user=self.test_user_extension)
 
     def tearDown(self):
-        self.selenium.quit()
+        super().tearDown()
 
     @pytest.mark.front_end_tests
     def test_add_new_row(self):
         selenium = self.selenium
         # login
         selenium.get('%s%s' % (self.live_server_url, '/koalixcrm/crm/reporting/time_tracking/'))
         # the browser will be redirected to the login page
         timeout = 5
         try:
             element_present = expected_conditions.presence_of_element_located((By.ID, 'id_username'))
             WebDriverWait(selenium, timeout).until(element_present)
         except TimeoutException:
             print("Timed out waiting for page to load")
-        username = selenium.find_element_by_xpath('//*[@id="id_username"]')
-        password = selenium.find_element_by_xpath('//*[@id="id_password"]')
-        submit_button = selenium.find_element_by_xpath('/html/body/div/article/div/div/form/div/ul/li/input')
+        username = selenium.find_element('xpath', '//*[@id="id_username"]')
+        password = selenium.find_element('xpath', '//*[@id="id_password"]')
+        submit_button = selenium.find_element('xpath', '/html/body/div/article/div/div/form/div/ul/li/input')
         username.send_keys("admin")
         password.send_keys("admin")
         submit_button.send_keys(Keys.RETURN)
+        time.sleep(5)
+        selenium.get('%s%s' % (self.live_server_url, '/koalixcrm/crm/reporting/time_tracking/'))
         # after the login, the browser is redirected to the target url /koalixcrm/crm/reporting/time_tracking
         try:
             element_present = expected_conditions.presence_of_element_located((By.ID, 'id_form-0-project'))
             WebDriverWait(selenium, timeout).until(element_present)
         except TimeoutException:
             print("Timed out waiting for page to load")
         # find the form element
-        assert_when_element_does_not_exist(self, '//*[@id="id_form-0-project"]')
-        assert_when_element_does_not_exist(self, '//*[@id="id_form-0-task"]')
-        assert_when_element_does_not_exist(self, '//*[@id="id_form-0-date"]')
-        assert_when_element_does_not_exist(self, '//*[@id="id_form-0-start_time"]')
-        assert_when_element_does_not_exist(self, '//*[@id="id_form-0-stop_time"]')
-        assert_when_element_does_not_exist(self, '//*[@id="id_form-0-description"]')
-        assert_when_element_does_not_exist(self, 'save')
+        fail_when_element_does_not_exist(self, '//*[@id="id_form-0-project"]')
+        fail_when_element_does_not_exist(self, '//*[@id="id_form-0-task"]')
+        fail_when_element_does_not_exist(self, '//*[@id="id_form-0-datetime_start_0"]')
+        fail_when_element_does_not_exist(self, '//*[@id="id_form-0-datetime_start_1"]')
+        fail_when_element_does_not_exist(self, '//*[@id="id_form-0-datetime_stop_0"]')
+        fail_when_element_does_not_exist(self, '//*[@id="id_form-0-datetime_stop_1"]')
+        fail_when_element_does_not_exist(self, '//*[@id="id_form-0-worked_hours"]')
+        fail_when_element_does_not_exist(self, '//*[@id="id_form-0-description"]')
+        fail_when_element_does_not_exist(self, '//*[@name="save"]')
         # check existence of a second form before pressing add more
-        assert_when_element_exists(self, '//*[@id="id_form-1-project"]')
-        add_more_button = selenium.find_element_by_xpath('//*[@id="add_more"]')
+        fail_when_element_exists(self, '//*[@id="id_form-1-project"]')
+        add_more_button = selenium.find_element('xpath', '//*[@id="add_more"]')
         add_more_button.send_keys(Keys.RETURN)
         # check existence of a second form after pressing add more
-        assert_when_element_does_not_exist(self, '//*[@id="id_form-1-project"]')
+        fail_when_element_does_not_exist(self, '//*[@id="id_form-1-project"]')
```

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_incomplete_sales_document_position.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_incomplete_sales_document_position.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_task_effective_effort.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_task_effective_effort.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_calculations_document.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_calculations_document.py`

 * *Files 0% similar despite different names*

```diff
@@ -322,15 +322,15 @@
         )
         datetime_now = make_date_utc(datetime.datetime(2024, 1, 1, 0, 00))
         date_now = datetime_now.date()
         Calculations.calculate_document_price(
             document=quote_7,
             pricing_date=date_now)
         self.assertEqual(
-            quote_7.last_calculated_price.__str__(), "20.75")
+            quote_7.last_calculated_price.__str__(), "20.80")
         self.assertEqual(
             quote_7.last_calculated_tax.__str__(), "2.05")
 
     @pytest.mark.back_end_tests
     def test_calculate_document_with_customer_group_transform(self):
         quote_8 = StandardQuoteFactory.create(
             customer=self.customer)
```

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_project_planned_costs.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_project_planned_costs.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_task_effective_duration.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_task_effective_duration.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_create_task.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_create_task.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_create_sales_document_from_quote.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_create_sales_document_from_invoice.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,47 @@
 # -*- coding: utf-8 -*-
 import pytest
 import os
 from django.contrib.staticfiles.testing import StaticLiveServerTestCase
 from selenium import webdriver
-from koalixcrm.test_support_functions import *
+from koalixcrm.test.test_support_functions import *
 from koalixcrm.crm.factories.factory_contract import StandardContractFactory
-from koalixcrm.crm.factories.factory_quote import StandardQuoteFactory
+from koalixcrm.crm.factories.factory_invoice import StandardInvoiceFactory
 from koalixcrm.crm.factories.factory_user import AdminUserFactory
 from koalixcrm.crm.factories.factory_customer_group import StandardCustomerGroupFactory
 from koalixcrm.djangoUserExtension.factories.factory_document_template import StandardQuoteTemplateFactory
 from koalixcrm.djangoUserExtension.factories.factory_document_template import StandardInvoiceTemplateFactory
 from koalixcrm.djangoUserExtension.factories.factory_document_template import StandardPurchaseOrderTemplateFactory
+from koalixcrm.djangoUserExtension.factories.factory_document_template import StandardDeliveryNoteTemplateFactory
+from koalixcrm.djangoUserExtension.factories.factory_document_template import StandardPaymentReminderTemplateFactory
 from koalixcrm.crm.documents.quote import Quote
 from koalixcrm.crm.documents.invoice import Invoice
 from koalixcrm.crm.documents.purchase_order import PurchaseOrder
+from koalixcrm.crm.documents.delivery_note import DeliveryNote
+from koalixcrm.crm.documents.payment_reminder import PaymentReminder
 
 
 class CreateSalesDocumentFromContract(StaticLiveServerTestCase):
 
     @classmethod
     def setUpClass(cls):
         super(CreateSalesDocumentFromContract, cls).setUpClass()
         firefox_options = webdriver.firefox.options.Options()
-        firefox_options.set_headless(headless=True)
-        cls.selenium = webdriver.Firefox(firefox_options=firefox_options)
+        firefox_options.add_argument("--headless")
+        cls.selenium = webdriver.Firefox(options=firefox_options)
         cls.selenium.implicitly_wait(10)
         cls.test_user = AdminUserFactory.create()
         cls.test_customer_group = StandardCustomerGroupFactory.create()
         cls.test_contract = StandardContractFactory.create()
-        cls.test_quote = StandardQuoteFactory.create(contract=cls.test_contract)
+        cls.test_invoice = StandardInvoiceFactory.create(contract=cls.test_contract)
         cls.test_quote_template = StandardQuoteTemplateFactory.create()
         cls.test_invoice_template = StandardInvoiceTemplateFactory.create()
         cls.test_purchase_order_template = StandardPurchaseOrderTemplateFactory.create()
+        cls.test_payment_reminder_template = StandardPaymentReminderTemplateFactory.create()
+        cls.test_delivery_note_template = StandardDeliveryNoteTemplateFactory.create()
 
     @classmethod
     def tearDownClass(cls):
         cls.selenium.quit()
         super(CreateSalesDocumentFromContract, cls).tearDownClass()
 
     def tearDown(self):
@@ -46,25 +52,25 @@
             self.selenium.save_screenshot(directory + "%s.png" % "test_name")
         super(CreateSalesDocumentFromContract, self).tearDown()
 
     @pytest.mark.front_end_tests
     def test_create_sales_document_from_quote(self):
         selenium = self.selenium
         # login
-        selenium.get('%s%s' % (self.live_server_url, '/admin/crm/quote/'))
+        selenium.get('%s%s' % (self.live_server_url, '/admin/crm/invoice/'))
         # the browser will be redirected to the login page
         timeout = 2
         try:
             element_present = expected_conditions.presence_of_element_located((By.ID, 'id_username'))
             WebDriverWait(selenium, timeout).until(element_present)
         except TimeoutException:
             print("Timed out waiting for page to load")
-        username = selenium.find_element_by_xpath('//*[@id="id_username"]')
-        password = selenium.find_element_by_xpath('//*[@id="id_password"]')
-        submit_button = selenium.find_element_by_xpath('/html/body/div/article/div/div/form/div/ul/li/input')
+        username = selenium.find_element('xpath', '//*[@id="id_username"]')
+        password = selenium.find_element('xpath', '//*[@id="id_password"]')
+        submit_button = selenium.find_element('xpath', '/html/body/div/article/div/div/form/div/ul/li/input')
         username.send_keys("admin")
         password.send_keys("admin")
         submit_button.send_keys(Keys.RETURN)
         # after the login, the browser is redirected to the target url /koalixcrm/crm/contract
         try:
             element_present = expected_conditions.presence_of_element_located((By.ID, 'id_form-0-project'))
             WebDriverWait(selenium, timeout).until(element_present)
@@ -76,18 +82,24 @@
                                    "template_to_select": self.test_quote_template},
                            Invoice: {"action_name": "create_invoice",
                                      "template_name": "invoice_template",
                                      "template_to_select": self.test_invoice_template},
                            PurchaseOrder: {"action_name": "create_purchase_order",
                                            "template_name": "purchase_order_template",
                                            "template_to_select": self.test_purchase_order_template},
+                           PaymentReminder: {"action_name": "create_payment_reminder",
+                                             "template_name": "payment_reminder_template",
+                                             "template_to_select": self.test_payment_reminder_template},
+                           DeliveryNote: {"action_name": "create_delivery_note",
+                                          "template_name": "delivery_note_template",
+                                          "template_to_select": self.test_delivery_note_template},
                            }
         for document_type in test_parameters:
             test_parameter = test_parameters[document_type]
             create_sales_document_from_reference(test_case=self,
                                                  timeout=timeout,
                                                  document_type=document_type,
-                                                 reference_type="quote",
-                                                 reference_id=self.test_quote,
+                                                 reference_type="invoice",
+                                                 reference_id=self.test_invoice,
                                                  action_name=test_parameter["action_name"],
                                                  template_name=test_parameter["template_name"],
                                                  template_to_select=test_parameter["template_to_select"])
```

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_task_effective_costs_with_agreement.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_task_effective_costs_with_agreement.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_task_effective_costs_no_agreement.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_task_effective_costs_no_agreement.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_project_effective_costs.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_project_effective_costs.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_version_increase.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_version_increase.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_task_planned_effort.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_task_planned_effort.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_task_constructor.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_task_constructor.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/tests/test_task_planned_duration.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_task_planned_duration.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/const/country.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/const/country.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*
 
-from django.utils.translation import ugettext as _
+from django.utils.translation import gettext as _
 
 COUNTRIES = (
     ('AF', 'AFG', '004', _('Afghanistan')),
     ('AX', 'ALA', '248', _('Aland Islands')),
     ('AL', 'ALB', '008', _('Albania')),
     ('DZ', 'DZA', '012', _('Algeria')),
     ('AS', 'ASM', '016', _('American Samoa')),
```

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/const/status.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/const/status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*
 
-from django.utils.translation import ugettext as _
+from django.utils.translation import gettext as _
 
 INVOICESTATUS = (
     ('P', _('Payed')),
     ('C', _('Invoice created')),
     ('I', _('Invoice sent')),
     ('F', _('First reminder sent')),
     ('R', _('Second reminder sent')),
```

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/const/purpose.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/const/purpose.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*
 
-from django.utils.translation import ugettext as _
+from django.utils.translation import gettext as _
 
 PURPOSESADDRESSINCONTRACT = (
     ('D', _('Delivery Address')),
     ('B', _('Billing Address')),
     ('C', _('Contact Address')),
 )
```

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/inlinemixin.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/inlinemixin.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/documents/contract.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/documents/contract.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 
 from django.db import models
 from django.contrib import admin
-from django.utils.translation import ugettext as _
+from django.utils.translation import gettext as _
 
 from koalixcrm.plugin import *
 from koalixcrm.crm.contact.phone_address import PhoneAddress
 from koalixcrm.crm.contact.email_address import EmailAddress
 from koalixcrm.crm.contact.postal_address import PostalAddress
 from koalixcrm.crm.documents.invoice import Invoice
 from koalixcrm.crm.documents.quote import Quote
@@ -107,14 +107,15 @@
                        'purpose',)
         }),
     )
     allow_add = True
 
 
 class Contract(models.Model):
+    id = models.BigAutoField(primary_key=True)
     staff = models.ForeignKey('auth.User',
                               on_delete=models.CASCADE,
                               limit_choices_to={'is_staff': True},
                               verbose_name=_("Staff"),
                               related_name="db_relcontractstaff",
                               blank=True,
                               null=True)
```

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/documents/sales_document.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/documents/sales_document.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 # -*- coding: utf-8 -*-
 
 from datetime import *
 from django.db import models
 from django.contrib import admin, messages
-from django.utils.translation import ugettext as _
+from django.utils.translation import gettext as _
 from koalixcrm.crm.const.purpose import *
 from koalixcrm.global_support_functions import xstr, make_date_utc
 from koalixcrm.crm.contact.phone_address import PhoneAddress
 from koalixcrm.crm.contact.email_address import EmailAddress
 from koalixcrm.crm.contact.postal_address import PostalAddress
 from koalixcrm.crm.documents.sales_document_position import SalesDocumentPosition, SalesDocumentInlinePosition
 from koalixcrm.djangoUserExtension.models import TextParagraphInDocumentTemplate, UserExtension
 from koalixcrm.crm.product.product_type import ProductType
 from koalixcrm.crm.exceptions import TemplateSetMissingInContract
 import koalixcrm.crm.documents.calculations
 from koalixcrm.crm.documents.pdf_export import PDFExport
 
 
 class TextParagraphInSalesDocument(models.Model):
+    id = models.BigAutoField(primary_key=True)
     sales_document = models.ForeignKey("SalesDocument", on_delete=models.CASCADE)
     purpose = models.CharField(verbose_name=_("Purpose"), max_length=2, choices=PURPOSESTEXTPARAGRAPHINDOCUMENTS)
     text_paragraph = models.TextField(verbose_name=_("Text"), blank=False, null=False)
 
     def create_paragraph(self, default_paragraph, sales_document):
         self.sales_document = sales_document
         self.purpose = default_paragraph.purpose
@@ -35,14 +36,15 @@
         verbose_name_plural = _('Text Paragraphs In Sales Documents')
 
     def __str__(self):
         return self.id.__str__()
 
 
 class SalesDocument(models.Model):
+    id = models.BigAutoField(primary_key=True)
     contract = models.ForeignKey("Contract",
                                  on_delete=models.CASCADE,
                                  verbose_name=_('Contract'))
     external_reference = models.CharField(verbose_name=_("External Reference"),
                                           max_length=100,
                                           blank=True)
     discount = models.DecimalField(max_digits=5,
```

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/documents/payment_reminder.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/documents/payment_reminder.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 
 from datetime import *
 from django.db import models
-from django.utils.translation import ugettext as _
+from django.utils.translation import gettext as _
 from koalixcrm.crm.const.status import *
 from django.core.validators import MaxValueValidator, MinValueValidator
 from koalixcrm.crm.documents.sales_document import SalesDocument, OptionSalesDocument
 from koalixcrm.plugin import *
 
 
 class PaymentReminder(SalesDocument):
```

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/documents/purchase_confirmation.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/documents/purchase_confirmation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-from django.utils.translation import ugettext as _
+from django.utils.translation import gettext as _
 from koalixcrm.crm.documents.sales_document import SalesDocument, OptionSalesDocument
 
 
 class PurchaseConfirmation(SalesDocument):
 
     def create_from_reference(self, calling_model):
         self.create_sales_document(calling_model)
```

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/documents/calculations.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/documents/calculations.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,23 +31,25 @@
         if positions.exists():
             for position in positions:
                 price += Calculations.calculate_position_price(position,
                                                                pricing_date,
                                                                contact_for_price_calculation,
                                                                document.currency)
                 tax += Calculations.calculate_position_tax(position, document.currency)
-
             if document.discount is not None:
                 discount = Decimal(document.discount)
                 total_price = price * (1 - discount / 100)
                 total_tax = tax * (1 - discount / 100)
                 total_price = Decimal(total_price)
                 total_tax = Decimal(total_tax)
                 price = document.currency.round(total_price)
                 tax = document.currency.round(total_tax)
+            else:
+                tax = document.currency.round(tax)
+                price = document.currency.round(price)
         document.last_calculated_price = price
         document.last_calculated_tax = tax
         document.last_pricing_date = pricing_date
         document.save()
         return 1
 
     @staticmethod
@@ -80,15 +82,15 @@
             raise SalesDocumentPosition.NoPriceFound
         nominal_total = position.position_price_per_unit * position.quantity
         if isinstance(position.discount, Decimal):
             nominal_minus_discount = nominal_total * (1 - position.discount / 100)
         else:
             nominal_minus_discount = nominal_total
         total_with_tax = Decimal(nominal_minus_discount)
-        position.last_calculated_price = currency.round(total_with_tax)
+        position.last_calculated_price = total_with_tax
         position.last_pricing_date = pricing_date
         position.save()
         return position.last_calculated_price
 
     @staticmethod
     def calculate_position_tax(position, currency):
         """Performs a tax calculation a position.
@@ -107,10 +109,10 @@
         nominal_total = position.position_price_per_unit * position.quantity
         if isinstance(position.discount, Decimal):
             nominal_minus_discount = nominal_total * (1 - position.discount / 100)
         else:
             nominal_minus_discount = nominal_total
         total_tax = nominal_minus_discount * position.product_type.get_tax_rate() / 100
         total_tax = Decimal(total_tax)
-        position.last_calculated_tax = currency.round(total_tax)
+        position.last_calculated_tax = total_tax
         position.save()
         return position.last_calculated_tax
```

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/documents/invoice.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/documents/invoice.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 
 from datetime import *
 from django import forms
 from django.db import models
 from django.contrib import admin
 from django.http import HttpResponseRedirect
-from django.utils.translation import ugettext as _
+from django.utils.translation import gettext as _
 from django.utils.html import format_html
 from django.contrib.admin import helpers
 from django.shortcuts import render
 from django.contrib import messages
 from django.template.context_processors import csrf
 from koalixcrm.crm.const.status import *
 from koalixcrm.crm.exceptions import *
@@ -116,21 +116,21 @@
         payment_account = forms.ModelChoiceField(Account.objects.filter(account_type="A"))
 
     def register_invoice_in_accounting(self, request, queryset):
         try:
             for obj in queryset:
                 obj.register_invoice_in_accounting(request)
             self.message_user(request, _("Successfully registered Invoice in the Accounting"))
-            return;
+            return
         except OpenInterestAccountMissing as e:
             self.message_user(request, "Did not register Invoice in Accounting: " + e.__str__(), level=messages.ERROR)
-            return;
+            return
         except IncompleteInvoice as e:
             self.message_user(request, "Did not register Invoice in Accounting: " + e.__str__(), level=messages.ERROR)
-            return;
+            return
 
     register_invoice_in_accounting.short_description = _("Register Invoice in Accounting")
 
     # def unregisterInvoiceInAccounting(self, request, queryset):
     # for obj in queryset:
     # obj.createPDF(deliveryorder=True)
     # self.message_user(request, _("Successfully unregistered Invoice in the Accounting"))
```

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/documents/quote.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/documents/quote.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 from datetime import *
 from django.db import models
 from django.contrib import admin
-from django.utils.translation import ugettext as _
+from django.utils.translation import gettext as _
 from django.utils.html import format_html
 from koalixcrm.crm.const.status import *
 from koalixcrm.plugin import *
 from koalixcrm.crm.documents.sales_document import SalesDocument, OptionSalesDocument
 from koalixcrm.global_support_functions import limit_string_length
```

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/documents/pdf_export.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/documents/pdf_export.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/documents/purchase_order.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/documents/purchase_order.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
 from django.db import models
-from django.utils.translation import ugettext as _
+from django.utils.translation import gettext as _
 from koalixcrm.crm.const.status import *
 from koalixcrm.crm.documents.sales_document import SalesDocument, OptionSalesDocument
 from koalixcrm.plugin import *
 
 
 class PurchaseOrder(SalesDocument):
     supplier = models.ForeignKey("Supplier", on_delete=models.CASCADE, verbose_name=_("Supplier"), null=True)
```

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/documents/sales_document_position.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/documents/sales_document_position.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # -*- coding: utf-8 -*-
 
 from django.db import models
 from django.contrib import admin
 from django.core.validators import MinValueValidator
-from django.utils.translation import ugettext as _
+from django.utils.translation import gettext as _
 
 
 class Position(models.Model):
+    id = models.BigAutoField(primary_key=True)
     position_number = models.PositiveIntegerField(verbose_name=_("Position Number"),
                                                   validators=[MinValueValidator(1)])
     quantity = models.DecimalField(verbose_name=_("Quantity"),
                                    decimal_places=3,
                                    max_digits=10)
     description = models.TextField(verbose_name=_("Description"),
                                    blank=True, null=True)
```

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/documents/delivery_note.py` & `koalix-crm-1.14.0rc1/koalixcrm/crm/documents/delivery_note.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
 from django.db import models
-from django.utils.translation import ugettext as _
+from django.utils.translation import gettext as _
 from koalixcrm.crm.const.status import *
 from koalixcrm.crm.documents.sales_document import SalesDocument, OptionSalesDocument
 
 
 class DeliveryNote(SalesDocument):
     tracking_reference = models.CharField(verbose_name=_("Tracking Reference"), max_length=100, blank=True)
     status = models.CharField(max_length=1, choices=DELIVERYNOTESTATUS)
```

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/locale/pt_BR/LC_MESSAGES/django.po` & `koalix-crm-1.14.0rc1/koalixcrm/crm/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/locale/pt_BR/LC_MESSAGES/django.mo` & `koalix-crm-1.14.0rc1/koalixcrm/crm/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/locale/de/LC_MESSAGES/django.po` & `koalix-crm-1.14.0rc1/koalixcrm/crm/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/koalixcrm/crm/locale/de/LC_MESSAGES/django.mo` & `koalix-crm-1.14.0rc1/koalixcrm/crm/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.13.dev9/README.md` & `koalix-crm-1.14.0rc1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -20,18 +20,19 @@
 <li> Create Project Reports</li>
 <li> Adjust Access Rights </li></ul></td>
   </tr></table>
 
 ## Quality badges on master
 | Project build: | Codacy results: |Docker: | Social Networks: |
 | --- | --- | --- | --- |
-| [![Build Status](https://travis-ci.org/scaphilo/koalixcrm.svg?branch=master)](https://travis-ci.org/scaphilo/koalixcrm) | [![Codacy Badge](https://api.codacy.com/project/badge/Grade/4f0acae8f6d04c2b81c0c4a4b2b48e09)](https://www.codacy.com/app/simon.riedener/koalixcrm?utm_source=github.com&utm_medium=referral&utm_content=scaphilo/koalixcrm&utm_campaign=badger) [![Codacy Badge](https://api.codacy.com/project/badge/Coverage/4f0acae8f6d04c2b81c0c4a4b2b48e09)](https://www.codacy.com/app/simon.riedener/koalixcrm?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=scaphilo/koalixcrm&amp;utm_campaign=Badge_Coverage) | [![Docker Automated build](https://img.shields.io/docker/automated/koalixswitzerland/koalixcrm.svg)]() [![Docker Build Status](https://img.shields.io/docker/build/koalixswitzerland/koalixcrm.svg)]()<br/> [![Docker Stars](https://img.shields.io/docker/stars/koalixswitzerland/koalixcrm.svg)]() [![Docker Pulls](https://img.shields.io/docker/pulls/koalixswitzerland/koalixcrm.svg)]() | [![Gitter chat](https://badges.gitter.im/gitterHQ/gitter.png)](https://gitter.im/koalix-crm/Lobby) |
+| [![Django CI](https://github.com/KoalixSwitzerland/koalixcrm/actions/workflows/django.yml/badge.svg)](https://github.com/KoalixSwitzerland/koalixcrm/actions/workflows/django.yml) | [![Codacy Badge](https://app.codacy.com/project/badge/Grade/cfae578b5c174f438786c935fa425002)](https://app.codacy.com/gh/KoalixSwitzerland/koalixcrm/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade) </br> [![Codacy Badge](https://app.codacy.com/project/badge/Coverage/cfae578b5c174f438786c935fa425002)](https://app.codacy.com/gh/KoalixSwitzerland/koalixcrm/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_coverage)| [![Docker Automated build](https://img.shields.io/docker/automated/koalixswitzerland/koalixcrm.svg)]() <br/> [![Docker Stars](https://img.shields.io/docker/stars/koalixswitzerland/koalixcrm.svg)]() [![Docker Pulls](https://img.shields.io/docker/pulls/koalixswitzerland/koalixcrm.svg)]() | [![Gitter chat](https://badges.gitter.im/gitterHQ/gitter.png)](https://gitter.im/koalix-crm/Lobby) |
 
 ## Demos
-[demo](http://koalixcrmdemoenglish.koalix.org/admin/).
+The demo-branch is automatically deployed and can be found here:
+[Demo-Deployment](https://demo.koalixcrm.koalix.net/admin/).
 
 To be able to log in use the following credentials 
 <ul>
   <li><b>user: guest</b></li>
   <li><b>password: guestpassword</b></li>
  </ul>
```

#### html2text {}

```diff
@@ -8,32 +8,33 @@
       interface                             * Manage Projects, Tasks, Work
     * High quality output documents           (Traditional project management)
     * Small business <10 employees with     * Manage Document Tempaltes
       access                                * Double Entry Accounting
     * Cloud hosted, Self-hosted, Not        * Create Project Reports
       hosted (single-user, offline)         * Adjust Access Rights
 ## Quality badges on master | Project build: | Codacy results: |Docker: |
-Social Networks: | | --- | --- | --- | --- | | [![Build Status](https://travis-
-ci.org/scaphilo/koalixcrm.svg?branch=master)](https://travis-ci.org/scaphilo/
-koalixcrm) | [![Codacy Badge](https://api.codacy.com/project/badge/Grade/
-4f0acae8f6d04c2b81c0c4a4b2b48e09)](https://www.codacy.com/app/simon.riedener/
-koalixcrm?utm_source=github.com&utm_medium=referral&utm_content=scaphilo/
-koalixcrm&utm_campaign=badger) [![Codacy Badge](https://api.codacy.com/project/
-badge/Coverage/4f0acae8f6d04c2b81c0c4a4b2b48e09)](https://www.codacy.com/app/
-simon.riedener/
-koalixcrm?utm_source=github.com&utm_medium=referral&utm_content=scaphilo/
-koalixcrm&utm_campaign=Badge_Coverage) | [![Docker Automated build](https://
-img.shields.io/docker/automated/koalixswitzerland/koalixcrm.svg)]() [![Docker
-Build Status](https://img.shields.io/docker/build/koalixswitzerland/
-koalixcrm.svg)]()
+Social Networks: | | --- | --- | --- | --- | | [![Django CI](https://
+github.com/KoalixSwitzerland/koalixcrm/actions/workflows/django.yml/badge.svg)]
+(https://github.com/KoalixSwitzerland/koalixcrm/actions/workflows/django.yml) |
+[![Codacy Badge](https://app.codacy.com/project/badge/Grade/
+cfae578b5c174f438786c935fa425002)](https://app.codacy.com/gh/KoalixSwitzerland/
+koalixcrm/
+dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
+[![Codacy Badge](https://app.codacy.com/project/badge/Coverage/
+cfae578b5c174f438786c935fa425002)](https://app.codacy.com/gh/KoalixSwitzerland/
+koalixcrm/
+dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_coverage)|
+[![Docker Automated build](https://img.shields.io/docker/automated/
+koalixswitzerland/koalixcrm.svg)]()
 [![Docker Stars](https://img.shields.io/docker/stars/koalixswitzerland/
 koalixcrm.svg)]() [![Docker Pulls](https://img.shields.io/docker/pulls/
 koalixswitzerland/koalixcrm.svg)]() | [![Gitter chat](https://badges.gitter.im/
-gitterHQ/gitter.png)](https://gitter.im/koalix-crm/Lobby) | ## Demos [demo]
-(http://koalixcrmdemoenglish.koalix.org/admin/). To be able to log in use the
+gitterHQ/gitter.png)](https://gitter.im/koalix-crm/Lobby) | ## Demos The demo-
+branch is automatically deployed and can be found here: [Demo-Deployment]
+(https://demo.koalixcrm.koalix.net/admin/). To be able to log in use the
 following credentials
     * uusseerr:: gguueesstt
     * ppaasssswwoorrdd:: gguueessttppaasssswwoorrdd
 ## Documentation You can find the documentation of koalixcrm here: [doc](http:/
 /readthedocs.org/docs/koalixcrm/en/master/) ## Installation Some information
 about the installation of koalixcrm: [installation](https://github.com/
 scaphilo/koalixcrm/wiki/Installation) ## Development environment setup
```

### Comparing `koalix-crm-1.13.dev9/koalix_crm.egg-info/SOURCES.txt` & `koalix-crm-1.14.0rc1/koalix_crm.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
+LICENSE
 MANIFEST.in
 README.md
 setup.py
 koalix_crm.egg-info/PKG-INFO
 koalix_crm.egg-info/SOURCES.txt
 koalix_crm.egg-info/dependency_links.txt
 koalix_crm.egg-info/not-zip-safe
 koalix_crm.egg-info/requires.txt
 koalix_crm.egg-info/top_level.txt
 koalixcrm/__init__.py
 koalixcrm/global_support_functions.py
 koalixcrm/plugin.py
-koalixcrm/test_support_functions.py
 koalixcrm/version.py
 koalixcrm/accounting/__init__.py
 koalixcrm/accounting/admin.py
 koalixcrm/accounting/exceptions.py
 koalixcrm/accounting/models.py
 koalixcrm/accounting/views.py
 koalixcrm/accounting/accounting/__init__.py
@@ -38,14 +38,15 @@
 koalixcrm/accounting/migrations/0004_auto_20171009_1949.py
 koalixcrm/accounting/migrations/0005_auto_20171110_1732.py
 koalixcrm/accounting/migrations/0006_auto_20180422_2048.py
 koalixcrm/accounting/migrations/0007_auto_20180422_2105.py
 koalixcrm/accounting/migrations/0008_auto_20181012_2056.py
 koalixcrm/accounting/migrations/0009_auto_20181012_2056.py
 koalixcrm/accounting/migrations/0010_auto_20181216_2224.py
+koalixcrm/accounting/migrations/0011_auto_20240329_2207.py
 koalixcrm/accounting/migrations/__init__.py
 koalixcrm/accounting/rest/__init__.py
 koalixcrm/accounting/rest/account_rest.py
 koalixcrm/accounting/rest/accounting_period_rest.py
 koalixcrm/accounting/rest/booking_rest.py
 koalixcrm/accounting/rest/product_categorie_rest.py
 koalixcrm/accounting/rest/restinterface.py
@@ -198,14 +199,15 @@
 koalixcrm/crm/migrations/0053_auto_20181014_2305.py
 koalixcrm/crm/migrations/0054_auto_20181020_1845.py
 koalixcrm/crm/migrations/0055_auto_20181022_1937.py
 koalixcrm/crm/migrations/0056_auto_20181216_2224.py
 koalixcrm/crm/migrations/0056_auto_20190102_2230.py
 koalixcrm/crm/migrations/0057_merge_20190106_1510.py
 koalixcrm/crm/migrations/0058_auto_20190401_2009.py
+koalixcrm/crm/migrations/0059_auto_20240329_2207.py
 koalixcrm/crm/migrations/__init__.py
 koalixcrm/crm/product/__init__.py
 koalixcrm/crm/product/currency.py
 koalixcrm/crm/product/currency_transform.py
 koalixcrm/crm/product/customer_group_transform.py
 koalixcrm/crm/product/price.py
 koalixcrm/crm/product/product.py
@@ -291,15 +293,15 @@
 koalixcrm/crm/tests/test_calculations_document.py
 koalixcrm/crm/tests/test_create_sales_document_from_contract.py
 koalixcrm/crm/tests/test_create_sales_document_from_invoice.py
 koalixcrm/crm/tests/test_create_sales_document_from_quote.py
 koalixcrm/crm/tests/test_create_task.py
 koalixcrm/crm/tests/test_delete_of_empty_row.py
 koalixcrm/crm/tests/test_incomplete_sales_document_position.py
-koalixcrm/crm/tests/test_poject_admin_view.py
+koalixcrm/crm/tests/test_project_admin_view.py
 koalixcrm/crm/tests/test_project_effective_costs.py
 koalixcrm/crm/tests/test_project_planned_costs.py
 koalixcrm/crm/tests/test_supplier_admin_view.py
 koalixcrm/crm/tests/test_task_constructor.py
 koalixcrm/crm/tests/test_task_effective_costs_no_agreement.py
 koalixcrm/crm/tests/test_task_effective_costs_with_agreement.py
 koalixcrm/crm/tests/test_task_effective_duration.py
@@ -343,14 +345,15 @@
 koalixcrm/djangoUserExtension/migrations/0001_initial.py
 koalixcrm/djangoUserExtension/migrations/0002_auto_20171009_1949.py
 koalixcrm/djangoUserExtension/migrations/0003_auto_20171110_1732.py
 koalixcrm/djangoUserExtension/migrations/0004_auto_20171210_2126.py
 koalixcrm/djangoUserExtension/migrations/0005_auto_20180612_1924.py
 koalixcrm/djangoUserExtension/migrations/0006_auto_20180701_2128.py
 koalixcrm/djangoUserExtension/migrations/0007_auto_20180702_1628.py
+koalixcrm/djangoUserExtension/migrations/0008_auto_20240329_2207.py
 koalixcrm/djangoUserExtension/migrations/__init__.py
 koalixcrm/djangoUserExtension/rest/__init__.py
 koalixcrm/djangoUserExtension/rest/document_template_rest.py
 koalixcrm/djangoUserExtension/rest/template_set_rest.py
 koalixcrm/djangoUserExtension/rest/user_extension_rest.py
 koalixcrm/djangoUserExtension/rest/user_rest.py
 koalixcrm/djangoUserExtension/user_extension/__init__.py
@@ -369,17 +372,16 @@
 koalixcrm/subscriptions/locale/pt_BR/LC_MESSAGES/django.mo
 koalixcrm/subscriptions/locale/pt_BR/LC_MESSAGES/django.po
 koalixcrm/subscriptions/migrations/0001_initial.py
 koalixcrm/subscriptions/migrations/0002_auto_20171009_1949.py
 koalixcrm/subscriptions/migrations/0003_auto_20171110_1732.py
 koalixcrm/subscriptions/migrations/0004_auto_20181013_2213.py
 koalixcrm/subscriptions/migrations/0005_auto_20181013_2228.py
+koalixcrm/subscriptions/migrations/0006_auto_20240329_2207.py
 koalixcrm/subscriptions/migrations/__init__.py
+koalixcrm/test/UITests.py
+koalixcrm/test/__init__.py
+koalixcrm/test/test_support_functions.py
 projectsettings/settings/__init__.py
 projectsettings/settings/base_settings.py
-projectsettings/settings/development_settings.py
-projectsettings/settings/development_sqlite_settings.py
-projectsettings/settings/development_sqlite_settings_linux.py
-projectsettings/settings/docker_development_settings.py
-projectsettings/settings/docker_production_settings.py
-projectsettings/settings/heroku_settings.py
-projectsettings/settings/production_settings.py
+projectsettings/settings/development_docker_sqlite_settings.py
+projectsettings/settings/production_docker_postgres_settings.py
```

### Comparing `koalix-crm-1.13.dev9/projectsettings/settings/base_settings.py` & `koalix-crm-1.14.0rc1/projectsettings/settings/base_settings.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,32 +1,15 @@
 """
-Django base settings for test_koalixcrm project.
-
-Generated by 'django-admin startproject' using Django 1.11.3.
-
-For more information on this file, see
-https://docs.djangoproject.com/en/1.11/topics/settings/
-
-For the full list of settings and their values, see
-https://docs.djangoproject.com/en/1.11/ref/settings/
+Django base settings for koalixcrm project.
 """
+
 import os
 
-# Build paths inside the project like this: os.path.join(BASE_DIR, ...)
 BASE_DIR = os.path.dirname(os.path.dirname(__file__))
 
-# Quick-start development settings - unsuitable for production
-# See https://docs.djangoproject.com/en/1.11/howto/deployment/checklist/
-
-# SECURITY WARNING: keep the secret key used in production secret!
-SECRET_KEY = 'modify_during_deployment'
-
-# SECURITY WARNING: don't run with debug turned on in production!
-DEBUG = True
-
 # Application definition
 PREREQUISITE_APPS = [
     'django.contrib.contenttypes',
     'grappelli.dashboard',
     'grappelli',
     'filebrowser',
     'django.contrib.admin',
@@ -97,32 +80,20 @@
         'NAME': 'django.contrib.auth.password_validation.CommonPasswordValidator',
     },
     {
         'NAME': 'django.contrib.auth.password_validation.NumericPasswordValidator',
     },
 ]
 
-
-# Internationalization
-# https://docs.djangoproject.com/en/1.11/topics/i18n/
-
 LANGUAGE_CODE = 'en-us'
-
 TIME_ZONE = 'UTC'
-
 USE_I18N = True
-
 USE_L10N = True
-
 USE_TZ = True
 
-
-# Static files (CSS, JavaScript, Images)
-# https://docs.djangoproject.com/en/1.11/howto/static-files/
-
 STATIC_URL = '/static/'
 STATIC_ROOT = os.path.join(BASE_DIR, 'static')
 
 MEDIA_URL = "/media/"
 MEDIA_ROOT = os.path.join(BASE_DIR)
 
 PROJECT_ROOT = BASE_DIR
```

