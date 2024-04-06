# Comparing `tmp/nwscript_language_server-0.8.dev0.tar.gz` & `tmp/nwscript_language_server-0.9.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nwscript_language_server-0.8.dev0.tar", max compression
+gzip compressed data, was "nwscript_language_server-0.9.dev0.tar", max compression
```

## Comparing `nwscript_language_server-0.8.dev0.tar` & `nwscript_language_server-0.9.dev0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11367 2024-02-16 00:12:07.757368 nwscript_language_server-0.8.dev0/LICENSE
--rw-r--r--   0        0        0     5622 2024-02-16 00:12:07.757368 nwscript_language_server-0.8.dev0/README.md
--rw-r--r--   0        0        0      122 2024-02-16 00:12:07.757368 nwscript_language_server-0.8.dev0/nwscript_language_server/__init__.py
--rw-r--r--   0        0        0     2676 2024-02-16 00:12:07.757368 nwscript_language_server-0.8.dev0/nwscript_language_server/cli.py
--rw-r--r--   0        0        0     4488 2024-02-16 00:12:07.757368 nwscript_language_server-0.8.dev0/nwscript_language_server/markup.py
--rw-r--r--   0        0        0        0 2024-02-16 00:12:07.757368 nwscript_language_server-0.8.dev0/nwscript_language_server/py.typed
--rw-r--r--   0        0        0    11158 2024-02-16 00:12:07.761368 nwscript_language_server-0.8.dev0/nwscript_language_server/server.py
--rw-r--r--   0        0        0      953 2024-02-16 00:12:07.761368 nwscript_language_server-0.8.dev0/pyproject.toml
--rw-r--r--   0        0        0     6424 1970-01-01 00:00:00.000000 nwscript_language_server-0.8.dev0/PKG-INFO
+-rw-r--r--   0        0        0    11367 2024-03-06 22:25:06.590447 nwscript_language_server-0.9.dev0/LICENSE
+-rw-r--r--   0        0        0     6033 2024-03-06 22:25:06.590447 nwscript_language_server-0.9.dev0/README.md
+-rw-r--r--   0        0        0      122 2024-03-06 22:25:06.590447 nwscript_language_server-0.9.dev0/nwscript_language_server/__init__.py
+-rw-r--r--   0        0        0     2676 2024-03-06 22:25:06.590447 nwscript_language_server-0.9.dev0/nwscript_language_server/cli.py
+-rw-r--r--   0        0        0     4747 2024-03-06 22:25:06.590447 nwscript_language_server-0.9.dev0/nwscript_language_server/markup.py
+-rw-r--r--   0        0        0        0 2024-03-06 22:25:06.590447 nwscript_language_server-0.9.dev0/nwscript_language_server/py.typed
+-rw-r--r--   0        0        0    11158 2024-03-06 22:25:06.590447 nwscript_language_server-0.9.dev0/nwscript_language_server/server.py
+-rw-r--r--   0        0        0      953 2024-03-06 22:25:06.594447 nwscript_language_server-0.9.dev0/pyproject.toml
+-rw-r--r--   0        0        0     6835 1970-01-01 00:00:00.000000 nwscript_language_server-0.9.dev0/PKG-INFO
```

### Comparing `nwscript_language_server-0.8.dev0/LICENSE` & `nwscript_language_server-0.9.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `nwscript_language_server-0.8.dev0/README.md` & `nwscript_language_server-0.9.dev0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,44 @@
 # nwscript-lsp
 
+[![PyPI version](https://badge.fury.io/py/nwscript-language-server.svg)](https://badge.fury.io/py/nwscript-language-server)
+
+
 The LSP is built on [pygls](https://github.com/openlawlibrary/pygls) and [rollnw](https://github.com/jd28/rollnw).  It is derived from the [Pygls Playground](https://github.com/openlawlibrary/pygls/tree/main/examples/vscode-playground) and aims, at this point, only to be a tested bed for implementing LSP features.  A more robust implementation will come later maybe integrating with [nasher.cfg](https://github.com/squattingmonk/nasher#nashercfg).  For now only the current document path will be added to the include path of the script context resman.
 
 That the testbed extension is for vscode is out of simplicity, obviously plugins for any LSP client emacs, (neo)vim, etc will be supported.
 
 Currently, it implements:
 * Completions
 * Hover
 * Workspace Diagnostics
 * Document Symbols
 * Signature Help
 
 ## Setup - Neovim
 
-1. Install the language server
+1. Install required package
+   ```
+   python -m pip install rollnw
+   ```
+
+2. Install the language server
    ```
    python -m pip install nwscript-language-server
    ```
 
-1. Make sure ``nwscript-language-server`` is on your PATH!
+Note: Sometimes "--break-system-packages" is needed to install
+   ```
+    python -m pip install --break-system-packages rollnw
+    python -m pip install --break-system-packages nwscript-language-server
+   ```
+
+3. Make sure ``nwscript-language-server`` is on your PATH!
 
-1. Setup neovim config - Obviously people's tastes will differ here and not all of it is fully implemented.
+4. Setup neovim config - Obviously people's tastes will differ here and not all of it is fully implemented.
    ```lua
    require("config.lazy")
 
    vim.api.nvim_exec(
    [[
    autocmd FileType nwscript setlocal lsp
    ]],
@@ -113,43 +127,43 @@
 Open a terminal in the repository's root directory
 
 1. Create a virtual environment
    ```
    python -m venv env
    ```
 
-1. Install pygls
+2. Install pygls
    ```
    python -m pip install -r requirements.txt
    ```
 
 ### Install Client Dependencies
 
 Open terminal in the same directory as this file and execute following commands:
 
 1. Install node dependencies
 
    ```
    npm install
    ```
-1. Compile the extension
+2. Compile the extension
 
    ```
    npm run compile
    ```
    Alternatively you can run `npm run watch` if you are going to be actively working on the extension itself.
 
 ### Run Extension
 
 1. Open this directory in VS Code
 
-1. The playground relies on the [Python extension for VSCode](https://marketplace.visualstudio.com/items?itemName=ms-python.python) for choosing the appropriate Python environment in which to run the example language servers.
+2. The playground relies on the [Python extension for VSCode](https://marketplace.visualstudio.com/items?itemName=ms-python.python) for choosing the appropriate Python environment in which to run the example language servers.
    If you haven't already, you will need to install it and reload the window.
 
-1. Open the Run and Debug view (`ctrl + shift + D`)
+3. Open the Run and Debug view (`ctrl + shift + D`)
 
-1. Select `Launch Client` and press `F5`, this will open a second VSCode window with the `vscode-playground` extension enabled.
+4. Select `Launch Client` and press `F5`, this will open a second VSCode window with the `vscode-playground` extension enabled.
 
-1. You will need to make sure that VSCode is using a virtual environment that contains an installation of `pygls`.
+5. You will need to make sure that VSCode is using a virtual environment that contains an installation of `pygls`.
    The `Python: Select Interpreter` command can be used to pick the correct one.
 
    Alternatively, you can set the `pygls.server.pythonPath` option in the `.vscode/settings.json` file
```

### Comparing `nwscript_language_server-0.8.dev0/nwscript_language_server/cli.py` & `nwscript_language_server-0.9.dev0/nwscript_language_server/cli.py`

 * *Files identical despite different names*

### Comparing `nwscript_language_server-0.8.dev0/nwscript_language_server/markup.py` & `nwscript_language_server-0.9.dev0/nwscript_language_server/markup.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,16 +28,19 @@
         if len(d):
             lines.append("\n\nParameters")
             for i in range(len(d)):
                 lines.append(
                     f"\n* `{nss.type_name(d[i])} {d[i].identifier()}`")
 
         if len(symbol.comment):
-            lines.append(f"\n\n```nwscript\n//{
-                symbol.comment.replace('\n', '\n//')}\n```")
+            lines.append(
+                "\n\n```nwscript\n//{" +
+                symbol.comment.replace('\n', '\n//') +
+                "}\n```"
+            )
 
         lines.append(f"\n```nwscript\n{symbol.view}\n```")
 
         return lsp.MarkupContent(markup_kind, ''.join(lines))
     else:
         # Force plain text if we don't know how to handle a markup kind
         markup_kind = lsp.MarkupKind.PlainText
@@ -48,15 +51,19 @@
         if len(d):
             lines.append("\n\nParameters")
             for i in range(len(d)):
                 lines.append(
                     f"\n* {nss.type_name(d[i])} {d[i].identifier()}")
 
         if len(symbol.comment):
-            lines.append(f"\n\n//{symbol.comment.replace('\n', '\n//')}")
+            lines.append(
+                "\n\n//{" +
+                symbol.comment.replace('\n', '\n//') +
+                "}"
+            )
 
         lines.append(f"\n{symbol.view}")
 
         return lsp.MarkupContent(markup_kind, ''.join(lines))
 
 
 def hover_struct_decl(nss: nws.Nss, symbol: nws.Symbol, markup_kind: lsp.MarkupKind) -> lsp.MarkupContent:
@@ -65,28 +72,35 @@
     if markup_kind == lsp.MarkupKind.Markdown:
         lines.append(f"**struct `{symbol.type}`**")
 
         if symbol.provider is not None:
             lines.append(f"\n* Provided by `{symbol.provider.name()}`")
 
         if len(symbol.comment):
-            lines.append(f"\n\n```nwscript\n//{
-                symbol.comment.replace('\n', '\n//')}\n```")
+            lines.append(
+                "\n\n```nwscript\n//{" +
+                symbol.comment.replace('\n', '\n//') +
+                "}\n```"
+            )
 
         lines.append(f"\n\n```nwscript\nstruct {symbol.type} {{}}\n```")
     else:
         # Force plain text if we don't know how to handle a markup kind
         markup_kind = lsp.MarkupKind.PlainText
         lines.append(f"**struct {symbol.type}**")
 
         if symbol.provider is not None:
             lines.append(f"\n* Provided by '{symbol.provider.name()}'")
 
         if len(symbol.comment):
-            lines.append(f"\n\n//{symbol.comment.replace('\n', '\n//')}")
+            lines.append(
+                "\n\n//{" +
+                symbol.comment.replace('\n', '\n//') +
+                "}"
+            )
 
         lines.append(f"struct {symbol.type} {{}}")
 
     return lsp.MarkupContent(markup_kind, ''.join(lines))
 
 
 def hover_var_decl(symbol: nws.Symbol, markup_kind: lsp.MarkupKind) -> lsp.MarkupContent:
@@ -96,24 +110,26 @@
         kind_str = "param"
     elif symbol.kind == nws.SymbolKind.field:
         kind_str = "field"
     else:
         kind_str = "variable"
 
     if markup_kind == lsp.MarkupKind.Markdown:
-        header = f"**{kind_str} `{symbol.decl.identifier()
-                                  }`: `{symbol.type}`**"
+        header = f"**{kind_str} `{symbol.decl.identifier()}`: `{symbol.type}`**"
         lines.append(header)
 
         if symbol.provider is not None:
             lines.append(f"\n* Provided by `{symbol.provider.name()}`")
 
         if len(symbol.comment):
             lines.append(
-                f"\n\n```nwscript\n//{symbol.comment.replace('\n', '\n//')}\n```")
+                "\n\n```nwscript\n//{" +
+                symbol.comment.replace('\n', '\n//') +
+                "}\n```"
+            )
 
         lines.append(f"\n\n```nwscript\n{symbol.view}\n```")
 
         return lsp.MarkupContent(markup_kind, ''.join(lines))
     else:
         # Force plain text if we don't know how to handle a markup kind
         markup_kind = lsp.MarkupKind.PlainText
