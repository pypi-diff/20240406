# Comparing `tmp/wellets_cli-1.9.2.tar.gz` & `tmp/wellets_cli-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wellets_cli-1.9.2.tar", max compression
+gzip compressed data, was "wellets_cli-1.9.3.tar", max compression
```

## Comparing `wellets_cli-1.9.2.tar` & `wellets_cli-1.9.3.tar`

### file list

```diff
@@ -1,30 +1,29 @@
--rw-r--r--   0        0        0     1211 2024-04-06 15:32:51.837237 wellets_cli-1.9.2/LICENSE
--rw-r--r--   0        0        0      914 2024-04-06 15:32:51.837237 wellets_cli-1.9.2/pyproject.toml
--rw-r--r--   0        0        0      210 2024-04-06 15:32:51.837237 wellets_cli-1.9.2/settings.toml
--rw-r--r--   0        0        0        6 2024-04-06 15:32:51.837237 wellets_cli-1.9.2/wellets_cli/VERSION
--rw-r--r--   0        0        0       46 2024-04-06 15:32:51.837237 wellets_cli-1.9.2/wellets_cli/__init__.py
--rw-r--r--   0        0        0      137 2024-04-06 15:32:51.837237 wellets_cli-1.9.2/wellets_cli/__main__.py
--rw-r--r--   0        0        0    15790 2024-04-06 15:32:51.841237 wellets_cli-1.9.2/wellets_cli/api.py
--rw-r--r--   0        0        0     1243 2024-04-06 15:32:51.841237 wellets_cli-1.9.2/wellets_cli/auth.py
--rw-r--r--   0        0        0      335 2024-04-06 15:32:51.841237 wellets_cli-1.9.2/wellets_cli/base.py
--rw-r--r--   0        0        0     2883 2024-04-06 15:32:51.841237 wellets_cli-1.9.2/wellets_cli/chart.py
--rw-r--r--   0        0        0     1455 2024-04-06 15:32:51.841237 wellets_cli-1.9.2/wellets_cli/cli.py
--rw-r--r--   0        0        0        0 2024-04-06 15:32:51.841237 wellets_cli-1.9.2/wellets_cli/commands/__init__.py
--rw-r--r--   0        0        0     8501 2024-04-06 15:32:51.841237 wellets_cli-1.9.2/wellets_cli/commands/accumulation.py
--rw-r--r--   0        0        0    10476 2024-04-06 15:32:51.841237 wellets_cli-1.9.2/wellets_cli/commands/asset.py
--rw-r--r--   0        0        0     1497 2024-04-06 15:32:51.841237 wellets_cli-1.9.2/wellets_cli/commands/currency.py
--rw-r--r--   0        0        0     2000 2024-04-06 15:32:51.841237 wellets_cli-1.9.2/wellets_cli/commands/investment.py
--rw-r--r--   0        0        0      734 2024-04-06 15:32:51.841237 wellets_cli-1.9.2/wellets_cli/commands/login.py
--rw-r--r--   0        0        0    11798 2024-04-06 15:32:51.841237 wellets_cli-1.9.2/wellets_cli/commands/portfolio.py
--rw-r--r--   0        0        0     1446 2024-04-06 15:32:51.841237 wellets_cli-1.9.2/wellets_cli/commands/register.py
--rw-r--r--   0        0        0     6938 2024-04-06 15:32:51.841237 wellets_cli-1.9.2/wellets_cli/commands/transaction.py
--rw-r--r--   0        0        0     3648 2024-04-06 15:32:51.841237 wellets_cli-1.9.2/wellets_cli/commands/transfer.py
--rw-r--r--   0        0        0    12729 2024-04-06 15:32:51.841237 wellets_cli-1.9.2/wellets_cli/commands/wallet.py
--rw-r--r--   0        0        0      246 2024-04-06 15:32:51.841237 wellets_cli-1.9.2/wellets_cli/commands/whoami.py
--rw-r--r--   0        0        0      415 2024-04-06 15:32:51.841237 wellets_cli-1.9.2/wellets_cli/config.py
--rw-r--r--   0        0        0     4510 2024-04-06 15:32:51.841237 wellets_cli-1.9.2/wellets_cli/model.py
--rw-r--r--   0        0        0      479 2024-04-06 15:32:51.841237 wellets_cli-1.9.2/wellets_cli/prompt.py
--rw-r--r--   0        0        0     9218 2024-04-06 15:32:51.841237 wellets_cli-1.9.2/wellets_cli/question.py
--rw-r--r--   0        0        0     4250 2024-04-06 15:32:51.841237 wellets_cli-1.9.2/wellets_cli/util.py
--rw-r--r--   0        0        0     6677 2024-04-06 15:32:51.841237 wellets_cli-1.9.2/wellets_cli/validator.py
--rw-r--r--   0        0        0      717 1970-01-01 00:00:00.000000 wellets_cli-1.9.2/PKG-INFO
+-rw-r--r--   0        0        0     1211 2024-04-06 16:31:44.164332 wellets_cli-1.9.3/LICENSE
+-rw-r--r--   0        0        0      870 2024-04-06 16:31:44.168332 wellets_cli-1.9.3/pyproject.toml
+-rw-r--r--   0        0        0        6 2024-04-06 16:31:44.168332 wellets_cli-1.9.3/wellets_cli/VERSION
+-rw-r--r--   0        0        0       46 2024-04-06 16:31:44.168332 wellets_cli-1.9.3/wellets_cli/__init__.py
+-rw-r--r--   0        0        0      137 2024-04-06 16:31:44.168332 wellets_cli-1.9.3/wellets_cli/__main__.py
+-rw-r--r--   0        0        0    15790 2024-04-06 16:31:44.168332 wellets_cli-1.9.3/wellets_cli/api.py
+-rw-r--r--   0        0        0     1243 2024-04-06 16:31:44.168332 wellets_cli-1.9.3/wellets_cli/auth.py
+-rw-r--r--   0        0        0      335 2024-04-06 16:31:44.168332 wellets_cli-1.9.3/wellets_cli/base.py
+-rw-r--r--   0        0        0     2875 2024-04-06 16:31:44.168332 wellets_cli-1.9.3/wellets_cli/chart.py
+-rw-r--r--   0        0        0     1455 2024-04-06 16:31:44.168332 wellets_cli-1.9.3/wellets_cli/cli.py
+-rw-r--r--   0        0        0        0 2024-04-06 16:31:44.168332 wellets_cli-1.9.3/wellets_cli/commands/__init__.py
+-rw-r--r--   0        0        0     8501 2024-04-06 16:31:44.168332 wellets_cli-1.9.3/wellets_cli/commands/accumulation.py
+-rw-r--r--   0        0        0    10476 2024-04-06 16:31:44.168332 wellets_cli-1.9.3/wellets_cli/commands/asset.py
+-rw-r--r--   0        0        0     1497 2024-04-06 16:31:44.168332 wellets_cli-1.9.3/wellets_cli/commands/currency.py
+-rw-r--r--   0        0        0     2000 2024-04-06 16:31:44.168332 wellets_cli-1.9.3/wellets_cli/commands/investment.py
+-rw-r--r--   0        0        0      720 2024-04-06 16:31:44.168332 wellets_cli-1.9.3/wellets_cli/commands/login.py
+-rw-r--r--   0        0        0    11798 2024-04-06 16:31:44.168332 wellets_cli-1.9.3/wellets_cli/commands/portfolio.py
+-rw-r--r--   0        0        0     1446 2024-04-06 16:31:44.168332 wellets_cli-1.9.3/wellets_cli/commands/register.py
+-rw-r--r--   0        0        0     6938 2024-04-06 16:31:44.168332 wellets_cli-1.9.3/wellets_cli/commands/transaction.py
+-rw-r--r--   0        0        0     3648 2024-04-06 16:31:44.168332 wellets_cli-1.9.3/wellets_cli/commands/transfer.py
+-rw-r--r--   0        0        0    12717 2024-04-06 16:31:44.168332 wellets_cli-1.9.3/wellets_cli/commands/wallet.py
+-rw-r--r--   0        0        0      246 2024-04-06 16:31:44.168332 wellets_cli-1.9.3/wellets_cli/commands/whoami.py
+-rw-r--r--   0        0        0     1245 2024-04-06 16:31:44.168332 wellets_cli-1.9.3/wellets_cli/config.py
+-rw-r--r--   0        0        0     4510 2024-04-06 16:31:44.168332 wellets_cli-1.9.3/wellets_cli/model.py
+-rw-r--r--   0        0        0      479 2024-04-06 16:31:44.168332 wellets_cli-1.9.3/wellets_cli/prompt.py
+-rw-r--r--   0        0        0     9218 2024-04-06 16:31:44.168332 wellets_cli-1.9.3/wellets_cli/question.py
+-rw-r--r--   0        0        0     4250 2024-04-06 16:31:44.168332 wellets_cli-1.9.3/wellets_cli/util.py
+-rw-r--r--   0        0        0     6677 2024-04-06 16:31:44.168332 wellets_cli-1.9.3/wellets_cli/validator.py
+-rw-r--r--   0        0        0      684 1970-01-01 00:00:00.000000 wellets_cli-1.9.3/PKG-INFO
```

### Comparing `wellets_cli-1.9.2/LICENSE` & `wellets_cli-1.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `wellets_cli-1.9.2/pyproject.toml` & `wellets_cli-1.9.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 [tool.poetry]
 name = "wellets_cli"
-version = "1.9.2"
+version = "1.9.3"
 description = "wellets-cli is the command line interface for Wellets, a crypto-oriented financial management tool that allows you to keep your money under control."
 authors = ["lparolari"]
-include = ["settings.toml"]
 
 [tool.poetry.dependencies]
 python = "^3.12"
 python-dotenv = "^1"
 requests = "^2"
 pydantic = "^2"
 click = "^8"
 tabulate = "^0.9"
 python-dateutil = "^2"
 inquirerpy = "^0.3"
 numpy = "^1.26"
 matplotlib = "^3.8"
-dynaconf = "^3"
 
 [tool.poetry.group.dev.dependencies]
 coverage = "^6"
 pytest = "^8"
 flake8 = "^7"
 black = "^24"
 isort = "^5"
```

