# Comparing `tmp/pcts-0.0.1.tar.gz` & `tmp/pcts-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pcts-0.0.1.tar", last modified: Sat Apr  6 13:55:01 2024, max compression
+gzip compressed data, was "pcts-0.0.2.tar", last modified: Sat Apr  6 17:35:50 2024, max compression
```

## Comparing `pcts-0.0.1.tar` & `pcts-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-06 13:55:01.088844 pcts-0.0.1/
--rw-r--r--   0 solst      (501) staff       (20)    11337 2024-04-06 12:12:21.000000 pcts-0.0.1/LICENSE
--rw-r--r--   0 solst      (501) staff       (20)      111 2024-04-06 12:12:21.000000 pcts-0.0.1/MANIFEST.in
--rw-r--r--   0 solst      (501) staff       (20)     3583 2024-04-06 13:55:01.088606 pcts-0.0.1/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)     2720 2024-04-06 13:54:53.000000 pcts-0.0.1/README.md
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-06 13:55:01.086621 pcts-0.0.1/pcts/
--rw-r--r--   0 solst      (501) staff       (20)      335 2024-04-06 13:54:16.000000 pcts-0.0.1/pcts/__init__.py
--rw-r--r--   0 solst      (501) staff       (20)     2059 2024-04-06 13:54:16.000000 pcts-0.0.1/pcts/_modidx.py
--rw-r--r--   0 solst      (501) staff       (20)     9364 2024-04-06 13:54:16.000000 pcts-0.0.1/pcts/core.py
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-06 13:55:01.087587 pcts-0.0.1/pcts.egg-info/
--rw-r--r--   0 solst      (501) staff       (20)     3583 2024-04-06 13:55:01.000000 pcts-0.0.1/pcts.egg-info/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)      294 2024-04-06 13:55:01.000000 pcts-0.0.1/pcts.egg-info/SOURCES.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2024-04-06 13:55:01.000000 pcts-0.0.1/pcts.egg-info/dependency_links.txt
--rw-r--r--   0 solst      (501) staff       (20)       30 2024-04-06 13:55:01.000000 pcts-0.0.1/pcts.egg-info/entry_points.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2024-04-06 13:38:33.000000 pcts-0.0.1/pcts.egg-info/not-zip-safe
--rw-r--r--   0 solst      (501) staff       (20)       74 2024-04-06 13:55:01.000000 pcts-0.0.1/pcts.egg-info/requires.txt
--rw-r--r--   0 solst      (501) staff       (20)        5 2024-04-06 13:55:01.000000 pcts-0.0.1/pcts.egg-info/top_level.txt
--rw-r--r--   0 solst      (501) staff       (20)      857 2024-04-06 13:53:03.000000 pcts-0.0.1/settings.ini
--rw-r--r--   0 solst      (501) staff       (20)       38 2024-04-06 13:55:01.088885 pcts-0.0.1/setup.cfg
--rw-r--r--   0 solst      (501) staff       (20)     2585 2024-04-06 12:12:21.000000 pcts-0.0.1/setup.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-06 17:35:50.441098 pcts-0.0.2/
+-rw-r--r--   0 solst      (501) staff       (20)    11337 2024-04-06 12:12:21.000000 pcts-0.0.2/LICENSE
+-rw-r--r--   0 solst      (501) staff       (20)      111 2024-04-06 12:12:21.000000 pcts-0.0.2/MANIFEST.in
+-rw-r--r--   0 solst      (501) staff       (20)     3583 2024-04-06 17:35:50.440850 pcts-0.0.2/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)     2720 2024-04-06 13:54:53.000000 pcts-0.0.2/README.md
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-06 17:35:50.438708 pcts-0.0.2/pcts/
+-rw-r--r--   0 solst      (501) staff       (20)      335 2024-04-06 17:35:47.000000 pcts-0.0.2/pcts/__init__.py
+-rw-r--r--   0 solst      (501) staff       (20)     3009 2024-04-06 17:35:47.000000 pcts-0.0.2/pcts/_modidx.py
+-rw-r--r--   0 solst      (501) staff       (20)    12199 2024-04-06 17:35:47.000000 pcts-0.0.2/pcts/core.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-06 17:35:50.439880 pcts-0.0.2/pcts.egg-info/
+-rw-r--r--   0 solst      (501) staff       (20)     3583 2024-04-06 17:35:50.000000 pcts-0.0.2/pcts.egg-info/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)      294 2024-04-06 17:35:50.000000 pcts-0.0.2/pcts.egg-info/SOURCES.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2024-04-06 17:35:50.000000 pcts-0.0.2/pcts.egg-info/dependency_links.txt
+-rw-r--r--   0 solst      (501) staff       (20)       30 2024-04-06 17:35:50.000000 pcts-0.0.2/pcts.egg-info/entry_points.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2024-04-06 13:38:33.000000 pcts-0.0.2/pcts.egg-info/not-zip-safe
+-rw-r--r--   0 solst      (501) staff       (20)       74 2024-04-06 17:35:50.000000 pcts-0.0.2/pcts.egg-info/requires.txt
+-rw-r--r--   0 solst      (501) staff       (20)        5 2024-04-06 17:35:50.000000 pcts-0.0.2/pcts.egg-info/top_level.txt
+-rw-r--r--   0 solst      (501) staff       (20)      857 2024-04-06 13:55:46.000000 pcts-0.0.2/settings.ini
+-rw-r--r--   0 solst      (501) staff       (20)       38 2024-04-06 17:35:50.441141 pcts-0.0.2/setup.cfg
+-rw-r--r--   0 solst      (501) staff       (20)     2585 2024-04-06 12:12:21.000000 pcts-0.0.2/setup.py
```

### Comparing `pcts-0.0.1/LICENSE` & `pcts-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pcts-0.0.1/PKG-INFO` & `pcts-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pcts
-Version: 0.0.1
+Version: 0.0.2
 Summary: util torch
 Home-page: https://github.com/dsm-72/pcts
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: utility for pytorch torch util pcts
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pcts-0.0.1/README.md` & `pcts-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pcts-0.0.1/pcts/_modidx.py` & `pcts-0.0.2/pcts/_modidx.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,23 +4,33 @@
                 'doc_baseurl': '/pcts',
                 'doc_host': 'https://dsm-72.github.io',
                 'git_url': 'https://github.com/dsm-72/pcts',
                 'lib_path': 'pcts'},
   'syms': { 'pcts.core': { 'pcts.core.accumulate_percents': ('core.html#accumulate_percents', 'pcts/core.py'),
                            'pcts.core.apercents': ('core.html#apercents', 'pcts/core.py'),
                            'pcts.core.asums': ('core.html#asums', 'pcts/core.py'),
+                           'pcts.core.diff_percents': ('core.html#diff_percents', 'pcts/core.py'),
+                           'pcts.core.dpercents': ('core.html#dpercents', 'pcts/core.py'),
                            'pcts.core.idxperm': ('core.html#idxperm', 'pcts/core.py'),
                            'pcts.core.idxstep': ('core.html#idxstep', 'pcts/core.py'),
                            'pcts.core.index_split_by_percents': ('core.html#index_split_by_percents', 'pcts/core.py'),
                            'pcts.core.index_step': ('core.html#index_step', 'pcts/core.py'),
                            'pcts.core.integer_percent': ('core.html#integer_percent', 'pcts/core.py'),
                            'pcts.core.integer_percents': ('core.html#integer_percents', 'pcts/core.py'),
                            'pcts.core.ipercent': ('core.html#ipercent', 'pcts/core.py'),
                            'pcts.core.ipercents': ('core.html#ipercents', 'pcts/core.py'),
+                           'pcts.core.norm_percents': ('core.html#norm_percents', 'pcts/core.py'),
+                           'pcts.core.normalize_percents': ('core.html#normalize_percents', 'pcts/core.py'),
+                           'pcts.core.npcts': ('core.html#npcts', 'pcts/core.py'),
+                           'pcts.core.npercents': ('core.html#npercents', 'pcts/core.py'),
                            'pcts.core.perbounds': ('core.html#perbounds', 'pcts/core.py'),
                            'pcts.core.percent': ('core.html#percent', 'pcts/core.py'),
+                           'pcts.core.percents': ('core.html#percents', 'pcts/core.py'),
                            'pcts.core.permute_indicies': ('core.html#permute_indicies', 'pcts/core.py'),
                            'pcts.core.pidxs': ('core.html#pidxs', 'pcts/core.py'),
                            'pcts.core.pints': ('core.html#pints', 'pcts/core.py'),
                            'pcts.core.range_percents': ('core.html#range_percents', 'pcts/core.py'),
                            'pcts.core.round_percent': ('core.html#round_percent', 'pcts/core.py'),
-                           'pcts.core.rpercents': ('core.html#rpercents', 'pcts/core.py')}}}
+                           'pcts.core.round_percents': ('core.html#round_percents', 'pcts/core.py'),
+                           'pcts.core.rpercents': ('core.html#rpercents', 'pcts/core.py'),
+                           'pcts.core.spercents': ('core.html#spercents', 'pcts/core.py'),
+                           'pcts.core.sum_percents': ('core.html#sum_percents', 'pcts/core.py')}}}
```

### Comparing `pcts-0.0.1/pcts/core.py` & `pcts-0.0.2/pcts/core.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/00_core.ipynb.
 
 # %% auto 0
