# Comparing `tmp/classixclustering-1.2.4.tar.gz` & `tmp/classixclustering-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "classixclustering-1.2.4.tar", last modified: Tue Jan 16 18:04:44 2024, max compression
+gzip compressed data, was "classixclustering-1.2.5.tar", last modified: Sat Apr  6 18:44:54 2024, max compression
```

## Comparing `classixclustering-1.2.4.tar` & `classixclustering-1.2.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0 chenxinye  (1000) chenxinye  (1000)        0 2024-01-16 18:04:44.380893 classixclustering-1.2.4/
--rwxrwxrwx   0 chenxinye  (1000) chenxinye  (1000)     1104 2024-01-16 17:55:12.000000 classixclustering-1.2.4/LICENSE
--rwxrwxrwx   0 chenxinye  (1000) chenxinye  (1000)     3858 2024-01-16 18:04:44.376577 classixclustering-1.2.4/PKG-INFO
--rwxrwxrwx   0 chenxinye  (1000) chenxinye  (1000)     3137 2024-01-16 17:55:12.000000 classixclustering-1.2.4/README.rst
-drwxrwxrwx   0 chenxinye  (1000) chenxinye  (1000)        0 2024-01-16 18:04:44.273043 classixclustering-1.2.4/classix/
--rwxrwxrwx   0 chenxinye  (1000) chenxinye  (1000)      359 2024-01-16 18:03:46.000000 classixclustering-1.2.4/classix/__init__.py
--rwxrwxrwx   0 chenxinye  (1000) chenxinye  (1000)     6169 2024-01-16 17:55:12.000000 classixclustering-1.2.4/classix/aggregate.py
--rwxrwxrwx   0 chenxinye  (1000) chenxinye  (1000)     7555 2024-01-16 17:55:12.000000 classixclustering-1.2.4/classix/aggregate_c.pyx
--rwxrwxrwx   0 chenxinye  (1000) chenxinye  (1000)     6886 2024-01-16 17:55:12.000000 classixclustering-1.2.4/classix/aggregate_cm.pyx
--rwxrwxrwx   0 chenxinye  (1000) chenxinye  (1000)   104012 2024-01-16 17:55:12.000000 classixclustering-1.2.4/classix/clustering.py
--rwxrwxrwx   0 chenxinye  (1000) chenxinye  (1000)    14075 2024-01-16 17:55:13.000000 classixclustering-1.2.4/classix/merge.py
--rwxrwxrwx   0 chenxinye  (1000) chenxinye  (1000)    16556 2024-01-16 17:55:13.000000 classixclustering-1.2.4/classix/merge_cm.pyx
--rwxrwxrwx   0 chenxinye  (1000) chenxinye  (1000)    16651 2024-01-16 17:55:13.000000 classixclustering-1.2.4/classix/merge_cm_win.pyx
-drwxrwxrwx   0 chenxinye  (1000) chenxinye  (1000)        0 2024-01-16 18:04:44.361593 classixclustering-1.2.4/classixclustering.egg-info/
--rwxrwxrwx   0 chenxinye  (1000) chenxinye  (1000)     3858 2024-01-16 18:04:43.000000 classixclustering-1.2.4/classixclustering.egg-info/PKG-INFO
--rwxrwxrwx   0 chenxinye  (1000) chenxinye  (1000)      406 2024-01-16 18:04:44.000000 classixclustering-1.2.4/classixclustering.egg-info/SOURCES.txt
--rwxrwxrwx   0 chenxinye  (1000) chenxinye  (1000)        1 2024-01-16 18:04:43.000000 classixclustering-1.2.4/classixclustering.egg-info/dependency_links.txt
--rwxrwxrwx   0 chenxinye  (1000) chenxinye  (1000)       72 2024-01-16 18:04:43.000000 classixclustering-1.2.4/classixclustering.egg-info/requires.txt
--rwxrwxrwx   0 chenxinye  (1000) chenxinye  (1000)        8 2024-01-16 18:04:43.000000 classixclustering-1.2.4/classixclustering.egg-info/top_level.txt
--rwxrwxrwx   0 chenxinye  (1000) chenxinye  (1000)       38 2024-01-16 18:04:44.380893 classixclustering-1.2.4/setup.cfg
--rwxrwxrwx   0 chenxinye  (1000) chenxinye  (1000)     3623 2024-01-16 18:01:50.000000 classixclustering-1.2.4/setup.py
+drwxr-xr-x   0 xinyechen  (1007) xinyechen  (1007)        0 2024-04-06 18:44:54.245038 classixclustering-1.2.5/
+-rw-r--r--   0 xinyechen  (1007) xinyechen  (1007)     1104 2024-04-06 18:44:21.000000 classixclustering-1.2.5/LICENSE
+-rw-r--r--   0 xinyechen  (1007) xinyechen  (1007)     3858 2024-04-06 18:44:54.245038 classixclustering-1.2.5/PKG-INFO
+-rw-r--r--   0 xinyechen  (1007) xinyechen  (1007)     3137 2024-04-06 18:44:21.000000 classixclustering-1.2.5/README.rst
+drwxr-xr-x   0 xinyechen  (1007) xinyechen  (1007)        0 2024-04-06 18:44:54.245038 classixclustering-1.2.5/classix/
+-rw-r--r--   0 xinyechen  (1007) xinyechen  (1007)      359 2024-04-06 18:44:21.000000 classixclustering-1.2.5/classix/__init__.py
+-rw-r--r--   0 xinyechen  (1007) xinyechen  (1007)     9040 2024-04-06 18:44:21.000000 classixclustering-1.2.5/classix/aggregate.py
+-rw-r--r--   0 xinyechen  (1007) xinyechen  (1007)    11006 2024-04-06 18:44:21.000000 classixclustering-1.2.5/classix/aggregate_c.pyx
+-rw-r--r--   0 xinyechen  (1007) xinyechen  (1007)    10148 2024-04-06 18:44:21.000000 classixclustering-1.2.5/classix/aggregate_cm.pyx
+-rw-r--r--   0 xinyechen  (1007) xinyechen  (1007)   104309 2024-04-06 18:44:21.000000 classixclustering-1.2.5/classix/clustering.py
+-rw-r--r--   0 xinyechen  (1007) xinyechen  (1007)    14075 2024-04-06 18:44:22.000000 classixclustering-1.2.5/classix/merge.py
+-rw-r--r--   0 xinyechen  (1007) xinyechen  (1007)    16556 2024-04-06 18:44:22.000000 classixclustering-1.2.5/classix/merge_cm.pyx
+-rw-r--r--   0 xinyechen  (1007) xinyechen  (1007)    16651 2024-04-06 18:44:22.000000 classixclustering-1.2.5/classix/merge_cm_win.pyx
+drwxr-xr-x   0 xinyechen  (1007) xinyechen  (1007)        0 2024-04-06 18:44:54.245038 classixclustering-1.2.5/classixclustering.egg-info/
+-rw-r--r--   0 xinyechen  (1007) xinyechen  (1007)     3858 2024-04-06 18:44:54.000000 classixclustering-1.2.5/classixclustering.egg-info/PKG-INFO
+-rw-r--r--   0 xinyechen  (1007) xinyechen  (1007)      406 2024-04-06 18:44:54.000000 classixclustering-1.2.5/classixclustering.egg-info/SOURCES.txt
+-rw-r--r--   0 xinyechen  (1007) xinyechen  (1007)        1 2024-04-06 18:44:54.000000 classixclustering-1.2.5/classixclustering.egg-info/dependency_links.txt
+-rw-r--r--   0 xinyechen  (1007) xinyechen  (1007)       72 2024-04-06 18:44:54.000000 classixclustering-1.2.5/classixclustering.egg-info/requires.txt
+-rw-r--r--   0 xinyechen  (1007) xinyechen  (1007)        8 2024-04-06 18:44:54.000000 classixclustering-1.2.5/classixclustering.egg-info/top_level.txt
+-rw-r--r--   0 xinyechen  (1007) xinyechen  (1007)       38 2024-04-06 18:44:54.245038 classixclustering-1.2.5/setup.cfg
+-rw-r--r--   0 xinyechen  (1007) xinyechen  (1007)     3623 2024-04-06 18:44:23.000000 classixclustering-1.2.5/setup.py
```

### Comparing `classixclustering-1.2.4/LICENSE` & `classixclustering-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `classixclustering-1.2.4/PKG-INFO` & `classixclustering-1.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: classixclustering
-Version: 1.2.4
+Version: 1.2.5
 Summary: Fast and explainable clustering based on sorting
 Home-page: https://github.com/nla-group/CLASSIX.git
 Author: Xinye Chen, Stefan Güttel
 Author-email: xinye.chen@manchester.ac.uk, stefan.guettel@manchester.ac.uk
 License: MIT License
 Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
```

