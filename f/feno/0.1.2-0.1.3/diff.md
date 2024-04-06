# Comparing `tmp/feno-0.1.2.tar.gz` & `tmp/feno-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feno-0.1.2.tar", last modified: Fri Apr  5 00:33:00 2024, max compression
+gzip compressed data, was "feno-0.1.3.tar", last modified: Sat Apr  6 20:51:25 2024, max compression
```

## Comparing `feno-0.1.2.tar` & `feno-0.1.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-05 00:33:00.316221 feno-0.1.2/
--rw-r--r--   0 lion      (1000) lion      (1000)     1043 2024-03-26 18:23:42.000000 feno-0.1.2/LICENSE
--rw-r--r--   0 lion      (1000) lion      (1000)      191 2024-03-26 18:23:42.000000 feno-0.1.2/MANIFEST.in
--rw-r--r--   0 lion      (1000) lion      (1000)     2322 2024-04-05 00:33:00.316221 feno-0.1.2/PKG-INFO
--rw-r--r--   0 lion      (1000) lion      (1000)     1469 2024-04-05 00:25:42.000000 feno-0.1.2/README.md
--rw-r--r--   0 lion      (1000) lion      (1000)      558 2024-04-04 23:38:13.000000 feno-0.1.2/changelog.md
--rw-r--r--   0 lion      (1000) lion      (1000)      306 2024-04-04 23:06:44.000000 feno-0.1.2/requirements.txt
--rw-r--r--   0 lion      (1000) lion      (1000)       74 2024-04-05 00:33:00.316221 feno-0.1.2/setup.cfg
--rw-r--r--   0 lion      (1000) lion      (1000)     3107 2024-04-01 17:24:14.000000 feno-0.1.2/setup.py
-drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-05 00:33:00.302888 feno-0.1.2/src/
-drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-05 00:33:00.309554 feno-0.1.2/src/feno/
--rw-r--r--   0 lion      (1000) lion      (1000)       22 2024-04-05 00:32:44.000000 feno-0.1.2/src/feno/__init__.py
--rw-r--r--   0 lion      (1000) lion      (1000)     2003 2024-04-04 23:51:34.000000 feno-0.1.2/src/feno/__main__.py
--rw-r--r--   0 lion      (1000) lion      (1000)     5188 2024-04-04 23:50:56.000000 feno-0.1.2/src/feno/actions.py
--rw-r--r--   0 lion      (1000) lion      (1000)      550 2024-03-26 19:17:45.000000 feno-0.1.2/src/feno/cases.py
--rw-r--r--   0 lion      (1000) lion      (1000)     1699 2024-04-01 17:39:49.000000 feno-0.1.2/src/feno/check.py
--rw-r--r--   0 lion      (1000) lion      (1000)      938 2024-03-26 19:19:40.000000 feno-0.1.2/src/feno/css_style.py
--rw-r--r--   0 lion      (1000) lion      (1000)     5382 2024-04-03 18:14:31.000000 feno-0.1.2/src/feno/filter.py
--rw-r--r--   0 lion      (1000) lion      (1000)     8485 2024-04-04 23:00:46.000000 feno-0.1.2/src/feno/html.py
--rw-r--r--   0 lion      (1000) lion      (1000)     2494 2024-03-27 13:44:12.000000 feno-0.1.2/src/feno/indexer.py
--rw-r--r--   0 lion      (1000) lion      (1000)     3503 2024-04-05 00:31:13.000000 feno-0.1.2/src/feno/jsontools.py
--rw-r--r--   0 lion      (1000) lion      (1000)      393 2024-04-01 23:10:29.000000 feno-0.1.2/src/feno/log.py
--rw-r--r--   0 lion      (1000) lion      (1000)    11201 2024-04-04 23:37:02.000000 feno-0.1.2/src/feno/mdpp.py
--rw-r--r--   0 lion      (1000) lion      (1000)     4976 2024-04-04 23:15:36.000000 feno-0.1.2/src/feno/remote_md.py
--rw-r--r--   0 lion      (1000) lion      (1000)     1375 2024-04-04 23:31:11.000000 feno-0.1.2/src/feno/tree.py
-drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-05 00:33:00.312888 feno-0.1.2/src/feno.egg-info/
--rw-r--r--   0 lion      (1000) lion      (1000)     2322 2024-04-05 00:33:00.000000 feno-0.1.2/src/feno.egg-info/PKG-INFO
--rw-r--r--   0 lion      (1000) lion      (1000)      542 2024-04-05 00:33:00.000000 feno-0.1.2/src/feno.egg-info/SOURCES.txt
--rw-r--r--   0 lion      (1000) lion      (1000)        1 2024-04-05 00:33:00.000000 feno-0.1.2/src/feno.egg-info/dependency_links.txt
--rw-r--r--   0 lion      (1000) lion      (1000)      144 2024-04-05 00:33:00.000000 feno-0.1.2/src/feno.egg-info/entry_points.txt
--rw-r--r--   0 lion      (1000) lion      (1000)       51 2024-04-05 00:33:00.000000 feno-0.1.2/src/feno.egg-info/requires.txt
--rw-r--r--   0 lion      (1000) lion      (1000)        5 2024-04-05 00:33:00.000000 feno-0.1.2/src/feno.egg-info/top_level.txt
+drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-06 20:51:25.126670 feno-0.1.3/
+-rw-r--r--   0 lion      (1000) lion      (1000)     1043 2024-03-26 18:23:42.000000 feno-0.1.3/LICENSE
+-rw-r--r--   0 lion      (1000) lion      (1000)      191 2024-03-26 18:23:42.000000 feno-0.1.3/MANIFEST.in
+-rw-r--r--   0 lion      (1000) lion      (1000)     2324 2024-04-06 20:51:25.126670 feno-0.1.3/PKG-INFO
+-rw-r--r--   0 lion      (1000) lion      (1000)     1471 2024-04-05 00:38:35.000000 feno-0.1.3/README.md
+-rw-r--r--   0 lion      (1000) lion      (1000)      630 2024-04-06 20:40:49.000000 feno-0.1.3/changelog.md
+-rw-r--r--   0 lion      (1000) lion      (1000)      306 2024-04-04 23:06:44.000000 feno-0.1.3/requirements.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)       74 2024-04-06 20:51:25.130003 feno-0.1.3/setup.cfg
+-rw-r--r--   0 lion      (1000) lion      (1000)     3107 2024-04-01 17:24:14.000000 feno-0.1.3/setup.py
+drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-06 20:51:25.096670 feno-0.1.3/src/
+drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-06 20:51:25.116670 feno-0.1.3/src/feno/
+-rw-r--r--   0 lion      (1000) lion      (1000)       22 2024-04-06 20:40:16.000000 feno-0.1.3/src/feno/__init__.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     2003 2024-04-04 23:51:34.000000 feno-0.1.3/src/feno/__main__.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     5188 2024-04-04 23:50:56.000000 feno-0.1.3/src/feno/actions.py
+-rw-r--r--   0 lion      (1000) lion      (1000)      550 2024-03-26 19:17:45.000000 feno-0.1.3/src/feno/cases.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     1699 2024-04-01 17:39:49.000000 feno-0.1.3/src/feno/check.py
+-rw-r--r--   0 lion      (1000) lion      (1000)      938 2024-03-26 19:19:40.000000 feno-0.1.3/src/feno/css_style.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     5382 2024-04-03 18:14:31.000000 feno-0.1.3/src/feno/filter.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     8925 2024-04-06 20:37:55.000000 feno-0.1.3/src/feno/html.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     2494 2024-03-27 13:44:12.000000 feno-0.1.3/src/feno/indexer.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     3503 2024-04-05 00:31:13.000000 feno-0.1.3/src/feno/jsontools.py
+-rw-r--r--   0 lion      (1000) lion      (1000)      393 2024-04-01 23:10:29.000000 feno-0.1.3/src/feno/log.py
+-rw-r--r--   0 lion      (1000) lion      (1000)    11201 2024-04-04 23:37:02.000000 feno-0.1.3/src/feno/mdpp.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     4976 2024-04-04 23:15:36.000000 feno-0.1.3/src/feno/remote_md.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     1375 2024-04-04 23:31:11.000000 feno-0.1.3/src/feno/tree.py
+drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-06 20:51:25.126670 feno-0.1.3/src/feno.egg-info/
+-rw-r--r--   0 lion      (1000) lion      (1000)     2324 2024-04-06 20:51:25.000000 feno-0.1.3/src/feno.egg-info/PKG-INFO
+-rw-r--r--   0 lion      (1000) lion      (1000)      542 2024-04-06 20:51:25.000000 feno-0.1.3/src/feno.egg-info/SOURCES.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)        1 2024-04-06 20:51:25.000000 feno-0.1.3/src/feno.egg-info/dependency_links.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)      144 2024-04-06 20:51:25.000000 feno-0.1.3/src/feno.egg-info/entry_points.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)       51 2024-04-06 20:51:25.000000 feno-0.1.3/src/feno.egg-info/requires.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)        5 2024-04-06 20:51:25.000000 feno-0.1.3/src/feno.egg-info/top_level.txt
```

### Comparing `feno-0.1.2/LICENSE` & `feno-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `feno-0.1.2/PKG-INFO` & `feno-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feno
-Version: 0.1.2
+Version: 0.1.3
 Summary: feno: Flexible Exercise Notation Organizer
 Home-page: https://github.com/senapk/feno
 Author: David Sena Oliveira
 Author-email: sena@ufc.br
 Project-URL: Bug Reports, https://github.com/senapk/feno/issues
 Project-URL: Source, https://github.com/senapk/feno/
 Keywords: programming,learning
@@ -44,17 +44,17 @@
 
 # pandoc para gerar os htmls
 sudo apt install pandoc
 ```
 
 ## Modo básico
 