-__all__ = ['WRAPS_ASSIGN_ANNDOCS', 'percent', 'round_percent', 'ipercent', 'integer_percent', 'ipercents', 'integer_percents',
-           'pints', 'apercents', 'accumulate_percents', 'asums', 'rpercents', 'perbounds', 'range_percents', 'idxstep',
-           'index_step', 'idxperm', 'permute_indicies', 'index_split_by_percents', 'pidxs']
+__all__ = ['WRAPS_ASSIGN_ANNDOCS', 'percent', 'round_percent', 'percents', 'round_percents', 'ipercent', 'integer_percent',
+           'ipercents', 'integer_percents', 'pints', 'spercents', 'sum_percents', 'apercents', 'accumulate_percents',
+           'asums', 'dpercents', 'diff_percents', 'rpercents', 'perbounds', 'range_percents', 'idxstep', 'index_step',
+           'idxperm', 'permute_indicies', 'index_split_by_percents', 'pidxs', 'npercents', 'npcts', 'norm_percents',
+           'normalize_percents']
 
 # %% ../nbs/00_core.ipynb 6
 import random
 from contextlib import redirect_stdout, redirect_stderr
-from functools import wraps
+from functools import wraps, partial
 from itertools import takewhile, accumulate
 from importlib import import_module
 
 # %% ../nbs/00_core.ipynb 8
 from types import FunctionType, ModuleType
 from numbers import Number
 