### Comparing `wellets_cli-1.9.2/wellets_cli/api.py` & `wellets_cli-1.9.3/wellets_cli/api.py`

 * *Files identical despite different names*

### Comparing `wellets_cli-1.9.2/wellets_cli/auth.py` & `wellets_cli-1.9.3/wellets_cli/auth.py`

 * *Files identical despite different names*

### Comparing `wellets_cli-1.9.2/wellets_cli/chart.py` & `wellets_cli-1.9.3/wellets_cli/chart.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,18 +11,18 @@
     return plt.figure(figsize=(10, 6))
 
 
 def show_chart(fig, path=None):
     if not path:
         path = tempfile.mktemp(suffix=".png")
 
-    if settings.app.show_charts:
+    if settings.show_charts:
         plt.show()
 
-    if settings.app.save_charts:
+    if settings.save_charts:
         fig.savefig(path)
         print("Saved to", path)
 
     return fig
 
 
 def plot_balance(fig, history, label=None):
```

### Comparing `wellets_cli-1.9.2/wellets_cli/cli.py` & `wellets_cli-1.9.3/wellets_cli/cli.py`

 * *Files identical despite different names*

### Comparing `wellets_cli-1.9.2/wellets_cli/commands/accumulation.py` & `wellets_cli-1.9.3/wellets_cli/commands/accumulation.py`

 * *Files identical despite different names*

### Comparing `wellets_cli-1.9.2/wellets_cli/commands/asset.py` & `wellets_cli-1.9.3/wellets_cli/commands/asset.py`

 * *Files identical despite different names*

### Comparing `wellets_cli-1.9.2/wellets_cli/commands/currency.py` & `wellets_cli-1.9.3/wellets_cli/commands/currency.py`

 * *Files identical despite different names*

### Comparing `wellets_cli-1.9.2/wellets_cli/commands/investment.py` & `wellets_cli-1.9.3/wellets_cli/commands/investment.py`

 * *Files identical despite different names*

### Comparing `wellets_cli-1.9.2/wellets_cli/commands/login.py` & `wellets_cli-1.9.3/wellets_cli/commands/login.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,19 +13,19 @@
 @click.option("--password")
 def login(email: Optional[str], password: Optional[str]):
     """
     Login with your Wellets credentials.
     """
     email = (
         email
-        or settings.get("api_username")
+        or settings.api_username
         or inquirer.text(message="Email").execute()
     )
     password = (
         password
-        or settings.get("api_password")
+        or settings.api_password
         or inquirer.secret(message="Password").execute()
     )
 
     user_session = api.login(email, password)
 
     persist_auth(user_session.model_dump_json())
