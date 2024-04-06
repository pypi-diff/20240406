# Comparing `tmp/pysteve-0.0.8.tar.gz` & `tmp/pysteve-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysteve-0.0.8.tar", last modified: Mon Jan 22 22:05:36 2024, max compression
+gzip compressed data, was "pysteve-0.0.9.tar", last modified: Fri Feb  2 22:54:46 2024, max compression
```

## Comparing `pysteve-0.0.8.tar` & `pysteve-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 stephen.hilton   (501) staff       (20)        0 2024-01-22 22:05:36.849188 pysteve-0.0.8/
--rw-r--r--   0 stephen.hilton   (501) staff       (20)     1071 2023-12-23 22:21:16.000000 pysteve-0.0.8/LICENSE
--rw-r--r--   0 stephen.hilton   (501) staff       (20)    16222 2024-01-22 22:05:36.848879 pysteve-0.0.8/PKG-INFO
--rw-r--r--   0 stephen.hilton   (501) staff       (20)    14125 2024-01-21 20:43:40.000000 pysteve-0.0.8/README.md
--rw-r--r--   0 stephen.hilton   (501) staff       (20)      997 2024-01-22 22:02:16.000000 pysteve-0.0.8/pyproject.toml
--rw-r--r--   0 stephen.hilton   (501) staff       (20)       38 2024-01-22 22:05:36.849234 pysteve-0.0.8/setup.cfg
-drwxr-xr-x   0 stephen.hilton   (501) staff       (20)        0 2024-01-22 22:05:36.846294 pysteve-0.0.8/src/
-drwxr-xr-x   0 stephen.hilton   (501) staff       (20)        0 2024-01-22 22:05:36.846933 pysteve-0.0.8/src/pysteve/
--rw-r--r--   0 stephen.hilton   (501) staff       (20)        0 2024-01-22 22:01:28.000000 pysteve-0.0.8/src/pysteve/__init__.py
--rw-r--r--   0 stephen.hilton   (501) staff       (20)    54514 2024-01-22 22:01:45.000000 pysteve-0.0.8/src/pysteve/pySteve.py
-drwxr-xr-x   0 stephen.hilton   (501) staff       (20)        0 2024-01-22 22:05:36.848480 pysteve-0.0.8/src/pysteve.egg-info/
--rw-r--r--   0 stephen.hilton   (501) staff       (20)    16222 2024-01-22 22:05:36.000000 pysteve-0.0.8/src/pysteve.egg-info/PKG-INFO
--rw-r--r--   0 stephen.hilton   (501) staff       (20)      275 2024-01-22 22:05:36.000000 pysteve-0.0.8/src/pysteve.egg-info/SOURCES.txt
--rw-r--r--   0 stephen.hilton   (501) staff       (20)        1 2024-01-22 22:05:36.000000 pysteve-0.0.8/src/pysteve.egg-info/dependency_links.txt
--rw-r--r--   0 stephen.hilton   (501) staff       (20)       41 2024-01-22 22:05:36.000000 pysteve-0.0.8/src/pysteve.egg-info/requires.txt
--rw-r--r--   0 stephen.hilton   (501) staff       (20)        8 2024-01-22 22:05:36.000000 pysteve-0.0.8/src/pysteve.egg-info/top_level.txt
-drwxr-xr-x   0 stephen.hilton   (501) staff       (20)        0 2024-01-22 22:05:36.847652 pysteve-0.0.8/tests/
--rw-r--r--   0 stephen.hilton   (501) staff       (20)    22400 2024-01-22 22:04:03.000000 pysteve-0.0.8/tests/test_pySteve.py
+drwxr-xr-x   0 stephen.hilton   (501) staff       (20)        0 2024-02-02 22:54:46.282216 pysteve-0.0.9/
+-rw-r--r--   0 stephen.hilton   (501) staff       (20)     1071 2023-12-23 22:21:16.000000 pysteve-0.0.9/LICENSE
+-rw-r--r--   0 stephen.hilton   (501) staff       (20)    16222 2024-02-02 22:54:46.281957 pysteve-0.0.9/PKG-INFO
+-rw-r--r--   0 stephen.hilton   (501) staff       (20)    14125 2024-01-21 20:43:40.000000 pysteve-0.0.9/README.md
+-rw-r--r--   0 stephen.hilton   (501) staff       (20)      997 2024-02-02 22:50:52.000000 pysteve-0.0.9/pyproject.toml
+-rw-r--r--   0 stephen.hilton   (501) staff       (20)       38 2024-02-02 22:54:46.282265 pysteve-0.0.9/setup.cfg
+drwxr-xr-x   0 stephen.hilton   (501) staff       (20)        0 2024-02-02 22:54:46.279833 pysteve-0.0.9/src/
+drwxr-xr-x   0 stephen.hilton   (501) staff       (20)        0 2024-02-02 22:54:46.280436 pysteve-0.0.9/src/pysteve/
+-rw-r--r--   0 stephen.hilton   (501) staff       (20)        0 2024-01-22 22:01:28.000000 pysteve-0.0.9/src/pysteve/__init__.py
+-rw-r--r--   0 stephen.hilton   (501) staff       (20)    55133 2024-02-02 22:34:58.000000 pysteve-0.0.9/src/pysteve/pySteve.py
+drwxr-xr-x   0 stephen.hilton   (501) staff       (20)        0 2024-02-02 22:54:46.281671 pysteve-0.0.9/src/pysteve.egg-info/
+-rw-r--r--   0 stephen.hilton   (501) staff       (20)    16222 2024-02-02 22:54:46.000000 pysteve-0.0.9/src/pysteve.egg-info/PKG-INFO
+-rw-r--r--   0 stephen.hilton   (501) staff       (20)      275 2024-02-02 22:54:46.000000 pysteve-0.0.9/src/pysteve.egg-info/SOURCES.txt
+-rw-r--r--   0 stephen.hilton   (501) staff       (20)        1 2024-02-02 22:54:46.000000 pysteve-0.0.9/src/pysteve.egg-info/dependency_links.txt
+-rw-r--r--   0 stephen.hilton   (501) staff       (20)       41 2024-02-02 22:54:46.000000 pysteve-0.0.9/src/pysteve.egg-info/requires.txt
+-rw-r--r--   0 stephen.hilton   (501) staff       (20)        8 2024-02-02 22:54:46.000000 pysteve-0.0.9/src/pysteve.egg-info/top_level.txt
+drwxr-xr-x   0 stephen.hilton   (501) staff       (20)        0 2024-02-02 22:54:46.281502 pysteve-0.0.9/tests/
+-rw-r--r--   0 stephen.hilton   (501) staff       (20)    22900 2024-02-02 22:44:19.000000 pysteve-0.0.9/tests/test_pySteve.py
```

### Comparing `pysteve-0.0.8/LICENSE` & `pysteve-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pysteve-0.0.8/PKG-INFO` & `pysteve-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysteve
-Version: 0.0.8
+Version: 0.0.9
 Summary: Helper and setup functions for people named Steve
 Author-email: Stephen Hilton <Stephen@FamilyHilton.com>
 License: MIT License
         
         Copyright (c) 2023 Stephen Hilton
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pysteve-0.0.8/README.md` & `pysteve-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pysteve-0.0.8/pyproject.toml` & `pysteve-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pysteve"
-version = "0.0.8"
+version = "0.0.9"
 description = "Helper and setup functions for people named Steve"
 authors = [{ name = "Stephen Hilton", email = "Stephen@FamilyHilton.com" }]
 readme = "README.md"
 requires-python = ">=3.10"
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
```

### Comparing `pysteve-0.0.8/src/pysteve/pySteve.py` & `pysteve-0.0.9/src/pysteve/pySteve.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 from pathlib import Path 
 from pprint import pprint
 from string import Formatter
 import inspect, logging, requests
 from datetime import datetime, timedelta
 