@@ -62,26 +64,55 @@
     return round(p if (p := abs(p)) < 1 else p / 100, ndigits)
 
 @wraps(percent, assigned=WRAPS_ASSIGN_ANNDOCS)
 def round_percent(p: float, ndigits: int = 3) -> float:
     '''Alias for `percent`.'''
     return percent(p, ndigits)
 
-# %% ../nbs/00_core.ipynb 25
-def ipercent(total: int = 1, p: float = 1., ndigits: int = 3) -> int:
-    '''Calculates the integer part of `p` percent of `total`, 
-    rounded to `ndigits` decimal places.
+# %% ../nbs/00_core.ipynb 24
+def percents(*pcts: float, ndigits: int = 3) -> tuple[float, ...]:
+    '''Converts the percentages `pcts` to a decimal, rounding to `ndigits` decimal places.
     
     Parameters
     ----------
-    total : int, default: 1
-        The total amount to calculate the percentage of.
+    pcts : *float
+        The percentages to convert.
+        
+    ndigits : int, default 3
+        The number of decimal places to round to.
+        
+    Returns
+    -------
+    tuple[float, ...]
+        The converted decimal percentage.
+        
+    See Also
+    --------
+    round_percent : Alias for percent
         
+    '''
+    return tuple(filter(bool, (percent((p or 0), ndigits=ndigits) for p in  pcts)))
+
+@wraps(percents, assigned=WRAPS_ASSIGN_ANNDOCS)
+def round_percents(*pcts: float, ndigits: int = 3) -> tuple[float, ...]:
+    '''Alias for `percent`.'''
+    return percents(*pcts, ndigits=ndigits)
+
+# %% ../nbs/00_core.ipynb 26
+def ipercent(p: float = 1., total: int = 1, ndigits: int = 3) -> int:
+    '''Calculates the integer part of `p` percent of `total`, 
+    rounded to `ndigits` decimal places.
+    
+    Parameters
+    ----------    
     p : float, default: 1.0
         The percentage to calculate.