### Comparing `classixclustering-1.2.4/README.rst` & `classixclustering-1.2.5/README.rst`

 * *Files identical despite different names*

### Comparing `classixclustering-1.2.4/classix/aggregate.py` & `classixclustering-1.2.5/classix/aggregate.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 #
 # CLASSIX: Fast and explainable clustering based on sorting
 #
 # MIT License
 #
-# Copyright (c) 2023 Stefan Güttel, Xinye Chen
+# Copyright (c) 2024 Stefan Güttel, Xinye Chen
 
 
 # Python implementation for aggregation
 
 
 import numpy as np
 from scipy.sparse.linalg import svds
@@ -219,7 +219,111 @@
 
         splist.append((i, num_group))  
         lab += 1
 
     return labels, splist, nr_dist, ind, sort_vals, data, half_nrm2
 
 
+
+
+
+def lm_aggregate(data, sorting="pca", tol=0.5): 
+    """Aggregate the data in low memory need (Linux)
+
+    Parameters
+    ----------
+    data : numpy.ndarray
+        The input that is array-like of shape (n_samples,).
+
+    sorting : str
+        The sorting method for aggregation, default='pca', other options: 'norm-mean', 'norm-orthant'.
+
+    tol : float
+        The tolerance to control the aggregation. if the distance between the starting point 
+        of a group and another data point is less than or equal to the tolerance,
+        the point is allocated to that group.  
+
+    Returns
+    -------
+    labels (list) : 
+        The group categories of the data after aggregation.
+    
+    splist (list) : 
+        The list of the starting points.
+    
+    nr_dist (int) :
+        The number of pairwise distance calculations.
+
+    ind (numpy.ndarray):
+        Array storing Sorting indices.
+
+    sort_vals (numpy.ndarray):
+        Sorting values.
+    
+    data (numpy.ndarray):
+        Sorted data.
+    
+    """
+
+    splist = list() # store the starting points
+    len_ind = data.shape[0]
+    fdim = data.shape[1]
+    
+    if sorting == "norm-mean" or sorting == "norm-orthant": 
+        sort_vals = np.linalg.norm(data, ord=2, axis=1)
+        
+    elif sorting == "pca":
+        # change to svd 
+        if fdim > 1:
+            if fdim <= 3: # memory inefficient
+                gemm = get_blas_funcs("gemm", [data.T, data])
+                _, U1 = eigh(gemm(1, data.T, data), subset_by_index=[fdim-1, fdim-1])
+                sort_vals = data@U1.reshape(-1)
+            else:
+                U1, s1, _ = svds(data, k=1, return_singular_vectors=True)
+                sort_vals = U1[:,0]*s1[0]
+
+        else:
+            sort_vals = data[:,0]
+            
+        sort_vals = sort_vals*np.sign(-sort_vals[0]) # flip to enforce deterministic output
+        
+
+    else: # no sorting
+        sort_vals = np.zeros(len_ind) 
+
+    ind = np.argsort(sort_vals)
+    data = data[ind]
+    sort_vals = sort_vals[ind]
+
+    lab = 0
+    labels = [-1]*len_ind
+    nr_dist = 0 
+    
+    for i in range(len_ind): 
+        if labels[i] >= 0:
+            continue
+        else:
+            clustc = data[i,:] 
+            labels[i] = lab
+            num_group = 1
+
+        for j in range(i+1, len_ind):
+            if labels[j] >= 0:
+                continue
+
+            if (sort_vals[j] - sort_vals[i] > tol):
+                break       
+
+            dat = clustc - data[j,:]
+            dist = np.inner(dat, dat)
+            nr_dist += 1
+                
+            if dist <= tol**2:
+                num_group += 1
+                labels[j] = lab
+
+        splist.append((i, num_group))  
+
+        lab += 1
+
+    return labels, splist, nr_dist, ind, sort_vals, data, None
```

### Comparing `classixclustering-1.2.4/classix/aggregate_c.pyx` & `classixclustering-1.2.5/classix/aggregate_c.pyx`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 #
 # CLASSIX: Fast and explainable clustering based on sorting
 #
 # MIT License
 #
-# Copyright (c) 2023 Stefan Guettel, Xinye Chen
+# Copyright (c) 2024 Stefan Guettel, Xinye Chen
 
 
 #!python
 #cython: language_level=3
 #cython: profile=True
 #cython: linetrace=True
 
@@ -249,7 +249,120 @@
 
         splist.append((i, num_group)) 
 
         lab += 1
 
     return labels, splist, nr_dist, ind, sort_vals, data, half_nrm2
 
+
+
+
+cpdef lm_aggregate(np.ndarray[np.float64_t, ndim=2] data, str sorting="pca", float tol=0.5):
+    """Aggregate the data in low memory need (Linux)
+
+    Parameters
+    ----------
+    data : numpy.ndarray
+        The input that is array-like of shape (n_samples,).
+
+    sorting : str
+        The sorting method for aggregation, default='pca', other options: 'norm-mean', 'norm-orthant'.
+
+    tol : float
+        The tolerance to control the aggregation. if the distance between the starting point 
+        of a group and another data point is less than or equal to the tolerance,
+        the point is allocated to that group.  
+
+    Returns
+    -------
+    labels (list) : 
+        The group categories of the data after aggregation.
+    
+    splist (list) : 
+        The list of the starting points.
+    
+    nr_dist (int) :
+        The number of pairwise distance calculations.
+
+    ind (numpy.ndarray):
+        Array storing Sorting indices.
+
+    sort_vals (numpy.ndarray):
+        Sorting values.
+    
+    data (numpy.ndarray):
+        Sorted data.
+
+    """
+    
+    cdef int num_group
+    cdef Py_ssize_t fdim = data.shape[1] # feature dimension
+    cdef Py_ssize_t len_ind = data.shape[0] # size of data
+    cdef np.ndarray[np.float64_t, ndim=2] U1
+    cdef int nr_dist = 0 # nr_dist:if necessary, count the distance computation
+    cdef int lab = 0 # lab: class
+    cdef double dist # distance 
+    cdef list labels = [-1]*len_ind
+    cdef list splist = list() # store the starting points
+    cdef np.ndarray[np.float64_t, ndim=1] sort_vals
+    cdef np.ndarray[np.float64_t, ndim=1] clustc
+    cdef np.ndarray[np.int64_t, ndim=1] ind
+    cdef Py_ssize_t i, j, coord
+    
+    
+    if sorting == "norm-mean" or sorting == "norm-orthant": 
+        sort_vals = np.linalg.norm(data, ord=2, axis=1)
+        ind = np.argsort(sort_vals)
+
+    elif sorting == "pca":
+        if fdim > 1:
+            if fdim <= 3: # memory inefficient
+                gemm = get_blas_funcs("gemm", [data.T, data])
+                _, U1 = eigh(gemm(1, data.T, data), subset_by_index=[fdim-1, fdim-1])
+                sort_vals = data@U1.reshape(-1)
+            else:
+                U1, s1, _ = svds(data, k=1, return_singular_vectors=True)
+                sort_vals = U1[:,0]*s1[0]
+
+        else:
+            sort_vals = data[:,0]
+            
+        sort_vals = sort_vals*np.sign(-sort_vals[0]) # flip to enforce deterministic output
+        
+
+    else: # no sorting
+        sort_vals = np.zeros(len_ind)
+    
+    ind = np.argsort(sort_vals)
+    data = data[ind]
+    sort_vals = sort_vals[ind] 
+    
+    for i in range(len_ind):
+
+        if labels[i] >= 0:
+            continue
+        
+        clustc = data[i,:] 
+        labels[i] = lab
+        num_group = 1
+
+        for j in range(i+1, len_ind):
+            if labels[j] >= 0:
+                continue
+            
+            if sort_vals[j] - sort_vals[i] > tol:
+                break       
+            
+            dist = 0
+            for coord in range(fdim):
+                dist += (clustc[coord] - data[j,coord])**2
+            
+            nr_dist += 1
+            
+            if dist <= tol**2:
+                num_group = num_group + 1
+                labels[j] = lab
+
+        splist.append((i, num_group)) 
+        lab += 1
+
+    return labels, splist, nr_dist, ind, sort_vals, data, None
```