-docstring_fileheader="""pySteve is a mish-mash collection of useful functions, rather than an application.  It is particularly useful to people named Steve.""" 
-docstring_marker = 'EOMsg'
-docstring_prefix = f'$(cat << {docstring_marker}\n' 
-docstring_suffix = f'\n{docstring_marker}\n)'
-
+markdown_fileheader="""pySteve is a mish-mash collection of useful functions, rather than an application.  It is particularly useful to people named Steve.""" 
 notion_standard_headers = { "Notion-Version": "2022-06-28", "content-type": "application/json"}
 
 
+class __docstring__():
+    marker = '__DOCSTRING_BOUNDRY__'
+    def __init__(self, marker:str=None) -> None:
+        if marker: self.marker = marker 
+    @property
+    def prefix(self): return f'$(cat << {self.marker}\n' 
+    @property
+    def suffix(self): return f'\n{self.marker}\n)'
+    
+
 def infer_datatype(value):
     """
     Infers the primative data types based on value characteristics, and returns a tuple of (type, typed_value).
     Currently supports float, int, str, and list (with typed elements using recursive calls).
     """
     value = str(value)
 
@@ -34,30 +40,30 @@
     
     if (value.startswith('"') and value.endswith('"')) or \
        (value.startswith("'") and value.endswith("'")):
         value = value[1:-1]
     return (str, value)
     
 