```

### Comparing `nwscript_language_server-0.8.dev0/nwscript_language_server/server.py` & `nwscript_language_server-0.9.dev0/nwscript_language_server/server.py`

 * *Files identical despite different names*

### Comparing `nwscript_language_server-0.8.dev0/pyproject.toml` & `nwscript_language_server-0.9.dev0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.7.1"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "nwscript-language-server"
-version = "0.8.dev0"
+version = "0.9.dev0"
 description = "A language server for Bioware's nwscript"
 authors = ["jmd <joshua.m.dean@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/jd28/nwscript-lsp"
 repository = "https://github.com/jd28/nwscript-lsp"
 keywords = [
     "nwscript",
```

### Comparing `nwscript_language_server-0.8.dev0/PKG-INFO` & `nwscript_language_server-0.9.dev0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nwscript-language-server
-Version: 0.8.dev0
+Version: 0.9.dev0
 Summary: A language server for Bioware's nwscript
 Home-page: https://github.com/jd28/nwscript-lsp
 Keywords: nwscript,completion,lsp,language-server-protocol
 Author: jmd
 Author-email: joshua.m.dean@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
@@ -17,35 +17,49 @@
 Requires-Dist: pygls (>=1.2.1,<2.0.0)
 Requires-Dist: rollnw (==0.25.*)
 Project-URL: Repository, https://github.com/jd28/nwscript-lsp
 Description-Content-Type: text/markdown
 
 # nwscript-lsp
 
+[![PyPI version](https://badge.fury.io/py/nwscript-language-server.svg)](https://badge.fury.io/py/nwscript-language-server)
+
+
 The LSP is built on [pygls](https://github.com/openlawlibrary/pygls) and [rollnw](https://github.com/jd28/rollnw).  It is derived from the [Pygls Playground](https://github.com/openlawlibrary/pygls/tree/main/examples/vscode-playground) and aims, at this point, only to be a tested bed for implementing LSP features.  A more robust implementation will come later maybe integrating with [nasher.cfg](https://github.com/squattingmonk/nasher#nashercfg).  For now only the current document path will be added to the include path of the script context resman.
 
 That the testbed extension is for vscode is out of simplicity, obviously plugins for any LSP client emacs, (neo)vim, etc will be supported.
 
 Currently, it implements:
 * Completions
 * Hover
 * Workspace Diagnostics
 * Document Symbols
 * Signature Help
 
 ## Setup - Neovim
 
-1. Install the language server
+1. Install required package
+   ```
+   python -m pip install rollnw
+   ```
+
+2. Install the language server
    ```
    python -m pip install nwscript-language-server
    ```
 
-1. Make sure ``nwscript-language-server`` is on your PATH!
+Note: Sometimes "--break-system-packages" is needed to install
+   ```
+    python -m pip install --break-system-packages rollnw
+    python -m pip install --break-system-packages nwscript-language-server
+   ```
+
+3. Make sure ``nwscript-language-server`` is on your PATH!
 
-1. Setup neovim config - Obviously people's tastes will differ here and not all of it is fully implemented.
+4. Setup neovim config - Obviously people's tastes will differ here and not all of it is fully implemented.
    ```lua
    require("config.lazy")
 
    vim.api.nvim_exec(
    [[
    autocmd FileType nwscript setlocal lsp
    ]],
@@ -134,44 +148,44 @@
 Open a terminal in the repository's root directory
 
 1. Create a virtual environment
    ```
    python -m venv env
    ```
 
-1. Install pygls
+2. Install pygls
    ```
    python -m pip install -r requirements.txt
    ```
 
 ### Install Client Dependencies
 
 Open terminal in the same directory as this file and execute following commands:
 
 1. Install node dependencies
 
    ```
    npm install
    ```
-1. Compile the extension
+2. Compile the extension
 
    ```
    npm run compile
    ```
    Alternatively you can run `npm run watch` if you are going to be actively working on the extension itself.
 
 ### Run Extension
 
 1. Open this directory in VS Code
 
-1. The playground relies on the [Python extension for VSCode](https://marketplace.visualstudio.com/items?itemName=ms-python.python) for choosing the appropriate Python environment in which to run the example language servers.
+2. The playground relies on the [Python extension for VSCode](https://marketplace.visualstudio.com/items?itemName=ms-python.python) for choosing the appropriate Python environment in which to run the example language servers.
    If you haven't already, you will need to install it and reload the window.
 
-1. Open the Run and Debug view (`ctrl + shift + D`)
+3. Open the Run and Debug view (`ctrl + shift + D`)
 
-1. Select `Launch Client` and press `F5`, this will open a second VSCode window with the `vscode-playground` extension enabled.
+4. Select `Launch Client` and press `F5`, this will open a second VSCode window with the `vscode-playground` extension enabled.
 
-1. You will need to make sure that VSCode is using a virtual environment that contains an installation of `pygls`.
+5. You will need to make sure that VSCode is using a virtual environment that contains an installation of `pygls`.
    The `Python: Select Interpreter` command can be used to pick the correct one.
 
    Alternatively, you can set the `pygls.server.pythonPath` option in the `.vscode/settings.json` file
```

