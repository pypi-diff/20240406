# Comparing `tmp/yosemite-tools-0.0.2.tar.gz` & `tmp/yosemite-tools-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yosemite-tools-0.0.2.tar", last modified: Fri Apr  5 14:32:19 2024, max compression
+gzip compressed data, was "yosemite-tools-0.0.3.tar", last modified: Sat Apr  6 03:45:52 2024, max compression
```

## Comparing `yosemite-tools-0.0.2.tar` & `yosemite-tools-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-04-05 14:32:19.832526 yosemite-tools-0.0.2/
--rw-r--r--   0 hammad     (501) staff       (20)      437 2024-04-05 14:32:19.830567 yosemite-tools-0.0.2/PKG-INFO
--rw-r--r--   0 hammad     (501) staff       (20)       38 2024-04-05 14:32:19.832765 yosemite-tools-0.0.2/setup.cfg
--rw-r--r--   0 hammad     (501) staff       (20)      554 2024-04-05 14:32:08.000000 yosemite-tools-0.0.2/setup.py
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-04-05 14:32:19.817744 yosemite-tools-0.0.2/yosemite_tools/
--rw-r--r--   0 hammad     (501) staff       (20)       22 2024-04-05 14:18:10.000000 yosemite-tools-0.0.2/yosemite_tools/__init__.py
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-04-05 14:32:19.827741 yosemite-tools-0.0.2/yosemite_tools/modules/
--rw-r--r--   0 hammad     (501) staff       (20)      160 2024-04-05 14:26:33.000000 yosemite-tools-0.0.2/yosemite_tools/modules/__init__.py
--rw-r--r--   0 hammad     (501) staff       (20)     8880 2024-04-05 14:13:25.000000 yosemite-tools-0.0.2/yosemite_tools/modules/inputs.py
--rw-r--r--   0 hammad     (501) staff       (20)     5614 2024-04-05 14:31:49.000000 yosemite-tools-0.0.2/yosemite_tools/modules/logger.py
--rw-r--r--   0 hammad     (501) staff       (20)     3213 2024-04-05 14:26:59.000000 yosemite-tools-0.0.2/yosemite_tools/modules/preconditions.py
--rw-r--r--   0 hammad     (501) staff       (20)    10620 2024-04-05 14:30:57.000000 yosemite-tools-0.0.2/yosemite_tools/modules/utils.py
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-04-05 14:32:19.829499 yosemite-tools-0.0.2/yosemite_tools.egg-info/
--rw-r--r--   0 hammad     (501) staff       (20)      437 2024-04-05 14:32:19.000000 yosemite-tools-0.0.2/yosemite_tools.egg-info/PKG-INFO
--rw-r--r--   0 hammad     (501) staff       (20)      397 2024-04-05 14:32:19.000000 yosemite-tools-0.0.2/yosemite_tools.egg-info/SOURCES.txt
--rw-r--r--   0 hammad     (501) staff       (20)        1 2024-04-05 14:32:19.000000 yosemite-tools-0.0.2/yosemite_tools.egg-info/dependency_links.txt
--rw-r--r--   0 hammad     (501) staff       (20)       41 2024-04-05 14:32:19.000000 yosemite-tools-0.0.2/yosemite_tools.egg-info/requires.txt
--rw-r--r--   0 hammad     (501) staff       (20)       15 2024-04-05 14:32:19.000000 yosemite-tools-0.0.2/yosemite_tools.egg-info/top_level.txt
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-04-06 03:45:52.173829 yosemite-tools-0.0.3/
+-rw-r--r--   0 hammad     (501) staff       (20)      437 2024-04-06 03:45:52.173249 yosemite-tools-0.0.3/PKG-INFO
+-rw-r--r--   0 hammad     (501) staff       (20)       38 2024-04-06 03:45:52.174010 yosemite-tools-0.0.3/setup.cfg
+-rw-r--r--   0 hammad     (501) staff       (20)      554 2024-04-06 03:45:47.000000 yosemite-tools-0.0.3/setup.py
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-04-06 03:45:52.163761 yosemite-tools-0.0.3/yosemite_tools/
+-rw-r--r--   0 hammad     (501) staff       (20)       22 2024-04-05 14:18:10.000000 yosemite-tools-0.0.3/yosemite_tools/__init__.py
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-04-06 03:45:52.171645 yosemite-tools-0.0.3/yosemite_tools/modules/
+-rw-r--r--   0 hammad     (501) staff       (20)      160 2024-04-05 14:26:33.000000 yosemite-tools-0.0.3/yosemite_tools/modules/__init__.py
+-rw-r--r--   0 hammad     (501) staff       (20)     8880 2024-04-05 14:13:25.000000 yosemite-tools-0.0.3/yosemite_tools/modules/inputs.py
+-rw-r--r--   0 hammad     (501) staff       (20)     6337 2024-04-06 03:45:33.000000 yosemite-tools-0.0.3/yosemite_tools/modules/logger.py
+-rw-r--r--   0 hammad     (501) staff       (20)     3213 2024-04-05 14:26:59.000000 yosemite-tools-0.0.3/yosemite_tools/modules/preconditions.py
+-rw-r--r--   0 hammad     (501) staff       (20)    10620 2024-04-05 14:30:57.000000 yosemite-tools-0.0.3/yosemite_tools/modules/utils.py
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-04-06 03:45:52.172647 yosemite-tools-0.0.3/yosemite_tools.egg-info/
+-rw-r--r--   0 hammad     (501) staff       (20)      437 2024-04-06 03:45:52.000000 yosemite-tools-0.0.3/yosemite_tools.egg-info/PKG-INFO
+-rw-r--r--   0 hammad     (501) staff       (20)      397 2024-04-06 03:45:52.000000 yosemite-tools-0.0.3/yosemite_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 hammad     (501) staff       (20)        1 2024-04-06 03:45:52.000000 yosemite-tools-0.0.3/yosemite_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 hammad     (501) staff       (20)       41 2024-04-06 03:45:52.000000 yosemite-tools-0.0.3/yosemite_tools.egg-info/requires.txt
+-rw-r--r--   0 hammad     (501) staff       (20)       15 2024-04-06 03:45:52.000000 yosemite-tools-0.0.3/yosemite_tools.egg-info/top_level.txt
```

### Comparing `yosemite-tools-0.0.2/setup.py` & `yosemite-tools-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="yosemite-tools",
-    version="0.0.02",
+    version="0.0.03",
     author="Hammad Saeed",
     author_email="hammad@supportvectors.com",
     description="yosemite",
     long_description="""
 Yosemite
     """,
     packages=setuptools.find_packages(),