### Comparing `classixclustering-1.2.4/classix/aggregate_cm.pyx` & `classixclustering-1.2.5/classix/aggregate_cm.pyx`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 #
 # CLASSIX: Fast and explainable clustering based on sorting
 #
 # MIT License
 #
-# Copyright (c) 2023 Stefan Güttel, Xinye Chen
+# Copyright (c) 2024 Stefan Güttel, Xinye Chen
 
 # Cython implementation for aggregation
 
 
 cimport cython
 import numpy as np
 cimport numpy as np 
@@ -234,7 +234,112 @@
         # list of [ starting point index of current group, sorting key, and number of group elements ]
 
         lab += 1
   
     return labels, splist, nr_dist, np.asarray(ind), np.asarray(sort_vals), np.asarray(data), np.asarray(half_nrm2)
 
 
+
+
+cpdef lm_aggregate(double[:,:] data, str sorting, double tol=0.5):
+    """Aggregate the data in low memory need (Linux)
+    
+    Parameters
+    ----------
+    data : numpy.ndarray
+        The input that is array-like of shape (n_samples,).
+    
+    sorting : str
+        The sorting way referred for aggregation, default='pca', other options: 'norm-mean', 'norm-orthant'.
+    
+    tol : float
+        The tolerance to control the aggregation, if the distance between the starting point 
+        and the object is less than or equal than the tolerance,
+        the object should allocated to the group which starting point belongs to.  
+    
+    
+    Returns
+    -------
+    labels (list) : 
+        The group categories of the data after aggregation.
+    
+    splist (list) : 
+        The list of the starting points.
+    
+    nr_dist (int) :
+        The number of pairwise distance calculations.
+
+    ind (numpy.ndarray):
+        Array storing Sorting indices.
+
+    sort_vals (numpy.ndarray):
+        Sorting values.
+    
+    data (numpy.ndarray):
+        Sorted data.
+    
+    """
+
+    cdef Py_ssize_t fdim = data.shape[1] # feature dimension
+    cdef Py_ssize_t len_ind = data.shape[0] # size of data
+    cdef double[:] sort_vals
+    cdef double[:, :] U1, _  # = np.empty((len_ind, ), dtype=float)
+    cdef long long[:] ind # = np.empty((len_ind, ), dtype=int)
+    cdef unsigned int lab=0, nr_dist=0, num_group
+    cdef double[:] clustc # starting point coordinates
+    cdef double dist
+    cdef list labels = [-1]*len_ind
+    cdef list splist = list() # list of starting points
+    cdef Py_ssize_t i, j, coord
+    
+    
+    if sorting == "norm-mean" or sorting == "norm-orthant":
+        sort_vals = np.linalg.norm(data, ord=2, axis=1)
+    
+    elif sorting == "pca":
+        if fdim > 1:
+            U1, s1, _ = svds(np.asarray(data), k=1, return_singular_vectors=True)
+            sort_vals = U1[:,0]*s1[0]
+        else:
+            sort_vals = data[:,0]
+            
+        sort_vals = sort_vals*np.sign(-sort_vals[0]) # flip to enforce deterministic output
+    
+    else: # no sorting
+        sort_vals = np.zeros(len_ind)
+
+    ind = np.argsort(sort_vals)
+    data = data.base[ind]
+    sort_vals = sort_vals.base[ind] 
+
+    for i in range(len_ind): 
+        if labels[i] >= 0:
+            continue
+        
+        clustc = data[i,:] 
+        labels[i] = lab
+        num_group = 1
+            
+        for j in range(i+1, len_ind): 
+                    
+            if labels[j] >= 0:
+                continue
+                
+            if sort_vals[j] - sort_vals[i] > tol:
+                break       
+            
+            dist = 0
+            for coord in range(fdim):
+                dist += (clustc[coord] - data[j,coord])**2
+            
+            nr_dist += 1
+            
+            if dist <= tol**2:
+                num_group += 1
+                labels[j] = lab
+
+        splist.append((i, num_group))  
+        # list of [ starting point index of current group, sorting key, and number of group elements ]
+
+        lab += 1
+  
+    return labels, splist, nr_dist, np.asarray(ind), np.asarray(sort_vals), np.asarray(data), None
```

### Comparing `classixclustering-1.2.4/classix/clustering.py` & `classixclustering-1.2.5/classix/clustering.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 #
 # CLASSIX: Fast and explainable clustering based on sorting
 #
 # MIT License
 #