+        
+    total : int, default: 1
+        The total amount to calculate the percentage of.
 
     ndigits : int, default: 3
         The number of decimal places to round to.
         
     Returns
     -------
     int
@@ -94,33 +125,33 @@
     return int(total * percent(p, ndigits))
 
 @wraps(ipercent, assigned=WRAPS_ASSIGN_ANNDOCS)
 def integer_percent(*args, **kwargs):
     '''Alias for `ipercent`.'''
     return ipercent(*args, **kwargs)
 
-# %% ../nbs/00_core.ipynb 27
+# %% ../nbs/00_core.ipynb 28
 def ipercents(
-    total: int, 
     *percents: float, 
+    total: int = 1, 
     ndigits: int = 3, 
     useall: bool = True, 
     overflow: bool = False,
 ) -> tuple[int, ...]:
     '''Divides total into the corresponding integer values given the
     percents in `*percents` and ensures that all values are used
     
     Parameters
     ----------
-    total : int
-        The total amount to divide according to `percents`.
-        
     *percents : float
         Percentages to divide `total` into.
         
+    total : int
+        The total amount to divide according to `percents`.
+        
     ndigits : int, default: 3
         The number of decimal places to round percentages to.
         
     useall : bool, default: True
         Whether to ensure that the sum of values is equal to `total`.
 
     overflow : bool, default: False
@@ -133,33 +164,42 @@
         The integer values corresponding to the percentages in `percents`.
         
     See Also
     --------
     pints : Alias for `ipercents`
     integer_percents : Alias for `ipercents`
     '''
-    pints = [ipercent(total, pct, ndigits) for pct in percents]    
+    pints = [ipercent(pct, total=total, ndigits=ndigits) for pct in percents]    
     if not overflow and sum(pints) > total: pints.pop()
     if useall and sum(pints) < total: pints.append(total - sum(pints))
     return pints
 
 @wraps(ipercents, assigned=WRAPS_ASSIGN_ANNDOCS)
 def integer_percents(*args, **kwargs):
     '''Alias for `ipercents`.'''
     return ipercents(*args, **kwargs)
 
 @wraps(ipercents, assigned=WRAPS_ASSIGN_ANNDOCS)
 def pints(*args, **kwargs):
     '''Alias for `ipercents`.'''
     return ipercents(*args, **kwargs)
 
-# %% ../nbs/00_core.ipynb 29
+# %% ../nbs/00_core.ipynb 30
+def spercents(*pcts: float, total: int = 1) -> tuple[float, ...]:
+    sums = tuple(takewhile(lambda s: s <= total, accumulate(pcts)))
+    return sums
+
+@wraps(spercents)
+def sum_percents(*pcts, total: int = 1) -> tuple[float, ...]:
+    return spercents(*pcts, total=total)
+
+# %% ../nbs/00_core.ipynb 31
 def apercents(
-    total: int, 
     *percents: float, 
+    total: int = 1, 
     ndigits: int = 3,
     useall: bool = True, 
     overflow: bool = False,
 ) -> tuple[int, ...]:
     '''Accumulate the integer values of the corresponding percentages for `total`.
     
     Parameters
@@ -186,46 +226,57 @@
         Tuples of start and end indices for each percentage of `total`.
         
     See Also
     --------
     accumulate_percents : Alias for `apercents`
     asums : Alias for `apercents`
     '''