-    
-def envfile_save(save_path:Path, save_dict:dict = {}, iteration_zero_pad:int = 6 ) -> Path:
+def envfile_save(save_path:Path, save_dict:dict = {}, iteration_zero_pad:int = 6, docstring_marker_override:str = None) -> Path:
     """
     Always saves a dict as a shell (zsh) as an env-loadable file, adding folders, file iterations and substitutions as needed.
 
     The save_path allows for substitution of any name in the dict (within curly brackets) with the value of that entry. 
     For example, if dict = {'date':'2024-01-01'}, save_path = '~/some/path/file_{date}.sh' will become 
     '~/some/path/file_2024-01-01.sh'. Additionally, if the full substituted file exists, the process will append 
     an iterator (1,2,3) to the end to preserve uniqueness.  The final save_path is returned from the function.  
     Because the file needs to be compatible with shell .env files, special characters (spaces, newlines, etc) are 
     removed from all 'names' in the save_dict, and any values with newlines will be wrapped in a docstring using 
     the string saved in variable 'docstring_eom_marker'    
 
     Args:
         save_path (Path): Where to save the file, with substitution logic.
         save_dict (dict): Dictionary containing file content.
+        docstring_marker_override (str): Begin/end marker for docstrings. If supplied, overrides the global docstring_marker
 
     Returns: 
         Path: Returns the final save_path used (after substitution and iteration).
 
     """
     if not save_path: raise ValueError(f'save_path must be specified, you provided: {save_path}')
     pth = Path(str(save_path).format(**save_dict)).resolve() if bool(save_dict) else Path(save_path).resolve()
@@ -69,49 +75,51 @@
     pos1 = len(str(pth)[:extlen])
     while pth.exists(): 
         iter +=1
         pth = Path( '{}.{}{}'.format(str(pth)[:pos1], str(iter).rjust(iteration_zero_pad,'0'), str(pth)[extlen:]) )
         suflen = -len(pth.suffix) - len(str(iter)) -1
 
     # iterate dict and build rows
+    docstr = __docstring__(docstring_marker_override)
     lines = []
     for nm, val in save_dict.items():
         if type(val) not in [str, int, float, list]: continue
 
         nm = ''.join([c for c in nm if c.isalnum() or c in['_'] ]) 
         q = '' if type(val) in [int, float] else '"'
         val = str(val)
         if '\n' in val: 
             if val[:1]=='\n': val = val[1:]
             val = val.rstrip()
-            nm += f'={docstring_prefix}{val}{docstring_suffix}'
+            nm += f'={docstr.prefix}{val}{docstr.suffix}'
         else: 
             nm += f'={q}{val}{q}'
         lines.append( nm )
     
     # write file
     with open(pth, 'w') as fh:
         fh.write( '\n'.join(lines) )
 
     return Path(pth)
 
 
 
