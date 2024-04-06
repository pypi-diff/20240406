# Comparing `tmp/wellets_cli-1.9.1.tar.gz` & `tmp/wellets_cli-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wellets_cli-1.9.1.tar", max compression
+gzip compressed data, was "wellets_cli-1.9.2.tar", max compression
```

## Comparing `wellets_cli-1.9.1.tar` & `wellets_cli-1.9.2.tar`

### file list

```diff
@@ -1,29 +1,30 @@
--rw-r--r--   0        0        0     1211 2024-03-17 10:55:55.909738 wellets_cli-1.9.1/LICENSE
--rw-r--r--   0        0        0      886 2024-03-17 10:55:55.913738 wellets_cli-1.9.1/pyproject.toml
--rw-r--r--   0        0        0        6 2024-03-17 10:55:55.913738 wellets_cli-1.9.1/wellets_cli/VERSION
--rw-r--r--   0        0        0       46 2024-03-17 10:55:55.913738 wellets_cli-1.9.1/wellets_cli/__init__.py
--rw-r--r--   0        0        0      137 2024-03-17 10:55:55.913738 wellets_cli-1.9.1/wellets_cli/__main__.py
--rw-r--r--   0        0        0    15790 2024-03-17 10:55:55.913738 wellets_cli-1.9.1/wellets_cli/api.py
--rw-r--r--   0        0        0     1243 2024-03-17 10:55:55.913738 wellets_cli-1.9.1/wellets_cli/auth.py
--rw-r--r--   0        0        0      335 2024-03-17 10:55:55.913738 wellets_cli-1.9.1/wellets_cli/base.py
--rw-r--r--   0        0        0     2702 2024-03-17 10:55:55.913738 wellets_cli-1.9.1/wellets_cli/chart.py
--rw-r--r--   0        0        0     1455 2024-03-17 10:55:55.913738 wellets_cli-1.9.1/wellets_cli/cli.py
--rw-r--r--   0        0        0        0 2024-03-17 10:55:55.913738 wellets_cli-1.9.1/wellets_cli/commands/__init__.py
--rw-r--r--   0        0        0     8501 2024-03-17 10:55:55.913738 wellets_cli-1.9.1/wellets_cli/commands/accumulation.py
--rw-r--r--   0        0        0    10286 2024-03-17 10:55:55.913738 wellets_cli-1.9.1/wellets_cli/commands/asset.py
--rw-r--r--   0        0        0     1497 2024-03-17 10:55:55.913738 wellets_cli-1.9.1/wellets_cli/commands/currency.py
--rw-r--r--   0        0        0     2000 2024-03-17 10:55:55.913738 wellets_cli-1.9.1/wellets_cli/commands/investment.py
--rw-r--r--   0        0        0      723 2024-03-17 10:55:55.913738 wellets_cli-1.9.1/wellets_cli/commands/login.py
--rw-r--r--   0        0        0    11798 2024-03-17 10:55:55.913738 wellets_cli-1.9.1/wellets_cli/commands/portfolio.py
--rw-r--r--   0        0        0     1446 2024-03-17 10:55:55.913738 wellets_cli-1.9.1/wellets_cli/commands/register.py
--rw-r--r--   0        0        0     6938 2024-03-17 10:55:55.913738 wellets_cli-1.9.1/wellets_cli/commands/transaction.py
--rw-r--r--   0        0        0     3648 2024-03-17 10:55:55.913738 wellets_cli-1.9.1/wellets_cli/commands/transfer.py
--rw-r--r--   0        0        0    12729 2024-03-17 10:55:55.913738 wellets_cli-1.9.1/wellets_cli/commands/wallet.py
--rw-r--r--   0        0        0      246 2024-03-17 10:55:55.913738 wellets_cli-1.9.1/wellets_cli/commands/whoami.py
--rw-r--r--   0        0        0      393 2024-03-17 10:55:55.913738 wellets_cli-1.9.1/wellets_cli/config.py
--rw-r--r--   0        0        0     4510 2024-03-17 10:55:55.913738 wellets_cli-1.9.1/wellets_cli/model.py
--rw-r--r--   0        0        0      479 2024-03-17 10:55:55.913738 wellets_cli-1.9.1/wellets_cli/prompt.py
--rw-r--r--   0        0        0     9218 2024-03-17 10:55:55.913738 wellets_cli-1.9.1/wellets_cli/question.py
--rw-r--r--   0        0        0     4250 2024-03-17 10:55:55.913738 wellets_cli-1.9.1/wellets_cli/util.py
--rw-r--r--   0        0        0     6677 2024-03-17 10:55:55.913738 wellets_cli-1.9.1/wellets_cli/validator.py
--rw-r--r--   0        0        0      717 1970-01-01 00:00:00.000000 wellets_cli-1.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1211 2024-04-06 15:32:51.837237 wellets_cli-1.9.2/LICENSE
+-rw-r--r--   0        0        0      914 2024-04-06 15:32:51.837237 wellets_cli-1.9.2/pyproject.toml
+-rw-r--r--   0        0        0      210 2024-04-06 15:32:51.837237 wellets_cli-1.9.2/settings.toml
+-rw-r--r--   0        0        0        6 2024-04-06 15:32:51.837237 wellets_cli-1.9.2/wellets_cli/VERSION
+-rw-r--r--   0        0        0       46 2024-04-06 15:32:51.837237 wellets_cli-1.9.2/wellets_cli/__init__.py
+-rw-r--r--   0        0        0      137 2024-04-06 15:32:51.837237 wellets_cli-1.9.2/wellets_cli/__main__.py
+-rw-r--r--   0        0        0    15790 2024-04-06 15:32:51.841237 wellets_cli-1.9.2/wellets_cli/api.py
+-rw-r--r--   0        0        0     1243 2024-04-06 15:32:51.841237 wellets_cli-1.9.2/wellets_cli/auth.py
+-rw-r--r--   0        0        0      335 2024-04-06 15:32:51.841237 wellets_cli-1.9.2/wellets_cli/base.py
+-rw-r--r--   0        0        0     2883 2024-04-06 15:32:51.841237 wellets_cli-1.9.2/wellets_cli/chart.py
+-rw-r--r--   0        0        0     1455 2024-04-06 15:32:51.841237 wellets_cli-1.9.2/wellets_cli/cli.py
+-rw-r--r--   0        0        0        0 2024-04-06 15:32:51.841237 wellets_cli-1.9.2/wellets_cli/commands/__init__.py
+-rw-r--r--   0        0        0     8501 2024-04-06 15:32:51.841237 wellets_cli-1.9.2/wellets_cli/commands/accumulation.py
+-rw-r--r--   0        0        0    10476 2024-04-06 15:32:51.841237 wellets_cli-1.9.2/wellets_cli/commands/asset.py
+-rw-r--r--   0        0        0     1497 2024-04-06 15:32:51.841237 wellets_cli-1.9.2/wellets_cli/commands/currency.py
+-rw-r--r--   0        0        0     2000 2024-04-06 15:32:51.841237 wellets_cli-1.9.2/wellets_cli/commands/investment.py
+-rw-r--r--   0        0        0      734 2024-04-06 15:32:51.841237 wellets_cli-1.9.2/wellets_cli/commands/login.py
+-rw-r--r--   0        0        0    11798 2024-04-06 15:32:51.841237 wellets_cli-1.9.2/wellets_cli/commands/portfolio.py
+-rw-r--r--   0        0        0     1446 2024-04-06 15:32:51.841237 wellets_cli-1.9.2/wellets_cli/commands/register.py
+-rw-r--r--   0        0        0     6938 2024-04-06 15:32:51.841237 wellets_cli-1.9.2/wellets_cli/commands/transaction.py
+-rw-r--r--   0        0        0     3648 2024-04-06 15:32:51.841237 wellets_cli-1.9.2/wellets_cli/commands/transfer.py
+-rw-r--r--   0        0        0    12729 2024-04-06 15:32:51.841237 wellets_cli-1.9.2/wellets_cli/commands/wallet.py
+-rw-r--r--   0        0        0      246 2024-04-06 15:32:51.841237 wellets_cli-1.9.2/wellets_cli/commands/whoami.py
+-rw-r--r--   0        0        0      415 2024-04-06 15:32:51.841237 wellets_cli-1.9.2/wellets_cli/config.py
+-rw-r--r--   0        0        0     4510 2024-04-06 15:32:51.841237 wellets_cli-1.9.2/wellets_cli/model.py
+-rw-r--r--   0        0        0      479 2024-04-06 15:32:51.841237 wellets_cli-1.9.2/wellets_cli/prompt.py
+-rw-r--r--   0        0        0     9218 2024-04-06 15:32:51.841237 wellets_cli-1.9.2/wellets_cli/question.py
+-rw-r--r--   0        0        0     4250 2024-04-06 15:32:51.841237 wellets_cli-1.9.2/wellets_cli/util.py
+-rw-r--r--   0        0        0     6677 2024-04-06 15:32:51.841237 wellets_cli-1.9.2/wellets_cli/validator.py
+-rw-r--r--   0        0        0      717 1970-01-01 00:00:00.000000 wellets_cli-1.9.2/PKG-INFO
```

### Comparing `wellets_cli-1.9.1/LICENSE` & `wellets_cli-1.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wellets_cli-1.9.1/pyproject.toml` & `wellets_cli-1.9.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 [tool.poetry]
 name = "wellets_cli"