```

### Comparing `wellets_cli-1.9.2/wellets_cli/commands/portfolio.py` & `wellets_cli-1.9.3/wellets_cli/commands/portfolio.py`

 * *Files identical despite different names*

### Comparing `wellets_cli-1.9.2/wellets_cli/commands/register.py` & `wellets_cli-1.9.3/wellets_cli/commands/register.py`

 * *Files identical despite different names*

### Comparing `wellets_cli-1.9.2/wellets_cli/commands/transaction.py` & `wellets_cli-1.9.3/wellets_cli/commands/transaction.py`

 * *Files identical despite different names*

### Comparing `wellets_cli-1.9.2/wellets_cli/commands/transfer.py` & `wellets_cli-1.9.3/wellets_cli/commands/transfer.py`

 * *Files identical despite different names*

### Comparing `wellets_cli-1.9.2/wellets_cli/commands/wallet.py` & `wellets_cli-1.9.3/wellets_cli/commands/wallet.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
             currency.dollar_rate, base_currency.dollar_rate, wallet.balance
         )
         return {
             "id": wallet.id,
             "alias": wallet.alias,
             "balance": f"{currency.acronym} {pp(wallet.balance, decimals=8, fixed=False)}",
             "countervalue": f"{base_currency.acronym} {pp(countervalue, decimals=2, fixed=False)}",
-            "updated_at": wallet.updated_at.strftime(settings.app.date_format),
+            "updated_at": wallet.updated_at.strftime(settings.date_format),
             **({} if compact else {"desc": wallet.description}),
         }
 
     data = list(map(get_row_value, wallets))
 
     print(tabulate(data, headers="keys"))
 