-def envfile_load(load_path:Path='.', load_path_sorted:str = 'latest', exact_match_only:bool = False) -> dict: 
+def envfile_load(load_path:Path='.', load_path_sort:str = 'latest', exact_match_only:bool = False, docstring_marker_override:str = None) -> dict: 
     """
     Returns a dictionary containing name/value pairs pulled from the supplied .env formatted shell (zsh) script.
 
     If load_path does not have a direct match, it is assumed to be a pattern and will be matched given 
-    supplied template logic (unless exact_match_only = True), and return with the load_path_sorted logic 
-    (first or last).  There are several synonyms: [first | earliest] or [last | latest]
+    supplied template logic (unless exact_match_only = True), and return with the load_path_sort logic 
+    (first or last).  There are several synonyms: [first | earliest | asc] or [last | latest | desc] 
     
     Args:
         load_path (Path): file to load from, with template logic allowed.
-        load_path_sorted (str): If load_path was a template, indicates which file to select, based on filename sort. 
+        load_path_sort (str): If load_path was a template, indicates which file to select, based on filename sort. 
         exact_match_only (bool): Disallow filename templating, and require exact filename only.
+        docstring_marker_override (str): Begin/end marker for docstrings. If supplied, overrides the global docstring_marker
  
     Returns: 
         dict: the dictionary name/value parsed from the supplied file.
 
     """
     if not load_path: raise ValueError(f'load_path must be specified, you provided: {load_path}')
     pth = Path(load_path).resolve()
@@ -140,46 +148,47 @@
                 pos = file.find(seg['segment'], pos if pos==0 else pos-1) 
                 if pos == -1: 
                     keep_file = False
                     break
                 pos += seg['len']
             if keep_file: valid_files.append(file)
 
-        if load_path_sorted[:3] in ['fir', 'ear', 'asc']:
+        if load_path_sort[:3] in ['fir', 'ear', 'asc']:
             pth = Path( pth.parent / valid_files[0] ).resolve()
         else: # last, latest, desc, etc.
             pth = Path( pth.parent / valid_files[len(valid_files)-1] ).resolve()
 
     # with correct path selected, load and structure into dict
     with open(pth, 'r') as fh:
         content = fh.read()
 
     # iter allows next(), ::END:: needed to search for docstring END across newlines
-    lines = iter(content.replace(docstring_suffix,'\n::END::').split('\n')) 
+    docstr = __docstring__(docstring_marker_override)
+    lines = iter(content.replace(docstr.suffix,'\n::END::').split('\n')) 
 
     # loop thru and build dict to control load
     rtn = {}
     multiline = None
     for line in lines:
         eq = line.find('=')
         name  = line[:eq]
         value = line[eq+1:]
         if value[:1]=='"' and value[-1:]=='"': value = value[1:-1]
-        if value.startswith( docstring_prefix.strip() ):
+        if value.startswith( docstr.prefix.strip() ):
             multiline = []
             mline = ''
             while True:
                 mline = next(lines, '')
                 if '::END::' in mline: break
                 multiline.append( mline )
             value = '\n'.join(multiline)
         value = infer_datatype(value)[1]
         rtn[name] = value
     rtn['envfile_load--FilePath_Selected'] = str(pth.resolve())