-version = "1.9.1"
+version = "1.9.2"
 description = "wellets-cli is the command line interface for Wellets, a crypto-oriented financial management tool that allows you to keep your money under control."
 authors = ["lparolari"]
+include = ["settings.toml"]
 
 [tool.poetry.dependencies]
 python = "^3.12"
 python-dotenv = "^1"
 requests = "^2"
 pydantic = "^2"
 click = "^8"
```

### Comparing `wellets_cli-1.9.1/wellets_cli/api.py` & `wellets_cli-1.9.2/wellets_cli/api.py`

 * *Files identical despite different names*

### Comparing `wellets_cli-1.9.1/wellets_cli/auth.py` & `wellets_cli-1.9.2/wellets_cli/auth.py`

 * *Files identical despite different names*

### Comparing `wellets_cli-1.9.1/wellets_cli/chart.py` & `wellets_cli-1.9.2/wellets_cli/chart.py`

 * *Files 13% similar despite different names*

```diff
@@ -75,15 +75,17 @@
     ax.set_ylabel(ylabel)
 
     return fig
 
 
 def plot_exposition(fig, exposition: float):
     ax = fig.gca()
-    ax.axhline(y=exposition, color="black", linestyle="--", label="Exposition")
+    ax.axhline(
+        y=exposition, color="black", linestyle="--", label="Exposition", linewidth=0.8
+    )
 
     xmin, _ = ax.get_xlim()
 
     ax.annotate(
         f"{exposition:.2f}",
         (xmin, exposition),
         xytext=(0, 4),
@@ -96,20 +98,30 @@
 def plot_position(fig, date, position, size, kind):
     markersize = mpl.rcParams["lines.markersize"] ** 2
 
     xs = np.array(date)
     ys = np.array(position)
     color = np.array(["green" if k == "buy" else "red" for k in kind])
     size = markersize / 4 + 1.2 * np.array(size) * markersize
-    ci = 1.96 * np.std(ys) / np.sqrt(len(xs))
 
     ax = fig.gca()
 
     ax.scatter(xs, ys, s=size, color=color)
-    ax.fill_between(xs, (ys - ci), (ys + ci), color="b", alpha=0.1)
+
+    return fig
+
+
+def plot_ema(fig, x, y, window, color):
+    ax = fig.gca()
+
+    y = np.array(y)
+    y = np.convolve(y, np.ones(window), "valid") / window
+    x = x[window - 1 :]
+
+    ax.plot(x, y, label=f"EMA {window}", linewidth=0.6, linestyle="--", color=color)
 
     return fig
 
 
 def xdate_fmt(fig):
     from matplotlib.dates import DateFormatter
```

### Comparing `wellets_cli-1.9.1/wellets_cli/cli.py` & `wellets_cli-1.9.2/wellets_cli/cli.py`

 * *Files identical despite different names*

### Comparing `wellets_cli-1.9.1/wellets_cli/commands/accumulation.py` & `wellets_cli-1.9.2/wellets_cli/commands/accumulation.py`

 * *Files identical despite different names*

### Comparing `wellets_cli-1.9.1/wellets_cli/commands/asset.py` & `wellets_cli-1.9.2/wellets_cli/commands/asset.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 import wellets_cli.api as api
 from wellets_cli.auth import get_auth_token
 from wellets_cli.chart import (
     mk_fig,
     plot_allocation,
     plot_balance,
+    plot_ema,
     plot_exposition,
     plot_position,
     plot_price,
     show_chart,
     xdate_fmt,
 )
 from wellets_cli.config import settings
@@ -292,15 +293,19 @@
         price_date,
         price,
         label=currency.acronym,
         ylabel=f"Price ({base_currency.acronym})",
     )
     fig = plot_exposition(fig, exposition.average_load_price)
     fig = plot_position(fig, position_date, position, size, kind)