@@ -227,19 +227,19 @@
         {"key": "id", "value": wallet.id},
         {"key": "alias", "value": wallet.alias},
         {"key": "balance", "value": wallet.balance},
         {"key": "currency", "value": wallet.currency.acronym},
         {"key": "desc", "value": wallet.description or "-"},
         {
             "key": "created_at",
-            "value": wallet.created_at.strftime(settings.app.datetime_format),
+            "value": wallet.created_at.strftime(settings.datetime_format),
         },
         {
             "key": "updated_at",
-            "value": wallet.updated_at.strftime(settings.app.datetime_format),
+            "value": wallet.updated_at.strftime(settings.datetime_format),
         },
         {
             "key": "portfolios",
             "value": f"{len(wallet.portfolios)} attached",
         },
     ]
```

### Comparing `wellets_cli-1.9.2/wellets_cli/model.py` & `wellets_cli-1.9.3/wellets_cli/model.py`

 * *Files identical despite different names*

### Comparing `wellets_cli-1.9.2/wellets_cli/question.py` & `wellets_cli-1.9.3/wellets_cli/question.py`

 * *Files identical despite different names*

### Comparing `wellets_cli-1.9.2/wellets_cli/util.py` & `wellets_cli-1.9.3/wellets_cli/util.py`

 * *Files identical despite different names*

### Comparing `wellets_cli-1.9.2/wellets_cli/validator.py` & `wellets_cli-1.9.3/wellets_cli/validator.py`

 * *Files identical despite different names*

### Comparing `wellets_cli-1.9.2/PKG-INFO` & `wellets_cli-1.9.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: wellets_cli
-Version: 1.9.2
+Version: 1.9.3
 Summary: wellets-cli is the command line interface for Wellets, a crypto-oriented financial management tool that allows you to keep your money under control.
 Author: lparolari
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: click (>=8,<9)
-Requires-Dist: dynaconf (>=3,<4)
 Requires-Dist: inquirerpy (>=0.3,<0.4)
 Requires-Dist: matplotlib (>=3.8,<4.0)
 Requires-Dist: numpy (>=1.26,<2.0)
 Requires-Dist: pydantic (>=2,<3)
 Requires-Dist: python-dateutil (>=2,<3)
 Requires-Dist: python-dotenv (>=1,<2)
 Requires-Dist: requests (>=2,<3)
```