-Em uma pasta de nome `label` , crie um arquivo `Readme.md` com o seguinte formato:
+Crie um arquivo `Readme.md` com o seguinte formato:
 
-    # @label - Título da atividade
+    # Título da atividade
 
     A descrição que você quiser
 
     ```txt
     >>>>>>>> teste 1
     entrada
     entrada
@@ -69,20 +69,24 @@
     ========
     saida
     saida
     <<<<<<<<
 
     ```
 
-- O rótulo label pode ser qualquer nome e estar em qualquer lugar do título e a pasta deve ter o mesmo nome do rótulo.
+- A primeira linha é o título da atividade.
 - Você pode inserir quantos testes quiser.
 - Execute o `feno` na pasta local com:
 
 ```bash
 feno .
 ```
 
 Ele vai criar uma pasta `.cache` com:
 
-- `q.html` - Um arquivo html com as questões.
+- `q.html` - Um arquivo html com a descrição do problema.
 - `q.tio` - Um arquivo com as questões no formato tio.
-- `mapi.json` - Um arquivo com o mapeamento dos testes para o moodle.
+- `mapi.json` - Um arquivo com os testes formatado para o moodle, que pode ser utilizado pelo projeto [mula](https://github.com/senapk/mula).
+
+## Utilizando TOC e rascunhos
+
+
```

### Comparing `feno-0.1.2/README.md` & `feno-0.1.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -19,17 +19,17 @@
 
 # pandoc para gerar os htmls
 sudo apt install pandoc
 ```
 
 ## Modo básico
 
-Em uma pasta de nome `label` , crie um arquivo `Readme.md` com o seguinte formato:
+Crie um arquivo `Readme.md` com o seguinte formato:
 
-    # @label - Título da atividade
+    # Título da atividade
 
     A descrição que você quiser
 
     ```txt
     >>>>>>>> teste 1
     entrada
     entrada
@@ -44,20 +44,24 @@
     ========
     saida
     saida
     <<<<<<<<
 
     ```
 
-- O rótulo label pode ser qualquer nome e estar em qualquer lugar do título e a pasta deve ter o mesmo nome do rótulo.
+- A primeira linha é o título da atividade.
 - Você pode inserir quantos testes quiser.
 - Execute o `feno` na pasta local com:
 
 ```bash
 feno .
 ```
 
 Ele vai criar uma pasta `.cache` com:
 
-- `q.html` - Um arquivo html com as questões.
+- `q.html` - Um arquivo html com a descrição do problema.
 - `q.tio` - Um arquivo com as questões no formato tio.
-- `mapi.json` - Um arquivo com o mapeamento dos testes para o moodle.
+- `mapi.json` - Um arquivo com os testes formatado para o moodle, que pode ser utilizado pelo projeto [mula](https://github.com/senapk/mula).
+
+## Utilizando TOC e rascunhos
+
+
```

### Comparing `feno-0.1.2/setup.py` & `feno-0.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `feno-0.1.2/src/feno/__main__.py` & `feno-0.1.3/src/feno/__main__.py`

 * *Files identical despite different names*

### Comparing `feno-0.1.2/src/feno/actions.py` & `feno-0.1.3/src/feno/actions.py`

 * *Files identical despite different names*

### Comparing `feno-0.1.2/src/feno/cases.py` & `feno-0.1.3/src/feno/cases.py`

 * *Files identical despite different names*

### Comparing `feno-0.1.2/src/feno/check.py` & `feno-0.1.3/src/feno/check.py`

 * *Files identical despite different names*

### Comparing `feno-0.1.2/src/feno/css_style.py` & `feno-0.1.3/src/feno/css_style.py`

 * *Files identical despite different names*

### Comparing `feno-0.1.2/src/feno/filter.py` & `feno-0.1.3/src/feno/filter.py`

 * *Files identical despite different names*

### Comparing `feno-0.1.2/src/feno/html.py` & `feno-0.1.3/src/feno/html.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,26 +2,41 @@
 from subprocess import PIPE
 # import markdown
 from .css_style import CssStyle
 
 class HTML:
 
     @staticmethod
+    def remove_css_link_from_html(html_file: str):
+        with open(html_file, "r") as f:
+            content = f.read()
+        output = []
+        for line in content.split("\n"):
+            if not line.startswith('  <link rel="stylesheet"'):
+                output.append(line)
+        with open(html_file, "w") as f:
+            f.write("\n".join(output))
+
+
+
+    @staticmethod
     def generate_html_with_pandoc(title: str, input_file: str, output_file: str, enable_latex: bool):
         fulltitle = title.replace('!', '\\!').replace('?', '\\?')
         cmd = ["pandoc", input_file, '--css', CssStyle.get_file(), '--metadata', 'pagetitle=' + fulltitle,
             '-s', '-o', output_file]
         if enable_latex:
             cmd.append("--mathjax")
         try:
             p = subprocess.Popen(cmd, stdout=PIPE, stderr=PIPE, universal_newlines=True)
             stdout, stderr = p.communicate()
             if stdout != "" or stderr != "":
                 print(stdout)
                 print(stderr)
+            HTML.remove_css_link_from_html(output_file)
+
         except Exception as e:
             print("Erro no comando pandoc:", e)
             exit(1)
 
 #     codehilite_css = """
 # <style>
```

### Comparing `feno-0.1.2/src/feno/indexer.py` & `feno-0.1.3/src/feno/indexer.py`

 * *Files identical despite different names*

### Comparing `feno-0.1.2/src/feno/jsontools.py` & `feno-0.1.3/src/feno/jsontools.py`

 * *Files identical despite different names*

### Comparing `feno-0.1.2/src/feno/mdpp.py` & `feno-0.1.3/src/feno/mdpp.py`

 * *Files identical despite different names*

### Comparing `feno-0.1.2/src/feno/remote_md.py` & `feno-0.1.3/src/feno/remote_md.py`

 * *Files identical despite different names*

### Comparing `feno-0.1.2/src/feno/tree.py` & `feno-0.1.3/src/feno/tree.py`

 * *Files identical despite different names*

### Comparing `feno-0.1.2/src/feno.egg-info/PKG-INFO` & `feno-0.1.3/src/feno.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feno
-Version: 0.1.2
+Version: 0.1.3
 Summary: feno: Flexible Exercise Notation Organizer
 Home-page: https://github.com/senapk/feno
 Author: David Sena Oliveira
 Author-email: sena@ufc.br
 Project-URL: Bug Reports, https://github.com/senapk/feno/issues
 Project-URL: Source, https://github.com/senapk/feno/
 Keywords: programming,learning
@@ -44,17 +44,17 @@
 
 # pandoc para gerar os htmls
 sudo apt install pandoc
 ```
 
 ## Modo básico
 
-Em uma pasta de nome `label` , crie um arquivo `Readme.md` com o seguinte formato:
+Crie um arquivo `Readme.md` com o seguinte formato:
 
-    # @label - Título da atividade
+    # Título da atividade
 
     A descrição que você quiser
 
     ```txt
     >>>>>>>> teste 1
     entrada
     entrada
@@ -69,20 +69,24 @@
     ========
     saida
     saida
     <<<<<<<<
 
     ```
 
-- O rótulo label pode ser qualquer nome e estar em qualquer lugar do título e a pasta deve ter o mesmo nome do rótulo.
+- A primeira linha é o título da atividade.
 - Você pode inserir quantos testes quiser.
 - Execute o `feno` na pasta local com:
 
 ```bash
 feno .
 ```
 
 Ele vai criar uma pasta `.cache` com:
 
-- `q.html` - Um arquivo html com as questões.
+- `q.html` - Um arquivo html com a descrição do problema.
 - `q.tio` - Um arquivo com as questões no formato tio.
-- `mapi.json` - Um arquivo com o mapeamento dos testes para o moodle.
+- `mapi.json` - Um arquivo com os testes formatado para o moodle, que pode ser utilizado pelo projeto [mula](https://github.com/senapk/mula).
+
+## Utilizando TOC e rascunhos
+
+
```

### Comparing `feno-0.1.2/src/feno.egg-info/SOURCES.txt` & `feno-0.1.3/src/feno.egg-info/SOURCES.txt`

 * *Files identical despite different names*