```

### Comparing `yosemite-tools-0.0.2/yosemite_tools/modules/inputs.py` & `yosemite-tools-0.0.3/yosemite_tools/modules/inputs.py`

 * *Files identical despite different names*

### Comparing `yosemite-tools-0.0.2/yosemite_tools/modules/logger.py` & `yosemite-tools-0.0.3/yosemite_tools/modules/logger.py`

 * *Files 6% similar despite different names*

```diff
@@ -61,67 +61,96 @@
             message (str): The message to be logged.
         """
         time = self.get_datetime()
         self.logger.debug(message)
         if module:
             if self.verbose:
                 self.text.display(f"[bold white]{self.logger.name}[/bold white] - [not bold white]{module}[/not bold white] | [grey not bold]{time}[grey not bold] [bold blue]DEBUG[/bold blue] - [dim grey not bold]{message}[/dim grey not bold]")
-        if self.verbose:
-            self.text.display(f" [bold white]{self.logger.name}[/bold white] | [grey not bold]{time}[grey not bold] [bold blue]DEBUG[/bold blue] - [dim grey not bold]{message}[/dim grey not bold]")
+            else:
+                pass
+        else:
+            if self.verbose:
+                self.text.display(f" [bold white]{self.logger.name}[/bold white] | [grey not bold]{time}[grey not bold] [bold blue]DEBUG[/bold blue] - [dim grey not bold]{message}[/dim grey not bold]")
+            else:
+                pass
 
     def info(self, message, module : Optional[str] = None):
         """
         Log an status message.
 
         Args:
             message (str): The message to be logged.
         """
         time = self.get_datetime()
         self.logger.info(message)
         if module:
             if self.verbose:
                 self.text.display(f"[bold white]{self.logger.name}[/bold white] - [not bold white]{module}[/not bold white] | [grey not bold]{time}[grey not bold] [bold green]INFO[/bold green] - [dim grey not bold]{message}[/dim grey not bold]")
-        if self.verbose:
-            self.text.display(f"[bold white]{self.logger.name}[/bold white] | [grey not bold]{time}[grey not bold] [bold green]INFO[/bold green] - [dim grey not bold]{message}[/dim grey not bold]")
+            else:
+                pass
+        else:
+            if self.verbose:
+                self.text.display(f"[bold white]{self.logger.name}[/bold white] | [grey not bold]{time}[grey not bold] [bold green]INFO[/bold green] - [dim grey not bold]{message}[/dim grey not bold]")
 
     def warning(self, message, module : Optional[str] = None):
         """
         Log a warning message.
 
         Args:
             message (str): The message to be logged.
         """
         time = self.get_datetime()
         self.logger.warning(message)
         if module:
             if self.verbose:
                 self.text.display(f"[bold white]{self.logger.name}[/bold white] - [not bold white]{module}[/not bold white] | [grey not bold]{time}[grey not bold] [bold yellow]WARNING[/bold yellow] - [dim grey not bold]{message}[/dim grey not bold]")
-        if self.verbose:
-            self.text.display(f"[bold white]{self.logger.name}[/bold white] | [grey not bold]{time}[grey not bold] [bold yellow]WARNING[/bold yellow] - [dim grey not bold]{message}[/dim grey not bold]")
+            else:
+                pass
+        else:
+            if self.verbose:
+                self.text.display(f"[bold white]{self.logger.name}[/bold white] | [grey not bold]{time}[grey not bold] [bold yellow]WARNING[/bold yellow] - [dim grey not bold]{message}[/dim grey not bold]")
+            else:
+                pass
 
     def error(self, message, module : Optional[str] = None):
         """
         Log an error message.
 
         Args:
             message (str): The message to be logged.
         """
         time = self.get_datetime()
         self.logger.error(message)
         if module:
             if self.verbose:
                 self.text.display(f"[bold white]{self.logger.name}[/bold white] - [not bold white]{module}[/not bold white] | [grey not bold]{time}[grey not bold] [bold red]ERROR[/bold red] - [dim grey not bold]{message}[/dim grey not bold]")
-        if self.verbose:
-            self.text.display(f"[bold white]{self.logger.name}[/bold white] | [grey not bold]{time}[grey not bold] [bold red]ERROR[/bold red] - [dim grey not bold]{message}[/dim grey not bold]")
+            else:
+                pass
+        else:
+            if self.verbose:
+                self.text.display(f"[bold white]{self.logger.name}[/bold white] | [grey not bold]{time}[grey not bold] [bold red]ERROR[/bold red] - [dim grey not bold]{message}[/dim grey not bold]")
+            else:
+                pass
 
     def critical(self, message, module : Optional[str] = None):
         """
         Log a critical message.
 
         Args:
             message (str): The message to be logged.
         """
         time = self.get_datetime()
         self.logger.critical(message)
         if module:
             self.text.display(f"[bold white]{self.logger.name}[/bold white] - [not bold white]{module}[/not bold white] | [grey not bold]{time}[grey not bold] [bold dark_red]CRITICAL[/bold dark_red] - [dim grey not bold]{message}[/dim grey not bold]")
-        self.text.display(f"[bold white]{self.logger.name}[/bold white] | [grey not bold]{time}[grey not bold] [bold dark_red]CRITICAL[/bold dark_red] - [dim grey not bold]{message}[/dim grey not bold]")
+        else:
+            self.text.display(f"[bold white]{self.logger.name}[/bold white] | [grey not bold]{time}[grey not bold] [bold dark_red]CRITICAL[/bold dark_red] - [dim grey not bold]{message}[/dim grey not bold]")
+
+
+if __name__ == "__main__":
+    logger = Logger("test", verbose=True)
+    logger.debug("This is a debug message.")
+    logger.info("This is an info message.", module="test")
+    logger.warning("This is a warning message.")
+    logger.error("This is an error message.", module="test")
+    logger.critical("This is a critical message.")
+    pass
```

### Comparing `yosemite-tools-0.0.2/yosemite_tools/modules/preconditions.py` & `yosemite-tools-0.0.3/yosemite_tools/modules/preconditions.py`

 * *Files identical despite different names*

### Comparing `yosemite-tools-0.0.2/yosemite_tools/modules/utils.py` & `yosemite-tools-0.0.3/yosemite_tools/modules/utils.py`

 * *Files identical despite different names*