-# Copyright (c) 2023 Stefan Güttel, Xinye Chen
+# Copyright (c) 2024 Stefan Güttel, Xinye Chen
 
 
 import warnings
 
 import os
 import copy
 import numbers
@@ -449,50 +449,53 @@
         if self.__verbose:
             print(self)
         
 
         from . import __enable_cython__
         self.__enable_cython__ = __enable_cython__
         self.__enable_aggregate_cython__ = False
+        import platform
         
         if self.__enable_cython__:
             try:
                 try:
-                    from .aggregate_cm import general_aggregate, pca_aggregate
+                    from .aggregate_cm import general_aggregate, pca_aggregate, lm_aggregate
                     
                 except ModuleNotFoundError:
-                    from .aggregate_c import general_aggregate, pca_aggregate
+                    from .aggregate_c import general_aggregate, pca_aggregate, lm_aggregate
                 
                 self.__enable_aggregate_cython__ = True
 
-                import platform
+                
                 
                 if platform.system() == 'Windows':
                     from .merge_cm_win import density_merge, distance_merge, distance_merge_mtg
                 else:
                     from .merge_cm import density_merge, distance_merge, distance_merge_mtg
 
             except (ModuleNotFoundError, ValueError):
                 if not self.__enable_aggregate_cython__:
-                    from .aggregate import general_aggregate, pca_aggregate
+                    from .aggregate import general_aggregate, pca_aggregate, lm_aggregate
                 
                 from .merge import density_merge, distance_merge, distance_merge_mtg
                 warnings.warn("This CLASSIX installation is not using Cython.")
 
         else:
-            from .aggregate import general_aggregate, pca_aggregate
+            from .aggregate import general_aggregate, pca_aggregate, lm_aggregate
             from .merge import density_merge, distance_merge, distance_merge_mtg
             warnings.warn("This run of CLASSIX is not using Cython.")
 
-
-        if sorting == 'pca':
-            self._aggregate = pca_aggregate
+        
+        if platform.system() == 'Windows':
+            if sorting == 'pca':
+                self._aggregate = pca_aggregate
+            else:
+                self._aggregate = general_aggregate
         else:
-            self._aggregate = general_aggregate
-            
+            self._aggregate = lm_aggregate
 
         self._density_merge = density_merge
         
         if self.__mergeTinyGroups:
             self._distance_merge = distance_merge
         else:
             self._distance_merge = distance_merge_mtg
@@ -546,24 +549,25 @@
             self.data = self.data / self.dataScale_
             
         else:
             self.mu_, self.dataScale_ = 0, 1 # no preprocessing
             self.data = (data - self.mu_) / self.dataScale_
         
         self.t1_prepare = time() - self.t1_prepare