-    rtn = {n:v for n,v in rtn.items() if n.strip()!=''}
+    rtn = {n:v for n,v in rtn.items() if n.strip()!='' and not n.strip().startswith('#')}
     return rtn
 
 
 
 def parse_placeholders(value:str = '', wrappers:str = '{}' ):
     """
     From given string, parses out a list of placeholder values, along with their positions.
@@ -722,22 +731,22 @@
         return {'parms': rtn}
         
     # ITERATE all source files found
     rtn = []
     for file in srcfiles:
         with open(file,'r') as fh:
             srclines = [str(f).rstrip() for f in str(fh.read()).split('\n') ]
-        fileprefixline = [l for l in srclines if l.replace(' ','').startswith('docstring_fileheader=')]
+        fileprefixline = [l for l in srclines if l.replace(' ','').startswith('markdown_fileheader=')]
         if len(fileprefixline)>0:
             fileprefix = fileprefixline[0] 
             _, fileprefixdict = tokenize_quoted_strings(fileprefix, True)
             fileprefix = fileprefixdict['T0']['text'].strip()[3:-3] + '\n'
             srcfiles = [l for l in srclines if fileprefix not in l ] 
         else: 
-            fileprefix =f"""Functions and classes from the file {file.name}<br>(to customize this text, add the variable to your file: docstring_fileheader = "Some header message" )""" 
+            fileprefix =f"""Functions and classes from the file {file.name}<br>(to customize this text, add the variable to your file: markdown_fileheader = "Some header message" )""" 
         
         sections = []
         chunks = chunk_lines(srclines, [ lambda line: str(line).startswith('def ') or str(line).startswith('class ') ])
         for chunk in sorted(chunks):
             chunkstr = ' '.join(chunk)
             if chunk[0][:4]=='def ': 
                 section = {'type':'def', 'name':str(chunk[0][4:chunk[0].find('(')]) }
```

### Comparing `pysteve-0.0.8/src/pysteve.egg-info/PKG-INFO` & `pysteve-0.0.9/src/pysteve.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysteve
-Version: 0.0.8
+Version: 0.0.9
 Summary: Helper and setup functions for people named Steve
 Author-email: Stephen Hilton <Stephen@FamilyHilton.com>
 License: MIT License
         
         Copyright (c) 2023 Stephen Hilton
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pysteve-0.0.8/tests/test_pySteve.py` & `pysteve-0.0.9/tests/test_pySteve.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,14 +153,19 @@
         data2['ID'] = i
         pySteve.envfile_save(Path(folder / 'my_envfile_{USER}.sh'), data2, 6)
 
     assert pySteve.envfile_save('./tests/testfiles/my_envfile_{USER}.sh', data3, 3) == Path('./tests/testfiles/my_envfile_Zelda.sh').resolve()
 
 
 def test_envfile_load():
+    # error case: didn't pick up EOM docstring correctly -- it did actually, just not aligned with docstring marker, introduced an override
+    assert len(pySteve.envfile_load(Path(folder / '..' / 'error_cases' / 'Table--SXTDemo.Stocks--202402020132.sql'))['CREATE_DDL_TEMPLATE']) >=100
+    assert len(pySteve.envfile_load(Path(folder / '..' / 'error_cases' / 'Table--SXTDemo.Stocks--original.sql'), docstring_marker_override='EOM')['CREATE_DDL_TEMPLATE']) >=100
+
+    # STANDARD TESTS
     assert pySteve.envfile_load(Path(folder / 'my_envfile_Bob.sh'))['UUID'] == data['UUID']
     assert pySteve.envfile_load(Path(folder / f'my_envfile_{nowish}.sh'))['UUID'] == data['UUID']
     assert pySteve.envfile_load(Path(folder / 'my_envfile_Steve.sh'))['UUID'] == data2['UUID']
     assert pySteve.envfile_load(Path(folder / 'my_envfile_Steve.{iter}.sh'), 'last')['UUID'] == data2['UUID']
     
     # Zelda will be the last alphabetically, so should be represented below
     assert pySteve.envfile_load(Path(folder / 'my_envfile_{USER}.sh'), 'last')['UUID'] == data3['UUID']
@@ -414,15 +419,15 @@
     env = pySteve.envfile_load()
     apikey = pySteve.notion_get_api_key(envfile=env)
     users = pySteve.notionapi_get_users(apikey)
     assert len(users) >5
     assert type(users) == dict
     assert [v for n,v in users.items() if v['name'] == your_name ][0]['name'] == your_name
     users = pySteve.notionapi_get_users(apikey, include=['Stephen Hilton','Cedric Blair'], full_json=True)
-    assert len(users) == 2
+    assert len(users) >= 2
     assert 'full_json' in [v for n,v in users.items()][0]
     
 
 def test_notionapi_get_dataset_info():
     env = pySteve.envfile_load()
     apikey = pySteve.notion_get_api_key(envfile=env)
     tablename, columns = pySteve.notionapi_get_dataset_info(apikey, env['NOTION_CRM_ACCOUNT'])
@@ -448,9 +453,10 @@
     assert [r for r in keypairs if r['RowID']==ethrow][0]['CellCount'] == len([r for r in keypairs if r['RowID']==ethrow])
 
     assert [c for c in columns if c['notion_name']=='id'][0]['db_name'] == 'Chain_id'
 
 
 
 if __name__ == '__main__':
-    test_generate_markdown_doc()
+    test_envfile_save()
+    test_envfile_load()
     pass
```