-    pints = ipercents(total, *percents, ndigits=ndigits, useall=useall, overflow=overflow)
-    asums = takewhile(lambda s: s <= total, accumulate(pints))
-    return list(asums)
+    pints = ipercents(*percents, total=total, ndigits=ndigits, useall=useall, overflow=overflow)
+    asums = sum_percents(*pints, total=total)
+    # asums = takewhile(lambda s: s <= total, accumulate(pints))
+    return tuple(asums)
 
 @wraps(apercents, assigned=WRAPS_ASSIGN_ANNDOCS)
 def accumulate_percents(*args, **kwargs):
     '''Alias for `apercents`.'''
     return apercents(*args, **kwargs)
 
 @wraps(apercents, assigned=WRAPS_ASSIGN_ANNDOCS)
 def asums(*args, **kwargs):
     '''Alias for `apercents`.'''
     return apercents(*args, **kwargs)
 
-# %% ../nbs/00_core.ipynb 31
+# %% ../nbs/00_core.ipynb 33
+def dpercents(*pcts, sums: tuple[float, ...] | None = None, total: int = 1) -> tuple[float, ...]:
+    if sums is None: sums = sum_percents(*pcts, total=total)
+    diff = tuple((idx-off, idx) for off, idx in zip(pcts, asums))
+    return diff
+
+@wraps(dpercents)
+def diff_percents(*pcts, sums: tuple[float, ...] | None = None, total: int = 1) -> tuple[float, ...]:
+    return dpercents(*pcts, sums=sums, total=total)
+
+# %% ../nbs/00_core.ipynb 34
 def rpercents(
-    total: int, 
     *percents: float, 
+    total: int = 1, 
     ndigits: int = 3,
     useall: bool = True, 
     overflow: bool = False,
 ) -> tuple[tuple[int, int], ...]:
     '''Generates tuples representing ranges based on percentages of `total`.
     
     Parameters
     ----------
-    total : int
-        The total amount to divide according to `percents`.
-        
     *percents : float
         Percentages to divide `total` into.
         
+    total : int
+        The total amount to divide according to `percents`.
+        
     ndigits : int, default: 3
         The number of decimal places to round percentages to.
         
     Returns
     -------
     tuple[tuple[int, int], ...]
         Tuples of start and end indices for each percentage of `total`.
@@ -233,16 +284,16 @@
     See Also
     --------
     range_percents : Alias for `rpercents`
     perbounds : Alias for `rpercents`
     idxstep : Alias for `rpercents`
     index_step : Alias for `rpercents`
     '''
-    pints = ipercents(total, *percents, ndigits=ndigits, useall=useall, overflow=overflow)
-    asums = apercents(total, *percents, ndigits=ndigits, useall=useall, overflow=overflow)
+    pints = ipercents(*percents, total=total, ndigits=ndigits, useall=useall, overflow=overflow)
+    asums = apercents(*percents, total=total, ndigits=ndigits, useall=useall, overflow=overflow)
     return list((idx-off, idx) for off, idx in zip(pints, asums))
 
 @wraps(rpercents, assigned=WRAPS_ASSIGN_ANNDOCS)
 def perbounds(*args, **kwargs):
     '''Alias for `rpercents`.'''
     return rpercents(*args, **kwargs)
 
@@ -258,26 +309,26 @@
 
 
 @wraps(rpercents, assigned=WRAPS_ASSIGN_ANNDOCS)
 def index_step(*args, **kwargs):
     '''Alias for `rpercents`.'''
     return rpercents(*args, **kwargs)
 
-# %% ../nbs/00_core.ipynb 33
-def idxperm(total: int, *percents: float, seed: int = 3) -> tuple[tuple[Number, ...], ...]:
+# %% ../nbs/00_core.ipynb 36
+def idxperm(*percents: float, total: int = 1, seed: int = 3) -> tuple[tuple[Number, ...], ...]:
     '''Generates a permutation of indices divided into segments based on `percents` of `total`.
     
     Parameters
     ----------
-    total : int
-        The total number of indices to permute.
-        
     *percents : float
         The percentages to divide the total indices into.
         
+    total : int
+        The total number of indices to permute.
+        
     seed : int, default 3
         The seed for the random number generator.
         
     Returns
     -------
     tuple[ints, ...]
         nums of indices for each segment based on `percents`.
@@ -288,27 +339,57 @@
     permute_indicies : Alias for `idxperm`.
     index_split_by_percents : Alias for `idxperm`.
     pidxs : Alias for `idxperm`.
     '''
     idx = list(range(total))
     seedall(seed)
     random.shuffle(idx)