-
         self.t2_aggregate = time()
         # aggregation
         
         self.groups_, self.splist_, self.nrDistComp_, self.ind, sort_vals, self.data, self.__half_nrm2 = self._aggregate(
                                                                                 data=self.data,
                                                                                 sorting=self.sorting, 
                                                                                 tol=self.radius
                                                                             ) 
             
+        if self.__half_nrm2 is None:
+            self.__half_nrm2 = np.einsum('ij,ij->i', self.data, self.data) * 0.5
             
         self.splist_ = np.array(self.splist_)
         self.t2_aggregate = time() - self.t2_aggregate
 
         self.t3_merge = time()
         if self.group_merging is None:
             self.inverse_ind = np.argsort(self.ind)
```

### Comparing `classixclustering-1.2.4/classix/merge.py` & `classixclustering-1.2.5/classix/merge.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 #
 # CLASSIX: Fast and explainable clustering based on sorting
 #
 # MIT License
 #
-# Copyright (c) 2023 Stefan Güttel, Xinye Chen
+# Copyright (c) 2024 Stefan Güttel, Xinye Chen
 
 # Python implementation for group merging
 
 import collections
 import numpy as np
 from scipy.special import betainc, gamma
```

### Comparing `classixclustering-1.2.4/classix/merge_cm.pyx` & `classixclustering-1.2.5/classix/merge_cm.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 #
 # CLASSIX: Fast and explainable clustering based on sorting
 #
 # MIT License
 #