+    fig = plot_ema(fig, price_date, price, window=30, color="orange")
+    fig = plot_ema(fig, price_date, price, window=100, color="orchid")
     fig = xdate_fmt(fig)
+    ax = fig.gca()
+    ax.legend()
     show_chart(fig)
 
 
 @asset.command(name="capital-gain")
 @click.option("--auth-token")
 @click.option("--asset-id")
 def show_capital_gain(auth_token, asset_id):
```

### Comparing `wellets_cli-1.9.1/wellets_cli/commands/currency.py` & `wellets_cli-1.9.2/wellets_cli/commands/currency.py`

 * *Files identical despite different names*

### Comparing `wellets_cli-1.9.1/wellets_cli/commands/investment.py` & `wellets_cli-1.9.2/wellets_cli/commands/investment.py`

 * *Files identical despite different names*

### Comparing `wellets_cli-1.9.1/wellets_cli/commands/login.py` & `wellets_cli-1.9.2/wellets_cli/commands/login.py`

 * *Files 17% similar despite different names*

```diff
@@ -24,8 +24,8 @@
         password
         or settings.get("api_password")
         or inquirer.secret(message="Password").execute()
     )
 
     user_session = api.login(email, password)
 
-    persist_auth(user_session.json())
+    persist_auth(user_session.model_dump_json())
```

### Comparing `wellets_cli-1.9.1/wellets_cli/commands/portfolio.py` & `wellets_cli-1.9.2/wellets_cli/commands/portfolio.py`

 * *Files identical despite different names*

### Comparing `wellets_cli-1.9.1/wellets_cli/commands/register.py` & `wellets_cli-1.9.2/wellets_cli/commands/register.py`

 * *Files identical despite different names*

### Comparing `wellets_cli-1.9.1/wellets_cli/commands/transaction.py` & `wellets_cli-1.9.2/wellets_cli/commands/transaction.py`

 * *Files identical despite different names*

### Comparing `wellets_cli-1.9.1/wellets_cli/commands/transfer.py` & `wellets_cli-1.9.2/wellets_cli/commands/transfer.py`

 * *Files identical despite different names*

### Comparing `wellets_cli-1.9.1/wellets_cli/commands/wallet.py` & `wellets_cli-1.9.2/wellets_cli/commands/wallet.py`

 * *Files identical despite different names*

### Comparing `wellets_cli-1.9.1/wellets_cli/model.py` & `wellets_cli-1.9.2/wellets_cli/model.py`

 * *Files identical despite different names*

### Comparing `wellets_cli-1.9.1/wellets_cli/question.py` & `wellets_cli-1.9.2/wellets_cli/question.py`

 * *Files identical despite different names*

### Comparing `wellets_cli-1.9.1/wellets_cli/util.py` & `wellets_cli-1.9.2/wellets_cli/util.py`

 * *Files identical despite different names*

### Comparing `wellets_cli-1.9.1/wellets_cli/validator.py` & `wellets_cli-1.9.2/wellets_cli/validator.py`

 * *Files identical despite different names*

### Comparing `wellets_cli-1.9.1/PKG-INFO` & `wellets_cli-1.9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wellets_cli
-Version: 1.9.1
+Version: 1.9.2
 Summary: wellets-cli is the command line interface for Wellets, a crypto-oriented financial management tool that allows you to keep your money under control.
 Author: lparolari
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: click (>=8,<9)
 Requires-Dist: dynaconf (>=3,<4)
```