-    return tuple(idx[a:b] for a, b in range_percents(total, *percents))
+    return tuple(idx[a:b] for a, b in range_percents(*percents, total=total))
 
 @wraps(idxperm, assigned=WRAPS_ASSIGN_ANNDOCS)
-def permute_indicies(total: int, *percents: float, seed: int = 3) -> tuple[tuple[Number, ...], ...]:
+def permute_indicies(*percents: float, total: int = 1, seed: int = 3) -> tuple[tuple[Number, ...], ...]:
     '''Alias for `idxperm`.'''
-    return idxperm(total, *percents, seed=seed)
+    return idxperm(*percents, total=total, seed=seed)
 
 @wraps(idxperm, assigned=WRAPS_ASSIGN_ANNDOCS)
-def index_split_by_percents(total: int, *percents: float, seed: int = 3) -> tuple[tuple[Number, ...], ...]:
+def index_split_by_percents(*percents: float, total: int = 1, seed: int = 3) -> tuple[tuple[Number, ...], ...]:
     '''Alias for `idxperm`.'''
-    return idxperm(total, *percents, seed=seed)
+    return idxperm(*percents, total=total, seed=seed)
 
 
 @wraps(idxperm, assigned=WRAPS_ASSIGN_ANNDOCS)
-def pidxs(total: int, *percents: float, seed: int = 3) -> tuple[tuple[Number, ...], ...]:
+def pidxs(*percents: float, total: int = 1, seed: int = 3) -> tuple[tuple[Number, ...], ...]:
     '''Alias for `idxperm`.'''
-    return idxperm(total, *percents, seed=seed)
+    return idxperm(*percents, total=total, seed=seed)
+
+# %% ../nbs/00_core.ipynb 38
+def npercents(*pcts, ndigits: int = 3) -> tuple[float, ...]:
+    ps = round_percents(*pcts, ndigits=ndigits)
+    if sum(ps) > 1: ps.pop()        
+    if sum(ps) <= 1: 
+        diff = percent(1 - sum(ps))
+        if len(ps) == len(pcts) or len(ps) == 1: 
+            ps[-1] += diff
+        else: 
+            ps.append(diff)
+    while len(ps) < len(pcts): ps.append(0)
+    return ps
+        
+
+@wraps(npercents, assigned=WRAPS_ASSIGN_ANNDOCS)
+def npcts(*percents: float) -> tuple[float, ...]:
+    '''Alias for `npercents`.'''
+    return npercents(*percents)
+
+@wraps(npercents, assigned=WRAPS_ASSIGN_ANNDOCS)
+def norm_percents(*percents: float) -> tuple[float, ...]:
+    '''Alias for `npercents`.'''
+    return npercents(*percents)
+
+@wraps(npercents, assigned=WRAPS_ASSIGN_ANNDOCS)
+def normalize_percents(*percents: float) -> tuple[float, ...]:
+    '''Alias for `npercents`.'''
+    return npercents(*percents)
+
 
-# %% ../nbs/00_core.ipynb 35
+# %% ../nbs/00_core.ipynb 40
 #| export
```

### Comparing `pcts-0.0.1/pcts.egg-info/PKG-INFO` & `pcts-0.0.2/pcts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pcts
-Version: 0.0.1
+Version: 0.0.2
 Summary: util torch
 Home-page: https://github.com/dsm-72/pcts
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: utility for pytorch torch util pcts
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pcts-0.0.1/settings.ini` & `pcts-0.0.2/settings.ini`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = pcts
 lib_name = pcts
-version = 0.0.1
+version = 0.0.2
 min_python = 3.11
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = pcts
 nbs_path = nbs
 recursive = True
```

### Comparing `pcts-0.0.1/setup.py` & `pcts-0.0.2/setup.py`

 * *Files identical despite different names*