-# Copyright (c) 2023 Stefan Güttel, Xinye Chen
+# Copyright (c) 2024 Stefan Güttel, Xinye Chen
 
 # Cython implementation for group merging
 
 #!python
 #cython: language_level=3
 #cython: profile=True
 #cython: linetrace=True
```

### Comparing `classixclustering-1.2.4/classix/merge_cm_win.pyx` & `classixclustering-1.2.5/classix/merge_cm_win.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 #
 # CLASSIX: Fast and explainable clustering based on sorting
 #
 # MIT License
 #
-# Copyright (c) 2023 Stefan Güttel, Xinye Chen
+# Copyright (c) 2024 Stefan Güttel, Xinye Chen
 #
 # Cython implementation for group merging
 
 #!python
 #cython: language_level=3
 #cython: profile=True
 #cython: linetrace=True
```

### Comparing `classixclustering-1.2.4/classixclustering.egg-info/PKG-INFO` & `classixclustering-1.2.5/classixclustering.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: classixclustering
-Version: 1.2.4
+Version: 1.2.5
 Summary: Fast and explainable clustering based on sorting
 Home-page: https://github.com/nla-group/CLASSIX.git
 Author: Xinye Chen, Stefan Güttel
 Author-email: xinye.chen@manchester.ac.uk, stefan.guettel@manchester.ac.uk
 License: MIT License
 Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
```

### Comparing `classixclustering-1.2.4/setup.py` & `classixclustering-1.2.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 try:
     from Cython.Distutils import build_ext
 except ImportError as e:
     warnings.warn(e.args[0])
     from setuptools.command.build_ext import build_ext
     
-_version="1.2.4"
+_version="1.2.5"
 logging.basicConfig()
 log = logging.getLogger(__file__)
 
 ext_errors = (CCompilerError, ModuleNotFoundError, DistutilsExecError, DistutilsPlatformError, IOError, SystemExit)
 
 with open("README.rst", 'r') as f:
     long_description = f.read()
```

